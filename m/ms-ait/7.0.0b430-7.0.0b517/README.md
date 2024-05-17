# Comparing `tmp/ms-ait-7.0.0b430.zip` & `tmp/ms-ait-7.0.0b517.zip`

## zipinfo {}

```diff
@@ -1,548 +1,548 @@
-Zip file size: 691450 bytes, number of entries: 546
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/ms_ait.egg-info/
--rwxrwxrwx  2.0 unx      228 b- defN 24-May-13 12:35 ms-ait-7.0.0b430/PKG-INFO
--rwxrwxrwx  2.0 unx     4802 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/README.md
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/requirements.txt
--rwxrwxrwx  2.0 unx       38 b- defN 24-May-13 12:35 ms-ait-7.0.0b430/setup.cfg
--rwxrwxrwx  2.0 unx     1855 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/setup.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/profile/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/tensor_view/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/tests/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/utils/
--rwxrwxrwx  2.0 unx      600 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/__init__.py
--rwxrwxrwx  2.0 unx     1744 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/
--rwxrwxrwx  2.0 unx     5220 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/README.md
--rwxrwxrwx  2.0 unx       65 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/requirements.txt
--rwxrwxrwx  2.0 unx     2227 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/analyze/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/analyze/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/__init__.py
--rwxrwxrwx  2.0 unx      695 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/analyze/model_evaluation/__install__.py
--rwxrwxrwx  2.0 unx     5943 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/__main__.py
--rwxrwxrwx  2.0 unx      843 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/config.py
--rwxrwxrwx  2.0 unx      936 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/op_info.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/
--rwxrwxrwx  2.0 unx      882 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/const.py
--rwxrwxrwx  2.0 unx     1078 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/log.py
--rwxrwxrwx  2.0 unx     1917 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/utils.py
--rwxrwxrwx  2.0 unx       95 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/__init__.py
--rwxrwxrwx  2.0 unx     1072 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/atc_err.py
--rwxrwxrwx  2.0 unx      730 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/engine.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/framework.py
--rwxrwxrwx  2.0 unx      852 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
--rwxrwxrwx  2.0 unx      692 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/soc_type.py
--rwxrwxrwx  2.0 unx      305 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/
--rwxrwxrwx  2.0 unx     7722 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/analysis.py
--rwxrwxrwx  2.0 unx     4707 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/result.py
--rwxrwxrwx  2.0 unx     1236 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/rule.py
--rwxrwxrwx  2.0 unx       51 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/__init__.py
--rwxrwxrwx  2.0 unx     2495 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/onnx.py
--rwxrwxrwx  2.0 unx       59 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/__init__.py
--rwxrwxrwx  2.0 unx     4428 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/opp.py
--rwxrwxrwx  2.0 unx     2212 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/op_map.py
--rwxrwxrwx  2.0 unx      683 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/__init__.py
--rwxrwxrwx  2.0 unx     2210 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/onnx.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/__init__.py
--rwxrwxrwx  2.0 unx     4426 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/atc.py
--rwxrwxrwx  2.0 unx     5374 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/model.py
--rwxrwxrwx  2.0 unx     5339 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/om.py
--rwxrwxrwx  2.0 unx      750 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/backend/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/infer_analyser/
--rwxrwxrwx  2.0 unx      762 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_infer.py
--rwxrwxrwx  2.0 unx     1835 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/install.sh
--rwxrwxrwx  2.0 unx    51061 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/README.md
--rwxrwxrwx  2.0 unx       26 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/requirements.txt
--rwxrwxrwx  2.0 unx     1769 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/
--rwxrwxrwx  2.0 unx     2426 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/benchmark/ais_bench/install.sh
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/__init__.py
--rwxrwxrwx  2.0 unx     1763 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/ais_bench/__install__.py
--rwxrwxrwx  2.0 unx      752 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/
--rwxrwxrwx  2.0 unx     2685 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/interface.py
--rwxrwxrwx  2.0 unx      759 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/log.py
--rwxrwxrwx  2.0 unx     1591 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/README.md
--rwxrwxrwx  2.0 unx     2433 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/recorder.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/__init__.py
--rwxrwxrwx  2.0 unx     3142 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
--rwxrwxrwx  2.0 unx     4606 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
--rwxrwxrwx  2.0 unx     1375 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
--rwxrwxrwx  2.0 unx     2196 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/download.sh
--rwxrwxrwx  2.0 unx     3978 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
--rwxrwxrwx  2.0 unx     4244 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/__init__.py
--rwxrwxrwx  2.0 unx     2999 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement.py
--rwxrwxrwx  2.0 unx     1260 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/
--rwxrwxrwx  2.0 unx     4614 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_adapter.py
--rwxrwxrwx  2.0 unx     7151 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_check.py
--rwxrwxrwx  2.0 unx    31048 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/benchmark_process.py
--rwxrwxrwx  2.0 unx    37710 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/interface.py
--rwxrwxrwx  2.0 unx    14389 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/io_oprations.py
--rwxrwxrwx  2.0 unx    10701 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/main_cli.py
--rwxrwxrwx  2.0 unx    10444 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/miscellaneous.py
--rwxrwxrwx  2.0 unx    12012 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/path_security_check.py
--rwxrwxrwx  2.0 unx     3260 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/registry.py
--rwxrwxrwx  2.0 unx     9472 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/summary.py
--rwxrwxrwx  2.0 unx    10122 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__init__.py
--rwxrwxrwx  2.0 unx     8700 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__main__.py
--rwxrwxrwx  2.0 unx     3025 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend.py
--rwxrwxrwx  2.0 unx     5400 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
--rwxrwxrwx  2.0 unx      960 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/__init__.py
--rwxrwxrwx  2.0 unx     1623 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/backend/install.sh
--rwxrwxrwx  2.0 unx     6911 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/backend/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/backend/__init__.py
--rwxrwxrwx  2.0 unx     2843 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/analyser.py
--rwxrwxrwx  2.0 unx     8588 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/infer_analyser.sh
--rwxrwxrwx  2.0 unx     1680 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/info_convert_json.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/
--rwxrwxrwx  2.0 unx     1520 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/build.sh
--rwxrwxrwx  2.0 unx     3162 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/README.md
--rwxrwxrwx  2.0 unx       43 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/convert/requirements.txt
--rwxrwxrwx  2.0 unx     2167 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aie/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aoe/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/atc/
--rwxrwxrwx  2.0 unx     3463 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/cmd_utils.py
--rwxrwxrwx  2.0 unx     1520 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/model_convert/install.sh
--rwxrwxrwx  2.0 unx      590 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/__init__.py
--rwxrwxrwx  2.0 unx     1382 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/model_convert/__install__.py
--rwxrwxrwx  2.0 unx     3982 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/model_convert/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aie/core/
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/__init__.py
--rwxrwxrwx  2.0 unx      775 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/config.py
--rwxrwxrwx  2.0 unx      646 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/__init__.py
--rwxrwxrwx  2.0 unx     2221 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/core/convert.py
--rwxrwxrwx  2.0 unx      591 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/core/__init__.py
--rwxrwxrwx  2.0 unx     9218 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aoe/aoe_args_map.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aoe/__init__.py
--rwxrwxrwx  2.0 unx    12775 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/atc/atc_args_map.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/atc/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/
--rwxrwxrwx  2.0 unx      787 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/debug/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/
--rwxrwxrwx  2.0 unx     5324 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/main.py
--rwxrwxrwx  2.0 unx    11876 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/README.md
--rwxrwxrwx  2.0 unx      160 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/requirements.txt
--rwxrwxrwx  2.0 unx     2317 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/
--rwxrwxrwx  2.0 unx    24580 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/cmp_process.py
--rwxrwxrwx  2.0 unx     2181 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/install.sh
--rwxrwxrwx  2.0 unx     5359 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
--rwxrwxrwx  2.0 unx     5175 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf_debug_runner.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__init__.py
--rwxrwxrwx  2.0 unx     1716 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__install__.py
--rwxrwxrwx  2.0 unx     7990 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__main__.py
--rwxrwxrwx  2.0 unx     5723 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
--rwxrwxrwx  2.0 unx     2293 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/__init__.py
--rwxrwxrwx  2.0 unx     3526 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/atc_utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/__init__.py
--rwxrwxrwx  2.0 unx     5651 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/__init__.py
--rwxrwxrwx  2.0 unx     8737 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/args_check.py
--rwxrwxrwx  2.0 unx     3621 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/convert.py
--rwxrwxrwx  2.0 unx     4757 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dump_data.py
--rwxrwxrwx  2.0 unx     1309 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
--rwxrwxrwx  2.0 unx     6098 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/tf_common.py
--rwxrwxrwx  2.0 unx    23475 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/__init__.py
--rwxrwxrwx  2.0 unx    11004 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/analyser.py
--rwxrwxrwx  2.0 unx    15491 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/net_compare.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/__init__.py
--rwxrwxrwx  2.0 unx    26647 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/npu_dump_data.py
--rwxrwxrwx  2.0 unx    17174 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/om_parser.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/__init__.py
--rwxrwxrwx  2.0 unx     9202 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/custom_op.py
--rwxrwxrwx  2.0 unx    15327 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/__init__.py
--rwxrwxrwx  2.0 unx      619 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/__init__.py
--rwxrwxrwx  2.0 unx     7707 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/single_op.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/__init__.py
--rwxrwxrwx  2.0 unx    13711 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/tf_dump_data.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/
--rwxrwxrwx  2.0 unx    11087 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/README.md
--rwxrwxrwx  2.0 unx      140 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/requirements.txt
--rwxrwxrwx  2.0 unx     2811 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/surgeon/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/
--rwxrwxrwx  2.0 unx    15282 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/ait_main.py
--rwxrwxrwx  2.0 unx     5587 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/options.py
--rwxrwxrwx  2.0 unx      878 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__init__.py
--rwxrwxrwx  2.0 unx     1160 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__install__.py
--rwxrwxrwx  2.0 unx     6305 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__main__.py
--rwxrwxrwx  2.0 unx     6012 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/args_check.py
--rwxrwxrwx  2.0 unx     8574 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/click_utils.py
--rwxrwxrwx  2.0 unx     2307 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/config.py
--rwxrwxrwx  2.0 unx     1633 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/log.py
--rwxrwxrwx  2.0 unx     2265 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/register.py
--rwxrwxrwx  2.0 unx      880 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/singleton.py
--rwxrwxrwx  2.0 unx     5111 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/utils.py
--rwxrwxrwx  2.0 unx     1032 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/__init__.py
--rwxrwxrwx  2.0 unx    11302 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
--rwxrwxrwx  2.0 unx       85 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
--rwxrwxrwx  2.0 unx     2102 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
--rwxrwxrwx  2.0 unx      784 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
--rwxrwxrwx  2.0 unx    28389 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
--rwxrwxrwx  2.0 unx     8101 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
--rwxrwxrwx  2.0 unx      755 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
--rwxrwxrwx  2.0 unx    28573 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
--rwxrwxrwx  2.0 unx     4880 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
--rwxrwxrwx  2.0 unx      747 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
--rwxrwxrwx  2.0 unx     4582 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
--rwxrwxrwx  2.0 unx     5214 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/README.md
--rwxrwxrwx  2.0 unx     1024 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
--rwxrwxrwx  2.0 unx      736 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
--rwxrwxrwx  2.0 unx     1694 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
--rwxrwxrwx  2.0 unx     2074 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
--rwxrwxrwx  2.0 unx     1390 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
--rwxrwxrwx  2.0 unx     4242 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
--rwxrwxrwx  2.0 unx     1556 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
--rwxrwxrwx  2.0 unx     2736 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
--rwxrwxrwx  2.0 unx      719 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
--rwxrwxrwx  2.0 unx     2234 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
--rwxrwxrwx  2.0 unx      679 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
--rwxrwxrwx  2.0 unx     1342 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
--rwxrwxrwx  2.0 unx     1404 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
--rwxrwxrwx  2.0 unx     1387 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
--rwxrwxrwx  2.0 unx     5279 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/
--rwxrwxrwx  2.0 unx     1565 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
--rwxrwxrwx  2.0 unx    15557 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/matcher.py
--rwxrwxrwx  2.0 unx     7709 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/pattern.py
--rwxrwxrwx  2.0 unx     6596 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/utils.py
--rwxrwxrwx  2.0 unx     2028 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
--rwxrwxrwx  2.0 unx     5589 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
--rwxrwxrwx  2.0 unx     7914 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
--rwxrwxrwx  2.0 unx     6563 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
--rwxrwxrwx  2.0 unx     6124 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
--rwxrwxrwx  2.0 unx    12418 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
--rwxrwxrwx  2.0 unx     5534 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
--rwxrwxrwx  2.0 unx    11185 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
--rwxrwxrwx  2.0 unx    10165 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
--rwxrwxrwx  2.0 unx     6285 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
--rwxrwxrwx  2.0 unx     7235 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
--rwxrwxrwx  2.0 unx     6958 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
--rwxrwxrwx  2.0 unx     3107 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
--rwxrwxrwx  2.0 unx    10959 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
--rwxrwxrwx  2.0 unx    19159 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
--rwxrwxrwx  2.0 unx     5350 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
--rwxrwxrwx  2.0 unx     8097 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
--rwxrwxrwx  2.0 unx    25805 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
--rwxrwxrwx  2.0 unx     1665 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
--rwxrwxrwx  2.0 unx    16842 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
--rwxrwxrwx  2.0 unx     5031 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
--rwxrwxrwx  2.0 unx    13241 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
--rwxrwxrwx  2.0 unx     8003 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
--rwxrwxrwx  2.0 unx     6050 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/inference.py
--rwxrwxrwx  2.0 unx     1559 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/log.py
--rwxrwxrwx  2.0 unx      505 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/README.md
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/
--rwxrwxrwx  2.0 unx    10044 b- defN 24-May-08 11:27 ms-ait-7.0.0b430/components/llm/README.md
--rwxrwxrwx  2.0 unx      108 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/requirements.txt
--rwxrwxrwx  2.0 unx     2370 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/llm/setup.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/llm/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/dump/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/transform/
--rwxrwxrwx  2.0 unx      903 b- defN 24-May-09 18:08 ms-ait-7.0.0b430/components/llm/ait_llm/install.sh
--rwxrwxrwx  2.0 unx      920 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/__init__.py
--rwxrwxrwx  2.0 unx     1792 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/llm/ait_llm/__install__.py
--rwxrwxrwx  2.0 unx    14898 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/__main__.py
--rwxrwxrwx  2.0 unx     2609 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/constant.py
--rwxrwxrwx  2.0 unx     4826 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/json_fitter.py
--rwxrwxrwx  2.0 unx     1581 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/log.py
--rwxrwxrwx  2.0 unx     3267 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/tool.py
--rwxrwxrwx  2.0 unx     4657 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/utils.py
--rwxrwxrwx  2.0 unx     8522 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/common/validate.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/__init__.py
--rwxrwxrwx  2.0 unx    22815 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/compare/atb_acc_cmp.py
--rwxrwxrwx  2.0 unx     5949 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_algorithm.py
--rwxrwxrwx  2.0 unx     8511 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_utils.py
--rwxrwxrwx  2.0 unx      957 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/compare/op_mapping.py
--rwxrwxrwx  2.0 unx    19113 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/compare/torchair_acc_cmp.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/compare/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/
--rwxrwxrwx  2.0 unx     8268 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/initial.py
--rwxrwxrwx  2.0 unx     2576 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/manual_dump.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/__init__.py
--rwxrwxrwx  2.0 unx     2445 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
--rwxrwxrwx  2.0 unx       91 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/__init__.py
--rwxrwxrwx  2.0 unx     3413 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_config.py
--rwxrwxrwx  2.0 unx     7648 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_hook.py
--rwxrwxrwx  2.0 unx     1647 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook.py
--rwxrwxrwx  2.0 unx     3067 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook_ops.py
--rwxrwxrwx  2.0 unx     7174 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/topo.py
--rwxrwxrwx  2.0 unx      722 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/__init__.py
--rwxrwxrwx  2.0 unx     4755 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/process.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/__init__.py
--rwxrwxrwx  2.0 unx     5241 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/case_filter.py
--rwxrwxrwx  2.0 unx    10300 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/metrics.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/
--rwxrwxrwx  2.0 unx     1645 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/case_manager.py
--rwxrwxrwx  2.0 unx    15421 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/opchecker.py
--rwxrwxrwx  2.0 unx    11806 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/operation_test.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/__init__.py
--rwxrwxrwx  2.0 unx     3879 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/build.sh
--rwxrwxrwx  2.0 unx      938 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
--rwxrwxrwx  2.0 unx    29744 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
--rwxrwxrwx  2.0 unx     1354 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/__init__.py
--rwxrwxrwx  2.0 unx     4577 b- defN 24-May-13 12:29 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/activation.py
--rwxrwxrwx  2.0 unx      925 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_gather.py
--rwxrwxrwx  2.0 unx     3251 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_reduce.py
--rwxrwxrwx  2.0 unx     1469 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/as_strided.py
--rwxrwxrwx  2.0 unx     1286 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/broadcast.py
--rwxrwxrwx  2.0 unx     1319 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/concat.py
--rwxrwxrwx  2.0 unx     1197 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/cumsum.py
--rwxrwxrwx  2.0 unx     5721 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/elewise.py
--rwxrwxrwx  2.0 unx     1783 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
--rwxrwxrwx  2.0 unx     1975 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
--rwxrwxrwx  2.0 unx     1592 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fill.py
--rwxrwxrwx  2.0 unx     2707 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/gather.py
--rwxrwxrwx  2.0 unx     1453 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
--rwxrwxrwx  2.0 unx     1274 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/kv_cache.py
--rwxrwxrwx  2.0 unx     4084 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/layer_norm.py
--rwxrwxrwx  2.0 unx     2687 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear.py
--rwxrwxrwx  2.0 unx     1165 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
--rwxrwxrwx  2.0 unx     2838 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
--rwxrwxrwx  2.0 unx     2631 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/matmul.py
--rwxrwxrwx  2.0 unx     1903 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/multinomial.py
--rwxrwxrwx  2.0 unx     1307 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/pad.py
--rwxrwxrwx  2.0 unx     1247 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/paged_attention.py
--rwxrwxrwx  2.0 unx     1372 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reduce.py
--rwxrwxrwx  2.0 unx     1210 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/repeat.py
--rwxrwxrwx  2.0 unx     1283 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
--rwxrwxrwx  2.0 unx     3504 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rms_norm.py
--rwxrwxrwx  2.0 unx     6893 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope.py
--rwxrwxrwx  2.0 unx     1942 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope_grad.py
--rwxrwxrwx  2.0 unx     9533 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/self_attention.py
--rwxrwxrwx  2.0 unx     1434 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/set_value.py
--rwxrwxrwx  2.0 unx     2261 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/slice.py
--rwxrwxrwx  2.0 unx     1222 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/softmax.py
--rwxrwxrwx  2.0 unx     1233 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/sort.py
--rwxrwxrwx  2.0 unx     1368 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/split.py
--rwxrwxrwx  2.0 unx     3198 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
--rwxrwxrwx  2.0 unx     2677 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
--rwxrwxrwx  2.0 unx     4783 b- defN 24-May-13 12:29 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transdata.py
--rwxrwxrwx  2.0 unx     1196 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transpose.py
--rwxrwxrwx  2.0 unx     2143 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/unpad.py
--rwxrwxrwx  2.0 unx      935 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/where.py
--rwxrwxrwx  2.0 unx     5680 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/__init__.py
--rwxrwxrwx  2.0 unx    12784 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant.py
--rwxrwxrwx  2.0 unx    22320 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
--rwxrwxrwx  2.0 unx     2542 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/profile/msprof/
--rwxrwxrwx  2.0 unx      602 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/
--rwxrwxrwx  2.0 unx     1835 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/install.sh
--rwxrwxrwx  2.0 unx     5011 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/README.md
--rwxrwxrwx  2.0 unx       10 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/requirements.txt
--rwxrwxrwx  2.0 unx     1581 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/msprof/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/msprof/__init__.py
--rwxrwxrwx  2.0 unx     4154 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/api.py
--rwxrwxrwx  2.0 unx     1277 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/args_adapter.py
--rwxrwxrwx  2.0 unx     4565 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/main_cli.py
--rwxrwxrwx  2.0 unx     4314 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/msprof_process.py
--rwxrwxrwx  2.0 unx      760 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__init__.py
--rwxrwxrwx  2.0 unx      694 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__install__.py
--rwxrwxrwx  2.0 unx     4513 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/
--rwxrwxrwx  2.0 unx       14 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/requirements.txt
--rwxrwxrwx  2.0 unx     1615 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/__init__.py
--rwxrwxrwx  2.0 unx     2261 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/atb.py
--rwxrwxrwx  2.0 unx     2240 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/handler.py
--rwxrwxrwx  2.0 unx     1035 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/logger.py
--rwxrwxrwx  2.0 unx     3438 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/main_cli.py
--rwxrwxrwx  2.0 unx     3921 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/operation.py
--rwxrwxrwx  2.0 unx      874 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/print_stat.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__init__.py
--rwxrwxrwx  2.0 unx      702 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__install__.py
--rwxrwxrwx  2.0 unx     3123 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tests/test_ait.sh
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/tests/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/
--rwxrwxrwx  2.0 unx    10875 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/install.bat
--rwxrwxrwx  2.0 unx     4111 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/install.sh
--rwxrwxrwx  2.0 unx    23645 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/README.md
--rwxrwxrwx  2.0 unx       94 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/requirements.txt
--rwxrwxrwx  2.0 unx     2329 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/report/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/
--rwxrwxrwx  2.0 unx    10875 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/app_analyze/install.bat
--rwxrwxrwx  2.0 unx     4481 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/transplt/app_analyze/install.sh
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/__init__.py
--rwxrwxrwx  2.0 unx     2441 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/app_analyze/__install__.py
--rwxrwxrwx  2.0 unx     3444 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/__main__.py
--rwxrwxrwx  2.0 unx    11196 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/common/kit_config.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/common/__init__.py
--rwxrwxrwx  2.0 unx     2257 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/exception_information.py
--rwxrwxrwx  2.0 unx     3419 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/source_scan_exception.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/__init__.py
--rwxrwxrwx  2.0 unx     4850 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/model.py
--rwxrwxrwx  2.0 unx     6911 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/project.py
--rwxrwxrwx  2.0 unx     3765 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/seq_project.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/__init__.py
--rwxrwxrwx  2.0 unx      983 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/app.py
--rwxrwxrwx  2.0 unx     5752 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/cmdline_input.py
--rwxrwxrwx  2.0 unx     1686 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/custom_input.py
--rwxrwxrwx  2.0 unx     1467 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/input_factory.py
--rwxrwxrwx  2.0 unx     2601 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/porting_input.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/__init__.py
--rwxrwxrwx  2.0 unx     1760 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/csv_report.py
--rwxrwxrwx  2.0 unx     1775 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/json_report.py
--rwxrwxrwx  2.0 unx     2202 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/report.py
--rwxrwxrwx  2.0 unx     1814 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/report_factory.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/
--rwxrwxrwx  2.0 unx    16004 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_parser.py
--rwxrwxrwx  2.0 unx    25628 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_utils.py
--rwxrwxrwx  2.0 unx    12287 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cmake_scanner.py
--rwxrwxrwx  2.0 unx     1750 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cxx_scanner.py
--rwxrwxrwx  2.0 unx     3043 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/func_parser.py
--rwxrwxrwx  2.0 unx     7174 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_parser.py
--rwxrwxrwx  2.0 unx     1464 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_scanner.py
--rwxrwxrwx  2.0 unx     1048 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner.py
--rwxrwxrwx  2.0 unx     1930 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_factory.py
--rwxrwxrwx  2.0 unx     1381 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_utils.py
--rwxrwxrwx  2.0 unx     6416 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scan_api.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/__init__.py
--rwxrwxrwx  2.0 unx     5839 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/comment_delete.py
--rwxrwxrwx  2.0 unx     6934 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/file_matrix.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/__init__.py
--rwxrwxrwx  2.0 unx     4525 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/acc_libs.py
--rwxrwxrwx  2.0 unx     1940 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/api_filter.py
--rwxrwxrwx  2.0 unx    10552 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/ast_visitor.py
--rwxrwxrwx  2.0 unx     5793 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_desc.py
--rwxrwxrwx  2.0 unx     8617 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_handler.py
--rwxrwxrwx  2.0 unx     4199 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_matcher.py
--rwxrwxrwx  2.0 unx     5428 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/__init__.py
--rwxrwxrwx  2.0 unx     6677 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/advisor.py
--rwxrwxrwx  2.0 unx     6732 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/seq_advisor.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/__init__.py
--rwxrwxrwx  2.0 unx     4986 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/clang_finder.py
--rwxrwxrwx  2.0 unx     3503 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/excel.py
--rwxrwxrwx  2.0 unx     1919 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/file_locker.py
--rwxrwxrwx  2.0 unx     2685 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/io_util.py
--rwxrwxrwx  2.0 unx     1970 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/lib_util.py
--rwxrwxrwx  2.0 unx     2638 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/log_util.py
--rwxrwxrwx  2.0 unx     1851 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/security.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/__init__.py
--rwxrwxrwx  2.0 unx    12215 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/utils/file_open_check.py
--rwxrwxrwx  2.0 unx     9893 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/utils/install.py
--rwxrwxrwx  2.0 unx     4690 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/utils/parser.py
--rwxrwxrwx  2.0 unx     8721 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/utils/security_check.py
--rwxrwxrwx  2.0 unx      886 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/utils/util.py
--rwxrwxrwx  2.0 unx      598 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/utils/__init__.py
--rwxrwxrwx  2.0 unx        1 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      147 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/entry_points.txt
--rwxrwxrwx  2.0 unx      228 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/PKG-INFO
--rwxrwxrwx  2.0 unx    23938 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/SOURCES.txt
--rwxrwxrwx  2.0 unx       11 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/top_level.txt
-546 files, 1866056 bytes uncompressed, 575030 bytes compressed:  69.2%
+Zip file size: 692381 bytes, number of entries: 546
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/ms_ait.egg-info/
+-rwxrwxrwx  2.0 unx      228 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/PKG-INFO
+-rwxrwxrwx  2.0 unx     4802 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/README.md
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/requirements.txt
+-rwxrwxrwx  2.0 unx       38 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/setup.cfg
+-rwxrwxrwx  2.0 unx     1855 b- defN 24-May-17 16:26 ms-ait-7.0.0b517/setup.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/profile/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/tensor_view/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/tests/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/utils/
+-rwxrwxrwx  2.0 unx      600 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/__init__.py
+-rwxrwxrwx  2.0 unx     1744 b- defN 24-May-08 11:39 ms-ait-7.0.0b517/components/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/
+-rwxrwxrwx  2.0 unx     5220 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/README.md
+-rwxrwxrwx  2.0 unx       65 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/requirements.txt
+-rwxrwxrwx  2.0 unx     2227 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/analyze/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/analyze/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/data/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/__init__.py
+-rwxrwxrwx  2.0 unx      695 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/analyze/model_evaluation/__install__.py
+-rwxrwxrwx  2.0 unx     5943 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/__main__.py
+-rwxrwxrwx  2.0 unx      843 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/config.py
+-rwxrwxrwx  2.0 unx      936 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/op_info.py
+-rwxrwxrwx  2.0 unx      712 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/
+-rwxrwxrwx  2.0 unx      882 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/const.py
+-rwxrwxrwx  2.0 unx     1078 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/log.py
+-rwxrwxrwx  2.0 unx     1917 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/utils.py
+-rwxrwxrwx  2.0 unx       95 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/__init__.py
+-rwxrwxrwx  2.0 unx     1072 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/atc_err.py
+-rwxrwxrwx  2.0 unx      730 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/engine.py
+-rwxrwxrwx  2.0 unx      712 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/framework.py
+-rwxrwxrwx  2.0 unx      852 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
+-rwxrwxrwx  2.0 unx      692 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/soc_type.py
+-rwxrwxrwx  2.0 unx      305 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/
+-rwxrwxrwx  2.0 unx     7722 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/analysis.py
+-rwxrwxrwx  2.0 unx     4707 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/result.py
+-rwxrwxrwx  2.0 unx     1236 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/rule.py
+-rwxrwxrwx  2.0 unx       51 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/__init__.py
+-rwxrwxrwx  2.0 unx     2495 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/onnx.py
+-rwxrwxrwx  2.0 unx       59 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/__init__.py
+-rwxrwxrwx  2.0 unx     4428 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/data/opp.py
+-rwxrwxrwx  2.0 unx     2212 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/data/op_map.py
+-rwxrwxrwx  2.0 unx      683 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/data/__init__.py
+-rwxrwxrwx  2.0 unx     2210 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/onnx.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/__init__.py
+-rwxrwxrwx  2.0 unx     4426 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/atc.py
+-rwxrwxrwx  2.0 unx     5374 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/model.py
+-rwxrwxrwx  2.0 unx     5339 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/om.py
+-rwxrwxrwx  2.0 unx      750 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/ais_bench/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/backend/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/infer_analyser/
+-rwxrwxrwx  2.0 unx      762 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_infer.py
+-rwxrwxrwx  2.0 unx     1835 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/install.sh
+-rwxrwxrwx  2.0 unx    51061 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/README.md
+-rwxrwxrwx  2.0 unx       26 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/requirements.txt
+-rwxrwxrwx  2.0 unx     1769 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/benchmark/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/benchmark/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/
+-rwxrwxrwx  2.0 unx     2426 b- defN 24-May-09 20:12 ms-ait-7.0.0b517/components/benchmark/ais_bench/install.sh
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/__init__.py
+-rwxrwxrwx  2.0 unx     1763 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/benchmark/ais_bench/__install__.py
+-rwxrwxrwx  2.0 unx      752 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/
+-rwxrwxrwx  2.0 unx     2685 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/interface.py
+-rwxrwxrwx  2.0 unx      759 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/log.py
+-rwxrwxrwx  2.0 unx     1591 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/README.md
+-rwxrwxrwx  2.0 unx     2433 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/recorder.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/__init__.py
+-rwxrwxrwx  2.0 unx     3142 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
+-rwxrwxrwx  2.0 unx     4606 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
+-rwxrwxrwx  2.0 unx     1375 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
+-rwxrwxrwx  2.0 unx     2196 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/download.sh
+-rwxrwxrwx  2.0 unx     3978 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
+-rwxrwxrwx  2.0 unx     4244 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/__init__.py
+-rwxrwxrwx  2.0 unx     2999 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/measurement.py
+-rwxrwxrwx  2.0 unx     1260 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/
+-rwxrwxrwx  2.0 unx     4614 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/args_adapter.py
+-rwxrwxrwx  2.0 unx     7151 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/args_check.py
+-rwxrwxrwx  2.0 unx    31048 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/benchmark_process.py
+-rwxrwxrwx  2.0 unx    37710 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/interface.py
+-rwxrwxrwx  2.0 unx    14389 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/io_oprations.py
+-rwxrwxrwx  2.0 unx    10701 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/main_cli.py
+-rwxrwxrwx  2.0 unx    10444 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/miscellaneous.py
+-rwxrwxrwx  2.0 unx    12012 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/path_security_check.py
+-rwxrwxrwx  2.0 unx     3260 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/registry.py
+-rwxrwxrwx  2.0 unx     9472 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/summary.py
+-rwxrwxrwx  2.0 unx    10122 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/__init__.py
+-rwxrwxrwx  2.0 unx     8700 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/__main__.py
+-rwxrwxrwx  2.0 unx     3025 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/backend.py
+-rwxrwxrwx  2.0 unx     5400 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
+-rwxrwxrwx  2.0 unx      960 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/__init__.py
+-rwxrwxrwx  2.0 unx     1623 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/benchmark/backend/install.sh
+-rwxrwxrwx  2.0 unx     6911 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/backend/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/backend/__init__.py
+-rwxrwxrwx  2.0 unx     2843 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/infer_analyser/analyser.py
+-rwxrwxrwx  2.0 unx     8588 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/infer_analyser/infer_analyser.sh
+-rwxrwxrwx  2.0 unx     1680 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/infer_analyser/info_convert_json.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/benchmark/infer_analyser/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/model_convert/
+-rwxrwxrwx  2.0 unx     1520 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/build.sh
+-rwxrwxrwx  2.0 unx     3162 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/README.md
+-rwxrwxrwx  2.0 unx       43 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/convert/requirements.txt
+-rwxrwxrwx  2.0 unx     2167 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/convert/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/convert/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/model_convert/aie/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/model_convert/aoe/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/model_convert/atc/
+-rwxrwxrwx  2.0 unx     3463 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/cmd_utils.py
+-rwxrwxrwx  2.0 unx     1520 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/convert/model_convert/install.sh
+-rwxrwxrwx  2.0 unx      590 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/__init__.py
+-rwxrwxrwx  2.0 unx     1382 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/convert/model_convert/__install__.py
+-rwxrwxrwx  2.0 unx     3982 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/convert/model_convert/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/convert/model_convert/aie/core/
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aie/__init__.py
+-rwxrwxrwx  2.0 unx      775 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/config.py
+-rwxrwxrwx  2.0 unx      646 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/__init__.py
+-rwxrwxrwx  2.0 unx     2221 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aie/core/convert.py
+-rwxrwxrwx  2.0 unx      591 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aie/core/__init__.py
+-rwxrwxrwx  2.0 unx     9218 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aoe/aoe_args_map.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/aoe/__init__.py
+-rwxrwxrwx  2.0 unx    12775 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/atc/atc_args_map.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/convert/model_convert/atc/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/
+-rwxrwxrwx  2.0 unx      787 b- defN 24-May-08 11:39 ms-ait-7.0.0b517/components/debug/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/
+-rwxrwxrwx  2.0 unx     5324 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/main.py
+-rwxrwxrwx  2.0 unx    11876 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/README.md
+-rwxrwxrwx  2.0 unx      160 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/requirements.txt
+-rwxrwxrwx  2.0 unx     2317 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/compare/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/compare/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/
+-rwxrwxrwx  2.0 unx    24580 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/cmp_process.py
+-rwxrwxrwx  2.0 unx     2181 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/install.sh
+-rwxrwxrwx  2.0 unx     5359 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
+-rwxrwxrwx  2.0 unx     5175 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf_debug_runner.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__init__.py
+-rwxrwxrwx  2.0 unx     1716 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__install__.py
+-rwxrwxrwx  2.0 unx     7990 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__main__.py
+-rwxrwxrwx  2.0 unx     5723 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
+-rwxrwxrwx  2.0 unx     2293 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/__init__.py
+-rwxrwxrwx  2.0 unx     3526 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/atc_utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/__init__.py
+-rwxrwxrwx  2.0 unx     5651 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/__init__.py
+-rwxrwxrwx  2.0 unx     8737 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/args_check.py
+-rwxrwxrwx  2.0 unx     3621 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/convert.py
+-rwxrwxrwx  2.0 unx     4757 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/dump_data.py
+-rwxrwxrwx  2.0 unx     1309 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
+-rwxrwxrwx  2.0 unx     6098 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/tf_common.py
+-rwxrwxrwx  2.0 unx    23475 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/__init__.py
+-rwxrwxrwx  2.0 unx    11004 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/analyser.py
+-rwxrwxrwx  2.0 unx    15491 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/net_compare.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/__init__.py
+-rwxrwxrwx  2.0 unx    26647 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/npu_dump_data.py
+-rwxrwxrwx  2.0 unx    17174 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/om_parser.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/__init__.py
+-rwxrwxrwx  2.0 unx     9202 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/custom_op.py
+-rwxrwxrwx  2.0 unx    15937 b- defN 24-May-14 19:57 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/__init__.py
+-rwxrwxrwx  2.0 unx      619 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/__init__.py
+-rwxrwxrwx  2.0 unx     7707 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/single_op.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/__init__.py
+-rwxrwxrwx  2.0 unx    13711 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/tf_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/
+-rwxrwxrwx  2.0 unx    11087 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/README.md
+-rwxrwxrwx  2.0 unx      140 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/requirements.txt
+-rwxrwxrwx  2.0 unx     2811 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/surgeon/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/
+-rwxrwxrwx  2.0 unx    15282 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/ait_main.py
+-rwxrwxrwx  2.0 unx     5587 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/options.py
+-rwxrwxrwx  2.0 unx      878 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__init__.py
+-rwxrwxrwx  2.0 unx     1160 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__install__.py
+-rwxrwxrwx  2.0 unx     6305 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__main__.py
+-rwxrwxrwx  2.0 unx     6012 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/args_check.py
+-rwxrwxrwx  2.0 unx     8574 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/click_utils.py
+-rwxrwxrwx  2.0 unx     2307 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/config.py
+-rwxrwxrwx  2.0 unx     1633 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/log.py
+-rwxrwxrwx  2.0 unx     2265 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/register.py
+-rwxrwxrwx  2.0 unx      880 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/singleton.py
+-rwxrwxrwx  2.0 unx     5111 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/utils.py
+-rwxrwxrwx  2.0 unx     1032 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/__init__.py
+-rwxrwxrwx  2.0 unx    11302 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+-rwxrwxrwx  2.0 unx       85 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
+-rwxrwxrwx  2.0 unx     2102 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
+-rwxrwxrwx  2.0 unx      784 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
+-rwxrwxrwx  2.0 unx    28389 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
+-rwxrwxrwx  2.0 unx     8101 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
+-rwxrwxrwx  2.0 unx      755 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
+-rwxrwxrwx  2.0 unx    28573 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
+-rwxrwxrwx  2.0 unx     4880 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+-rwxrwxrwx  2.0 unx      747 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
+-rwxrwxrwx  2.0 unx     4582 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
+-rwxrwxrwx  2.0 unx     5214 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/README.md
+-rwxrwxrwx  2.0 unx     1024 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
+-rwxrwxrwx  2.0 unx      736 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
+-rwxrwxrwx  2.0 unx     1694 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
+-rwxrwxrwx  2.0 unx     2074 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
+-rwxrwxrwx  2.0 unx     1390 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
+-rwxrwxrwx  2.0 unx     4242 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
+-rwxrwxrwx  2.0 unx     1556 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
+-rwxrwxrwx  2.0 unx     2736 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
+-rwxrwxrwx  2.0 unx      719 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
+-rwxrwxrwx  2.0 unx     2234 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
+-rwxrwxrwx  2.0 unx      679 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
+-rwxrwxrwx  2.0 unx     1342 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
+-rwxrwxrwx  2.0 unx     1404 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
+-rwxrwxrwx  2.0 unx     1387 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
+-rwxrwxrwx  2.0 unx     5279 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/
+-rwxrwxrwx  2.0 unx     1565 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
+-rwxrwxrwx  2.0 unx    15557 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/matcher.py
+-rwxrwxrwx  2.0 unx     7709 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/pattern.py
+-rwxrwxrwx  2.0 unx     6596 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/utils.py
+-rwxrwxrwx  2.0 unx     2028 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
+-rwxrwxrwx  2.0 unx     5589 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
+-rwxrwxrwx  2.0 unx     7914 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
+-rwxrwxrwx  2.0 unx     6563 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
+-rwxrwxrwx  2.0 unx     6124 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
+-rwxrwxrwx  2.0 unx    12418 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
+-rwxrwxrwx  2.0 unx     5534 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
+-rwxrwxrwx  2.0 unx    11185 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
+-rwxrwxrwx  2.0 unx    10165 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
+-rwxrwxrwx  2.0 unx     6285 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
+-rwxrwxrwx  2.0 unx     7235 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
+-rwxrwxrwx  2.0 unx     6958 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
+-rwxrwxrwx  2.0 unx     3107 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
+-rwxrwxrwx  2.0 unx    10959 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
+-rwxrwxrwx  2.0 unx    19159 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
+-rwxrwxrwx  2.0 unx     5350 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
+-rwxrwxrwx  2.0 unx     8097 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
+-rwxrwxrwx  2.0 unx    25805 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
+-rwxrwxrwx  2.0 unx     1665 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
+-rwxrwxrwx  2.0 unx    16842 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
+-rwxrwxrwx  2.0 unx     5031 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
+-rwxrwxrwx  2.0 unx    13241 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
+-rwxrwxrwx  2.0 unx     8003 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
+-rwxrwxrwx  2.0 unx     6050 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/inference.py
+-rwxrwxrwx  2.0 unx     1559 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/log.py
+-rwxrwxrwx  2.0 unx      505 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/README.md
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/
+-rwxrwxrwx  2.0 unx    10044 b- defN 24-May-08 11:27 ms-ait-7.0.0b517/components/llm/README.md
+-rwxrwxrwx  2.0 unx      108 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/requirements.txt
+-rwxrwxrwx  2.0 unx     2370 b- defN 24-May-09 20:12 ms-ait-7.0.0b517/components/llm/setup.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/llm/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/dump/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/metrics/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/transform/
+-rwxrwxrwx  2.0 unx      903 b- defN 24-May-09 18:08 ms-ait-7.0.0b517/components/llm/ait_llm/install.sh
+-rwxrwxrwx  2.0 unx      920 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/__init__.py
+-rwxrwxrwx  2.0 unx     1792 b- defN 24-May-09 20:12 ms-ait-7.0.0b517/components/llm/ait_llm/__install__.py
+-rwxrwxrwx  2.0 unx    14898 b- defN 24-May-09 19:39 ms-ait-7.0.0b517/components/llm/ait_llm/__main__.py
+-rwxrwxrwx  2.0 unx     2609 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/common/constant.py
+-rwxrwxrwx  2.0 unx     4826 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/common/json_fitter.py
+-rwxrwxrwx  2.0 unx     1581 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/common/log.py
+-rwxrwxrwx  2.0 unx     3267 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/common/tool.py
+-rwxrwxrwx  2.0 unx     4657 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/common/utils.py
+-rwxrwxrwx  2.0 unx     8522 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/common/validate.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/common/__init__.py
+-rwxrwxrwx  2.0 unx    22815 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/compare/atb_acc_cmp.py
+-rwxrwxrwx  2.0 unx     5949 b- defN 24-May-09 19:39 ms-ait-7.0.0b517/components/llm/ait_llm/compare/cmp_algorithm.py
+-rwxrwxrwx  2.0 unx     8511 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/compare/cmp_utils.py
+-rwxrwxrwx  2.0 unx      957 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/compare/op_mapping.py
+-rwxrwxrwx  2.0 unx    19113 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/compare/torchair_acc_cmp.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/compare/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/
+-rwxrwxrwx  2.0 unx     8268 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/initial.py
+-rwxrwxrwx  2.0 unx     2576 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/manual_dump.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/__init__.py
+-rwxrwxrwx  2.0 unx     2445 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
+-rwxrwxrwx  2.0 unx       91 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/__init__.py
+-rwxrwxrwx  2.0 unx     3413 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/dump_config.py
+-rwxrwxrwx  2.0 unx     7648 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/dump_hook.py
+-rwxrwxrwx  2.0 unx     1647 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/hook.py
+-rwxrwxrwx  2.0 unx     3067 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/hook_ops.py
+-rwxrwxrwx  2.0 unx     7174 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/topo.py
+-rwxrwxrwx  2.0 unx      722 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/__init__.py
+-rwxrwxrwx  2.0 unx     4755 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/process.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/__init__.py
+-rwxrwxrwx  2.0 unx     5241 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/metrics/case_filter.py
+-rwxrwxrwx  2.0 unx    10300 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/metrics/metrics.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/metrics/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/
+-rwxrwxrwx  2.0 unx     1645 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/case_manager.py
+-rwxrwxrwx  2.0 unx    15632 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/opchecker.py
+-rwxrwxrwx  2.0 unx    13397 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/operation_test.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/__init__.py
+-rwxrwxrwx  2.0 unx     3879 b- defN 24-May-09 20:12 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/build.sh
+-rwxrwxrwx  2.0 unx      938 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
+-rwxrwxrwx  2.0 unx    29744 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
+-rwxrwxrwx  2.0 unx     1354 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/__init__.py
+-rwxrwxrwx  2.0 unx     4577 b- defN 24-May-13 12:29 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/activation.py
+-rwxrwxrwx  2.0 unx     1301 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/all_gather.py
+-rwxrwxrwx  2.0 unx     3447 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/all_reduce.py
+-rwxrwxrwx  2.0 unx     1469 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/as_strided.py
+-rwxrwxrwx  2.0 unx     1286 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/broadcast.py
+-rwxrwxrwx  2.0 unx     1319 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/concat.py
+-rwxrwxrwx  2.0 unx     1197 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/cumsum.py
+-rwxrwxrwx  2.0 unx     5721 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/elewise.py
+-rwxrwxrwx  2.0 unx     1783 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
+-rwxrwxrwx  2.0 unx     1975 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
+-rwxrwxrwx  2.0 unx     1592 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fill.py
+-rwxrwxrwx  2.0 unx     2707 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/gather.py
+-rwxrwxrwx  2.0 unx     1453 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
+-rwxrwxrwx  2.0 unx     1274 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/kv_cache.py
+-rwxrwxrwx  2.0 unx     4084 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/layer_norm.py
+-rwxrwxrwx  2.0 unx     2754 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear.py
+-rwxrwxrwx  2.0 unx     1165 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
+-rwxrwxrwx  2.0 unx     2838 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
+-rwxrwxrwx  2.0 unx     2631 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/matmul.py
+-rwxrwxrwx  2.0 unx     1903 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/multinomial.py
+-rwxrwxrwx  2.0 unx     1307 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/pad.py
+-rwxrwxrwx  2.0 unx     1247 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/paged_attention.py
+-rwxrwxrwx  2.0 unx     1372 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/reduce.py
+-rwxrwxrwx  2.0 unx     1210 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/repeat.py
+-rwxrwxrwx  2.0 unx     1283 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
+-rwxrwxrwx  2.0 unx     3504 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rms_norm.py
+-rwxrwxrwx  2.0 unx     6893 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rope.py
+-rwxrwxrwx  2.0 unx     1942 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rope_grad.py
+-rwxrwxrwx  2.0 unx     9651 b- defN 24-May-17 16:25 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/self_attention.py
+-rwxrwxrwx  2.0 unx     1434 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/set_value.py
+-rwxrwxrwx  2.0 unx     2261 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/slice.py
+-rwxrwxrwx  2.0 unx     1222 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/softmax.py
+-rwxrwxrwx  2.0 unx     1233 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/sort.py
+-rwxrwxrwx  2.0 unx     1368 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/split.py
+-rwxrwxrwx  2.0 unx     3198 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
+-rwxrwxrwx  2.0 unx     2677 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
+-rwxrwxrwx  2.0 unx     4783 b- defN 24-May-13 12:29 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/transdata.py
+-rwxrwxrwx  2.0 unx     1196 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/transpose.py
+-rwxrwxrwx  2.0 unx     2143 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/unpad.py
+-rwxrwxrwx  2.0 unx      935 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/where.py
+-rwxrwxrwx  2.0 unx     5680 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/__init__.py
+-rwxrwxrwx  2.0 unx    12784 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/transform/transform_quant.py
+-rwxrwxrwx  2.0 unx    22320 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
+-rwxrwxrwx  2.0 unx     2542 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/transform/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/llm/ait_llm/transform/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/profile/msprof/
+-rwxrwxrwx  2.0 unx      602 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/profile/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/
+-rwxrwxrwx  2.0 unx     1835 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/install.sh
+-rwxrwxrwx  2.0 unx     5011 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/README.md
+-rwxrwxrwx  2.0 unx       10 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/requirements.txt
+-rwxrwxrwx  2.0 unx     1581 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/profile/msprof/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/profile/msprof/__init__.py
+-rwxrwxrwx  2.0 unx     4154 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/api.py
+-rwxrwxrwx  2.0 unx     1277 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/args_adapter.py
+-rwxrwxrwx  2.0 unx     4565 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/main_cli.py
+-rwxrwxrwx  2.0 unx     4314 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/msprof_process.py
+-rwxrwxrwx  2.0 unx      760 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__init__.py
+-rwxrwxrwx  2.0 unx      694 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__install__.py
+-rwxrwxrwx  2.0 unx     4513 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/
+-rwxrwxrwx  2.0 unx       14 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/requirements.txt
+-rwxrwxrwx  2.0 unx     1615 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/__init__.py
+-rwxrwxrwx  2.0 unx     2261 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/atb.py
+-rwxrwxrwx  2.0 unx     2240 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/handler.py
+-rwxrwxrwx  2.0 unx     1035 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/logger.py
+-rwxrwxrwx  2.0 unx     3438 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/main_cli.py
+-rwxrwxrwx  2.0 unx     3921 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/operation.py
+-rwxrwxrwx  2.0 unx      874 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/print_stat.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/__init__.py
+-rwxrwxrwx  2.0 unx      702 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/__install__.py
+-rwxrwxrwx  2.0 unx     3123 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/tests/test_ait.sh
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/tests/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/
+-rwxrwxrwx  2.0 unx    10875 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/install.bat
+-rwxrwxrwx  2.0 unx     4111 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/install.sh
+-rwxrwxrwx  2.0 unx    23645 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/README.md
+-rwxrwxrwx  2.0 unx       94 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/transplt/requirements.txt
+-rwxrwxrwx  2.0 unx     2329 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/transplt/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/transplt/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/exception/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/report/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/solution/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/
+-rwxrwxrwx  2.0 unx    10875 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/transplt/app_analyze/install.bat
+-rwxrwxrwx  2.0 unx     4481 b- defN 24-May-09 20:12 ms-ait-7.0.0b517/components/transplt/app_analyze/install.sh
+-rwxrwxrwx  2.0 unx      596 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/__init__.py
+-rwxrwxrwx  2.0 unx     2441 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/transplt/app_analyze/__install__.py
+-rwxrwxrwx  2.0 unx     3444 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/__main__.py
+-rwxrwxrwx  2.0 unx    11196 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/common/kit_config.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/common/__init__.py
+-rwxrwxrwx  2.0 unx     2257 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/exception/exception_information.py
+-rwxrwxrwx  2.0 unx     3419 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/exception/source_scan_exception.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/exception/__init__.py
+-rwxrwxrwx  2.0 unx     4850 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/model/model.py
+-rwxrwxrwx  2.0 unx     6911 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/model/project.py
+-rwxrwxrwx  2.0 unx     3765 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/model/seq_project.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/model/__init__.py
+-rwxrwxrwx  2.0 unx      983 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/app.py
+-rwxrwxrwx  2.0 unx     5752 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/cmdline_input.py
+-rwxrwxrwx  2.0 unx     1686 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/custom_input.py
+-rwxrwxrwx  2.0 unx     1467 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/input_factory.py
+-rwxrwxrwx  2.0 unx     2601 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/porting_input.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/porting/__init__.py
+-rwxrwxrwx  2.0 unx     1760 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/report/csv_report.py
+-rwxrwxrwx  2.0 unx     1775 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/report/json_report.py
+-rwxrwxrwx  2.0 unx     2202 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/report/report.py
+-rwxrwxrwx  2.0 unx     1814 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/report/report_factory.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/report/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/
+drwxrwxrwx  2.0 unx        0 b- stor 24-May-17 16:27 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/
+-rwxrwxrwx  2.0 unx    16004 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/clang_parser.py
+-rwxrwxrwx  2.0 unx    25628 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/clang_utils.py
+-rwxrwxrwx  2.0 unx    12287 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/cmake_scanner.py
+-rwxrwxrwx  2.0 unx     1750 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/cxx_scanner.py
+-rwxrwxrwx  2.0 unx     3043 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/func_parser.py
+-rwxrwxrwx  2.0 unx     7174 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/python_parser.py
+-rwxrwxrwx  2.0 unx     1464 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/python_scanner.py
+-rwxrwxrwx  2.0 unx     1048 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner.py
+-rwxrwxrwx  2.0 unx     1930 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner_factory.py
+-rwxrwxrwx  2.0 unx     1381 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner_utils.py
+-rwxrwxrwx  2.0 unx     6416 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scan_api.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/__init__.py
+-rwxrwxrwx  2.0 unx     5839 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/comment_delete.py
+-rwxrwxrwx  2.0 unx     6934 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/file_matrix.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/__init__.py
+-rwxrwxrwx  2.0 unx     4525 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/acc_libs.py
+-rwxrwxrwx  2.0 unx     1940 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/api_filter.py
+-rwxrwxrwx  2.0 unx    10552 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+-rwxrwxrwx  2.0 unx     5793 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_desc.py
+-rwxrwxrwx  2.0 unx     8617 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_handler.py
+-rwxrwxrwx  2.0 unx     4199 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+-rwxrwxrwx  2.0 unx     5428 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/__init__.py
+-rwxrwxrwx  2.0 unx     6677 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/solution/advisor.py
+-rwxrwxrwx  2.0 unx     6732 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/solution/seq_advisor.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/solution/__init__.py
+-rwxrwxrwx  2.0 unx     4986 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/clang_finder.py
+-rwxrwxrwx  2.0 unx     3503 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/excel.py
+-rwxrwxrwx  2.0 unx     1919 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/file_locker.py
+-rwxrwxrwx  2.0 unx     2685 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/io_util.py
+-rwxrwxrwx  2.0 unx     1970 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/lib_util.py
+-rwxrwxrwx  2.0 unx     2638 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/log_util.py
+-rwxrwxrwx  2.0 unx     1851 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/security.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b517/components/transplt/app_analyze/utils/__init__.py
+-rwxrwxrwx  2.0 unx    12215 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/utils/file_open_check.py
+-rwxrwxrwx  2.0 unx     9893 b- defN 24-May-09 20:12 ms-ait-7.0.0b517/components/utils/install.py
+-rwxrwxrwx  2.0 unx     4690 b- defN 24-May-08 11:39 ms-ait-7.0.0b517/components/utils/parser.py
+-rwxrwxrwx  2.0 unx     8721 b- defN 24-May-08 10:39 ms-ait-7.0.0b517/components/utils/security_check.py
+-rwxrwxrwx  2.0 unx      886 b- defN 24-May-08 11:39 ms-ait-7.0.0b517/components/utils/util.py
+-rwxrwxrwx  2.0 unx      598 b- defN 24-May-09 14:03 ms-ait-7.0.0b517/components/utils/__init__.py
+-rwxrwxrwx  2.0 unx        1 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/ms_ait.egg-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      147 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/ms_ait.egg-info/entry_points.txt
+-rwxrwxrwx  2.0 unx      228 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/ms_ait.egg-info/PKG-INFO
+-rwxrwxrwx  2.0 unx    23938 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/ms_ait.egg-info/SOURCES.txt
+-rwxrwxrwx  2.0 unx       11 b- defN 24-May-17 16:27 ms-ait-7.0.0b517/ms_ait.egg-info/top_level.txt
+546 files, 1869225 bytes uncompressed, 575961 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,1639 +1,1639 @@
-Filename: ms-ait-7.0.0b430/
+Filename: ms-ait-7.0.0b517/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/
+Filename: ms-ait-7.0.0b517/components/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/
+Filename: ms-ait-7.0.0b517/ms_ait.egg-info/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/PKG-INFO
+Filename: ms-ait-7.0.0b517/PKG-INFO
 Comment: 
 
-Filename: ms-ait-7.0.0b430/README.md
+Filename: ms-ait-7.0.0b517/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/requirements.txt
+Filename: ms-ait-7.0.0b517/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/setup.cfg
+Filename: ms-ait-7.0.0b517/setup.cfg
 Comment: 
 
-Filename: ms-ait-7.0.0b430/setup.py
+Filename: ms-ait-7.0.0b517/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/
+Filename: ms-ait-7.0.0b517/components/analyze/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/
+Filename: ms-ait-7.0.0b517/components/benchmark/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/
+Filename: ms-ait-7.0.0b517/components/convert/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/
+Filename: ms-ait-7.0.0b517/components/debug/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/
+Filename: ms-ait-7.0.0b517/components/llm/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/
+Filename: ms-ait-7.0.0b517/components/profile/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/
+Filename: ms-ait-7.0.0b517/components/tensor_view/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tests/
+Filename: ms-ait-7.0.0b517/components/tests/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/
+Filename: ms-ait-7.0.0b517/components/transplt/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/
+Filename: ms-ait-7.0.0b517/components/utils/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/__init__.py
+Filename: ms-ait-7.0.0b517/components/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/__main__.py
+Filename: ms-ait-7.0.0b517/components/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/README.md
+Filename: ms-ait-7.0.0b517/components/analyze/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/requirements.txt
+Filename: ms-ait-7.0.0b517/components/analyze/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/setup.py
+Filename: ms-ait-7.0.0b517/components/analyze/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/data/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/__install__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/__main__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/config.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/op_info.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/op_info.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/const.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/const.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/log.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/utils.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/atc_err.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/atc_err.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/engine.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/engine.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/framework.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/framework.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/soc_type.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/soc_type.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/analysis.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/analysis.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/result.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/result.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/rule.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/rule.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/onnx.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/onnx.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/opp.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/data/opp.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/op_map.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/data/op_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/data/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/onnx.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/onnx.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/atc.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/atc.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/model.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/model.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/om.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/om.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/__init__.py
+Filename: ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/
+Filename: ms-ait-7.0.0b517/components/benchmark/backend/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/
+Filename: ms-ait-7.0.0b517/components/benchmark/infer_analyser/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_infer.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_infer.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/install.sh
+Filename: ms-ait-7.0.0b517/components/benchmark/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/README.md
+Filename: ms-ait-7.0.0b517/components/benchmark/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/requirements.txt
+Filename: ms-ait-7.0.0b517/components/benchmark/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/setup.py
+Filename: ms-ait-7.0.0b517/components/benchmark/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/install.sh
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/__install__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/__main__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/interface.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/interface.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/log.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/README.md
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/recorder.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/recorder.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/download.sh
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/download.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/measurement.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_adapter.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_check.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/benchmark_process.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/benchmark_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/interface.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/interface.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/io_oprations.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/io_oprations.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/main_cli.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/main_cli.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/miscellaneous.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/miscellaneous.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/path_security_check.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/path_security_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/registry.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/registry.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/summary.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/summary.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/utils.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__main__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/backend.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/install.sh
+Filename: ms-ait-7.0.0b517/components/benchmark/backend/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/setup.py
+Filename: ms-ait-7.0.0b517/components/benchmark/backend/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/backend/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/analyser.py
+Filename: ms-ait-7.0.0b517/components/benchmark/infer_analyser/analyser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/infer_analyser.sh
+Filename: ms-ait-7.0.0b517/components/benchmark/infer_analyser/infer_analyser.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/info_convert_json.py
+Filename: ms-ait-7.0.0b517/components/benchmark/infer_analyser/info_convert_json.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/__init__.py
+Filename: ms-ait-7.0.0b517/components/benchmark/infer_analyser/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/build.sh
+Filename: ms-ait-7.0.0b517/components/convert/build.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/README.md
+Filename: ms-ait-7.0.0b517/components/convert/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/requirements.txt
+Filename: ms-ait-7.0.0b517/components/convert/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/setup.py
+Filename: ms-ait-7.0.0b517/components/convert/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aoe/
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aoe/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/atc/
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/atc/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/cmd_utils.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/cmd_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/install.sh
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/__install__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/__main__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/core/
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/core/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/config.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/core/convert.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/core/convert.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/core/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aie/core/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aoe/aoe_args_map.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aoe/aoe_args_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aoe/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/aoe/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/atc/atc_args_map.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/atc/atc_args_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/atc/__init__.py
+Filename: ms-ait-7.0.0b517/components/convert/model_convert/atc/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/
+Filename: ms-ait-7.0.0b517/components/debug/compare/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/main.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/main.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/README.md
+Filename: ms-ait-7.0.0b517/components/debug/compare/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/requirements.txt
+Filename: ms-ait-7.0.0b517/components/debug/compare/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/setup.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/cmp_process.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/cmp_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/install.sh
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf_debug_runner.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf_debug_runner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__install__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__main__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/atc_utils.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/atc_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/args_check.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/convert.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/convert.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dump_data.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/tf_common.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/tf_common.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/utils.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/analyser.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/analyser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/net_compare.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/net_compare.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/npu_dump_data.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/npu_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/om_parser.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/om_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/custom_op.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/custom_op.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/single_op.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/single_op.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/tf_dump_data.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/tf_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/README.md
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/requirements.txt
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/setup.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/ait_main.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/ait_main.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/options.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/options.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__install__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__main__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/args_check.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/click_utils.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/click_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/config.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/log.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/register.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/register.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/singleton.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/singleton.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/utils.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/README.md
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/matcher.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/matcher.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/pattern.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/pattern.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/utils.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/inference.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/log.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/README.md
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/__init__.py
+Filename: ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/README.md
+Filename: ms-ait-7.0.0b517/components/llm/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/requirements.txt
+Filename: ms-ait-7.0.0b517/components/llm/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/setup.py
+Filename: ms-ait-7.0.0b517/components/llm/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/metrics/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/transform/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/install.sh
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/__install__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/__main__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/constant.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/constant.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/json_fitter.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/json_fitter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/log.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/tool.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/tool.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/utils.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/validate.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/validate.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/atb_acc_cmp.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/atb_acc_cmp.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_algorithm.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/cmp_algorithm.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_utils.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/cmp_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/op_mapping.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/op_mapping.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/torchair_acc_cmp.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/torchair_acc_cmp.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/initial.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/initial.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/manual_dump.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/manual_dump.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_config.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/dump_config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_hook.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/dump_hook.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/hook.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook_ops.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/hook_ops.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/topo.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/topo.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/process.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/case_filter.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/metrics/case_filter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/metrics.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/metrics/metrics.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/metrics/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/case_manager.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/case_manager.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/opchecker.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/opchecker.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/operation_test.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/operation_test.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/build.sh
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/build.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/activation.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/activation.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_gather.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/all_gather.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_reduce.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/all_reduce.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/as_strided.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/as_strided.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/broadcast.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/broadcast.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/concat.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/concat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/cumsum.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/cumsum.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/elewise.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/elewise.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fill.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fill.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/gather.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/gather.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/kv_cache.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/kv_cache.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/layer_norm.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/layer_norm.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/matmul.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/matmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/multinomial.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/multinomial.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/pad.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/pad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/paged_attention.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/paged_attention.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reduce.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/reduce.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/repeat.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/repeat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rms_norm.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rms_norm.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rope.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope_grad.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rope_grad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/self_attention.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/self_attention.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/set_value.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/set_value.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/slice.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/slice.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/softmax.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/softmax.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/sort.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/sort.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/split.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/split.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transdata.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/transdata.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transpose.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/transpose.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/unpad.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/unpad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/where.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/where.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/transform/transform_quant.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/utils.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/transform/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/__init__.py
+Filename: ms-ait-7.0.0b517/components/llm/ait_llm/transform/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/
+Filename: ms-ait-7.0.0b517/components/profile/msprof/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/__init__.py
+Filename: ms-ait-7.0.0b517/components/profile/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/install.sh
+Filename: ms-ait-7.0.0b517/components/profile/msprof/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/README.md
+Filename: ms-ait-7.0.0b517/components/profile/msprof/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/requirements.txt
+Filename: ms-ait-7.0.0b517/components/profile/msprof/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/setup.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/__init__.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/api.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/api.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/args_adapter.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/main_cli.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/main_cli.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/msprof_process.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/msprof_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/utils.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__init__.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__install__.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__main__.py
+Filename: ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/requirements.txt
+Filename: ms-ait-7.0.0b517/components/tensor_view/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/setup.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/__init__.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/atb.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/atb.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/handler.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/handler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/logger.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/logger.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/main_cli.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/main_cli.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/operation.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/operation.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/print_stat.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/print_stat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__init__.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__install__.py
+Filename: ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tests/test_ait.sh
+Filename: ms-ait-7.0.0b517/components/tests/test_ait.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tests/__init__.py
+Filename: ms-ait-7.0.0b517/components/tests/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/install.bat
+Filename: ms-ait-7.0.0b517/components/transplt/install.bat
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/install.sh
+Filename: ms-ait-7.0.0b517/components/transplt/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/README.md
+Filename: ms-ait-7.0.0b517/components/transplt/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/requirements.txt
+Filename: ms-ait-7.0.0b517/components/transplt/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/setup.py
+Filename: ms-ait-7.0.0b517/components/transplt/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/common/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/exception/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/report/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/solution/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/install.bat
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/install.bat
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/install.sh
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/__install__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/__main__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/common/kit_config.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/common/kit_config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/common/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/exception_information.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/exception/exception_information.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/source_scan_exception.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/exception/source_scan_exception.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/exception/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/model.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/model/model.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/project.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/model/project.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/seq_project.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/model/seq_project.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/app.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/app.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/cmdline_input.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/cmdline_input.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/custom_input.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/custom_input.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/input_factory.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/input_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/porting_input.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/porting_input.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/porting/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/csv_report.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/report/csv_report.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/json_report.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/report/json_report.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/report.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/report/report.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/report_factory.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/report/report_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/report/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_parser.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/clang_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_utils.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/clang_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cmake_scanner.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/cmake_scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cxx_scanner.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/cxx_scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/func_parser.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/func_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_parser.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/python_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_scanner.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/python_scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_factory.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_utils.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scan_api.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scan_api.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/comment_delete.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/comment_delete.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/file_matrix.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/file_matrix.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/acc_libs.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/acc_libs.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/api_filter.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/api_filter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/ast_visitor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_desc.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_desc.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_handler.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_handler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_matcher.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_utils.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/advisor.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/solution/advisor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/seq_advisor.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/solution/seq_advisor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/solution/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/clang_finder.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/clang_finder.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/excel.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/excel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/file_locker.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/file_locker.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/io_util.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/io_util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/lib_util.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/lib_util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/log_util.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/log_util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/security.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/security.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/__init__.py
+Filename: ms-ait-7.0.0b517/components/transplt/app_analyze/utils/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/file_open_check.py
+Filename: ms-ait-7.0.0b517/components/utils/file_open_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/install.py
+Filename: ms-ait-7.0.0b517/components/utils/install.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/parser.py
+Filename: ms-ait-7.0.0b517/components/utils/parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/security_check.py
+Filename: ms-ait-7.0.0b517/components/utils/security_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/util.py
+Filename: ms-ait-7.0.0b517/components/utils/util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/__init__.py
+Filename: ms-ait-7.0.0b517/components/utils/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/dependency_links.txt
+Filename: ms-ait-7.0.0b517/ms_ait.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/entry_points.txt
+Filename: ms-ait-7.0.0b517/ms_ait.egg-info/entry_points.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/PKG-INFO
+Filename: ms-ait-7.0.0b517/ms_ait.egg-info/PKG-INFO
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/SOURCES.txt
+Filename: ms-ait-7.0.0b517/ms_ait.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/top_level.txt
+Filename: ms-ait-7.0.0b517/ms_ait.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `ms-ait-7.0.0b430/README.md` & `ms-ait-7.0.0b517/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/setup.py` & `ms-ait-7.0.0b517/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ait_sub_task_entry_points = [
     f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
     for t in ait_sub_tasks
 ]
 
 setup(
     name='ms-ait',
-    version='7.0.0b430',
+    version='7.0.0b517',
     description='AIT, Ascend Inference Tools',
     long_description_content_type='text/markdown',
     url='https://gitee.com/ascend/ait',
     packages=find_packages(),
     package_data={
         '': [
             'LICENSE',
```

## Comparing `ms-ait-7.0.0b430/components/__init__.py` & `ms-ait-7.0.0b517/components/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/__main__.py` & `ms-ait-7.0.0b517/components/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/README.md` & `ms-ait-7.0.0b517/components/analyze/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/setup.py` & `ms-ait-7.0.0b517/components/analyze/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/__init__.py` & `ms-ait-7.0.0b517/components/analyze/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/__install__.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/__main__.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/config.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/op_info.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/op_info.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/__init__.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/bean/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/const.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/const.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/log.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/utils.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/atc_err.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/atc_err.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/engine.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/engine.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/framework.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/framework.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/onnx_checker_err.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/onnx_checker_err.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/soc_type.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/common/enum/soc_type.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/analysis.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/core/analysis.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/result.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/core/result.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/rule.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/core/rule.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/onnx.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/core/checker/onnx.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/data/opp.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/data/opp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/data/op_map.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/data/op_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/data/__init__.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/data/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/onnx.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/graph/onnx.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/atc.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/atc.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/model.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/model.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/om.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/om.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/__init__.py` & `ms-ait-7.0.0b517/components/analyze/model_evaluation/parser/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_infer.py` & `ms-ait-7.0.0b517/components/benchmark/ais_infer.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/install.sh` & `ms-ait-7.0.0b517/components/benchmark/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/README.md` & `ms-ait-7.0.0b517/components/benchmark/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/setup.py` & `ms-ait-7.0.0b517/components/benchmark/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/__init__.py` & `ms-ait-7.0.0b517/components/benchmark/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/install.sh` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/__install__.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/__main__.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/interface.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/interface.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/log.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/README.md` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/recorder.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/recorder.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/download.sh` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/download.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/measurement.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_adapter.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_check.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/benchmark_process.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/benchmark_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/interface.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/interface.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/io_oprations.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/io_oprations.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/main_cli.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/main_cli.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/miscellaneous.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/miscellaneous.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/path_security_check.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/path_security_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/registry.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/registry.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/summary.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/summary.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/utils.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__main__.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/backend.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend_trtexec.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/backend_trtexec.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/__init__.py` & `ms-ait-7.0.0b517/components/benchmark/ais_bench/infer/backends/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/backend/install.sh` & `ms-ait-7.0.0b517/components/benchmark/backend/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/backend/setup.py` & `ms-ait-7.0.0b517/components/benchmark/backend/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/infer_analyser/analyser.py` & `ms-ait-7.0.0b517/components/benchmark/infer_analyser/analyser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/infer_analyser/infer_analyser.sh` & `ms-ait-7.0.0b517/components/benchmark/infer_analyser/infer_analyser.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/infer_analyser/info_convert_json.py` & `ms-ait-7.0.0b517/components/benchmark/infer_analyser/info_convert_json.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/build.sh` & `ms-ait-7.0.0b517/components/convert/build.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/README.md` & `ms-ait-7.0.0b517/components/convert/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/setup.py` & `ms-ait-7.0.0b517/components/convert/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/__init__.py` & `ms-ait-7.0.0b517/components/convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/cmd_utils.py` & `ms-ait-7.0.0b517/components/convert/model_convert/cmd_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/install.sh` & `ms-ait-7.0.0b517/components/convert/model_convert/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/__init__.py` & `ms-ait-7.0.0b517/components/convert/model_convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/__install__.py` & `ms-ait-7.0.0b517/components/convert/model_convert/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/__main__.py` & `ms-ait-7.0.0b517/components/convert/model_convert/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/config.py` & `ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/__init__.py` & `ms-ait-7.0.0b517/components/convert/model_convert/aie/bean/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/core/convert.py` & `ms-ait-7.0.0b517/components/convert/model_convert/aie/core/convert.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/core/__init__.py` & `ms-ait-7.0.0b517/components/convert/model_convert/aie/core/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aoe/aoe_args_map.py` & `ms-ait-7.0.0b517/components/convert/model_convert/aoe/aoe_args_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/atc/atc_args_map.py` & `ms-ait-7.0.0b517/components/convert/model_convert/atc/atc_args_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/__init__.py` & `ms-ait-7.0.0b517/components/debug/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/main.py` & `ms-ait-7.0.0b517/components/debug/compare/main.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/README.md` & `ms-ait-7.0.0b517/components/debug/compare/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/setup.py` & `ms-ait-7.0.0b517/components/debug/compare/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/cmp_process.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/cmp_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/install.sh` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/l1_buffer_data_parser.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/l1_buffer_data_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf_debug_runner.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf_debug_runner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__install__.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__main__.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/atc_utils.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/atc/atc_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/args_check.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/convert.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/convert.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dump_data.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/tf_common.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/tf_common.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/utils.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/analyser.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/analyser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/net_compare.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/net_compare/net_compare.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/npu_dump_data.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/npu_dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/om_parser.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/npu/om_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/custom_op.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/custom_op.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,32 @@
 
     def _load_onnx(self, model_path):
         # model_path str -> read as bytes -> deserialize to onnx_model
         #                                 -> onnxruntime load as session
         with open(model_path, "rb") as ff:
             model_contents = ff.read()
         onnx_model = onnx.load_model(model_path)
+        unique_index = 999
+        name_set = set((node.name for node in onnx_model.graph.node))
+
+        def get_unique_name(ori_name, index):
+            new_name = f"{ori_name}_{index}"
+            if new_name not in name_set:
+                return new_name, index + 1
+            else:
+                return get_unique_name(ori_name, index + 1)
+
         for index, node in enumerate(onnx_model.graph.node):
-            if not node.name:
-                node.name = node.op_type + "_" + str(index)
+            if node.name:
+                continue
+            new_name = node.op_type + "_" + str(index)
+            if new_name in name_set:
+                new_name, unique_index = get_unique_name(new_name, unique_index)
+            name_set.add(new_name)
+            node.name = new_name
         return onnx_model, model_contents
 
     def _new_model_save_path(self, origin_path):
         save_name = "new_" + os.path.basename(origin_path)
         return os.path.join(self.model_dir, save_name)
 
     def _create_dir(self):
@@ -177,14 +192,16 @@
             if self.dump:
                 model_dir = os.path.join(self.out_path, model_relative_name)
                 utils.create_directory(model_dir)
         return data_dir, onnx_dump_data_dir, model_dir
 
     def _modify_model_add_outputs_nodes(self, onnx_model, save_path):
         if self.dump:
+            del onnx_model.graph.output[:]
+            
             onnx_model.graph.output.extend(
                 onnx.ValueInfoProto(name=tensor_name) 
                 for node in onnx_model.graph.node 
                 for tensor_name in node.output
             )
         
         model_size = onnx_model.ByteSize()
```

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/single_op.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/single_op/single_op.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/tf_dump_data.py` & `ms-ait-7.0.0b517/components/debug/compare/msquickcmp/tf/tf_dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/README.md` & `ms-ait-7.0.0b517/components/debug/surgeon/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/setup.py` & `ms-ait-7.0.0b517/components/debug/surgeon/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/ait_main.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/ait_main.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/options.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/options.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__install__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__main__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/args_check.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/click_utils.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/click_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/config.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/log.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/register.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/register.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/singleton.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/singleton.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/utils.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/common/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/README.md` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/README.md` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/matcher.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/matcher.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/pattern.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/pattern.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/utils.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/inference.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/log.py` & `ms-ait-7.0.0b517/components/debug/surgeon/auto_optimizer/tools/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/README.md` & `ms-ait-7.0.0b517/components/llm/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/setup.py` & `ms-ait-7.0.0b517/components/llm/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/__init__.py` & `ms-ait-7.0.0b517/components/llm/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/install.sh` & `ms-ait-7.0.0b517/components/llm/ait_llm/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/__init__.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/__install__.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/__main__.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/constant.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/common/constant.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/json_fitter.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/common/json_fitter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/log.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/tool.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/common/tool.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/utils.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/validate.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/common/validate.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/atb_acc_cmp.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/compare/atb_acc_cmp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_algorithm.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/compare/cmp_algorithm.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_utils.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/compare/cmp_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/op_mapping.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/compare/op_mapping.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/torchair_acc_cmp.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/compare/torchair_acc_cmp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/initial.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/initial.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/manual_dump.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/manual_dump.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_config.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/dump_config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_hook.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/dump_hook.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/hook.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook_ops.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/hook_ops.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/topo.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/topo.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/__init__.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/dump/torch_dump/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/process.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/errcheck/process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/metrics/case_filter.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/metrics/case_filter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/metrics/metrics.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/metrics/metrics.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/case_manager.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/case_manager.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/opchecker.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/opchecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             'tensor_path': string
         '''
         self.csv_data = {}
         self.cases_info = {}
         self.completed_op_id_queue = queue.Queue()
         self.special_cases = ['KvCacheOperation', 'ReshapeAndCacheOperation', 'SelfAttentionOperation']
         self.base_path = ''
+        self.pid = None
         self.tensor_path = ''
         self.op_path = ''
         self.output_dir = ''
         self.output_path = ''
         self.ids = ''
         self.check_ids_string = []
         self.opname = None
@@ -96,45 +97,50 @@
             return False
 
         return True
 
     def get_base_path(self, cur_path):
         dirseg = cur_path.split(os.path.sep)
         if len(dirseg) >= 4 and dirseg[-3] == 'tensors' and dirseg[-4] == 'ait_dump':
-            return cur_path
+            try:
+                pid = dirseg[-2].split("_")[1]
+            except:
+                pid = None
+            return cur_path, pid
         elif cur_path == os.path.dirname(cur_path):
-            return None
+            return None, None
         else:
             return self.get_base_path(os.path.dirname(cur_path))
 
     def check_input_legality(self, input_path):
         ret = False
         base_path = None
+        pid = None
 
         input_path = os.path.realpath(input_path)
         if not os.path.exists(input_path):
             logger_text = f"Input path not found: {input_path}"
             logger.error(logger_text)
-            return input_path, base_path, ret
+            return input_path, base_path, pid, ret
         
-        base_path = self.get_base_path(input_path)
+        base_path, pid = self.get_base_path(input_path)
         if base_path is None:
             logger_text = f"input path is not in ait_dump tensors directory: {input_path}"
             logger.error(logger_text)
-            return input_path, base_path, ret
+            return input_path, base_path, pid, ret
         
         ret = True
-        return input_path, base_path, ret
+        return input_path, base_path, pid, ret
 
     def args_init(self, args):
         import torch_npu
 
         execution_flag = True
 
-        self.tensor_path, self.base_path, ret = self.check_input_legality(args.input)
+        self.tensor_path, self.base_path, self.pid, ret = self.check_input_legality(args.input)
         if not ret:
             execution_flag = False
         
         self.output_dir = os.path.realpath(args.output) 
         self.output_path = os.path.join(self.output_dir, f"opcheck_result_{self.timestamp}.xlsx")
         self.ids = args.ids
         if self.ids != '':
@@ -286,15 +292,15 @@
 
         op_id, op_name = self.parse_op_id_name(dirpath)
         if op_id is None or op_name is None:
             return
 
         case_info = {
             'op_id': op_id, 'op_name': op_name, 'op_param': op_param, 'tensor_path': tensor_path,
-            'precision_type': self.precision_type, 'rerun': self.rerun
+            'precision_type': self.precision_type, 'rerun': self.rerun, 'pid': self.pid
         }
 
         ret = self.is_exec_node(case_info)
         if ret:
             self.add_case_to_cases(case_info)
         return
 
@@ -388,8 +394,8 @@
         
         if len(op_result['res_detail']) > 0:
             for cur_id, res_detail in enumerate(op_result['res_detail']):
                 ws.append(self._update_single_op_result(op_info, cur_id, res_detail))
         else:
             cur_id, res_detail = 'NaN', {}
             ws.append(self._update_single_op_result(op_info, cur_id, res_detail))
-        wb.save(self.output_path)
+        wb.save(self.output_path)
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/operation_test.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/operation_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.case_info = case_info
         self.case_info['res_detail'] = []
         self.excuted_ids = excuted_ids
         self.op_id = case_info['op_id']
         self.op_name = case_info['op_name']
         self.op_param = case_info['op_param']
         self.tensor_path = case_info['tensor_path']
+        self.pid = case_info['pid']
         self.in_tensors = []
         self.out_tensors = []
         self.rerun = self.case_info["rerun"]
 
         error1 = 'Error0.1‰'
         error2 = 'Error0.5‰'
         error3 = 'Error1‰'
@@ -73,35 +74,61 @@
         testloader = unittest.TestLoader()
         testnames = testloader.getTestCaseNames(optest_class)
         suite = unittest.TestSuite()
         for name in testnames:
             suite.addTest(optest_class(name, case_info=case_info, excuted_ids=excuted_ids))
         return suite
 
+    def validate_param(self, *param_names):
+        ret = True
+        for param_name in param_names:
+            param = self.op_param.get(param_name, None)
+            if param is None:
+                ret = False
+                msg = f"Cannot get golden data because opParam {param_name} is not correctly set!"
+                logger.error(msg)
+        return ret
+
+    def validate_path(self, path):
+        if not path or not os.path.exists(path):
+            raise RuntimeError(f"{path} not valid")
+
+    def get_tensor_path(self, path, tensor_type):
+        _tensor_path = [x for x in os.listdir(path) if x.startswith(tensor_type)]
+        _tensor_path.sort(key=lambda x:int(x.split(tensor_type)[1].split('.')[0]))  
+        tensor_files = [os.path.join(path, x) for x in _tensor_path]
+        return tensor_files
+
+    def read_tensor_from_file(self, tensor_files):
+        res = []
+        for tensor_file in tensor_files:
+            tensor = read_atb_data(tensor_file).npu()
+            res.append(tensor)
+        return res
+
+    def get_new_in_tensors(self):
+        rank = self.op_param.get("rank", None) 
+        rank_root = self.op_param.get("rankRoot", None)
+        rank_size = self.op_param.get("rankSize", None)
+        new_in_tensors = []
+        for i in range(rank_root, rank_size):
+            old_did_pid = f"{rank}_{self.pid}"
+            new_did_pid = f"{i}_{int(self.pid) - rank + i}"
+            new_tensor_path = self.tensor_path[::-1].replace(old_did_pid[::-1], new_did_pid[::-1], 1)[::-1]
+            self.validate_path(new_tensor_path)
+            _in_tensor_files = self.get_tensor_path(new_tensor_path, "intensor")
+            new_in_tensors.extend(self.read_tensor_from_file(_in_tensor_files))
+        return new_in_tensors
+
     def setUp(self):
-        def get_tensor_path(tensor_type):
-            _tensor_path = [x for x in os.listdir(self.tensor_path) if x.startswith(tensor_type)]
-            _tensor_path.sort(key=lambda x:int(x.split(tensor_type)[1].split('.')[0]))  
-            _tensor_path = [os.path.join(self.tensor_path, x) for x in _tensor_path]
-            return _tensor_path
-
-        if self.tensor_path:
-            if os.path.isdir(self.tensor_path):
-                _in_tensor_path = get_tensor_path("intensor")
-                for path in _in_tensor_path:
-                    _in_tensor = read_atb_data(path).npu()
-                    self.in_tensors.append(_in_tensor)
-                _out_tensor_path = get_tensor_path("outtensor")
-                for path in _out_tensor_path:
-                    _out_tensor = read_atb_data(path).npu()
-                    self.out_tensors.append(_out_tensor)
-            else:
-                raise RuntimeError(f"{self.tensor_path} not valid")
-        else:
-            raise RuntimeError(f"{self.tensor_path} not valid")
+        self.validate_path(self.tensor_path)
+        _in_tensor_files = self.get_tensor_path(self.tensor_path, "intensor")
+        self.in_tensors = self.read_tensor_from_file(_in_tensor_files)
+        _out_tensor_files = self.get_tensor_path(self.tensor_path, "outtensor")
+        self.out_tensors = self.read_tensor_from_file(_out_tensor_files)
 
     def tearDown(self):
         self.excuted_ids.put(self.op_id)
         if self.case_info['excuted_information'] != 'PASS':
             self.case_info['excuted_information'] = 'FAILED'
 
     def rerun_op(self, excute_type): 
@@ -125,18 +152,14 @@
     def excute_common(self, excute_type):
         logger_text = f"———————— {self.op_id} {self.op_name} test start ————————"
         logger.info(logger_text)
         if self.rerun:
             out_tensors = self.rerun_op(excute_type)
         else:
             out_tensors = self.out_tensors
-        
-        if self.op_name == "AllGatherOperation":
-            rank = self.op_param.get("rank", 0)
-            out_tensors[0] = out_tensors[0][rank]
 
         golden_out_tensors = self.golden_calc(self.in_tensors)
         try:
             logger.debug("out_tensor", out_tensors[0].size())
             logger.debug("golden_out_tensor", golden_out_tensors[0].size())
         except TypeError as e:
             logger_text = "The output is abnormal. Please check! Exception: {}".format(e)
@@ -220,14 +243,30 @@
         device_count = torch.npu.device_count()
         current_device = torch.npu.current_device()
         logger_text = "Device Properties: device_name: {}, soc_version: {}, device_count: {}, current_device: {}" \
                     .format(device_name, soc_version, device_count, current_device)
         logger.debug(logger_text)
         return soc_version
 
+    def convert_data_format(self, data):
+        dim0, dim1 = data.shape[0], data.shape[1]
+        data = data.reshape([1, dim1 // 16, dim0, 16]).permute(0, 2, 1, 3).reshape([dim0, dim1])
+        return data
+    
+    def nz_2_nd(self, data):
+        origin_shape = data.shape
+        dims = list(range(len(origin_shape)))
+        last_dims = dims[-4:]
+
+        perm = dims[:-4] + [last_dims[1]] + [last_dims[2]] + [last_dims[0]] + [last_dims[3]]
+        data = data.permute(perm)
+        nd_shape = data.shape[:-4] + (data.shape[-4] * data.shape[-3], data.shape[-2], data.shape[-1])
+        data = data.reshape(nd_shape)
+        return data
+
     def __golden_compare_all(self, out_tensors, golden_out_tensors):
         message, pass_flag = [], True
 
         my_data_len, golden_data_len = len(out_tensors), len(golden_out_tensors)
         if my_data_len != golden_data_len:
             pass_flag = False
             logger.info(f"Data count not equal, {my_data_len} != {golden_data_len}. Will compare only partial")
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/build.sh` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/build.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/activation.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/activation.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_gather.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/concat.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,16 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
+from ait_llm.common.log import logger
 
 
-class OpcheckAllGatherOperation(operation_test.OperationTest):
+class OpcheckConcatOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        golden_result = torch.stack(in_tensors, dim=0)
-        return [golden_result]        
+        concat_dim = self.op_param.get("concatDim", None)
+        axis_num = concat_dim if concat_dim >= 0 else concat_dim + len(in_tensors[0].size())
+        golden_result = torch.cat(in_tensors, axis=axis_num)
+        return [golden_result]
 
-    def test_all_gather(self):
+    def test(self):
+        concat_dim = self.op_param.get("concatDim", None)
+        if concat_dim is None:
+            msg = "Cannot get golden data because concatDim is not correctly set!"
+            logger.error(msg)
+            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_reduce.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/all_reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,43 +47,49 @@
             result = torch.min(result, in_tensors[i])
         return [result]
 
     def prod_cal(self, in_tensors):
         result = in_tensors[0]
         for i in range(1, len(in_tensors)):
             result = torch.mul(result, in_tensors[i])
-        return [result] 
+        return [result]
 
     def golden_calc(self, in_tensors):
         all_reduce_type = self.op_param.get('allReduceType', None)
         backend = self.op_param.get('backend', None)
+
+        new_in_tensors = self.get_new_in_tensors()
                     
         if all_reduce_type == "sum":
             if backend == "lccl":
-                golden = self.lccl_sum_cal(in_tensors)
+                golden = self.lccl_sum_cal(new_in_tensors)
             else:
-                golden = self.sum_cal(in_tensors)
+                golden = self.sum_cal(new_in_tensors)
         elif all_reduce_type == "max":
-            golden = self.max_cal(in_tensors)
+            golden = self.max_cal(new_in_tensors)
         elif all_reduce_type == "min":
-            golden = self.min_cal(in_tensors)
+            golden = self.min_cal(new_in_tensors)
         elif all_reduce_type == "prod":
-            golden = self.prod_cal(in_tensors)
+            golden = self.prod_cal(new_in_tensors)
 
         return golden
 
     def test_all_reduce(self):
+        if self.pid is None:
+            logger_text = f"Cannot get a valid pid, AllReduceOperation is not supported!"
+            logger.error(logger_text)
+            return
+
+        ret = self.validate_param("allReduceType", "backend", "rank", "rankRoot", "rankSize")
+        if not ret:
+            return
+
         all_reduce_type = self.op_param.get('allReduceType', None)
         backend = self.op_param.get('backend', None)
-
         logger_text1 = f"backend: {backend}, allreduceType: {all_reduce_type}"
         logger_text2 = "env: {}".format(os.getenv("LCCL_DETERMINISTIC", ""))
         logger_text3 = "env: {}".format(os.getenv("HCCL_DETERMINISTIC", ""))
         logger.debug(logger_text1)
         logger.debug(logger_text2)
         logger.debug(logger_text3)
 
-        if all_reduce_type is None or backend is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/as_strided.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/as_strided.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/broadcast.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/broadcast.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/concat.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/sort.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 import torch_npu
+import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
-class OpcheckConcatOperation(operation_test.OperationTest):
+class OpcheckSortOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        concat_dim = self.op_param.get("concatDim", None)
-        axis_num = concat_dim if concat_dim >= 0 else concat_dim + len(in_tensors[0].size())
-        golden_result = torch.cat(in_tensors, axis=axis_num)
-        return [golden_result]
+        num = self.param.get("num", None)
+        values, indices = torch.topk(in_tensors[0], k=num[0], largest=True)
+        return [values, indices.int()]
 
-    def test(self):
-        concat_dim = self.op_param.get("concatDim", None)
-        if concat_dim is None:
-            msg = "Cannot get golden data because concatDim is not correctly set!"
+    def test_3d_float(self):
+        num = self.param.get("num", None)
+        if num is None:
+            msg = "Cannot get golden data because num is not correctly set!"
             logger.error(msg)
             return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/cumsum.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/cumsum.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/elewise.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/elewise.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fill.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/fill.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/gather.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/gather.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/genattentionmask.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/genattentionmask.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/kv_cache.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/kv_cache.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/layer_norm.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/layer_norm.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,21 +40,23 @@
                 in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1))
         golden_result = torch.matmul(in_tensor_0, in_tensor_1)
         return golden_result
 
     def golden_calc(self, in_tensors):
         transpose_a = self.op_param.get("transposeA", None)
         transpose_b = self.op_param.get("transposeB", None)
+        soc_version = self.get_soc_version()
+        if soc_version == 'Ascend310P':
+            in_tensors[1] = self.convert_data_format(in_tensors[1])
+            logger_text = "The result of this case is unreliable on Ascend310P!"
+            logger.info(logger_text)
         golden_result = self.golden_flp(transpose_a, transpose_b, in_tensors[0], in_tensors[1])
         has_bias = self.op_param.get("hasBias", False)
         if has_bias:
             golden_result = golden_result + in_tensors[2]
         return [golden_result]
 
     def test(self):
-        transpose_a = self.op_param.get("transposeA", None)
-        transpose_b = self.op_param.get("transposeB", None)
-        if transpose_a is None or transpose_b is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
+        ret = self.validate_param("transposeA", "transposeB")
+        if not ret:
             return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_parallel.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear_parallel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_sparse.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/linear_sparse.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/matmul.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/matmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/multinomial.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/multinomial.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/pad.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/pad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/paged_attention.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/paged_attention.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reduce.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/reduce.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/repeat.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/repeat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rms_norm.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rms_norm.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rope.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope_grad.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/rope_grad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/self_attention.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/self_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,21 @@
         logger.debug(score.shape)
         return score
 
     def undefined_golden_func(self, in_tensors):
         mixed_q, mixed_k, mixed_v, cache_k, cache_v, attention_mask, token_offset, seq_len, layerid = in_tensors[0], \
             in_tensors[1], in_tensors[2], in_tensors[3], in_tensors[4], in_tensors[5], in_tensors[6], in_tensors[7], \
             int(in_tensors[8][0])
-        
+
+        soc_version = self.get_soc_version()
+        if soc_version == 'Ascend310P':
+            cache_k = self.nz_2_nd(cache_k)
+            cache_v = self.nz_2_nd(cache_v)
+            attention_mask = self.nz_2_nd(attention_mask)
+
         batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
         if batch_run_status_enable:
             batch_status = in_tensors[9]
         else:
             batch_status = len(seq_len)
         q_scale, qk_scale, head_num, head_size = self.op_param.get("qScale", 1.0), self.op_param.get("qkScale", 1.0), \
             self.op_param.get("headNum", 32), mixed_k.size(-1)
@@ -89,14 +95,18 @@
         out = torch.concat(context_list, dim=0)
         return out
 
     def encoder_golden_func(self, in_tensors):
         mixed_q, mixed_k, mixed_v, attention_mask, seq_len = in_tensors[0], in_tensors[1], in_tensors[2], \
             in_tensors[3], in_tensors[4]
         
+        soc_version = self.get_soc_version()
+        if soc_version == 'Ascend310P':
+            attention_mask = self.nz_2_nd(attention_mask)
+
         dtype = mixed_q.dtype
         batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
         if batch_run_status_enable:
             batch_status = in_tensors[5]
         else:
             batch_status = len(seq_len)
 
@@ -113,15 +123,15 @@
             k_slice = mixed_k[k_offset:k_offset + kv_s][:].view(kv_s, group_num, embed)
             k_slice = torch.permute(k_slice, (1, 0, 2))
             k_slice_t = torch.permute(k_slice, (0, 2, 1))   # get K^T (kv_heads, embed, k_seq)
             v_slice = mixed_v[v_offset:v_offset + kv_s][:].view(kv_s, group_num, embed)
             v_slice = torch.permute(v_slice, (1, 0, 2))
             score = self.group_matmul(heads, group_num, q_slice, k_slice_t)
             s = score.view(-1) if s is None else torch.concat((s, score.view(-1)), 0)
-            
+
             score = score / math.sqrt(1.0 * embed)
             score_max = torch.max(score, axis=-1).values
             score = score - score_max.view((heads, q_s, 1))
             score_exp = torch.exp(score)
             if not dtype == torch.float32:
                 score_sum = torch.sum(score_exp, axis=-1)
                 _p = score_exp.view(-1) if _p is None else torch.concat((_p, score_exp.view(-1)), 0)
@@ -162,20 +172,14 @@
         else:
             logger_text = f"CalcType: {calc_type}. Using encoder of PageAttention!"
             logger.debug(logger_text)
             out = self.pa_encoder_golden_func(in_tensors)
         return [out]
 
     def test(self):
-        soc_version = self.get_soc_version()
-        if soc_version != 'Ascend910B':
-            logger_text = f"{soc_version} is not supported! Only supports Ascend910B!"
-            logger.error(logger_text)
-            return
-        
         batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
 
         if len(self.in_tensors) <= 6:
             if batch_run_status_enable:
                 batch_run_status = self.in_tensors[5].tolist()
                 logger_text = f"Enabling batchRunStatus: {batch_run_status}"
                 logger.debug(logger_text)
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/set_value.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/set_value.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/slice.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/slice.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/softmax.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/softmax.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/sort.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/split.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 import torch_npu
-import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
-class OpcheckSortOperation(operation_test.OperationTest):
+class OpcheckAddOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        num = self.param.get("num", None)
-        values, indices = torch.topk(in_tensors[0], k=num[0], largest=True)
-        return [values, indices.int()]
+        split_num = self.op_param.get('splitNum', None)
+        split_dim = self.op_param.get('splitDim', None)
+        split_output = torch.chunk(in_tensors[0], chunks=split_num, dim=split_dim)
+        return split_output
 
-    def test_3d_float(self):
-        num = self.param.get("num", None)
-        if num is None:
-            msg = "Cannot get golden data because num is not correctly set!"
+    def test(self):
+        split_num = self.op_param.get('splitNum', None)
+        split_dim = self.op_param.get('splitDim', None)
+        if split_num is None or split_dim is None:
+            msg = "Cannot get golden data because opParam is not correctly set!"
             logger.error(msg)
             return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/split.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/transpose.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
-class OpcheckAddOperation(operation_test.OperationTest):
+class OpcheckTransposeOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        split_num = self.op_param.get('splitNum', None)
-        split_dim = self.op_param.get('splitDim', None)
-        split_output = torch.chunk(in_tensors[0], chunks=split_num, dim=split_dim)
-        return split_output
+        perm = self.op_param.get("perm", None)
+        golden_result = in_tensors[0].permute(perm)
+        return [golden_result]
 
-    def test(self):
-        split_num = self.op_param.get('splitNum', None)
-        split_dim = self.op_param.get('splitDim', None)
-        if split_num is None or split_dim is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
+    def test_2d_float(self):
+        perm = self.op_param.get("perm", None)
+        if perm is None:
+            msg = "Cannot get golden data because perm is not correctly set!"
             logger.error(msg)
             return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transdata.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/transdata.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transpose.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/all_gather.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
-class OpcheckTransposeOperation(operation_test.OperationTest):
+class OpcheckAllGatherOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        perm = self.op_param.get("perm", None)
-        golden_result = in_tensors[0].permute(perm)
-        return [golden_result]
-
-    def test_2d_float(self):
-        perm = self.op_param.get("perm", None)
-        if perm is None:
-            msg = "Cannot get golden data because perm is not correctly set!"
-            logger.error(msg)
+        new_in_tensors = self.get_new_in_tensors()
+        golden_result = torch.stack(new_in_tensors, dim=0)
+        return [golden_result]        
+
+    def test_all_gather(self):
+        if self.pid is None:
+            logger_text = f"Cannot get a valid pid, AllGatherOperation is not supported!"
+            logger.error(logger_text)
+            return
+
+        ret = self.validate_param("rank", "rankRoot", "rankSize")
+        if not ret:
             return
+
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/unpad.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/unpad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/where.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/where.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/__init__.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/opcheck/check_case/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/transform/transform_quant.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/transform/utils.py` & `ms-ait-7.0.0b517/components/llm/ait_llm/transform/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/__init__.py` & `ms-ait-7.0.0b517/components/profile/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/install.sh` & `ms-ait-7.0.0b517/components/profile/msprof/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/README.md` & `ms-ait-7.0.0b517/components/profile/msprof/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/setup.py` & `ms-ait-7.0.0b517/components/profile/msprof/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/api.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/api.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/args_adapter.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/main_cli.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/main_cli.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/msprof_process.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/msprof_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/utils.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__install__.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__main__.py` & `ms-ait-7.0.0b517/components/profile/msprof/ait_prof/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/setup.py` & `ms-ait-7.0.0b517/components/tensor_view/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/atb.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/atb.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/handler.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/handler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/logger.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/logger.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/main_cli.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/main_cli.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/operation.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/operation.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/print_stat.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/print_stat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__install__.py` & `ms-ait-7.0.0b517/components/tensor_view/ait_tensor_view/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tests/test_ait.sh` & `ms-ait-7.0.0b517/components/tests/test_ait.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/install.bat` & `ms-ait-7.0.0b517/components/transplt/install.bat`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/install.sh` & `ms-ait-7.0.0b517/components/transplt/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/README.md` & `ms-ait-7.0.0b517/components/transplt/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/setup.py` & `ms-ait-7.0.0b517/components/transplt/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/__init__.py` & `ms-ait-7.0.0b517/components/transplt/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/install.bat` & `ms-ait-7.0.0b517/components/transplt/app_analyze/install.bat`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/install.sh` & `ms-ait-7.0.0b517/components/transplt/app_analyze/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/__install__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/__install__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/__main__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/common/kit_config.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/common/kit_config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/common/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/common/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/exception/exception_information.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/exception/exception_information.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/exception/source_scan_exception.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/exception/source_scan_exception.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/exception/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/exception/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/model.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/model/model.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/project.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/model/project.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/seq_project.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/model/seq_project.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/model/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/app.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/porting/app.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/cmdline_input.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/porting/cmdline_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/custom_input.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/porting/custom_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/input_factory.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/porting/input_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/porting_input.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/porting/porting_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/porting/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/csv_report.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/report/csv_report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/json_report.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/report/json_report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/report.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/report/report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/report_factory.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/report/report_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/report/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_parser.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/clang_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_utils.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/clang_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cmake_scanner.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/cmake_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cxx_scanner.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/cxx_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/func_parser.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/func_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_parser.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/python_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_scanner.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/python_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_factory.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_utils.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scanner_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scan_api.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/scan_api.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/comment_delete.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/comment_delete.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/file_matrix.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/file_matrix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/module/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/acc_libs.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/acc_libs.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/api_filter.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/api_filter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/ast_visitor.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/ast_visitor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_desc.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_desc.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_handler.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_handler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_matcher.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_matcher.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_utils.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/scan/sequence/seq_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/solution/advisor.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/solution/advisor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/solution/seq_advisor.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/solution/seq_advisor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/solution/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/solution/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/clang_finder.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/clang_finder.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/excel.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/excel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/file_locker.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/file_locker.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/io_util.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/io_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/lib_util.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/lib_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/log_util.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/log_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/security.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/security.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/__init__.py` & `ms-ait-7.0.0b517/components/transplt/app_analyze/utils/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/file_open_check.py` & `ms-ait-7.0.0b517/components/utils/file_open_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/install.py` & `ms-ait-7.0.0b517/components/utils/install.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/parser.py` & `ms-ait-7.0.0b517/components/utils/parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/security_check.py` & `ms-ait-7.0.0b517/components/utils/security_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/util.py` & `ms-ait-7.0.0b517/components/utils/util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/__init__.py` & `ms-ait-7.0.0b517/components/utils/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/ms_ait.egg-info/SOURCES.txt` & `ms-ait-7.0.0b517/ms_ait.egg-info/SOURCES.txt`

 * *Files identical despite different names*

