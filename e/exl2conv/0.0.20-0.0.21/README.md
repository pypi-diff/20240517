# Comparing `tmp/exl2conv-0.0.20.tar.gz` & `tmp/exl2conv-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exl2conv-0.0.20.tar", last modified: Mon Apr 29 15:19:05 2024, max compression
+gzip compressed data, was "exl2conv-0.0.21.tar", last modified: Fri May 17 02:42:16 2024, max compression
```

## Comparing `exl2conv-0.0.20.tar` & `exl2conv-0.0.21.tar`

### file list

```diff
@@ -1,186 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.039785 exl2conv-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-29 15:18:33.000000 exl2conv-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 15:18:33.000000 exl2conv-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 15:19:05.039785 exl2conv-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-29 15:18:33.000000 exl2conv-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.023785 exl2conv-0.0.20/exl2conv/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18758 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/architecture.py
--rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/attn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.027785 exl2conv-0.0.20/exl2conv/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)    22378 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/adaptivegptq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    24398 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/qparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/quantize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.027785 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/
--rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/c4.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/code.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/multilingual.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/technical.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/tiny.utf8
--rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/wiki.utf8
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.031785 exl2conv-0.0.20/exl2conv/exl2conv_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.031785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx2_target.h
--rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/profiling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/profiling.h
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/compat.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_add.cu
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_add.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/head_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/head_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/layer_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/lora.cu
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/lora.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    21853 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rms_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cu
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_gemm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_gemm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_hadamard.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_hadamard.h
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.h
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_rope.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_rope.h
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/fasttensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/generator/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/ngram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33700 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/hadamard/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_100.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_116.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_156.txt
--rw-r--r--   0 runner    (1001) docker     (127)    29755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_172.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35531 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_188.txt
--rw-r--r--   0 runner    (1001) docker     (127)    55931 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_236.txt
--rw-r--r--   0 runner    (1001) docker     (127)    59779 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_244.txt
--rw-r--r--   0 runner    (1001) docker     (127)   183612 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_428.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_52.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_92.txt
--rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/primes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/headnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29232 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/model_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/moe_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/parallel_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/rmsnorm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/server/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/server/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/server/websocket_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.039785 exl2conv-0.0.20/exl2conv/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/spm.py
--rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.027785 exl2conv-0.0.20/exl2conv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:19:05.039785 exl2conv-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-29 15:18:33.000000 exl2conv-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.297567 exl2conv-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-17 02:41:38.000000 exl2conv-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 02:41:38.000000 exl2conv-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 02:42:16.297567 exl2conv-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-17 02:41:38.000000 exl2conv-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.285567 exl2conv-0.0.21/exl2conv/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23880 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35438 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12383 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.285567 exl2conv-0.0.21/exl2conv/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    22378 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/adaptivegptq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24619 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/qparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18989 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/quantize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.285567 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/c4.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/code.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/multilingual.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/technical.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/tiny.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/wiki.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/conversion/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.289567 exl2conv-0.0.21/exl2conv/exl2conv_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.289567 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/avx2_target.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/generator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/profiling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/profiling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/quantize_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.293567 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/cache.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/cache.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.293567 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/compat.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_add.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_add.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/head_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/head_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/layer_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/lora.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/lora.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_attn.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_attn.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    21853 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_matrix.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.293567 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quantize.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quantize.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rms_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rope.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rope.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/util.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_hadamard.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_hadamard.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_norm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qattn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qattn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmlp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmlp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_quant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_quant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_rope.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_rope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/fasttensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.293567 exl2conv-0.0.21/exl2conv/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.293567 exl2conv-0.0.21/exl2conv/generator/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/filters/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/filters/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/ngram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41208 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/generator/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.297567 exl2conv-0.0.21/exl2conv/hadamard/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_100.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_116.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_156.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29755 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_172.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35531 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_188.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55931 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_236.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    59779 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_244.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   183612 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_428.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_52.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/hadamard_92.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/hadamard/primes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/headnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30036 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/model_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/moe_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/parallel_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/pos_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.297567 exl2conv-0.0.21/exl2conv/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/server/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/server/websocket_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.297567 exl2conv-0.0.21/exl2conv/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/tokenizer/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/tokenizer/spm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23840 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/tokenizer/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 02:41:38.000000 exl2conv-0.0.21/exl2conv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:42:16.285567 exl2conv-0.0.21/exl2conv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 02:42:16.000000 exl2conv-0.0.21/exl2conv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-17 02:42:16.000000 exl2conv-0.0.21/exl2conv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 02:42:16.000000 exl2conv-0.0.21/exl2conv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 02:42:16.000000 exl2conv-0.0.21/exl2conv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 02:42:16.000000 exl2conv-0.0.21/exl2conv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 02:42:16.297567 exl2conv-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-17 02:41:38.000000 exl2conv-0.0.21/setup.py
```

### Comparing `exl2conv-0.0.20/LICENSE` & `exl2conv-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/README.md` & `exl2conv-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/architecture.py` & `exl2conv-0.0.21/exl2conv/architecture.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+from enum import Enum
 
 # Common keys
 
 layer_keys_llama_norms = [["input_layernorm"],
                           ["post_attention_layernorm"]]
 layer_keys_cohere_norms = [["input_layernorm"]]
+layer_keys_gpt2_norms = [["ln_1"],
+                         ["ln_2"]]
 layer_keys_yi_norms = [["ln1", "input_layernorm"],
                        ["ln2", "post_attention_layernorm"]]
 layer_keys_llama_attn = [["self_attn.q_proj"],
                          ["self_attn.k_proj"],
                          ["self_attn.v_proj"],
                          ["self_attn.o_proj"]]
+layer_keys_gpt2_attn = [["self_attn.c_attn", "self_attn.q_proj"],
+                        ["self_attn.c_attn", "self_attn.k_proj"],
+                        ["self_attn.c_attn", "self_attn.v_proj"],
+                        ["self_attn.o_proj"]]
 layer_keys_dbrx_attn = [["self_attn.Wqkv", "self_attn.q_proj"],
                         ["self_attn.Wqkv", "self_attn.k_proj"],
                         ["self_attn.Wqkv", "self_attn.v_proj"],
                         ["self_attn.o_proj"]]
 layer_keys_phi3_attn = [["self_attn.qkv_proj", "self_attn.q_proj"],
                         ["self_attn.qkv_proj", "self_attn.k_proj"],
                         ["self_attn.qkv_proj", "self_attn.v_proj"],
@@ -32,46 +39,69 @@
                        ["block_sparse_moe.experts.*.w1", "block_sparse_moe.experts.w1"],
                        ["block_sparse_moe.experts.*.w2", "block_sparse_moe.experts.w2"],
                        ["block_sparse_moe.gate"]]
 layer_keys_llama_mlp_swiglu = [["mlp.swiglu.w12"],
                                ["mlp.swiglu.w3"]]
 layer_keys_starcoder2_mlp = [["mlp.c_fc"],
                              ["mlp.c_proj"]]
+layer_keys_gpt2_mlp = [["mlp.c_fc"],
+                       ["mlp.c_proj"]]
 expect_keys_llama = [["lm_head"],
                      ["model.norm"],
                      ["model.embed_tokens"]]
 expect_keys_gemma = [["model.norm"],
                      ["model.embed_tokens"]]
 expect_keys_starcoder2 = [["model.norm"],
                           ["model.embed_tokens"]]
+expect_keys_gpt2 = [["model.embed_tokens"]]
 
 dbrx_keymap = [("transformer.", "model."),
                (".blocks.", ".layers."),
                (".ffn.experts.mlp.", ".block_sparse_moe.experts."),
                (".ffn.router.layer.", ".block_sparse_moe.gate."),
                (".norm_attn_norm.norm_1.", ".input_layernorm."),
                (".norm_attn_norm.norm_2.", ".post_attention_layernorm."),
                (".norm_attn_norm.attn.", ".self_attn."),
                (".out_proj.", ".o_proj."),
                (".norm_f.", ".norm."),
                (".wte.", ".embed_tokens.")]
-
+bigcode_keymap = [("transformer.ln_f", "model.norm"),
+                  ("transformer.", "model."),
+                  (".attn.c_proj.", ".self_attn.o_proj."),
+                  (".attn.", ".self_attn."),
+                  (".h.", ".layers."),
+                  (".wte.", ".embed_tokens.")]
+gpt2_keymap = [("$ln_f.", "model.norm."),
+               (".attn.c_proj.", ".self_attn.o_proj."),
+               (".attn.", ".self_attn."),
+               ("$h.", "model.layers."),
+               ("$wte.", "model.embed_tokens."),
+               ("$wpe.", "model.wpe.")]
+
+class RopeStyle(Enum):
+    NONE = 0
+    GPTJ = 1
+    NEOX = 2
 
 class ExLlamaV2ArchParams:
 
     def __init__(self, arch_string, read_config):
 
         self.arch_string = arch_string
         arch_recognized = False
 
         self.expect_keys = []  # Keys to expect in model dict
         self.layer_keys = []  # Keys to expect in model dict, per layer
 
         self.fused_mlp_key_12 = None
         self.fused_mlp_key_3 = None
+        self.learned_pos_emb_key = None
+
+        self.default_inner_dim_mult = None
+        self.orig_weights_transposed = False
 
         # Mistral
 
         if arch_string == "MistralForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
@@ -93,17 +123,19 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Mixtral
 
         if arch_string == "MixtralForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
@@ -126,17 +158,19 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Yi
 
         if arch_string == "YiForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_yi_norms + \
@@ -158,17 +192,19 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".ln1"
             self.norm_key_2 = ".ln2"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Orion
 
         if arch_string == "OrionForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
@@ -190,17 +226,19 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Qwen2 (1.5)
 
         if arch_string == "Qwen2ForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
@@ -222,17 +260,19 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Gemma
 
         if arch_string == "GemmaForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
@@ -254,17 +294,19 @@
             self.lm_head_key = "model.embed_tokens"
             self.normalize_embeddings = True
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 1
             self.parallel_decoder_blocks = False
             self.requires_bos = True
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # StarCoder2
 
         if arch_string == "Starcoder2ForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
@@ -285,17 +327,19 @@
             self.lm_head_key = "model.embed_tokens"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # GemMoE
 
         if arch_string == "GemmoeForCausalLM":
             arch_recognized = True
             print(f" !! Warning, Gemmoe support is experimental and has not been fully tested")
             self.layer_keys += \
@@ -319,17 +363,19 @@
             self.lm_head_key = "model.embed_tokens"
             self.normalize_embeddings = True
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 1
             self.parallel_decoder_blocks = False
             self.requires_bos = True
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Cohere
 
         if arch_string == "CohereForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_cohere_norms + \
@@ -351,17 +397,19 @@
             self.lm_head_key = "model.embed_tokens"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = None
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = True
             self.requires_bos = True
-            self.rope_neox_style = False
+            self.rope_style = RopeStyle.GPTJ
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # DBRX
 
         if arch_string == "DbrxForCausalLM":
             arch_recognized = True
             self.keymap = dbrx_keymap
             self.layer_keys += \
@@ -385,19 +433,21 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = dbrx_keymap
             self.fused_qkv_key = "Wqkv"
+            self.mqa = False
+            self.scale_attn_weights = False
 
-        # Llama (default + fallback)
+        # Phi3
 
         if arch_string == "Phi3ForCausalLM":
             arch_recognized = True
             self.layer_keys += \
                 layer_keys_llama_norms + \
                 layer_keys_phi3_attn + \
                 layer_keys_phi3_mlp
@@ -417,18 +467,92 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = "qkv_proj"
             self.fused_mlp_key_12 = "gate_up_proj"
+            self.mqa = False
+            self.scale_attn_weights = False
+
+        # GPTBigCode
+
+        if arch_string == "GPTBigCodeForCausalLM":
+            arch_recognized = True
+            self.layer_keys += \
+                layer_keys_gpt2_norms + \
+                layer_keys_gpt2_attn + \
+                layer_keys_gpt2_mlp
+            self.expect_keys += \
+                expect_keys_gpt2
+            self.norm_eps_key = "layer_norm_epsilon"
+            self.attention_bias_qkv = True
+            self.attention_bias_o = True
+            self.mlp_bias = True
+            self.mlp_gate = False
+            self.mlp_key_gate = None
+            self.mlp_key_up = ".mlp.c_fc"
+            self.mlp_key_down = ".mlp.c_proj"
+            self.mlp_act_func = "gelu"
+            self.is_moe = False
+            self.norm = "layernorm"
+            self.lm_head_key = "model.embed_tokens"
+            self.normalize_embeddings = False
+            self.norm_key_1 = ".ln_1"
+            self.norm_key_2 = ".ln_2"
+            self.norm_constant_bias = 0
+            self.parallel_decoder_blocks = False
+            self.requires_bos = False
+            self.rope_style = RopeStyle.NONE
+            self.keymap = gpt2_keymap
+            self.fused_qkv_key = "c_attn"
+            self.mqa = True
+            self.learned_pos_emb_key = "model.wpe"
+            self.scale_attn_weights = True
+
+        # GPT2
+
+        if arch_string == "GPT2LMHeadModel":
+            arch_recognized = True
+            self.layer_keys += \
+                layer_keys_gpt2_norms + \
+                layer_keys_gpt2_attn + \
+                layer_keys_gpt2_mlp
+            self.expect_keys += \
+                expect_keys_gpt2
+            self.norm_eps_key = "layer_norm_epsilon"
+            self.attention_bias_qkv = True
+            self.attention_bias_o = True
+            self.mlp_bias = True
+            self.mlp_gate = False
+            self.mlp_key_gate = None
+            self.mlp_key_up = ".mlp.c_fc"
+            self.mlp_key_down = ".mlp.c_proj"
+            self.mlp_act_func = "gelu"
+            self.is_moe = False
+            self.norm = "layernorm"
+            self.lm_head_key = "model.embed_tokens"
+            self.normalize_embeddings = False
+            self.norm_key_1 = ".ln_1"
+            self.norm_key_2 = ".ln_2"
+            self.norm_constant_bias = 0
+            self.parallel_decoder_blocks = False
+            self.requires_bos = False
+            self.rope_style = RopeStyle.NONE
+            self.keymap = gpt2_keymap
+            self.fused_qkv_key = "c_attn"
+            self.mqa = False
+            self.learned_pos_emb_key = "model.wpe"
+            self.scale_attn_weights = True
+            self.default_inner_dim_mult = 4
+            self.orig_weights_transposed = True
 
         # Llama (default + fallback)
 
         if arch_string != "LlamaForCausalLM" and not arch_recognized:
             print(f" !! Warning, unknown architecture: {arch_string}")
             print(f" !! Loading as LlamaForCausalLM")
             self.arch_string = "LlamaForCausalLM"
@@ -453,24 +577,34 @@
             self.lm_head_key = "lm_head"
             self.normalize_embeddings = False
             self.norm_key_1 = ".input_layernorm"
             self.norm_key_2 = ".post_attention_layernorm"
             self.norm_constant_bias = 0
             self.parallel_decoder_blocks = False
             self.requires_bos = False
