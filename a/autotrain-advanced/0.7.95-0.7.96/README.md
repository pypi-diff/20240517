# Comparing `tmp/autotrain-advanced-0.7.95.tar.gz` & `tmp/autotrain-advanced-0.7.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.95.tar", last modified: Wed May 15 14:36:37 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.96.tar", last modified: Fri May 17 06:37:39 2024, max compression
```

## Comparing `autotrain-advanced-0.7.95.tar` & `autotrain-advanced-0.7.96.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.829802 autotrain-advanced-0.7.95/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.95/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-15 14:36:37.829802 autotrain-advanced-0.7.95/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-15 14:23:32.000000 autotrain-advanced-0.7.95/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-15 14:36:37.829802 autotrain-advanced-0.7.95/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-15 14:36:15.000000 autotrain-advanced-0.7.95/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.95/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.95/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-15 14:31:42.000000 autotrain-advanced-0.7.95/src/autotrain/app/colab.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.95/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-15 08:43:33.000000 autotrain-advanced-0.7.95/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.95/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.95/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-15 11:15:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_object_detection.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.95/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.95/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-15 11:35:44.000000 autotrain-advanced-0.7.95/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.95/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.95/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.95/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-15 11:27:08.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7592 2024-05-14 11:01:54.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.95/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.333607 autotrain-advanced-0.7.96/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.96/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-17 06:37:39.333607 autotrain-advanced-0.7.96/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.96/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-17 06:37:39.333607 autotrain-advanced-0.7.96/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.96/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.309608 autotrain-advanced-0.7.96/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.309608 autotrain-advanced-0.7.96/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-17 06:37:26.000000 autotrain-advanced-0.7.96/src/autotrain/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/app/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.96/src/autotrain/app/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.96/src/autotrain/app/api_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.96/src/autotrain/app/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.96/src/autotrain/app/colab.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.96/src/autotrain/app/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.96/src/autotrain/app/models.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.96/src/autotrain/app/oauth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.96/src/autotrain/app/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/app/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.96/src/autotrain/app/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/app/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.96/src/autotrain/app/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.96/src/autotrain/app/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.96/src/autotrain/app/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.96/src/autotrain/app/templates/login.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1923 2024-05-17 06:28:50.000000 autotrain-advanced-0.7.96/src/autotrain/app/training_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17663 2024-05-17 06:34:17.000000 autotrain-advanced-0.7.96/src/autotrain/app/ui_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3409 2024-05-17 06:28:48.000000 autotrain-advanced-0.7.96/src/autotrain/app/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/backends/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.96/src/autotrain/backends/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/backends/base.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.96/src/autotrain/backends/endpoints.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.96/src/autotrain/backends/local.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.96/src/autotrain/backends/ngc.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.96/src/autotrain/backends/nvcf.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.96/src/autotrain/backends/spaces.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.96/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_object_detection.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_text_regression.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.96/src/autotrain/cli/run_tools.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.96/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.96/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.96/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.96/src/autotrain/parser.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.96/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.96/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.96/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.96/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/tools/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.96/src/autotrain/tools/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.96/src/autotrain/tools/convert_to_kohya.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.96/src/autotrain/tools/merge_adapter.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.313608 autotrain-advanced-0.7.96/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_default.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_dpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_orpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_reward.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_sft.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/train.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/train_xl.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7592 2024-05-14 11:01:54.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.317607 autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.96/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.321607 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-17 06:37:39.000000 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-17 06:37:39.000000 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-17 06:37:39.000000 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-17 06:37:39.000000 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-17 06:37:39.000000 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-17 06:37:39.000000 autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 06:37:39.321607 autotrain-advanced-0.7.96/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.96/static/logo.png
```

### Comparing `autotrain-advanced-0.7.95/LICENSE` & `autotrain-advanced-0.7.96/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/PKG-INFO` & `autotrain-advanced-0.7.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.95
+Version: 0.7.96
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.95/README.md` & `autotrain-advanced-0.7.96/README.md`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/setup.py` & `autotrain-advanced-0.7.96/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/__init__.py` & `autotrain-advanced-0.7.96/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warnings.filterwarnings("ignore", category=UserWarning, module="peft")
 warnings.filterwarnings("ignore", category=UserWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="datasets")
 warnings.filterwarnings("ignore", category=FutureWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="huggingface_hub")
 
 logger = Logger().get_logger()
-__version__ = "0.7.95"
+__version__ = "0.7.96"
 
 
 def is_colab():
     try:
         import google.colab
 
         return True
```

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/api_routes.py` & `autotrain-advanced-0.7.96/src/autotrain/app/api_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/app.py` & `autotrain-advanced-0.7.96/src/autotrain/app/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/colab.py` & `autotrain-advanced-0.7.96/src/autotrain/app/colab.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/db.py` & `autotrain-advanced-0.7.96/src/autotrain/app/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/models.py` & `autotrain-advanced-0.7.96/src/autotrain/app/models.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.96/src/autotrain/app/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/params.py` & `autotrain-advanced-0.7.96/src/autotrain/app/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.96/src/autotrain/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.96/src/autotrain/app/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.96/src/autotrain/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.96/src/autotrain/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/templates/login.html` & `autotrain-advanced-0.7.96/src/autotrain/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.96/src/autotrain/app/training_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import asyncio
 import os
