# Comparing `tmp/pyatf-0.0.2.tar.gz` & `tmp/pyatf-0.0.3.tar.gz`

## Comparing `pyatf-0.0.2.tar` & `pyatf-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.2/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/feature_demonstration/result_check/result_check.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
--rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/cuda__saxpy/cuda__saxpy.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/opencl__saxpy/opencl__saxpy.py
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/opencl__sgemm/cltune_gemm.cl
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.2/examples/full_examples/opencl__sgemm/opencl__sgemm.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/range.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/result_check.py
--rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_space.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/tp.py
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/tuner.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/tuning_data.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/__init__.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/abort_condition.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/cost.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/duration.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/evaluations.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/fraction.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/abort_conditions/speedup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/__init__.py
--rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/cuda.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/generic.py
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/opencl.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/cost_functions/python.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/__init__.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/auc_bandit.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/differential_evolution.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/exhaustive.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/opentuner.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/pattern_search.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/random.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/round_robin.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/search_technique.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/search_technique_1d.py
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/simulated_annealing.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 pyatf-0.0.2/src/pyatf/search_techniques/torczon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/test_range.py
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/test_search_space.py
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 pyatf-0.0.2/tests/test_tuning_data.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.2/LICENSE
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.2/PyPI/README.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.3/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/feature_demonstration/result_check/result_check.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
+-rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/cuda__saxpy/cuda__saxpy.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/opencl__saxpy/opencl__saxpy.py
+-rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/opencl__sgemm/cltune_gemm.cl
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/opencl__sgemm/opencl__sgemm.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/range.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/result_check.py
+-rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_space.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/tp.py
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/tuner.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/tuning_data.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/__init__.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/abort_condition.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/cost.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/duration.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/evaluations.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/fraction.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/speedup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/__init__.py
+-rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/cuda.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/generic.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/opencl.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/python.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/__init__.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/auc_bandit.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/differential_evolution.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/exhaustive.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/opentuner.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/pattern_search.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/random.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/round_robin.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/search_technique.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/search_technique_1d.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/simulated_annealing.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/torczon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/test_range.py
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/test_search_space.py
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/test_tuning_data.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.3/LICENSE
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.3/PyPI/README.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.3/PKG-INFO
```

### Comparing `pyatf-0.0.2/README.md` & `pyatf-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py` & `pyatf-0.0.3/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/feature_demonstration/result_check/result_check.py` & `pyatf-0.0.3/examples/feature_demonstration/result_check/result_check.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py` & `pyatf-0.0.3/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp` & `pyatf-0.0.3/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py` & `pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp` & `pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/cuda__saxpy/cuda__saxpy.py` & `pyatf-0.0.3/examples/full_examples/cuda__saxpy/cuda__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/opencl__saxpy/opencl__saxpy.py` & `pyatf-0.0.3/examples/full_examples/opencl__saxpy/opencl__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/opencl__sgemm/cltune_gemm.cl` & `pyatf-0.0.3/examples/full_examples/opencl__sgemm/cltune_gemm.cl`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/examples/full_examples/opencl__sgemm/opencl__sgemm.py` & `pyatf-0.0.3/examples/full_examples/opencl__sgemm/opencl__sgemm.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/range.py` & `pyatf-0.0.3/src/pyatf/range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_space.py` & `pyatf-0.0.3/src/pyatf/search_space.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/tp.py` & `pyatf-0.0.3/src/pyatf/tp.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/tuner.py` & `pyatf-0.0.3/src/pyatf/tuner.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/tuning_data.py` & `pyatf-0.0.3/src/pyatf/tuning_data.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/abort_conditions/abort_condition.py` & `pyatf-0.0.3/src/pyatf/abort_conditions/abort_condition.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/abort_conditions/duration.py` & `pyatf-0.0.3/src/pyatf/abort_conditions/duration.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/abort_conditions/evaluations.py` & `pyatf-0.0.3/src/pyatf/abort_conditions/evaluations.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/abort_conditions/fraction.py` & `pyatf-0.0.3/src/pyatf/abort_conditions/fraction.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/abort_conditions/speedup.py` & `pyatf-0.0.3/src/pyatf/abort_conditions/speedup.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/cost_functions/cuda.py` & `pyatf-0.0.3/src/pyatf/cost_functions/cuda.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/cost_functions/generic.py` & `pyatf-0.0.3/src/pyatf/cost_functions/generic.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/cost_functions/opencl.py` & `pyatf-0.0.3/src/pyatf/cost_functions/opencl.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/cost_functions/python.py` & `pyatf-0.0.3/src/pyatf/cost_functions/python.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/auc_bandit.py` & `pyatf-0.0.3/src/pyatf/search_techniques/auc_bandit.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/differential_evolution.py` & `pyatf-0.0.3/src/pyatf/search_techniques/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/exhaustive.py` & `pyatf-0.0.3/src/pyatf/search_techniques/exhaustive.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/opentuner.py` & `pyatf-0.0.3/src/pyatf/search_techniques/opentuner.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/pattern_search.py` & `pyatf-0.0.3/src/pyatf/search_techniques/pattern_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,87 +48,85 @@
         self._current_parameter = 0
         self._current_state = PatternSearch.State.INITIALIZATION
 
     def finalize(self):
         pass
 
     def get_next_coordinates(self) -> Set[Coordinates]:
-        match self._current_state:
-            case PatternSearch.State.INITIALIZATION:
-                self._exploratory_coordinates = list(self._base)
-                self._pattern_coordinates = list(self._base)
-                return {clamp_coordinates_capped(self._base)}
-            case PatternSearch.State.EXPLORATORY_PLUS:
-                self._exploratory_coordinates[self._current_parameter] += self._step_size
-                return {clamp_coordinates_capped(tuple(self._exploratory_coordinates))}
-            case PatternSearch.State.EXPLORATORY_MINUS:
-                if self._trigger:
-                    self._exploratory_coordinates[self._current_parameter] -= 2 * self._step_size
-                else:
-                    self._exploratory_coordinates[self._current_parameter] -= self._step_size
-                return {clamp_coordinates_capped(tuple(self._exploratory_coordinates))}
-            case PatternSearch.State.PATTERN:
-                return {clamp_coordinates_capped(tuple(self._pattern_coordinates))}
+        if self._current_state == PatternSearch.State.INITIALIZATION:
+            self._exploratory_coordinates = list(self._base)
+            self._pattern_coordinates = list(self._base)
+            return {clamp_coordinates_capped(self._base)}
+        elif self._current_state == PatternSearch.State.EXPLORATORY_PLUS:
+            self._exploratory_coordinates[self._current_parameter] += self._step_size
+            return {clamp_coordinates_capped(tuple(self._exploratory_coordinates))}
+        elif self._current_state == PatternSearch.State.EXPLORATORY_MINUS:
+            if self._trigger:
+                self._exploratory_coordinates[self._current_parameter] -= 2 * self._step_size
+            else:
+                self._exploratory_coordinates[self._current_parameter] -= self._step_size
+            return {clamp_coordinates_capped(tuple(self._exploratory_coordinates))}
+        elif self._current_state == PatternSearch.State.PATTERN:
+            return {clamp_coordinates_capped(tuple(self._pattern_coordinates))}
 
     def report_costs(self, costs: Dict[Coordinates, Cost]):
         if len(costs) != 1:
             raise ValueError('expecting costs for exactly one coordinate')
         coordinates, cost = next(iter(costs.items()))
         if cost is None:
             cost = float('inf')
-        match self._current_state:
-            case PatternSearch.State.INITIALIZATION:
-                if cost == float('inf'):
-                    self._base = tuple(1.0 - random.random() for _ in range(self._dimensionality))
+        if self._current_state == PatternSearch.State.INITIALIZATION:
+            if cost == float('inf'):
+                self._base = tuple(1.0 - random.random() for _ in range(self._dimensionality))
+            else:
+                self._base_fitness = cost
+                self._exploratory_coordinates_fitness = cost
+                self._pattern_coordinates_fitness = cost
+                self._current_state = PatternSearch.State.EXPLORATORY_PLUS
+        elif self._current_state == PatternSearch.State.EXPLORATORY_PLUS:
+            if cost < self._exploratory_coordinates_fitness:
+                self._exploratory_coordinates[self._current_parameter] += self._step_size
+                if (self._exploratory_coordinates[self._current_parameter] <= 0.0
+                        or self._exploratory_coordinates[self._current_parameter] > 1.0):
+                    self._exploratory_coordinates[self._current_parameter] = math.fmod(
+                        abs(self._exploratory_coordinates[self._current_parameter]), 1.0)
+                self._exploratory_coordinates_fitness = cost
+                self._trigger = True
+            self._current_state = PatternSearch.State.EXPLORATORY_MINUS
+        elif self._current_state == PatternSearch.State.EXPLORATORY_MINUS:
+            if cost < self._exploratory_coordinates_fitness:
+                if self._trigger:
+                    self._exploratory_coordinates[self._current_parameter] -= 2 * self._step_size
                 else:
-                    self._base_fitness = cost
-                    self._exploratory_coordinates_fitness = cost
-                    self._pattern_coordinates_fitness = cost
-                    self._current_state = PatternSearch.State.EXPLORATORY_PLUS
-            case PatternSearch.State.EXPLORATORY_PLUS:
-                if cost < self._exploratory_coordinates_fitness:
-                    self._exploratory_coordinates[self._current_parameter] += self._step_size
-                    if (self._exploratory_coordinates[self._current_parameter] <= 0.0
-                            or self._exploratory_coordinates[self._current_parameter] > 1.0):
-                        self._exploratory_coordinates[self._current_parameter] = math.fmod(
-                            abs(self._exploratory_coordinates[self._current_parameter]), 1.0)
-                    self._exploratory_coordinates_fitness = cost
-                    self._trigger = True
-                self._current_state = PatternSearch.State.EXPLORATORY_MINUS
-            case PatternSearch.State.EXPLORATORY_MINUS:
-                if cost < self._exploratory_coordinates_fitness:
-                    if self._trigger:
-                        self._exploratory_coordinates[self._current_parameter] -= 2 * self._step_size
-                    else:
-                        self._exploratory_coordinates[self._current_parameter] -= self._step_size
-                    if (self._exploratory_coordinates[self._current_parameter] <= 0.0
-                            or self._exploratory_coordinates[self._current_parameter] > 1.0):
-                        self._exploratory_coordinates[self._current_parameter] = math.fmod(
-                            abs(self._exploratory_coordinates[self._current_parameter]), 1.0)
-                    self._exploratory_coordinates_fitness = cost
-                self._trigger = False
-                self._current_parameter += 1
+                    self._exploratory_coordinates[self._current_parameter] -= self._step_size
+                if (self._exploratory_coordinates[self._current_parameter] <= 0.0
+                        or self._exploratory_coordinates[self._current_parameter] > 1.0):
+                    self._exploratory_coordinates[self._current_parameter] = math.fmod(
+                        abs(self._exploratory_coordinates[self._current_parameter]), 1.0)
+                self._exploratory_coordinates_fitness = cost
+            self._trigger = False
+            self._current_parameter += 1
 
-                if self._current_parameter == self._dimensionality:
-                    if self._exploratory_coordinates_fitness < self._pattern_coordinates_fitness:
-                        for d in range(self._dimensionality):
-                            self._pattern_coordinates[d] = 2 * self._exploratory_coordinates[d] - self._base[d]
-                            if self._pattern_coordinates[d] <= 0.0 or self._pattern_coordinates[d] > 1.0:
-                                self._pattern_coordinates[d] = math.fmod(abs(self._pattern_coordinates[d]), 1.0)
-                        self._base = tuple(self._exploratory_coordinates)
-                        self._base_fitness = self._exploratory_coordinates_fitness
-                        self._exploratory_coordinates = self._pattern_coordinates.copy()
-                        self._current_state = PatternSearch.State.PATTERN
-                    else:
-                        self._exploratory_coordinates = list(self._base)
-                        self._exploratory_coordinates_fitness = self._base_fitness
-                        self._pattern_coordinates = list(self._base)
-                        self._pattern_coordinates_fitness = self._base_fitness
-                        self._step_size *= 0.5
-                        self._current_state = PatternSearch.State.EXPLORATORY_PLUS
-                    self._current_parameter = 0
+            if self._current_parameter == self._dimensionality:
+                if self._exploratory_coordinates_fitness < self._pattern_coordinates_fitness:
+                    for d in range(self._dimensionality):
+                        self._pattern_coordinates[d] = 2 * self._exploratory_coordinates[d] - self._base[d]
+                        if self._pattern_coordinates[d] <= 0.0 or self._pattern_coordinates[d] > 1.0:
+                            self._pattern_coordinates[d] = math.fmod(abs(self._pattern_coordinates[d]), 1.0)
+                    self._base = tuple(self._exploratory_coordinates)
+                    self._base_fitness = self._exploratory_coordinates_fitness
+                    self._exploratory_coordinates = self._pattern_coordinates.copy()
+                    self._current_state = PatternSearch.State.PATTERN
                 else:
+                    self._exploratory_coordinates = list(self._base)
+                    self._exploratory_coordinates_fitness = self._base_fitness
+                    self._pattern_coordinates = list(self._base)
+                    self._pattern_coordinates_fitness = self._base_fitness
+                    self._step_size *= 0.5
                     self._current_state = PatternSearch.State.EXPLORATORY_PLUS
-            case PatternSearch.State.PATTERN:
-                self._pattern_coordinates_fitness = cost
-                self._exploratory_coordinates_fitness = cost
+                self._current_parameter = 0
+            else:
                 self._current_state = PatternSearch.State.EXPLORATORY_PLUS
+        elif self._current_state == PatternSearch.State.PATTERN:
+            self._pattern_coordinates_fitness = cost
+            self._exploratory_coordinates_fitness = cost
+            self._current_state = PatternSearch.State.EXPLORATORY_PLUS
```

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/random.py` & `pyatf-0.0.3/src/pyatf/search_techniques/random.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/round_robin.py` & `pyatf-0.0.3/src/pyatf/search_techniques/round_robin.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/search_technique.py` & `pyatf-0.0.3/src/pyatf/search_techniques/search_technique.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/search_technique_1d.py` & `pyatf-0.0.3/src/pyatf/search_techniques/search_technique_1d.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/simulated_annealing.py` & `pyatf-0.0.3/src/pyatf/search_techniques/simulated_annealing.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,88 +89,86 @@
         self._max_time = len(self._schedule) - 1
         self._neighbors = {}
 
     def finalize(self):
         pass
 
     def get_next_coordinates(self) -> Set[Coordinates]:
-        match self._current_state:
-            case SimulatedAnnealing.State.INITIALIZATION:
-                self._current_parameter = 0
-                self._temp = self._schedule[min(self._time, self._max_time)]
-                self._step_size = get_step_size(self._time, self._temp)
-                self._current_coordinates = tuple(1.0 - random.random() for _ in range(self._dimensionality))
-                self._neighbors[self._current_coordinates] = 0.0
-                return {clamp_coordinates_capped(self._current_coordinates)}
-            case SimulatedAnnealing.State.EXPLORE_PLUS:
-                if self._current_coordinates[self._current_parameter] < 1.0:
-                    new_coordinates = list(self._current_coordinates)
-                    new_coordinates[self._current_parameter] += self._step_size * random.random()
-                    new_coordinates = tuple(new_coordinates)
-                    self._neighbors[new_coordinates] = 0.0
-                    if self._current_coordinates[self._current_parameter] <= 0.0:
-                        self._current_state = SimulatedAnnealing.State.EXPLORE_MINUS
-                    return {clamp_coordinates_capped(new_coordinates)}
-                else:
+        if self._current_state == SimulatedAnnealing.State.INITIALIZATION:
+            self._current_parameter = 0
+            self._temp = self._schedule[min(self._time, self._max_time)]
+            self._step_size = get_step_size(self._time, self._temp)
+            self._current_coordinates = tuple(1.0 - random.random() for _ in range(self._dimensionality))
+            self._neighbors[self._current_coordinates] = 0.0
+            return {clamp_coordinates_capped(self._current_coordinates)}
+        elif self._current_state == SimulatedAnnealing.State.EXPLORE_PLUS:
+            if self._current_coordinates[self._current_parameter] < 1.0:
+                new_coordinates = list(self._current_coordinates)
+                new_coordinates[self._current_parameter] += self._step_size * random.random()
+                new_coordinates = tuple(new_coordinates)
+                self._neighbors[new_coordinates] = 0.0
+                if self._current_coordinates[self._current_parameter] <= 0.0:
                     self._current_state = SimulatedAnnealing.State.EXPLORE_MINUS