-            self.rope_neox_style = True
+            self.rope_style = RopeStyle.NEOX
             self.keymap = None
             self.fused_qkv_key = None
+            self.mqa = False
+            self.scale_attn_weights = False
 
         # Arch overrides
 
         if read_config.get("attention_bias", False):
             self.attention_bias_qkv = True
             self.attention_bias_o = True
 
+        if read_config.get("mlp_bias", False):
+            self.mlp_bias = True
+
+        if read_config.get("tie_word_embeddings", False):
+            if ["lm_head"] in self.expect_keys:
+                self.expect_keys.remove(["lm_head"])
+                self.lm_head_key = "model.embed_tokens"
+
 
     def make_fused_mlp(self):
 
         for x in layer_keys_llama_mlp: self.layer_keys.remove(x)
         self.layer_keys += layer_keys_llama_mlp_swiglu
         self.fused_mlp_key_12 = layer_keys_llama_mlp_swiglu[0][0]
         self.fused_mlp_key_3 = layer_keys_llama_mlp_swiglu[1][0]
```

### Comparing `exl2conv-0.0.20/exl2conv/attn.py` & `exl2conv-0.0.21/exl2conv/attn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
+
 import torch
 from torch import nn
 from exl2conv.module import ExLlamaV2Module
 from exl2conv.rmsnorm import ExLlamaV2RMSNorm
 from exl2conv.layernorm import ExLlamaV2LayerNorm
+from exl2conv.headnorm import ExLlamaV2HeadNorm
 from exl2conv.linear import ExLlamaV2Linear
 from exl2conv.cache import ExLlamaV2CacheBase
 from exl2conv.ext import exl2conv_ext as ext_c, none_tensor
 from exl2conv.compat import safe_move_tensor
 from exl2conv.lora import ExLlamaV2Lora
+from exl2conv.architecture import RopeStyle
 import math
 # import xformers.ops as xops
-# from exl2conv.util import list_live_tensors, set_snapshot, diff_snapshot, print_vram_usage_peak
+# from exllamav2.util import list_live_tensors, set_snapshot, diff_snapshot, print_vram_usage_peak
 # import torch.nn.functional as F
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from exl2conv.model import ExLlamaV2
+    from exllamav2.model import ExLlamaV2
 
 # Detect flash-attn
 
 has_flash_attn = False
 try:
     import flash_attn
     flash_attn_ver = [int(t) for t in flash_attn.__version__.split(".") if t.isdigit()]
@@ -39,14 +42,16 @@
 
     layer_idx: int
     input_layernorm: ExLlamaV2RMSNorm | ExLlamaV2LayerNorm | None
     q_proj: ExLlamaV2Linear | None
     k_proj: ExLlamaV2Linear | None
     v_proj: ExLlamaV2Linear | None
     o_proj: ExLlamaV2Linear | None
+    q_norm: ExLlamaV2HeadNorm | None
+    k_norm: ExLlamaV2HeadNorm | None
 
     q_handle: int | None
 
     temp_state: torch.tensor
     temp_q: torch.tensor
     temp_k: torch.tensor
     temp_v: torch.tensor
@@ -209,38 +214,62 @@
         f_key = (key + ".self_attn." + cfg.arch.fused_qkv_key) if cfg.arch.fused_qkv_key else None
 
         self.q_proj = ExLlamaV2Linear(model, key + ".self_attn.q_proj", hidden_size, cfg.num_attention_heads * cfg.head_dim, cfg.arch.attention_bias_qkv, f_key = f_key, f_beg = f_a, f_end = f_b)
         self.k_proj = ExLlamaV2Linear(model, key + ".self_attn.k_proj", hidden_size, cfg.num_key_value_heads * cfg.head_dim, cfg.arch.attention_bias_qkv, f_key = f_key, f_beg = f_b, f_end = f_c)
         self.v_proj = ExLlamaV2Linear(model, key + ".self_attn.v_proj", hidden_size, cfg.num_key_value_heads * cfg.head_dim, cfg.arch.attention_bias_qkv, f_key = f_key, f_beg = f_c, f_end = f_d)
         self.o_proj = ExLlamaV2Linear(model, key + ".self_attn.o_proj", cfg.num_attention_heads * cfg.head_dim, hidden_size, cfg.arch.attention_bias_o)
 
+        if cfg.use_qk_norm:
+            self.q_norm = ExLlamaV2HeadNorm(model, key + ".self_attn.q_norm", cfg.num_attention_heads, cfg.head_dim)
+            self.k_norm = ExLlamaV2HeadNorm(model, key + ".self_attn.k_norm", cfg.num_key_value_heads, cfg.head_dim)
+        else:
+            self.q_norm = None
+            self.k_norm = None
+
         self.submodules = [self.q_proj,
                            self.k_proj,
                            self.v_proj,
                            self.o_proj]
         if self.has_norm:
             self.submodules += [self.input_layernorm]
+        if cfg.use_qk_norm:
+            self.submodules += [self.q_norm,
+                                self.k_norm]
+
+        # if cfg.arch.scale_attn_weights:
+        #     self.unscale_factor = self.layer_idx + 1
+        #     self.scale_factor = 1 / self.unscale_factor
+        # else:
+        self.unscale_factor = 1
+        self.scale_factor = 1
 
 
     def numel(self) -> int:
 
-        return self.q_proj.numel() + \
-               self.k_proj.numel() + \
-               self.v_proj.numel() + \
-               self.o_proj.numel()
+        numel = self.q_proj.numel() + \
+                self.k_proj.numel() + \
+                self.v_proj.numel() + \
+                self.o_proj.numel()
+
+        if self.input_layernorm is not None: numel += self.input_layernorm.numel()
+        if self.q_norm is not None: numel += self.q_norm.numel()
+        if self.k_norm is not None: numel += self.k_norm.numel()
+
+        return numel
 
 
     def load(self):
 
-        if self.input_layernorm is not None:
-            self.input_layernorm.load()
+        if self.input_layernorm is not None: self.input_layernorm.load()
         self.q_proj.load()
         self.k_proj.load()
         self.v_proj.load()
         self.o_proj.load()
+        if self.q_norm is not None: self.q_norm.load()
+        if self.k_norm is not None: self.k_norm.load()
 
         if self.q_proj.is_quant():
 
             assert self.k_proj.is_quant() and self.v_proj.is_quant() and self.o_proj.is_quant(), "Partially quantized attention layer"
 
             device_tensors = self.model.get_device_tensors(self.device_idx)
             device_tensors.begin_scratch_alloc()
@@ -258,14 +287,24 @@
                 eps = self.input_layernorm.variance_epsilon
             else:
                 norm_weight = none_tensor
                 norm_bias = none_tensor
                 is_rms = False
                 eps = 0
 
+            if self.q_norm is None:
+                q_norm = none_tensor
+            else:
+                q_norm = self.q_norm.weight
+
+            if self.k_norm is None:
+                k_norm = none_tensor
+            else:
+                k_norm = self.k_norm.weight
+
             self.q_handle = ext_c.make_q_attn(norm_weight,
                                               norm_bias,
                                               is_rms,
                                               eps,
                                               self.q_proj.q_handle,
                                               self.k_proj.q_handle,
                                               self.v_proj.q_handle,
@@ -278,15 +317,17 @@
                                               self.model.config.max_input_len * self.model.config.max_batch_size,
                                               self.model.config.hidden_size,
                                               self.model.config.num_attention_heads,
                                               self.model.config.num_key_value_heads,
                                               self.model.config.head_dim,
                                               self.model.config.max_seq_len,
                                               self.has_residual,
-                                              self.model.config.arch.rope_neox_style)
+                                              self.model.config.arch.rope_style.value,
+                                              q_norm,
+                                              k_norm)
 
 
     def unload(self):
         if self.q_handle is not None:
             ext_c.free_q_attn(self.q_handle)
             self.q_handle = None
 
@@ -295,23 +336,31 @@
         if self.k_proj is not None: self.k_proj.unload()
         if self.v_proj is not None: self.v_proj.unload()
         self.o_proj.unload()
 
         self.temp_state = None
         self.temp_dq = None
 
+        if self.q_norm is not None: self.q_norm.unload()
+        if self.k_norm is not None: self.k_norm.unload()
+
 
     def weight_footprint(self):
 
         fp = self.q_proj.weight_footprint() + \
              self.k_proj.weight_footprint() + \
              self.v_proj.weight_footprint() + \
              self.o_proj.weight_footprint()
         if self.input_layernorm is not None:
             fp += self.input_layernorm.weight_footprint()
+        if self.q_norm is not None:
+            fp += self.q_norm.weight_footprint()
+        if self.k_norm is not None:
+            fp += self.k_norm.weight_footprint()
+
         return fp
 
 
     def scratch_space_fixed(self):
 
         return self.temp_state_size() + \
                self.temp_dq_size()
@@ -373,21 +422,21 @@
 
         return 2 * att_max * self.model.config.num_attention_heads * 2 + 128
 
 
     def set_device_idx(self, idx):
         super().set_device_idx(idx)
 
-        if self.input_layernorm is not None:
-            self.input_layernorm.set_device_idx(idx)
-
+        if self.input_layernorm is not None: self.input_layernorm.set_device_idx(idx)
         self.q_proj.set_device_idx(idx)
         self.k_proj.set_device_idx(idx)
         self.v_proj.set_device_idx(idx)
         self.o_proj.set_device_idx(idx)
+        if self.q_norm is not None: self.q_norm.set_device_idx(idx)
+        if self.k_norm is not None: self.k_norm.set_device_idx(idx)
 
 
     def repeat_kv(self, hidden_states: torch.Tensor, n_rep: int) -> torch.Tensor:
 
         if n_rep == 1: return hidden_states
 
         batch, num_key_value_heads, slen, head_dim = hidden_states.shape
@@ -398,38 +447,47 @@
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 cache: ExLlamaV2CacheBase | None = None,
                 attn_params: ExLlamaV2Attention.Params | None = None,
                 past_len: int | None = None,
                 intermediates: bool = False,
-                loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                loras: list[ExLlamaV2Lora] | None = None,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         global has_flash_attn
 
         if self.q_handle is None or intermediates:
-            return self.forward_torch(hidden_states, cache, attn_params, past_len, intermediates, loras = loras)
+            return self.forward_torch(hidden_states,
+                                      cache,
+                                      attn_params,
+                                      past_len,
+                                      intermediates,
+                                      loras = loras,
+                                      **kwargs)
 
         batch_size = hidden_states.shape[0]
         q_len = hidden_states.shape[1]
 
+        cfg = self.model.config
+
         direct = (batch_size == 1 and cache is not None and isinstance(cache, ExLlamaV2CacheBase))
 
         # past_len = 0
         # if cache is not None:
         #     if isinstance(cache, ExLlamaV2Cache):
         #         past_len = cache.current_seq_len
         #     if isinstance(cache, list):
         #         past_len = [c.current_seq_len for c in cache]
 
-        num_attention_heads = self.model.config.num_attention_heads
-        num_key_value_heads = self.model.config.num_key_value_heads
-        num_key_value_groups = self.model.config.num_key_value_groups
-        head_dim = self.model.config.head_dim
-        hidden_size = self.model.config.hidden_size
+        num_attention_heads = cfg.num_attention_heads
+        num_key_value_heads = cfg.num_key_value_heads
+        num_key_value_groups = cfg.num_key_value_groups
+        head_dim = cfg.head_dim
+        hidden_size = cfg.hidden_size
 
         constants = self.model.get_device_tensors(self.device_idx)
 
         q_shape = hidden_states.shape[:-1] + (self.q_proj.out_features,)
         k_shape = hidden_states.shape[:-1] + (self.k_proj.out_features,)
         v_shape = hidden_states.shape[:-1] + (self.v_proj.out_features,)
         q_states = torch.empty(q_shape, device = hidden_states.device, dtype = torch.half)
@@ -510,46 +568,55 @@
                     # Key/value tensors with past
 
                     k_states = batch_keys.narrow(0, 0, batch_size).narrow(1, 0, past_len + q_len)
                     v_states = batch_values.narrow(0, 0, batch_size).narrow(1, 0, past_len + q_len)
 
             # Torch matmul attention
 
-            if self.model.config.no_flash_attn or not has_flash_attn or not attn_params.is_causal():
+            if cfg.no_flash_attn or not has_flash_attn or not attn_params.is_causal():
 
                 q_states = q_states.transpose(1, 2)
                 k_states = k_states.transpose(1, 2)
                 v_states = v_states.transpose(1, 2)
 
                 k_states = self.repeat_kv(k_states, num_key_value_groups)
                 k_states = k_states.transpose(-1, -2)
 
                 attn_weights = torch.matmul(q_states, k_states)
                 k_states = None
                 q_states = None
 
-                attn_weights /= math.sqrt(head_dim)
+                # attn_weights *= self.scale_factor / math.sqrt(head_dim)
+                # attn_mask = attn_params.get_attn_mask(hidden_states.device)
+                # if self.unscale_factor != 1: attn_weights *= self.unscale_factor
+                attn_weights *= 1 / math.sqrt(head_dim)
                 attn_mask = attn_params.get_attn_mask(hidden_states.device)
                 if attn_mask is not None: attn_weights = attn_weights + attn_mask
                 attn_weights = nn.functional.softmax(attn_weights, dim = -1, dtype = torch.float16)
 
                 v_states = self.repeat_kv(v_states, num_key_value_groups)
                 attn_output = torch.matmul(attn_weights, v_states)
                 v_states = None
 
                 attn_output = attn_output.transpose(1, 2)
-                attn_output = attn_output.reshape((batch_size, q_len, self.model.config.num_attention_heads * self.model.config.head_dim))
+                attn_output = attn_output.reshape((batch_size, q_len, cfg.num_attention_heads * cfg.head_dim))
 
             # Flash Attention 2
 
             else:
 
                 # TODO: Enable flash-attn with input mask
-                attn_output = flash_attn_func(q_states, k_states, v_states, causal = True)
-                attn_output = attn_output.reshape((batch_size, q_len, self.model.config.num_attention_heads * self.model.config.head_dim))
+                attn_output = flash_attn_func(
+                    q_states,
+                    k_states,
+                    v_states,
+                    # softmax_scale = None if self.scale_factor == 1 else self.scale_factor / math.sqrt(head_dim),
+                    causal = True
+                )
+                attn_output = attn_output.reshape((batch_size, q_len, cfg.num_attention_heads * cfg.head_dim))
 
             # xformers memory_efficient_attention
 
             # attn_output = xops.memory_efficient_attention(q_states, k_states, v_states, attn_bias = xops.LowerTriangularMask())
             # attn_output = attn_output.reshape((batch_size, q_len, hidden_size));
 
             # Torch SDP attention:
@@ -650,62 +717,61 @@
 
     def forward_torch(self,
                       hidden_states: torch.Tensor,
                       cache: ExLlamaV2CacheBase | None = None,
                       attn_params: ExLlamaV2Attention.Params | None = None,
                       past_len: int | None = None,
                       intermediates: bool = False,
-                      loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict:
+                      loras: list[ExLlamaV2Lora] | None = None,
+                      **kwargs) -> torch.Tensor | dict:
 
