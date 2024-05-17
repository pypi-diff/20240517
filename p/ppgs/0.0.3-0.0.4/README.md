# Comparing `tmp/ppgs-0.0.3.tar.gz` & `tmp/ppgs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppgs-0.0.3.tar", last modified: Mon Mar  4 22:14:33 2024, max compression
+gzip compressed data, was "ppgs-0.0.4.tar", last modified: Fri May 17 14:51:52 2024, max compression
```

## Comparing `ppgs-0.0.3.tar` & `ppgs-0.0.4.tar`

### file list

```diff
@@ -1,144 +1,143 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.144557 ppgs-0.0.3/
--rw-rw-r--   0 max       (1000) max       (1000)     1078 2024-03-04 22:09:40.000000 ppgs-0.0.3/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)    16594 2024-03-04 22:14:33.144557 ppgs-0.0.3/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)    15412 2024-03-04 22:09:40.000000 ppgs-0.0.3/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.132557 ppgs-0.0.3/ppgs/
--rw-rw-r--   0 max       (1000) max       (1000)      874 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1635 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/__main__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.132557 ppgs-0.0.3/ppgs/assets/
--rw-rw-r--   0 max       (1000) max       (1000)     7277 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/balanced_similarity.pt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.132557 ppgs-0.0.3/ppgs/assets/configs/
--rw-rw-r--   0 max       (1000) max       (1000)     3813 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/configs/bottleneck.yaml
--rw-rw-r--   0 max       (1000) max       (1000)     4559 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/configs/ppg-quality-mushra.yaml
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.132557 ppgs-0.0.3/ppgs/assets/partitions/
--rw-rw-r--   0 max       (1000) max       (1000)   327530 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/partitions/arctic.json
--rw-rw-r--   0 max       (1000) max       (1000)       40 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/partitions/commonvoice.json.REMOVED.git-id
--rw-rw-r--   0 max       (1000) max       (1000)   142800 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/partitions/timit.json
--rw-rw-r--   0 max       (1000) max       (1000)      899 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/assets/phoneme_weights.pt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.132557 ppgs-0.0.3/ppgs/config/
--rw-rw-r--   0 max       (1000) max       (1000)       30 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/config/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     5076 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/config/defaults.py
--rw-rw-r--   0 max       (1000) max       (1000)      761 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/config/static.py
--rw-rw-r--   0 max       (1000) max       (1000)      254 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/config/w2v2fb.py
--rw-rw-r--   0 max       (1000) max       (1000)    24066 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/
--rw-rw-r--   0 max       (1000) max       (1000)      160 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     2134 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/collate.py
--rw-rw-r--   0 max       (1000) max       (1000)     7106 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/dataset.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/datasets/
--rw-rw-r--   0 max       (1000) max       (1000)       67 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/datasets/arctic/
--rw-rw-r--   0 max       (1000) max       (1000)       40 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/arctic/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     6689 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/arctic/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/datasets/arctic/words/
--rw-rw-r--   0 max       (1000) max       (1000)       40 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/arctic/words/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     5353 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/arctic/words/align.py
--rw-rw-r--   0 max       (1000) max       (1000)     6026 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/arctic/words/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/datasets/commonvoice/
--rw-rw-r--   0 max       (1000) max       (1000)       20 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/commonvoice/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     5001 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/commonvoice/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/datasets/timit/
--rw-rw-r--   0 max       (1000) max       (1000)       20 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/timit/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     9124 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/datasets/timit/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/download/
--rw-rw-r--   0 max       (1000) max       (1000)       40 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/download/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      722 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/download/__main__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/download/align/
--rw-rw-r--   0 max       (1000) max       (1000)       19 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/download/align/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     6742 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/download/align/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     1984 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/download/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     1112 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/loader.py
--rw-rw-r--   0 max       (1000) max       (1000)     2535 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/sampler.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/data/stats/
--rw-rw-r--   0 max       (1000) max       (1000)       20 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/stats/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      426 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/stats/__main__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1067 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/data/stats/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/edit/
--rw-rw-r--   0 max       (1000) max       (1000)       38 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/edit/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     4834 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/edit/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     3302 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/edit/grid.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/evaluate/
--rw-rw-r--   0 max       (1000) max       (1000)       73 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/evaluate/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      803 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/evaluate/__main__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3260 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/evaluate/core.py
--rw-rw-r--   0 max       (1000) max       (1000)    12777 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/evaluate/metrics.py
--rw-rw-r--   0 max       (1000) max       (1000)    12573 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/evaluate/visualize.py
--rw-rw-r--   0 max       (1000) max       (1000)     3931 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/load.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/model/
--rw-rw-r--   0 max       (1000) max       (1000)      173 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      806 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/convolution.py
--rw-rw-r--   0 max       (1000) max       (1000)      872 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     1852 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/mamba.py
--rw-rw-r--   0 max       (1000) max       (1000)     2692 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/transformer.py
--rw-rw-r--   0 max       (1000) max       (1000)     1602 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/w2v2.py
--rw-rw-r--   0 max       (1000) max       (1000)     1365 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/model/w2v2fc.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/partition/
--rw-rw-r--   0 max       (1000) max       (1000)       20 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/partition/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      591 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/partition/__main__.py
--rw-rw-r--   0 max       (1000) max       (1000)     2304 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/partition/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     3158 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/phonemes.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.136557 ppgs-0.0.3/ppgs/plot/
--rw-rw-r--   0 max       (1000) max       (1000)       43 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/plot/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1976 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/plot/__main__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/plot/accuracy/
--rw-rw-r--   0 max       (1000) max       (1000)       20 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/plot/accuracy/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      928 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/plot/accuracy/__main__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3900 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/plot/accuracy/core.py
--rw-rw-r--   0 max       (1000) max       (1000)    18560 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/plot/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/
--rw-rw-r--   0 max       (1000) max       (1000)     1005 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1154 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/__main__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/bottleneck/
--rw-rw-r--   0 max       (1000) max       (1000)       53 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/
--rw-rw-r--   0 max       (1000) max       (1000)       30 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     2498 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/build_ppg_model.py
--rw-rw-r--   0 max       (1000) max       (1000)      713 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/e2e_asr_common.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     7103 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/attention.py
--rw-rw-r--   0 max       (1000) max       (1000)     9297 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/conformer_encoder.py
--rw-rw-r--   0 max       (1000) max       (1000)     2108 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/convolution.py
--rw-rw-r--   0 max       (1000) max       (1000)     4847 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/embedding.py
--rw-rw-r--   0 max       (1000) max       (1000)     8765 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder.py
--rw-rw-r--   0 max       (1000) max       (1000)     5297 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder_layer.py
--rw-rw-r--   0 max       (1000) max       (1000)      874 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/layer_norm.py
--rw-rw-r--   0 max       (1000) max       (1000)     3148 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/multi_layer_conv.py
--rw-rw-r--   0 max       (1000) max       (1000)      969 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/positionwise_feed_forward.py
--rw-rw-r--   0 max       (1000) max       (1000)      676 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/repeat.py
--rw-rw-r--   0 max       (1000) max       (1000)     7216 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/subsampling.py
--rw-rw-r--   0 max       (1000) max       (1000)      483 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/swish.py
--rw-rw-r--   0 max       (1000) max       (1000)     2111 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/vgg.py
--rw-rw-r--   0 max       (1000) max       (1000)    13227 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoders.py
--rw-rw-r--   0 max       (1000) max       (1000)     4747 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/frontend.py
--rw-rw-r--   0 max       (1000) max       (1000)     2500 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/log_mel.py
--rw-rw-r--   0 max       (1000) max       (1000)     4718 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/nets_utils.py
--rw-rw-r--   0 max       (1000) max       (1000)     1878 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/stft.py
--rw-rw-r--   0 max       (1000) max       (1000)     2140 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/utterance_mvn.py
--rw-rw-r--   0 max       (1000) max       (1000)     3641 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/bottleneck/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     6465 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/core.py
--rw-rw-r--   0 max       (1000) max       (1000)     1642 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/dac.py
--rw-rw-r--   0 max       (1000) max       (1000)     1629 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/encodec.py
--rw-rw-r--   0 max       (1000) max       (1000)     2310 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/mel.py
--rw-rw-r--   0 max       (1000) max       (1000)     2027 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/spectrogram.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/w2v2fb/
--rw-rw-r--   0 max       (1000) max       (1000)       19 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/w2v2fb/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3416 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/w2v2fb/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/w2v2fc/
--rw-rw-r--   0 max       (1000) max       (1000)       19 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/w2v2fc/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3244 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/w2v2fc/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.140557 ppgs-0.0.3/ppgs/preprocess/w2v2ft/
--rw-rw-r--   0 max       (1000) max       (1000)       19 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/w2v2ft/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     2034 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/preprocess/w2v2ft/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.144557 ppgs-0.0.3/ppgs/train/
--rw-rw-r--   0 max       (1000) max       (1000)       20 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/train/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1090 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/train/__main__.py
--rw-rw-r--   0 max       (1000) max       (1000)    11802 2024-03-04 22:09:40.000000 ppgs-0.0.3/ppgs/train/core.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-03-04 22:14:33.144557 ppgs-0.0.3/ppgs.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    16594 2024-03-04 22:14:33.000000 ppgs-0.0.3/ppgs.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     3937 2024-03-04 22:14:33.000000 ppgs-0.0.3/ppgs.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2024-03-04 22:14:33.000000 ppgs-0.0.3/ppgs.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)      230 2024-03-04 22:14:33.000000 ppgs-0.0.3/ppgs.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)        5 2024-03-04 22:14:33.000000 ppgs-0.0.3/ppgs.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)       38 2024-03-04 22:14:33.144557 ppgs-0.0.3/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)     1273 2024-03-04 22:13:49.000000 ppgs-0.0.3/setup.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.223160 ppgs-0.0.4/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1078 2024-05-14 15:36:24.000000 ppgs-0.0.4/LICENSE
+-rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    16188 2024-05-17 14:51:52.223160 ppgs-0.0.4/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    15113 2024-05-17 14:36:27.000000 ppgs-0.0.4/README.md
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.183160 ppgs-0.0.4/ppgs/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      874 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1494 2024-05-17 14:36:18.000000 ppgs-0.0.4/ppgs/__main__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.183160 ppgs-0.0.4/ppgs/assets/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     7277 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/assets/balanced_similarity.pt
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.183160 ppgs-0.0.4/ppgs/assets/configs/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3813 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/assets/configs/bottleneck.yaml
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4559 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/assets/configs/ppg-quality-mushra.yaml
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/assets/partitions/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   327530 2024-05-17 14:25:56.000000 ppgs-0.0.4/ppgs/assets/partitions/arctic.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001) 31082871 2024-05-17 14:25:59.000000 ppgs-0.0.4/ppgs/assets/partitions/commonvoice.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   142800 2024-05-17 14:26:01.000000 ppgs-0.0.4/ppgs/assets/partitions/timit.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      899 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/assets/phoneme_weights.pt
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/config/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       30 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/config/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5304 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/config/defaults.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      770 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/config/static.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      254 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/config/w2v2fb.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    18148 2024-05-17 14:32:54.000000 ppgs-0.0.4/ppgs/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      160 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2195 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/data/collate.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     7144 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/data/dataset.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/datasets/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       67 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/__init__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/datasets/arctic/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       40 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/arctic/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     6689 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/arctic/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/datasets/arctic/words/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       40 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/arctic/words/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5353 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/arctic/words/align.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     6026 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/arctic/words/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/datasets/commonvoice/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/commonvoice/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5001 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/commonvoice/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/datasets/timit/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/timit/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9124 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/datasets/timit/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/download/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       40 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/download/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      722 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/download/__main__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/download/align/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/download/align/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     6729 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/data/download/align/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1988 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/data/download/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1112 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/loader.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2536 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/data/sampler.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/data/stats/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/stats/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      426 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/stats/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1067 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/data/stats/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/edit/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/edit/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5941 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/edit/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3302 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/edit/grid.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.215160 ppgs-0.0.4/ppgs/evaluate/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       73 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/evaluate/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      803 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/evaluate/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3273 2024-05-17 14:15:37.000000 ppgs-0.0.4/ppgs/evaluate/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12777 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/evaluate/metrics.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12573 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/evaluate/visualize.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4091 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/load.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/model/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      148 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/model/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      806 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/model/convolution.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      806 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/model/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3027 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/model/transformer.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1602 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/model/w2v2.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1365 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/model/w2v2fc.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/partition/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/partition/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      591 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/partition/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2304 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/partition/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3158 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/phonemes.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/plot/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       43 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/plot/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1380 2024-05-17 14:47:44.000000 ppgs-0.0.4/ppgs/plot/__main__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/plot/accuracy/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/plot/accuracy/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      928 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/plot/accuracy/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3900 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/plot/accuracy/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    15726 2024-05-17 14:45:55.000000 ppgs-0.0.4/ppgs/plot/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/preprocess/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1005 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1154 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/__main__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/preprocess/bottleneck/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       53 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/__init__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       30 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2498 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/build_ppg_model.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      713 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/e2e_asr_common.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.219160 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     7103 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/attention.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9297 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/conformer_encoder.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2108 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/convolution.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4847 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/embedding.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8765 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5297 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder_layer.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      874 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/layer_norm.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3148 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/multi_layer_conv.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      969 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/positionwise_feed_forward.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      676 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/repeat.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     7216 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/subsampling.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      483 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/swish.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2111 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/vgg.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    13227 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoders.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4747 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/frontend.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2500 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/log_mel.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4718 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/nets_utils.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1878 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/stft.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2140 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/utterance_mvn.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3641 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/bottleneck/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     6483 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/preprocess/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1405 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/preprocess/dac.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1630 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/preprocess/encodec.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2310 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/mel.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2027 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/spectrogram.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.223160 ppgs-0.0.4/ppgs/preprocess/w2v2fb/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/w2v2fb/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3438 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/preprocess/w2v2fb/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.223160 ppgs-0.0.4/ppgs/preprocess/w2v2fc/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/w2v2fc/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3278 2024-05-14 15:41:12.000000 ppgs-0.0.4/ppgs/preprocess/w2v2fc/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.223160 ppgs-0.0.4/ppgs/preprocess/w2v2ft/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/w2v2ft/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2034 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/preprocess/w2v2ft/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.223160 ppgs-0.0.4/ppgs/train/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-14 15:36:24.000000 ppgs-0.0.4/ppgs/train/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1121 2024-05-14 20:33:25.000000 ppgs-0.0.4/ppgs/train/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    11777 2024-05-14 20:46:38.000000 ppgs-0.0.4/ppgs/train/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-17 14:51:52.223160 ppgs-0.0.4/ppgs.egg-info/
+-rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    16188 2024-05-17 14:51:52.000000 ppgs-0.0.4/ppgs.egg-info/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3902 2024-05-17 14:51:52.000000 ppgs-0.0.4/ppgs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2024-05-17 14:51:52.000000 ppgs-0.0.4/ppgs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      207 2024-05-17 14:51:52.000000 ppgs-0.0.4/ppgs.egg-info/requires.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        5 2024-05-17 14:51:52.000000 ppgs-0.0.4/ppgs.egg-info/top_level.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2024-05-17 14:51:52.223160 ppgs-0.0.4/setup.cfg
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1217 2024-05-14 15:41:12.000000 ppgs-0.0.4/setup.py
```

### Comparing `ppgs-0.0.3/LICENSE` & `ppgs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/PKG-INFO` & `ppgs-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: ppgs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Phonetic posteriorgrams
 Home-page: https://github.com/interactiveaudiolab/ppgs
 Author: Interactive Audio Lab
 Author-email: interactiveaudiolab@gmail.com
 License: MIT
 Keywords: phonemes,ppg,pronunciation,speech
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: espnet
 Requires-Dist: huggingface-hub