-                    new_coordinates = list(self._current_coordinates)
-                    new_coordinates[self._current_parameter] -= self._step_size * random.random()
-                    new_coordinates = tuple(new_coordinates)
-                    self._neighbors[new_coordinates] = 0.0
-                    return {clamp_coordinates_capped(new_coordinates)}
-            case SimulatedAnnealing.State.EXPLORE_MINUS:
+                return {clamp_coordinates_capped(new_coordinates)}
+            else:
+                self._current_state = SimulatedAnnealing.State.EXPLORE_MINUS
                 new_coordinates = list(self._current_coordinates)
                 new_coordinates[self._current_parameter] -= self._step_size * random.random()
                 new_coordinates = tuple(new_coordinates)
                 self._neighbors[new_coordinates] = 0.0
                 return {clamp_coordinates_capped(new_coordinates)}
+        elif self._current_state == SimulatedAnnealing.State.EXPLORE_MINUS:
+            new_coordinates = list(self._current_coordinates)
+            new_coordinates[self._current_parameter] -= self._step_size * random.random()
+            new_coordinates = tuple(new_coordinates)
+            self._neighbors[new_coordinates] = 0.0
+            return {clamp_coordinates_capped(new_coordinates)}
 
     def report_costs(self, costs: Dict[Coordinates, Cost]):
         if len(costs) != 1:
             raise ValueError('expecting costs for exactly one coordinate')
         coordinates, cost = next(iter(costs.items()))
         if cost is None:
             cost = float('inf')