-        num_attention_heads = self.model.config.num_attention_heads
-        num_key_value_heads = self.model.config.num_key_value_heads
-        num_key_value_groups = self.model.config.num_key_value_groups
-        head_dim = self.model.config.head_dim
-        hidden_size = self.model.config.hidden_size
+        cfg = self.model.config
+        num_attention_heads = cfg.num_attention_heads
+        num_key_value_heads = cfg.num_key_value_heads
+        num_key_value_groups = cfg.num_key_value_groups
+        head_dim = cfg.head_dim
+        hidden_size = cfg.hidden_size
 
         batch_size, q_len, _ = hidden_states.size()
 
         past_len = 0 if cache is None else cache.current_seq_len
 
         # Project q, k, v
 
         residual = hidden_states
         post_norm = self.input_layernorm.forward(hidden_states) if self.has_norm else hidden_states
 
-        query_states_im = self.q_proj.forward(post_norm, loras = loras)
-        key_states_im = self.k_proj.forward(post_norm, loras = loras)
-        value_states_im = self.v_proj.forward(post_norm, loras = loras)
-
-        # if intermediates:
-        #
-        #     query_states = query_states_im.clone()
-        #     key_states = key_states_im.clone()
-        #     value_states = value_states_im.clone()
-        #
-        # else:
-
-        query_states = query_states_im
-        key_states = key_states_im
-        value_states = value_states_im
+        query_states = self.q_proj.forward(post_norm, loras = loras)
+        key_states = self.k_proj.forward(post_norm, loras = loras)
+        value_states = self.v_proj.forward(post_norm, loras = loras)
 
-        # Apply position embeddings
+        # Shape for attention
 
         query_states = query_states.view(batch_size, q_len, num_attention_heads, head_dim)
         key_states = key_states.view(batch_size, q_len, num_key_value_heads, head_dim)
         value_states = value_states.view(batch_size, q_len, num_key_value_heads, head_dim)
 
+        # Apply Q/K norms
+
+        if cfg.use_qk_norm:
+            query_states = self.q_norm.forward(query_states)
+            key_states = self.k_norm.forward(key_states)
+
+        # Apply position embeddings
+
         constants = self.model.get_device_tensors(self.device_idx, scratch = False)
 
         if attn_params.position_offsets is not None:
             position_offsets = attn_params.get_position_offsets(hidden_states.device)
         else:
             position_offsets = none_tensor
 
-        ext_c.rope_(query_states, constants.sin, constants.cos, past_len, num_attention_heads, head_dim, position_offsets, self.model.config.arch.rope_neox_style)
-        ext_c.rope_(key_states, constants.sin, constants.cos, past_len, num_key_value_heads, head_dim, position_offsets, self.model.config.arch.rope_neox_style)
+        if cfg.arch.rope_style != RopeStyle.NONE:
+            ext_c.rope_(query_states, constants.sin, constants.cos, past_len, num_attention_heads, head_dim, position_offsets, cfg.arch.rope_style == RopeStyle.NEOX)
+            ext_c.rope_(key_states, constants.sin, constants.cos, past_len, num_key_value_heads, head_dim, position_offsets, cfg.arch.rope_style == RopeStyle.NEOX)
 
         # Add keys and values to cache
 
         if cache is not None:
 
             batch_keys, batch_values = cache.get_kv_state(self.layer_idx, batch_size, 0, past_len)
             new_keys = batch_keys.narrow(1, past_len, q_len).narrow(0, 0, batch_size)
@@ -716,41 +782,50 @@
             # Key/value tensors with past
 
             key_states = batch_keys.narrow(1, 0, past_len + q_len).narrow(0, 0, batch_size)
             value_states = batch_values.narrow(1, 0, past_len + q_len).narrow(0, 0, batch_size)
 
         # Torch matmul attention
 
-        if self.model.config.no_flash_attn or not has_flash_attn or not attn_params.is_causal():
+        if cfg.no_flash_attn or not has_flash_attn or not attn_params.is_causal():
 
             query_states = query_states.transpose(1, 2)
             key_states = key_states.transpose(1, 2)
             value_states = value_states.transpose(1, 2)
 
-            key_states = self.repeat_kv(key_states, self.model.config.num_key_value_groups)
+            key_states = self.repeat_kv(key_states, cfg.num_key_value_groups)
             key_states = key_states.transpose(-1, -2)
 
             attn_weights = torch.matmul(query_states, key_states)
-            attn_weights /= math.sqrt(head_dim)
+            # attn_weights *= self.scale_factor / math.sqrt(head_dim)
+            # attn_mask = attn_params.get_attn_mask(hidden_states.device)
+            # if self.scale_factor != 1: attn_weights *= self.unscale_factor
+            attn_weights *= 1 / math.sqrt(head_dim)
             attn_mask = attn_params.get_attn_mask(hidden_states.device)
             if attn_mask is not None: attn_weights = attn_weights + attn_mask
             attn_weights = nn.functional.softmax(attn_weights, dim = -1, dtype = torch.float16)
 
-            value_states = self.repeat_kv(value_states, self.model.config.num_key_value_groups)
+            value_states = self.repeat_kv(value_states, cfg.num_key_value_groups)
             attn_output = torch.matmul(attn_weights, value_states)
 
             attn_output = attn_output.transpose(1, 2)
-            attn_output = attn_output.reshape((batch_size, q_len, self.model.config.num_attention_heads * self.model.config.head_dim))
+            attn_output = attn_output.reshape((batch_size, q_len, cfg.num_attention_heads * cfg.head_dim))
 
         # Flash Attention 2
 
         else:
 
-            attn_output = flash_attn_func(query_states, key_states, value_states, causal = True)
-            attn_output = attn_output.reshape((batch_size, q_len, self.model.config.num_attention_heads * self.model.config.head_dim))
+            attn_output = flash_attn_func(
+                query_states,
+                key_states,
+                value_states,
+                # softmax_scale = None if self.scale_factor == 1 else self.scale_factor / math.sqrt(head_dim),
+                causal = True
+            )
+            attn_output = attn_output.reshape((batch_size, q_len, cfg.num_attention_heads * cfg.head_dim))
 
         # Update 8-bit/Q4 cache
 
         if cache is not None:
             cache.store_kv_state(self.layer_idx, batch_size, past_len, q_len)
 
         # Output projection
@@ -769,14 +844,16 @@
             return hidden_states
 
 
     def update_loras(self):
 
         if self.q_handle is None: return
 
+        cfg = self.model.config
+
         q_proj_lora_a = { id(k): v for k, v in self.q_proj.lora_a_tensors.items() }
         q_proj_lora_b = { id(k): v for k, v in self.q_proj.lora_b_tensors.items() }
         k_proj_lora_a = { id(k): v for k, v in self.k_proj.lora_a_tensors.items() }
         k_proj_lora_b = { id(k): v for k, v in self.k_proj.lora_b_tensors.items() }
         v_proj_lora_a = { id(k): v for k, v in self.v_proj.lora_a_tensors.items() }
         v_proj_lora_b = { id(k): v for k, v in self.v_proj.lora_b_tensors.items() }
         o_proj_lora_a = { id(k): v for k, v in self.o_proj.lora_a_tensors.items() }
@@ -788,13 +865,12 @@
                                                 k_proj_lora_a,
                                                 k_proj_lora_b,
                                                 v_proj_lora_a,
                                                 v_proj_lora_b,
                                                 o_proj_lora_a,
                                                 o_proj_lora_b)
 
-        self.temp_lora_size = temp_lora_size * self.model.config.max_batch_size * self.model.config.max_input_len
+        self.temp_lora_size = temp_lora_size * cfg.max_batch_size * cfg.max_input_len
 
 
     def is_quant(self):
         return self.q_handle is not None
-
```

### Comparing `exl2conv-0.0.20/exl2conv/cache.py` & `exl2conv-0.0.21/exl2conv/cache.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/compat.py` & `exl2conv-0.0.21/exl2conv/compat.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/config.py` & `exl2conv-0.0.21/exl2conv/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 no_default = object()
 
 def read(input_dict: dict[str, Any], expected_type: type, keys: str | list[str], default = no_default) -> T:
 
     if isinstance(keys, str): keys = [keys]
 
     for key in keys:
+        input_dict_s = input_dict
 
         key_split = key.split("->")
         for subk in key_split[:-1]:
-            input_dict = input_dict.get(subk, None)
-            if not input_dict:
+            input_dict_s = input_dict_s.get(subk, None)
+            if not input_dict_s:
                 key = None
                 break
         if key is None: continue
         key = key_split[-1]
 
-        x = input_dict.get(key, None)
+        x = input_dict_s.get(key, None)
         if x is not None:
 
             if expected_type == float and isinstance(x, int):
                 x = float(x)
             if expected_type == int and isinstance(x, float) and x == int(x):
                 x = int(x)
 
@@ -130,15 +131,15 @@
 
     # Set low-mem options
 
     def set_low_mem(self):
 
         self.max_input_len = 1024
         self.max_attention_size = 1024 ** 2
-        self.max_output_len = 1024
+        self.max_output_len = min(self.max_output_len, 1024)
 
 
     # Populate config with required files from model_dir
 
     def prepare(self, no_tensors: bool = False):
 
         assert self.model_dir is not None, "No model_dir specified in ExLlamaV2Config"
@@ -148,14 +149,31 @@
 
         self.model_config = os.path.join(self.model_dir, "config.json")
         assert os.path.exists(self.model_config), "Can't find " + self.model_config
 
         with open(self.model_config, encoding = "utf8") as f:
             read_config = json.load(f)
 
+        # Load generation_config.json
+
+        self.generation_config_path = os.path.join(self.model_dir, "generation_config.json")
+        if os.path.exists(self.generation_config_path):
+            with open(self.generation_config_path, encoding = "utf8") as f:
+                gen_config = json.load(f)
+                self.generation_config = {}
+                try:
+                    self.generation_config['eos_token_id'] = read(gen_config, list, "eos_token_id", None)
+                except (ValueError, TypeError):
+                    eos_token_id_as_int = read(gen_config, int, "eos_token_id", None)
+                    if eos_token_id_as_int is not None:
+                        self.generation_config['eos_token_id'] = [eos_token_id_as_int]
+                    else:
+                        self.generation_config['eos_token_id'] = None
+                    
+        
         # Model architecture
 
         assert len(read_config["architectures"]) == 1, "Multiple architectures defined in config.json"
         self.architecture = read_config["architectures"][0]
         self.arch = ExLlamaV2ArchParams(self.architecture, read_config)
 
         # Vocab params
@@ -164,54 +182,63 @@
         self.eos_token_id = read(read_config, int, "eos_token_id", None)  # 2
         self.pad_token_id = read(read_config, int, "pad_token_id", None)  # 0
         self.vocab_size = read(read_config, int, "vocab_size")
 
         # Standard params
 
         self.initializer_range = read(read_config, float, ["initializer_range"])
-        self.num_hidden_layers = read(read_config, int, ["num_hidden_layers", "n_layers"])
+        self.num_hidden_layers = read(read_config, int, ["num_hidden_layers", "n_layers", "n_layer"])
 
         # Norm params
 
         if self.arch.norm_eps_key:
             self.norm_eps = read(read_config, float, self.arch.norm_eps_key)
         else:
             self.norm_eps = 1e-5  # Torch default
 
         # Model dimensions
 
-        self.hidden_size = read(read_config, int, ["hidden_size", "d_model"])
+        self.hidden_size = read(read_config, int, ["hidden_size", "d_model", "n_embd"])
 
         # Attn params
 
-        self.num_attention_heads = read(read_config, int, ["num_attention_heads", "n_heads"])
+        self.num_attention_heads = read(read_config, int, ["num_attention_heads", "n_heads", "n_head"])
         self.head_dim = read(read_config, int, "head_dim", self.hidden_size // self.num_attention_heads)
 
-        self.num_key_value_heads = read(read_config, int, ["num_key_value_heads", "attn_config->kv_n_heads"], self.num_attention_heads)
+        if self.arch.mqa:
+            self.num_key_value_heads = 1
+        else:
+            self.num_key_value_heads = read(read_config, int, ["num_key_value_heads", "attn_config->kv_n_heads"], self.num_attention_heads)
         self.num_key_value_groups = self.num_attention_heads // self.num_key_value_heads
         self.use_qk_norm = read(read_config, bool, ["use_qk_norm"], False)
 
         # MLP params
 
-        self.intermediate_size = read(read_config, int, ["intermediate_size", "ffn_config->ffn_hidden_size"])
+        if self.arch.default_inner_dim_mult is not None:
+            default_intermediate_size = self.arch.default_inner_dim_mult * self.hidden_size
+        else:
+            default_intermediate_size = no_default
+
+        self.intermediate_size = read(read_config, int, ["intermediate_size", "ffn_config->ffn_hidden_size", "n_inner"], default_intermediate_size)
         self.num_experts = read(read_config, int, ["num_local_experts", "ffn_config->moe_num_experts"], None)
         self.num_experts_per_token = read(read_config, int,["num_experts_per_tok", "ffn_config->moe_top_k"], None)
 
         # Logit scale
 
         self.logit_scale = read(read_config, float, "logit_scale", 1)
 
         # Positional embeddings
 
         self.rotary_embedding_base = read(read_config, float, ["rope_theta", "attn_config->rope_theta"], 10000.0)
 
         self.max_seq_len = read(read_config, int,["max_sequence_length",
                                                   "model_max_length",
                                                   "max_position_embeddings",
-                                                  "max_seq_len"], 2048)
+                                                  "max_seq_len",
+                                                  "n_positions"], 2048)
         self.original_max_seq_len = self.max_seq_len
 
         rs = read(read_config, dict, "rope_scaling", None)
         if rs:
             scaling_type = rs.get("type", None)
             if scaling_type == "linear":
                 assert "factor" in rs, "'factor' missing from 'rope_scaling' config"
```

### Comparing `exl2conv-0.0.20/exl2conv/conversion/adaptivegptq.py` & `exl2conv-0.0.21/exl2conv/conversion/adaptivegptq.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/compile.py` & `exl2conv-0.0.21/exl2conv/conversion/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from exl2conv.model import \
 (
     ExLlamaV2Embedding,
+    ExLlamaV2PosEmbedding,
     ExLlamaV2Attention,
     ExLlamaV2MLP,
     ExLlamaV2MoEMLP,
     ExLlamaV2ParallelDecoder,
     ExLlamaV2Linear,
     ExLlamaV2RMSNorm,
     ExLlamaV2LayerNorm
@@ -65,14 +66,18 @@
 
         module = model.modules[index]
 
         if isinstance(module, ExLlamaV2Embedding):
 
             d = get_f_module(job, module); out_dict.update(d); current_size += _dsize(d)
 
+        if isinstance(module, ExLlamaV2PosEmbedding):
+
+            d = get_f_module(job, module); out_dict.update(d); current_size += _dsize(d)
+
         if isinstance(module, ExLlamaV2Attention):
 
             d = get_f_module(job, module.input_layernorm); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.q_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.k_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.v_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.o_proj); out_dict.update(d); current_size += _dsize(d)