+import signal
+import sys
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
 
 from autotrain import logger
 from autotrain.app.db import AutoTrainDB
 from autotrain.app.utils import get_running_jobs, kill_process_by_pid
@@ -16,14 +18,22 @@
 TASK_ID = int(os.environ.get("TASK_ID"))
 PARAMS = os.environ.get("PARAMS")
 DATA_PATH = os.environ.get("DATA_PATH")
 MODEL = os.environ.get("MODEL")
 DB = AutoTrainDB("autotrain.db")
 
 
+def graceful_exit(signum, frame):
+    logger.info("SIGTERM received. Performing cleanup...")
+    sys.exit(0)
+
+
+signal.signal(signal.SIGTERM, graceful_exit)
+
+
 class BackgroundRunner:
     async def run_main(self):
         while True:
             running_jobs = get_running_jobs(DB)
             if not running_jobs:
                 logger.info("No running jobs found. Shutting down the server.")
                 kill_process_by_pid(os.getpid())
@@ -34,17 +44,23 @@
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
     process_pid = run_training(params=PARAMS, task_id=TASK_ID)
     logger.info(f"Started training with PID {process_pid}")
     DB.add_job(process_pid)
-    asyncio.create_task(runner.run_main())
+    task = asyncio.create_task(runner.run_main())
     yield
 
+    task.cancel()
+    try:
+        await task
+    except asyncio.CancelledError:
+        logger.info("Background runner task cancelled.")
+
 
 api = FastAPI(lifespan=lifespan)
 logger.info(f"AUTOTRAIN_USERNAME: {AUTOTRAIN_USERNAME}")
 logger.info(f"PROJECT_NAME: {PROJECT_NAME}")
 logger.info(f"TASK_ID: {TASK_ID}")
 logger.info(f"DATA_PATH: {DATA_PATH}")
 logger.info(f"MODEL: {MODEL}")
```

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/ui_routes.py` & `autotrain-advanced-0.7.96/src/autotrain/app/ui_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import os
+import signal
+import sys
 from typing import List
 
 import torch
 from fastapi import APIRouter, Depends, File, Form, HTTPException, Query, Request, UploadFile, status
 from fastapi.responses import HTMLResponse, JSONResponse, RedirectResponse
 from fastapi.templating import Jinja2Templates
 from huggingface_hub import repo_exists
@@ -34,14 +36,23 @@
 DB = AutoTrainDB("autotrain.db")
 MODEL_CHOICE = fetch_models()
 
 ui_router = APIRouter()
 templates_path = os.path.join(BASE_DIR, "templates")
 templates = Jinja2Templates(directory=templates_path)
 
+
+def graceful_exit(signum, frame):
+    logger.info("SIGTERM received. Performing cleanup...")
+    sys.exit(0)
+
+
+signal.signal(signal.SIGTERM, graceful_exit)
+
+
 logger.info("AutoTrain started successfully")
 
 
 def user_authentication(request: Request):
     # priority: hf_token env var > oauth_info in session > token in bearer header
     # if "oauth_info" in request.session:
     if HF_TOKEN is not None:
@@ -359,15 +370,15 @@
         DB.add_job(job_id)
         monitor_url = "Monitor your job locally / in logs"
     elif hardware.startswith("ep-"):
         monitor_url = f"https://ui.endpoints.huggingface.co/{autotrain_user}/endpoints/{job_id}"
     elif hardware.startswith("spaces-"):
         monitor_url = f"https://hf.co/spaces/{job_id}"
     else:
-        monitor_url = "Success! Monitor your job in logs. Job ID: {job_id}"
+        monitor_url = f"Success! Monitor your job in logs. Job ID: {job_id}"
 
     return {"success": "true", "monitor_url": monitor_url}
 
 
 @ui_router.get("/help/{element_id}", response_class=JSONResponse)
 async def fetch_help(element_id: str, authenticated: bool = Depends(user_authentication)):
     """
@@ -421,15 +432,19 @@
         logs = f.read()
     if len(str(logs).strip()) == 0:
         logs = "No logs available."
 
     logs = logs.split("\n")
     logs = logs[::-1]
     # remove lines containing /is_model_training & /accelerators
-    logs = [log for log in logs if "/is_model_training" not in log and "/accelerators" not in log]
+    logs = [
+        log
+        for log in logs
+        if "/ui/is_model_training" not in log and "/ui/accelerators" not in log and "/ui/logs" not in log
+    ]
 
     cuda_available = torch.cuda.is_available()
     if cuda_available:
         devices = Device.all()
         device_logs = []
         for device in devices:
             device_logs.append(
```