-        match self._current_state:
-            case SimulatedAnnealing.State.INITIALIZATION:
-                self._neighbors[coordinates] = cost
+        if self._current_state == SimulatedAnnealing.State.INITIALIZATION:
+            self._neighbors[coordinates] = cost
+            self._best_coordinates = coordinates
+            self._best_result = cost
+            self._current_state = SimulatedAnnealing.State.EXPLORE_PLUS
+        elif self._current_state == SimulatedAnnealing.State.EXPLORE_PLUS:
+            self._neighbors[coordinates] = cost
+            if cost < self._best_result:
                 self._best_coordinates = coordinates
                 self._best_result = cost
+            self._current_state = SimulatedAnnealing.State.EXPLORE_MINUS
+        elif self._current_state == SimulatedAnnealing.State.EXPLORE_MINUS:
+            self._neighbors[coordinates] = cost
+            if cost < self._best_result:
+                self._best_coordinates = coordinates
+                self._best_result = cost
+            self._current_parameter += 1
+            if self._current_parameter == self._dimensionality:
+                self._current_parameter = 0
+                current_result = None
+                while True:
+                    if not self._neighbors:
+                        self._current_coordinates = self._best_coordinates
+                        current_result = self._best_result
+                        break
+                    candidate_coordinates, candidate_cost = random.choice(list(self._neighbors.items()))
+                    if random.random() < AcceptanceFunction(1.0,
+                                                            relative(candidate_cost, self._best_result),
+                                                            self._temp):
+                        self._current_coordinates = candidate_coordinates
+                        current_result = candidate_cost
+                        break
+                    del self._neighbors[candidate_coordinates]
+                self._time += 1
+                if self._time > self._max_time:
+                    self._time -= self._max_time
+                self._temp = self._schedule[min(self._time, self._max_time)]
+                self._step_size = get_step_size(self._time, self._temp)
+                self._neighbors.clear()
+                self._neighbors[self._current_coordinates] = current_result
+                self._current_state = SimulatedAnnealing.State.EXPLORE_PLUS
+            else:
                 self._current_state = SimulatedAnnealing.State.EXPLORE_PLUS