```

### Comparing `exl2conv-0.0.20/exl2conv/conversion/convert.py` & `exl2conv-0.0.21/exl2conv/conversion/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from exl2conv import ExLlamaV2, ExLlamaV2Config, ExLlamaV2Tokenizer
+from exl2conv.architecture import RopeStyle
 import argparse, os, shutil
 import sys
 import json
 from exl2conv.conversion.tokenize import tokenize
 from exl2conv.conversion.measure import embeddings, measure_quant
 from exl2conv.conversion.quantize import quant
 from exl2conv.conversion.optimize import optimize
 from exl2conv.conversion.compile import compile_model
 from exl2conv.conversion.qparams import qparams_headoptions
+import torch
 
 def convert_hf_to_exl2(options):
 
     # Create config
 
     config = ExLlamaV2Config()
     config.model_dir = options["in_dir"]
     config.qkv_embed = False
     config.prepare()
 
     # Tokenizer
 
     tokenizer = ExLlamaV2Tokenizer(config)
 
-    # Create job
+    # 
+    torch.set_printoptions(precision = 7, sci_mode = False, linewidth = 200)
 
+    # Create job
 
     def save_job():
         global job_file, job
         with open(job_file, "w", encoding = "utf8") as f:
             f.write(json.dumps(job, indent = 4))
 
 
@@ -147,14 +151,25 @@
     if "rope_alpha" in job: config.scale_alpha_value = job["rope_alpha"]
 
     # Create model without loading weights
 
     model = ExLlamaV2(config)
     model.load(lazy = True)
 
+    # Limit context length if necessary
+    
+    if model.config.arch.rope_style == RopeStyle.NONE:
+        max_ctx = model.config.max_seq_len
+        if job["length"] > max_ctx:
+            print (f" !! Warning: Reducing calibration length to model max context: {max_ctx}")
+            job["length"] = max_ctx
+        if job["measurement_length"] > max_ctx:
+            print (f" !! Warning: Reducing measurement calibration length to model max context: {max_ctx}")
+            job["measurement_length"] = max_ctx
+
     # Do the things
 
     save_job()
 
     while True:
 
         progress = job["progress"]
```

### Comparing `exl2conv-0.0.20/exl2conv/conversion/measure.py` & `exl2conv-0.0.21/exl2conv/conversion/measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from exl2conv.model import \
 (
     ExLlamaV2Embedding,
+    ExLlamaV2PosEmbedding,
     ExLlamaV2Attention,
     ExLlamaV2MLP,
     ExLlamaV2MoEMLP,
     ExLlamaV2Linear,
     ExLlamaV2RMSNorm,
     ExLlamaV2LayerNorm,
     ExLlamaV2ParallelDecoder
@@ -483,14 +484,17 @@
         elif isinstance(module, ExLlamaV2Linear):
             mode = "linear"
             # Don't measure head layer
 
         elif isinstance(module, ExLlamaV2RMSNorm) or isinstance(module, ExLlamaV2LayerNorm):
             mode = "norm"
 
+        elif isinstance(module, ExLlamaV2PosEmbedding):
+            mode = "pos_emb"
+
         # Reference forward pass
 
         cache = None
         attn_params = ExLlamaV2Attention.Params(1, hidden_states[0].shape[1], 0, None, None) \
             if mode in ["self_attn", "parallel_decoder"] else None
 
         target_states = []
@@ -533,14 +537,17 @@
                 quantizers["o_proj"].add_batch(outputs["attn_output"])
                 quantizers["down_proj"].add_batch(outputs["pre_down"])
                 hidden_states[i] = outputs["post_norm"]
                 target_states_attn.append(outputs["hidden_states_attn"].to("cpu"))
                 target_states_mlp.append(outputs["hidden_states_mlp"].to("cpu"))
                 target_states.append(outputs["hidden_states"].to("cpu"))
 
+            if mode == "pos_emb":
+                target_states.append(outputs["hidden_states"].to("cpu"))
+
         # For MoE layers, warn if any layer received less than 10% of a calibration batch
 
         if mode == "block_sparse_moe":
             for j in range(model.config.num_experts):
                 ue = uncalibrated_experts[j]
                 if ue > len(hidden_states) * 0.20:
                     print(f" !! Warning: w2.{j} has less than 10% calibration for {ue}/{len(hidden_states)} rows")
```

### Comparing `exl2conv-0.0.20/exl2conv/conversion/qparams.py` & `exl2conv-0.0.21/exl2conv/conversion/qparams.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/quantize.py` & `exl2conv-0.0.21/exl2conv/conversion/quantize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from exl2conv.model import \
 (
     ExLlamaV2Embedding,
+    ExLlamaV2PosEmbedding,
     ExLlamaV2Attention,
     ExLlamaV2MLP,
     ExLlamaV2MoEMLP,
     ExLlamaV2ParallelDecoder,
     ExLlamaV2Linear,
     ExLlamaV2RMSNorm,
     ExLlamaV2LayerNorm
@@ -323,14 +324,17 @@
             mode = "linear"
             assert module.key == "lm_head"
             quantizers["lm_head"] = AdaptiveGPTQ(module.linear)
 
         elif isinstance(module, ExLlamaV2RMSNorm) or isinstance(module, ExLlamaV2LayerNorm):
             mode = "norm"
 
+        elif isinstance(module, ExLlamaV2PosEmbedding):
+            mode = "pos_emb"
+
         elif isinstance(module, ExLlamaV2ParallelDecoder):
             mode = "parallel_decoder"
             quantizers["q_proj"] = AdaptiveGPTQ(module.attn.q_proj.linear)
             quantizers["k_proj"] = AdaptiveGPTQ(module.attn.k_proj.linear)
             quantizers["v_proj"] = AdaptiveGPTQ(module.attn.v_proj.linear)
             quantizers["o_proj"] = AdaptiveGPTQ(module.attn.o_proj.linear)
             has_gate = module.model.config.arch.mlp_gate
@@ -522,8 +526,8 @@
                 os.replace(temp_filename, states_filename)
 
             job["q_last_module_idx"] = index
 
             del job["invalid"]
             save_fn()
 
-            last_snapshot_time = time.time()
+            last_snapshot_time = time.time()
```

### Comparing `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/c4.utf8` & `exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/c4.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/code.utf8` & `exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/code.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/multilingual.utf8` & `exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/multilingual.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/technical.utf8` & `exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/technical.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/tiny.utf8` & `exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/tiny.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/wiki.utf8` & `exl2conv-0.0.21/exl2conv/conversion/standard_cal_data/wiki.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/conversion/tokenize.py` & `exl2conv-0.0.21/exl2conv/conversion/tokenize.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,23 +40,23 @@
     cal_ds = job["cal_dataset"]
 
     if cal_ds is not None:
         rows = job["measurement_rows"] if measure else job["dataset_rows"]
         length = job["measurement_length"] if measure else job["length"]
         cal_tokens = get_tokens(rows, length, cal_ds, tokenizer)
     else:
-        cal_tokens = get_standard_calibration(measure, tokenizer)
+        cal_tokens = get_standard_calibration(job, measure, tokenizer)
 
     cal_filename = os.path.join(job["out_dir"], "cal_data.safetensors")
     cal_dict = { "input_ids": cal_tokens }
     save_file(cal_dict, cal_filename)
     job["cal_filename"] = cal_filename
 
 
-def get_standard_calibration(measure, tokenizer):
+def get_standard_calibration(job, measure, tokenizer):
 
     data_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "standard_cal_data")
     file_c4 =os.path.join(data_dir, "c4.utf8")
     file_code =os.path.join(data_dir, "code.utf8")
     file_multilingual =os.path.join(data_dir, "multilingual.utf8")
     file_technical =os.path.join(data_dir, "technical.utf8")
     file_wiki = os.path.join(data_dir, "wiki.utf8")
@@ -68,23 +68,25 @@
     rows_code = 3 if measure else 15
     rows_tiny = 2 if measure else 10
     rows_multilingual = 3 if measure else 15
     rows_multilingual_s = 1 if measure else 5
     rows_technical = 2 if measure else 10
     rows_random = 2
 
+    ctx = min(2048, job["measurement_length"] if measure else job["length"])
+
     # C4: 10 rows
 
     with open(file_c4, "r", encoding="utf8") as f:
         lines = f.readlines()
 
     text = "\n\n".join(lines)
     tokens = tokenizer.encode(text)
-    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % 2048)]
-    tokenized_rows = tokens.view(-1, 2048)
+    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % ctx)]
+    tokenized_rows = tokens.view(-1, ctx)
 
     for i in range(rows_c4):
         rows.append(tokenized_rows[i:i+1])
 
     # Wiki: 24 aligned rows + 24 aligned rows with BOS
 
     with open(file_wiki, "r", encoding="utf8") as f:
@@ -93,30 +95,30 @@
     articles = [a[a.find("\n") + 1:] for a in text.split("</doc>\n")]
     tokenized_articles = [tokenizer.encode(a, add_bos = True, add_eos = True) for a in articles]
 
     idx = 0
     for r in range(rows_wiki):
         length = 0
         idx0 = idx
-        while length < 2049:
+        while length < ctx + 1:
             length += tokenized_articles[idx].shape[-1]
             idx += 1
         row = torch.cat(tokenized_articles[idx0 : idx], dim = -1)
-        if r < rows_wiki // 2: row = row[:, 1:2049]
-        else: row = row[:, :2048]
+        if r < rows_wiki // 2: row = row[:, 1:ctx+1]
+        else: row = row[:, :ctx]
         rows.append(row)
 
     # Code: 15 rows
 
     with open(file_code, "r", encoding="utf8") as f:
         text = f.read()
 
     tokens = tokenizer.encode(text)
-    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % 2048)]
-    tokenized_rows = tokens.view(-1, 2048)
+    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % ctx)]
+    tokenized_rows = tokens.view(-1, ctx)
 
     for i in range(rows_code):
         rows.append(tokenized_rows[i:i+1])
 
     # Tinystories: 5 aligned rows + 5 aligned rows with BOS
 
     with open(file_tiny, "r", encoding="utf8") as f:
@@ -125,59 +127,59 @@
     articles = text.split("<|endoftext|>")
     tokenized_articles = [tokenizer.encode(a.strip(), add_bos = True, add_eos = True) for a in articles]
 
     idx = 0
     for r in range(rows_tiny):
         length = 0
         idx0 = idx
-        while length < 2049:
+        while length < ctx + 1:
             length += tokenized_articles[idx].shape[-1]
             idx += 1
         row = torch.cat(tokenized_articles[idx0 : idx], dim = -1)
-        if r < rows_tiny // 2: row = row[:, 1:2049]
-        else: row = row[:, :2048]
+        if r < rows_tiny // 2: row = row[:, 1:ctx+1]
+        else: row = row[:, :ctx]
         rows.append(row)
 
     # Multilingual: 15 rows + 5 shuffled rows
 
     with open(file_multilingual, "r", encoding="utf8") as f:
         text = f.read()
 
     tokens = tokenizer.encode(text)
-    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % 2048)]
-    tokenized_rows = tokens.view(-1, 2048)
+    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % ctx)]
+    tokenized_rows = tokens.view(-1, ctx)
 
     for i in range(rows_multilingual):
         rows.append(tokenized_rows[i:i+1])
 
     tokenized_rows = tokens.view(-1, 128)
     random.seed(69420)
     for i in range(rows_multilingual_s):
         row = []
-        for j in range(2048 // 128):
+        for j in range(ctx // 128):
             k = random.randint(0, tokenized_rows.shape[0] - 1)
             row.append(tokenized_rows[k].unsqueeze(0))
         rows.append(torch.cat(row, dim = -1))
 
     # Randomized: 2 rows
 
     vocab_size = tokenizer.get_vocab_size()
     random.seed(69420)
     for i in range(rows_random):
-        row = torch.randint(0, vocab_size, (1, 2048), dtype = torch.long)
+        row = torch.randint(0, vocab_size, (1, ctx), dtype = torch.long)
         rows.append(row)
 
     # Technical: 10 rows
 
     with open(file_technical, "r", encoding="utf8") as f:
         text = f.read()
 
     tokens = tokenizer.encode(text)
-    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % 2048)]
-    tokenized_rows = tokens.view(-1, 2048)
+    tokens = tokens[:, : tokens.shape[-1] - (tokens.shape[-1] % ctx)]
+    tokenized_rows = tokens.view(-1, ctx)
 
     for i in range(rows_technical):
         rows.append(tokenized_rows[i:i+1])
 
     # for idx, r in enumerate(rows):
     #     print("------------------------------------------------------------------------------")
     #     print(idx)
```

### Comparing `exl2conv-0.0.20/exl2conv/embedding.py` & `exl2conv-0.0.21/exl2conv/embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,19 @@
                 cache = None,
                 attn_params: ExLlamaV2Attention.Params = None,
                 past_len = None,
                 intermediates: bool = False,
                 loras = None,
                 **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
