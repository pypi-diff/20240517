# Comparing `tmp/InternEvo-0.5.1.dev20240517.tar.gz` & `tmp/InternEvo-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.5.1.dev20240517.tar", last modified: Fri May 17 11:01:23 2024, max compression
+gzip compressed data, was "InternEvo-0.5.2.tar", last modified: Mon May 13 03:46:12 2024, max compression
```

## Comparing `InternEvo-0.5.1.dev20240517.tar` & `InternEvo-0.5.2.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.786229 InternEvo-0.5.1.dev20240517/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:19.928513 InternEvo-0.5.1.dev20240517/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5181 2024-05-17 11:01:21.000000 InternEvo-0.5.1.dev20240517/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4864 2024-05-17 11:01:21.000000 InternEvo-0.5.1.dev20240517/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-17 11:01:21.000000 InternEvo-0.5.1.dev20240517/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      178 2024-05-17 11:01:21.000000 InternEvo-0.5.1.dev20240517/InternEvo.egg-info/requires.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-17 11:01:21.000000 InternEvo-0.5.1.dev20240517/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.5.1.dev20240517/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5181 2024-05-17 11:01:23.006127 InternEvo-0.5.1.dev20240517/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.5.1.dev20240517/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:19.935511 InternEvo-0.5.1.dev20240517/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.5.1.dev20240517/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:19.968160 InternEvo-0.5.1.dev20240517/internlm/accelerator/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/accelerator/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/accelerator/abstract_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/accelerator/cuda_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/accelerator/dipu_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/accelerator/npu_accelerator.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:19.985703 InternEvo-0.5.1.dev20240517/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1.dev20240517/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.5.1.dev20240517/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.024352 InternEvo-0.5.1.dev20240517/internlm/checkpoint/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/checkpoint/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.5.1.dev20240517/internlm/checkpoint/checkpoint_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.5.1.dev20240517/internlm/checkpoint/components.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14172 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/checkpoint/load_funcs.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.5.1.dev20240517/internlm/checkpoint/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.052238 InternEvo-0.5.1.dev20240517/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.5.1.dev20240517/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.082185 InternEvo-0.5.1.dev20240517/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.5.1.dev20240517/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.5.1.dev20240517/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8456 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.097062 InternEvo-0.5.1.dev20240517/internlm/core/parallel/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1.dev20240517/internlm/core/parallel/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3810 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/core/parallel/shard.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.121256 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/base_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.140002 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4958 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8882 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63472 2024-05-17 09:05:58.000000 InternEvo-0.5.1.dev20240517/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7600 2024-05-17 10:34:43.000000 InternEvo-0.5.1.dev20240517/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.160564 InternEvo-0.5.1.dev20240517/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.5.1.dev20240517/internlm/data/build_dataloader.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.208177 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/dummy_dataset_multimodal.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/data/tokenized/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/data/train_state.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2546 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.222758 InternEvo-0.5.1.dev20240517/internlm/eval/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/eval/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.5.1.dev20240517/internlm/eval/evaluation.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.249049 InternEvo-0.5.1.dev20240517/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.5.1.dev20240517/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.5.1.dev20240517/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5934 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27583 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.263059 InternEvo-0.5.1.dev20240517/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1.dev20240517/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.320026 InternEvo-0.5.1.dev20240517/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1.dev20240517/internlm/model/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1354 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.342027 InternEvo-0.5.1.dev20240517/internlm/model/llava/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1.dev20240517/internlm/model/llava/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/llava/clip_builder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/llava/clip_encoder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/llava/projector_builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.356488 InternEvo-0.5.1.dev20240517/internlm/model/losses/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.5.1.dev20240517/internlm/model/losses/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1716 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/losses/ce_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16875 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16199 2024-05-15 07:15:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22009 2024-05-15 07:15:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21291 2024-05-15 07:15:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10481 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/modeling_llava.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17821 2024-05-15 07:15:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/modeling_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.396904 InternEvo-0.5.1.dev20240517/internlm/model/modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13791 2024-05-17 08:32:11.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21583 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27792 2024-05-17 08:32:11.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/mha.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4613 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      424 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3277 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/modules/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.429965 InternEvo-0.5.1.dev20240517/internlm/model/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/base_layer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20335 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/gshard_layer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.460143 InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8669 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13597 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2563 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11288 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4848 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.5.1.dev20240517/internlm/model/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.501626 InternEvo-0.5.1.dev20240517/internlm/model/ops/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    33645 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/attention.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2084 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/cross_entropy.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2400 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2489 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5346 2024-05-17 08:32:11.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/rotary_emb.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1670 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/ops/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2952 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/model/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2141 2024-05-15 07:15:26.000000 InternEvo-0.5.1.dev20240517/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.526944 InternEvo-0.5.1.dev20240517/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.538480 InternEvo-0.5.1.dev20240517/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.5.1.dev20240517/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/solver/activation_checkpoint.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.580567 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1946 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/compatible_adamw.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42554 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.598509 InternEvo-0.5.1.dev20240517/internlm/solver/schedulers/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.5.1.dev20240517/internlm/solver/schedulers/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.5.1.dev20240517/internlm/solver/schedulers/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.5.1.dev20240517/internlm/solver/schedulers/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.615979 InternEvo-0.5.1.dev20240517/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      601 2024-05-17 10:03:57.000000 InternEvo-0.5.1.dev20240517/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26151 2024-05-17 10:34:43.000000 InternEvo-0.5.1.dev20240517/internlm/train/pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3575 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.677898 InternEvo-0.5.1.dev20240517/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1.dev20240517/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7964 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.5.1.dev20240517/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3953 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.5.1.dev20240517/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.5.1.dev20240517/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4032 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.5.1.dev20240517/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-17 11:01:23.009221 InternEvo-0.5.1.dev20240517/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1235 2024-05-17 10:03:57.000000 InternEvo-0.5.1.dev20240517/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.690385 InternEvo-0.5.1.dev20240517/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1.dev20240517/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4526 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.709215 InternEvo-0.5.1.dev20240517/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1.dev20240517/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5566 2024-05-17 09:35:05.000000 InternEvo-0.5.1.dev20240517/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6968 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-17 10:59:20.776803 InternEvo-0.5.1.dev20240517/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.5.1.dev20240517/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.5.1.dev20240517/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.5.1.dev20240517/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8054 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11809 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14426 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3855 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6773 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12656 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14290 2024-05-10 09:00:44.000000 InternEvo-0.5.1.dev20240517/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:12.030272 InternEvo-0.5.2/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:10.965394 InternEvo-0.5.2/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5169 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4864 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      178 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/requires.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-17 04:37:11.000000 InternEvo-0.5.2/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5169 2024-05-13 03:46:12.167481 InternEvo-0.5.2/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-22 07:03:00.000000 InternEvo-0.5.2/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:10.975908 InternEvo-0.5.2/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:33.000000 InternEvo-0.5.2/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.018832 InternEvo-0.5.2/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.040834 InternEvo-0.5.2/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-18 05:06:05.000000 InternEvo-0.5.2/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.093571 InternEvo-0.5.2/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:15.000000 InternEvo-0.5.2/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:58.000000 InternEvo-0.5.2/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14172 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:31.000000 InternEvo-0.5.2/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.130052 InternEvo-0.5.2/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-17 04:37:12.000000 InternEvo-0.5.2/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.162033 InternEvo-0.5.2/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8456 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.176696 InternEvo-0.5.2/internlm/core/parallel/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:36.000000 InternEvo-0.5.2/internlm/core/parallel/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3810 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/parallel/shard.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.203598 InternEvo-0.5.2/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-06 04:29:21.000000 InternEvo-0.5.2/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-04-25 06:33:10.000000 InternEvo-0.5.2/internlm/core/scheduler/base_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.234384 InternEvo-0.5.2/internlm/core/scheduler/comm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/comm/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/comm/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4958 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/comm/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8882 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63810 2024-05-11 06:37:47.000000 InternEvo-0.5.2/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:43.000000 InternEvo-0.5.2/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.268831 InternEvo-0.5.2/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:24:57.000000 InternEvo-0.5.2/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.325172 InternEvo-0.5.2/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:25.000000 InternEvo-0.5.2/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:49:50.000000 InternEvo-0.5.2/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:49:50.000000 InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset_multimodal.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 12:29:02.000000 InternEvo-0.5.2/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2546 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.344261 InternEvo-0.5.2/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:33:26.000000 InternEvo-0.5.2/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.375831 InternEvo-0.5.2/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-18 05:06:05.000000 InternEvo-0.5.2/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-17 04:37:12.000000 InternEvo-0.5.2/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5934 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27583 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.393144 InternEvo-0.5.2/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.455857 InternEvo-0.5.2/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.2/internlm/model/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1354 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.484054 InternEvo-0.5.2/internlm/model/llava/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.2/internlm/model/llava/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/llava/clip_builder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/llava/clip_encoder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/llava/projector_builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.502303 InternEvo-0.5.2/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1716 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16875 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15915 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21691 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20973 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10481 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_llava.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17537 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.550424 InternEvo-0.5.2/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 03:21:42.000000 InternEvo-0.5.2/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13791 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21583 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27792 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/mha.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4613 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      424 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3277 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.586775 InternEvo-0.5.2/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.2/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20335 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.618307 InternEvo-0.5.2/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:21.000000 InternEvo-0.5.2/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8669 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13597 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2563 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11288 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4848 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.662252 InternEvo-0.5.2/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 03:21:42.000000 InternEvo-0.5.2/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    33645 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/attention.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2084 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/cross_entropy.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2400 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2489 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5346 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/rotary_emb.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1670 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2952 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      883 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.688618 InternEvo-0.5.2/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.701011 InternEvo-0.5.2/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.770758 InternEvo-0.5.2/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:26.000000 InternEvo-0.5.2/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-18 05:06:05.000000 InternEvo-0.5.2/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1946 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/solver/optimizer/compatible_adamw.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 09:32:05.000000 InternEvo-0.5.2/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42554 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 09:32:05.000000 InternEvo-0.5.2/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:12.000000 InternEvo-0.5.2/internlm/solver/optimizer/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.794767 InternEvo-0.5.2/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:42:40.000000 InternEvo-0.5.2/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.822875 InternEvo-0.5.2/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      601 2024-05-11 06:37:47.000000 InternEvo-0.5.2/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26101 2024-05-11 07:01:18.000000 InternEvo-0.5.2/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3575 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.894858 InternEvo-0.5.2/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7964 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:15:50.000000 InternEvo-0.5.2/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3953 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:42:40.000000 InternEvo-0.5.2/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4032 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-13 03:46:12.170532 InternEvo-0.5.2/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1235 2024-05-13 03:04:28.000000 InternEvo-0.5.2/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.906807 InternEvo-0.5.2/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4526 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.931278 InternEvo-0.5.2/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.5.2/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-23 01:33:18.000000 InternEvo-0.5.2/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6968 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:12.020983 InternEvo-0.5.2/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:58.000000 InternEvo-0.5.2/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 04:30:38.000000 InternEvo-0.5.2/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.5.2/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8054 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11809 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14426 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3855 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6773 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12656 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14290 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.5.1.dev20240517/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.5.2/InternEvo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.5.1.dev20240517
+Version: 0.5.2
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.5.1.dev20240517 Summary: an
-open-sourced lightweight training framework aims to support model pre-training
-without the need for extensive dependencies Classifier: Programming Language ::
-Python :: 3.10 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.5.2 Summary: an open-sourced
+lightweight training framework aims to support model pre-training without the
+need for extensive dependencies Classifier: Programming Language :: Python ::
+3.10 Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Education Classifier: Intended Audience :: Science/Research Description-
+Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.5.1.dev20240517/InternEvo.egg-info/SOURCES.txt` & `InternEvo-0.5.2/InternEvo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/LICENSE` & `InternEvo-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/PKG-INFO` & `InternEvo-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.5.1.dev20240517
+Version: 0.5.2
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.5.1.dev20240517 Summary: an
-open-sourced lightweight training framework aims to support model pre-training
-without the need for extensive dependencies Classifier: Programming Language ::
-Python :: 3.10 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.5.2 Summary: an open-sourced
+lightweight training framework aims to support model pre-training without the
+need for extensive dependencies Classifier: Programming Language :: Python ::
+3.10 Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Education Classifier: Intended Audience :: Science/Research Description-
+Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.5.1.dev20240517/README.md` & `InternEvo-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/accelerator/abstract_accelerator.py` & `InternEvo-0.5.2/internlm/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/accelerator/cuda_accelerator.py` & `InternEvo-0.5.2/internlm/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/accelerator/dipu_accelerator.py` & `InternEvo-0.5.2/internlm/accelerator/dipu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/accelerator/npu_accelerator.py` & `InternEvo-0.5.2/internlm/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/apis/inference.py` & `InternEvo-0.5.2/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/checkpoint/checkpoint_manager.py` & `InternEvo-0.5.2/internlm/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/checkpoint/components.py` & `InternEvo-0.5.2/internlm/checkpoint/components.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/checkpoint/load_funcs.py` & `InternEvo-0.5.2/internlm/checkpoint/load_funcs.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/checkpoint/utils.py` & `InternEvo-0.5.2/internlm/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/context/__init__.py` & `InternEvo-0.5.2/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/context/parallel_context.py` & `InternEvo-0.5.2/internlm/core/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/context/process_group_initializer.py` & `InternEvo-0.5.2/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/context/random.py` & `InternEvo-0.5.2/internlm/core/context/random.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/engine.py` & `InternEvo-0.5.2/internlm/core/engine.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/gradient_handler.py` & `InternEvo-0.5.2/internlm/core/gradient_handler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/naive_amp.py` & `InternEvo-0.5.2/internlm/core/naive_amp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/parallel/shard.py` & `InternEvo-0.5.2/internlm/core/parallel/shard.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.5.2/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/__init__.py` & `InternEvo-0.5.2/internlm/core/scheduler/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/p2p.py` & `InternEvo-0.5.2/internlm/core/scheduler/comm/p2p.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/scheduler/comm/utils.py` & `InternEvo-0.5.2/internlm/core/scheduler/comm/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.5.2/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.5.2/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,15 +564,15 @@
             moe_losses.append(moe_loss)
         # Before running 1F1B, need to receive first forward tensor.
         # If all microbatches are run in warmup / cooldown phase, then no need to
         # receive this tensor here.
         if num_1f1b_micropairs > 0:
             if not gpc.is_first_rank(ParallelMode.PIPELINE):
                 if forward_recv_shapes is None:
-                    forward_recv_shapes = comm.recv_obj_meta()
+                    forward_recv_shapes = comm.recv_obj_meta(forward_recv_shapes)
                 input_obj = comm.recv_forward(
                     forward_recv_shapes,
                     dtype=self.dtype,
                     scatter_gather_tensors=self.scatter_gather_tensors,
                 )
             else:
                 input_obj = None
@@ -810,15 +810,23 @@
         micro_batch_data, micro_batch_label = self._load_micro_batch(
             data=self.batch_data,
             label=self.batch_label,
             offset=self.microbatch_offset[model_chunk_id],
             bsz_stride=self.bsz_stride,
         )
         if self.data_process_func:
-            micro_batch_data, micro_batch_label = self.data_process_func(micro_batch_data, micro_batch_label)
+            micro_batch_data["input_ids"] = self.data_process_func(
+                micro_batch_data["input_ids"], micro_batch_data["cu_seqlens"]
+            )
+            micro_batch_label = self.data_process_func(
+                micro_batch_label, micro_batch_data["cu_seqlens"], padding_v=-100
+            )
+
+            micro_batch_data.pop("cu_seqlens")
+            micro_batch_data.pop("indexes")
 
         micro_batch_data["label"] = micro_batch_label
         self.microbatch_offset[model_chunk_id] += self.bsz_stride
         return move_to_device(micro_batch_data)
 
     def _forward_step(self, engine, chunk_id):
         """Forward step for passed-in model. If it is the first stage, the input tensor
@@ -958,15 +966,15 @@
             num_warmup_microsteps (int): The number of warm-up microsteps.
             receive_extra_backward (bool, optional): Whether to receive extra backward input for the 1F1B stage.
                                                      Default is False.
             forward_only (bool, optional): Whether to only perform forward pass. Default is False.
         """
         if not gpc.is_pipeline_first_stage():
             if self._input_obj_shapes[0] is None:
-                self._input_obj_shapes[0] = comm.recv_obj_meta()
+                self._input_obj_shapes[0] = comm.recv_obj_meta(self._input_obj_shapes[0])
             self._input_objs[0].append(
                 comm.recv_forward(
                     self._input_obj_shapes[0],
                     dtype=self.dtype,
                     scatter_gather_tensors=self.scatter_gather_tensors,
                 )
             )
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/core/trainer.py` & `InternEvo-0.5.2/internlm/core/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if batch_sampler:
             self.init_batch_sampler(batch_sampler)
 
         # tgs statistic
         self.tgs_statistic = {
             "sum_step": 0,
             "sum_tg": 0,
-            "total_time": 0,
+            "sum_time": 0,
             "sum_last_tg_10": 0,
             "sum_last_time_10": 0,
             "sum_last_tg_50": 0,
             "sum_last_time_50": 0,
             "SMA_tg_50": 0,
             "SMA_time_50": 0,
             "SMA_tg_50_list": deque(),
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/build_dataloader.py` & `InternEvo-0.5.2/internlm/data/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/batch_sampler.py` & `InternEvo-0.5.2/internlm/data/tokenized/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/collaters.py` & `InternEvo-0.5.2/internlm/data/tokenized/collaters.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/dataset.py` & `InternEvo-0.5.2/internlm/data/tokenized/dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/dummy_dataset.py` & `InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/dummy_dataset_multimodal.py` & `InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset_multimodal.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/packed_dataset.py` & `InternEvo-0.5.2/internlm/data/tokenized/packed_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/tokenized/single_dataset.py` & `InternEvo-0.5.2/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/data/utils.py` & `InternEvo-0.5.2/internlm/data/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/eval/evaluation.py` & `InternEvo-0.5.2/internlm/eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/initialize/initialize_tensor.py` & `InternEvo-0.5.2/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/initialize/initialize_trainer.py` & `InternEvo-0.5.2/internlm/initialize/initialize_trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/initialize/launch.py` & `InternEvo-0.5.2/internlm/initialize/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/initialize/legacy/launch.py` & `InternEvo-0.5.2/internlm/initialize/legacy/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/builder.py` & `InternEvo-0.5.2/internlm/model/builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/llava/clip_encoder.py` & `InternEvo-0.5.2/internlm/model/llava/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/llava/projector_builder.py` & `InternEvo-0.5.2/internlm/model/llava/projector_builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/losses/ce_loss.py` & `InternEvo-0.5.2/internlm/model/losses/ce_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/metrics.py` & `InternEvo-0.5.2/internlm/model/metrics.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modeling_internlm.py` & `InternEvo-0.5.2/internlm/model/modeling_internlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from internlm.initialize.initialize_tensor import normal_, scaled_init_method_normal
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import MHA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
 from internlm.model.utils import (
-    convert_attn_args_to_kwargs,
-    convert_attn_kwargs_to_args,
     internlm1_mha_pre_load_convert,
     internlm1_mha_save_convert,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
@@ -160,21 +158,19 @@
                     if self.use_scaled_init and "fc1" not in name:
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
                         normal_(std=0.006 if "fc1" in name else 0.0015)(param.data)
 
     def forward(self, hidden_states, **kwargs):
         if self.checkpoint and self.training:
-            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
-            args = convert_attn_kwargs_to_args(kwargs)
-            return activation_checkpoint(self._forward, False, hidden_states, *args)
+            return activation_checkpoint(self._forward, False, hidden_states, **kwargs)
         else:
             return self._forward(hidden_states, **kwargs)
 
-    def _forward(self, hidden_states, *args, **kwargs):
+    def _forward(self, hidden_states=None, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -190,16 +186,15 @@
             residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, hidden_states)
         else:
             residual, hidden_states = _dropout_and_norm_attn(hidden_states)
 
         if self.residual_in_fp32:
             residual = residual.to(torch.float32)
 
-        mixer_kwargs = convert_attn_args_to_kwargs(args, kwargs)
-        hidden_states = self.mixer(hidden_states, **mixer_kwargs)
+        hidden_states = self.mixer(hidden_states, **kwargs)
 
         def _dropout_and_norm_ffn(_residual, _hidden_states):
             _dropped = self.dropout2(_hidden_states)
             _residual = (_dropped + _residual) if _residual is not None else _dropped
             _hidden_states = self.norm2(_residual.float())
             return _residual, _hidden_states
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modeling_internlm2.py` & `InternEvo-0.5.2/internlm/model/modeling_internlm2.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     uniform_,
 )
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import GQA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
-from internlm.model.utils import (
-    convert_attn_args_to_kwargs,
-    convert_attn_kwargs_to_args,
-)
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
 
 
 class InternLM2Decoder(nn.Module):
@@ -197,21 +193,19 @@
                     else:
                         self.init_func(std=self.ffn_uplayer_init_std if "fc1" in name else self.ffn_other_init_std)(
                             param.data
                         )
 
     def forward(self, hidden_states, residual=None, **kwargs):
         if self.checkpoint and self.training:
-            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
-            args = convert_attn_kwargs_to_args(kwargs)
-            return activation_checkpoint(self._forward, False, hidden_states, residual, *args)
+            return activation_checkpoint(self._forward, False, hidden_states, residual, **kwargs)
         else:
             return self._forward(hidden_states, residual, **kwargs)
 
-    def _forward(self, hidden_states, residual, *args, **kwargs):
+    def _forward(self, hidden_states=None, residual=None, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -229,16 +223,15 @@
                 residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, residual, hidden_states)
             else:
                 residual, hidden_states = _dropout_and_norm_attn(residual, hidden_states)
 
             if self.residual_in_fp32:
                 residual = residual.to(torch.float32)
 
-            attn_kwargs = convert_attn_args_to_kwargs(args, kwargs)
-            hidden_states = self.attention(hidden_states, **attn_kwargs)
+            hidden_states = self.attention(hidden_states, **kwargs)
 
             if not isinstance(self.feed_forward, nn.Identity):
                 if not self.fused_dropout_add_ln:
 
                     def _dropout_and_norm_ffn(_residual, _hidden_states):
                         _dropped = self.dropout2(_hidden_states)
                         _residual = (_dropped + _residual) if _residual is not None else _dropped
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modeling_llama.py` & `InternEvo-0.5.2/internlm/model/modeling_llama.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     uniform_,
 )
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import GQA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
-from internlm.model.utils import (
-    convert_attn_args_to_kwargs,
-    convert_attn_kwargs_to_args,
-)
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
 
 
 class Llama2Decoder(nn.Module):