-            case SimulatedAnnealing.State.EXPLORE_PLUS:
-                self._neighbors[coordinates] = cost
-                if cost < self._best_result:
-                    self._best_coordinates = coordinates
-                    self._best_result = cost
-                self._current_state = SimulatedAnnealing.State.EXPLORE_MINUS
-            case SimulatedAnnealing.State.EXPLORE_MINUS:
-                self._neighbors[coordinates] = cost
-                if cost < self._best_result:
-                    self._best_coordinates = coordinates
-                    self._best_result = cost
-                self._current_parameter += 1
-                if self._current_parameter == self._dimensionality:
-                    self._current_parameter = 0
-                    current_result = None
-                    while True:
-                        if not self._neighbors:
-                            self._current_coordinates = self._best_coordinates
-                            current_result = self._best_result
-                            break
-                        candidate_coordinates, candidate_cost = random.choice(list(self._neighbors.items()))
-                        if random.random() < AcceptanceFunction(1.0,
-                                                                relative(candidate_cost, self._best_result),
-                                                                self._temp):
-                            self._current_coordinates = candidate_coordinates
-                            current_result = candidate_cost
-                            break
-                        del self._neighbors[candidate_coordinates]
-                    self._time += 1
-                    if self._time > self._max_time:
-                        self._time -= self._max_time
-                    self._temp = self._schedule[min(self._time, self._max_time)]
-                    self._step_size = get_step_size(self._time, self._temp)
-                    self._neighbors.clear()
-                    self._neighbors[self._current_coordinates] = current_result
-                    self._current_state = SimulatedAnnealing.State.EXPLORE_PLUS
-                else:
-                    self._current_state = SimulatedAnnealing.State.EXPLORE_PLUS
```

### Comparing `pyatf-0.0.2/src/pyatf/search_techniques/torczon.py` & `pyatf-0.0.3/src/pyatf/search_techniques/torczon.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,35 +107,34 @@
 
     def _switch_state(self, new_state: 'Torczon.State'):
         self._current_state = new_state
         self._current_vertex = 0
         self._cost_improved = False
 
     def _generate_next_simplex(self):