+Requires-Dist: librosa
+Requires-Dist: matplotlib
 Requires-Dist: moviepy
 Requires-Dist: numpy
 Requires-Dist: pypar
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchutil
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: opencv-python
 Requires-Dist: yapecs
-Requires-Dist: gdown>=4.6.2
 Provides-Extra: train
 Requires-Dist: dac; extra == "train"
 Requires-Dist: encodec; extra == "train"
 Requires-Dist: g2pM; extra == "train"
 Requires-Dist: gdown>=4.6.2; extra == "train"
 Requires-Dist: humanfriendly; extra == "train"
-Requires-Dist: librosa; extra == "train"
-Requires-Dist: mamba-ssm; extra == "train"
-Requires-Dist: matplotlib; extra == "train"
 Requires-Dist: nltk; extra == "train"
 Requires-Dist: pyyaml; extra == "train"
 Requires-Dist: torch-complex; extra == "train"
 
 <h1 align="center">High-Fidelity Neural Phonetic Posteriorgrams</h1>
 <div align="center">
 
@@ -54,15 +52,14 @@
 - [Installation](#installation)
 - [Inference](#inference)
     * [Application programming interface (API)](#application-programming-interface-api)
         * [`ppgs.from_audio`](#ppgsfrom_audio)
         * [`ppgs.from_file`](#ppgsfrom_file)
         * [`ppgs.from_file_to_file`](#ppgsfrom_file_to_file)
         * [`ppgs.from_files_to_files`](#ppgsfrom_files_to_files)
-        * [`ppgs.from_paths_to_paths`](#ppgsfrom_paths_to_paths)
     * [Command-line interface (CLI)](#command-line-interface-cli)
 - [Distance](#distance)
 - [Interpolate](#interpolate)
 - [Edit](#edit)
     * [`ppgs.edit.grid.constant`](#ppgseditgridconstant)
     * [`ppgs.edit.grid.from_alignments`](#ppgseditgridfrom_alignments)
     * [`ppgs.edit.grid.of_length`](#ppgseditgridof_length)
@@ -134,25 +131,28 @@
 
 #### `ppgs.from_audio`
 
 ```python
 def from_audio(
     audio: torch.Tensor,
     sample_rate: Union[int, float],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: int = None
 ) -> torch.Tensor:
     """Infer ppgs from audio
 
     Arguments
         audio
             Batched audio to process
             shape=(batch, 1, samples)
         sample_rate
             Audio sampling rate
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
 
     Returns
         ppgs
@@ -163,22 +163,25 @@
 
 
 #### `ppgs.from_file`
 
 ```python
 def from_file(
     file: Union[str, bytes, os.PathLike],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> torch.Tensor:
     """Infer ppgs from an audio file
 
     Arguments
         file
             The audio file
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
 
     Returns
         ppgs
@@ -190,83 +193,56 @@
 
 #### `ppgs.from_file_to_file`
 
 ```python
 def from_file_to_file(
     audio_file: Union[str, bytes, os.PathLike],
     output_file: Union[str, bytes, os.PathLike],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> None:
     """Infer ppg from an audio file and save to a torch tensor file
 
     Arguments
         audio_file
             The audio file
         output_file
             The .pt file to save PPGs
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
     """
 ```
 
 
 #### `ppgs.from_files_to_files`
 
 ```python
 def from_files_to_files(
     audio_files: List[Union[str, bytes, os.PathLike]],
     output_files: List[Union[str, bytes, os.PathLike]],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = ppgs.NUM_WORKERS,
+    num_workers: int = 0,
     gpu: Optional[int] = None,
     max_frames: int = ppgs.MAX_INFERENCE_FRAMES
 ) -> None:
     """Infer ppgs from audio files and save to torch tensor files
 
     Arguments
         audio_files
             The audio files
         output_files
             The .pt files to save PPGs
-        checkpoint
-            The checkpoint file
-        num_workers
-            Number of CPU threads for multiprocessing
-        gpu
-            The index of the GPU to use for inference
-        max_frames
-            The maximum number of frames on the GPU at once
-    """
-```
-
-
-#### `ppgs.from_paths_to_paths`
-
-```python
-def from_paths_to_paths(
-    input_paths: List[Union[str, bytes, os.PathLike]],
-    output_paths: Optional[List[Union[str, bytes, os.PathLike]]] = None,
-    extensions: Optional[List[str]] = None,
-    checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = ppgs.NUM_WORKERS,
-    gpu: Optional[int] = None,
-    max_frames: int = ppgs.MAX_INFERENCE_FRAMES
-) -> None:
-    """Infer ppgs from audio files and save to torch tensor files
-
-    Arguments
-        input_paths
-            Paths to audio files and/or directories
-        output_paths
-            The one-to-one corresponding outputs
-        extensions
-            Extensions to glob for in directories
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         num_workers
             Number of CPU threads for multiprocessing
         gpu
             The index of the GPU to use for inference
         max_frames
@@ -276,67 +252,72 @@
 
 
 ### Command-line interface (CLI)
 
 ```
 usage: python -m ppgs
     [-h]
-    [--input_paths INPUT_PATHS [INPUT_PATHS ...]]
-    [--output_paths OUTPUT_PATHS [OUTPUT_PATHS ...]]
-    [--extensions EXTENSIONS [EXTENSIONS ...]]
+    [--audio_files AUDIO_FILES [AUDIO_FILES ...]]
+    [--output_files OUTPUT_FILES [OUTPUT_FILES ...]]
+    [--representation REPRESENTATION]
     [--checkpoint CHECKPOINT]
     [--num-workers NUM_WORKERS]
     [--gpu GPU]
     [--max-frames MAX_TRAINING_FRAMES]
 
 arguments:
-    --input_paths INPUT_PATHS [INPUT_PATHS ...]
-        Paths to audio files and/or directories
+    --audio_files AUDIO_FILES [AUDIO_FILES ...]
+        Paths to input audio files
+    --output_files OUTPUT_FILES [OUTPUT_FILES ...]
+        The one-to-one corresponding output files
 
 optional arguments:
     -h, --help
         Show this help message and exit
-    --output_paths OUTPUT_PATHS [OUTPUT_PATHS ...]
-        The one-to-one corresponding output paths
-    --extensions EXTENSIONS [EXTENSIONS ...]
-        Extensions to glob for in directories
+    --representation REPRESENTATION
+        Representation to use for inference
     --checkpoint CHECKPOINT
         The checkpoint file
     --num-workers NUM_WORKERS
         Number of CPU threads for multiprocessing
     --gpu GPU
         The index of the GPU to use for inference. Defaults to CPU.
+    --max-frames MAX_FRAMES
+        Maximum number of frames in a batch
 ```
 
 
 ## Distance
 
 To compute the proposed normalized Jenson-Shannon divergence pronunciation
 distance between two PPGs, use `ppgs.distance()`.
 
 ```python
 def distance(
     ppgX: torch.Tensor,
     ppgY: torch.Tensor,
     reduction: str = 'mean',
-    normalize: bool = True
+    normalize: bool = True,
+    exponent: float = ppgs.SIMILARITY_EXPONENT
 ) -> torch.Tensor:
     """Compute the pronunciation distance between two aligned PPGs
 
     Arguments
         ppgX
             Input PPG X
             shape=(len(ppgs.PHONEMES), frames)
         ppgY
             Input PPG Y to compare with PPG X
             shape=(len(ppgs.PHONEMES), frames)
         reduction
             Reduction to apply to the output. One of ['mean', 'none', 'sum'].
         normalize
             Apply similarity based normalization
+        exponent
+            Similarty exponent
 
     Returns
         Normalized Jenson-shannon divergence between PPGs
     """
 ```
 
 
@@ -557,21 +538,22 @@
             Input phoneme B
 
     Returns
         Edited PPG
     """
 ```
 
+
 ## Sparsify
 
 ```python
 def sparsify(
     ppg: torch.Tensor,
-    method: str='percentile',
-    threshold: Union[float, int]=0.85
+    method: str = 'percentile',
+    threshold: Union[float, int] = 0.85
 ) -> torch.Tensor:
     """Make phonetic posteriorgrams sparse
 
     Arguments
         ppg
             Input PPG
             shape=(*, len(ppgs.PHONEMES), frames)
@@ -605,15 +587,15 @@
 
 ### Preprocess
 
 Prepares representations for training. Representations are stored
 in `data/cache/`.
 
 ```
-python -m ppgs.data.preprocess \
+python -m ppgs.preprocess \
    --datasets <datasets> \
    --representatations <representations> \
    --gpu <gpu> \
    --num-workers <workers>
 ```
 
 
@@ -656,15 +638,19 @@
 
 ### Evaluate
 
 Performs objective evaluation of phoneme accuracy. Results are stored
 in `eval/`.
 
 ```
-python -m ppgs.evaluate --config <name> --datasets <datasets> --gpu <gpu>
+python -m ppgs.evaluate \
+    --config <name> \
+    --datasets <datasets> \
+    --checkpoint <checkpoint> \
+    --gpu <gpu>
 ```
 
 
 ## Citation
 
 ### IEEE
 C. Churchwell, M. Morrison, and B. Pardo, "High-Fidelity Neural Phonetic Posteriorgrams,"
```

### Comparing `ppgs-0.0.3/README.md` & `ppgs-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 - [Installation](#installation)
 - [Inference](#inference)
     * [Application programming interface (API)](#application-programming-interface-api)
         * [`ppgs.from_audio`](#ppgsfrom_audio)
         * [`ppgs.from_file`](#ppgsfrom_file)
         * [`ppgs.from_file_to_file`](#ppgsfrom_file_to_file)
         * [`ppgs.from_files_to_files`](#ppgsfrom_files_to_files)
-        * [`ppgs.from_paths_to_paths`](#ppgsfrom_paths_to_paths)
     * [Command-line interface (CLI)](#command-line-interface-cli)
 - [Distance](#distance)
 - [Interpolate](#interpolate)
 - [Edit](#edit)
     * [`ppgs.edit.grid.constant`](#ppgseditgridconstant)
     * [`ppgs.edit.grid.from_alignments`](#ppgseditgridfrom_alignments)
     * [`ppgs.edit.grid.of_length`](#ppgseditgridof_length)
@@ -96,25 +95,28 @@
 
 #### `ppgs.from_audio`
 
 ```python
 def from_audio(
     audio: torch.Tensor,
     sample_rate: Union[int, float],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: int = None
 ) -> torch.Tensor:
     """Infer ppgs from audio
 
     Arguments
         audio
             Batched audio to process
             shape=(batch, 1, samples)
         sample_rate
             Audio sampling rate
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
 
     Returns
         ppgs
@@ -125,22 +127,25 @@
 
 
 #### `ppgs.from_file`
 
 ```python
 def from_file(
     file: Union[str, bytes, os.PathLike],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> torch.Tensor:
     """Infer ppgs from an audio file
 
     Arguments
         file
             The audio file
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
 
     Returns
         ppgs
@@ -152,83 +157,56 @@
 
 #### `ppgs.from_file_to_file`
 
 ```python
 def from_file_to_file(
     audio_file: Union[str, bytes, os.PathLike],
     output_file: Union[str, bytes, os.PathLike],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> None:
     """Infer ppg from an audio file and save to a torch tensor file
 
     Arguments
         audio_file
             The audio file
         output_file
             The .pt file to save PPGs
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
     """
 ```
 
 
 #### `ppgs.from_files_to_files`
 
 ```python
 def from_files_to_files(
     audio_files: List[Union[str, bytes, os.PathLike]],
     output_files: List[Union[str, bytes, os.PathLike]],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = ppgs.NUM_WORKERS,
+    num_workers: int = 0,
     gpu: Optional[int] = None,
     max_frames: int = ppgs.MAX_INFERENCE_FRAMES
 ) -> None:
     """Infer ppgs from audio files and save to torch tensor files
 
     Arguments
         audio_files
             The audio files
         output_files
             The .pt files to save PPGs
-        checkpoint
-            The checkpoint file
-        num_workers
-            Number of CPU threads for multiprocessing
-        gpu
-            The index of the GPU to use for inference
-        max_frames
-            The maximum number of frames on the GPU at once
-    """
-```
-
-
-#### `ppgs.from_paths_to_paths`
-
-```python
-def from_paths_to_paths(
-    input_paths: List[Union[str, bytes, os.PathLike]],
-    output_paths: Optional[List[Union[str, bytes, os.PathLike]]] = None,
-    extensions: Optional[List[str]] = None,
-    checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = ppgs.NUM_WORKERS,
-    gpu: Optional[int] = None,
-    max_frames: int = ppgs.MAX_INFERENCE_FRAMES
-) -> None:
-    """Infer ppgs from audio files and save to torch tensor files
-
-    Arguments
-        input_paths
-            Paths to audio files and/or directories
-        output_paths
-            The one-to-one corresponding outputs
-        extensions
-            Extensions to glob for in directories
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         num_workers
             Number of CPU threads for multiprocessing
         gpu
             The index of the GPU to use for inference
         max_frames
@@ -238,67 +216,72 @@
 
 
 ### Command-line interface (CLI)
 
 ```
 usage: python -m ppgs
     [-h]
-    [--input_paths INPUT_PATHS [INPUT_PATHS ...]]
-    [--output_paths OUTPUT_PATHS [OUTPUT_PATHS ...]]
-    [--extensions EXTENSIONS [EXTENSIONS ...]]
+    [--audio_files AUDIO_FILES [AUDIO_FILES ...]]
+    [--output_files OUTPUT_FILES [OUTPUT_FILES ...]]
+    [--representation REPRESENTATION]
     [--checkpoint CHECKPOINT]
     [--num-workers NUM_WORKERS]
     [--gpu GPU]
     [--max-frames MAX_TRAINING_FRAMES]
 
 arguments:
-    --input_paths INPUT_PATHS [INPUT_PATHS ...]
-        Paths to audio files and/or directories
+    --audio_files AUDIO_FILES [AUDIO_FILES ...]
+        Paths to input audio files
+    --output_files OUTPUT_FILES [OUTPUT_FILES ...]
+        The one-to-one corresponding output files
 
 optional arguments:
     -h, --help
         Show this help message and exit
-    --output_paths OUTPUT_PATHS [OUTPUT_PATHS ...]
-        The one-to-one corresponding output paths
-    --extensions EXTENSIONS [EXTENSIONS ...]
-        Extensions to glob for in directories
+    --representation REPRESENTATION
+        Representation to use for inference
     --checkpoint CHECKPOINT
         The checkpoint file
     --num-workers NUM_WORKERS
         Number of CPU threads for multiprocessing
     --gpu GPU
         The index of the GPU to use for inference. Defaults to CPU.
+    --max-frames MAX_FRAMES
+        Maximum number of frames in a batch
 ```
 
 
 ## Distance
 
 To compute the proposed normalized Jenson-Shannon divergence pronunciation
 distance between two PPGs, use `ppgs.distance()`.
 
 ```python
 def distance(
     ppgX: torch.Tensor,
     ppgY: torch.Tensor,
     reduction: str = 'mean',
-    normalize: bool = True
+    normalize: bool = True,
+    exponent: float = ppgs.SIMILARITY_EXPONENT
 ) -> torch.Tensor:
     """Compute the pronunciation distance between two aligned PPGs
 
     Arguments
         ppgX
             Input PPG X
             shape=(len(ppgs.PHONEMES), frames)
         ppgY
             Input PPG Y to compare with PPG X
             shape=(len(ppgs.PHONEMES), frames)
         reduction
             Reduction to apply to the output. One of ['mean', 'none', 'sum'].
         normalize
             Apply similarity based normalization
+        exponent
+            Similarty exponent
 
     Returns
         Normalized Jenson-shannon divergence between PPGs
     """
 ```
 
 
@@ -519,21 +502,22 @@
             Input phoneme B
 
     Returns
         Edited PPG
     """
 ```
 
+
 ## Sparsify
 
 ```python
 def sparsify(
     ppg: torch.Tensor,
-    method: str='percentile',
-    threshold: Union[float, int]=0.85
+    method: str = 'percentile',
+    threshold: Union[float, int] = 0.85
 ) -> torch.Tensor:
     """Make phonetic posteriorgrams sparse
 
     Arguments
         ppg
             Input PPG
             shape=(*, len(ppgs.PHONEMES), frames)
@@ -567,15 +551,15 @@
 
 ### Preprocess
 
 Prepares representations for training. Representations are stored
 in `data/cache/`.
 
 ```
-python -m ppgs.data.preprocess \
+python -m ppgs.preprocess \
    --datasets <datasets> \
    --representatations <representations> \
    --gpu <gpu> \
    --num-workers <workers>
 ```
 
 
@@ -618,15 +602,19 @@
 
 ### Evaluate
 
 Performs objective evaluation of phoneme accuracy. Results are stored
 in `eval/`.
 
 ```
-python -m ppgs.evaluate --config <name> --datasets <datasets> --gpu <gpu>
+python -m ppgs.evaluate \
+    --config <name> \
+    --datasets <datasets> \
+    --checkpoint <checkpoint> \
+    --gpu <gpu>
 ```
 
 
 ## Citation
 
 ### IEEE
 C. Churchwell, M. Morrison, and B. Pardo, "High-Fidelity Neural Phonetic Posteriorgrams,"
```

### Comparing `ppgs-0.0.3/ppgs/__init__.py` & `ppgs-0.0.4/ppgs/__init__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/__main__.py` & `ppgs-0.0.4/ppgs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 
 
 def parse_args():
     """Parse command-line arguments"""
     parser = yapecs.ArgumentParser(
         description='Phonetic posteriorgram inference')
     parser.add_argument(
-        '--input_paths',
+        '--audio_files',
         nargs='+',
         type=Path,
         required=True,
-        help='Paths to audio files and/or directories')
+        help='Paths to audio files')
     parser.add_argument(
-        '--output_paths',
+        '--output_files',
         type=Path,
+        required=True,
         nargs='+',
-        help='The one-to-one corresponding output paths')
+        help='The one-to-one corresponding output files')
     parser.add_argument(
-        '--extensions',
-        nargs='+',
+        '--representation',
         type=str,
-        help='Extensions to glob for in directories')
+        default=None,
+        help='Representation to use for inference')
     parser.add_argument(
         '--checkpoint',
         type=Path,
         help='The checkpoint file')
     parser.add_argument(
         '--num-workers',
         type=int,
@@ -43,17 +44,11 @@
         type=int,
         help='The index of the GPU to use for inference. Defaults to CPU.')
     parser.add_argument(
         '--max-frames',
         type=int,
         default=ppgs.MAX_INFERENCE_FRAMES,
         help='Maximum number of frames in a batch')
-    parser.add_argument(
-        '--representation',
-        type=str,
-        default=None,
-        help='Representation to use for inference'
-    )
     return parser.parse_args()
 
 
-ppgs.from_paths_to_paths(**vars(parse_args()))
+ppgs.from_files_to_files(**vars(parse_args()))
```

### Comparing `ppgs-0.0.3/ppgs/assets/balanced_similarity.pt` & `ppgs-0.0.4/ppgs/assets/balanced_similarity.pt`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/assets/configs/bottleneck.yaml` & `ppgs-0.0.4/ppgs/assets/configs/bottleneck.yaml`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/assets/configs/ppg-quality-mushra.yaml` & `ppgs-0.0.4/ppgs/assets/configs/ppg-quality-mushra.yaml`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/assets/partitions/arctic.json` & `ppgs-0.0.4/ppgs/assets/partitions/arctic.json`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/assets/partitions/timit.json` & `ppgs-0.0.4/ppgs/assets/partitions/timit.json`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/assets/phoneme_weights.pt` & `ppgs-0.0.4/ppgs/assets/phoneme_weights.pt`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/config/defaults.py` & `ppgs-0.0.4/ppgs/config/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,31 +61,40 @@
 
 
 ###############################################################################
 # Directories
 ###############################################################################
 
 
+# Root location for saving outputs
+ROOT_DIR = Path(__file__).parent.parent.parent
+
 # Location to save assets to be bundled with pip release
 ASSETS_DIR = Path(__file__).parent.parent / 'assets'
 
 # Location of initial downloads before processing into DATA_DIR
 SOURCES_DIR = Path(__file__).parent.parent.parent / 'data' / 'sources'
 
 # Location of preprocessed features
-CACHE_DIR = Path(__file__).parent.parent.parent / 'data' / 'cache'
+CACHE_DIR = ROOT_DIR / 'data' / 'cache'
 
 # Location of datasets on disk
-DATA_DIR = Path(__file__).parent.parent.parent / 'data' / 'datasets'
+DATA_DIR = ROOT_DIR / 'data' / 'datasets'
 
 # Location to save evaluation artifacts
-EVAL_DIR = Path(__file__).parent.parent.parent / 'eval'
+EVAL_DIR = ROOT_DIR / 'eval'
 
 # Location to save training and adaptation artifacts
-RUNS_DIR = Path(__file__).parent.parent.parent / 'runs'
+RUNS_DIR = ROOT_DIR / 'runs'
+
+# Location of initial downloads before processing into DATA_DIR
+SOURCES_DIR = ROOT_DIR / 'data' / 'sources'
+
+# Location of similarity matrix
+SIMILARITY_MATRIX_PATH = ASSETS_DIR / 'balanced_similarity.pt'
 
 # Location of checkpoints
 CHECKPOINT_DIR = ASSETS_DIR / 'checkpoints'
 
 # Location of similarity matrix
 SIMILARITY_MATRIX_PATH = ASSETS_DIR / 'balanced_similarity.pt'
 
@@ -116,14 +125,17 @@
 
 # Number of attention heads
 ATTENTION_HEADS = 2
 
 # Attention window size
 ATTENTION_WINDOW_SIZE = 4
 
+# Use causal masking/methods
+IS_CAUSAL = False
+
 # This function takes as input a torch.Device and returns a callable frontend
 FRONTEND = None
 
 # Network width
 HIDDEN_CHANNELS = 256
 
 # Dimensionality of input representation
```

### Comparing `ppgs-0.0.3/ppgs/config/static.py` & `ppgs-0.0.4/ppgs/config/static.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 
 ###############################################################################
 # Data parameters
 ###############################################################################
 
 
 # Maximum number of frames on the GPU during inference
-MAX_INFERENCE_FRAMES = min(ppgs.MAX_TRAINING_FRAMES, ppgs.MAX_PREPROCESS_FRAMES)
+MAX_INFERENCE_FRAMES = min(
+    ppgs.MAX_TRAINING_FRAMES,
+    ppgs.MAX_PREPROCESS_FRAMES)
```

### Comparing `ppgs-0.0.3/ppgs/core.py` & `ppgs-0.0.4/ppgs/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Application programming interface
 ###############################################################################
 
 
 def from_audio(
     audio: torch.Tensor,
     sample_rate: Union[int, float],
-    representation: Optional[str] = None,
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: int = None
 ) -> torch.Tensor:
     """Infer ppgs from audio
 
     Arguments
         audio
@@ -47,33 +47,32 @@
             shape=(batch, len(ppgs.PHONEMES), frames)
     """
     # Preprocess
     features = ppgs.preprocess.from_audio(
         audio=audio,
         sample_rate=sample_rate,
         representation=representation,
-        gpu=gpu
-    )
+        gpu=gpu)
 
     # Get length in frames
     length = torch.tensor([features.shape[-1]], dtype=torch.long)
 
     # Infer
     return from_features(
         features=features,
-        lengths=length, 
+        lengths=length,
         representation=representation,
-        checkpoint=checkpoint, 
+        checkpoint=checkpoint,
         gpu=gpu)
 
 
 def from_features(
     features: torch.Tensor,
     lengths: torch.Tensor,
-    representation: Optional[str],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None,
     softmax: bool = True
 ) -> torch.Tensor:
     """Infer ppgs from input features (e.g. w2v2fb, mel, etc.)
 
     Arguments
@@ -96,35 +95,38 @@
         ppgs
             Phonetic posteriorgrams
             shape=(batch, len(ppgs.PHONEMES), frames)
     """
     device = torch.device('cpu' if gpu is None else f'cuda:{gpu}')
 
     if representation is None: # neither mel nor w2v2fb have a frontend
+
         # Maybe load and cache codebook
-        if not hasattr(from_features, 'frontend') and ppgs.FRONTEND is not None:
+        if (
+            not hasattr(from_features, 'frontend') and
+            ppgs.FRONTEND is not None
+        ):
             from_features.frontend = ppgs.FRONTEND(device)
 
         # Codebook lookup
         if hasattr(from_features, 'frontend'):
             features = from_features.frontend(features.to(device))
 
     # Infer
     return infer(
         features=features.to(device),
         lengths=lengths.to(device),
         representation=representation,
         checkpoint=checkpoint,
-        softmax=softmax
-    )
+        softmax=softmax)
 
 
 def from_file(
     file: Union[str, bytes, os.PathLike],
-    representation: Optional[str] = None,
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> torch.Tensor:
     """Infer ppgs from an audio file
 
     Arguments
         file
@@ -153,15 +155,15 @@
         gpu=gpu
     ).squeeze(0)
 
 
 def from_file_to_file(
     audio_file: Union[str, bytes, os.PathLike],
     output_file: Union[str, bytes, os.PathLike],
-    representation: Optional[str] = None,
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> None:
     """Infer ppg from an audio file and save to a torch tensor file
 
     Arguments
         audio_file
@@ -173,28 +175,27 @@
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
     """
     # Compute PPGs
     result = from_file(
-        file=audio_file, 
-        checkpoint=checkpoint, 
+        file=audio_file,
+        checkpoint=checkpoint,
         representation=representation,
-        gpu=gpu
-    )
+        gpu=gpu)
 
     # Save to disk
     torch.save(result.detach().cpu(), output_file)
 
 
 def from_files_to_files(
     audio_files: List[Union[str, bytes, os.PathLike]],
     output_files: List[Union[str, bytes, os.PathLike]],
-    representation: Optional[str] = None,
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     num_workers: int = 0,
     gpu: Optional[int] = None,
     max_frames: int = ppgs.MAX_INFERENCE_FRAMES
 ) -> None:
     """Infer ppgs from audio files and save to torch tensor files
 
@@ -241,81 +242,30 @@
 
         # Batch inference
         from_dataloader(
             dataloader=dataloader,
             output_files=output_files,
             representation=representation,
             checkpoint=checkpoint,
-            num_workers=num_workers // 2,
+            save_workers=num_workers // 2,
             gpu=gpu
         )
 
 
-def from_paths_to_paths(
-    input_paths: List[Union[str, bytes, os.PathLike]],
-    output_paths: Optional[List[Union[str, bytes, os.PathLike]]] = None,
-    extensions: Optional[List[str]] = None,
-    representation: Optional[str] = None,
-    checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = 0,
-    gpu: Optional[int] = None,
-    max_frames: int = ppgs.MAX_INFERENCE_FRAMES
-) -> None:
-    """Infer ppgs from audio files and save to torch tensor files
-
-    Arguments
-        input_paths
-            Paths to audio files and/or directories
-        output_paths
-            The one-to-one corresponding outputs
-        extensions
-            Extensions to glob for in directories
-        representation
-            The representation to use, 'mel' and 'w2v2fb' are currently supported
-        checkpoint
-            The checkpoint file
-        num_workers
-            Number of CPU threads for multiprocessing
-        gpu
-            The index of the GPU to use for inference
-        max_frames
-            The maximum number of frames on the GPU at once
-    """
-    if output_paths is not None:
-        input_files, output_files = aggregate(
-            input_paths,
-            sinks=output_paths,
-            source_extensions=extensions,
-            sink_extension=f'-{ppgs.REPRESENTATION}-ppg.pt')
-    else:
-        input_files, output_files = aggregate(
-            input_paths,
-            source_extensions=extensions)
-    from_files_to_files(
-        audio_files=input_files,
-        output_files=output_files,
-        representation=representation,
-        checkpoint=checkpoint,
-        num_workers=num_workers,
-        gpu=gpu,
-        max_frames=max_frames
-    )
-
-
 ###############################################################################
 # Multiprocessing
 ###############################################################################
 
 
 def from_dataloader(
     dataloader: torch.utils.data.DataLoader,
     output_files: Dict[
         Union[str, bytes, os.PathLike],
         Union[str, bytes, os.PathLike]],
-    representation: Optional[str] = ppgs.REPRESENTATION,
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Union[str, bytes, os.PathLike] = None,
     save_workers: int = 1,
     gpu: Optional[int] = None
 ) -> None:
     """Infer ppgs from a dataloader yielding audio files
 
     Arguments
@@ -362,15 +312,15 @@
                 ).from_audios(
                     audios,
                     lengths,
                     gpu=gpu)
                 attention_mask_lengths = frame_lengths
 
             if features.requires_grad:
-                raise ValueError('all representations should be detached!')
+                raise ValueError('All representations should be detached')
 
             # Infer
             result = from_features(
                 features=features,
                 lengths=attention_mask_lengths,
                 representation=representation,
                 checkpoint=checkpoint,
@@ -437,14 +387,16 @@
         ppgY
             Input PPG Y to compare with PPG X
             shape=(len(ppgs.PHONEMES), frames)
         reduction
             Reduction to apply to the output. One of ['mean', 'none', 'sum'].
         normalize
             Apply similarity based normalization
+        exponent
+            Similarty exponent
 
     Returns
         Normalized Jenson-shannon divergence between PPGs
     """
     # Handle numerical instability at boundaries
     ppgX = torch.clamp(ppgX, 1e-8, 1 - 1e-8)
     ppgY = torch.clamp(ppgY, 1e-8, 1 - 1e-8)
@@ -518,21 +470,23 @@
     Returns
         Interpolated PPGs
         shape=(len(ppgs.PHONEMES), frames)
     """
     # "acos_vml_cpu" not implemented for 'Half'
     dtype = ppgX.dtype
     if dtype in [torch.float16, torch.bfloat16]:
-        omega = torch.acos(
-            (ppgX.to(torch.float32) * ppgY.to(torch.float32)).sum(
-                -2,
-                keepdim=True)
-        ).to(dtype)
+        p = ppgX.to(torch.float32) * ppgY.to(torch.float32)
+        s = p.sum(-2, keepdim=True)
+        s = s.clamp(-1.0, 1.0)
+        omega = torch.acos(s).to(dtype)
     else:
-        omega = torch.acos((ppgX * ppgY).sum(-2, keepdim=True))
+        p = ppgX * ppgY
+        s = p.sum(-2, keepdim=True)
+        s = s.clamp(-1.0, 1.0)
+        omega = torch.acos(s)
 
     sin_omega = torch.clip(torch.sin(omega), 1e-6)
     interpolated = (
         torch.sin((1. - interp) * omega) / sin_omega * ppgX +
         torch.sin(interp * omega) / sin_omega * ppgY)
 
     # Fix locations where ppgX == ppgY
@@ -546,16 +500,16 @@
 ###############################################################################
 # PPG sparsification
 ###############################################################################
 
 
 def sparsify(
     ppg: torch.Tensor,
-    method: str='percentile',
-    threshold: Union[float, int]=0.85
+    method: str = 'percentile',
+    threshold: Union[float, int] = 0.85
 ) -> torch.Tensor:
     """Make phonetic posteriorgrams sparse
 
     Arguments
         ppg
             Input PPG
             shape=(*, len(ppgs.PHONEMES), frames)
@@ -588,126 +542,20 @@
 
 
 ###############################################################################
 # Utilities
 ###############################################################################
 
 
-def aggregate(
-    *sources: List[Union[str, bytes, os.PathLike]],
-    sinks: Optional[List[Union[str, bytes, os.PathLike]]] = None,
-    source_extensions: Optional[str] = None,
-    sink_extension: str = '.pt'):
-    """
-    Aggregates lists of input and output directories and files into two lists
-    of files, using the provided extension to glob directories.
-    """
-    if len(sources) == 0:
-        raise ValueError('At least one source list must be provided')
-    elif len(sources) == 1:
-        assert sources[0] is not None, 'At least one source list must be provieded, but found None'
-    else:
-        assert source_extensions is None
-
-    sources = list(sources)
-    for i in range(0, len(sources)):
-        if sources[i] is None:
-            sources[i] = itertools.repeat(None)
-
-    # Standardize extensions
-    if source_extensions is not None:
-        source_extensions = set([
-            '.' + ext if '.' not in ext else ext
-            for ext in source_extensions])
-    else:
-        source_extensions = []
-    sink_extension = (
-        '.' + sink_extension if '.' not in sink_extension
-        else sink_extension)
-
-    lengths = set()
-    for source_list in sources:
-        lengths.add(len(source_list))
-
-    assert len(lengths) == 1, 'all source lists must have the same lengths'
-
-    if sinks is not None:
-        assert len(sinks) == len(sources[0]), 'sinks must have the same length as the source lists'
-
-    if sinks is None:
-
-        # Get sources as a list of files
-        source_files = [[] for _ in sources]
-        for source_tuple in zip(*sources):
-            source_paths = [Path(source) for source in source_tuple]
-            source_is_dir = list(set([source.is_dir() for source in source_paths]))
-            if len(source_is_dir) > 1 and True in source_is_dir:
-                raise ValueError('cannot handle directories when more than one input list is given')
-            elif len(source_is_dir) == 1 and source_is_dir[0]:
-                for extension in source_extensions:
-                    source_files[0] += list(source_paths[0].rglob(f'*{extension}'))
-            else:
-                for i, source in enumerate(source_paths):
-                    source_files[i].append(source)
-
-        # Sink files are source files with sink extension
-        source_files = sum(source_files, [])
-        sink_files = [
-            file.with_suffix(sink_extension) for file in source_files]
-
-    else:
-
-        # Get sources and sinks as file lists
-        source_files, sink_files = [[] for _ in sources], []
-        for source_tuple, sink in zip(zip(*sources), sinks):
-            source_paths = [Path(source) for source in source_tuple]
-            source_is_dir = list(set([source.is_dir() for source in source_paths]))
-            sink = Path(sink)
-
-            if len(source_is_dir) > 1 and True in source_is_dir:
-                raise ValueError('cannot handle directories when more than one input list is given')
-
-            # Handle input directory (only if one source list)
-            if True in source_is_dir:
-                if not sink.is_dir():
-                    raise RuntimeError(
-                        f'For input tuple {source_tuple}, corresponding '
-                        f'output {sink} is not a directory')
-                for extension in source_extensions:
-                    source_files[0] += list(source_tuple[0].rglob(f'*{extension}'))
-
-                # Ensure one-to-one
-                source_stems = [file.stem for file in source_files[0]]
-                if not len(source_stems) == len(set(source_stems)):
-                    raise ValueError(
-                        'Two or more files have the same '
-                        'stem with different extensions')
-
-                # Get corresponding output files
-                sink_files += [
-                    sink / (file.stem + sink_extension)
-                    for file in source_files]
-
-            # Handle input file(s)
-            else:
-                if sink.is_dir():
-                    raise RuntimeError(
-                        f'For input file {source}, corresponding '
-                        f'output {sink} is a directory')
-                for i, source in enumerate(source_tuple):
-                    source_files[i].append(source)
-                sink_files.append(sink)
-
-    # if len(source_files) == 1:
-    #     source_files = source_files[0]
-
-    return source_files, sink_files
-
-
-def infer(features, lengths, representation='mel', checkpoint=None, softmax=True):
+def infer(
+    features,
+    lengths,
+    representation='mel',
+    checkpoint=None,
+    softmax=True):
     """Perform model inference"""
 
     # Skip inference if we want input representations
     if ppgs.REPRESENTATION_KIND == 'latents':
         return features
 
     # Maybe cache model
@@ -716,15 +564,17 @@
         not hasattr(infer, 'model') or
         infer.checkpoint != checkpoint or
         infer.device_type != features.device.type or
         infer.representation != representation
     ):
         model_key = str(representation) + str(checkpoint)
         if model_key not in infer.models:
-            infer.models[model_key] = ppgs.load.model(checkpoint=checkpoint, representation=representation)
+            infer.models[model_key] = ppgs.load.model(
+                checkpoint=checkpoint,
+                representation=representation)
         infer.model = infer.models[model_key]
         infer.checkpoint = checkpoint
         infer.representation = representation
         infer.device_type = features.device.type
 
     # Move model to correct device (no-op if devices are the same)
     infer.model = infer.model.to(features.device)
@@ -749,14 +599,17 @@
         return audio
     resampler = torchaudio.transforms.Resample(sample_rate, target_rate)
     resampler = resampler.to(audio.device)
     return resampler(audio)
 
 
 def representation_file_extension():
-    if ppgs.REPRESENTATION == ppgs.BEST_REPRESENTATION and ppgs.REPRESENTATION_KIND == 'ppg':
+    if (
+        ppgs.REPRESENTATION == ppgs.BEST_REPRESENTATION and
+        ppgs.REPRESENTATION_KIND == 'ppg'
+    ):
         return '-ppg.pt'
     else:
         if ppgs.REPRESENTATION_KIND == 'ppg':
             return f'-{ppgs.REPRESENTATION}-ppg.pt'
         else:
             return f'-{ppgs.REPRESENTATION}.pt'
```

### Comparing `ppgs-0.0.3/ppgs/data/collate.py` & `ppgs-0.0.4/ppgs/data/collate.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,18 @@
                 for i, audio in enumerate(values):
                     padded_audio[i, 0, :audio.shape[-1]] = audio[0]
                 batch_values.append(padded_audio)
 
             # Pack target phonemes
             elif feature == 'phonemes':
                 max_length = max([indices.shape[-1] for indices in values])
-                padded_indices = torch.full((batch_size, max_length), -100, dtype=torch.long)
+                padded_indices = torch.full(
+                    (batch_size, max_length),
+                    -100,
+                    dtype=torch.long)
                 for i, indices in enumerate(values):
                     padded_indices[i, :indices.shape[-1]] = indices
                 batch_values.append(padded_indices)
 
             # Pack stem
             elif feature == 'stem':
                 batch_values.append(values)
```

### Comparing `ppgs-0.0.3/ppgs/data/dataset.py` & `ppgs-0.0.4/ppgs/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,17 @@
             self.cache = None
 
         if not lengths:
 
             # Compute length in frames
             for stem, audio_file in zip(self.stems, self.audio_files):
                 info = torchaudio.info(audio_file)
-                length = int(info.num_frames * (ppgs.SAMPLE_RATE / info.sample_rate)) // ppgs.HOPSIZE
+                length = int(
+                    info.num_frames * (ppgs.SAMPLE_RATE / info.sample_rate)
+                ) // ppgs.HOPSIZE
 
                 # Omit if length is too long to avoid OOM
                 if length <= max_frames:
                     lengths[stem] = length
                 else:
                     warnings.warn(
                         f'File {audio_file} of length {length} '
```

### Comparing `ppgs-0.0.3/ppgs/data/datasets/arctic/core.py` & `ppgs-0.0.4/ppgs/data/datasets/arctic/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/datasets/arctic/words/align.py` & `ppgs-0.0.4/ppgs/data/datasets/arctic/words/align.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/datasets/arctic/words/core.py` & `ppgs-0.0.4/ppgs/data/datasets/arctic/words/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/datasets/commonvoice/core.py` & `ppgs-0.0.4/ppgs/data/datasets/commonvoice/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/datasets/timit/core.py` & `ppgs-0.0.4/ppgs/data/datasets/timit/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/download/__main__.py` & `ppgs-0.0.4/ppgs/data/download/__main__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/download/align/core.py` & `ppgs-0.0.4/ppgs/data/download/align/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import csv
 
 import pypar
 import numpy as np
 
-import ppgs
-
 
 ###############################################################################
 # Merge phoneme and word alignments
 ###############################################################################
 
 
 def from_sequence_data(phone_timings_seq, word_timings_seq):
```

### Comparing `ppgs-0.0.3/ppgs/data/download/core.py` & `ppgs-0.0.4/ppgs/data/download/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import tempfile
 import zipfile
 from pathlib import Path
 
-import gdown
 import torchutil
 
 import ppgs
 
 
 ###############################################################################
 # Download datasets
@@ -44,14 +43,15 @@
     """Create case insensitive glob fragment"""
     characters = list(fragment.lower())
     return ''.join([f'[{c}{c.upper()}]' for c in characters])
 
 
 def download_google_drive_zip(url, path, skip_first=True):
     """Download a zip file from google drive, extract contents to path"""
+    import gdown
     f = tempfile.NamedTemporaryFile(mode='r+b', suffix='.zip', delete=False)
     f.close()
     gdown.download(url, f.name)
     with zipfile.ZipFile(f.name) as zf:
         for zipinfo in torchutil.iterator(
             zf.infolist()[1 if skip_first else 0:],
             'Extracting zip contents',
```

### Comparing `ppgs-0.0.3/ppgs/data/loader.py` & `ppgs-0.0.4/ppgs/data/loader.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/data/sampler.py` & `ppgs-0.0.4/ppgs/data/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 
 import ppgs
 
+
 ###############################################################################
 # Sampler selection
 ###############################################################################
 
 
 def sampler(dataset, partition):
     """Create batch sampler"""
```

### Comparing `ppgs-0.0.3/ppgs/data/stats/core.py` & `ppgs-0.0.4/ppgs/data/stats/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/edit/core.py` & `ppgs-0.0.4/ppgs/edit/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,54 @@
 
     # Update target probabilities
     ppg[target_index] += reallocation_probability
 
     return ppg
 
 
+def regex_find(
+    ppg: torch.Tensor,
+    find_phonemes: List[str],
+) -> torch.Tensor:
+    """Regex match and replace (via swap) for phoneme sequences
+
+    Arguments
+        ppg
+            Input PPG
+            shape=(len(ppgs.PHONEMES), frames)
+        find_phonemes
+            Source phoneme sequence
+
+    Returns
+        sequence of indices
+    """
+    source_indices = [ppgs.PHONEMES.index(phone) for phone in find_phonemes]
+
+    # Decode to phoneme indices using argmax
+    indices = ppg.argmax(dim=0)
+    unique_indices, inverse = torch.unique_consecutive(
+        indices,
+        return_inverse=True)
+
+    # Regex search for source matches
+    pattern = re.escape(
+        struct.pack('b' * len(source_indices),
+        *source_indices))
+    string = struct.pack('b' * len(unique_indices), *unique_indices)
+    match_spans = torch.tensor(
+        [match.span() for match in re.finditer(pattern, string)])
+
+    return [
+        [
+            torch.argwhere(inverse == start)[0],
+            torch.argwhere(inverse == end-1)[-1] + 1
+        ]
+    for start, end in match_spans]
+
+
 def regex(
     ppg: torch.Tensor,
     source_phonemes: List[str],
     target_phonemes: List[str],
     reallocate=False
 ) -> torch.Tensor:
     """Regex match and replace (via swap) for phoneme sequences
@@ -100,15 +140,16 @@
         slicing = torch.isin(inverse, match_indices + i)
         if reallocate:
             reallocation_probability = ppg[source_indices[i], slicing].clone()
             ppg[source_indices[i], slicing] = 0.
             ppg[target_indices[i], slicing] += reallocation_probability
         else:
             temporary = ppg[target_indices[i], slicing].clone()
-            ppg[target_indices[i], slicing] = ppg[source_indices[i], slicing].clone()
+            ppg[target_indices[i], slicing] = \
+                ppg[source_indices[i], slicing].clone()
             ppg[source_indices[i], slicing] = temporary
 
     return ppg
 
 
 def shift(ppg: torch.Tensor, phoneme: str, value: float):
     """Shift probability of a phoneme and reallocate proportionally
```

### Comparing `ppgs-0.0.3/ppgs/edit/grid.py` & `ppgs-0.0.4/ppgs/edit/grid.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/evaluate/__main__.py` & `ppgs-0.0.4/ppgs/evaluate/__main__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/evaluate/core.py` & `ppgs-0.0.4/ppgs/evaluate/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 @torchutil.notify('evaluate')
 def datasets(datasets, gpu=None, checkpoint=None):
     """Perform evaluation"""
     device = torch.device('cpu' if gpu is None else f'cuda:{gpu}')
 
     # Get model checkpoint
     if checkpoint is None:
-        checkpoint = torchutil.checkpoint.latest_path(ppgs.RUNS_DIR / ppgs.CONFIG)
+        checkpoint = torchutil.checkpoint.latest_path(
+            ppgs.RUNS_DIR / ppgs.CONFIG)
 
     # Containers for results
     results = {}
 
     # Per-dataset metrics
     dataset_metrics = ppgs.evaluate.Metrics()
```

### Comparing `ppgs-0.0.3/ppgs/evaluate/metrics.py` & `ppgs-0.0.4/ppgs/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/evaluate/visualize.py` & `ppgs-0.0.4/ppgs/evaluate/visualize.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/load.py` & `ppgs-0.0.4/ppgs/load.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,68 +9,70 @@
 import ppgs
 
 
 ###############################################################################
 # Loading utilities
 ###############################################################################
 
-def ppg_from_stem(stem: str):
-    """Given a stem, loads the corresponding PPG"""
-
-    if not hasattr(ppg_from_stem, 'extension'):
-        ppg_from_stem.extension = ppgs.representation_file_extension()
-
-    path = Path(str(stem) + ppg_from_stem.extension)
-
-    return torch.load(path)
-
 
 def audio(file):
     """Load audio from disk"""
     path = Path(file)
     if path.suffix.lower() == '.mp3':
         try:
             audio, sample_rate = torchaudio.load(path, format='mp3')
         except RuntimeError:
-            raise RuntimeError("Failed to load mp3 file, make sure ffmpeg<=4.3 is installed")
+            raise RuntimeError(
+                'Failed to load mp3 file, make sure ffmpeg<=4.3 is installed')
     else:
         audio, sample_rate = torchaudio.load(file)
 
     # Maybe resample
     return ppgs.resample(audio, sample_rate)
 
+
 def model(checkpoint=None, representation=None):
     """Load a model"""
-    breakpoint()
     if representation is not None:
         if representation == 'w2v2fb':
             checkpoint = huggingface_hub.hf_hub_download(
                 'CameronChurchwell/ppgs',
                 'w2v2fb-425k.pt')
             conf = vars(ppgs.config.w2v2fb)
             conf = {k: v for k, v in conf.items() if not k.startswith('__')}
             kwargs = {kv[0].lower() : kv[1] for kv in conf.items()}
         elif representation == 'mel':
-            pass # nothing to do
+            kwargs = {}
         else:
-            raise ValueError("supplying representation directly only supported for w2v2fb and mel")
+            raise ValueError(
+                'Supplying representation directly only supported '
+                'for w2v2fb and mel')
     else:
         kwargs = {}
 
     model = ppgs.Model(**kwargs)
 
     # Pretrained model
     if ppgs.MODEL in ['W2V2FC', 'W2V2FS']:
         return model
 
     # Maybe download from HuggingFace
     if checkpoint is None and ppgs.LOCAL_CHECKPOINT is None:
-        checkpoint = huggingface_hub.hf_hub_download(
-            'CameronChurchwell/ppgs',
-            'mel-800k.pt')
+        if ppgs.REPRESENTATION == 'mel' or ppgs.REPRESENTATION is None:
+            checkpoint = huggingface_hub.hf_hub_download(
+                'CameronChurchwell/ppgs',
+                'mel-800k.pt')
+        elif ppgs.REPRESENTATION == 'w2v2fb':
+            checkpoint = huggingface_hub.hf_hub_download(
+                'CameronChurchwell/ppgs',
+                'w2v2fb-425k.pt')
+        else:
+            raise ValueError(
+                f'No default checkpoints exist for '
+                f'representation {ppgs.REPRESENTATION}')
     elif checkpoint is None and ppgs.LOCAL_CHECKPOINT is not None:
         checkpoint = ppgs.LOCAL_CHECKPOINT
 
     # Load from checkpoint
     state_dict = torch.load(checkpoint, map_location='cpu')
     if 'model' in state_dict:
         state_dict = state_dict['model']
```

### Comparing `ppgs-0.0.3/ppgs/model/convolution.py` & `ppgs-0.0.4/ppgs/model/convolution.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/model/core.py` & `ppgs-0.0.4/ppgs/model/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,14 @@
         init_fn = ppgs.model.Convolution
     elif ppgs.MODEL == 'transformer':
         init_fn = ppgs.model.Transformer
     elif ppgs.MODEL == 'Wav2Vec2.0':
         init_fn = ppgs.model.W2V2
     elif ppgs.MODEL == 'W2V2FC':
         init_fn = ppgs.model.W2V2FC
-    elif ppgs.MODEL == 'mamba':
-        init_fn = ppgs.model.Mamba
     else:
         raise ValueError(f'Model {ppgs.MODEL} is not defined')
 
     sig = inspect.signature(init_fn)
     valid_keys = set(sig.parameters.keys())
     kwargs = {k: v for k, v in kwargs.items() if k in valid_keys}
-    return init_fn(**kwargs)
+    return init_fn(**kwargs)
```

### Comparing `ppgs-0.0.3/ppgs/model/transformer.py` & `ppgs-0.0.4/ppgs/model/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     def __init__(
         self,
         num_hidden_layers=ppgs.NUM_HIDDEN_LAYERS,
         hidden_channels=ppgs.HIDDEN_CHANNELS,
         input_channels=ppgs.INPUT_CHANNELS,
         output_channels=ppgs.OUTPUT_CHANNELS,
         kernel_size=ppgs.KERNEL_SIZE,
-        attention_heads=ppgs.ATTENTION_HEADS
+        attention_heads=ppgs.ATTENTION_HEADS,
+        is_causal=ppgs.IS_CAUSAL
     ):
         super().__init__()
         self.position = PositionalEncoding(hidden_channels)
         self.input_layer = torch.nn.Conv1d(
             input_channels,
             hidden_channels,
             kernel_size=kernel_size,
@@ -32,20 +33,29 @@
             torch.nn.TransformerEncoderLayer(hidden_channels, attention_heads),
             num_hidden_layers)
         self.output_layer = torch.nn.Conv1d(
             hidden_channels,
             output_channels,
             kernel_size=kernel_size,
             padding='same')
+        self.is_causal = is_causal
 
     def forward(self, x, lengths):
+        if self.is_causal:
+            causal_mask = torch.nn.Transformer.generate_square_subsequent_mask(
+                torch.max(lengths),
+                device = x.device
+            )
+        else:
+            causal_mask = None
         mask = mask_from_lengths(lengths).unsqueeze(1)
         x = self.input_layer(x) * mask
         x = self.model(
             self.position(x.permute(2, 0, 1)),
+            mask=causal_mask,
             src_key_padding_mask=~mask.squeeze(1)
         ).permute(1, 2, 0)
         return self.output_layer(x) * mask
 
 
 ###############################################################################
 # Utilities
```

### Comparing `ppgs-0.0.3/ppgs/model/w2v2.py` & `ppgs-0.0.4/ppgs/model/w2v2.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/model/w2v2fc.py` & `ppgs-0.0.4/ppgs/model/w2v2fc.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/partition/__main__.py` & `ppgs-0.0.4/ppgs/partition/__main__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/partition/core.py` & `ppgs-0.0.4/ppgs/partition/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/phonemes.py` & `ppgs-0.0.4/ppgs/phonemes.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/plot/__main__.py` & `ppgs-0.0.4/ppgs/plot/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,63 +10,42 @@
 
 
 def parse_args():
     """Parse command-line arguments"""
     parser = yapecs.ArgumentParser(
         description='Phonetic posteriorgram plotting')
     parser.add_argument(
-        '--audio_paths',
+        '--audio_files',
         nargs='+',
         type=Path,
-        required=False,
-        help='Paths to audio files and/or directories')
+        help='Audio filenames')
     parser.add_argument(
-        '--audio_extensions',
-        nargs='+',
-        default=['wav', 'mp3'],
-        help='Extensions for audio files in provided directories'
-    )
-    parser.add_argument(
-        '--ppg_paths',
+        '--ppg_files',
         nargs='+',
         type=Path,
-        required=False,
-        help='Paths to PPG files and/or directories')
+        help='PPG filenames')
     parser.add_argument(
-        '--textgrid_paths',
+        '--textgrid_files',
         nargs='+',
         type=Path,
-        required=False,
-        help='Paths to textgrid files and/or directories')
+        help='TextGrid files containing lexical alignments')
     parser.add_argument(
-        '--output_paths',
+        '--output_files',
         type=Path,
         nargs='+',
-        default=None,
-        help='The one-to-one corresponding output paths')
-    parser.add_argument(
-        '--video',
-        action='store_true',
-        help='Create video visualizations instead of images'
-    )
-    parser.add_argument(
-        '--pdf',
-        action='store_true',
-        help='Save resulting images as pdf files'
-    )
+        help='The one-to-one corresponding output files')
     parser.add_argument(
         '--checkpoint',
-        default=None,
+        type=Path,
         help='The checkpoint file')
     parser.add_argument(
         '--font_filename',
-        default=None,
-        help='The font file to use for text'
-    )
+        type=Path,
+        help='The font file to use for text')
     parser.add_argument(
         '--gpu',
         type=int,
         help='The index of the GPU to use for inference. Defaults to CPU.')
     return parser.parse_args()
 
 
-ppgs.plot.from_paths_to_paths(**vars(parse_args()))
+ppgs.plot.from_files_to_files(**vars(parse_args()))
```

### Comparing `ppgs-0.0.3/ppgs/plot/accuracy/__main__.py` & `ppgs-0.0.4/ppgs/plot/accuracy/__main__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/plot/accuracy/core.py` & `ppgs-0.0.4/ppgs/plot/accuracy/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/plot/core.py` & `ppgs-0.0.4/ppgs/plot/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,178 +11,96 @@
 import torchutil
 from moviepy import editor as mpy
 from PIL import Image, ImageDraw, ImageFont
 from itertools import repeat
 
 import ppgs
 
-def from_paths_to_paths(
-    audio_paths: List[Union[str, bytes, os.PathLike]] = None,
-    ppg_paths: List[Union[str, bytes, os.PathLike]] = None,
-    textgrid_paths: List[Union[str, bytes, os.PathLike]] = None,
-    output_paths: Optional[List[Union[str, bytes, os.PathLike]]] = None,
-    audio_extensions: Optional[List[str]] = None,
-    checkpoint: Union[str, bytes, os.PathLike] = None,
-    video: bool = False,
-    font_filename: Union[str, bytes, os.PathLike] = None,
-    pdf: bool = False,
-    gpu: Optional[int] = None) -> None:
-    """Infer ppgs from audio files and save to torch tensor files
-
-    Arguments
-        input_paths
-            Paths to audio files and/or directories
-        output_paths
-            The one-to-one corresponding outputs
-        extensions
-            Extensions to glob for in directories
-        checkpoint
-            The checkpoint file
-        num_workers
-            Number of CPU threads for multiprocessing
-        gpu
-            The index of the GPU to use for inference
-    """
-
-    if video:
-        output_extension = 'mp4'
-    elif pdf:
-        output_extension = 'pdf'
-    else:
-        output_extension = 'jpg'
-
-    if audio_paths is not None and ppg_paths is not None:
-        if textgrid_paths is None:
-            (audio_files, ppg_files), output_files = ppgs.aggregate(
-                audio_paths,
-                ppg_paths,
-                sinks=output_paths,
-                sink_extension=output_extension
-            )
-            textgrid_files = None
-        else:
-            (audio_files, ppg_files, textgrid_files), output_files = ppgs.aggregate(
-                audio_paths,
-                ppg_paths,
-                textgrid_paths,
-                sinks=output_paths,
-                sink_extension=output_extension
-            )
-    elif audio_paths is not None and ppg_paths is None:
-        if textgrid_paths is None:
-            audio_files, output_files = ppgs.aggregate(
-                audio_paths,
-                sinks=output_paths,
-                source_extensions=audio_extensions,
-                sink_extension=output_extension
-            )
-            textgrid_files = None
-        else:
-            (audio_files, textgrid_files), output_files = ppgs.aggregate(
-                audio_paths,
-                textgrid_paths,
-                sinks=output_paths,
-                sink_extension=output_extension
-            )
-        ppg_files = None
-    elif audio_paths is None and ppg_paths is not None:
-        if textgrid_paths is None:
-            ppg_files, output_files = ppgs.aggregate(
-                ppg_paths,
-                sinks=output_paths,
-                source_extensions=['pt'],
-                sink_extension=output_extension
-            )
-            textgrid_files = None
-        else:
-            (ppg_files, textgrid_files), output_files = ppgs.aggregate(
-                ppg_paths,
-                textgrid_paths,
-                sinks=output_paths,
-                sink_extension=output_extension
-            )
-        audio_files = None
-    else:
-        raise ValueError('must provide audio_paths, OR ppg_paths, OR both')
 
-    from_files_to_files(
-        audio_files=audio_files,
-        ppg_files=ppg_files,
-        textgrid_files=textgrid_files,
-        output_files=output_files,
-        font_filename=font_filename,
-        checkpoint=checkpoint,
-        gpu=gpu)
+###############################################################################
+# Plot phonetic posteriorgrams
+###############################################################################
 
 
 def from_files_to_files(
     audio_files: List[Union[str, bytes, os.PathLike]],
     ppg_files: List[Union[str, bytes, os.PathLike]],
     textgrid_files: List[Union[str, bytes, os.PathLike]],
     output_files: List[Union[str, bytes, os.PathLike]],
     font_filename: Union[str, bytes, os.PathLike] = None,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None) -> None:
-    """Infer ppgs from audio files and save to torch tensor files
+    """Plot ppgs and save to disk
 
     Arguments
         audio_files
             The audio files
+        ppg_files
+            The PyTorch files containing PPGs
+        textgrid_files
+            The files containing the forced alignment
         output_files
-            The .pt files to save PPGs
+            The corresponding files to save the plots
+        font_filename
+            The file path containing font information
         checkpoint
             The checkpoint file
-        num_workers
-            Number of CPU threads for multiprocessing
         gpu
             The index of the GPU to use for inference
     """
     assert output_files is not None
     assert audio_files is not None or ppg_files is not None
 
     if textgrid_files is None:
         textgrid_files = repeat(None)
 
     if ppg_files is not None:
         if audio_files is None:
             audio_files = repeat(None)
-        for audio_file, ppg_file, textgrid_file, output_file in zip(audio_files, ppg_files, textgrid_files, output_files):
+        for audio_file, ppg_file, textgrid_file, output_file in zip(
+            audio_files,
+            ppg_files,
+            textgrid_files,
+            output_files
+        ):
             output_ext = str(output_file).split('.')[-1]
             if output_ext == 'mp4':
                 mode = 'video'
             elif output_ext in ['jpg', 'png', 'pdf']:
                 mode = 'image'
             else:
                 raise ValueError(f'Unknown extension {output_ext}')
             from_ppg_file_to_file(
                 ppg_filename=ppg_file,
                 audio_filename=audio_file,
                 textgrid_filename=textgrid_file,
                 output_filename=output_file,
                 font_filename=font_filename,
-                mode=mode
-            )
+                mode=mode)
     else:
-        for audio_file, textgrid_file, output_file in zip(audio_files, textgrid_files, output_files):
+        for audio_file, textgrid_file, output_file in zip(
+            audio_files,
+            textgrid_files,
+            output_files
+        ):
             output_ext = str(output_file).split('.')[-1]
             if output_ext == 'mp4':
                 mode = 'video'
             elif output_ext in ['jpg', 'png', 'pdf']:
                 mode = 'image'
             else:
                 raise ValueError(f'Unknown extension {output_ext}')
             from_audio_file_to_file(
                 audio_filename=audio_file,
                 output_filename=output_file,
                 textgrid_filename=textgrid_file,
                 checkpoint=checkpoint,
                 gpu=gpu,
                 font_filename=font_filename,
-                mode=mode
-            )
+                mode=mode)
 
 
 ###############################################################################
 # Constants
 ###############################################################################
 
 
@@ -333,15 +251,17 @@
     textgrid_filename=None,
     preprocess_only=False,
     labels=ppgs.PHONEMES,
     scalefactor=16):
     """Takes ppg of shape time,categories and creates a visualization"""
     # Load audio
     if audio_filename is not None:
-        audio_clip = mpy.AudioFileClip(str(audio_filename), fps=ppgs.SAMPLE_RATE)
+        audio_clip = mpy.AudioFileClip(
+            str(audio_filename),
+            fps=ppgs.SAMPLE_RATE)
 
     num_frames = ppg.T.shape[-1]
 
     ppg_pixels = from_ppg_to_pixels(ppg)
     textgrid_pixels = from_textgrid_to_pixels(
         textgrid_filename,
         num_frames)
@@ -543,14 +463,17 @@
 
     #clear all but red channels
     combined[..., 1:] = 0
     if blue is not None:
         combined[..., 2] = blue[..., 2]
     if green is not None:
         combined[..., 1] = green[..., 1]
+    if blue is None and green is None:
+        combined[..., 1] = combined[..., 0]
+        combined[..., 2] = combined[..., 0]
 
     return combined
 
 
 def from_textgrid_to_pixels(
     textgrid_filename,
     num_frames,
```

### Comparing `ppgs-0.0.3/ppgs/preprocess/__init__.py` & `ppgs-0.0.4/ppgs/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/__main__.py` & `ppgs-0.0.4/ppgs/preprocess/__main__.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/build_ppg_model.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/build_ppg_model.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/e2e_asr_common.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/attention.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/attention.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/conformer_encoder.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/convolution.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/convolution.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/embedding.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/embedding.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder_layer.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/layer_norm.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/layer_norm.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/multi_layer_conv.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/positionwise_feed_forward.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/repeat.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/repeat.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/subsampling.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/subsampling.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/vgg.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoder/vgg.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/encoders.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/encoders.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/frontend.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/frontend.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/log_mel.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/log_mel.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/nets_utils.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/nets_utils.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/stft.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/stft.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/conformer_ppg_model/utterance_mvn.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/conformer_ppg_model/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/bottleneck/core.py` & `ppgs-0.0.4/ppgs/preprocess/bottleneck/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/core.py` & `ppgs-0.0.4/ppgs/preprocess/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,20 @@
 
         # Shutdown multiprocessing
         if num_workers > 0:
             pool.close()
             pool.join()
 
 
-def from_audio(audio, representation=ppgs.REPRESENTATION, sample_rate=ppgs.SAMPLE_RATE, gpu=None):
+def from_audio(
+    audio,
+    representation=ppgs.REPRESENTATION,
+    sample_rate=ppgs.SAMPLE_RATE,
+    gpu=None
+):
     """Preprocess audio"""
     audio = ppgs.resample(audio, sample_rate)
 
     if representation is None:
         representation = ppgs.REPRESENTATION
 
     # Compute representation
```

### Comparing `ppgs-0.0.3/ppgs/preprocess/dac.py` & `ppgs-0.0.4/ppgs/preprocess/dac.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import torch
-import torchaudio
 
 import ppgs
 
 # Window size of the model
 WINDOW_SIZE = 400
 HOP_SIZE = 320
 
 ###############################################################################
 # Preprocess EnCodec input representation
 ###############################################################################
 
+
 def from_audios(audio, lengths, sample_rate=ppgs.SAMPLE_RATE, gpu=None):
     device = torch.device(f'cuda:{gpu}' if gpu is not None else 'cpu')
     expected_length = audio.shape[-1] // ppgs.HOPSIZE
 
     # Cache model
     if not hasattr(from_audios, 'model'):
         import dac
@@ -24,21 +24,14 @@
 
     with torch.autocast(device.type):
 
         audio = audio.to(device)
 
         # Encode
         model_input = from_audios.model.preprocess(audio, sample_rate)
-        
-        # Maybe resample
-        # audio = ppgs.resample(audio, sample_rate)
-
-        # pad = WINDOW_SIZE // 2 - HOP_SIZE // 2
-        # pad=0
-        # padded_audio = torch.nn.functional.pad(audio, (pad, pad))
         z, codes, latents, _, _ = from_audios.model.encode(model_input)
 
         # Upsample
         return torch.nn.functional.interpolate(
             codes.to(torch.float),
             size=expected_length,
             mode='nearest'
```

### Comparing `ppgs-0.0.3/ppgs/preprocess/encodec.py` & `ppgs-0.0.4/ppgs/preprocess/encodec.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import ppgs
 
 
 ###############################################################################
 # Preprocess EnCodec input representation
 ###############################################################################
 
+
 def from_audios(audio, lengths, sample_rate=ppgs.SAMPLE_RATE, gpu=None):
     device = torch.device(f'cuda:{gpu}' if gpu is not None else 'cpu')
     expected_length = audio.shape[-1] // ppgs.HOPSIZE
     # Cache resampler
     if (
         not hasattr(from_audios, 'resampler') or
         sample_rate != from_audios.sample_rate
```

### Comparing `ppgs-0.0.3/ppgs/preprocess/mel.py` & `ppgs-0.0.4/ppgs/preprocess/mel.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/spectrogram.py` & `ppgs-0.0.4/ppgs/preprocess/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/preprocess/w2v2fb/core.py` & `ppgs-0.0.4/ppgs/preprocess/w2v2fb/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,17 @@
                 config).to(device)
             from_audios.device = device
 
         # Maybe resample
         audio = ppgs.resample(audio, sample_rate, SAMPLE_RATE).to(device)
 
         # Pad
-        lengths = torch.ceil(lengths * (SAMPLE_RATE / sample_rate)).to(torch.long)
+        lengths = torch.ceil(
+            lengths * (SAMPLE_RATE / sample_rate)
+        ).to(torch.long)
         pad = WINDOW_SIZE // 2 - HOP_SIZE // 2
         padded_audio = torch.nn.functional.pad(
             audio,
             (pad, pad)
         ).squeeze(dim=1)
 
         # Infer W2V2FB latents
```

### Comparing `ppgs-0.0.3/ppgs/preprocess/w2v2fc/core.py` & `ppgs-0.0.4/ppgs/preprocess/w2v2fc/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
         if not hasattr(from_audio, 'model'):
             from_audio.model = transformers.Wav2Vec2Model.from_pretrained(
                 config).to(device)
 
         # Maybe resample
         audio = ppgs.resample(audio, sample_rate, SAMPLE_RATE).to(device)
         pad = WINDOW_SIZE // 2 - ppgs.HOPSIZE // 2
-        padded_audio = torch.nn.functional.pad(audio, (pad, pad)).squeeze(dim=1)
+        padded_audio = torch.nn.functional.pad(
+            audio,
+            (pad, pad)
+        ).squeeze(dim=1)
 
         # Infer W2V2FC latents
         mask = ppgs.model.transformer.mask_from_lengths(
             lengths
         ).squeeze(dim=1).to(torch.long).to(audio.device)
         output = from_audio.model(padded_audio, mask).last_hidden_state
         output = torch.transpose(output, 1, 2)
```

### Comparing `ppgs-0.0.3/ppgs/preprocess/w2v2ft/core.py` & `ppgs-0.0.4/ppgs/preprocess/w2v2ft/core.py`

 * *Files identical despite different names*

### Comparing `ppgs-0.0.3/ppgs/train/__main__.py` & `ppgs-0.0.4/ppgs/train/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # Training CLI
 ###############################################################################
 
 
 def main(config, dataset, gpu=None):
     """Train from configuration"""
     # Create output directory
-    directory = ppgs.RUNS_DIR / config.stem
+    directory = ppgs.RUNS_DIR / ppgs.CONFIG
     directory.mkdir(parents=True, exist_ok=True)
 
     # Save configuration
-    shutil.copyfile(config, directory / config.name)
+    if config is not None:
+        shutil.copyfile(config, directory / config.name)
 
     # Train
     ppgs.train(dataset, directory, gpu)
 
 
 def parse_args():
     """Parse command-line arguments"""
```

### Comparing `ppgs-0.0.3/ppgs/train/core.py` & `ppgs-0.0.4/ppgs/train/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import functools
 import math
 
 # import accelerate
 import matplotlib
-import numpy as np
 import torch
 import torchutil
 
 import ppgs
 
 
 ###############################################################################
@@ -154,15 +153,15 @@
                     # Unscale gradients
                     scaler.unscale_(optimizer)
 
                     if ppgs.GRADIENT_CLIP_THRESHOLD_L2 is not None:
 
                         # Compare gradient norm to threshold
                         grad_norm = gradient_statistics['gradients/norm']
-                        if grad_norm > promonet.GRADIENT_CLIP_THRESHOLD_L2:
+                        if grad_norm > ppgs.GRADIENT_CLIP_THRESHOLD_L2:
 
                             # Clip
                             # accelerator.clip_grad_norm_(
                             #     model.parameters(),
                             #     ppgs.GRADIENT_CLIPPING_THRESHOLD,
                             #     norm_type=2.0)
                             torch.nn.utils.clip_grad_norm_(
@@ -172,15 +171,15 @@
 
                     if ppgs.GRADIENT_CLIP_THRESHOLD_INF is not None:
 
                         # Compare maximum gradient to threshold
                         max_grad = max(
                             gradient_statistics['gradients/max'],
                             math.abs(gradient_statistics['gradients/min']))
-                        if max_grad > promonet.GRADIENT_CLIP_THRESHOLD_INF:
+                        if max_grad > ppgs.GRADIENT_CLIP_THRESHOLD_INF:
 
                             # Clip
                             # accelerator.clip_grad_norm_(
                             #     model.parameters(),
                             #     ppgs.GRADIENT_CLIPPING_THRESHOLD,
                             #     norm_type='inf')
                             torch.nn.utils.clip_grad_norm_(
@@ -199,15 +198,15 @@
                 # Evaluate #
                 ############
 
                 if step % ppgs.EVALUATION_INTERVAL == 0:
 
                     # Log VRAM utilization
                     # index = accelerator.device.index
-                    print(torch.cuda.memory_summary(device.index))
+                    # print(torch.cuda.memory_summary(device.index))
                     torchutil.tensorboard.update(
                         directory,
                         step,
                         scalars=torchutil.cuda.utilization(device, 'MB'))
 
                     # Clear cache to make space for evaluation tensors
                     del train_loss
```

### Comparing `ppgs-0.0.3/ppgs.egg-info/PKG-INFO` & `ppgs-0.0.4/ppgs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: ppgs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Phonetic posteriorgrams
 Home-page: https://github.com/interactiveaudiolab/ppgs
 Author: Interactive Audio Lab
 Author-email: interactiveaudiolab@gmail.com
 License: MIT
 Keywords: phonemes,ppg,pronunciation,speech
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: espnet
 Requires-Dist: huggingface-hub
+Requires-Dist: librosa
+Requires-Dist: matplotlib
 Requires-Dist: moviepy
 Requires-Dist: numpy
 Requires-Dist: pypar
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchutil
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: opencv-python
 Requires-Dist: yapecs
-Requires-Dist: gdown>=4.6.2
 Provides-Extra: train
 Requires-Dist: dac; extra == "train"
 Requires-Dist: encodec; extra == "train"
 Requires-Dist: g2pM; extra == "train"
 Requires-Dist: gdown>=4.6.2; extra == "train"
 Requires-Dist: humanfriendly; extra == "train"
-Requires-Dist: librosa; extra == "train"
-Requires-Dist: mamba-ssm; extra == "train"
-Requires-Dist: matplotlib; extra == "train"
 Requires-Dist: nltk; extra == "train"
 Requires-Dist: pyyaml; extra == "train"
 Requires-Dist: torch-complex; extra == "train"
 
 <h1 align="center">High-Fidelity Neural Phonetic Posteriorgrams</h1>
 <div align="center">
 
@@ -54,15 +52,14 @@
 - [Installation](#installation)
 - [Inference](#inference)
     * [Application programming interface (API)](#application-programming-interface-api)
         * [`ppgs.from_audio`](#ppgsfrom_audio)
         * [`ppgs.from_file`](#ppgsfrom_file)
         * [`ppgs.from_file_to_file`](#ppgsfrom_file_to_file)
         * [`ppgs.from_files_to_files`](#ppgsfrom_files_to_files)
-        * [`ppgs.from_paths_to_paths`](#ppgsfrom_paths_to_paths)
     * [Command-line interface (CLI)](#command-line-interface-cli)
 - [Distance](#distance)
 - [Interpolate](#interpolate)
 - [Edit](#edit)
     * [`ppgs.edit.grid.constant`](#ppgseditgridconstant)
     * [`ppgs.edit.grid.from_alignments`](#ppgseditgridfrom_alignments)
     * [`ppgs.edit.grid.of_length`](#ppgseditgridof_length)
@@ -134,25 +131,28 @@
 
 #### `ppgs.from_audio`
 
 ```python
 def from_audio(
     audio: torch.Tensor,
     sample_rate: Union[int, float],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: int = None
 ) -> torch.Tensor:
     """Infer ppgs from audio
 
     Arguments
         audio
             Batched audio to process
             shape=(batch, 1, samples)
         sample_rate
             Audio sampling rate
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
 
     Returns
         ppgs
@@ -163,22 +163,25 @@
 
 
 #### `ppgs.from_file`
 
 ```python
 def from_file(
     file: Union[str, bytes, os.PathLike],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> torch.Tensor:
     """Infer ppgs from an audio file
 
     Arguments
         file
             The audio file
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
 
     Returns
         ppgs
@@ -190,83 +193,56 @@
 
 #### `ppgs.from_file_to_file`
 
 ```python
 def from_file_to_file(
     audio_file: Union[str, bytes, os.PathLike],
     output_file: Union[str, bytes, os.PathLike],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
     gpu: Optional[int] = None
 ) -> None:
     """Infer ppg from an audio file and save to a torch tensor file
 
     Arguments
         audio_file
             The audio file
         output_file
             The .pt file to save PPGs
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         gpu
             The index of the GPU to use for inference
     """
 ```
 
 
 #### `ppgs.from_files_to_files`
 
 ```python
 def from_files_to_files(
     audio_files: List[Union[str, bytes, os.PathLike]],
     output_files: List[Union[str, bytes, os.PathLike]],
+    representation: str = ppgs.REPRESENTATION,
     checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = ppgs.NUM_WORKERS,
+    num_workers: int = 0,
     gpu: Optional[int] = None,
     max_frames: int = ppgs.MAX_INFERENCE_FRAMES
 ) -> None:
     """Infer ppgs from audio files and save to torch tensor files
 
     Arguments
         audio_files
             The audio files
         output_files
             The .pt files to save PPGs
-        checkpoint
-            The checkpoint file
-        num_workers
-            Number of CPU threads for multiprocessing
-        gpu
-            The index of the GPU to use for inference
-        max_frames
-            The maximum number of frames on the GPU at once
-    """
-```
-
-
-#### `ppgs.from_paths_to_paths`
-
-```python
-def from_paths_to_paths(
-    input_paths: List[Union[str, bytes, os.PathLike]],
-    output_paths: Optional[List[Union[str, bytes, os.PathLike]]] = None,
-    extensions: Optional[List[str]] = None,
-    checkpoint: Optional[Union[str, bytes, os.PathLike]] = None,
-    num_workers: int = ppgs.NUM_WORKERS,
-    gpu: Optional[int] = None,
-    max_frames: int = ppgs.MAX_INFERENCE_FRAMES
-) -> None:
-    """Infer ppgs from audio files and save to torch tensor files
-
-    Arguments
-        input_paths
-            Paths to audio files and/or directories
-        output_paths
-            The one-to-one corresponding outputs
-        extensions
-            Extensions to glob for in directories
+        representation
+            The representation to use, 'mel' and 'w2v2fb' are currently supported
         checkpoint
             The checkpoint file
         num_workers
             Number of CPU threads for multiprocessing
         gpu
             The index of the GPU to use for inference
         max_frames
@@ -276,67 +252,72 @@
 
 
 ### Command-line interface (CLI)
 
 ```
 usage: python -m ppgs
     [-h]
-    [--input_paths INPUT_PATHS [INPUT_PATHS ...]]
-    [--output_paths OUTPUT_PATHS [OUTPUT_PATHS ...]]
-    [--extensions EXTENSIONS [EXTENSIONS ...]]
+    [--audio_files AUDIO_FILES [AUDIO_FILES ...]]
+    [--output_files OUTPUT_FILES [OUTPUT_FILES ...]]
+    [--representation REPRESENTATION]
     [--checkpoint CHECKPOINT]
     [--num-workers NUM_WORKERS]
     [--gpu GPU]
     [--max-frames MAX_TRAINING_FRAMES]
 
 arguments:
-    --input_paths INPUT_PATHS [INPUT_PATHS ...]
-        Paths to audio files and/or directories
+    --audio_files AUDIO_FILES [AUDIO_FILES ...]
+        Paths to input audio files
+    --output_files OUTPUT_FILES [OUTPUT_FILES ...]
+        The one-to-one corresponding output files
 
 optional arguments:
     -h, --help
         Show this help message and exit
-    --output_paths OUTPUT_PATHS [OUTPUT_PATHS ...]
-        The one-to-one corresponding output paths
-    --extensions EXTENSIONS [EXTENSIONS ...]
-        Extensions to glob for in directories
+    --representation REPRESENTATION
+        Representation to use for inference
     --checkpoint CHECKPOINT
         The checkpoint file
     --num-workers NUM_WORKERS
         Number of CPU threads for multiprocessing
     --gpu GPU
         The index of the GPU to use for inference. Defaults to CPU.
+    --max-frames MAX_FRAMES
+        Maximum number of frames in a batch
 ```
 
 
 ## Distance
 
 To compute the proposed normalized Jenson-Shannon divergence pronunciation
 distance between two PPGs, use `ppgs.distance()`.
 
 ```python
 def distance(
     ppgX: torch.Tensor,
     ppgY: torch.Tensor,
     reduction: str = 'mean',
-    normalize: bool = True
+    normalize: bool = True,
+    exponent: float = ppgs.SIMILARITY_EXPONENT
 ) -> torch.Tensor:
     """Compute the pronunciation distance between two aligned PPGs
 
     Arguments
         ppgX
             Input PPG X
             shape=(len(ppgs.PHONEMES), frames)
         ppgY
             Input PPG Y to compare with PPG X
             shape=(len(ppgs.PHONEMES), frames)
         reduction
             Reduction to apply to the output. One of ['mean', 'none', 'sum'].
         normalize
             Apply similarity based normalization
+        exponent
+            Similarty exponent
 
     Returns
         Normalized Jenson-shannon divergence between PPGs
     """
 ```
 
 
@@ -557,21 +538,22 @@
             Input phoneme B
 
     Returns
         Edited PPG
     """
 ```
 
+
 ## Sparsify
 
 ```python
 def sparsify(
     ppg: torch.Tensor,
-    method: str='percentile',
-    threshold: Union[float, int]=0.85
+    method: str = 'percentile',
+    threshold: Union[float, int] = 0.85
 ) -> torch.Tensor:
     """Make phonetic posteriorgrams sparse
 
     Arguments
         ppg
             Input PPG
             shape=(*, len(ppgs.PHONEMES), frames)
@@ -605,15 +587,15 @@
 
 ### Preprocess
 
 Prepares representations for training. Representations are stored
 in `data/cache/`.
 
 ```
-python -m ppgs.data.preprocess \
+python -m ppgs.preprocess \
    --datasets <datasets> \
    --representatations <representations> \
    --gpu <gpu> \
    --num-workers <workers>
 ```
 
 
@@ -656,15 +638,19 @@
 
 ### Evaluate
 
 Performs objective evaluation of phoneme accuracy. Results are stored
 in `eval/`.
 
 ```
-python -m ppgs.evaluate --config <name> --datasets <datasets> --gpu <gpu>
+python -m ppgs.evaluate \
+    --config <name> \
+    --datasets <datasets> \
+    --checkpoint <checkpoint> \
+    --gpu <gpu>
 ```
 
 
 ## Citation
 
 ### IEEE
 C. Churchwell, M. Morrison, and B. Pardo, "High-Fidelity Neural Phonetic Posteriorgrams,"
```

### Comparing `ppgs-0.0.3/ppgs.egg-info/SOURCES.txt` & `ppgs-0.0.4/ppgs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ppgs.egg-info/requires.txt
 ppgs.egg-info/top_level.txt
 ppgs/assets/balanced_similarity.pt
 ppgs/assets/phoneme_weights.pt
 ppgs/assets/configs/bottleneck.yaml
 ppgs/assets/configs/ppg-quality-mushra.yaml
 ppgs/assets/partitions/arctic.json
-ppgs/assets/partitions/commonvoice.json.REMOVED.git-id
+ppgs/assets/partitions/commonvoice.json
 ppgs/assets/partitions/timit.json
 ppgs/config/__init__.py
 ppgs/config/defaults.py
 ppgs/config/static.py
 ppgs/config/w2v2fb.py
 ppgs/data/__init__.py
 ppgs/data/collate.py
@@ -52,15 +52,14 @@
 ppgs/evaluate/__main__.py
 ppgs/evaluate/core.py
 ppgs/evaluate/metrics.py
 ppgs/evaluate/visualize.py
 ppgs/model/__init__.py
 ppgs/model/convolution.py
 ppgs/model/core.py
-ppgs/model/mamba.py
 ppgs/model/transformer.py
 ppgs/model/w2v2.py
 ppgs/model/w2v2fc.py
 ppgs/partition/__init__.py
 ppgs/partition/__main__.py
 ppgs/partition/core.py
 ppgs/plot/__init__.py
```

### Comparing `ppgs-0.0.3/setup.py` & `ppgs-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,47 +4,45 @@
 with open('README.md') as file:
     long_description = file.read()
 
 
 setup(
     name='ppgs',
     description='Phonetic posteriorgrams',
-    version='0.0.3',
+    version='0.0.4',
     author='Interactive Audio Lab',
     author_email='interactiveaudiolab@gmail.com',
     url='https://github.com/interactiveaudiolab/ppgs',
     extras_require={
         'train': [
             'dac',
             'encodec',
             'g2pM',
             'gdown>=4.6.2',
             'humanfriendly',
-            'librosa',
-            'mamba-ssm',
-            'matplotlib',
             'nltk',
             'pyyaml',
             'torch-complex'
         ]
     },
     install_requires=[
         'espnet',
         'huggingface-hub',
+        'librosa',
+        'matplotlib',
         'moviepy',
         'numpy',
         'pypar',
         'torch',
         'torchaudio',
         'torchutil',
         'tqdm',
         'transformers',
         'opencv-python',
         'yapecs',
-        'gdown>=4.6.2'
     ],
     packages=find_packages(),
     package_data={'ppgs': ['assets/*', 'assets/*/*']},
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['phonemes', 'ppg', 'pronunciation', 'speech'],
     classifiers=['License :: OSI Approved :: MIT License'],
```