+        # If input IDs contain negative values, assume they are padding tokens from a model with not pad_token_id
+        # defined
+
+        hidden_states = hidden_states.clamp(min = 0)
+
         # Apply indexed embeddings
 
         indexed_embeddings = kwargs.get("indexed_embeddings")
         if indexed_embeddings is not None:
 
             # Split prompt
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx2_target.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/avx2_target.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx_mathfun.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/avx_mathfun.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/profiling.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/profiling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/quantize_func.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,17 @@
             columns,
             qzero,
             maxq
         );
 
         vv_mul_sub_cuda
         (
-            ((const float*) hessian_inv.data_ptr()) + c * hcolumns + c,
-            ((const float*) error.data_ptr()) + c * columns,
-            ((float*) weights.data_ptr()) + c * columns,
+            ((const float*) hessian_inv.data_ptr()) + (uint64_t)c * (uint64_t)hcolumns + (uint64_t)c,
+            ((const float*) error.data_ptr()) + (uint64_t)c * (uint64_t)columns,
+            ((float*) weights.data_ptr()) + (uint64_t)c * (uint64_t)columns,
             b - c,
             columns
         );
     }
 
     torch::Tensor x = hessian_inv.slice(0, a, b).slice(1, b).transpose(0, 1);
     torch::Tensor y = error.slice(0, a, b);
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/quantize_func.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/safetensors.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/safetensors.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -71,30 +71,33 @@
     if (beg < 0) beg = 0;
 
     // Iter over context, backwards
 
     for (int i = seq_len; i > beg;)
     {
         uint64_t t = sequence[--i];
+        if (t < g_vocab_size)
+        {
 
-        // If t has not been encountered before, apply rep_p and pres_p
+            // If t has not been encountered before, apply rep_p and pres_p
 
-        if (!g_rep_mask[t])
-        {
-            if (logits[t] > 0.0) logits[t] /= rep_p;  // Multiplicative penalty
-            else logits[t] *= rep_p;
+            if (!g_rep_mask[t])
+            {
+                if (logits[t] > 0.0) logits[t] /= rep_p;  // Multiplicative penalty
+                else logits[t] *= rep_p;
 
-            logits[t] -= pres_p;  // Additive penalty
+                logits[t] -= pres_p;  // Additive penalty
 
-            g_rep_mask[t] = true;  // Only once per logit
-        }
+                g_rep_mask[t] = true;  // Only once per logit
+            }
 
-        // Apply freq_p penalty for every time a token is encountered, so the total additive penalty is count * freq_p
+            // Apply freq_p penalty for every time a token is encountered, so the total additive penalty is count * freq_p
 
-        logits[t] -= freq_p;
+            logits[t] -= freq_p;
+        }
 
         // If we're in the "decay" range, reduce penalties for every token
 
         if (--sust < 0)
         {
             rep_p += d_rep_p;
             freq_p += d_freq_p;
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/util.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cpp/util.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/cache.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/cache.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/compat.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/compat.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_add.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_add.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/h_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/head_norm.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/head_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/layer_norm.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/lora.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/lora.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/matrix_view.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/matrix_view.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/pack_tensor.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_attn.cu`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     int _max_rows,
     int _hidden_size,
     int _num_heads,
     int _num_kv_heads,
     int _head_dim,
     int _max_seq_len,
     bool _has_residual,
-    bool _neox_style,
+    int _rope_style,
     half* _q_norm,
     half* _k_norm
 ):
     layernorm(_layernorm),
     layernorm_bias(_layernorm_bias),
     layernorm_is_rms(_layernorm_is_rms),
     norm_epsilon(_norm_epsilon),
@@ -111,15 +111,15 @@
     max_rows(_max_rows),
     hidden_size(_hidden_size),
     num_heads(_num_heads),
     num_kv_heads(_num_kv_heads),
     head_dim(_head_dim),
     max_seq_len(_max_seq_len),
     has_residual(_has_residual),
-    neox_style(_neox_style),
+    rope_style(_rope_style),
     q_norm(_q_norm),
     k_norm(_k_norm)
 {
 }
 
 QAttn::~QAttn()
 {
@@ -165,30 +165,34 @@
 
     apply_loras_cuda(cublas_handle, q_proj_lora, loras, q_proj, norm_state, temp_q, lora_temp, q_len * batch_size);
     apply_loras_cuda(cublas_handle, k_proj_lora, loras, k_proj, norm_state, temp_k, lora_temp, q_len * batch_size);
     apply_loras_cuda(cublas_handle, v_proj_lora, loras, v_proj, norm_state, temp_v, lora_temp, q_len * batch_size);
 
 //    rope_cuda(temp_q, sin, cos, batch_size, q_len * num_heads,    head_dim, num_heads,    past_len, past_lens);
 //    rope_cuda(temp_k, sin, cos, batch_size, q_len * num_kv_heads, head_dim, num_kv_heads, past_len, past_lens);
-    rope_cuda_qk
-    (
-        temp_q,
-        temp_k,
-        sin,
-        cos,
-        batch_size,
-        q_len * num_heads,
-        q_len * num_kv_heads,
-        head_dim,
-        num_heads,
-        num_kv_heads,
-        past_len,
-        past_lens,
-        neox_style
-    );
+
+    if (rope_style != ROPE_STYLE_NONE)
+    {
+        rope_cuda_qk
+        (
+            temp_q,
+            temp_k,
+            sin,
+            cos,
+            batch_size,
+            q_len * num_heads,
+            q_len * num_kv_heads,
+            head_dim,
+            num_heads,
+            num_kv_heads,
+            past_len,
+            past_lens,
+            rope_style == ROPE_STYLE_NEOX
+        );
+    }
 }
 
 void QAttn::forward_cuda_2
 (
     cublasHandle_t cublas_handle,
     const half* attn_output,
     half* hidden_state,
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_attn.cuh`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 #include <cuda_fp16.h>
 #include <cstdint>
 #include <cstdio>
 #include <ATen/cuda/CUDAContext.h>
 
 #include "q_matrix.cuh"
 
+#define ROPE_STYLE_NONE 0
+#define ROPE_STYLE_GPTJ 1
+#define ROPE_STYLE_NEOX 2
+
 class QAttn
 {
 public:
 
     half* layernorm;
     half* layernorm_bias;
     bool layernorm_is_rms;
@@ -42,15 +46,15 @@
 
     std::unordered_map<uintptr_t, std::tuple<half*, half*, int>> q_proj_lora;
     std::unordered_map<uintptr_t, std::tuple<half*, half*, int>> k_proj_lora;
     std::unordered_map<uintptr_t, std::tuple<half*, half*, int>> v_proj_lora;
     std::unordered_map<uintptr_t, std::tuple<half*, half*, int>> o_proj_lora;
 
     bool has_residual;
-    bool neox_style;
+    int rope_style;
 
     QAttn
     (
         half* _layernorm,
         half* _layermorm_bias,
         bool _layernorm_is_rms,
         float _norm_epsilon,
@@ -66,15 +70,15 @@
         int _max_rows,
         int _hidden_size,
         int _num_heads,
         int _num_kv_heads,
         int _head_dim,
         int _max_seq_len,
         bool _has_residual,
-        bool _neox_style,
+        int _rope_style,
         half* _q_norm,
         half* _k_norm
     );
 
     ~QAttn();
 
     void forward_cuda_1
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_matrix.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_matrix.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quantize.cu`

 * *Files 6% similar despite different names*

```diff
@@ -123,15 +123,16 @@
     h_x = __hsub(h_x, h_qzero);
     h_x = __hmul(h_x, h_s);
     float q = __half2float(h_x);
     quant[idx] = q;
 
     // Adjust error
 
-    float d = hessian_inv[row * rows + row];  // H diagonal
+    uint64_t d_idx = (uint64_t)row * (uint64_t)rows + (uint64_t)row;
+    float d = hessian_inv[d_idx];  // H diagonal
     float w = weights[idx];
     error[idx] = (w - q) / d;
 }
 
 void fused_quantize_adjust_cuda
 (
     const float*    weights,
@@ -181,39 +182,40 @@
     int column = blockIdx.x * blockDim.x + threadIdx.x;
     int row = blockIdx.y * blockDim.y + threadIdx.y;
     if (column >= columns) return;
     if (row >= rows) return;
 
     // Quantize
 
-    float x = input[row * columns + column];
+    uint64_t idx = (uint64_t)row * (uint64_t)columns + (uint64_t)column;
+    float x = input[idx];
     float s = scale[column];
     x /= s;
     x = rintf(x);
     x += qzero;
     x = clamp(x, 0.0f, maxq);
 
     // Optionally save quant
 
     if (out_q)
     {
         uint16_t q = static_cast<uint16_t>(x);
-        out_q[row * columns + column] = q;
+        out_q[idx] = q;
     }
 
     half h_s = __float2half_rn(s);
     half h_x = __float2half_rn(x);
     half h_qzero = __float2half_rn(qzero);
 
     h_x = __hsub(h_x, h_qzero);
     h_x = __hmul(h_x, h_s);
 
     // Dequantize
 
-    output[row * columns + column] = __half2float(h_x);
+    output[idx] = __half2float(h_x);
 }
 
 void quantize_cuda
 (
     const float* input,
     float* output,
     const float* scale,
@@ -302,16 +304,17 @@
     int row = blockIdx.y * blockDim.y + threadIdx.y;
     if (column >= columns) return;
     if (row >= rows) return;
 
     float clamp_min = -qzero;
     float clamp_max = maxq - qzero;
 
+    uint64_t idx = (uint64_t)row * (uint64_t)columns + (uint64_t)column;
     float4 sc4 = *((float4*) (scale + column));
-    float4 w4 = *((float4*) (input + row * columns + column));
+    float4 w4 = *((float4*) (input + idx));
 
     for (int i = 0; i <= p_grid; i++)
     {
         float pi = __int2float_rn(i) / __int2float_rn(p_grid);
         float p = min_p * (1.0f - pi) + max_p * pi;
 
         float4 s4 = sc4;
@@ -378,15 +381,15 @@
 )
 {
     int y_idx = (blockIdx.x * blockDim.x + threadIdx.x) * 4;
     int x_idx = blockIdx.y * blockDim.y + threadIdx.y;
     if (y_idx >= y_size) return;
     if (x_idx >= x_size) return;
 
-    int z_idx = y_size * x_idx + y_idx;
+    uint64_t z_idx = (uint64_t)y_size * (uint64_t)x_idx + (uint64_t)y_idx;
 
     float vx = x[x_idx];
     float4 vy = *((float4*) (y + y_idx));
     float4 vz = *((float4*) (z + z_idx));
     vz.x -= vy.x * vx;
     vz.y -= vy.y * vx;
     vz.z -= vy.z * vx;
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/quantize.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rms_norm.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rope.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/rope.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cu` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/util.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cuh` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/cuda/util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_bindings.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     m.def("apply_rep_penalty", &apply_rep_penalty, "apply_rep_penalty");
     m.def("sample_basic", &sample_basic, "sample_basic");
     m.def("logit_filter_exclusive", &logit_filter_exclusive, "logit_filter_exclusive");
     m.def("fast_fill_cpu_ones_bool", &fast_fill_cpu_ones_bool, "fast_fill_cpu_ones_bool");
     m.def("fast_fadd_cpu", &fast_fadd_cpu, "fast_fadd_cpu");
     m.def("fast_copy_cpu", &fast_copy_cpu, "fast_copy_cpu");
     m.def("dump_profile_results", &dump_profile_results, "dump_profile_results");
+    m.def("partial_strings_match", &partial_strings_match, "partial_strings_match");
 
     // safetensors
 
     m.def("safetensors_open", &safetensors_open, "safetensors_open");
     m.def("safetensors_close", &safetensors_close, "safetensors_close");
     m.def("safetensors_load", &safetensors_load, "safetensors_load");
     m.def("safetensors_pinned_buffer", &safetensors_pinned_buffer, "safetensors_pinned_buffer");
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_cache.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_cache.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_gemm.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_gemm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_hadamard.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_hadamard.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_norm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_norm.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qattn.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     int max_rows,
     int hidden_size,
     int num_heads,
     int num_kv_heads,
     int head_dim,
     int max_seq_len,
     bool has_residual,
-    bool neox_style,
+    int rope_style,
     torch::Tensor q_norm,
     torch::Tensor k_norm
 )
 {
     QMatrix* qm_q_proj = reinterpret_cast<QMatrix*> (q_q_proj);
     QMatrix* qm_k_proj = reinterpret_cast<QMatrix*> (q_k_proj);
     QMatrix* qm_v_proj = reinterpret_cast<QMatrix*> (q_v_proj);
@@ -72,15 +72,15 @@
         max_rows,
         hidden_size,
         num_heads,
         num_kv_heads,
         head_dim,
         max_seq_len,
         has_residual,
-        neox_style,
+        rope_style,
         (half*) q_norm.is_meta() ? NULL : (half*) q_norm.data_ptr(),
         (half*) k_norm.is_meta() ? NULL : (half*) k_norm.data_ptr()
     );
 
     return reinterpret_cast<uintptr_t> (attn);
 }
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qattn.h`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     int max_rows,
     int hidden_size,
     int num_heads,
     int num_kv_heads,
     int head_dim,
     int max_seq_len,
     bool has_residual,
-    bool neox_style,
+    int rope_style,
     torch::Tensor q_norm,
     torch::Tensor k_norm
 );
 
 void free_q_attn
 (
     uintptr_t handle
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmatrix.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmatrix.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmlp.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_qmlp.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_quant.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_quant.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_rope.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_rope.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.cpp` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_sampling.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #define _mm_malloc(a, b) _aligned_malloc(a, b)
 #define _mm_free(a) _aligned_free(a)
 #endif
 
 #include "config.h"
 #include "ext_sampling.h"
 
+#include "cpp/generator.h"
 #include "cpp/sampling.h"
 
 #include "cpp/util.h"
 
 void apply_rep_penalty
 (
     torch::Tensor sequence,
```

### Comparing `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.h` & `exl2conv-0.0.21/exl2conv/exl2conv_ext/ext_sampling.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+#include "cpp/generator.h"
+
 void apply_rep_penalty
 (
     torch::Tensor sequence,
     float penalty_max,
     int sustain,
     int decay,
     float alpha_frequency,
```

### Comparing `exl2conv-0.0.20/exl2conv/ext.py` & `exl2conv-0.0.21/exl2conv/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         "cuda/comp_units/unit_exl2_1b.cu",
         "cuda/comp_units/unit_exl2_2a.cu",
         "cuda/comp_units/unit_exl2_2b.cu",
         "cuda/comp_units/unit_exl2_3a.cu",
         "cuda/comp_units/unit_exl2_3b.cu",
         "cpp/quantize_func.cpp",
         "cpp/profiling.cpp",
+        "cpp/generator.cpp",
         "cpp/sampling.cpp",
         "cpp/sampling_avx2.cpp",
         "cpp/safetensors.cpp"
     ]
 
     sources = [os.path.join(sources_dir, s) for s in sources_]
```

### Comparing `exl2conv-0.0.20/exl2conv/fasttensors.py` & `exl2conv-0.0.21/exl2conv/fasttensors.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,18 @@
 
         if keymap:
             self.tensor_remap = {}
             nheader = {}
             for key in self.header.keys():
                 nkey = key
                 for z in keymap:
-                    nkey = nkey.replace(z[0], z[1])
+                    if z[0].startswith("$") and nkey.startswith(z[0][1:]):
+                        nkey = ("$" + nkey).replace(z[0], z[1])
+                    else:
+                        nkey = nkey.replace(z[0], z[1])
                 nheader[nkey] = self.header[key]
                 self.tensor_remap[nkey] = key
             self.header = nheader
 
         if fast and os.name == "nt":
             print(" !! Warning, fasttensors disabled on Windows")
             fast = False
@@ -172,15 +175,15 @@
                    key: str,
                    device,
                    not_fast: bool = False,
                    cached: bool = False,
                    out_dtype = None) -> torch.Tensor:
         global global_tensorcache
 
-        if self.tensor_remap:
+        if self.tensor_remap and (not_fast or not self.fast):
             key = self.tensor_remap[key]
 
         if cached:
             cachekey = self.filename + "::" + key + "::" + device
             for (k, v) in global_tensorcache:
                 if k == cachekey: return v
```

### Comparing `exl2conv-0.0.20/exl2conv/generator/base.py` & `exl2conv-0.0.21/exl2conv/generator/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/generator/filters/base.py` & `exl2conv-0.0.21/exl2conv/generator/filters/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/generator/filters/prefix.py` & `exl2conv-0.0.21/exl2conv/generator/filters/prefix.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/generator/filters/select.py` & `exl2conv-0.0.21/exl2conv/generator/filters/select.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/generator/ngram.py` & `exl2conv-0.0.21/exl2conv/generator/ngram.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/generator/sampler.py` & `exl2conv-0.0.21/exl2conv/generator/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     @staticmethod
     def sample(logits: torch.tensor,
                settings: Settings,
                sequence_ids: torch.tensor,
                random: float,
                tokenizer: ExLlamaV2Tokenizer,
                prefix_token: torch.Tensor | None = None,
-               return_top_tokens: int = 0):
+               return_top_tokens: int = 0,
+               blocked_tokens: list[int] | None = None):
         """
         Sample tokens from (batched) logits tensor
 
         :param logits:
             Input logits, float tensor of shape (batch_size, 1, vocab_size)
 
         :param settings:
@@ -118,14 +119,17 @@
         :param prefix_token:
             Tensor of shape (batch_size, 1). If provided, sampling will be restricted to token pieces that begin with
             this token. Used for token healing.
 
         :param return_top_tokens:
             Number of top tokens to return
 
+        :param blocked_tokens:
+            List of tokens to ban temporarily
+
         :return:
             Tuple of:
             - Sampled tokens, tensor of shape (batch_size, 1)
             - Top candidates per token (batch_size, 1, return_top_tokens), or meta tensor if return_top_tokens = 0
             - Top probs per token (batch_size, 1, return_top_tokens), or meta tensor if return_top_tokens = 0
             - Probabilities per token, shape (batch_size, 1)
             - True if the current filter has reached a stop condition
@@ -164,14 +168,19 @@
                                     settings.token_repetition_penalty,
                                     settings.token_repetition_range,
                                     settings.token_repetition_decay,
                                     settings.token_frequency_penalty,
                                     settings.token_presence_penalty,
                                     logits)
 
+        # Temporarily ban individual tokens
+
+        if blocked_tokens:
+            logits[:, blocked_tokens] = -1e30
+
         # Token bias
 
         if settings.token_bias is not None:
             # logits = logits + settings.token_bias
             ext_c.fast_fadd_cpu(logits, settings.token_bias)
 
         # Evaluate filters
```

### Comparing `exl2conv-0.0.20/exl2conv/generator/streaming.py` & `exl2conv-0.0.21/exl2conv/generator/streaming.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     ExLlamaV2BaseGenerator
 )
 from exl2conv.generator.ngram import NgramCache
 import torch
 import random
 import threading
 from exl2conv.generator.hooks import ExLlamaV2PostSamplingHook, ExLlamaV2PostSamplingResult
+from exl2conv.embedding import EMBEDDING_INDEX
+from exl2conv.ext import exl2conv_ext as ext_c, none_tensor
+import numpy as np
 
 class ExLlamaV2StreamingGenerator(ExLlamaV2BaseGenerator):
 
     # Constants
 
     tail_decode_tokens: int = 2
     max_fallback_tokens: int = 4
@@ -38,18 +41,21 @@
 
     return_probabilities: bool
     return_top_tokens: int
     return_logits: bool
 
     position_offsets: torch.Tensor | None
     input_mask: torch.Tensor | None
+    indexed_embeddings: torch.Tensor | None
 
     # Stop conditions
 
     stop_strings: set
+    stop_strings_utf32_buffer: np.array or None
+    stop_strings_utf32_offsets: np.array or None
     stop_tokens: set
     remaining_tokens: int
 
     # Speculative decoding
 
     future_logits: torch.Tensor | None
     future_tokens: torch.Tensor | None
@@ -99,29 +105,43 @@
 
     active_loras: list[ExLlamaV2Lora]
 
     # Extra decoding options
 
     decode_special_tokens: bool
 
+    # Banned strings
+
+    banned_strings: list[str]
+    banned_strings_utf32_buffer: np.array or None
+    banned_strings_utf32_offsets: np.array or None
+    ban_checkpoint: dict | None
+    blocked_tokens: list[int]
+    blocked_position: int
+    current_blocked_tokens: list[int]
+    reuse_logits: torch.Tensor | None
+
 
     def __init__(self, model, cache, tokenizer, draft_model = None, draft_cache = None, num_speculative_tokens = 5):
         super().__init__(model, cache, tokenizer)
 
         # Stop conditions
 
         self.stop_strings = set()
+        self.stop_strings_utf32_buffer = None
+        self.stop_strings_utf32_offsets = None
         self.stop_tokens = {tokenizer.eos_token_id,}
         self.remaining_tokens = 0
 
         # Generation settings
 
         self.return_probabilities = False
         self.return_top_tokens = 0
         self.return_logits = False
+        self.indexed_embeddings = None
 
         # Speculative decoding
 
         self.future_logits = None
         self.future_tokens = None
 
         self.total_draft_tokens = 0
@@ -161,14 +181,25 @@
         self.held_fallback_tokens = None
         self.expect_utf8: int = 0
 
         # Token healing
 
         self.active_loras = []
 
+        # Banned strings
+
+        self.banned_strings = []
+        self.banned_strings_utf32_buffer = None
+        self.banned_strings_utf32_offsets = None
+        self.ban_checkpoint = None
+        self.blocked_tokens = []
+        self.blocked_position = 0
+        self.current_blocked_tokens = []
+        self.reuse_logits = None
+
 
     def set_stop_conditions(self,
                             stop_conditions: list | tuple | set):
         """
         :param stop_conditions:
             List of either token IDs or strings that will cause stream_ex to emit the EOS signal. String values do not
             have to match whole tokens and can span multiple tokens.
@@ -179,26 +210,29 @@
 
         self.stop_strings = set()
         self.stop_tokens = set()
         for t in stop_conditions:
             if isinstance(t, int): self.stop_tokens.add(t)
             elif isinstance(t, str): self.stop_strings.add(t)
             else: raise ValueError("Unsupported type in stop_conditions")
+        self.stop_strings_utf32_buffer, self.stop_strings_utf32_offsets = \
+            self.strings_to_utf32(list(self.stop_strings))
 
 
     # Legacy function
 
     def begin_stream(self,
                      input_ids: torch.Tensor,
                      gen_settings: ExLlamaV2Sampler.Settings,
                      token_healing: bool = False,
                      loras: ExLlamaV2Lora | list[ExLlamaV2Lora] = None,
                      input_mask: torch.Tensor | None = None,
                      position_offsets: torch.Tensor | None = None,
-                     abort_event: threading.Event = None):
+                     abort_event: threading.Event = None,
+                     **kwargs):
         """
         See ExLlamaV2StreamingGenerator.begin_stream_ex
         """
 
         self.begin_stream_ex(input_ids,
                              gen_settings,
                              token_healing,
@@ -217,15 +251,18 @@
                         loras: ExLlamaV2Lora | list[ExLlamaV2Lora] = None,
                         input_mask: torch.Tensor | None = None,
                         position_offsets: torch.Tensor | None = None,
                         return_probabilities: bool = False,
                         return_top_tokens: int = 0,
                         return_logits: bool = False,
                         abort_event: threading.Event = None,
-                        decode_special_tokens: bool = False):
+                        input_embeddings: torch.Tensor | None = None,
+                        decode_special_tokens: bool = False,
+                        banned_strings: list[str] | None = None,
+                        **kwargs):
         """
         Resets the generator and starts a new completion of the supplied input_ids. Reuses the existing
         cache for any token IDs matching the previous sequence.
 
         :param input_ids:
             Input token ID sequence, as produced by ExLlamaV2Tokenizer. Streaming generator does not
             currently support batch size > 1 except when performing CFG, in which case batch size
@@ -256,16 +293,27 @@
 
         :param return_logits:
             Return the raw logits output by the model for each streamed token
 
         :param abort_event:
             Forwarded to the model during generation. Will abort prefill/context ingestion if triggered.
 
+        :param input_embeddings:
+            Tensor of shape (batch_size, n, hidden_size) added to the beginning of the prompt. Batching
+            is not supported when passing input embeddings unless all prompts are the same. Prompt must
+            contain the string `{{EMBED_HERE}}` to indicate where embeddings are to be inserted.
+
         :param decode_special_tokens:
             Also decode special tokens into output text stream
+
+        :param banned_strings:
+            List of strings that the generator will refuse to output. As soon as a partial match happens,
+            a checkpoint is saved that the generator can rewind to if need be. Subsequent tokens are then
+            held until the full string is resolved (match or no match) and either emitted or discarded,
+            accordingly. Strings are case-insensitive.
         """
 
         self.return_probabilities = return_probabilities
         self.return_top_tokens = return_top_tokens
         self.return_logits = return_logits
 
         self.abort_event = abort_event