-        match self._current_state:
-            case Torczon.State.TORC_INITIAL:
-                self._test_simplex.vertices = self._reflect_base_simplex_vertices()
+        if self._current_state == Torczon.State.TORC_INITIAL:
+            self._test_simplex.vertices = self._reflect_base_simplex_vertices()
+            self._test_simplex.best_vertex = 0
+            self._current_simplex = self._test_simplex
+            self._switch_state(Torczon.State.TORC_REFLECTED)
+        elif self._current_state == Torczon.State.TORC_REFLECTED:
+            if self._cost_improved:
+                self._base_simplex = copy.copy(self._test_simplex)
+                self._test_simplex.vertices = self._expand_base_simplex_vertices()
                 self._test_simplex.best_vertex = 0
                 self._current_simplex = self._test_simplex
-                self._switch_state(Torczon.State.TORC_REFLECTED)
-            case Torczon.State.TORC_REFLECTED:
-                if self._cost_improved:
-                    self._base_simplex = copy.copy(self._test_simplex)
-                    self._test_simplex.vertices = self._expand_base_simplex_vertices()
-                    self._test_simplex.best_vertex = 0
-                    self._current_simplex = self._test_simplex
-                    self._switch_state(Torczon.State.TORC_EXPANDED)
-                else:
-                    self._base_simplex.vertices = self._contract_base_simplex_vertices()
-                    self._base_simplex.best_vertex = 0
-                    self._current_simplex = self._base_simplex
-                    self._best_cost = float('inf')
-                    self._current_center = 0
-                    self._switch_state(Torczon.State.TORC_INITIAL)
-            case Torczon.State.TORC_EXPANDED:
-                if self._cost_improved:
-                    self._base_simplex = copy.copy(self._test_simplex)
-                self._current_center = self._base_simplex.best_vertex
-                self._test_simplex.vertices = self._reflect_base_simplex_vertices()
-                self._test_simplex.best_vertex = 0
-                self._current_simplex = self._test_simplex
-                self._switch_state(Torczon.State.TORC_REFLECTED)
+                self._switch_state(Torczon.State.TORC_EXPANDED)
+            else:
+                self._base_simplex.vertices = self._contract_base_simplex_vertices()
+                self._base_simplex.best_vertex = 0
+                self._current_simplex = self._base_simplex
+                self._best_cost = float('inf')
+                self._current_center = 0
+                self._switch_state(Torczon.State.TORC_INITIAL)
+        elif self._current_state == Torczon.State.TORC_EXPANDED:
+            if self._cost_improved:
+                self._base_simplex = copy.copy(self._test_simplex)
+            self._current_center = self._base_simplex.best_vertex
+            self._test_simplex.vertices = self._reflect_base_simplex_vertices()
+            self._test_simplex.best_vertex = 0
+            self._current_simplex = self._test_simplex
+            self._switch_state(Torczon.State.TORC_REFLECTED)
```

### Comparing `pyatf-0.0.2/tests/test_range.py` & `pyatf-0.0.3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/tests/test_search_space.py` & `pyatf-0.0.3/tests/test_search_space.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/tests/test_tuning_data.py` & `pyatf-0.0.3/tests/test_tuning_data.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/LICENSE` & `pyatf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/pyproject.toml` & `pyatf-0.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyatf"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Richard Schulze", email="r.schulze@uni-muenster.de" },
     { name="Ari Rasch", email="a.rasch@uni-muenster.de" }
 ]
 description = "Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained"
 readme = "./PyPI/README.md"
 requires-python = ">=3.9"
```

### Comparing `pyatf-0.0.2/PyPI/README.md` & `pyatf-0.0.3/PyPI/README.md`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.2/PKG-INFO` & `pyatf-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained
 Project-URL: Homepage, https://atf-project.org/
 Project-URL: Issues, https://github.com/atf-tuner/pyATF/issues
 Author-email: Richard Schulze <r.schulze@uni-muenster.de>, Ari Rasch <a.rasch@uni-muenster.de>
 License-File: LICENSE
 Keywords: auto-tuning,constraints,optimization,performance,tuning
 Classifier: License :: OSI Approved :: MIT License
```