### Comparing `autotrain-advanced-0.7.95/src/autotrain/app/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/app/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 import psutil
 import requests
 
 from autotrain import config, logger
 
 
+def graceful_exit(signum, frame):
+    logger.info("SIGTERM received. Performing cleanup...")
+    sys.exit(0)
+
+
+signal.signal(signal.SIGTERM, graceful_exit)
+
+
 def get_running_jobs(db):
     running_jobs = db.get_running_jobs()
     if running_jobs:
         for _pid in running_jobs:
             proc_status = get_process_status(_pid)
             proc_status = proc_status.strip().lower()
             if proc_status in ("completed", "error", "zombie"):
@@ -35,22 +43,21 @@
     except psutil.NoSuchProcess:
         logger.info(f"No process found with PID: {pid}")
         return "Completed"
 
 
 def kill_process_by_pid(pid):
     """Kill process by PID."""
-
-    def sigint_handler(signum, frame):
-        """Handle SIGINT signal gracefully."""
-        logger.info("SIGINT received. Exiting gracefully...")
-        sys.exit(0)  # Exit with code 0
-
-    signal.signal(signal.SIGINT, sigint_handler)
-    os.kill(pid, signal.SIGTERM)
+    try:
+        os.kill(pid, signal.SIGTERM)
+        logger.info(f"Sent SIGTERM to process with PID {pid}")
+    except ProcessLookupError:
+        logger.error(f"No process found with PID {pid}")
+    except Exception as e:
+        logger.error(f"Failed to send SIGTERM to process with PID {pid}: {e}")
 
 
 def token_verification(token):
     if token.startswith("hf_oauth"):
         _api_url = config.HF_API + "/oauth/userinfo"
     else:
         _api_url = config.HF_API + "/api/whoami-v2"
```

### Comparing `autotrain-advanced-0.7.95/src/autotrain/backends/base.py` & `autotrain-advanced-0.7.96/src/autotrain/backends/base.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/backends/endpoints.py` & `autotrain-advanced-0.7.96/src/autotrain/backends/endpoints.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/backends/ngc.py` & `autotrain-advanced-0.7.96/src/autotrain/backends/ngc.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/backends/nvcf.py` & `autotrain-advanced-0.7.96/src/autotrain/backends/nvcf.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/backends/spaces.py` & `autotrain-advanced-0.7.96/src/autotrain/backends/spaces.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_object_detection.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_object_detection.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_seq2seq.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_text_regression.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_text_regression.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_token_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/run_tools.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/run_tools.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/commands.py` & `autotrain-advanced-0.7.96/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/help.py` & `autotrain-advanced-0.7.96/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/logging.py` & `autotrain-advanced-0.7.96/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/parser.py` & `autotrain-advanced-0.7.96/src/autotrain/parser.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.96/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.96/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.96/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.96/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/project.py` & `autotrain-advanced-0.7.96/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/tasks.py` & `autotrain-advanced-0.7.96/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/tools/convert_to_kohya.py` & `autotrain-advanced-0.7.96/src/autotrain/tools/convert_to_kohya.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/tools/merge_adapter.py` & `autotrain-advanced-0.7.96/src/autotrain/tools/merge_adapter.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_default.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_dpo.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_dpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_orpo.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_orpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_reward.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_reward.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_sft.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/train_clm_sft.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/clm/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/common.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/train.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train_xl.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/train_xl.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/text_regression/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/trainers/token_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain/utils.py` & `autotrain-advanced-0.7.96/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.95
+Version: 0.7.96
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.96/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.95/static/logo.png` & `autotrain-advanced-0.7.96/static/logo.png`

 * *Files identical despite different names*