@@ -278,14 +326,16 @@
 
         self.position_offsets = position_offsets
         self.input_mask = input_mask
 
         if loras is not None and isinstance(loras, ExLlamaV2Lora): loras = [loras]
         self.active_loras = loras
 
+        self.indexed_embeddings = input_embeddings
+
         # Decluttering
 
         self.no_logits = torch.empty((0, ((self.model.config.vocab_size + 31) // 32) * 32), dtype = torch.float)
         self.no_tokens = torch.empty((1, 0), dtype = torch.long)
         self.no_probs = torch.empty((1, 0), dtype = torch.float)
         self.no_ptokens = torch.empty((1, 0, self.return_top_tokens), dtype = torch.long)
         self.no_pprobs = torch.empty((1, 0, self.return_top_tokens), dtype = torch.float)
@@ -299,33 +349,81 @@
         self.expect_utf8 = 0
         self.held_tokens = self.no_tokens
         self.held_ptokens = self.no_ptokens
         self.held_probs = self.no_probs
         self.held_pprobs = self.no_pprobs
         self.held_logits = self.no_logits
         self.settings = gen_settings
-        self._gen_begin_reuse(input_ids, gen_settings)
 
+        # Ingest prompt
+
+        assert input_embeddings is None or self.draft_model is None, \
+            "Can not use input embeddings with draft model"
+
+        self._gen_begin_reuse(input_ids, gen_settings)
         self.heal_next_token = (token_healing and self.sequence_ids.shape[-1] >= 2)
 
+        # Remove indexed embeddings from generator's sequence
+
+        if input_embeddings is not None:
+            self.sequence_ids[self.sequence_ids >= EMBEDDING_INDEX] = self.tokenizer.pad_token_id
+
         # Initialize n-gram cache
 
         if self.speculative_ngram:
             self.ngram = NgramCache(self.speculative_ngram_min,
                                     self.speculative_ngram_max,
                                     self.ngram_preloaded)
             self.ngram.update(self.sequence_ids[0].tolist())
 
+        # Banned strings
+
+        if banned_strings is None: banned_strings = []
+        self.banned_strings = [s.lower() for s in banned_strings]
+        self.banned_strings_utf32_buffer, self.banned_strings_utf32_offsets = \
+            self.strings_to_utf32(self.banned_strings)
+
+        self.ban_checkpoint = None
+        self.blocked_tokens = []
+        self.blocked_position = -1
+        self.current_blocked_tokens = []
+        self.reuse_logits = None
+
+
+    # Convert list of strings to UTF32 format needed, to pass by reference to partial matching function
+
+    def strings_to_utf32(self, strings: list[str]) -> (np.array, list[int]):
+
+        if not strings: return bytearray(), None
+
+        encoded_strings = [s.encode("utf-32-le") for s in strings]
+        encoded_lengths = [len(s) for s in encoded_strings]
+        offsets = [0] + encoded_lengths
+        for i in range(1, len(offsets)):
+            offsets[i] += offsets[i - 1]
+        total_length = offsets[-1]
+        concat_strings = bytearray(total_length)
+        for s, offset in zip(encoded_strings, offsets[:-1]):
+            concat_strings[offset:offset + len(s)] = s
+
+        concat_strings = np.frombuffer(concat_strings, dtype = np.uint8)
+        offsets = np.frombuffer(np.array(offsets, dtype = np.int32), dtype = np.uint8)
+        return concat_strings, offsets
+
 
     # Get the next chunk of text in the stream
 
-    def stream_ex(self):
+    def stream_ex(self, ban_tokens: list[int] | None = None, **kwargs):
         """
-        Perform one streaming iteration, returning one chunk of text. Returns a dict with the following
-        entries:
+        Perform one streaming iteration, returning one chunk of text.
+
+        :param ban_tokens:
+            List of tokens to disallow for this iteration only.
+
+        Returns a dict with the following entries:
 
             chunk:
                 Decoded output text. May be an empty string if the generator holds text to resolve a
                 stop condition.
 
             eos:
                 Boolean EOS signal. True if one of the specified stop conditions has been met
@@ -349,15 +447,17 @@
                 final sampling stage. If less than k tokens were candidates, the list will be padded with
                 zero-probability tokens whose order is undefined.
 
             return_logits: (if return_logits == True)
                 Raw output logits for the model, shape (1, n, vocab_size)
         """
 
-        chunk, eos, chunk_token_ids, probs, ptokens, pprobs, logits = self._stream()
+        chunk, eos, chunk_token_ids, probs, ptokens, pprobs, logits, extra = self._stream(
+            ban_tokens = ban_tokens
+        )
 
         ret = { "chunk": chunk,
                 "eos": eos,
                 "chunk_token_ids": chunk_token_ids }
 
         if self.return_probabilities:
             ret["probs"] = probs
@@ -365,42 +465,50 @@
         if self.return_top_tokens > 0:
             ret["top_probs"] = pprobs
             ret["top_tokens"] = ptokens
 
         if self.return_logits:
             ret["logits"] = logits.unsqueeze(0)
 
+        if extra:
+            ret.update(extra)
+
         return ret
 
 
     # Legacy function
 
-    def stream(self) -> Union[Tuple[str, bool, torch.Tensor],
-                              Tuple[str, bool, torch.Tensor, torch.Tensor],
-                              Tuple[str, bool, torch.Tensor, torch.Tensor, torch.Tensor]]:
+    def stream(self, **kwargs) -> Union[Tuple[str, bool, torch.Tensor],
+                                  Tuple[str, bool, torch.Tensor, torch.Tensor],
+                                  Tuple[str, bool, torch.Tensor, torch.Tensor, torch.Tensor]]:
         """
         Legacy functions that returns a tuple rather than a dict. See ExLlamaV2StreamingGenerator.stream_ex
         """
 
         assert self.return_top_tokens == 0, "Use stream_ex() to return top K probs"
 
-        chunk, eos, chunk_token_ids, probs, _, _, logits = self._stream()
+        chunk, eos, chunk_token_ids, probs, _, _, logits, _ = self._stream()
         ret = [chunk, eos, chunk_token_ids]
 
         if self.return_probabilities:
             ret.append(probs)
 
         if self.return_logits:
             ret.append(logits)
         
         return tuple(ret)
 
 
-    # @profile
-    def _stream(self) -> (str, bool, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor):
+    def _stream(self, ban_tokens: list[str] | None = None) -> (str, bool, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict | None):
+
+        # Blocked/banned tokens
+
+        self.current_blocked_tokens = [] if ban_tokens is None else ban_tokens
+        if self.cache.current_seq_len == self.blocked_position:
+            self.current_blocked_tokens += self.blocked_tokens
 
         # Token healing
 
         if self.heal_next_token:
 
             # Pop the last token
 
@@ -415,42 +523,42 @@
             if self.first_token:
 
                 self.settings.begin_filters(self.tokenizer.get_id_to_piece_list(self.decode_special_tokens)[last_token])
                 self.first_token = False
 
             # Regenerate the last token again, with prefix
 
-            healed_token, _, _, _, eos, logits = self._gen_single_token(self.settings, prefix_token = last_token)
+            healed_token, _, _, _, eos, logits, dev_logits = self._gen_single_token(self.settings, prefix_token = last_token)
             new_tail = self.tokenizer.decode(self.sequence_ids[:, -self.tail_decode_tokens:],
                                              decode_special_tokens = self.decode_special_tokens)[0]
             self.held_text += new_tail[len(old_tail):]
 
             self.heal_next_token = False
 
             # In case we only needed the healed token
 
-            if eos: return self.held_text, True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits
+            if eos: return self.held_text, True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits, None
 
         # Start filters when not healing
 
         else:
 
             if self.first_token:
 
                 self.settings.begin_filters()
                 self.first_token = False
 
         # Generate a single token and append to the sequence
 
-        next_token, next_ptokens, next_pprobs, next_prob, eos, next_logits = self._gen_single_token(self.settings)
+        next_token, next_ptokens, next_pprobs, next_prob, eos, next_logits, dev_logits = self._gen_single_token(self.settings)
 
         # End immediately if it was a stop token
 
         if next_token.item() in self.stop_tokens:
-            return self.held_text, True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits
+            return self.held_text, True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits, None
 
         id_to_piece = self.tokenizer.get_id_to_piece_list(self.decode_special_tokens)
         new_text = id_to_piece[next_token]
 
         next_token, new_text = self._catch_utf8(next_token, new_text)
         next_token, new_text = self._catch_fallback(next_token, new_text)
 
@@ -462,54 +570,96 @@
             self.held_ptokens = torch.cat([self.held_ptokens, next_ptokens], dim = 1)
             self.held_pprobs = torch.cat([self.held_pprobs, next_pprobs], dim = 1)
         if self.return_logits:
             self.held_logits = torch.cat([self.held_logits, next_logits], dim = 0)
 
         # Return now if newly added token ends a filter
 
-        if eos: return self.held_text, True, self.held_tokens, self.held_probs, self.held_ptokens, self.held_pprobs, self.held_logits
-
-        # Hold text as long as it contains part of a stop string
-
-        partial_ss = False
-        for ss in self.stop_strings:
-
-            # Check if held_text fully contains stop string
-
-            position = self.held_text.find(ss)
-            if position != -1:
-                return self.held_text[:position], True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits
-
-            # Check for overlap between end of held_text and start of stop string
-
-            overlap = 0
-            for j in range(1, min(len(self.held_text), len(ss)) + 1):
-                if self.held_text[-j:] == ss[:j]: overlap = j
-            if overlap > 0: partial_ss = True
+        if eos: return self.held_text, True, self.held_tokens, self.held_probs, self.held_ptokens, self.held_pprobs, self.held_logits, None
 
-        # If holding text because of a partial stop condition, return nothing but also EOS = False
-
-        if partial_ss:
-            return "", False, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits
-
-        # No stop condition, so return whatever is being held
+        # Hold text as long as it contains part of a banned string
 
+        def set_checkpoint():
+            self.ban_checkpoint = {
+                "position": self.cache.current_seq_len - 1,
+                "held_text": self.held_text[:-len(new_text)],
+                "held_tokens": self.held_tokens[:, :-1],
+                "held_probs": self.held_probs[:, :-1],
+                "held_ptokens": self.held_ptokens[:, :-1, :],
+                "held_pprobs": self.held_pprobs[:, :-1, :],
+                "held_logits": self.held_logits[:-1, :],
+                "offending_token": next_token,
+                "next_logits": dev_logits
+            }
+            self.blocked_position = self.cache.current_seq_len - 1
+
+        def rewind_checkpoint():
+            cp = self.ban_checkpoint
+            self.sequence_ids = self.sequence_ids[:, :cp["position"]+1]
+            self.cache.current_seq_len = cp["position"]
+            off_text = self.held_text[len(cp["held_text"]):]
+            self.held_text = cp["held_text"]
+            self.held_tokens = cp["held_tokens"]
+            self.held_probs = cp["held_probs"]
+            self.held_ptokens = cp["held_ptokens"]
+            self.held_pprobs = cp["held_pprobs"]
+            self.held_logits = cp["held_logits"]
+            self.future_logits = None
+            self.future_tokens = None
+            self.ban_checkpoint = None
+            self.reuse_logits = cp["next_logits"]
+            return cp["offending_token"], off_text
+
+        if self.banned_strings_utf32_offsets is not None:
+            match = ext_c.partial_strings_match(
+                np.frombuffer(self.held_text.lower().encode("utf-32-le"), dtype = np.uint8),
+                self.banned_strings_utf32_offsets,
+                self.banned_strings_utf32_buffer
+            )
+            if match >= 0:
+                if self.ban_checkpoint is None: set_checkpoint()
+                offending_token, offending_text = rewind_checkpoint()
+                self.blocked_tokens.append(offending_token.item())
+                extra_ret = { "suppressed": offending_text }
+                return "", False, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits, extra_ret
+            if match == -2:
+                if self.ban_checkpoint is None: set_checkpoint()
+                return "", False, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits, None
+
+        # Check for stop strings and hold text as long as it contains part of a stop string
+
+        if self.stop_strings_utf32_offsets is not None:
+            match = ext_c.partial_strings_match(
+                np.frombuffer(self.held_text.encode("utf-32-le"), dtype = np.uint8),
+                self.stop_strings_utf32_offsets,
+                self.stop_strings_utf32_buffer
+            )
+            if match >= 0:
+                return self.held_text[:match], True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits, None
+            if match == -2:
+                return "", False, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits, None
+
+        # No stop condition or banned string, so clear checkpoint and return whatever is being held
+
+        self.ban_checkpoint = None
+        self.blocked_tokens = []
+        self.blocked_position = -1
         stream_text = self.held_text
         stream_tokens = self.held_tokens
         stream_probs = self.held_probs
         stream_ptokens = self.held_ptokens
         stream_pprobs = self.held_pprobs
         stream_logits = self.held_logits
         self.held_text = ""
         self.held_tokens = self.no_tokens
         self.held_probs = self.no_probs
         self.held_ptokens = self.no_ptokens
         self.held_pprobs = self.no_pprobs
         self.held_logits = self.no_logits
-        return stream_text, False, stream_tokens, stream_probs, stream_ptokens, stream_pprobs, stream_logits
+        return stream_text, False, stream_tokens, stream_probs, stream_ptokens, stream_pprobs, stream_logits, None
 
 
     # Functions for catching and holding partial UTF-8 characters
 
     def _decode_utf8(self):
 
         if self.held_utf8_tokens.shape[-1] == 0: return self.no_tokens, ""
@@ -598,15 +748,16 @@
         self.cache.current_seq_len = 0
         self.model.forward(self.sequence_ids[:, :-1],
                            self.cache,
                            preprocess_only = True,
                            loras = self.active_loras,
                            input_mask = self.input_mask,
                            position_offsets = self.position_offsets,
-                           abort_event = self.abort_event)
+                           abort_event = self.abort_event,
+                           indexed_embeddings = self.indexed_embeddings)
         if self.abort_event and self.abort_event.is_set():
             self._truncate_seq_to_cache()
             return
 
         if self.draft_model is not None:
             self.draft_cache.current_seq_len = 0
             self.draft_model.forward(self.sequence_ids[:1, :-1],
@@ -672,15 +823,16 @@
 
         self.model.forward(self.sequence_ids[:, start : -1],
                            self.cache,
                            preprocess_only = True,
                            loras = self.active_loras,
                            input_mask = self.input_mask,
                            position_offsets = self.position_offsets,
-                           abort_event = self.abort_event)
+                           abort_event = self.abort_event,
+                           indexed_embeddings = self.indexed_embeddings)
         if self.abort_event and self.abort_event.is_set():
             self._truncate_seq_to_cache()
             return
 
         if self.draft_model is not None:
             self.draft_model.forward(self.sequence_ids[:, start: -1],
                                      self.draft_cache,
@@ -698,36 +850,49 @@
     # Generate a single token and append to sequence
 
     def _gen_single_token(self, gen_settings, prefix_token = None):
 
         if self.speculative_ngram:
 
             token, ptokens, pprobs, prob, eos, logits = self._gen_single_token_ngram(gen_settings, prefix_token)
+            dev_logits = None
 
         elif self.draft_model is None:
 
-            logits = self.model.forward(self.sequence_ids[:, -1:],
-                                        self.cache,
-                                        loras = self.active_loras,
-                                        input_mask = self.input_mask,
-                                        position_offsets = self.position_offsets).float().cpu()
-
-            token, ptokens, pprobs, prob, eos = \
-                ExLlamaV2Sampler.sample(logits,
-                                        gen_settings,
-                                        self.sequence_ids[:1, :],
-                                        random.random(),
-                                        self.tokenizer,
-                                        prefix_token,
-                                        self.return_top_tokens)
+            if self.reuse_logits is not None:
+                dev_logits = self.reuse_logits
+                self.reuse_logits = None
+                self.cache.current_seq_len += 1
+                logits = dev_logits.float().cpu()
+            else:
+                dev_logits = self.model.forward(
+                    self.sequence_ids[:, -1:],
+                    self.cache,
+                    loras = self.active_loras,
+                    input_mask = self.input_mask,
+                    position_offsets = self.position_offsets
+                )
+                logits = dev_logits.float().cpu()
+
+            token, ptokens, pprobs, prob, eos = ExLlamaV2Sampler.sample(
+                logits,
+                gen_settings,
+                self.sequence_ids[:1, :],
+                random.random(),
+                self.tokenizer,
+                prefix_token,
+                self.return_top_tokens,
+                blocked_tokens = self.current_blocked_tokens
+            )
 
         else:
 
             token, ptokens, pprobs, prob, eos, logits = \
                 self._gen_single_token_speculative(gen_settings, prefix_token)
+            dev_logits = None
 
         # Post sampling hook
 
         if gen_settings.post_sampling_hooks:
             p = ExLlamaV2PostSamplingResult(
                 sampled_token = token,
                 sampled_prob = prob,
@@ -747,15 +912,15 @@
         # Accept token
         
         if self.sequence_ids.shape[0] > 1 and token.shape[0] == 1:
             self.sequence_ids = torch.cat([self.sequence_ids, token.repeat(self.sequence_ids.shape[0], 1)], dim = 1)
         else:
             self.sequence_ids = torch.cat([self.sequence_ids, token], dim = 1)
         
-        return token, ptokens, pprobs, prob, eos, logits.flatten(1)
+        return token, ptokens, pprobs, prob, eos, logits.flatten(1), dev_logits
 
 
     # Speculative decoding with draft model
 
     def _gen_single_token_speculative(self, gen_settings, prefix_token = None):
 
         if self.future_tokens is None:
@@ -802,15 +967,23 @@
             # Rewind model cache
 
             self.cache.current_seq_len -= num_drafted_tokens + 1
 
         # Sample the first future logits
 
         logits = self.future_logits[:, :1, :]
-        token, ptokens, pprobs, prob, eos = ExLlamaV2Sampler.sample(logits, gen_settings, self.sequence_ids[:1, :], random.random(), self.tokenizer, prefix_token, self.return_top_tokens)
+        token, ptokens, pprobs, prob, eos = ExLlamaV2Sampler.sample(
+            logits,
+            gen_settings,
+            self.sequence_ids[:1, :], random.random(),
+            self.tokenizer,
+            prefix_token,
+            self.return_top_tokens,
+            blocked_tokens = self.current_blocked_tokens
+        )
         self.future_logits = self.future_logits[:, 1:, :]
         self.future_tokens = self.future_tokens[:, 1:]
         self.cache.current_seq_len += 1
         self.draft_cache.current_seq_len += 1
 
         # If sampled token doesn't match future token or no more future tokens
 
@@ -854,15 +1027,24 @@
 
             self.cache.current_seq_len -= len(inf_ids)
             self.total_draft_tokens += len(inf_ids) - 1
 
         # Sample the first future logits
 
         logits = self.future_logits[:, :1, :]
-        token, ptokens, pprobs, prob, eos = ExLlamaV2Sampler.sample(logits, gen_settings, self.sequence_ids[:1, :], random.random(), self.tokenizer, prefix_token, self.return_top_tokens)
+        token, ptokens, pprobs, prob, eos = ExLlamaV2Sampler.sample(
+            logits,
+            gen_settings,
+            self.sequence_ids[:1, :],
+            random.random(),
+            self.tokenizer,
+            prefix_token,
+            self.return_top_tokens,
+            blocked_tokens = self.current_blocked_tokens
+        )
         self.future_logits = self.future_logits[:, 1:, :]
         self.future_tokens = self.future_tokens[:, 1:]
         self.cache.current_seq_len += 1
 
         # Update predictor
 
         tail_ids = self.sequence_ids[0, -(self.speculative_ngram_max - 1):].tolist() + [token.item()]
```

### Comparing `exl2conv-0.0.20/exl2conv/hadamard/hadamard.py` & `exl2conv-0.0.21/exl2conv/hadamard/hadamard.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/hadamard/primes.txt` & `exl2conv-0.0.21/exl2conv/hadamard/primes.txt`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/headnorm.py` & `exl2conv-0.0.21/exl2conv/headnorm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/layernorm.py` & `exl2conv-0.0.21/exl2conv/layernorm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/linear.py` & `exl2conv-0.0.21/exl2conv/linear.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/lora.py` & `exl2conv-0.0.21/exl2conv/lora.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/mlp.py` & `exl2conv-0.0.21/exl2conv/mlp.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/model.py` & `exl2conv-0.0.21/exl2conv/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 import os, sys
+
+from exl2conv.architecture import RopeStyle
+
 min_version = (3, 8)
 if sys.version_info < min_version:
     print("")
     print(f" ## Warning: this project requires Python {min_version[0]}.{min_version[1]} or higher.")
     print("")
 
 # Set CUDA context to lazy loading since we won't need 95% of the modules in Torch
@@ -27,14 +30,15 @@
 from exl2conv.layernorm import ExLlamaV2LayerNorm
 from exl2conv.attn import ExLlamaV2Attention
 from exl2conv.lora import ExLlamaV2Lora
 from exl2conv.mlp import ExLlamaV2MLP
 from exl2conv.moe_mlp import ExLlamaV2MoEMLP
 from exl2conv.parallel_decoder import ExLlamaV2ParallelDecoder
 from exl2conv.embedding import ExLlamaV2Embedding
+from exl2conv.pos_embedding import ExLlamaV2PosEmbedding
 from exl2conv.compat import safe_move_tensor
 from exl2conv.fasttensors import cleanup_stfiles
 # from exl2conv.util import list_live_tensors, print_vram_usage, set_snapshot, diff_snapshot, print_vram_usage_peak
 import gc
 import threading
 from typing import Callable
 
@@ -109,21 +113,26 @@
         scratch_slice = self.scratch.narrow(0, self.scratch_idx, size_half)
         self.scratch_idx += size_half
         return scratch_slice
 
 
     def prepare_sincos(self):
 
+        device = _torch_device(self.device_idx)
+
         cfg = self.model.config
+        if cfg.arch.rope_style == RopeStyle.NONE:
+            self.sin = torch.zeros((1,), device = device, dtype = torch.half)
+            self.cos = self.sin
+            return
 
         base = cfg.rotary_embedding_base
         alpha = cfg.scale_alpha_value or 1.0
         scale = cfg.scale_pos_emb or 1.0
         head_dim = cfg.head_dim
-        device = _torch_device(self.device_idx)
         scaling_factor = 1.0
 
         # Alpha scaling for any rope_scaling type
 
         if alpha != 1.0: base *= alpha ** (cfg.head_dim / (cfg.head_dim - 2))
 
         # "su"
@@ -148,18 +157,20 @@
 
         # Common
 
         t = torch.arange(cfg.max_seq_len, device = device, dtype = torch.float32)
         if scale != 1.0: t /= scale
 
         freqs = torch.einsum("i,j->ij", t, inv_freq)
-        if cfg.arch.rope_neox_style:
+        if cfg.arch.rope_style == RopeStyle.NEOX:
             emb = torch.cat((freqs, freqs), dim=-1)
-        else:
+        elif cfg.arch.rope_style == RopeStyle.GPTJ:
             emb = torch.repeat_interleave(freqs, 2, dim=-1)
+        else:
+            raise ValueError()
 
         self.sin = emb.sin()[None, None, :, :]
         self.cos = emb.cos()[None, None, :, :]
         if scaling_factor != 1.0:
             self.sin *= scaling_factor
             self.cos *= scaling_factor
         self.sin = self.sin.half()
@@ -187,14 +198,18 @@
         self.loaded = False
 
         # Build model
 
         emb = ExLlamaV2Embedding(self, "model.embed_tokens")
         self.modules += [emb]
 
+        if self.config.arch.learned_pos_emb_key:
+            pos_emb = ExLlamaV2PosEmbedding(self, self.config.arch.learned_pos_emb_key)
+            self.modules += [pos_emb]
+
         for layer_idx in range(self.config.num_hidden_layers):
 
             layer_key = f"model.layers.{layer_idx}"
             if self.config.arch.parallel_decoder_blocks:
                 pd = ExLlamaV2ParallelDecoder(self, layer_key, layer_idx)
                 self.modules += [pd]
             else:
@@ -700,20 +715,28 @@
 
             # Limit chunk_size to max_input_len
 
             chunk_size = min(remaining_q_len, effective_max_input_len)
 
             # Limit chunk_size to keep size of attention operation <= max_attention_size
 
-            past_len = cache.current_seq_len
-            attn_size = (past_len + remaining_q_len) * remaining_q_len
-            max_a = self.config.max_attention_size
-            if attn_size > max_a:
-                cs = (math.sqrt(past_len ** 2 + 4 * max_a) - past_len) / 2
-                chunk_size = min(chunk_size, math.floor(cs))
+            if has_flash_attn:
+
+                # Can't measure increase in VRAM usage with longer k_len, assume usage is constant
+                # for given chunk_size
+                pass
+
+            else:
+
+                past_len = cache.current_seq_len
+                attn_size = (past_len + remaining_q_len) * remaining_q_len
+                max_a = self.config.max_attention_size
+                if attn_size > max_a:
+                    cs = (math.sqrt(past_len ** 2 + 4 * max_a) - past_len) / 2
+                    chunk_size = min(chunk_size, math.floor(cs))
 
             # Process chunk
 
             chunk_end = min(chunk_begin + chunk_size, q_len)
 
             # print(f"Forward chunk length: {chunk_end - chunk_begin}")
 
@@ -824,8 +847,9 @@
         # Set padding logits to -inf
 
         if x is not None:
             head_padding = self.modules[-1].padding
             if head_padding > 0:
                 x[:, :, -head_padding:] = -65504.
 
-        return x, last_state
+        return x, last_state
+
```

### Comparing `exl2conv-0.0.20/exl2conv/model_init.py` & `exl2conv-0.0.21/exl2conv/model_init.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/module.py` & `exl2conv-0.0.21/exl2conv/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,48 +119,58 @@
             # Torch
 
             if key + ".weight" in self.model.config.tensor_file_map:
                 if key + ".bias" in self.model.config.tensor_file_map:
                     tensors = self.load_multi(key, ["weight", "bias"])
                     tensor = tensors["weight"].half()
                     bias = tensors["bias"].half()
+                    if self.model.config.arch.orig_weights_transposed and len(tensor.shape) == 2:
+                        tensor = tensor.T
                     return nn.Parameter(tensor), nn.Parameter(bias)
                 else:
                     tensors = self.load_multi(key, ["weight"])
                     tensor = tensors["weight"].half()
+                    # if self.model.config.arch.orig_weights_transposed:
+                    #     tensor = tensor.T
                     return nn.Parameter(tensor)
 
             # No weights found for key
 
         return None
 
 
     def load_weight_fused(self,
                           f_key: str,
                           f_beg: int,
                           f_end: int,
                           in_feat: int,
                           out_feat: int):
 
-        for key in [f_key, f_key + ".weight"]:
+        res = []
+        for key in [f_key, f_key + ".weight", f_key + ".bias"]:
 
             filename = self.model.config.tensor_file_map.get(key)
             if not filename: continue
 
             stfile = STFile.open(filename, fast = self.model.config.fasttensors, keymap = self.model.config.arch.keymap)
             # tensor = stfile.get_tensor(key, device = self.device()).half()
             tensor = stfile.get_tensor(key, device = "cpu", cached = True, out_dtype = torch.half)
-            tensor = tensor[f_beg:f_end, :]
-            if in_feat != out_feat and \
-                tensor.shape[1] == out_feat and \
-                tensor.shape[0] == in_feat:
+            if self.model.config.arch.orig_weights_transposed and len(tensor.shape) == 2:
                 tensor = tensor.T
+            tensor = tensor[f_beg:f_end]
+            if not key.endswith(".bias"):
+                if in_feat != out_feat and \
+                    tensor.shape[1] == out_feat and \
+                    tensor.shape[0] == in_feat:
+                    tensor = tensor.T
             tensor = tensor.contiguous().to(self.device())
-            return nn.Parameter(tensor)
+            res.append(nn.Parameter(tensor))
 
+        if len(res) == 2: return res[0], res[1]
+        if len(res) == 1: return res[0]
         return None
 
 
     def weight_footprint(self) -> int:
 
         if self.footprint == -1:
```

### Comparing `exl2conv-0.0.20/exl2conv/moe_mlp.py` & `exl2conv-0.0.21/exl2conv/moe_mlp.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/parallel_decoder.py` & `exl2conv-0.0.21/exl2conv/parallel_decoder.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/rmsnorm.py` & `exl2conv-0.0.21/exl2conv/rmsnorm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/server/websocket.py` & `exl2conv-0.0.21/exl2conv/server/websocket.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/server/websocket_actions.py` & `exl2conv-0.0.21/exl2conv/server/websocket_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
                 min_p: float,                       # (optional) min-P threshold (0 to disable)
                 typical: float,                     # (optional) typical threshold (0 to disable)
                 temperature: float,                 # (optional) sampling temperature (1.0 = no temp adjust)
                 rep_pen: float,                     # (optional) repetition penalty (1.0 = no penalty)
                 freq_pen: float,                    # (optional) frequency penalty (0.0 = no penalty)
                 pres_pen: float,                    # (optional) presence penalty (0.0 = no penalty)
                 skew: float,                        # (optional) skew factor (0.0 = disabled)
+                customBos: str,                     # (optional) custom BOS token
                 stop_conditions: [str|int],         # (optional) list of stop conditions
                 token_healing: bool,                # (optionsl) enable token healing
                 tag: str }                          # (optional) tag to echo in response packet
 
     streams:  { action: str = "infer",
                 request_id: str,                    # (optional)
                 response_id: str,                   # (optional)
@@ -163,21 +164,32 @@
 
         full_response = request['stream_full'] if 'stream_full' in request else False
         # Tokenize and trim prompt
 
         full_ctx = request["text"]
         num_tokens = request["max_new_tokens"]
 
-        ids = server.tokenizer.cached_encode_str(full_ctx)
+        cb=''
+        if 'customBos' in request:
+            cb = request['customBos']
+        ids = server.tokenizer.cached_encode_str(cb+full_ctx)
         overflow = ids.shape[-1] + num_tokens - server.model.config.max_seq_len
-        if overflow > 0:
-            ids = ids[:, overflow:]
+
+
+        if overflow < 0:
+            util_ctx = cb+full_ctx
+
+        elif 'customBos' in request:
+            ids = ids[:,:1]+ids[:, overflow+1:]
             util_ctx = server.tokenizer.decode(ids)
+
         else:
-            util_ctx = full_ctx
+            ids = ids[:, overflow:]
+            util_ctx = server.tokenizer.decode(ids)
+            
 
         # Sampler
 
         gs = ExLlamaV2Sampler.Settings()
         gs.top_k = int(request["top_k"]) if "top_k" in request else 100
         gs.top_p = float(request["top_p"]) if "top_p" in request else 0.8
         gs.top_a = float(request["top_a"]) if "top_a" in request else 0
```

### Comparing `exl2conv-0.0.20/exl2conv/tokenizer/base.py` & `exl2conv-0.0.21/exl2conv/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/tokenizer/hf.py` & `exl2conv-0.0.21/exl2conv/tokenizer/hf.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/tokenizer/spm.py` & `exl2conv-0.0.21/exl2conv/tokenizer/spm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/tokenizer/tokenizer.py` & `exl2conv-0.0.21/exl2conv/tokenizer/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,20 @@
         self.bos_token = (self.tokenizer_model.bos_token() or self.extended_id_to_piece.get(self.bos_token_id, None)) or self.tokenizer_model.id_to_piece(self.bos_token_id)
         self.eos_token = (self.tokenizer_model.eos_token() or self.extended_id_to_piece.get(self.eos_token_id, None)) or self.tokenizer_model.id_to_piece(self.eos_token_id)
 
         # Use "<pad>" or BOS token as fallback for padding token
 
         if self.pad_token_id is None:
             pad_test = self.tokenizer_model.piece_to_id("<pad>")
-            self.pad_token_id = pad_test or self.bos_token_id
+            if pad_test:
+                self.pad_token_id = pad_test
+            elif self.eos_token_id != self.bos_token_id:
+                self.pad_token_id = self.eos_token_id
+            else:
+                self.pad_token_id = -1
 
         # Special case if <unk> and <pad> have the same ID
 
         if self.unk_token_id == self.pad_token_id:
             self.unk_token = self.pad_token
 
         # Make sure extended vocab contains control tokens, but avoid empty pieces
@@ -245,14 +250,20 @@
             self.get_id_to_piece_list()
             self.get_piece_to_id_dict()
             self.get_prefix_to_ids_dict()
             self.get_prefix_id_to_ids_dict()
             self.get_char_trie()
             self.get_char_trie_ci()
 
+        # Take stock and issue warnings if needed
+
+        if self.pad_token_id == self.bos_token_id:
+            print(" !! Warning: PAD and EOS tokens are identical. Generations might break " + \
+                  "and batch sizes > 1 are unlikely to work correctly.")
+
 
     # Return size of valid vocabulary
 
     def get_vocab_size(self) -> int:
         """
         Get vocab size
 
@@ -443,14 +454,16 @@
             max_token = self.tokenizer_model.vocab_size()
             seq = [t for t in seq if (t != self.pad_token_id and t < max_token and t != self.eos_token_id)]
             if self.eos_token_id in seq: seq = seq[:seq.index(self.eos_token_id)]
             return self.decode_unspecial(seq)
 
         else:
 
+            max_token = self.tokenizer_model.vocab_size()
+            seq = [t for t in seq if (t != self.pad_token_id and t < max_token)]
             text = ""
             start = 0
             end = 0
             while end < len(seq):
                 if seq[end] in self.extended_id_to_piece:
                     if end > start: text += self.tokenizer_model.decode(seq[start : end])
                     text += self.extended_id_to_piece[seq[end]]
```

### Comparing `exl2conv-0.0.20/exl2conv/tokenizer.py` & `exl2conv-0.0.21/exl2conv/tokenizer.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv/util.py` & `exl2conv-0.0.21/exl2conv/util.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.20/exl2conv.egg-info/SOURCES.txt` & `exl2conv-0.0.21/exl2conv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 exl2conv/lora.py
 exl2conv/mlp.py
 exl2conv/model.py
 exl2conv/model_init.py
 exl2conv/module.py
 exl2conv/moe_mlp.py
 exl2conv/parallel_decoder.py
+exl2conv/pos_embedding.py
 exl2conv/rmsnorm.py
 exl2conv/tokenizer.py
 exl2conv/util.py
 exl2conv/version.py
 exl2conv.egg-info/PKG-INFO
 exl2conv.egg-info/SOURCES.txt
 exl2conv.egg-info/dependency_links.txt
@@ -66,14 +67,16 @@
 exl2conv/exl2conv_ext/ext_rope.h
 exl2conv/exl2conv_ext/ext_safetensors.cpp
 exl2conv/exl2conv_ext/ext_safetensors.h
 exl2conv/exl2conv_ext/ext_sampling.cpp
 exl2conv/exl2conv_ext/ext_sampling.h
 exl2conv/exl2conv_ext/cpp/avx2_target.h
 exl2conv/exl2conv_ext/cpp/avx_mathfun.h
+exl2conv/exl2conv_ext/cpp/generator.cpp
+exl2conv/exl2conv_ext/cpp/generator.h
 exl2conv/exl2conv_ext/cpp/profiling.cpp
 exl2conv/exl2conv_ext/cpp/profiling.h
 exl2conv/exl2conv_ext/cpp/quantize_func.cpp
 exl2conv/exl2conv_ext/cpp/quantize_func.h
 exl2conv/exl2conv_ext/cpp/safetensors.cpp
 exl2conv/exl2conv_ext/cpp/safetensors.h
 exl2conv/exl2conv_ext/cpp/sampling.cpp
```

### Comparing `exl2conv-0.0.20/setup.py` & `exl2conv-0.0.21/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,16 @@
                 "exl2conv/exl2conv_ext/cuda/pack_tensor.cu",
                 "exl2conv/exl2conv_ext/cuda/quantize.cu",
                 "exl2conv/exl2conv_ext/cuda/q_matrix.cu",
                 "exl2conv/exl2conv_ext/cuda/q_attn.cu",
                 "exl2conv/exl2conv_ext/cuda/q_mlp.cu",
                 "exl2conv/exl2conv_ext/cuda/q_gemm.cu",
                 "exl2conv/exl2conv_ext/cuda/rms_norm.cu",
-                "exl2conv/exl2conv_ext/cuda/layer_norm.cu",
                 "exl2conv/exl2conv_ext/cuda/head_norm.cu",
+                "exl2conv/exl2conv_ext/cuda/layer_norm.cu",
                 "exl2conv/exl2conv_ext/cuda/rope.cu",
                 "exl2conv/exl2conv_ext/cuda/cache.cu",
                 "exl2conv/exl2conv_ext/cuda/util.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu",
@@ -66,14 +66,15 @@
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu",
                 "exl2conv/exl2conv_ext/cpp/quantize_func.cpp",
                 "exl2conv/exl2conv_ext/cpp/profiling.cpp",
+                "exl2conv/exl2conv_ext/cpp/generator.cpp",
                 "exl2conv/exl2conv_ext/cpp/sampling.cpp",
                 "exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp",
                 "exl2conv/exl2conv_ext/cpp/safetensors.cpp"
             ],
             extra_compile_args=extra_compile_args,
             libraries=["cublas"] if windows else [],
         )],
```