@@ -189,21 +185,19 @@
                     else:
                         self.init_func(std=self.ffn_uplayer_init_std if "fc1" in name else self.ffn_other_init_std)(
                             param.data
                         )
 
     def forward(self, hidden_states, residual=None, **kwargs):
         if self.checkpoint and self.training:
-            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
-            args = convert_attn_kwargs_to_args(kwargs)
-            return activation_checkpoint(self._forward, False, hidden_states, residual, *args)
+            return activation_checkpoint(self._forward, False, hidden_states, residual, **kwargs)
         else:
             return self._forward(hidden_states, residual, **kwargs)
 
-    def _forward(self, hidden_states, residual, *args, **kwargs):
+    def _forward(self, hidden_states=None, residual=None, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -221,16 +215,15 @@
                 residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, residual, hidden_states)
             else:
                 residual, hidden_states = _dropout_and_norm_attn(residual, hidden_states)
 
             if self.residual_in_fp32:
                 residual = residual.to(torch.float32)
 
-            attn_kwargs = convert_attn_args_to_kwargs(args, kwargs)
-            hidden_states = self.attention(hidden_states, **attn_kwargs)
+            hidden_states = self.attention(hidden_states, **kwargs)
 
             if not isinstance(self.feed_forward, nn.Identity):
                 if not self.fused_dropout_add_ln:
 
                     def _dropout_and_norm_ffn(_residual, _hidden_states):
                         _dropped = self.dropout2(_hidden_states)
                         _residual = (_dropped + _residual) if _residual is not None else _dropped
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modeling_llava.py` & `InternEvo-0.5.2/internlm/model/modeling_llava.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modeling_moe.py` & `InternEvo-0.5.2/internlm/model/modeling_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import MHA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
 from internlm.model.moe.moe import MoE
 from internlm.model.utils import (
-    convert_attn_args_to_kwargs,
-    convert_attn_kwargs_to_args,
     internlm1_mha_pre_load_convert,
     internlm1_mha_save_convert,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
@@ -177,21 +175,19 @@
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
                         normal_(std=0.006 if "fc1" in name else 0.0015)(param.data)
 
     def forward(self, hidden_states, **kwargs):
         if self.checkpoint and self.training:
             # TODO: check whether this will be affected by moe
-            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
-            args = convert_attn_kwargs_to_args(kwargs)
-            return activation_checkpoint(self._forward, False, hidden_states, *args)
+            return activation_checkpoint(self._forward, False, hidden_states, **kwargs)
         else:
             return self._forward(hidden_states, **kwargs)
 
-    def _forward(self, hidden_states, *args, **kwargs):
+    def _forward(self, hidden_states=None, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -207,16 +203,15 @@
             residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, hidden_states)
         else:
             residual, hidden_states = _dropout_and_norm_attn(hidden_states)
 
         if self.residual_in_fp32:
             residual = residual.to(torch.float32)
 
-        mixer_kwargs = convert_attn_args_to_kwargs(args, kwargs)
-        hidden_states = self.mixer(hidden_states, **mixer_kwargs)
+        hidden_states = self.mixer(hidden_states, **kwargs)
 
         def _dropout_and_norm_ffn(_residual, _hidden_states):
             _dropped = self.dropout2(_hidden_states)
             _residual = (_dropped + _residual) if _residual is not None else _dropped
             _hidden_states = self.norm2(_residual.float())
             return _residual, _hidden_states
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modules/embedding.py` & `InternEvo-0.5.2/internlm/model/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modules/linear.py` & `InternEvo-0.5.2/internlm/model/modules/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modules/mha.py` & `InternEvo-0.5.2/internlm/model/modules/mha.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modules/mlp.py` & `InternEvo-0.5.2/internlm/model/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/modules/utils.py` & `InternEvo-0.5.2/internlm/model/modules/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/base_layer.py` & `InternEvo-0.5.2/internlm/model/moe/base_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/experts.py` & `InternEvo-0.5.2/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/gshard_layer.py` & `InternEvo-0.5.2/internlm/model/moe/gshard_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/megablock_dmoe.py` & `InternEvo-0.5.2/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/megablock_moe.py` & `InternEvo-0.5.2/internlm/model/moe/megablock/megablock_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/mlp.py` & `InternEvo-0.5.2/internlm/model/moe/megablock/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/megablock/utils.py` & `InternEvo-0.5.2/internlm/model/moe/megablock/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/moe.py` & `InternEvo-0.5.2/internlm/model/moe/moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/moe/utils.py` & `InternEvo-0.5.2/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/ops/attention.py` & `InternEvo-0.5.2/internlm/model/ops/attention.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/ops/cross_entropy.py` & `InternEvo-0.5.2/internlm/model/ops/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/ops/linear.py` & `InternEvo-0.5.2/internlm/model/ops/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/ops/norm.py` & `InternEvo-0.5.2/internlm/model/ops/norm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/ops/rotary_emb.py` & `InternEvo-0.5.2/internlm/model/ops/rotary_emb.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/ops/utils.py` & `InternEvo-0.5.2/internlm/model/ops/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/model/registry.py` & `InternEvo-0.5.2/internlm/model/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/monitor/alert.py` & `InternEvo-0.5.2/internlm/monitor/alert.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/monitor/monitor.py` & `InternEvo-0.5.2/internlm/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/monitor/utils.py` & `InternEvo-0.5.2/internlm/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/activation_checkpoint.py` & `InternEvo-0.5.2/internlm/solver/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.5.2/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/compatible_adamw.py` & `InternEvo-0.5.2/internlm/solver/optimizer/compatible_adamw.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.5.2/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.5.2/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/store.py` & `InternEvo-0.5.2/internlm/solver/optimizer/store.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/optimizer/utils.py` & `InternEvo-0.5.2/internlm/solver/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/schedulers/beta2_scheduler.py` & `InternEvo-0.5.2/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/solver/schedulers/lr_scheduler.py` & `InternEvo-0.5.2/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/train/__init__.py` & `InternEvo-0.5.2/internlm/train/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/train/pipeline.py` & `InternEvo-0.5.2/internlm/train/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,15 +504,14 @@
     batch_count,
     batch,
     train_state,
     optimizer,
     beta2_scheduler,
     trainer,
     start_time,
-    very_begining_time,
     loss,
     moe_loss,
     grad_norm,
     metric,
 ):
     """
     Print some training metrics of current batch.
@@ -543,15 +542,15 @@
         tk_per_gpu = round(
             num_tokens_in_batch * gpc.get_world_size(ParallelMode.DATA) / gpc.get_world_size(ParallelMode.GLOBAL),
             4,
         )
         tgs_statistic = train_state.tgs_statistic
         tgs_statistic["sum_step"] += 1
         tgs_statistic["sum_tg"] += tk_per_gpu
-        tgs_statistic["total_time"] = time.time() - very_begining_time
+        tgs_statistic["sum_time"] += time_cost
         tgs_statistic["sum_last_tg_10"] += tk_per_gpu
         tgs_statistic["sum_last_time_10"] += time_cost
         tgs_statistic["sum_last_tg_50"] += tk_per_gpu
         tgs_statistic["sum_last_time_50"] += time_cost
         tgs_statistic["SMA_tg_50"] += tk_per_gpu
         tgs_statistic["SMA_time_50"] += time_cost
         tgs_statistic["SMA_tg_50_list"].append(tk_per_gpu)
@@ -574,15 +573,15 @@
             tgs_statistic["last_tgs_50"] = round(tgs_statistic["sum_last_tg_50"] / tgs_statistic["sum_last_time_50"], 2)
             tgs_statistic["sum_last_tg_50"] = 0
             tgs_statistic["sum_last_time_50"] = 0
 
         last_tgs_10 = tgs_statistic["last_tgs_10"]
         last_tgs_50 = tgs_statistic["last_tgs_50"]
 
-        tgs_all = round(tgs_statistic["sum_tg"] / tgs_statistic["total_time"], 2)
+        tgs_all = round(tgs_statistic["sum_tg"] / tgs_statistic["sum_time"], 2)
         tgs_avg = round(tgs_statistic["sum_tgs"] / tgs_statistic["sum_step"], 2)
         tgs_SMA = round(tgs_statistic["SMA_tg_50"] / tgs_statistic["SMA_time_50"], 2)
 
         tflops = get_tflops_func(time_cost)
 
         tgs_origin = round(
             num_tokens_in_batch
```

### Comparing `InternEvo-0.5.1.dev20240517/internlm/train/utils.py` & `InternEvo-0.5.2/internlm/train/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/common.py` & `InternEvo-0.5.2/internlm/utils/common.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/gputest.py` & `InternEvo-0.5.2/internlm/utils/gputest.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/logger.py` & `InternEvo-0.5.2/internlm/utils/logger.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/megatron_timers.py` & `InternEvo-0.5.2/internlm/utils/megatron_timers.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/parallel.py` & `InternEvo-0.5.2/internlm/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.5.2/internlm/utils/simple_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/storage_manager.py` & `InternEvo-0.5.2/internlm/utils/storage_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/timeout.py` & `InternEvo-0.5.2/internlm/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/utils.py` & `InternEvo-0.5.2/internlm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/internlm/utils/writer.py` & `InternEvo-0.5.2/internlm/utils/writer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/setup.py` & `InternEvo-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/common_fixture.py` & `InternEvo-0.5.2/tests/common_fixture.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_core/test_pipeline.py` & `InternEvo-0.5.2/tests/test_core/test_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import multiprocessing as mp
 
 import pytest
 import torch
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import Config
-from internlm.model.ops.fusion_ops_import_helper import try_import_FusedAdamW
 from internlm.utils.common import get_current_device
 from tests.test_core.utils import (
     MlpModel,
     MyLoss,
     build_environment,
     init_model_and_optim,
     loose_close,
@@ -131,15 +131,23 @@
     # engine.step()
 
     # torch related
     if gpc.is_last_rank(ParallelMode.PIPELINE):
         torch_xs = torch.tensor(x_list).to(device).to(torch.float32)
         torch_ys = torch.tensor(y_list).to(device).to(torch.float32)
         torch_model = MlpModel(0, 32, "torch").to(device)
-        adam_extra_kwargs, internlm_adamw = try_import_FusedAdamW()
+        adam_extra_kwargs = {}
+        if get_accelerator().get_accelerator_backend() == AcceleratorType.NPU:
+            import torch_npu
+
+            internlm_adamw = torch_npu.optim.NpuFusedAdamW
+        else:
+            internlm_adamw = torch.optim.AdamW
+            if torch.__version__ >= "2.1.0":
+                adam_extra_kwargs["fused"] = True
 
         torch_optimizer = internlm_adamw(
             params=[{"params": torch_model.parameters(), "weight_decay": config.adam.weight_decay}],
             lr=config.adam.lr,
             betas=(config.adam.adam_beta1, config.adam.adam_beta2),
             eps=config.adam.adam_eps,
             **adam_extra_kwargs,
```

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_core/utils.py` & `InternEvo-0.5.2/tests/test_core/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/7B_check_acc.py` & `InternEvo-0.5.2/tests/test_training/7B_check_acc.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/7B_check_init.py` & `InternEvo-0.5.2/tests/test_training/7B_check_init.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.5.2/tests/test_training/test_forward_output_no_fa.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.5.2/tests/test_training/test_load_ckpt_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/test_loss.py` & `InternEvo-0.5.2/tests/test_training/test_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/test_no_fa_train_temp.py` & `InternEvo-0.5.2/tests/test_training/test_no_fa_train_temp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/test_norm_weight.py` & `InternEvo-0.5.2/tests/test_training/test_norm_weight.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.5.2/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.1.dev20240517/tests/test_training/train_CI.py` & `InternEvo-0.5.2/tests/test_training/train_CI.py`

 * *Files identical despite different names*

