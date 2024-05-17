# Comparing `tmp/mezcla-1.3.9.9.tar.gz` & `tmp/mezcla-1.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mezcla-1.4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mezcla-1.3.9.9.tar` & `mezcla-1.4.0.0.tar`

### file list

```diff
@@ -1,222 +1,236 @@
--rw-r--r--   0        0        0      542 2023-06-18 00:28:36.095854 mezcla-1.3.9.9/.coveragerc
--rw-r--r--   0        0        0       67 2023-12-23 00:35:49.550955 mezcla-1.3.9.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      129 2024-01-10 03:17:12.006045 mezcla-1.3.9.9/.github/workflows/act-event.json
--rw-r--r--   0        0        0     3483 2024-01-12 23:59:44.940873 mezcla-1.3.9.9/.github/workflows/act.yml
--rw-r--r--   0        0        0     3955 2024-01-12 23:59:44.940873 mezcla-1.3.9.9/.github/workflows/debug.yml
--rw-r--r--   0        0        0      134 2024-01-10 03:17:12.010045 mezcla-1.3.9.9/.github/workflows/github-event.json
--rw-r--r--   0        0        0     3220 2024-01-20 01:04:29.190369 mezcla-1.3.9.9/.github/workflows/github.yml
--rw-r--r--   0        0        0      137 2024-01-10 03:17:12.010045 mezcla-1.3.9.9/.github/workflows/skip-docker.json
--rw-r--r--   0        0        0      137 2024-01-10 03:17:12.010045 mezcla-1.3.9.9/.github/workflows/use-docker.json
--rw-r--r--   0        0        0     2150 2024-02-05 02:22:35.674201 mezcla-1.3.9.9/.gitignore
--rw-r--r--   0        0        0     6279 2024-01-15 02:08:46.605161 mezcla-1.3.9.9/Dockerfile
--rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.095854 mezcla-1.3.9.9/LICENSE.txt
--rw-r--r--   0        0        0      883 2024-02-15 05:46:43.319262 mezcla-1.3.9.9/README.txt
--rw-r--r--   0        0        0      380 2023-06-18 00:28:36.095854 mezcla-1.3.9.9/TODO.txt
--rw-r--r--   0        0        0      250 2024-01-06 01:21:58.419999 mezcla-1.3.9.9/_temp-user-docker.env
-lrwxr-xr-x   0        0        0        0 2023-11-20 19:32:27.964661 mezcla-1.3.9.9/local-workflows.sh -> tools/local-workflows.sh
--rw-r--r--   0        0        0      265 2023-11-19 20:31:47.986747 mezcla-1.3.9.9/mezcla/TODO.md
--rwxr-xr-x   0        0        0     2294 2024-02-27 21:18:43.570553 mezcla-1.3.9.9/mezcla/__init__.py
--rwxr-xr-x   0        0        0     1376 2023-10-28 05:49:57.823956 mezcla-1.3.9.9/mezcla/__main__.py
--rwxr-xr-x   0        0        0    10872 2023-07-03 03:15:57.247954 mezcla-1.3.9.9/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    18007 2024-01-10 03:53:41.456581 mezcla-1.3.9.9/mezcla/audio.py
--rwxr-xr-x   0        0        0     5052 2023-08-04 17:22:24.731552 mezcla-1.3.9.9/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2023-06-18 00:28:36.099855 mezcla-1.3.9.9/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25718 2023-07-03 03:15:57.251955 mezcla-1.3.9.9/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     8307 2023-12-05 06:09:36.641882 mezcla-1.3.9.9/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     9241 2023-07-03 03:15:57.251955 mezcla-1.3.9.9/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14896 2023-12-25 20:30:57.995670 mezcla-1.3.9.9/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0     6042 2024-01-14 21:22:54.323127 mezcla-1.3.9.9/mezcla/convert_emoticons.py
--rwxr-xr-x   0        0        0    22554 2023-08-04 17:22:24.731552 mezcla-1.3.9.9/mezcla/cut.py
--rwxr-xr-x   0        0        0     4795 2023-11-07 23:03:56.570514 mezcla-1.3.9.9/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    52432 2024-02-10 06:04:37.816315 mezcla-1.3.9.9/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0     4842 2024-02-18 01:07:01.707066 mezcla-1.3.9.9/mezcla/evaluate_example_tests.py
--rwxr-xr-x   0        0        0        0 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12874 2023-07-03 03:15:57.251955 mezcla-1.3.9.9/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3644 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/download_user_gist.py
--rw-r--r--   0        0        0      118 2023-09-03 04:28:25.907636 mezcla-1.3.9.9/mezcla/examples/dummy-image.png
--rwxr-xr-x   0        0        0     6477 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8811 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0    54141 2024-02-24 00:18:03.430170 mezcla-1.3.9.9/mezcla/examples/hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     4660 2024-01-19 02:56:58.191707 mezcla-1.3.9.9/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     6011 2024-02-18 02:09:14.186107 mezcla-1.3.9.9/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/plot_forest_importances.py
--rw-r--r--   0        0        0       20 2024-01-06 01:21:58.419999 mezcla-1.3.9.9/mezcla/examples/resources/translate_es_1.txt
--rw-r--r--   0        0        0     1809 2024-01-06 01:21:58.419999 mezcla-1.3.9.9/mezcla/examples/resources/translate_es_25.txt
--rw-r--r--   0        0        0   105004 2024-01-06 01:21:58.423999 mezcla-1.3.9.9/mezcla/examples/resources/us1.wav
--rw-r--r--   0        0        0    89644 2024-01-06 01:21:58.423999 mezcla-1.3.9.9/mezcla/examples/resources/us10.wav
--rw-r--r--   0        0        0   159725 2023-09-24 17:55:32.838498 mezcla-1.3.9.9/mezcla/examples/sd-spooky-pacman.png
--rwxr-xr-x   0        0        0    13004 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     2072 2024-02-13 23:48:53.709200 mezcla-1.3.9.9/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0    13881 2024-01-26 22:05:20.253359 mezcla-1.3.9.9/mezcla/examples/tests/test_hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     4608 2024-01-19 02:57:22.956854 mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_speechrec.py
--rw-r--r--   0        0        0     5783 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_translation.py
--rw-r--r--   0        0        0     4272 2024-02-05 06:18:22.947788 mezcla-1.3.9.9/mezcla/examples/tests/test_youtube_transcript.py
--rwxr-xr-x   0        0        0     3617 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     3351 2024-02-13 23:49:45.739212 mezcla-1.3.9.9/mezcla/examples/youtube_transcript.py
--rwxr-xr-x   0        0        0     5645 2023-10-28 05:49:57.827956 mezcla-1.3.9.9/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     8648 2023-12-05 06:09:36.641882 mezcla-1.3.9.9/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2836 2024-02-25 21:50:11.199678 mezcla-1.3.9.9/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32976 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    38023 2024-02-14 01:20:37.557523 mezcla-1.3.9.9/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    51316 2024-01-26 22:07:19.425573 mezcla-1.3.9.9/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     5800 2024-01-19 07:25:16.197480 mezcla-1.3.9.9/mezcla/ipython_utils.py
--rwxr-xr-x   0        0        0     5718 2024-01-13 00:02:35.064560 mezcla-1.3.9.9/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17985 2023-10-16 22:30:24.461638 mezcla-1.3.9.9/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    52196 2024-02-25 23:17:36.844026 mezcla-1.3.9.9/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-06-18 00:28:36.115856 mezcla-1.3.9.9/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11040 2024-02-05 02:23:37.860124 mezcla-1.3.9.9/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0      608 2023-10-28 05:49:57.831956 mezcla-1.3.9.9/mezcla/mezcla
--rwxr-xr-x   0        0        0    16908 2024-01-29 02:43:05.206522 mezcla-1.3.9.9/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0    10273 2024-01-29 02:46:17.354076 mezcla-1.3.9.9/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    23846 2024-02-24 00:35:11.471795 mezcla-1.3.9.9/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0     1323 2024-01-16 02:17:35.819701 mezcla-1.3.9.9/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31564 2023-10-16 22:30:24.461638 mezcla-1.3.9.9/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      915 2023-11-28 08:56:45.997810 mezcla-1.3.9.9/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     3202 2023-07-21 06:17:43.311676 mezcla-1.3.9.9/mezcla/python_ast.py
--rwxr-xr-x   0        0        0     7345 2023-11-19 20:31:47.994747 mezcla-1.3.9.9/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     9144 2023-11-28 08:56:46.001810 mezcla-1.3.9.9/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40735 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39709 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/run_bert_classifier.py
--rw-r--r--   0        0        0    24045 2023-12-23 00:35:49.666955 mezcla-1.3.9.9/mezcla/samples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0    17400 2023-06-18 00:28:36.119856 mezcla-1.3.9.9/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     2930 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    22899 2024-02-09 05:58:53.199379 mezcla-1.3.9.9/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3168 2024-01-10 03:13:25.131399 mezcla-1.3.9.9/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2023-06-18 00:28:36.119856 mezcla-1.3.9.9/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    54669 2024-01-27 06:59:58.811207 mezcla-1.3.9.9/mezcla/system.py
--rw-r--r--   0        0        0   908397 2023-12-23 00:35:49.678955 mezcla-1.3.9.9/mezcla/temp/compound_CID_3672.xml
--rw-r--r--   0        0        0     1124 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/temp/plot.py
--rwxr-xr-x   0        0        0    45776 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     6257 2024-02-18 02:10:12.834939 mezcla-1.3.9.9/mezcla/template.py
--rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      140 2023-11-19 20:31:47.994747 mezcla-1.3.9.9/mezcla/tests/README.md
--rw-r--r--   0        0        0      462 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1082 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/adhoc-tests.batspp
--rwxr-xr-x   0        0        0     1900 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/tests/conftest.py
--rw-r--r--   0        0        0     1306 2023-12-23 00:35:49.678955 mezcla-1.3.9.9/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt
--rw-r--r--   0        0        0    21583 2023-12-23 00:35:49.678955 mezcla-1.3.9.9/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb
--rw-r--r--   0        0        0    28841 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py.ipynb
--rw-r--r--   0        0        0    44701 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py_experimental.ipynb
--rw-r--r--   0        0        0    23692 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb
--rw-r--r--   0        0        0    29559 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_translation.ipynb
--rw-r--r--   0        0        0    58860 2024-01-06 01:21:58.443999 mezcla-1.3.9.9/mezcla/tests/jupyter/test_template.ipynb
--rw-r--r--   0        0        0     1176 2023-11-28 08:56:46.001810 mezcla-1.3.9.9/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3898 2023-11-23 07:44:42.985055 mezcla-1.3.9.9/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0     3283 2024-01-13 02:25:33.199045 mezcla-1.3.9.9/mezcla/tests/misc_tests.py
--rw-r--r--   0        0        0      312 2023-11-19 20:31:47.994747 mezcla-1.3.9.9/mezcla/tests/regression.batspp
--rw-r--r--   0        0        0     1453 2023-12-13 03:20:36.066992 mezcla-1.3.9.9/mezcla/tests/resources/argentinian-attraction-snippets.txt
--rw-r--r--   0        0        0      810 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0   324207 2023-08-15 23:14:53.434294 mezcla-1.3.9.9/mezcla/tests/resources/random-10pct-tweet-emotions.tsv
--rw-r--r--   0        0        0     1152 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0      415 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-ar.list
--rw-r--r--   0        0        0      391 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-en.list
--rw-r--r--   0        0        0      294 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-es.list
--rw-r--r--   0        0        0      472 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-ru.list
--rw-r--r--   0        0        0     2780 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/resources/test.arpa
--rwxr-xr-x   0        0        0    14631 2024-02-25 21:50:57.298231 mezcla-1.3.9.9/mezcla/tests/resources/word-POS.freq
--rwxr-xr-x   0        0        0    11479 2024-02-25 21:44:14.241332 mezcla-1.3.9.9/mezcla/tests/resources/word.freq
--rw-r--r--   0        0        0      254 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     5120 2024-02-26 23:37:28.019883 mezcla-1.3.9.9/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     1766 2024-01-10 03:13:25.131399 mezcla-1.3.9.9/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     5942 2024-01-10 03:13:25.131399 mezcla-1.3.9.9/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0     2343 2023-10-24 00:05:30.113456 mezcla-1.3.9.9/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     7559 2023-12-13 03:20:36.066992 mezcla-1.3.9.9/mezcla/tests/test_compute_tfidf.py
--rwxr-xr-x   0        0        0     4681 2024-01-29 02:49:52.352507 mezcla-1.3.9.9/mezcla/tests/test_convert_emoticons.py
--rwxr-xr-x   0        0        0     2905 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    17872 2024-01-13 02:25:33.199045 mezcla-1.3.9.9/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     2654 2024-02-18 00:52:35.708230 mezcla-1.3.9.9/mezcla/tests/test_evaluate_example_tests.py
--rwxr-xr-x   0        0        0     5469 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0    17414 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_format_profile.py
--rwxr-xr-x   0        0        0     3449 2023-07-03 03:15:57.263955 mezcla-1.3.9.9/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    17227 2024-02-11 07:09:18.051172 mezcla-1.3.9.9/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13525 2024-01-19 07:26:02.648020 mezcla-1.3.9.9/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0     2023 2023-10-16 22:30:24.465638 mezcla-1.3.9.9/mezcla/tests/test_ipython_utils.py
--rwxr-xr-x   0        0        0    11821 2024-01-10 05:20:11.597430 mezcla-1.3.9.9/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     3473 2023-12-24 04:34:38.391312 mezcla-1.3.9.9/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0    10850 2024-02-15 05:50:30.569406 mezcla-1.3.9.9/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     9528 2024-02-16 17:38:36.156177 mezcla-1.3.9.9/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     4204 2024-01-19 07:24:28.075538 mezcla-1.3.9.9/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0     5098 2023-12-25 20:30:57.995670 mezcla-1.3.9.9/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0     1400 2024-01-16 02:25:00.658659 mezcla-1.3.9.9/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8297 2023-07-03 03:15:57.263955 mezcla-1.3.9.9/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1183 2023-07-03 03:15:57.263955 mezcla-1.3.9.9/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0     2156 2023-08-08 20:42:24.883287 mezcla-1.3.9.9/mezcla/tests/test_python_ast.py
--rwxr-xr-x   0        0        0     1735 2023-11-19 20:31:47.998747 mezcla-1.3.9.9/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2389 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0     2372 2023-10-24 00:05:30.113456 mezcla-1.3.9.9/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     5511 2023-12-31 19:50:34.708502 mezcla-1.3.9.9/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0    12822 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_spell.py
--rwxr-xr-x   0        0        0      882 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    36834 2024-02-16 17:38:36.156177 mezcla-1.3.9.9/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     2231 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     5752 2023-11-07 23:03:56.586514 mezcla-1.3.9.9/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     8905 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7361 2023-08-06 02:05:25.411349 mezcla-1.3.9.9/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    25913 2024-02-16 17:38:36.160177 mezcla-1.3.9.9/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0     2041 2023-08-15 23:14:53.434294 mezcla-1.3.9.9/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0     4172 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/test_transpose_data.py
--rw-r--r--   0        0        0      435 2023-12-23 00:35:49.686955 mezcla-1.3.9.9/mezcla/tests/test_transpose_lines.input
--rwxr-xr-x   0        0        0     5709 2024-02-26 23:45:37.397580 mezcla-1.3.9.9/mezcla/tests/test_unittest_wrapper.py
--rwxr-xr-x   0        0        0     2355 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_xml_utils.py
--rwxr-xr-x   0        0        0      676 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_corpus.py
--rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_dockeyword.py
--rwxr-xr-x   0        0        0      688 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_document.py
--rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    36563 2023-11-07 23:03:56.586514 mezcla-1.3.9.9/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    28563 2024-02-24 00:24:18.170215 mezcla-1.3.9.9/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    13236 2024-02-18 02:11:59.716346 mezcla-1.3.9.9/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2023-12-13 03:20:36.066992 mezcla-1.3.9.9/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0      777 2023-11-25 07:31:25.091092 mezcla-1.3.9.9/mezcla/tfidf/config.py
--rwxr-xr-x   0        0        0    19427 2023-12-25 20:30:57.995670 mezcla-1.3.9.9/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     3146 2023-12-13 03:20:36.070992 mezcla-1.3.9.9/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7925 2023-12-13 03:20:36.070992 mezcla-1.3.9.9/mezcla/tfidf/document.py
--rwxr-xr-x   0        0        0    19704 2024-02-24 01:15:02.034525 mezcla-1.3.9.9/mezcla/tfidf/preprocess.py
--rw-r--r--   0        0        0     3961 2023-12-13 03:20:36.070992 mezcla-1.3.9.9/mezcla/tfidf/tests/misc_test.py
--rwxr-xr-x   0        0        0    60411 2024-01-10 03:13:25.139399 mezcla-1.3.9.9/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5272 2023-12-23 00:35:49.686955 mezcla-1.3.9.9/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5149 2023-08-15 23:14:53.434294 mezcla-1.3.9.9/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6673 2023-10-16 22:30:24.473638 mezcla-1.3.9.9/mezcla/transpose_data.py
--rwxr-xr-x   0        0        0    27371 2024-02-26 23:42:50.612807 mezcla-1.3.9.9/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2023-06-18 00:28:36.139858 mezcla-1.3.9.9/mezcla/xml_utils.py
--rw-r--r--   0        0        0      432 2024-01-10 03:13:25.139399 mezcla-1.3.9.9/non-binary-requirements.txt
--rw-r--r--   0        0        0      803 2024-02-27 21:18:43.570553 mezcla-1.3.9.9/pyproject.toml
--rw-r--r--   0        0        0      750 2024-01-10 03:13:25.139399 mezcla-1.3.9.9/required-packages.txt
--rw-r--r--   0        0        0     3737 2024-02-05 04:51:35.245886 mezcla-1.3.9.9/requirements.txt
-lrwxr-xr-x   0        0        0        0 2023-11-20 19:32:33.112667 mezcla-1.3.9.9/run_tests.bash -> tools/run_tests.bash
--rwxr-xr-x   0        0        0     1943 2024-02-27 21:18:43.570553 mezcla-1.3.9.9/setup.py
--rwxr-xr-x   0        0        0    45023 2023-06-18 00:28:36.139858 mezcla-1.3.9.9/temp/simple_batspp.py
--rw-r--r--   0        0        0     1382 2024-02-24 23:00:50.169992 mezcla-1.3.9.9/tools/_temp_test_settings.bash
--rwxr-xr-x   0        0        0     3002 2024-01-10 03:26:05.393620 mezcla-1.3.9.9/tools/local-workflows.sh
--rwxr-xr-x   0        0        0     3770 2024-02-24 23:04:45.025995 mezcla-1.3.9.9/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-06-18 00:28:36.139858 mezcla-1.3.9.9/tox.ini
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 mezcla-1.3.9.9/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/.coveragerc
+-rw-r--r--   0        0        0       67 2024-05-12 06:12:49.213578 mezcla-1.4.0.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      129 2024-05-12 06:12:49.213578 mezcla-1.4.0.0/.github/workflows/act-event.json
+-rw-r--r--   0        0        0     3483 2024-05-12 06:12:49.213578 mezcla-1.4.0.0/.github/workflows/act.yml
+-rw-r--r--   0        0        0     3955 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/.github/workflows/debug.yml
+-rw-r--r--   0        0        0      134 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/.github/workflows/github-event.json
+-rw-r--r--   0        0        0     3228 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/.github/workflows/github.yml
+-rw-r--r--   0        0        0      137 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/.github/workflows/skip-docker.json
+-rw-r--r--   0        0        0      137 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/.github/workflows/use-docker.json
+-rw-r--r--   0        0        0     2150 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/.gitignore
+-rw-r--r--   0        0        0     7007 2024-05-12 06:12:49.217578 mezcla-1.4.0.0/Dockerfile
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.4.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      881 2024-05-14 04:54:27.006918 mezcla-1.4.0.0/README.txt
+-rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/TODO.txt
+-rw-r--r--   0        0        0      250 2024-05-12 06:12:49.221578 mezcla-1.4.0.0/_temp-user-docker.env
+-rw-r--r--   0        0        0      634 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/docs/Makefile
+-rw-r--r--   0        0        0     1085 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/docs/conf.py
+-rw-r--r--   0        0        0     4062 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2024-05-12 06:12:49.221578 mezcla-1.4.0.0/local-workflows.sh -> tools/local-workflows.sh
+-rw-r--r--   0        0        0      265 2024-05-12 06:12:49.221578 mezcla-1.4.0.0/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     2294 2024-05-16 02:57:56.726842 mezcla-1.4.0.0/mezcla/__init__.py
+-rwxr-xr-x   0        0        0     1358 2024-05-12 06:12:49.221578 mezcla-1.4.0.0/mezcla/__main__.py
+-rwxr-xr-x   0        0        0        0 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/mezcla/adhoc/__init__.py
+-rwxr-xr-x   0        0        0    26129 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/mezcla/adhoc/check_time_tracking.py
+-rwxr-xr-x   0        0        0     3740 2024-05-12 06:12:49.221578 mezcla-1.4.0.0/mezcla/adhoc/tests/test_check_time_tracking.py
+-rwxr-xr-x   0        0        0    10872 2024-05-12 06:12:49.225578 mezcla-1.4.0.0/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    18007 2024-05-12 06:12:49.225578 mezcla-1.4.0.0/mezcla/audio.py
+-rwxr-xr-x   0        0        0     5051 2024-05-12 06:13:34.837710 mezcla-1.4.0.0/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.4.0.0/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25718 2024-05-12 06:12:49.225578 mezcla-1.4.0.0/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     8307 2024-05-12 06:12:49.225578 mezcla-1.4.0.0/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     9241 2024-05-12 06:12:49.225578 mezcla-1.4.0.0/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14896 2024-05-12 06:12:49.229578 mezcla-1.4.0.0/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0     6040 2024-05-12 06:12:49.229578 mezcla-1.4.0.0/mezcla/convert_emoticons.py
+-rwxr-xr-x   0        0        0    23141 2024-05-12 06:13:34.841710 mezcla-1.4.0.0/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4795 2024-05-12 06:12:49.229578 mezcla-1.4.0.0/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    52703 2024-05-14 04:54:27.010918 mezcla-1.4.0.0/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0     5033 2024-05-12 06:12:49.233578 mezcla-1.4.0.0/mezcla/evaluate_example_tests.py
+-rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12874 2024-05-12 06:12:49.233578 mezcla-1.4.0.0/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3644 2024-05-12 06:12:49.233578 mezcla-1.4.0.0/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/examples/download_user_gist.py
+-rw-r--r--   0        0        0      118 2024-05-12 06:12:49.233578 mezcla-1.4.0.0/mezcla/examples/dummy-image.png
+-rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.4.0.0/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.4.0.0/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8811 2024-05-12 06:12:49.233578 mezcla-1.4.0.0/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    54141 2024-05-12 06:12:49.237578 mezcla-1.4.0.0/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     4660 2024-05-12 06:12:49.237578 mezcla-1.4.0.0/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     6076 2024-05-12 06:13:34.841710 mezcla-1.4.0.0/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.4.0.0/mezcla/examples/iris.csv
+-rwxr-xr-x   0        0        0     8645 2024-05-12 06:12:49.237578 mezcla-1.4.0.0/mezcla/examples/matrix_multiply_benchmarking.py
+-rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.4.0.0/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.4.0.0/mezcla/examples/plot_forest_importances.py
+-rw-r--r--   0        0        0       20 2024-05-12 06:12:49.237578 mezcla-1.4.0.0/mezcla/examples/resources/translate_es_1.txt
+-rw-r--r--   0        0        0     1809 2024-05-12 06:12:49.237578 mezcla-1.4.0.0/mezcla/examples/resources/translate_es_25.txt
+-rw-r--r--   0        0        0   105004 2024-05-12 06:12:49.241578 mezcla-1.4.0.0/mezcla/examples/resources/us1.wav
+-rw-r--r--   0        0        0    89644 2024-05-12 06:12:49.245578 mezcla-1.4.0.0/mezcla/examples/resources/us10.wav
+-rw-r--r--   0        0        0   159725 2024-05-12 06:12:49.245578 mezcla-1.4.0.0/mezcla/examples/sd-spooky-pacman.png
+-rwxr-xr-x   0        0        0    13004 2024-05-12 06:12:49.245578 mezcla-1.4.0.0/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     2211 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     5462 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tests/template.py
+-rwxr-xr-x   0        0        0    13881 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     4608 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tests/test_hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     5783 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tests/test_hugging_face_translation.py
+-rwxr-xr-x   0        0        0     3199 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tests/test_matrix_multiply_benchmarking.py
+-rwxr-xr-x   0        0        0     3873 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tests/test_youtube_transcript.py
+-rwxr-xr-x   0        0        0     3617 2024-05-12 06:12:49.249578 mezcla-1.4.0.0/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     3401 2024-05-12 06:12:49.253579 mezcla-1.4.0.0/mezcla/examples/youtube_transcript.py
+-rwxr-xr-x   0        0        0     5645 2024-05-12 06:12:49.253579 mezcla-1.4.0.0/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     8648 2024-05-12 06:12:49.253579 mezcla-1.4.0.0/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.4.0.0/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     3073 2024-05-12 06:13:34.841710 mezcla-1.4.0.0/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32976 2024-05-12 06:12:49.253579 mezcla-1.4.0.0/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    42250 2024-05-14 04:54:27.010918 mezcla-1.4.0.0/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0     2231 2024-05-12 06:13:34.845710 mezcla-1.4.0.0/mezcla/gpu_utils.py
+-rwxr-xr-x   0        0        0    51212 2024-05-12 06:12:49.257578 mezcla-1.4.0.0/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     5861 2024-05-12 06:12:49.257578 mezcla-1.4.0.0/mezcla/ipython_utils.py
+-rwxr-xr-x   0        0        0     5718 2024-05-12 06:12:49.257578 mezcla-1.4.0.0/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17985 2024-05-12 06:12:49.257578 mezcla-1.4.0.0/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    16511 2024-05-14 04:54:27.010918 mezcla-1.4.0.0/mezcla/llm_desktop_search.py
+-rwxr-xr-x   0        0        0    52863 2024-05-12 06:13:34.849710 mezcla-1.4.0.0/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11040 2024-05-12 06:12:49.261578 mezcla-1.4.0.0/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0      608 2024-05-12 06:12:49.261578 mezcla-1.4.0.0/mezcla/mezcla
+-rwxr-xr-x   0        0        0    16908 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0    10273 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    24478 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0     1323 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31564 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      915 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     3202 2024-05-12 06:12:49.265578 mezcla-1.4.0.0/mezcla/python_ast.py
+-rwxr-xr-x   0        0        0     7337 2024-05-12 06:13:34.849710 mezcla-1.4.0.0/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     9407 2024-05-12 06:13:34.849710 mezcla-1.4.0.0/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40735 2024-05-12 06:12:49.269579 mezcla-1.4.0.0/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39709 2024-05-12 06:12:49.269579 mezcla-1.4.0.0/mezcla/run_bert_classifier.py
+-rw-r--r--   0        0        0    24045 2024-05-12 06:12:49.273579 mezcla-1.4.0.0/mezcla/samples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     2930 2024-05-12 06:12:49.273579 mezcla-1.4.0.0/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    22899 2024-05-12 06:12:49.273579 mezcla-1.4.0.0/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3168 2024-05-12 06:12:49.273579 mezcla-1.4.0.0/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.4.0.0/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    56713 2024-05-14 04:54:27.014918 mezcla-1.4.0.0/mezcla/system.py
+-rw-r--r--   0        0        0   908397 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/temp/compound_CID_3672.xml
+-rwxr-xr-x   0        0        0     1124 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/temp/plot.py
+-rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     6218 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/template.py
+-rw-r--r--   0        0        0     7418 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      140 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/tests/README.md
+-rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0     1341 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/tests/adhoc-tests.batspp
+-rwxr-xr-x   0        0        0     1900 2024-05-12 06:12:49.289579 mezcla-1.4.0.0/mezcla/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2024-05-12 06:12:49.293578 mezcla-1.4.0.0/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt
+-rw-r--r--   0        0        0    21583 2024-05-12 06:12:49.293578 mezcla-1.4.0.0/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb
+-rw-r--r--   0        0        0    28841 2024-05-12 06:12:49.293578 mezcla-1.4.0.0/mezcla/tests/jupyter/test_audio_py.ipynb
+-rw-r--r--   0        0        0    44701 2024-05-12 06:12:49.293578 mezcla-1.4.0.0/mezcla/tests/jupyter/test_audio_py_experimental.ipynb
+-rw-r--r--   0        0        0    23692 2024-05-12 06:12:49.293578 mezcla-1.4.0.0/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb
+-rw-r--r--   0        0        0    29559 2024-05-12 06:12:49.297579 mezcla-1.4.0.0/mezcla/tests/jupyter/test_hugging_face_translation.ipynb
+-rw-r--r--   0        0        0    58860 2024-05-12 06:12:49.297579 mezcla-1.4.0.0/mezcla/tests/jupyter/test_template.ipynb
+-rw-r--r--   0        0        0     1176 2024-05-12 06:12:49.297579 mezcla-1.4.0.0/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3898 2024-05-12 06:12:49.297579 mezcla-1.4.0.0/mezcla/tests/misc_doctests.py
+-rwxr-xr-x   0        0        0     3722 2024-05-12 06:13:34.853710 mezcla-1.4.0.0/mezcla/tests/misc_tests.py
+-rw-r--r--   0        0        0      312 2024-05-12 06:12:49.297579 mezcla-1.4.0.0/mezcla/tests/regression.batspp
+-rw-r--r--   0        0        0     1453 2024-05-12 06:12:49.297579 mezcla-1.4.0.0/mezcla/tests/resources/argentinian-attraction-snippets.txt
+-rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.4.0.0/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.4.0.0/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.4.0.0/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0   324207 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/random-10pct-tweet-emotions.tsv
+-rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0      415 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/spell-py-ar.list
+-rw-r--r--   0        0        0      391 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/spell-py-en.list
+-rw-r--r--   0        0        0      294 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/spell-py-es.list
+-rw-r--r--   0        0        0      472 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/spell-py-ru.list
+-rw-r--r--   0        0        0     2780 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/test.arpa
+-rwxr-xr-x   0        0        0    14631 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/word-POS.freq
+-rwxr-xr-x   0        0        0    11479 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/resources/word.freq
+-rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     6108 2024-05-14 04:54:27.014918 mezcla-1.4.0.0/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     1766 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     5942 2024-05-12 06:12:49.309579 mezcla-1.4.0.0/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0     2343 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     7559 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     4681 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_convert_emoticons.py
+-rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.4.0.0/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.4.0.0/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    17872 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     2654 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_evaluate_example_tests.py
+-rwxr-xr-x   0        0        0     5469 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0    19004 2024-05-12 06:12:49.313579 mezcla-1.4.0.0/mezcla/tests/test_format_profile.py
+-rwxr-xr-x   0        0        0     3589 2024-05-12 06:12:49.317579 mezcla-1.4.0.0/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    20109 2024-05-12 06:13:34.853710 mezcla-1.4.0.0/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0     5162 2024-05-12 06:13:34.857710 mezcla-1.4.0.0/mezcla/tests/test_gpu_utils.py
+-rwxr-xr-x   0        0        0    14480 2024-05-12 06:12:49.317579 mezcla-1.4.0.0/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0     2023 2024-05-12 06:12:49.317579 mezcla-1.4.0.0/mezcla/tests/test_ipython_utils.py
+-rwxr-xr-x   0        0        0    11821 2024-05-12 06:12:49.317579 mezcla-1.4.0.0/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     3473 2024-05-12 06:12:49.317579 mezcla-1.4.0.0/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0    10237 2024-05-14 04:54:27.014918 mezcla-1.4.0.0/mezcla/tests/test_llm_desktop_search.py
+-rwxr-xr-x   0        0        0    10850 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     9528 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     4204 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0     5098 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0     1398 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8297 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1183 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0     2156 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_python_ast.py
+-rwxr-xr-x   0        0        0     1735 2024-05-12 06:12:49.321579 mezcla-1.4.0.0/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2389 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0     2372 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     5511 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0    13977 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_spell.py
+-rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    36834 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     2231 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     6015 2024-05-12 06:12:49.325579 mezcla-1.4.0.0/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0    11593 2024-05-12 06:13:34.857710 mezcla-1.4.0.0/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7361 2024-05-12 06:12:49.329579 mezcla-1.4.0.0/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    28922 2024-05-12 06:12:49.329579 mezcla-1.4.0.0/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.4.0.0/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0     2041 2024-05-12 06:12:49.329579 mezcla-1.4.0.0/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0     4172 2024-05-12 06:12:49.329579 mezcla-1.4.0.0/mezcla/tests/test_transpose_data.py
+-rw-r--r--   0        0        0      435 2024-05-12 06:12:49.329579 mezcla-1.4.0.0/mezcla/tests/test_transpose_lines.input
+-rwxr-xr-x   0        0        0     7214 2024-05-12 06:13:34.857710 mezcla-1.4.0.0/mezcla/tests/test_unittest_wrapper.py
+-rwxr-xr-x   0        0        0     2355 2024-05-12 06:12:49.329579 mezcla-1.4.0.0/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.4.0.0/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.4.0.0/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.4.0.0/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.4.0.0/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    36563 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    28563 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    13236 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0      777 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/tfidf/config.py
+-rwxr-xr-x   0        0        0    19427 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     3146 2024-05-12 06:12:49.333579 mezcla-1.4.0.0/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7925 2024-05-12 06:12:49.337579 mezcla-1.4.0.0/mezcla/tfidf/document.py
+-rwxr-xr-x   0        0        0    19704 2024-05-12 06:12:49.337579 mezcla-1.4.0.0/mezcla/tfidf/preprocess.py
+-rw-r--r--   0        0        0     3961 2024-05-12 06:12:49.337579 mezcla-1.4.0.0/mezcla/tfidf/tests/misc_test.py
+-rwxr-xr-x   0        0        0    60750 2024-05-12 06:12:49.337579 mezcla-1.4.0.0/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5272 2024-05-12 06:12:49.337579 mezcla-1.4.0.0/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5149 2024-05-12 06:12:49.341579 mezcla-1.4.0.0/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6673 2024-05-12 06:12:49.341579 mezcla-1.4.0.0/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    28787 2024-05-14 04:54:27.014918 mezcla-1.4.0.0/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.4.0.0/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      432 2024-05-12 06:12:49.341579 mezcla-1.4.0.0/non-binary-requirements.txt
+-rw-r--r--   0        0        0      750 2024-05-12 06:13:34.857710 mezcla-1.4.0.0/packages-required.txt
+-rw-r--r--   0        0        0      803 2024-05-16 02:57:56.726842 mezcla-1.4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3936 2024-05-12 06:13:34.861710 mezcla-1.4.0.0/requirements.txt
+lrwxr-xr-x   0        0        0        0 2024-05-12 06:12:49.341579 mezcla-1.4.0.0/run_tests.bash -> tools/run_tests.bash
+-rwxr-xr-x   0        0        0     1943 2024-05-16 02:57:56.726842 mezcla-1.4.0.0/setup.py
+-rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.4.0.0/temp/simple_batspp.py
+-rw-r--r--   0        0        0     1382 2024-05-12 06:12:49.341579 mezcla-1.4.0.0/tools/_temp_test_settings.bash
+-rwxr-xr-x   0        0        0     3002 2024-05-12 06:12:49.345579 mezcla-1.4.0.0/tools/local-workflows.sh
+-rwxr-xr-x   0        0        0     3770 2024-05-12 06:12:49.345579 mezcla-1.4.0.0/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.4.0.0/tox.ini
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 mezcla-1.4.0.0/PKG-INFO
```

### Comparing `mezcla-1.3.9.9/.coveragerc` & `mezcla-1.4.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/.github/workflows/act.yml` & `mezcla-1.4.0.0/.github/workflows/act.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/.github/workflows/debug.yml` & `mezcla-1.4.0.0/.github/workflows/debug.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/.github/workflows/github.yml` & `mezcla-1.4.0.0/.github/workflows/github.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     strategy:
       matrix:
         os: [ubuntu-latest]
         ## TODO: os: [ubuntu-20.04, ubuntu-latest]
         ## OLD: python-version: ["3.8", "3.9", "3.10"]
         ## NOTE: Need 3.8.17+ for typing support, due to backporting limitations with typing_extensions (see html_utils.py)
         ## TODO?:
-        python-version: ["3.8.17", "3.9", "3.10"]
+        python-version: ["3.8.17", "3.9", "3.10", "3.12"]
         # Note: The Dockerfile uses 3.11 so try different versions for the runner VM
         ## TODO: python-version: ["3.9", "3.10", "3.11"]
 
     steps:
       - name: Checkout Repository
         uses: actions/checkout@v3
```

### Comparing `mezcla-1.3.9.9/.gitignore` & `mezcla-1.4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/Dockerfile` & `mezcla-1.4.0.0/Dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,32 @@
 ## TODO2: fixme (see tools/run_tests.bash for workaround).
 ## TODO: ARG DEBUG_LEVEL=2
 ARG DEBUG_LEVEL=4
 ## DEBUG: ARG DEBUG_LEVEL=5
 ARG TEST_REGEX=""
 ## DEBUG: ARG TEST_REGEX="simple_main_example"
 
+# Show initial disk usage
+# See https://github.com/orgs/community/discussions/25678 [No space left on device]
+#
+RUN <<END_RUN
+    df --human-readable
+    ## TODO: track down stupid problem with step failing
+    ## echo "Top directories by disk usage (pre-install):";
+    ## du --block-size=1K / 2>&1 | sort -rn | head -20;
+    true;                               # ensure success (quirk w/ head)
+END_RUN
+
+# Temp: remove unneeded software taking up much disk space (e.g., node)
+RUN <<END_RUN
+    echo "Warning: removing unneeded software"
+    /bin/rm -rf /opt/acttoolcache/node
+    df -h /
+END_RUN
+
 # Install Python
 # See https://stackoverflow.com/a/70866416 [How to install python specific version on docker?]
 #
 # Download, extract, and install the specified Python version
 # Note:
 # - Uses versions prepared for Github Actions
 # - To find URL links, see https://github.com/actions/python-versions:
@@ -124,16 +142,17 @@
 # Note: cleans the apt-get cache
 RUN apt-get update -y && apt-get install --yes lsb-release && apt-get clean all
 # note: rcs needed for merge (TODO: place in required-packages.txt)
 RUN apt-get install --yes enchant-2 rcs
 
 # Show disk usage when debugging
 RUN <<END_RUN
-  if [ "$DEBUG_LEVEL" -ge 5 ]; then
-      echo "Top directories by disk usage:";
-      du --block-size=1K / 2>&1 | sort -rn | head -20;
-  fi
+    df --human-readable
+    ## TODO: track down stupid problem with step failing
+    ## echo "Top directories by disk usage (post-install):";
+    ## du --block-size=1K / 2>&1 | sort -rn | head -20;
+    true;                               # ensure success (quirk w/ head)
 END_RUN
 
 # Run the test, normally pytest over mezcla/tests
 # Note: the status code (i.e., $?) determines whether docker run succeeds (e.g., OK if 0)
 ENTRYPOINT DEBUG_LEVEL=$DEBUG_LEVEL TEST_REGEX="$TEST_REGEX" './tools/run_tests.bash'
```

### Comparing `mezcla-1.3.9.9/LICENSE.txt` & `mezcla-1.4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/README.txt` & `mezcla-1.4.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,24 @@
-﻿Note: This is an upgrade of the misc-utility repository with Python 2 support being phased out.
+Metadata-Version: 2.1
+Name: mezcla
+Version: 1.4.0.0
+Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
+Home-page: https://github.com/tomasohara/mezcla
+License: LGPLv3
+Author: Tomás O'Hara
+Author-email: tomasohara@gmail.com
+Description-Content-Type: text/plain
+
+﻿Note: This is an upgrade of the misc-utility repository with Python 2 support now phased out.
 
 Miscellaneous Python scripts developed over the course of several independent consulting projects. This also includes some code samples I adapted from publicly available source. (The code is not proprietary in nature. For example, it was not "borrowed" from proprietary source files, nor based on proprietary processes.)
 
 Spoiler alter: this is not "Pythonic python": I'm more into R&D than production programming. Nonetheless, there's a some useful scripts here, so I made the repository available. It is public in the spirit of open source software. 
 
 This is a companion script to shell-scripts from Github:
      https://github.com/tomasohara/shell-scripts
 
 This repository is licensed under the GNU Lesser General Public Version 3 (LGPLv3). See LICENSE.txt.
 
 Tom O'Hara
-May 2021
+May 2024
+
```

### Comparing `mezcla-1.3.9.9/mezcla/__init__.py` & `mezcla-1.4.0.0/mezcla/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-version = "1.3.9.9"
+version = "1.4.0.0"
 __VERSION__ = version
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
```

### Comparing `mezcla-1.3.9.9/mezcla/__main__.py` & `mezcla-1.4.0.0/mezcla/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 # Also see
 #    https://stackoverflow.com/questions/4042905/what-is-main-py
 #
 
 """Entry point for mezcla"""
 
 # Standard module(s)
-## OLD
-## import os
-## import re
-## import sys
+## TODO: import logging
 
 # Installed modules
 import mezcla
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import system
@@ -29,15 +26,15 @@
     if not omit_warnings:
         system.print_error(f"Warning: {__file__} is not intended as standalone.")
     file_path = system.real_path(gh.dirname(__file__))
     debug.trace(TL.USUAL, f"Version: {mezcla.__VERSION__}")
     debug.trace(TL.USUAL, f"Install path: {file_path}")
 
     # Derive module name
-    # ex: /home/tomohara/python/Mezcla/mezcla/__main__.py => "mezcla"
+    # example: /home/tomohara/python/Mezcla/mezcla/__main__.py => "mezcla"
     module = "<module>"
     sep = my_re.escape(system.path_separator())
     match = my_re.search(fr"([^{sep}]*){sep}[^{sep}]*$", __file__)
     if match:
         module = match.group(1)
     if not omit_warnings:
         system.print_error(f"Likewise for the package (e.g., via 'python -m {module}')\n")
```

### Comparing `mezcla-1.3.9.9/mezcla/analyze_tfidf.py` & `mezcla-1.4.0.0/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/audio.py` & `mezcla-1.4.0.0/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/bash_ast.py` & `mezcla-1.4.0.0/mezcla/bash_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,18 +125,18 @@
 
 def main():
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
     # Show simple usage if --help given
     dummy_main_app = Main(description=__doc__.format(prog=gh.basename(__file__)),
-                          skip_input=False, manual_input=False)
+                          skip_input=False, manual_input=True)
     debug.assertion(dummy_main_app.parsed_args)
 
-    # Prase Bash snippet from stdin
+    # Parse Bash snippet from stdin
     snippet = dummy_main_app.read_entire_input()
     ast = BashAST(snippet)
     print(ast.dump())
     return
     
 #-------------------------------------------------------------------------------
```

### Comparing `mezcla-1.3.9.9/mezcla/bert_multi_classification.py` & `mezcla-1.4.0.0/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/bert_text_classification.py` & `mezcla-1.4.0.0/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/bing_search.py` & `mezcla-1.4.0.0/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/check_html_javascript.py` & `mezcla-1.4.0.0/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/compute_tfidf.py` & `mezcla-1.4.0.0/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/convert_emoticons.py` & `mezcla-1.4.0.0/mezcla/convert_emoticons.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,27 +85,27 @@
         Note:
         - REPLACEMENT can be used for subsituted text (e.g., instead of "").
         - with AUGMENT the emoticon is still included (a la REPLACE plus STRIP).
         """
         # EX: ce.convert("✅ Success") => "[checkmark] Success"
         # EX: ce.convert("✅ Success", augment=True) => "✅ [checkmark] Success"
         # EX: ce.convert("año") => "año"       # ignore diacritic; Spanish for year
-        debug.trace_expr(6, replace, strip, replacement, augment, prefix=f"in ce.convert: text=_; ")
+        debug.trace_expr(6, replace, strip, replacement, augment, prefix="in ce.convert: text=_; ")
         debug.assertion(text is not None)
         debug.assertion(not (replace and strip))
         debug.assertion(not (augment and strip))
         if strip is None:
             strip = self.strip
         if replace is None:
             replace = self.replace
         if replacement is None:
             replacement = self.replacement
         if augment is None:
             augment = self.augment
-        debug.trace_expr(5, replace, strip, replacement, augment, prefix=f"ce.convert: text=_; ")
+        debug.trace_expr(5, replace, strip, replacement, augment, prefix="ce.convert: text=_; ")
         in_text = text
         text = (text or "")
         #
         chars = []
         for ch in text:
             new_ch = ch
             if unicodedata.category(ch) == self.OTHER_SYMBOL:
```

### Comparing `mezcla-1.3.9.9/mezcla/cut.py` & `mezcla-1.4.0.0/mezcla/cut.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # - Add option for specifying output dialect.
 # - Add support for selecting by columns instead of fields (e.g., as with -c1-40 with cut command).
 #
 
 """Extracts columns from a file as with Unix cut command"""
 
 # Standard modules
+import argparse
 import csv
 import re
 import sys
 
 # Installed modules
 ## OLD: import more_itertools
 import functools
@@ -61,27 +62,32 @@
 TAB = "\t"
 SPACE = " "
 COMMA = ","
 ## TODO: make -style suffix optional (e.g., --tab[-style])
 EXCEL_STYLE = "excel-style"             # use Excel dialect for CSV (redundant with default)
 UNIX_STYLE = "unix-style"               # use Unix dialect for CSV (otherwise Excel is used)
 PYSPARK_STYLE = "pyspark-style"         # use PySpark dialect for CSV (otherwise Unix is used)
+## TEMP: workaround problem under MacOS
+FORCE_SINGLE_LINE = system.getenv_bool(
+    "FORCE_SINGLE_LINE", False,
+    description="Force single line quotedchar handling (i.e., non-strict mode)")
 TAB_STYLE = "tab-style"                 # use (non-Excel) tab dialect
 DIALECT = "dialect"                     # --dialect option
 OUTPUT_DIALECT = "output-dialect"       # --output-dialect option
 EXCEL_DIALECT = "excel"                 # dialect parameter for Excel style
 UNIX_DIALECT = "unix"                   # "" for Unix style
 PYSPARK_DIALECT = "pyspark"             # "" for Pyspark style
 SNIFFER_LOOKAHEAD = 65536               # buffer size for guessing dialect (64k)
 TAB_DIALECT = "tab"                     # dialect option for TSV
 SINGLE_LINE = "single-line"             # collapse multi-line fields into one
 MAX_FIELD_LEN = "max-field-len"         # value length before elided
 ## TODO: TODO_ARG = "TODO-arg"          # TODO: comment
 NEW_FIX = system.getenv_bool("NEW_FIX", False,
                              "HACK: Fix for --fix bug")
+NUM_FN_SHORTCUTS = 9
 
 #...............................................................................
 
 MAX_VALUE_LEN = 128
 #
 def elide_values(in_list, max_len=MAX_VALUE_LEN):
     """Elide each of the values in IN_LIST (up to MAX_LEN each).
@@ -144,15 +150,16 @@
 #
 # note: Uses hive as alias for pyspark.
 csv.register_dialect("hive", pyspark_dialect)
 
 class tab_dialect(csv.Dialect):
     """TSV module dialect for tab-separated values (non-Excel)."""
     delimiter = TAB
-    quotechar = ''               # default of '"' leads to multiline rows
+    ## OLD: quotechar = ''               # default of '"' leads to multiline rows
+    quotechar = ('"' if not FORCE_SINGLE_LINE else '')
     doublequote = False          # uses escaped double quote when embedded
     # TODO: use special Unicode space-like character
     escapechar = '\\'
     skipinitialspace = False     # keep leaing space afer delimiter
     lineterminator = '\n'
     quoting = csv.QUOTE_NONE     # no special processing for quotes
 #
@@ -180,21 +187,28 @@
     def setup(self):
         """Check results of command line processing"""
         # Note: The defaults above might be changed based on other arguments;
         # but, the user-specified value is normally not overridden.
         debug.trace_fmtd(5, "Script.setup(): self={s}", s=self)
 
         # Check main options
+        # note: several options regarding fields including --Fn aliases
         ## OLD: fields = self.get_parsed_option(FIELDS, self.fields)
-        fields = self.get_parsed_option(F_OPT, ",".join(self.fields))
+        for i in range(NUM_FN_SHORTCUTS):
+            if self.get_parsed_option(f"F{i + 1}"):
+                self.fields.append(str(i + 1))
+        FIELDS_DEFAULT = ",".join(self.fields)
+        debug.trace_expr(4, FIELDS_DEFAULT)
+        fields = self.get_parsed_option(F_OPT, FIELDS_DEFAULT)
         fields = self.get_parsed_option(FIELDS, fields)
         if fields:
             self.fields = self.parse_field_spec(fields)
         self.all_fields = self.get_parsed_option(ALL_FIELDS, (not fields))
         debug.assertion(not (self.fields and self.all_fields))
+        #
         self.fix = self.get_parsed_option(FIX, self.fix)
 
         # Check delimiter options
         # Note: output delimiter defaults to input unless convert specified
         self.csv = self.get_parsed_option(CSV, self.csv)
         if self.csv:
             self.delimiter = COMMA
@@ -434,28 +448,31 @@
     debug.trace_fmt(4, "Environment options: {eo}",
                     eo=system.formatted_environment_option_descriptions())
     app = Script(
         description=__doc__,
         skip_input=False,
         manual_input=True,
         multiple_files=True,
-        boolean_options=[(CSV, "Comma-separated values ({xls} as per csv module)".format(xls=EXCEL_STYLE)),
-                         (TSV, "Tab-separated values"),
-                         OUTPUT_CSV, OUTPUT_TSV,
-                         (CONVERT_DELIM, "Convert csv to tsv (or vice versa)"),
-                         (SNIFFER_ARG, "Detect csv dialect by lookahead (file-input only)"),
-                         ## TODO: INPUT_CSV, OUTPUT_CSV, INPUT_TSV, OUTPUT_TSV,
-                         (FIX, "Fix up sloppy input (e.g., multiple spaces into tab)--csv fixup not yet supported"),
-                         (ALL_FIELDS, "Alternative to {f} option".format(f=FIELDS)),
-                         (EXCEL_STYLE, "Use Excel conventions for CSV files (see csv python package docs)"),
-                         (PYSPARK_STYLE, "Use PySpark conventions for CSV files (see {f} source)".format(f=__file__)),
-                         (SINGLE_LINE, "Remove embedded newlines from mult-line fields"),
-                         (TAB_STYLE, "Non-excel TSV conventions (default)"),
-                         ## (TODO_ARG, "TODO: arg desc").
-                         (UNIX_STYLE, "Use Unix conventions for CSV files (see csv python package docs)")],
+        boolean_options=(
+            [("Fn", "alias for --field n")] +
+            [(f"F{i + 1}", argparse.SUPPRESS) for i in range(NUM_FN_SHORTCUTS)] +
+            [(CSV, "Comma-separated values ({xls} as per csv module)".format(xls=EXCEL_STYLE)),
+             (TSV, "Tab-separated values"),
+             OUTPUT_CSV, OUTPUT_TSV,
+             (CONVERT_DELIM, "Convert csv to tsv (or vice versa)"),
+             (SNIFFER_ARG, "Detect csv dialect by lookahead (file-input only)"),
+             ## TODO: INPUT_CSV, OUTPUT_CSV, INPUT_TSV, OUTPUT_TSV,
+             (FIX, "Fix up sloppy input (e.g., multiple spaces into tab)--csv fixup not yet supported"),
+             (ALL_FIELDS, "Alternative to {f} option".format(f=FIELDS)),
+             (EXCEL_STYLE, "Use Excel conventions for CSV files (see csv python package docs)"),
+             (PYSPARK_STYLE, "Use PySpark conventions for CSV files (see {f} source)".format(f=__file__)),
+             (SINGLE_LINE, "Remove embedded newlines from mult-line fields"),
+             (TAB_STYLE, "Non-excel TSV conventions (default)"),
+             ## (TODO_ARG, "TODO: arg desc").
+             (UNIX_STYLE, "Use Unix conventions for CSV files (see csv python package docs)")]),
         int_options = [(MAX_FIELD_LEN, "Maximum length per field")],
         text_options=[(DELIM, "Input field separator"),
                       (DIALECT, "CSV module dialect: standard (i.e., excel, excel-tab, or unix) or adhoc (e.g., pyspark, hive)"),
                       (OUTPUT_DIALECT, "dialect for output--defaults to input one"),
                       (FIELDS, "Field specification (1-based): single column, range of columns, or comma-separated columns"),
                       (F_OPT, "Alias for --fields"),
                       (OUT_DELIM, "Output field separator")])
```

### Comparing `mezcla-1.3.9.9/mezcla/data_utils.py` & `mezcla-1.4.0.0/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/debug.py` & `mezcla-1.4.0.0/mezcla/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 import os
 from pprint import pprint
 import re
 ## OLD: from xml.dom.minidom import Element
 import six
 import sys
 import time
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Local packages
 ## OLD:
 ## # note: The following redefines sys.version_info to be python3 compatible;
 ## # this is used in _to_utf8, which should be reworked via six-based wrappers.
 ## import mezcla.sys_version_info_hack      # pylint: disable=unused-import
 
@@ -475,14 +476,16 @@
         - Use MAX_LEN to specify maximum value length ({max_len}).
         - Use PREFIX to specify initial trace output (e.g., for function call tracing).
         - Use SUFFIX to specify final value to be printed (e.g., for perlish para grep over multi-line trace).
         - See misc_utils.trace_named_objects for similar function taking string input, which is more general but harder to use and maintain"""
         trace_fmt(MOST_VERBOSE, "trace_expr({l}, a={args}, kw={kw}); debug_level={dl}",
                   l=level, args=values, kw=kwargs, dl=trace_level)
         ## TODO1: check for unknown keywords, which could be cut-n-paste error
+        ## TODO2: try to handle numpy arrays better; ex: 'arr=array([[11, 12],\n       [21, 22]])'
+        ##        => 'arr=array([[11, 12], [21, 22]])'
         ## EX (from convert_emoticons.py): debug.trace_expr(7, replace=None, strip=None, replacement=None, text=None, prefix="in ConvertEmoticons.__init__: ")
         ## DEBUG:
         ## trace_fmt(1, "(global_trace_level:{g} < level:{l})={v}",
         ##           g=trace_level, l=level, v=(trace_level < level))
         if (trace_level < level):
             # note: Short-circuits processing to avoid errors about known problems (e.g., under ipython)
             return
@@ -1092,15 +1095,15 @@
         open_debug_file()
         return
                         
 
     def debug_init():
         """Debug-only initialization"""
         time_start = time.time()
-        trace(DETAILED, f"in debug_init(); {timestamp()}")
+        trace(DETAILED, f"in debug_init(); DEBUG_LEVEL={trace_level}; {timestamp()}")
         ## DEBUG: trace_values(8, inspect.stack(), max_len=256)
         # note: shows command invocation unless invoked via "python -c ..."
         command_line = " ".join(sys.argv)
         assertion(command_line)
         if (command_line and (command_line != "-c") and (command_line != "-m")):
             # TODO2: simplify misc. trace suppression options (n.b., check shellscript repo)
             if _getenv_bool("TRACE_INVOCATION", False):
@@ -1116,14 +1119,15 @@
         ##                      in ["1", "TRUE"])
         output_timestamps = _getenv_bool("OUTPUT_DEBUG_TIMESTAMPS", False)
     
         # Show startup time and tracing info
         module_file = __file__
         trace_fmtd(DETAILED, "[{f}] loaded at {t}", f=module_file, t=timestamp())
         trace_fmtd(DETAILED, "trace_level={l}; output_timestamps={ots}", l=trace_level, ots=output_timestamps)
+        trace_expr(QUITE_DETAILED, __file__)
 
         # Determine other debug-only environment options
         global para_mode_tracing
         para_mode_tracing = _getenv_bool("PARA_MODE_TRACING", para_mode_tracing)
         global max_trace_value_len
         max_trace_value_len = _getenv_int("MAX_TRACE_VALUE_LEN", max_trace_value_len)
         global use_logging
```

### Comparing `mezcla-1.3.9.9/mezcla/docs/audio_uml.svg` & `mezcla-1.4.0.0/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/evaluate_example_tests.py` & `mezcla-1.4.0.0/mezcla/evaluate_example_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,42 +12,40 @@
 Convert example comments in Python scource to doctest format and evaluate.
 
 Sample usage:
    {script} text_utils.py
 """
 
 # Standard modules
-from types import ModuleType
+from types import ModuleType            # pylint: disable=unused-import
 
 # Installed modules
 ## TODO2: import ast_tools
 
 # Local modules
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.main import Main
 from mezcla.my_regex import my_re
 from mezcla import system
 
-# Constants for switches omitting leading dashes
-OUTPUT_ARG = "output"
+# Constants for switches, omitting leading dashes
+OUTPUT_ARG = "output"                   # TODO: => just-output
 
 # Constants
 TL = debug.TL
 
 # Environment options
-# Note: These are just intended for internal options, not for end users.
-# It also allows for enabling options in one place rather than four
-# (e.g., [Main member] initialization, run-time value, and argument spec., along
-# with string constant definition).
-# WARNING: To minimize environment comflicts with other programs make the names
-# longer such as two or more tokens (e.g., "FUBAR" => "FUBAR_LEVEL").
-#
-TODO_FUBAR = system.getenv_bool("TODO_FUBAR", False,
-                                description="TODO:Fouled Up Beyond All Recognition processing")
+SKIP_BACKGROUND = system.getenv_bool(
+    "SKIP_BACKGROUND", False,
+    description="Skip example tests involving background jobs")
+NORMALIZE_RESULT = system.getenv_bool(
+    "NORMALIZE_RESULT", False,
+    description="Normalize result to acount for doctest quirks as with quotes")
+
 
 class TestConverter:
     """Class to convert example EX-style comments into doctest text format"""
 
     def __init__(self):
         """Initializer"""
         debug.trace_fmtd(TL.VERBOSE, "Helper.__init__(): self={s}", s=self)
@@ -63,78 +61,90 @@
     def add_module(self, module_spec):
         """Add import-* spec from MODULE_SPEC"""
         # pylint: disable=eval-used,exec-used
         ## TODO2: debug.assertion(eval("isintance(eval({module_spec!r}, module)"))
         exec(f"import {module_spec}")
         debug.assertion(eval(f"isinstance({module_spec}, ModuleType)"))
         self.test_text += f">>> from {module_spec} import *\n\n"
-    
+
     def convert(self, line, line_num):
         """Convert example test in LINE at LINE_NUM"""
         expression = result = None
         OK = False
-        if my_re.search(r"EX: (.*) => (.*)", line):
+
+        # Parse test expression
+        if my_re.search(r"EX: (.*)\s*=>\s*(.*)", line):
             expression, result = my_re.groups()
             OK = True
         elif my_re.search(r"EX: (.*)", line):
             expression = my_re.group(1)
             result = "True"
             OK = True
         else:
             pass
-        if ((expression is None) and (result is None)):
+
+        # Exclude certain commands
+        if expression and SKIP_BACKGROUND and my_re.search(r"run|issue(.*&)", expression):
+            debug.trace(4, f"Ignoring invocation of background job at {line_num}: {line}")
+            OK = False
+
+        # Normalize result
+        ## TODO3: my_re.search(r'^".*[^"].*"$', result)
+        if result and NORMALIZE_RESULT and my_re.search(r'^".*"$', result):
+            result = f'{result[1:-1]}'
+
+        # Add to tests
+        if ((not OK) or ((expression is None) and (result is None))):
             debug.trace(6, f"Ignoring line {line_num}: {line}")
         else:
             self.test_text += f">>> {expression.strip()}\n{result.strip()}\n\n"
         return OK
 
 
 class Script(Main):
     """Input processing class"""
     output_arg = False
     exc = None
+    num_tests = 0
 
     def setup(self):
         """Check results of command line processing"""
         debug.trace_fmtd(TL.VERBOSE, "Script.setup(): self={s}", s=self)
-        ## TODO: extract argument values
         self.output_arg = self.get_parsed_option(OUTPUT_ARG, self.output_arg)
-        ## TODO:
-        ## self.text_arg = self.get_parsed_option(TEXT_ARG, self.text_arg)
-        ## self.alt_filename = self.get_parsed_argument(ALT_FILENAME)
         self.exc = TestConverter()
         module = gh.basename(self.filename, ".py")
         self.exc.add_module(module)
         debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
 
     def process_line(self, line):
         """Processes current line looking for EX comments and converting"""
         debug.trace_fmtd(TL.QUITE_DETAILED, "Script.process_line({l})", l=line)
-        self.exc.convert(line, self.line_num)
+        ok = self.exc.convert(line, self.line_num)
+        if ok:
+            self.num_tests += 1
 
     def wrap_up(self):
         """Output the final set of tests"""
         debug.trace_fmtd(TL.VERBOSE, "Script.wrap_up(): self={s}", s=self)
         test_spec = self.exc.get_tests()
         if self.output_arg:
             print(test_spec)
-        else:
+        elif self.num_tests:
             system.write_file(self.temp_file, test_spec)
-            print(gh.run("python -m doctest -v {self.temp_file}"))
+            print(gh.run(f"python -m doctest -v {self.temp_file}"))
+        else:
+            debug.trace(4, "FYI: No tests extracted")
         
 def main():
     """Entry point"""
     app = Script(
         description=__doc__.format(script=gh.basename(__file__)),
-        skip_input=False,
-        manual_input=False,
-        boolean_options=[(OUTPUT_ARG, "Output converted tests without running")],
-        float_options=None)
+        skip_input=False, manual_input=False,
+        boolean_options=[(OUTPUT_ARG, "Output converted tests without running")])
     app.run()
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_VERBOSE)
     debug.trace(5, f"module __doc__: {__doc__}")
-    debug.assertion("TODO:" not in __doc__)
     main()
```

### Comparing `mezcla-1.3.9.9/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.4.0.0/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.4.0.0/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/consume_all_memory.py` & `mezcla-1.4.0.0/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/download_user_gist.py` & `mezcla-1.4.0.0/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/dump_checkpoints.py` & `mezcla-1.4.0.0/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/encoded-iris.csv` & `mezcla-1.4.0.0/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/feature_importance.py` & `mezcla-1.4.0.0/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.4.0.0/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/hf_stable_diffusion.py` & `mezcla-1.4.0.0/mezcla/examples/hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.4.0.0/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/hugging_face_translation.py` & `mezcla-1.4.0.0/mezcla/examples/hugging_face_translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     MT_TASK = f"translation_{source_lang}_to_{target_lang}"                 # pylint: disable=invalid-name
     MT_MODEL = f"Helsinki-NLP/opus-mt-{source_lang}-{target_lang}"          # pylint: disable=invalid-name
     mt_task = dummy_app.get_parsed_option(TASK_ARG, MT_TASK)
     mt_model = dummy_app.get_parsed_option(MODEL_ARG, MT_MODEL)
     use_interface = dummy_app.get_parsed_option(UI_ARG, USE_INTERFACE)
 
     # Get input file
+    debug.trace_expr(5, dummy_app.input_stream, text, TEXT_FILE)
     text_file = TEXT_FILE
     if ((text is not None) or use_interface):
         pass
     elif text_file == "-":
         text_file = dummy_app.temp_file
         text = dummy_app.read_entire_input()
     else:
```

### Comparing `mezcla-1.3.9.9/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.4.0.0/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/iris.csv` & `mezcla-1.4.0.0/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.4.0.0/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/plot_forest_importances.py` & `mezcla-1.4.0.0/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/resources/translate_es_25.txt` & `mezcla-1.4.0.0/mezcla/examples/resources/translate_es_25.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/resources/us1.wav` & `mezcla-1.4.0.0/mezcla/examples/resources/us1.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/resources/us10.wav` & `mezcla-1.4.0.0/mezcla/examples/resources/us10.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/sd-spooky-pacman.png` & `mezcla-1.4.0.0/mezcla/examples/sd-spooky-pacman.png`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.4.0.0/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/template.py` & `mezcla-1.4.0.0/mezcla/examples/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from mezcla.main import Main
 ## TODO: from mezcla.my_regex import my_re
 from mezcla import system
 ## TODO2: streamline imports by exposing common functions, etc. in mezcla
 
 # Constants
 TL = debug.TL
-## TODO: TODO_OPT1 = "todo-option1"
+## TODO: TODO_BOOL_OPT1 = "todo-bool-option1"
+## TODO: TODO_TEXT_OPT1 = "todo-text-option1"
 
 ## TODO:
 ## # Environment options
 ## # Notes:
 ## # - These are just intended for internal options, not for end users.
 ## # - They also allow for enabling options in one place rather than four
 ## #   when using main.Main (e.g., [Main member] initialization, run-time
@@ -46,15 +47,16 @@
 def main():
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
     # Parse command line options, show usage if --help given
     # TODO: manual_input=True; short_options=True
     main_app = Main(description=__doc__.format(script=gh.basename(__file__)),
-                    ## TODO: boolean_options=[(TODO_OPT1, "TODO desc1")]
+                    ## TODO: boolean_options=[(TODO_BOOL_OPT1, "TODO desc1")]
+                    ## TODO: boolean_options=[(TODO_TEXT_OPT1, "TODO desc1")]
                     skip_input=False)
     debug.assertion(main_app.parsed_args)
     ## TODO_OPT1 = main_app.get_parsed_option(TODO_OPT1)
 
     ## TODO:
     system.print_error("Error: Implement me!")
     ## ALT TODO:
```

### Comparing `mezcla-1.3.9.9/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.4.0.0/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/tests/test_hf_stable_diffusion.py` & `mezcla-1.4.0.0/mezcla/examples/tests/test_hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_speechrec.py` & `mezcla-1.4.0.0/mezcla/examples/tests/test_hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_translation.py` & `mezcla-1.4.0.0/mezcla/examples/tests/test_hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/tests/test_youtube_transcript.py` & `mezcla-1.4.0.0/mezcla/examples/tests/test_youtube_transcript.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 #! /usr/bin/env python
 #
-# TODO: Test(s) for ../<module>.py
+# Test(s) for ../youtube_transcript.py
 #
 # Notes:
-# - Fill out TODO's below. Use numbered tests to order (e.g., test_1_usage).
-# - * See test_python_ast.py for simple example of customization.
-# - TODO: If any of the setup/cleanup methods defined, make sure to invoke base
-#   (see examples below for setUp and tearDown).
-# - For debugging the tested script, the ALLOW_SUBCOMMAND_TRACING environment
-#   option shows tracing output normally suppressed by unittest_wrapper.py.
-# - This can be run as follows:
-#   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_<module>.py
+# - This can be run as follows (e.g., from repo base dir):
+#   $ pytest ./mezcla/examples/tests/test_youtube_transcript.py
 #
 #................................................................................
 # Sample test:
 #
 #   [via https://www.youtube.com/watch?v=E9yhGw66v2Q]
 #   0:51        good morning mr. lover I thought I'd
 #   0:57        find you out here how long have you been
@@ -25,15 +19,15 @@
 #   20:30       the neighborhood then they're gonna have
 #   20:33       to struggle and work hard is that
 #   20:35       Dickens to make sure they they win and
 #   20:39       they can win all you gotta do is do it
 #   22:25       you
 #   
    
-"""TODO: Tests for <module> module"""
+"""Tests for youtube_transcript module"""
 
 # Standard modules
 ## TODO: from collections import defaultdict
 
 # Installed modules
 import pytest
```

### Comparing `mezcla-1.3.9.9/mezcla/examples/tracemalloc_display.py` & `mezcla-1.4.0.0/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/examples/youtube_transcript.py` & `mezcla-1.4.0.0/mezcla/examples/youtube_transcript.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     debug.assertion(main_app.parsed_args)
     url = main_app.filename
     video_id= url
     YOUTUBE_PREFIX = "https://www.youtube.com/watch?v="
     if url.startswith(YOUTUBE_PREFIX):
         video_id = url[len(YOUTUBE_PREFIX):]
     else:
+        debug.assertion("youtube.com" not in url)
         url = YOUTUBE_PREFIX + url
     ## TODO: video_id = my_re.sub(r"(https://)?www.youtube.com/watch\?v=", "", main_app.filename)
     debug.trace_expr(5, url, video_id)
 
     # Download the transcript and print using YouTubeLike-format
     # note: youtube_transcript_api
     print(misc_utils.get_formatted_date())
```

### Comparing `mezcla-1.3.9.9/mezcla/extract_document_text.py` & `mezcla-1.4.0.0/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/file_utils.py` & `mezcla-1.4.0.0/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/filter_random.py` & `mezcla-1.4.0.0/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/format_profile.py` & `mezcla-1.4.0.0/mezcla/format_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,30 +46,36 @@
 # Standard packages
 import sys
 import pstats
 
 # Local packages
 from mezcla import debug
 ## OLD: from tpo_common import *
-from mezcla.system import getenv_text, print_stderr
+from mezcla.system import getenv_bool, getenv_text, print_stderr
 
 ## OLD: PROFILE_KEY = getenv_text("PROFILE_KEY", "cumulative")
-PROFILE_KEY = getenv_text("PROFILE_KEY", "cumulative",
-                          "Sort key (e.g., cumtime, filename, ncalls, tottime)")
+PROFILE_KEY = getenv_text(
+    "PROFILE_KEY", "cumulative",
+    desc="Sort key (e.g., cumtime, filename, ncalls, tottime)")
+FULL_PATH = getenv_bool(
+    "FULL_PATH", False,
+    desc="Show full path in filename field")
 
 #------------------------------------------------------------------------
 # Functions
 
 def usage():
     """Displays usage notes for script"""
     print_stderr("""
 
 Usage: {program} profile-log
 
 Notes:
+- use FULL_PATH to include directoy for filename
+  (e.g., helps to resolve all those __init__.py entries)
 - use PROFILE_KEY to over default sorting (cumulative)
 - main keys: 
        cumtime, filename, ncalls, tottime
 - other keys: 
        module, pcalls, line, name, nfl, stdname
 - alternative keys:
        calls, cumulative, file, time
@@ -90,14 +96,16 @@
     if ((len(sys.argv) < 2) or (sys.argv[1] == "--help")):
         usage()
         sys.exit()
     file = sys.argv[1]
 
     # Generate listing and sort by cumulative time
     p = pstats.Stats(file)
-    p.strip_dirs().sort_stats(PROFILE_KEY).print_stats()
+    if not FULL_PATH:
+        p = p.strip_dirs()
+    p.sort_stats(PROFILE_KEY).print_stats()
     return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     main()
```

### Comparing `mezcla-1.3.9.9/mezcla/gensim_test.py` & `mezcla-1.4.0.0/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/glue_helpers.py` & `mezcla-1.4.0.0/mezcla/glue_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 # NOTE:
 # - Some of the utilities are specific to Unix (e.g., full_mkdir and real_path). In
 #   contrast, system.py attempts to be more cross platform.
 # - ** It can be confusing debugging script that use run, because the trace level
 #  is raised by default. To disable this, set the SUB_DEBUG_LEVEL as follows:
 #     l=5; DEBUG_LEVEL=$l SUB_DEBUG_LEVEL=$l merge_files.py ...
 # - Also see ALLOW_SUBCOMMAND_TRACING usage below and in unittest_wrapper.py.
+# - By default, temporary files are created in the system temporary directory. To
+#   facilate debugging, two environment variables allow for overriding this
+#      TEMP_FILE: fixed temporary file to use
+#      TEMP_BASE: basename for temporary files (or a directory if USE_TEMP_BASE_DIR)
 #
 # TODO:
 # - Add more functions to facilitate command-line scripting (check bash scripts for commonly used features).
 # - Add functions to facilitate functional programming (e.g., to simply debugging traces).
 #
 
 """Helpers gluing scripts together
@@ -39,14 +43,17 @@
 
 # Local packages
 from mezcla import debug
 from mezcla import system
 from mezcla import tpo_common as tpo
 ## OLD: from mezcla.tpo_common import debug_format, debug_print, print_stderr, setenv
 from mezcla.tpo_common import debug_format, debug_print
+## OLD: from mezcla.main import DISABLE_RECURSIVE_DELETE
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
+## TODO3: debug.trace_expr(6, __file__)
 
 # Constants
 TL = debug.TL
 
 # Environment options
 #
 # note:
@@ -89,42 +96,66 @@
     "TEMP_BASE", None,
     description="Override for temporary file basename")
 TEMP_BASE_DIR_DEFAULT = (TEMP_BASE and
                          (system.is_directory(TEMP_BASE) or TEMP_BASE.endswith("/")))
 USE_TEMP_BASE_DIR = system.getenv_bool(
     "USE_TEMP_BASE_DIR", TEMP_BASE_DIR_DEFAULT,
     description="Whether TEMP_BASE should be a dir instead of prefix")
+DISABLE_RECURSIVE_DELETE = system.getenv_value(
+    "DISABLE_RECURSIVE_DELETE", None,
+    description="Disable use of potentially dangerous rm -r style recursive deletions")
+PRESERVE_TEMP_FILE = system.getenv_value(
+    "PRESERVE_TEMP_FILE", None,
+    desc="Retain value of TEMP_FILE even if TEMP_BASE set--see INFER_TEMP_FILE")
 
 # Globals
-# note: see init() for initialization
+# note:
+# - see init() for main initialization;
+# - these are placeholds until module initialized
+# - os.path.join used to likewise avoid chick-n-egg problems with init
+# - TEMP_FILE is normally None to indicate use of random temp file name
+# - TEMP_LOG_FILE and TEMP_SCRIPT_FILE are used in run, issue, etc.
+TMP = system.getenv_text(
+    "TMP", "/tmp",
+    description="Temporary directory")
+PID = system.get_process_id()
 TEMP_FILE = None
+GLOBAL_TEMP_FILE = os.path.join(TMP, f"temp-{PID}")
+TEMP_LOG_FILE = os.path.join(TMP, f"{GLOBAL_TEMP_FILE}.log")
+TEMP_SCRIPT_FILE = os.path.join(TMP, f"{GLOBAL_TEMP_FILE}.script")
 
 #------------------------------------------------------------------------
 
 def get_temp_file(delete=None):
     """Return name of unique temporary file, optionally with DELETE"""
     # Note: delete defaults to False if detailed debugging
     # TODO: allow for overriding other options to NamedTemporaryFile
     if ((delete is None) and debug.detailed_debugging()):
         delete = False
     temp_file_name = (TEMP_FILE or tempfile.NamedTemporaryFile(**NTF_ARGS).name)
     debug.assertion(not delete, "Support for delete not implemented")
     debug_format("get_temp_file() => {r}", 5, r=temp_file_name)
     return temp_file_name
-#
-TEMP_LOG_FILE = system.getenv_text("TEMP_LOG_FILE", get_temp_file() + "-log",
-                                "Log file for stderr such as for issue function")
-TEMP_SCRIPT_FILE = system.getenv_text("TEMP_SCRIPT_FILE", get_temp_file() + "-script",
-                                   "File for command invocation")
+
+
+def get_temp_dir(delete=None):
+    """Gets temporary file to use as a directory
+    note: Optionally DELETEs directory afterwards
+    """
+    debug.assertion(False, "work-in-progress implementation")
+    temp_dir_path = get_temp_file(delete=delete)
+    full_mkdir(temp_dir_path)
+    return temp_dir_path
+
 
 def create_temp_file(contents, binary=False):
     """Create temporary file with CONTENTS and return full path"""
     temp_filename = get_temp_file()
     system.write_file(temp_filename, contents, binary=binary)
-    debug.trace(6, "create_temp_file({contents!r}) => {temp_filename}")
+    debug.trace(6, f"create_temp_file({contents!r}) => {temp_filename}")
     return temp_filename
 
 
 def basename(filename, extension=None):
     """Remove directory from FILENAME along with optional EXTENSION, as with Unix basename command. Note: the period in the extension must be explicitly supplied (e.g., '.data' not 'data')"""
     # EX: basename("fubar.py", ".py") => "fubar"
     # EX: basename("fubar.py", "py") => "fubar."
@@ -208,15 +239,15 @@
             try:
                 frame = inspect.currentframe().f_back
                 calling_filename = frame.f_globals['__file__']
                 base_dir = os.path.dirname(calling_filename)
                 debug.trace_expr(4, calling_filename, base_dir)
             except (AttributeError, KeyError):
                 base_dir = ""
-                debug_print("Exception during resolve_path: " + str(sys.exc_info()), 5)
+                debug_print("Error: Exception during resolve_path: " + str(sys.exc_info()), 5)
             finally:
                 if frame:
                     del frame
         
         # Check calling directory (TODO2: add more check dirs such as children)
         dirs_to_check = [base_dir]
         if heuristic:
@@ -226,42 +257,43 @@
             if os.path.exists(check_path):
                 path = check_path
                 break
     # Fall back to using find command
     if (not os.path.exists(path)) and heuristic:
         debug.trace(4, "FYI: resolve_path falling back to find")
         debug.assertion(" " not in path)
-        path = run(f"find {base_dir} -name '{path}'")
+        debug.assertion(base_dir)
+        path = run(f"find {base_dir or '.'} -name '{path}'")
             
     debug_format("resolve_path({f}) => {p}", 4, f=filename, p=path)
     return path
 
 
 def form_path(*filenames, create=False):
     """Wrapper around os.path.join over FILENAMEs (with tracing)
     Note: includes sanity check about absolute filenames except for first
     If CREATE, then the directory for the path is created if needed
     Warning: This might be deprecated: use system.form_path instead.
     """
     ## TODO3: return system.form_path(*filenames)
     debug.assertion(not any(f.startswith(system.path_separator()) for f in filenames[1:]))
     if create:
-        path_dir = os.path.join(filenames[:-1])
+        path_dir = os.path.join(*filenames[:-1])
         if not system.file_exists(path_dir):
             full_mkdir(path_dir)
 
     path = os.path.join(*filenames)
     debug_format("form_path{f} => {p}", 6, f=tuple(filenames), p=path)
     return path
 
 
 def is_directory(path):
-    """Determins wther PATH represents a directory"""
+    """Determines whether PATH represents a directory"""
     is_dir = os.path.isdir(path)
-    debug_format("is_dir{p} => {r}", 6, p=path, r=is_dir)
+    debug_format("is_dir({p}) => {r}", 6, p=path, r=is_dir)
     return is_dir
 
 
 ## TODO2: add decorator for flagging obsolete functions
 ##   def obsolete():
 ##      """Flag fucntion as obsolete in docstring and issue warning if called"""
 ##      warning = f"Warning {func} obsolete use version in system.py instead"
@@ -279,18 +311,22 @@
         debug_format("os.mkdir({p})", 6, p=path)
     else:
         debug.assertion(os.path.isdir(path))
     return
 
 
 def full_mkdir(path):
-    """Issues mkdir to ensure path directory, including parents (assuming Linux like shell)"""
+    """Issues mkdir to ensure path directory, including parents (assuming Linux like shell)
+    Note: Doesn't handle case when file exists but is not a directory
+    """
+    debug.trace(6, f"full_mkdir({path!r})")
     ## TODO: os.makedirs(path, exist_ok=True)
     debug.assertion(os.name == "posix")
-    issue('mkdir --parents "{p}"', p=path)
+    if not system.file_exists(path):
+        issue('mkdir --parents "{p}"', p=path)
     debug.assertion(is_directory(path))
     return
 
 
 def real_path(path):
     """Return resolved absolute pathname for PATH, as with Linux realpath command
     Note: Use version in system instead"""
@@ -386,28 +422,27 @@
     # TODO: make sure no template markers left in command text (e.g., "tar cvfz {tar_file}")
     # EX: "root" in run("ls /")
     # Note: Script tracing controlled DEBUG_LEVEL environment variable.
     debug.assertion(isinstance(trace_level, int))
     debug.trace(trace_level + 2, f"run({command}, tl={trace_level}, sub_tr={subtrace_level}, iss={just_issue}, out={output}")
     global default_subtrace_level
     # Keep track of current debug level setting
-    debug_level_env = None
+    debug_level_env = os.getenv("DEBUG_LEVEL")
     if subtrace_level is None:
         subtrace_level = default_subtrace_level
     if subtrace_level != trace_level:
-        debug_level_env = os.getenv("DEBUG_LEVEL")
         system.setenv("DEBUG_LEVEL", str(subtrace_level))
     in_just_issue = just_issue
     if just_issue is None:
         just_issue = False
     save_temp_base = TEMP_BASE
     if TEMP_BASE:
          system.setenv("TEMP_BASE", TEMP_BASE + "_subprocess_")
     save_temp_file = TEMP_FILE
-    if TEMP_FILE:
+    if TEMP_FILE and (PRESERVE_TEMP_FILE is not True):
         system.setenv("TEMP_FILE", TEMP_FILE + "_subprocess_")
     # Expand the command template
     # TODO: make this optional
     command_line = command
     if re.search("{.*}", command):
         command_line = tpo.format(command_line, indirect_caller=True, ignore_exception=False, **namespace)
     debug_print("issuing: %s" % command_line, trace_level)
@@ -430,20 +465,18 @@
     wait_for_command = (foreground_wait and not just_issue)
     debug.trace_expr(5, foreground_wait, just_issue, wait_for_command)
     ## TODO3: clarify what output is when stdout redirected (e.g., for issue in support of unittest_wrapper.run_script
     result = getoutput(command_line) if wait_for_command else str(os.system(command_line))
     if output:
         print(result)
     # Restore debug level setting in environment
-    if debug_level_env:
-        system.setenv("DEBUG_LEVEL", debug_level_env)
-    if save_temp_base:
-        system.setenv("TEMP_BASE", save_temp_base)
-    if save_temp_file:
-        system.setenv("TEMP_FILE", save_temp_file)
+    system.setenv("DEBUG_LEVEL", debug_level_env or "")
+    system.setenv("TEMP_BASE", save_temp_base or "")
+    if save_temp_file and (PRESERVE_TEMP_FILE is not True):
+        system.setenv("TEMP_FILE", save_temp_file or "")
     debug_print("run(_) => {\n%s\n}" % indent_lines(result), (trace_level + 1))
     return result
 
 
 def run_via_bash(command, trace_level=4, subtrace_level=None, init_file=None,
                  enable_aliases=False,
                  **namespace):
@@ -700,14 +733,33 @@
     shutil.copy(source, target)
     target_file = (target if system.is_regular_file(target) else form_path(target, basename(source)))
     ## TODO: debug.assertion(file_size(source) == file_size(target_file))
     debug.assertion(non_empty_file(target_file))
     return
 
 
+def copy_directory(source, dest):
+    """copy SOURCE dir to DEST dir"""
+    # Note: meta data is not copied (e.g., access control lists)); see
+    #    https://docs.python.org/3/library/shutil.html
+    debug.trace_fmt(5, f'copy_directory({source}, {dest})')
+
+    def non_empty_directory(path):
+        """Whether PATH exists and is not empty"""
+        size = len(get_directory_listing(path)) if is_directory(path) else -1
+        non_empty = size > 0
+        debug.trace_fmt(5, f'non_empty_directory({path}) => {non_empty} (files={size})')
+        return non_empty
+    
+    debug.assertion(non_empty_directory(source))
+    dest_path = shutil.copytree(src=source, dst=dest)
+    debug.assertion(len(get_directory_listing(source)) == len(get_directory_listing(dest_path)))
+    debug.assertion(non_empty_directory(dest_path))
+
+
 def rename_file(source, target):
     """Rename SOURCE file as TARGET file"""
     # TODO: have option to skip if target exists
     debug_print("rename_file(%s, %s)" % (tpo.normalize_unicode(source), tpo.normalize_unicode(target)), 5)
     debug.assertion(non_empty_file(source))
     debug.assertion(source != target)
     os.rename(source, target)
@@ -732,14 +784,31 @@
     """Deletes FILENAME if it exists and is not a directory or other special file"""
     ok = False
     if file_exists(filename):
         ok = delete_file(filename)
     tpo.debug_format("delete_existing_file({f}) => {r}", 5, f=filename, r=ok)
     return ok
 
+def delete_directory(path):
+    """Deletes PATH"""
+    debug.trace_fmt(5, f"delete_directory({path})")
+    ok = False
+    try:
+        if DISABLE_RECURSIVE_DELETE:
+            debug.trace(4, f"FYI: Only deleting top-level files in {path} to avoid potentially dangerous rm -r")
+            run(f"rm -vf {path}/* {path}/.*")
+            run(f"rm -vf {path}")
+            ok = None
+        else:
+            debug.trace(4, f"FYI: Using potentially dangerous rm -r over {path}")
+            run(f"rm -rvf {path}")
+            ok = None
+    except OSError:
+        debug.trace_fmt(5, f"Exception during deletion of {path}: {system.get_exception()}")
+    return ok
 
 def file_size(filename):
     """Returns size of FILENAME in bytes (or -1 if not found)"""
     size = -1
     if os.path.exists(filename):
         size = os.path.getsize(filename)
     tpo.debug_format("file_size({f}) => {s}", 5, f=filename, s=size)
@@ -855,20 +924,43 @@
         return
 
 def init():
     """Work around for Python quirk"""
     # See https://stackoverflow.com/questions/1590608/how-do-i-forward-declare-a-function-to-avoid-nameerrors-for-functions-defined
     debug.trace(5, "glue_helpers.init()")
     global TEMP_FILE
-    temp_filename = "temp-file.list"
+    ## OLD: temp_filename = "temp-file.list"
+    temp_filename = f"temp-{PID}.list"
     if USE_TEMP_BASE_DIR and TEMP_BASE:
         full_mkdir(TEMP_BASE)
-    temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}")
-    TEMP_FILE = system.getenv_value("TEMP_FILE", temp_file_default,
-                                    "Override for temporary filename")
+    #
+    ## BAD: temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}")
+    ## BAD: temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}" if TEMP_BASE else temp_filename)
+    ## OLD: temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}" if TEMP_BASE else None)
+    # note: Normally TEMP_FILE gets overriden when TEMP_BASE set. However,
+    # this complicates preserving test-specific test files (see unittest_wrapper.py).
+    temp_file_default = None
+    if TEMP_BASE and not PRESERVE_TEMP_FILE:
+        temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}")
+    debug.trace_expr(5, system.getenv("TEMP_FILE"))
+    TEMP_FILE = system.getenv_value(
+        "TEMP_FILE", temp_file_default,
+        description="Override for temporary filename")
+    debug.trace_expr(5, system.getenv("TEMP_FILE"))
+    #
+    global TEMP_LOG_FILE
+    TEMP_LOG_FILE = system.getenv_text(
+        "TEMP_LOG_FILE", get_temp_file() + "-log",
+        description="Log file for stderr such as for issue function")
+    global TEMP_SCRIPT_FILE
+    TEMP_SCRIPT_FILE = system.getenv_text(
+        "TEMP_SCRIPT_FILE", get_temp_file() + "-script",
+        description="File for command invocation")
+#
+init()
 
 def main():
     """Entry point"""
     # Uses dynamic import to avoid circularity
     from mezcla.main import Main        # pylint: disable=import-outside-toplevel
     
     # Note: Uses main-based arg parsing for sake of show environment options
```

### Comparing `mezcla-1.3.9.9/mezcla/html_utils.py` & `mezcla-1.4.0.0/mezcla/html_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,44 +53,38 @@
 """HTML utility functions"""
 
 # Standard packages
 import html
 import re
 import sys
 import time
-## OLD: import urllib
 import urllib.request
 from urllib.error import HTTPError, URLError
 from http.client import HTTPMessage
-## OLD: from typing import Dict
 try:
     from typing_extensions import Any, Callable, Dict, List, Optional, Union
 except:
-    ## OLD: sys.exit("Error: html_utils.py requires Python 3.9+ (backport limitations with typing_extensions)")
     sys.stderr.write("Error importing extensions: {sys.exc_info}\n")
     sys.exit("Error: html_utils.py requires Python typing_extensions >= 4.7.0 (backport limitations with typing_extensions)")
 
 # Installed packages
 # Note: selenium import now optional; BeautifulSoup also optional
-## OLD: from selenium import webdriver
 import requests
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import system
 from mezcla.system import write_temp_file
 
 # Constants
-## OLD: DEFAULT_STATUS_CODE = "000"
 DEFAULT_STATUS_CODE = 0
 MAX_DOWNLOAD_TIME = system.getenv_integer("MAX_DOWNLOAD_TIME", 60,
                                           "Time in seconds for rendered-HTML download as with get_inner_html")
-## OLD: MID_DOWNLOAD_SLEEP_SECONDS = system.getenv_integer("MID_DOWNLOAD_SLEEP_SECONDS", 60)
 MID_DOWNLOAD_SLEEP_SECONDS = system.getenv_integer("MID_DOWNLOAD_SLEEP_SECONDS", 15,
                                                    "Mid-stream delay if document not ready")
 POST_DOWNLOAD_SLEEP_SECONDS = system.getenv_integer("POST_DOWNLOAD_SLEEP_SECONDS", 1,
                                                     "Courtesy delay after URL access--prior to download")
 SKIP_BROWSER_CACHE = system.getenv_boolean("SKIP_BROWSER_CACHE", False,
                                            "Don't use cached webdriver browsers")
 USE_BROWSER_CACHE = not SKIP_BROWSER_CACHE
@@ -101,14 +95,20 @@
                                        "Timeout in seconds for request-based as with download_web_document")
 HEADLESS_WEBDRIVER = system.getenv_bool("HEADLESS_WEBDRIVER", True,
                                         "Whether Selenium webdriver is hidden")
 STABLE_DOWNLOAD_CHECK = system.getenv_bool("STABLE_DOWNLOAD_CHECK", False,
                                            "Wait until download size stablizes--for dynamic content")
 EXCLUDE_IMPORTS = system.getenv_bool("EXCLUDE_IMPORTS", False,
                                      "Sets --follow-imports=silent; no import files are checked")
+TARGET_BOOTSTRAP =  system.getenv_bool(
+    "TARGET_BOOTSTRAP", False,
+    description="Format tooltips, etc. for use with bootstrap")
+FIREFOX_WEBDRIVER = system.getenv_bool(
+    "FIREFOX_WEBDRIVER", True,          ## TODO: "FIREFOX_WEBDRIVER", False,
+    description="Use Firefox webdriver for Selenium")
 HEADERS = "headers"
 FILENAME = "filename"
 
 # Custom Types
 OptStrBytes = Union[str, bytes, None]
 OptBoolStr = Union[bool, str, None]
 
@@ -141,19 +141,26 @@
                     "Note: Browser automation without cache not well tested!")
 
     # Check for cached version of browser. If none, create one and access page.
     browser = browser_cache.get(url) if USE_BROWSER_CACHE else None
     if not browser:
         # Make the browser hidden by default (i.e., headless)
         # See https://stackoverflow.com/questions/46753393/how-to-make-firefox-headless-programmatically-in-selenium-with-python.
-        # pylint: disable=import-outside-toplevel
-        from selenium.webdriver.firefox.options import Options
-        webdriver_options = Options()
-        webdriver_options.headless = HEADLESS_WEBDRIVER
-        browser = webdriver.Firefox(options=webdriver_options)
+        ## TODO2: add an option to use Chrome
+        ## OLD:
+        ## # pylint: disable=import-outside-toplevel
+        ## from selenium.webdriver.firefox.options import Options
+        options_module = (webdriver.firefox.options if FIREFOX_WEBDRIVER else webdriver.chrome.options)
+        webdriver_options = options_module.Options()
+        ## OLD: webdriver_options.headless = HEADLESS_WEBDRIVER
+        if HEADLESS_WEBDRIVER:
+            webdriver_options.add_argument('-headless')
+        ## OLD: browser = webdriver.Firefox(options=webdriver_options)
+        browser_class = (webdriver.Firefox if FIREFOX_WEBDRIVER else webdriver.Chrome)
+        browser = browser_class(options=webdriver_options)
         debug.trace_object(5, browser)
 
         # Get the page, setting optional cache entry and sleeping afterwards
         if USE_BROWSER_CACHE:
             browser_cache[url] = browser
         browser.get(url)
 
@@ -180,15 +187,14 @@
     debug.trace_fmt(5, "get_inner_html({u})", u=url)
     try:
         # Navigate to the page (or get browser instance with existing page)
         browser = get_browser(url)
         # Wait for Javascript to finish processing
         wait_until_ready(url)
         # Extract fully-rendered HTML
-        ## OLD: inner_html = browser.execute_script("return document.body.innerHTML")
         inner_html:str = browser.page_source
     except:
         inner_html = ""
         system.print_exception_info("get_inner_html")
     debug.trace_fmt(7, "get_inner_html({u}) => {h}", u=url, h=inner_html)
     return inner_html
 
@@ -289,15 +295,15 @@
         debug.trace(5, "Warning: set_param_dict is not thread-safe")
     user_parameters = param_dict
 
 
 def get_url_param(name : str, default_value : Optional[str] = None, param_dict : Optional[Dict] = None, escaped : bool = False):
     """Get value for NAME from PARAM_DICT (e.g., USER_PARAMETERS), using DEFAULT_VALUE (normally "").
     Note: It can be ESCAPED for use in HTML.
-    Different from get_url_parameter_value in possible returning list.
+    Different from get_url_parameter_value in possibly returning list.
     """
     # TODO3: default_value => default
     if default_value is None:
         default_value = ""
     param_dict = (get_param_dict(param_dict) or {})
     value = param_dict.get(name, default_value)
     value = system.to_unicode(value)
@@ -329,15 +335,14 @@
     # EX: get_url_param_checkbox_spec("param", param_dict={"param": "on"}) => "checked"
     # EX: get_url_param_checkbox_spec("param", param_dict={"param": "off"}) => ""
     # NOTE: 1 also treated as True
     # TODO: implement in terms of get_url_param
     param_dict = (get_param_dict(param_dict) or {})
     param_value = param_dict.get(name, default_value)
     param_value = system.to_unicode(param_value)
-    ## OLD: value = "checked" if (param_value in [True, "on"]) else ""
     value = "checked" if (param_value in ["1", "on", True]) else ""
     debug.trace_fmtd(4, "get_url_param_checkbox_spec({n}, [{d}]) => {v})",
                      n=name, d=default_value, v=value)
     return value
 #
 get_url_parameter_checkbox_spec = get_url_param_checkbox_spec
 
@@ -360,18 +365,16 @@
     """Get boolean value for PARAM from PARAM_DICT, with "on" treated as True. @note the hash defaults to user_parameters, and the default value is False
     Note: Only treates {"1", "on", "True", True} as True.
     Warning: defaults with non-None values might return unintuitive results unless
     coerced to boolean beforehand.
     """
     # EX: get_url_parameter_bool("abc", False, { "abc": "on" }) => True
     # TODO: implement in terms of get_url_param and also system.to_bool
-    ## OLD: result = (param_dict.get(param, default_value) in ["on", True])
     debug.assertion((default_value is None) or isinstance(default_value, bool))
     result = (get_url_parameter_value(param, default_value, param_dict)
-              ## OLD: in ["1", "on", True])
               in ["1", "on", "True", True])
     ## HACK: result = ((system.to_unicode(param_dict.get(param, default_value))) in ["on", True])
     debug.trace_fmtd(4, "get_url_parameter_bool({p}, {dft}, _) => {r}",
                      p=param, dft=default_value, r=result)
     return result
 #
 get_url_param_bool = get_url_parameter_bool
@@ -402,15 +405,14 @@
 
 
 def fix_url_parameters(url_parameters : Dict):
     """Uses the last values for any user parameter with multiple values
     and ensures dashes are used instead of embedded underscores in the keys"""
     # EX: fix_url_parameters({'w_v':[7, 8], 'h_v':10}) => {'w-v':8, 'h-v':10}
     # EX: fix_url_parameters({'_':'_'}) => {'_':'_'}
-    ## OLD: new_url_parameters = {p.replace("_", "-"):v for  (p, v) in url_parameters.items()}
     new_url_parameters = {my_re.sub(r"([a-z0-9])_", r"\1-", p):v
                           for  (p, v) in url_parameters.items()}
     new_url_parameters = {p:(v[-1] if isinstance(v, list) else v) for (p, v) in new_url_parameters.items()}
     debug.trace_fmt(6, "fix_url_parameters({up}) => {new}",
                     up=url_parameters, new=new_url_parameters)
     return new_url_parameters
 
@@ -477,15 +479,14 @@
     if "//" not in url:
         url = "http://" + url
     if download_dir is None:
         download_dir = "downloads"
     if (not system.file_exists(download_dir)):
         gh.full_mkdir(download_dir)
     local_filename = gh.form_path(download_dir, filename)
-    ## OLD: headers = ""
     ## TEST: headers = {}
     ## TEST: headers : Dict[Any, Any] = {}
     headers : HTTPMessage = HTTPMessage()
     status_code = DEFAULT_STATUS_CODE
     ok = False
     if DOWNLOAD_TIMEOUT:
         # HACK: set global socket timeout
@@ -714,26 +715,26 @@
     debug.trace_expr(7, param_name, label, default_value, disabled, prefix="in format_checkbox: ")
     checkbox_spec = get_url_param_checkbox_spec(param_name, default_value)
     disabled_spec = ("disabled" if disabled else "")
     status_spec = f"{checkbox_spec} {disabled_spec}".strip()
     style_spec = (f"style='{style}'" if style else "")
     misc_spec = (misc_attr if misc_attr else "")
     if (label is None):
-        ## OLD: label = (param_name.replace("-", " ").capitalize() + "?")
         label = (param_name.replace("-", " ") + "?")
         if not skip_capitalize:
             label = label.capitalize()
-    ## OLD: result = ""
     ## TODO: use hidden only if (default_value in ["1", "on", True])???
     result = f"<input type='hidden' name='{param_name}' value='off'>"
-    ## OLD: result += f"<label>{label} <input type='checkbox' id='{param_name}-id' name='{param_name}' {status_spec}></label>&nbsp;"
     tooltip_start_spec = tooltip_end_spec = ""
     if tooltip:
-        tooltip_start_spec = f'<span class="tooltip-control"><span class="tooltip-field">{tooltip}</span>'
-        tooltip_end_spec = "</span>"
+        if TARGET_BOOTSTRAP:
+            misc_spec += f" data-bs-toggle='tooltip' title='{tooltip}'"
+        else:
+            tooltip_start_spec = f'<span class="tooltip-control"><span class="tooltip-field">{tooltip}</span>'
+            tooltip_end_spec = "</span>"
     result += f"<label>{tooltip_start_spec}{label}{tooltip_end_spec}<input type='checkbox' id='{param_name}-id' name='{param_name}' {style_spec} {status_spec} {misc_spec}></label>"
     debug.trace(6, f"format_checkbox({param_name}, ...) => {result}")
     return result
 
 
 def format_url_param(name : str, default : Optional[str] = None):
     """Return URL parameter NAME formatted for an HTML form (e.g., escaped)"""
@@ -774,31 +775,32 @@
             label = label.capitalize()
     if (default_value is None):
         default_value = ""
     if (num_rows is None):
         num_rows = 1
     if (size is None):
         size = max_len
-    ## OLD: value_spec = (f"{default_value}" if default_value else "")
     value_spec = (get_url_param(param_name) or default_value)
     disabled_spec = ("disabled" if disabled else "")
     style_spec = (f"style='{style}'" if style else "")
     misc_spec = (misc_attr if misc_attr else "")
     misc_spec += (f"onchange={on_change}" if on_change else "")
     tooltip_start_spec = tooltip_end_spec = ""
     if tooltip:
-        tooltip_start_spec = f'<span class="tooltip-control"><span class="tooltip-field">{tooltip}</span>'
-        tooltip_end_spec = "</span>"
+        if TARGET_BOOTSTRAP:
+            misc_spec += f" data-bs-toggle='tooltip' title='{tooltip}'"
+        else:
+            tooltip_start_spec = f'<span class="tooltip-control"><span class="tooltip-field">{tooltip}</span>'
+            tooltip_end_spec = "</span>"
     result = f'<label>{tooltip_start_spec}{label}{tooltip_end_spec}&nbsp;'
     if text_area:
         max_len_spec = (f'maxlength="{max_len}"' if max_len else "")
         value_spec = format_url_param(param_name)
         result += f'<textarea id="{param_name}-id" name="{param_name}" rows={num_rows} {style_spec} {max_len_spec} {disabled_spec} {misc_spec}>{value_spec}</textarea>'
     else:
-        ## OLD: max_len_spec = (f"maxlength={max_len} size={max_len}" if max_len else "")
         len_spec = ""
         if max_len:
             len_spec += f' maxlength="{max_len}"'
         if size:
             len_spec += f' size="{size}"'
         result += f'<input id="{param_name}-id" value="{value_spec}" name="{param_name}" {style_spec} {len_spec} {disabled_spec} {misc_spec}>'
     result += "</label>"
@@ -841,15 +843,14 @@
 
 def html_to_text(document_data : str):
     """Returns text version of html DATA"""
     # EX: html_to_text("<html><body><!-- a cautionary tale -->\nMy <b>fat</b> dog has fleas</body></html>") => "My fat dog has fleas"
     # Note: stripping javascript and style sections based on following:
     #   https://stackoverflow.com/questions/22799990/beatifulsoup4-get-text-still-has-javascript
     debug.trace_fmtd(7, "html_to_text(_):\n\tdata={d}", d=document_data)
-    ## OLD: soup = BeautifulSoup(document_data)
     init_BeautifulSoup()
     soup = BeautifulSoup(document_data, "lxml") if BeautifulSoup else None
     # Remove all script and style elements
     text = ""
     if soup:
         for script in soup.find_all(["script", "style"]):
             # *** TODO: soup = soup.extract(script)
@@ -913,18 +914,14 @@
         if (image.attrs.get('style') in ["display:none", "visibility:hidden"]):
             debug.trace_fmt(5, "Ignoring hidden image: {img}", img=image)
             continue
         image_src = image.get("src", "")
         if not image_src:
             debug.trace_fmt(5, "Ignoring image without src: {img}", img=image)
             continue
-        ## OLD:
-        ## if image_src.startswith("/"):
-        ##     image_src = web_site_url + image_src
-        ## elif not image_src.startswith("http"):
         if image_src.startswith("//"):
             url_proto = (my_re.search(r"^(\w+):", url) and my_re.group(1))
             image_src = f"{url_proto}:{image_src}"
         elif not my_re.search(r"^(http)|(data:)", image_src):
             image_src = base_url + image_src.lstrip("/")
         else:
             debug.trace(7, f"Using image src as is: {image_src}")
@@ -938,30 +935,30 @@
 
 #-------------------------------------------------------------------------------
 
 def main(args : List[str]) -> None:
     """Supporting code for command-line processing"""
     ## NOTE: This is work-in-progress from a debug-only utility
     debug.trace_fmtd(6, "main({a})", a=args)
-    ## OLD:
-    ## user = system.getenv_text("USER")
-    ## system.print_stderr("Warning, {u}: this is not intended for direct invocation".format(u=user))
 
     # Parse command line arguments
     # TODO2: use master.Main for arg parsing
-    skip_inner = False
+    plain_text = False
+    plain_html = False
     show_usage = False
     use_stdout = False
     quiet = False
     filename : Optional[str] = None
     for i, arg in enumerate(args[1:]):
         if (arg == "--help"):
             show_usage = True
         elif (arg == "--regular"):
-            skip_inner = True
+            plain_text = True
+        elif (arg == "--html"):
+            plain_html = True
         elif (arg == "--inner"):
             pass
         elif (arg == "--stdout"):
             use_stdout = True
         elif (arg == "--quiet"):
             quiet = True
         elif (not arg.startswith("-")):
@@ -970,75 +967,80 @@
         else:
             system.print_stderr(f"Error: unknown argument: {arg}")
             show_usage = True
             break
         i += 1
 
     # HACK: Convert local html document to text
-    if (filename and (not my_re.search("www|http", filename) or skip_inner)):
+    if (filename and (not my_re.search("www|http", filename) or plain_text)):
         doc_filename = filename
         document_data = system.read_file(doc_filename)
         document_text = html_to_text(document_data)
         if use_stdout:
             print(document_text)
         else:
             system.write_file(doc_filename + ".list", document_text)
             print(f"See {doc_filename}.list")
     
     # HACK: Do simple test of inner-HTML support
     # TODO: Do simpler test of download_web_document
     # TODO1: add explicit argument for inner-html support
-    ## OLD: if (len(args) > 1):
     elif (filename):
         # Get web page text
         debug.trace_fmt(4, "browser_cache: {bc}", bc=browser_cache)
         url = filename
         debug.trace_expr(6, retrieve_web_document(url))
         html_data = download_web_document(url)
         filename = system.quote_url_text(url)
         if not filename:
             filename = ""
-        if debug.debugging():
-            write_temp_file("pre-" + filename, html_data)
-        
-        # Show inner/outer HTML
-        # Note: The browser is hidden unless MOZ_HEADLESS false
-        # TODO: Support Chrome
-        ## OLD: wait_until_ready(url)
-        ## BAD: rendered_html = render(html_data)
-        system.setenv("MOZ_HEADLESS",
-                      str(int(system.getenv_bool("MOZ_HEADLESS", True))))
-        rendered_html = get_inner_html(url)
-        output_filename = "post-" + filename
-        if (not use_stdout) or debug.debugging():
-            write_temp_file(output_filename, rendered_html)
-        if use_stdout:
-            if not quiet:
-                print("Rendered html:")
-            print(system.to_utf8(rendered_html))            
+
+        if plain_html:
+            if use_stdout:
+                print(html_data)
+            else:
+                system.write_file(doc_filename + ".html", html_data)
+                print(f"See {doc_filename}.html")
         else:
-            print(f"See {output_filename}")
+            if debug.debugging():
+                write_temp_file("pre-" + filename, html_data)
             
-        if debug.debugging():
-            rendered_text = get_inner_text(url)
-            debug.trace_fmt(5, "type(rendered_text): {t}", t=rendered_text)
-            write_temp_file("post-" + filename + ".txt", rendered_text)
-        debug.trace_fmt(4, "browser_cache: {bc}", bc=browser_cache)
+            # Show inner/outer HTML
+            # Note: The browser is hidden unless MOZ_HEADLESS false
+            # TODO: Support Chrome
+            system.setenv("MOZ_HEADLESS",
+                          str(int(system.getenv_bool("MOZ_HEADLESS", True))))
+            rendered_html = get_inner_html(url)
+            output_filename = "post-" + filename
+            if (not use_stdout) or debug.debugging():
+                write_temp_file(output_filename, rendered_html)
+            if use_stdout:
+                if not quiet:
+                    print("Rendered html:")
+                print(system.to_utf8(rendered_html))            
+            else:
+                print(f"See {output_filename}")
+                
+            if debug.debugging():
+                rendered_text = get_inner_text(url)
+                debug.trace_fmt(5, "type(rendered_text): {t}", t=rendered_text)
+                write_temp_file("post-" + filename + ".txt", rendered_text)
+            debug.trace_fmt(4, "browser_cache: {bc}", bc=browser_cache)
     else:
         show_usage = True
 
     # Not sure what to do
-    ## OLD: else:
     if show_usage:
-        ## OLD: print("Specify a URL as argument 1 for a simple test of inner access")
         script = gh.basename(__file__)
-        print("Usage: {prog} [--help] [--stdout] [--quiet] [[--regular | --inner] [filename]]")
-        print("- Specify a local HTML file to save as text.")
+        print("Usage: {prog} [--help] [--stdout] [--quiet] [[--regular | --inner | --html] [filename]]")
+        print("- Specify a local HTML file to download (e.g., save as text).")
         print("- Otherwise, specify a URL for a simple test of inner html access (n.b., via stdout).")
-        print("- Use --regular to bypass default inner processing.")
+        print("- Use --regular to bypass default inner processing (and save as text).")
+        ## TODO3: add explicit option like --text to make processing more consistent
+        print("- With --html or --inner, the result is saved as html.")
         print()
         print("Examples:")
         print(f"- {script} --inner --stdout --quiet https://twitter.com/home > twitter-home.html")
         print(f"- {script} --regular --stdout bootstrap-hello-world.html > bootstrap-hello-world.txt")
     return
 
 if __name__ == '__main__':
```

### Comparing `mezcla-1.3.9.9/mezcla/ipython_utils.py` & `mezcla-1.4.0.0/mezcla/ipython_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     import mezcla.ipython_utils
     reload(mezcla.ipython_utils)
     import_module_globals = mezcla.ipython_utils.import_module_globals
     import_module_globals("mezcla.misc_utils", globals_dict=builtins.globals());
     (TYPICAL_EPSILON, VALUE_EPSILON)
     >>>
     (1e-06, 0.001)
+
+Misc. usage:
+    set_xterm_title(f"ipython: {os.getcwd()}")
 """
 
 # Note: most imports are done for the sake of ipython usage
 #
 # pylint: disable=unused-import
 
 # Standard modules
```

### Comparing `mezcla-1.3.9.9/mezcla/kenlm_example.py` & `mezcla-1.4.0.0/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/keras_param_search.py` & `mezcla-1.4.0.0/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/main.py` & `mezcla-1.4.0.0/mezcla/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 # Local packages
 from mezcla import debug
 from mezcla import tpo_common as tpo
 from mezcla import glue_helpers as gh
 from mezcla import system
 from mezcla.my_regex import my_re
 from mezcla.system import getenv_bool
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Constants
 HELP_ARG = "--help"
 USAGE_ARG = "--usage"
 VERBOSE_ARG = "verbose"
 USE_PARAGRAPH_MODE_DEFAULT = getenv_bool("USE_PARAGRAPH_MODE", False)
 USE_PARAGRAPH_MODE = getenv_bool("PARAGRAPH_MODE", USE_PARAGRAPH_MODE_DEFAULT,
@@ -172,23 +173,25 @@
                  multiple_files=False,
                  use_temp_base_dir=None,
                  usage_notes=None,
                  program=None,
                  paragraph_mode=None, track_pages=None, file_input_mode=None, newlines=None,
                  boolean_options=None, text_options=None, int_options=None,
                  float_options=None, positional_options=None, positional_arguments=None,
-                 skip_input=None, manual_input=None, auto_help=None, brief_usage=None,
+                 skip_input=None, manual_input=None, skip_stdin=None, auto_help=None, brief_usage=None,
                  short_options=None, **kwargs):
         """Class constructor: parses RUNTIME_ARGS (or command line), with specifications
         for BOOLEAN_OPTIONS, TEXT_OPTIONS, INT_OPTIONS, FLOAT_OPTIONS, and POSITIONAL_OPTIONS
-        (see convert_option). Includes options to SKIP_INPUT, or to have MANUAL_INPUT, or to use AUTO_HELP invocation (i.e., assuming {ha} if no args). Also allows for SHORT_OPTIONS"""
+        (see convert_option). Includes options to SKIP_INPUT, or to have MANUAL_INPUT, or to use AUTO_HELP invocation (i.e., assuming {ha} if no args). Also allows for SHORT_OPTIONS.
+        Note: SKIP_STDIN makes explicit SKIP_INPUT which gets inferred from MANUAL_INPUT when no specified. This avoids the - argument support that blocks help usage.
+        """
         #
         def trace_args(level:int, label:str):
             """Trace out input arguments, each on separate line to simplify diff"""
-            debug.trace_expr(level, runtime_args, description, skip_args, multiple_files, use_temp_base_dir, usage_notes, program, paragraph_mode, track_pages, file_input_mode, newlines, boolean_options, text_options, int_options, float_options, positional_options, positional_arguments, skip_input, manual_input, auto_help, brief_usage, short_options, kwargs, prefix=f"{label}: {{", delim="\n\t", suffix="}")
+            debug.trace_expr(level, runtime_args, description, skip_args, multiple_files, use_temp_base_dir, usage_notes, program, paragraph_mode, track_pages, file_input_mode, newlines, boolean_options, text_options, int_options, float_options, positional_options, positional_arguments, skip_input, manual_input, skip_stdin, auto_help, brief_usage, short_options, kwargs, prefix=f"{label}: {{", delim="\n\t", suffix="}")
         #
         debug.trace(4, f"Main.__init__(): self={self}")
         trace_args(5, "input")
         self.description = "TODO: what the script does"   # *** DONT'T MODIFY: default TODO note for client
         self.boolean_options = []
         self.text_options = []
         self.int_options = []
@@ -202,14 +205,16 @@
         self.rel_line_num = -1
         self.rel_para_num = -1
         self.page_num = -1
         self.para_num = -1
         self.line_num = -1
         self.char_offset = -1
         self.raw_line = None
+        # note: auto_help is typically used when there is a filename argument
+        debug.assertion(not (auto_help and skip_stdin))
         if (auto_help is None):
             ## TODO?: if (all(map(lambda v: v is None, [auto_help, skip_input, manual_input]))):
             ## TEST: auto_help = ((skip_input is None) and (manual_input is None)))
             # Note: auto-help is enabled by default unless no input
             auto_help = ((not skip_input) or manual_input)
             debug.trace(7, f"inferred auto_help: {auto_help}")
         self.auto_help = auto_help      # adds --help to command line if no arguments
@@ -219,15 +224,16 @@
         # TODO: *** Add better sanity checking (such as a filename on command line).
         if manual_input is None:
             # NOTE: skip_input=>manual_input: T=>T  F=>F  None=>F (i.e., bool(skip_input))
             manual_input = False if (skip_input is None) else skip_input
             debug.trace_fmt(7, "inferred manual_input: {mi}", mi=manual_input)
         self.manual_input = manual_input
         if skip_input is None:
-            skip_input = self.manual_input
+            ## OLD: skip_input = self.manual_input
+            skip_input = (self.manual_input or skip_stdin)
             debug.trace_fmt(7, "inferred skip_input: {si}", si=skip_input)
         self.skip_input = skip_input
         #
         self.parser = None
         if brief_usage is None:
             brief_usage = BRIEF_USAGE
         self.brief_usage = brief_usage  # show brief usage instead of full --help
@@ -381,14 +387,16 @@
         includes an optional nargs component, such as"
              ("other-files", "Other file names", ["f1", "f2", "f3"], "+")
         """
         # EX: label, _desc, _default = Main.convert_option("--mucho-backflips"); label => "--mucho-backflips"
         ## TODO2: add short option support as in ("--num-eggs/-#", "Number of eggs", 2)
         ## TODO3: make the component representation structured (e.g., namedtuple)
         ## TEST: result = ["", "", ""]
+        tpo.debug_format("in convert_option({o}, {d}, {p})", 6,
+                         o=option_spec, d=default_value, p=positional)
         opt_label = None
         opt_desc = None
         opt_default = default_value
         opt_nargs = None
         opt_prefix = "--" if not positional else ""
         # TODO: use keyword arguments (or namedtuple)
         if isinstance(option_spec, tuple):
@@ -708,18 +716,19 @@
                 debug.assertion(self.filename != ["-"])
                 if not self.multiple_files:
                     # note: check_arguments sets self.other_filenames
                     debug.trace(3, "Warning: Not opening multiple-valued filename arg")
                     debug.trace_expr(3, self.filename, self.other_filenames)
             else:
                 debug.assertion(isinstance(self.filename, str))
-                debug.assertion(os.path.exists(self.filename))
-                mode = ("r" if (not self.binary_input) else "rb")
-                self.input_stream = system.open_file(self.filename, mode=mode, errors=self.input_error)
-                debug.assertion(self.input_stream)
+                if not (self.manual_input and self.skip_input):
+                    debug.assertion(os.path.exists(self.filename))
+                    mode = ("r" if (not self.binary_input) else "rb")
+                    self.input_stream = system.open_file(self.filename, mode=mode, errors=self.input_error)
+                    debug.assertion(self.input_stream)
         # Optionally reopen stream to change built-in settings
         error_handling_change = (self.input_error and (self.input_error != self.input_stream.errors))
         reopen_stream = (error_handling_change or self.newlines)
         if reopen_stream:
             if self.newlines:
                 debug.trace(4, f"Changing input stream newlines from {self.input_stream.newlines!r} to {self.newlines!r}")
             if error_handling_change:
```

### Comparing `mezcla-1.3.9.9/mezcla/merge_files.py` & `mezcla-1.4.0.0/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/merge_notes.py` & `mezcla-1.4.0.0/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/mezcla` & `mezcla-1.4.0.0/mezcla/mezcla`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/misc_utils.py` & `mezcla-1.4.0.0/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/my_regex.py` & `mezcla-1.4.0.0/mezcla/my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/ngram_tfidf.py` & `mezcla-1.4.0.0/mezcla/ngram_tfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # - This provides the wrapper class ngram_tfidf_analysis around tfidf for use
 #   in applications like Visual Diff Search (VDS) that use text from external sources.
 # - This incorporates a few optional heuristics, such as filtering overlapping ngrams
 #   and boosting captialized ngrams.
 # - See compute_tfidf.py for computing tfidf over files.
 #
 # TODO:
-# - Add more optional heuristics: part-of-speech boosting, adjoining ngram fitlering,
+# - Add more optional heuristics: part-of-speech boosting, adjoining ngram filtering,
 #   noun-phrase boosting, etc.
 # - Isolate ngram support into separate module.
 # - Reconcile with compute_tfidf.py (e.g., subsumption here with overlap there).
 #
 
 """TF-IDF using phrasal terms via ngram analysis
 
@@ -28,14 +28,15 @@
   {script} -
 
   echo $'a b c\\nb c d\\nc d e' | MIN_NGRAM_SIZE=2 MAX_NGRAM_SIZE=2 SKIP_TFIDF_PREPROCESSOR=1 {script} {options} -
 """
 ## TODO: fix description (e.g., add pointer to VDS code)
 
 # Standard packages
+from collections import defaultdict
 import re
 import sys
 
 # Installed packages
 from sklearn.feature_extraction.text import CountVectorizer
 
 # Local packages
@@ -153,14 +154,16 @@
         self.text_proc = None
         if TFIDF_NP_BOOST or TFIDF_VP_BOOST:
             self.text_proc = create_text_proc(TFIDF_TEXT_PROC)
         ## TODO2: add international stopwords (e.g., English plus frequent ones from common languages)
         self.stopwords = None
         self.good_terms = (good_terms or [])
         self.bad_terms = (bad_terms or [])
+        self.noun_phrases = None
+        self.verb_phrases = None
         self.reset()
         super().__init__(*args, **kwargs)
 
     def reset(self):
         """Re-initialize the instance"""
         self.pp = tfidf_preprocessor(language=self.pp_lang,
                                      gramsize=self.max_ngram_size,
@@ -169,28 +172,36 @@
                                      stemmer=lambda x: x)
         self.corpus = tfidf_corpus(gramsize=self.max_ngram_size,
                                    min_ngram_size=self.min_ngram_size,
                                    all_ngrams=ALL_NGRAMS,
                                    language=self.pp_lang,
                                    preprocessor=self.pp)
         self.stopwords = (self.pp.stopwords or ENGLISH_STOPWORDS)
+        self.noun_phrases = []
+        self.verb_phrases = []
 
     def set_good_terms(self, text):
         """Sets good terms to TEXT split into word tokens"""
         self.good_terms = split_tokens(text)
         
     def set_bad_terms(self, text):
         """Sets bad terms to TEXT split into word tokens"""
         self.bad_terms = split_tokens(text)
         
     def add_doc(self, text, doc_id=None):
         """Add document TEXT to collection with key DOC_ID, which defaults to order processed (1-based)"""
         if doc_id is None:
             doc_id = str(len(self.corpus) + 1)
         self.corpus[doc_id] = text
+        self.noun_phrases = defaultdict(list)
+        self.verb_phrases = defaultdict(list)
+        if TFIDF_NP_BOOST:
+            self.noun_phrases[doc_id] = self.text_proc.noun_phrases(text) 
+        if TFIDF_VP_BOOST:
+            self.verb_phrases[doc_id] = self.text_proc.verb_phrases(text) 
 
     def get_doc(self, doc_id):
         """Return document data for DOC_ID"""
         return self.corpus[doc_id]
 
     def is_stopword(self, word):
         """Whether WORD is a stop word for preprocessing language or English if none"""
@@ -260,18 +271,20 @@
         if apply_reranking:
             boosted = False
             for (i, (ngram, score)) in enumerate(top_term_info):
                 ngram = top_term_info[i][0]
                 old_score = top_term_info[i][1]
 
                 # Apply boost if entire ngram is a noun phrase and likewise for verb phrase
-                if (TFIDF_NP_BOOST and self.text_proc.noun_phrases(ngram) == [ngram]):
+                ## OLD: if (TFIDF_NP_BOOST and self.text_proc.noun_phrases(ngram) == [ngram]):
+                if (TFIDF_NP_BOOST and (ngram in self.noun_phrases[doc_id])):
                     score = old_score * TFIDF_NP_BOOST
                     debug.trace(5, f"boosted NP {ngram!r} from {rnd(old_score)} to {rnd(score)}")
-                if (TFIDF_VP_BOOST and self.text_proc.verb_phrases(ngram) == [ngram]):
+                ## OLD: if (TFIDF_VP_BOOST and self.text_proc.verb_phrases(ngram) == [ngram]):
+                if (TFIDF_VP_BOOST and (ngram in self.verb_phrases[doc_id])):
                     score = old_score * TFIDF_VP_BOOST
                     debug.trace(5, f"boosted VP {ngram!r} from {rnd(old_score)} to {rnd(score)}")
                 if (TFIDF_NUMERIC_BOOST and any(tpo.is_numeric(token) for token in split_tokens(ngram))):
                     score = old_score * TFIDF_NUMERIC_BOOST
                     debug.trace(5, f"boosted numeric {ngram!r} from {rnd(old_score)} to {rnd(score)}")
                 if (TFIDF_GOOD_BOOST and system.intersection(split_tokens(ngram), self.good_terms)):
                     score = old_score * TFIDF_GOOD_BOOST
```

### Comparing `mezcla-1.3.9.9/mezcla/os_utils.py` & `mezcla-1.4.0.0/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/pandas_sklearn.py` & `mezcla-1.4.0.0/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/plot_utils.py` & `mezcla-1.4.0.0/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/python_ast.py` & `mezcla-1.4.0.0/mezcla/python_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/randomize_lines.py` & `mezcla-1.4.0.0/mezcla/randomize_lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ## OLD: """Randomize lines from stardard input"""
 
 """
 Randomize lines in a file (without reading entirely into memory).
 Note: The default seed is {seed}.
 
 Sample usage:
-    {script} --include-header --percent 10 ./examples/pima-indians-diabetes.csv
+    {script} --header --percent 10 ./examples/pima-indians-diabetes.csv
 """
 
 # Standard modules
 ## OLD: import argparse
 import os
 import random
 import sys
```

### Comparing `mezcla-1.3.9.9/mezcla/rgb_color_name.py` & `mezcla-1.4.0.0/mezcla/rgb_color_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # Notes:
 # - Based on https://computergraphics.stackexchange.com/questions/1542/convert-rgb-hex-or-any-other-color-format-to-standard-color-programmatically.
 # - Color rgb:(0, 255, 0) is reported as lime instead of green. See
 #     https://webcolors.readthedocs.io
 # - For utility to extract colors from images, see
 #   https://pypi.org/project/extcolors
 #
+# TODO2: Put on a new low-priority script with respect to testing coverage.
+#
 #--------------------------------------------------------------------------------
 # Sample input (based on extcolors):
 #
 #   Extracted colors:
 #   (128, 128, 128):  72.98% (1888)
 #   (39, 39, 39)   :  24.35% (630)
 #   (255, 255, 255):   2.67% (69)
@@ -30,14 +32,15 @@
 #   Pixels in output: 2587 of 11648
 #
 #................................................................................
 # TODO:
 # - Add example usage with extcolors:
 #   extcolors self.filename | self.program -
 # - Add option to invoke extcolors automatically.
+# - Add direct way to generate webcolor listing.
 #
 
 r"""Convert RGB tuples into color names
 
 Sample usage:
    {script} --hex3 <<<"#eee"
 
@@ -103,15 +106,18 @@
         debug.assertion(my_re.search(spec_regex, self.rgb_regex, flags=my_re.IGNORECASE))
         self.hex = self.get_parsed_option(HEX, self.hex)
         self.skip_direct = self.get_parsed_option(SKIP_DIRECT, self.skip_direct)
         self.show_hex = self.get_parsed_option(SHOW_HEX, self.show_hex)
         self.check_direct_match = not self.skip_direct
 
         # Populate color names into spatial name database
+        # TODO2: isolate into helper class
         hexnames = webcolors.CSS3_HEX_TO_NAMES
+        debug.trace_values(6, hexnames)
+        debug.trace_expr(5, hexnames, max_len=2**16)
         self.color_names = []
         color_positions = []
         #
         for hex_code, name in hexnames.items():
             debug.trace(6, f"color: {name}={hex_code}")
             self.color_names.append(name)
             color_positions.append(webcolors.hex_to_rgb(hex_code))
```

### Comparing `mezcla-1.3.9.9/mezcla/run_albert_classifier.py` & `mezcla-1.4.0.0/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/run_bert_classifier.py` & `mezcla-1.4.0.0/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/samples/pima-indians-diabetes.csv` & `mezcla-1.4.0.0/mezcla/samples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/show_bert_representation.py` & `mezcla-1.4.0.0/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/simple_main_example.py` & `mezcla-1.4.0.0/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/spacy_nlp.py` & `mezcla-1.4.0.0/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/spell.py` & `mezcla-1.4.0.0/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/sys_version_info_hack.py` & `mezcla-1.4.0.0/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/system.py` & `mezcla-1.4.0.0/mezcla/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 # Installed packages
 import six
 
 # Local packages
 from mezcla import debug
 from mezcla.debug import UTF8
+## TODO3: debug.trace_expr(6, __file__)
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Constants
 STRING_TYPES = six.string_types
 MAX_SIZE = six.MAXSIZE
 MAX_INT = MAX_SIZE
 TEMP_DIR = None
 
@@ -389,26 +391,30 @@
 
 
 def open_file(filename, /, mode="r", *, encoding=None, errors=None, **kwargs):
     """Wrapper around around open() with FILENAME using UTF-8 encoding and ignoring ERRORS (both by default)
     Notes:
     - The mode is left at default (i.e., 'r')
     - As with open(), result can be used in a with statement:
-        with system.open_file(filename) as f: ...
+    ____ with system.open_file(filename) as f: ..
     """
+    ## TODO1: fix up ^^ for maldito sphinx: had to add ____'s for indendation
     # Note: position-only args precedes / and keyword only follow * (based on https://stackoverflow.com/questions/24735311/what-does-the-slash-mean-when-help-is-listing-method-signatures):
     #   def f(pos_only1, pos_only2, /, pos_or_kw1, pos_or_kw2, *, kw_only1, kw_only2): pass
     if (encoding is None) and ("b" not in mode):
         encoding = "UTF-8"
     if (encoding and (errors is None)):
         errors = 'ignore'
+    if kwargs.get(ENCODING) is None:
+        kwargs[ENCODING] = encoding
     result = None
     try:
         # pylint: disable=consider-using-with; note: bogus 'Bad option value' warning
-        result = open(filename, mode=mode, encoding=encoding, errors=errors, **kwargs)
+        ## BAD: result = open(filename, mode=mode, encoding=encoding, errors=errors, **kwargs)
+        result = open(filename, mode=mode, errors=errors, **kwargs)
     except IOError:
         debug.trace_fmtd(3, "Unable to open {f!r}: {exc}", f=filename, exc=get_exception())
     debug.trace_fmt(5, "open({f}, [{enc}, {err}], kwargs={kw}) => {r}",
                     f=filename, enc=encoding, err=errors, kw=kwargs, r=result)
     return result
 
 
@@ -556,16 +562,20 @@
 def read_entire_file(filename, **kwargs):
     """Read all of FILENAME and return as a string
     Note: optional arguments to open() passed along (e.g., encoding amd error handling)"""
     # TODO: allow for overriding handling of newlines (e.g., block \r being treated as line delim)
     # EX: write_file("/tmp/fu123", "1\n2\n3\n"); read_entire_file("/tmp/fu123") => "1\n2\n3\n"
     data = ""
     try:
+        ENCODING = "encoding"
+        if kwargs.get(ENCODING) is None:
+            kwargs[ENCODING] = "UTF-8"
         ## TODO: with open_file(filename, **kwargs) as f:
-        with open(filename, encoding="UTF-8", **kwargs) as f:
+        ## BAD: with open(filename, encoding="UTF-8", **kwargs) as f:
+        with open(filename, **kwargs) as f:
             data = f.read()
     except (AttributeError, IOError):
         debug.trace_exception(1, "read_entire_file/IOError")
         report_errors = (kwargs.get("errors") != "ignore")
         if report_errors:
             print_stderr("Error: Unable to read file '{f}': {exc}",
                          f=filename, exc=get_exception())
@@ -608,15 +618,19 @@
     return data
 
 
 def read_directory(directory):
     """Returns list of files in DIRECTORY"""
     # Note simple wrapper around os.listdir with tracing
     # EX: (intersection(["init.d", "passwd"], read_directory("/etc")))
-    files = os.listdir(directory)
+    files = []
+    try:
+        files = os.listdir(directory)
+    except:
+        print_exception_info(f"reading dir {directory!r}")
     debug.trace_fmtd(5, "read_directory({d}) => {r}", d=directory, r=files,
                      max_len=4096)
     return files
 
 
 def get_directory_filenames(directory, just_regular_files=False):
     """Returns full pathname for files in DIRECTORY, optionally restrictded to JUST_REGULAR_FILES
@@ -1294,16 +1308,48 @@
 
 def get_args():
     """Return command-line arguments (as a list of strings)"""
     result = sys.argv
     debug.trace_fmtd(6, "get_args() => {r}", r=result)
     return result
 
+
+def make_wrapper(function_name, function, trace_level=6):
+    """Creates wrapper around FUNCTION with NAME"""
+    debug.trace(7, f"make_wrapper{(function_name, function, trace_level)}")
+    # EX: make_wrapper("get_process_id", os.getpid).__doc__ => "Wrapper around posix.getpid"
+    # TODO3: resolve module used in refernce so that docstring more intuitive (e.g., posix.getpid => os.getpid)
+    #
+    def wrapper(*args, **kwargs):
+        """placeholder docstring"""
+        debug.trace(trace_level + 1, f"in f{function_name}: {args=} {kwargs=}")
+        result = function(*args, **kwargs)
+        debug.trace(trace_level, f"{function_name}() => {result!r}")
+        return result
+    #
+    function_spec = f"{function.__module__}.{function.__name__}"
+    wrapper.__doc__ = f"Wrapper around {function_spec}"
+    return wrapper
+
+def install_wrapper(function_name, function, **kwargs):
+    """Creates wrapper via make_wrapper (q.v.) and install in current namespace"""
+    debug.trace(7, f"install_wrapper{(function_name, function, kwargs)}")
+    wrapper = make_wrapper(function_name, function, **kwargs)
+    global_namespace = globals()
+    global_namespace[function_name] = wrapper
+
+#-------------------------------------------------------------------------------
+# Wrapper support
+# TODO: look into ways to inform pylint about function definitions
+
+install_wrapper("get_parent_pid", os.getppid)
+get_process_id = make_wrapper("get_process_id", os.getpid, trace_level=7)
+
 #-------------------------------------------------------------------------------
-# Memomization support (i.e., functiona result caching), based on 
+# Memomization support (i.e., function result caching), based on 
 #     See http://code.activestate.com/recipes/578231-probably-the-fastest-memoization-decorator-in-the-. [world!]
 # This is implemented transparently via Python decorators. See
 #     http://stackoverflow.com/questions/739654/understanding-python-decorators
 #
 # usage example:
 #
 #    @memodict
```

### Comparing `mezcla-1.3.9.9/mezcla/temp/compound_CID_3672.xml` & `mezcla-1.4.0.0/mezcla/temp/compound_CID_3672.xml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/temp/plot.py` & `mezcla-1.4.0.0/mezcla/temp/plot.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/temp/simple_batspp.py` & `mezcla-1.4.0.0/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/template.py` & `mezcla-1.4.0.0/mezcla/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,17 @@
 # Note: These are just intended for internal options, not for end users.
 # It also allows for enabling options in one place rather than four
 # (e.g., [Main member] initialization, run-time value, and argument spec., along
 # with string constant definition).
 # WARNING: To minimize environment comflicts with other programs make the names
 # longer such as two or more tokens (e.g., "FUBAR" => "FUBAR_LEVEL").
 #
-TODO_FUBAR = system.getenv_bool("TODO_FUBAR", False,
-                                description="TODO:Fouled Up Beyond All Recognition processing")
+TODO_FUBAR = system.getenv_bool(
+    "TODO_FUBAR", False,
+    description="TODO:Fouled Up Beyond All Recognition processing")
 
 ## TODO: Use helper class for main logic
 ## class Helper:
 ##     """TODO: class for doing ..."""
 ## 
 ##     def __init__(self, ...):
 ##         """Initializer: ..."""
@@ -85,15 +86,15 @@
     ## WARNING: For Script classes involving complex logic, it is best to use helper classes,
     ## as done in show_bert_representation.py.
     ## NOTE: Such class decomposition is also beneficial for unit tests.
     #
     ## def __init__(self, *args, **kwargs):
     ##     debug.trace_expr(TL.VERBOSE, self, args, kwargs, delim="\n\t", prefix="in {self.__class__.__name__}.__init__({a})")
     ##     super().__init__(*args, **kwargs)
-    
+
     def setup(self):
         """Check results of command line processing"""
         debug.trace_fmtd(TL.VERBOSE, "Script.setup(): self={s}", s=self)
         ## TODO: extract argument values
         self.todo_arg = self.get_parsed_option(TODO_ARG, self.todo_arg)
         ## TODO:
         ## self.text_arg = self.get_parsed_option(TEXT_ARG, self.text_arg)
@@ -146,16 +147,16 @@
         ## positional_arguments=[ALT_FILENAME], 
         ## text_options=[(TEXT_ARG, "TODO-desc")],
         ## Note: Following added for indentation float options not common (TODO: remove?)
         float_options=None)
     app.run()
     # Make sure no TODO_vars above (i.e., in namespace)
     debug.assertion(not any(my_re.search(r"^TODO_", m, my_re.IGNORECASE)
-                            for m in dir(app)))    
-    
+                            for m in dir(app)))
+
 #-------------------------------------------------------------------------------
-    
+
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_VERBOSE)
     debug.trace(5, f"module __doc__: {__doc__}")
     debug.assertion("TODO:" not in __doc__)
     main()
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/LICENSE.txt` & `mezcla-1.4.0.0/mezcla/tests/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+TODO4: use LICENSE.txt fom repo base directory
+
 GNU LESSER GENERAL PUBLIC LICENSE
 Version 3, 29 June 2007
 
 Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
 
 Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.4.0.0/mezcla/tests/adhoc-tests.batspp`

 * *Files 12% similar despite different names*

```diff
@@ -33,7 +33,14 @@
 ## $ ls | count-it '^test_(.)*.py$' | grep m
 ## m	2
 
 $ r1=$(ls *.py | count-it 'test_(m)')
 $ r2=$(ls | count-it '^test_(.)*.py$' | grep m)
 $ [ "$r1" = "$r2" ]; echo "$?"
 0
+
+#-------------------------------------------------------------------------------
+# TODO": check for bad references
+
+## $ pytest ./mezcla/tests/test_youtube_transcript.py
+## ...
+## ERROR: file or directory not found: ./mezcla/tests/test_youtube_transcript.py
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/conftest.py` & `mezcla-1.4.0.0/mezcla/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt` & `mezcla-1.4.0.0/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb` & `mezcla-1.4.0.0/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py.ipynb` & `mezcla-1.4.0.0/mezcla/tests/jupyter/test_audio_py.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py_experimental.ipynb` & `mezcla-1.4.0.0/mezcla/tests/jupyter/test_audio_py_experimental.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb` & `mezcla-1.4.0.0/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_translation.ipynb` & `mezcla-1.4.0.0/mezcla/tests/jupyter/test_hugging_face_translation.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/jupyter/test_template.ipynb` & `mezcla-1.4.0.0/mezcla/tests/jupyter/test_template.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/misc-tests.batspp` & `mezcla-1.4.0.0/mezcla/tests/misc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/misc_doctests.py` & `mezcla-1.4.0.0/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/misc_tests.py` & `mezcla-1.4.0.0/mezcla/tests/misc_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,7 +76,15 @@
     def test_03_check_permissions(self):
         """Make sure modules don't use certain standard library calls directly
         Note: The mezcla equivalent should be used for sake of debugging traces"""
         debug.trace(4, "test_03_check_permissions()")
         for module in self.get_python_module_files():
             has_execute_perm = gh.run(f'ls -l "{module}" | grep ^...x..x..x')
             self.do_assert(has_execute_perm)
+
+    @pytest.mark.xfail
+    def test_04_usage_statements(self):
+        """Make sure usage statments refer to valid arguments"""
+        debug.trace(4, "test_04_usage_statements()")
+        # note: addresses change like --include-header => --header in randomize_lines.py
+        #   for module in ...: for usage in module usage: assert (not "test_04_usage_statements" in run_script(usage))
+        self.do_assert(False, "TODO: implement")
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/argentinian-attraction-snippets.txt` & `mezcla-1.4.0.0/mezcla/tests/resources/argentinian-attraction-snippets.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.4.0.0/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.4.0.0/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/cars.csv` & `mezcla-1.4.0.0/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/cars.tsv` & `mezcla-1.4.0.0/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/example_text.txt` & `mezcla-1.4.0.0/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.4.0.0/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/iris_output.txt` & `mezcla-1.4.0.0/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/random-10pct-tweet-emotions.tsv` & `mezcla-1.4.0.0/mezcla/tests/resources/random-10pct-tweet-emotions.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.4.0.0/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.4.0.0/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.4.0.0/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/test.arpa` & `mezcla-1.4.0.0/mezcla/tests/resources/test.arpa`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/word-POS.freq` & `mezcla-1.4.0.0/mezcla/tests/resources/word-POS.freq`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/resources/word.freq` & `mezcla-1.4.0.0/mezcla/tests/resources/word.freq`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/template.py` & `mezcla-1.4.0.0/mezcla/examples/tests/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 # Notes:
 # - Fill out TODO's below. Use numbered tests to order (e.g., test_1_usage).
 # - * See test_python_ast.py for simple example of customization.
 # - TODO: If any of the setup/cleanup methods defined, make sure to invoke base
 #   (see examples below for setUp and tearDown).
 # - For debugging the tested script, the ALLOW_SUBCOMMAND_TRACING environment
 #   option shows tracing output normally suppressed by unittest_wrapper.py.
-# - This can be run as follows:
-#   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_<module>.py
+# - This can be run as follows (e.g., from root of repo):
+#   $ pytest ./mezcla/examples/tests/test_<module>.py
 #
 
+## TODO1: [Warning] Make sure this template adhered to as much as possible. For,
+## example, only delete todo comments not regular code, unless suggested in tip).
+## In particular, it is critical that script_module gets initialized properly.
+
 """TODO: Tests for <module> module"""
 
 # Standard modules
 ## TODO: from collections import defaultdict
 
 # Installed modules
 import pytest
@@ -31,28 +35,33 @@
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                        global module object
 #    TestIt.script_module:              path to file
 ## TODO (vvv): insert new module name in commented out template teo lines below
 THE_MODULE = None         ## TODO: remove this line: avoids <module> syntax error in next)
-## import mezcla.<module> as THE_MODULE   ## TODO: uncomment this line (<<<)
+ mezcla.
+import 
+## TODO: ## import <module> as THE_MODULE
+import 
 ## TODO (^^^): use modified line above
+## TODO1: ## import mezcla.examples.<module> as THE_MODULE
 #
 # Note: sanity test for customization (TODO: remove if desired)
 if not my_re.search(__file__, r"\btemplate.py$"):
     debug.assertion("mezcla.template" not in str(THE_MODULE))
 
 ## TODO:
 ## # Environment options
 ## # Note: These are just intended for internal options, not for end users.
 ## # It also allows for enabling options in one place.
 ## #
-## FUBAR = system.getenv_bool("FUBAR", False,
-##                            description="Fouled Up Beyond All Recognition processing")
+## FUBAR = system.getenv_bool(
+##     "FUBAR", False,
+##     description="Fouled Up Beyond All Recognition processing")
 
 #------------------------------------------------------------------------
 
 class TestIt(TestWrapper):
     """Class for command-line based testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     #
@@ -98,17 +107,17 @@
         """Test for something_else: TODO..."""
         debug.trace(4, f"TestIt.test_02_something_else(); self={self}")
         self.do_assert(False)
         ## ex: self.do_assert(THE_MODULE.TODO_function() == TODO_value)
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
-    def test_02_whatever(self):
+    def test_03_whatever(self):
         """TODO: flesh out test for whatever (capsys-like)"""
-        debug.trace(4, f"TestIt2.test_02_whatever(); self={self}")
+        debug.trace(4, f"TestIt2.test_03_whatever(); self={self}")
         THE_MODULE.TODO_whatever()
         captured = self.get_stderr()
         self.do_assert("whatever" in captured, "TODO_whatever trace")
         return
 
     ## TODO: optional cleanup methods
     ##
@@ -125,8 +134,9 @@
     ##     ...
     ##     return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
+    ## TODO2: here and elsewhere: invoke_tests(__file__)
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test___init__.py` & `mezcla-1.4.0.0/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_audio.py` & `mezcla-1.4.0.0/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.4.0.0/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_bing_search.py` & `mezcla-1.4.0.0/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.4.0.0/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_convert_emoticons.py` & `mezcla-1.4.0.0/mezcla/tests/test_convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_cut.py` & `mezcla-1.4.0.0/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_data_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_debug.py` & `mezcla-1.4.0.0/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_evaluate_example_tests.py` & `mezcla-1.4.0.0/mezcla/tests/test_evaluate_example_tests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_extract_document_text.py` & `mezcla-1.4.0.0/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_file_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_filter_random.py` & `mezcla-1.4.0.0/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_format_profile.py` & `mezcla-1.4.0.0/mezcla/tests/test_format_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,66 +87,93 @@
         rstrip_count = system.to_float(my_re.group(1))
         my_re.search(r"^\s*(\S+)\s+.*method 'append'", output, flags=my_re.MULTILINE)
         join_count = system.to_float(my_re.group(1))
         self.do_assert(rstrip_count > join_count)
 
         return
     
+    # Test Helper method
+    @pytest.mark.skip
+    def test_helper_formatprofile(
+        self,
+        key_arg,
+        testing_script,
+        ):
+        """Helper function for format_profile tests"""
+        debug.trace(4, f"test_helper_formatprofile(); self={self}")
+        empty_file = gh.get_temp_file()
+        profile_log = gh.get_temp_file()
+        
+        command1 = f"python3 -m cProfile -o {profile_log} {testing_script}"
+        command2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file}"
+        gh.run(command1)
+        gh.run(command2)
+
+        output = (gh.read_file(empty_file)).split("\n")
+        output = [line.strip() for line in output]        
+        return output
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_cumulative(self):
         "Ensures that test_formatprofile_PK_cumulative works as expected"
 
         key_arg = "cumulative"
         testing_script = "test_glue_helpers.py"
-        SAMPLE_OUTPUT = ["<frozen importlib._bootstrap>:211(_call_with_frames_removed)q", "2    0.000    0.000    0.000    0.000 logging.py:128(_get_auto_indent)"]
-        
-        debug.trace(4, f"test_formatprofile_PK_cumulative(); self={self}")
-        empty_file1 = gh.get_temp_file()
-        profile_log  = gh.get_temp_file()
-        test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
-        test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
+        # OLD: SAMPLE_OUTPUT = ["<frozen importlib._bootstrap>:211(_call_with_frames_removed)q", "2    0.000    0.000    0.000    0.000 logging.py:128(_get_auto_indent)"]
+        SAMPLE_OUTPUT = [
+            "1    0.000    0.000    0.000    0.000 <frozen importlib._bootstrap>:581(_module_repr_from_spec)", 
+            "2    0.000    0.000    0.000    0.000 logging.py:128(_get_auto_indent)"
+        ]
 
-        gh.run(test_command_1)
-        gh.run(test_command_2)
-
-        output = gh.read_file(empty_file1)
+        debug.trace(4, f"test_formatprofile_PK_cumulative(); self={self}")
+        # empty_file1 = gh.get_temp_file()
+        # profile_log  = gh.get_temp_file()
+        # test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
+        # test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
+        # gh.run(test_command_1)
+        # gh.run(test_command_2)
+        # output = gh.read_file(empty_file1)
+        output = self.test_helper_formatprofile(key_arg, testing_script)
         assert (SAMPLE_OUTPUT[0] not in output and SAMPLE_OUTPUT[1] in output)
         return
     
+    ## TODO: Find other input sample
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_cumtime(self):
         "Ensures that test_formatprofile_PK_cumtime works as expected"
-
+        debug.trace(4, f"test_formatprofile_PK_cumtime(); self={self}")
         key_arg = "cumtime"
         testing_script = "test_glue_helpers.py"
-        SAMPLE_OUTPUT = ["_hooks.py:244(__call__)qq", "1    0.000    0.000    0.000    0.000 <attrs generated eq attr.validators._NumberValidator>:1(<module>)"]
-        
-        debug.trace(4, f"test_formatprofile_PK_cumtime(); self={self}")
-        empty_file1 = gh.get_temp_file()
-        profile_log  = gh.get_temp_file()
-        test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
-        test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
+        SAMPLE_OUTPUT = [
+            "_hooks.py:244(__call__)qq", 
+            "1    0.000    0.000    0.000    0.000 <attrs generated eq attr.validators._NumberValidator>:1(<module>)"
+            ]
+        ## OLD
+        # empty_file1 = gh.get_temp_file()
+        # profile_log  = gh.get_temp_file()
+        # test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
+        # test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
 
-        gh.run(test_command_1)
-        gh.run(test_command_2)
+        # gh.run(test_command_1)
+        # gh.run(test_command_2)
 
-        output = gh.read_file(empty_file1)
+        # output = gh.read_file(empty_file1)
+        output = self.test_helper_formatprofile(key_arg, testing_script)
         assert (SAMPLE_OUTPUT[0] not in output and SAMPLE_OUTPUT[1] in output)
-        return
+        # return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_file(self):
         "Ensures that test_formatprofile_PK_file works as expected"
 
-        key_arg = "filename"
+        key_arg = "file"
         testing_script = "test_glue_helpers.py"
         SAMPLE_OUTPUT = ["{built-in method __new__ of type object at 0x909780}", "{built-in method _ssl.txt2obj}"]
         
-        debug.trace(4, f"test_formatprofile_PK_filename(); self={self}")
+        debug.trace(4, f"test_formatprofile_PK_file(); self={self}")
         empty_file1 = gh.get_temp_file()
         profile_log  = gh.get_temp_file()
         test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
         test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
 
         gh.run(test_command_1)
         gh.run(test_command_2)
@@ -159,25 +186,29 @@
     def test_formatprofile_PK_filename(self):
         "Ensures that test_formatprofile_PK_filename works as expected"
 
         key_arg = "filename"
         testing_script = "test_glue_helpers.py"
         SAMPLE_OUTPUT = ["1    0.000    0.000    0.000    0.000 :1(ReprEntryNativeAttributes)", "6768    0.000    0.000    0.000    0.000 :1(ReprEntryAttributes)"]
 
+
+        ## OLD
         debug.trace(4, f"test_formatprofile_PK_filename(); self={self}")
-        empty_file1 = gh.get_temp_file()
-        profile_log  = gh.get_temp_file()
-        test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
-        test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
+        # empty_file1 = gh.get_temp_file()
+        # profile_log  = gh.get_temp_file()
+        # test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
+        # test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
 
-        gh.run(test_command_1)
-        gh.run(test_command_2)
+        # gh.run(test_command_1)
+        # gh.run(test_command_2)
 
-        output = gh.read_file(empty_file1)
-        assert (SAMPLE_OUTPUT[0] in output and SAMPLE_OUTPUT[1] not in output)
+        # output = gh.read_file(empty_file1)
+
+        output = self.test_helper_formatprofile(key_arg, testing_script)
+        assert (SAMPLE_OUTPUT[0] not in output and SAMPLE_OUTPUT[1] not in output)
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_module(self):
         "Ensures that test_formatprofile_PK_module works as expected"
 
         key_arg = "module"
@@ -193,32 +224,34 @@
         gh.run(test_command_1)
         gh.run(test_command_2)
 
         output = gh.read_file(empty_file1)
         assert (SAMPLE_OUTPUT[0] in output)
         return
 
+    ## TODO: Find other input sample
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_ncalls(self):
         "Ensures that test_formatprofile_PK_ncalls works as expected"
 
         key_arg = "ncalls"
         testing_script = "test_glue_helpers.py"
         SAMPLE_OUTPUT = ["{xxyyzzbuilt-in method builtins.len}", "ast.py:222(iter_child_nodes)"]
 
         debug.trace(4, f"test_formatprofile_PK_ncalls(); self={self}")
-        empty_file1 = gh.get_temp_file()
-        profile_log  = gh.get_temp_file()
-        test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
-        test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
 
-        gh.run(test_command_1)
-        gh.run(test_command_2)
-
-        output = gh.read_file(empty_file1)
+        ## OLD
+        # empty_file1 = gh.get_temp_file()
+        # profile_log  = gh.get_temp_file()
+        # test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
+        # test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
+        # gh.run(test_command_1)
+        # gh.run(test_command_2)
+        # output = gh.read_file(empty_file1)
+        output = self.test_helper_formatprofile(key_arg, testing_script)
         assert (SAMPLE_OUTPUT[0] not in output and SAMPLE_OUTPUT[1] in output)
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_pcalls(self):
         "Ensures that test_formatprofile_PK_pcalls works as expected"
 
@@ -362,31 +395,33 @@
         gh.run(test_command_1)
         gh.run(test_command_2)
 
         output = gh.read_file(empty_file1)
         assert (SAMPLE_OUTPUT[0] in output and SAMPLE_OUTPUT[1] not in output)
         return
 
+    ## TODO: Find other input sample
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_formatprofile_PK_tottime(self):
         "Ensures that test_formatprofile_PK_tottime works as expected"
         
         key_arg = "tottime"
         testing_script = "test_glue_helpers.py"
         SAMPLE_OUTPUT = ["<attrs generated init attr.validators._IsCallableValidator>:1(__init__)q", "1    0.000    0.000    0.000    0.000 unix_events.py:1252(ThreadedChildWatcher)"]
 
         debug.trace(4, f"test_formatprofile_PK_tottime(); self={self}")
-        empty_file1 = gh.get_temp_file()
-        profile_log  = gh.get_temp_file()
-        test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
-        test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
-
-        gh.run(test_command_1)
-        gh.run(test_command_2)
-
-        output = gh.read_file(empty_file1)
+        
+        ## OLD
+        # empty_file1 = gh.get_temp_file()
+        # profile_log  = gh.get_temp_file()
+        # test_command_1 = f"python -m cProfile -o {profile_log} {testing_script}"
+        # test_command_2 = f"PROFILE_KEY={key_arg} ../format_profile.py {profile_log} > {empty_file1}"
+        # gh.run(test_command_1)
+        # gh.run(test_command_2)
+        # output = gh.read_file(empty_file1)
+        output = self.test_helper_formatprofile(key_arg, testing_script)
         assert (SAMPLE_OUTPUT[0] not in output and SAMPLE_OUTPUT[1] in output)
         return
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_gensim_test.py` & `mezcla-1.4.0.0/mezcla/tests/test_gensim_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,24 +59,26 @@
         data_file = "LICENSE.txt"
         temp_data_file = self.temp_base + "-" + data_file
         gh.copy_file(gh.resolve_path(data_file), temp_data_file)
         output = self.run_script("--save", temp_data_file)
         ## TODO: assert re.search("storing corpus in Matrix Market format", output)
         assert gh.non_empty_file(temp_data_file.replace(".txt", ".bow.mm"))
         debug.trace_expr(5, output)
+        ## TODO3: check for expected entries (e.g., .wordids.txt.bz2 file)
         return
 
     @pytest.mark.skipif(not gensim, reason="gensim module missing")
     def test_vector_printing(self):
         """Test printing of corpus vector for simple input"""
         tpo.debug_print("test_vector_printing()", 4)
         temp_file = self.temp_base + ".txt"
         gh.write_file(temp_file, "My dog has fleas.\n")
         output = self.run_script("--print --verbose", temp_file)
         assert re.search(r"\(u?'dog', 1\),.*\(u?'has', 1\)", output)
+        ## TODO4: likewise do non-trivial input like LICENSE.txt
         debug.trace_expr(5, output)
         return
 
     
 class TestGensimTest2:
      """Class for internal testcase definitions"""
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_glue_helpers.py` & `mezcla-1.4.0.0/mezcla/tests/test_glue_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 import pytest
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import tpo_common as tpo    # Deprecated, only used for mock
-## OLD: from mezcla.unittest_wrapper import TestWrapper
+from mezcla.unittest_wrapper import TestWrapper
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.glue_helpers as THE_MODULE # pylint: disable=reimported
 
-class TestGlueHelpers:      ## TODO: (TestWrapper)
+class TestGlueHelpers(TestWrapper):      ## TODO: (TestWrapper)
     """Class for testcase definition"""
     ## TEMP
     temp_file = gh.get_temp_file()
 
     def test_get_temp_file(self):
         """Ensure get_temp_file works as expected"""
         debug.trace(4, "test_get_temp_file()")
@@ -101,21 +101,30 @@
         assert(system.file_exists(test_temp_dir))
         assert(not system.file_exists(test_temp_file))
 
     @pytest.mark.xfail
     def test_create_directory(self):
         """Ensure create_directory works as expected"""
         debug.trace(4, "test_create_directory()")
-        assert False
+        assert False, "TODO: implement"
 
     @pytest.mark.xfail
     def test_full_mkdir(self):
         """Ensure full_mkdir works as expected"""
         debug.trace(4, "test_full_mkdir()")
-        assert False
+        temp_dir_abc = gh.form_path(gh.TMP, "a", "b", "c", str(system.get_process_id()))
+        debug.assertion(not system.is_directory(temp_dir_abc))
+        THE_MODULE.full_mkdir(temp_dir_abc)
+        assert  system.is_directory(temp_dir_abc)
+
+    @pytest.mark.xfail
+    def test_get_temp_dir(self):
+        """Tests get_temp_dir"""
+        debug.trace(4, "test_get_temp_dir()")
+        assert False, "TODO: implement"
 
     @pytest.mark.xfail
     def test_real_path(self):
         """Ensure real_path works as expected"""
         debug.trace(4, "test_real_path()")
         debug.assertion(my_re.search("ubuntu", gh.run("uname -a"),
                                      flags=my_re.IGNORECASE))
@@ -154,47 +163,47 @@
         debug.trace(4, "test_elide_values()")
         assert THE_MODULE.elide_values(["1", "22", "333"], max_len=2) == ["1", "22", "33..."]
 
     @pytest.mark.xfail
     def test_disable_subcommand_tracing(self):
         """Ensure disable_subcommand_tracing works as expected"""
         debug.trace(4, "test_disable_subcommand_tracing()")
-        assert False
+        assert False, "TODO: implement"
 
     @pytest.mark.xfail
     def test_run(self):
         """Ensure run works as expected"""
         debug.trace(4, "test_run()")
         assert "root" in THE_MODULE.run("ls /")
 
-    def test_issue(self, monkeypatch, capsys):
+    def test_issue(self):
         """Ensure issue works as expected"""
         debug.trace(4, "test_issue()")
 
         # Simple command test
         temp_file = gh.get_temp_file()
         THE_MODULE.issue(f'echo "this is a simple test" > {temp_file}')
         assert 'this is a simple test' in gh.read_file(temp_file)
 
         # Setup log file
         log_file = gh.get_temp_file()
         system.write_file(log_file, 'random content')
         def debugging_mock():
             return True
-        monkeypatch.setattr(tpo, 'debugging', debugging_mock)
-        monkeypatch.setenv('TEMP_LOG_FILE', log_file, prepend=False)
+        self.monkeypatch.setattr(tpo, 'debugging', debugging_mock)
+        self.monkeypatch.setenv('TEMP_LOG_FILE', log_file, prepend=False)
 
         # Run test with log file
         THE_MODULE.issue('bash bad_filename.bash')
 
         # Check result of test with log file
         if debug.debugging():
-            captured = capsys.readouterr()
-            assert 'stderr' in captured.err
-            assert 'bad_filename.bash' in captured.err
+            captured = self.get_stderr()
+            assert 'stderr' in captured
+            assert 'bad_filename.bash' in captured
         ## TODO: for some reason the log_file is not being overriden
         ## assert 'random content' not in gh.read_file(log_file)
         ## assert 'bad_filename.bash' in gh.read_file(log_file)
 
     def test_get_hex_dump(self):
         """Ensure get_hex_dump works as expected"""
         debug.trace(4, "test_get_hex_dump()")
@@ -253,36 +262,36 @@
 
     def test_count_it(self):
         """Ensure count_it works as expected"""
         debug.trace(4, "test_count_it()")
         assert dict(THE_MODULE.count_it("[a-z]", "Panama")) == {"a": 3, "n": 1, "m": 1}
         assert THE_MODULE.count_it(r"\w+", "My d@wg's fleas have fleas")["fleas"] == 2
 
-    def test_read_lines(self, monkeypatch, capsys):
+    def test_read_lines(self):
         """Ensure read_lines works as expected"""
         debug.trace(4, "test_read_lines()")
 
         # Test valid file
         temp_file = gh.get_temp_file()
         gh.write_file(temp_file, 'file\nwith\nmultiple\nlines\n')
         assert THE_MODULE.read_lines(temp_file) == ['file', 'with', 'multiple', 'lines']
 
         # Test no filename (read from stdin)
-        monkeypatch.setattr('sys.stdin', StringIO('my input\nsome line'))
+        self.monkeypatch.setattr('sys.stdin', StringIO('my input\nsome line'))
         assert THE_MODULE.read_lines() == ['my input', 'some line']
         ## TODO: solve "ValueError: I/O operation on closed file."
         ## THE_MODULE.read_lines()
         ## captured = capsys.readouterr()
         ## assert 'stdin' in captured.err
 
         # Test invalid filename
         assert(not THE_MODULE.read_lines(filename='bad_filename.txt'))
         if debug.debugging():
-            captured = capsys.readouterr()
-            assert 'Warning:' in captured.err
+            captured = self.get_stderr()
+            assert 'Warning:' in captured
 
     def test_write_lines(self):
         """Ensure write_lines works as expected"""
         debug.trace(4, "test_write_lines()")
 
         content = (
             'this is\n'
@@ -347,86 +356,139 @@
         THE_MODULE.rename_file(test_filename, new_test_filename)
 
         # Check integrity of renamed file
         assert gh.file_exists(new_test_filename)
         assert not gh.file_exists(test_filename)
         assert gh.read_file(new_test_filename) == 'some content\n'
 
-    def test_delete_file(self, capsys):
+    def test_delete_file(self):
         """Ensure delete_file works as expected"""
         debug.trace(4, "test_delete_file()")
 
         # Test valid file to delete
         test_filename = gh.get_temp_file()
         gh.write_file(test_filename, 'some content')
         assert gh.file_exists(test_filename)
         THE_MODULE.delete_file(test_filename)
         assert not gh.file_exists(test_filename)
 
         # Test invalid file
         THE_MODULE.delete_file('bad_filename.txt')
         if debug.debugging():
-            captured = capsys.readouterr()
-            assert 'assertion failed' in captured.err.lower()
+            captured = self.get_stderr()
+            assert 'assertion failed' in captured.lower()
 
     def test_file_size(self):
         """Ensure file_size works as expected"""
         debug.trace(4, "test_file_size()")
         temp_file = gh.get_temp_file()
         gh.write_file(temp_file, 'content')
         assert THE_MODULE.file_size(temp_file) == 8
         assert THE_MODULE.file_size('non-existent-file.txt') == -1
 
     @pytest.mark.xfail
     def test_get_matching_files(self):
         """Ensure get_matching_files works as expected"""
         debug.trace(4, "test_get_matching_files()")
-        assert False
+        assert False, "TODO: implement"
 
     @pytest.mark.xfail
     def test_get_files_matching_specs(self):
         """Ensure get_files_matching_specs works as expected"""
         debug.trace(4, "test_get_files_matching_specs()")
-        assert False
+        assert False, "TODO: implement"
 
     @pytest.mark.xfail
     def test_get_directory_listing(self):
         """Ensure get_directory_listing works as expected"""
         debug.trace(4, "test_get_directory_listing()")
         filenames = [gh.get_temp_file() for _ in range(5)]
         for file in filenames:
             gh.write_file(file, 'random content')
         debug.assertion("/tmp" == system.getenv("TMP"))
         filenames = [file.replace('/tmp/', '') for file in filenames]
         assert set(filenames).issubset(THE_MODULE.get_directory_listing('/tmp/'))
 
-    def test_getenv_filename(self, monkeypatch, capfd):
+    def test_getenv_filename(self):
         """Ensure getenv_filename works as expected"""
         debug.trace(4, "test_getenv_filename()")
 
         # Test valid filename with valid content
         test_filename = gh.get_temp_file()
         gh.write_file(test_filename, 'random content')
-        monkeypatch.setenv('TEST_ENV_FILENAME', test_filename, prepend=False)
+        self.monkeypatch.setenv('TEST_ENV_FILENAME', test_filename, prepend=False)
         assert THE_MODULE.getenv_filename('TEST_ENV_FILENAME') == test_filename
 
         # Test valid filename with empty content
         test_filename = gh.get_temp_file()
         with open(test_filename, 'wb') as _:
             pass # gh.write_file cant be used because appends a newline
         debug.set_level(7)
-        monkeypatch.setenv('TEST_ENV_FILENAME', test_filename, prepend=False)
+        self.monkeypatch.setenv('TEST_ENV_FILENAME', test_filename, prepend=False)
         # This avoids flaky tpo.stderr due to other tests
         ## TODO: fix tpo.restore_stderr() to work with pytest 
         tpo.stderr = sys.stderr
         THE_MODULE.getenv_filename('TEST_ENV_FILENAME')
-        captured = capfd.readouterr() # Note: capfd must be used instead of capsys to capture stderr
-        assert 'Error' in captured.err
-        assert test_filename in captured.err
+        captured = self.get_stderr() # Note: capfd must be used instead of capsys to capture stderr
+        assert 'Error' in captured
+        assert test_filename in captured
 
         # Test non enviroment var
         assert THE_MODULE.getenv_filename('BAD_ENV_FILE_VAR', default='missing-file') == 'missing-file'
 
+    @pytest.mark.xfail
+    def test_copy_directory(self):
+        """Ensure copy_directory works as expected"""
+        debug.trace(4, "test_copy_directory()")
+        temp_dir = '/tmp/test_copy_dir_'
+        system.create_directory(f'{temp_dir}1')
+        system.write_file(f'{temp_dir}1/test_file', "copy")
+        assert 'test_file' in system.read_directory(THE_MODULE.copy_directory(f'{temp_dir}1', f'{temp_dir}2'))
+        assert 'copy' in system.read_file(f'{temp_dir}2/test_file')
 
+    @pytest.mark.xfail
+    def test_delete_directory(self):
+        """Ensure delete_directory works as expected"""
+        debug.trace(4, "test_delete_directory()")
+        old = THE_MODULE.DISABLE_RECURSIVE_DELETE
+
+        # test an empty directory gets deleted
+        empty_dir = '/tmp/test_delete_directory-1/'
+        system.create_directory(empty_dir)
+        assert THE_MODULE.is_directory(empty_dir)
+        assert THE_MODULE.delete_directory(empty_dir) is None
+
+        # test a directory with files gets deleted
+        non_empty_dir = '/tmp/test_delete_directory-2'
+        system.create_directory(non_empty_dir)
+        system.write_file(f'{non_empty_dir}/test_delete_directory', '2')
+        assert THE_MODULE.is_directory(non_empty_dir)
+        assert THE_MODULE.delete_directory(non_empty_dir) is None
+
+        # test a directory with subdirs doesnt get deleted if DISABLE_RECURSIVE_DELETE
+        THE_MODULE.DISABLE_RECURSIVE_DELETE = True
+        dir_with_subdirs = '/tmp/test_delete_directory-3'
+        subdir = f"{dir_with_subdirs}/subdir"
+        system.create_directory(dir_with_subdirs)
+        system.create_directory(subdir)
+        system.write_file(f"{subdir}/subdir_file", '3')
+        assert THE_MODULE.is_directory(subdir)
+        assert not THE_MODULE.delete_directory(dir_with_subdirs)
+
+        # test a directory with subdirs gets deleted if not DISABLE_RECURSIVE_DELETE
+        assert THE_MODULE.is_directory(subdir)
+        system.write_file(f"{subdir}/subdir_file", '4')
+        THE_MODULE.DISABLE_RECURSIVE_DELETE = False
+        assert THE_MODULE.delete_directory(dir_with_subdirs) is None
+
+        THE_MODULE.DISABLE_RECURSIVE_DELETE = old
+
+    @pytest.mark.xfail
+    def test_initialization(self):
+        """Make sure module initialized OK"""
+        # TODO1: add checks for TEMP_BASE and TEMP_FILE, along with PRESERVE_TEMP_FILE
+        # TODO3: add checks for TEMP_LOG_FILE and TEMP_SCRIPT_FILE
+        assert False, "TODO: implement"
+        
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_html_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_html_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,29 @@
 ## OLD: import bs4
 
 # Local packages
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla import debug
 from mezcla import system
 from mezcla import glue_helpers as gh
+from mezcla.my_regex import my_re
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 ## TODO: template => new name
 import mezcla.html_utils as THE_MODULE
 
 # Environment options
 TEST_SELENIUM = system.getenv_bool("TEST_SELENIUM", False,
                                    "Include tests requiring selenium")
 
 class TestHtmlUtils(TestWrapper):
     """Class for testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__)
+    scrappycito_url = "http://www.scrappycito.com"
     # TODO: use_temp_base_dir = True            # treat TEMP_BASE as directory
     # note: temp_file defined by parent (along with script_module, temp_base, and test_num)
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_get_browser(self):
         """Ensure get_browser() works as expected"""
         debug.trace(4, "test_get_browser()")
@@ -98,14 +100,30 @@
         debug.trace_expr(5, rendered_html)
         assert re.search(
             r"<li>Browser dimensions:\s*<span.*>\d+x\d+</span></li>",
             rendered_html,
             )
 
     @pytest.mark.xfail                   # TODO: remove xfail
+    def test_get_inner_html_alt(self):
+        """Alternative test of get_inner_html"""
+        debug.trace(4, f"TestIt.test_get_inner_html_alt(); self={self}")
+        output = THE_MODULE.get_inner_html(self.scrappycito_url)
+        self.do_assert(not my_re.search(r"sign.out", output.strip(), flags=my_re.IGNORECASE))
+        return
+
+    @pytest.mark.xfail                   # TODO: remove xfail
+    def test_run_script_for_inner_html(self):
+        """Test of getting inner HTML via script invocation"""
+        debug.trace(4, f"TestIt.test_run_script_for_inner_html(); self={self}")
+        output = self.run_script(options=f"--inner --stdout {self.scrappycito_url}", data_file=self.temp_file)
+        self.do_assert(not my_re.search(r"sign.out", output.strip(), flags=my_re.IGNORECASE))
+        return
+
+    @pytest.mark.xfail                   # TODO: remove xfail
     def test_document_ready(self):
         """Ensure document_ready() works as expected"""
         debug.trace(4, "test_document_ready()")
         assert False, "TODO: code test"
 
     def test_escape_html_value(self):
         """Ensure escape_html_value() works as expected"""
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_ipython_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_ipython_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_kenlm_example.py` & `mezcla-1.4.0.0/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_keras_param_search.py` & `mezcla-1.4.0.0/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_main.py` & `mezcla-1.4.0.0/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_merge_files.py` & `mezcla-1.4.0.0/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_merge_notes.py` & `mezcla-1.4.0.0/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_misc_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_my_regex.py` & `mezcla-1.4.0.0/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.4.0.0/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_os_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_os_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     def test_split_extension(self):
         """Ensure test_split_extension works as expected"""
         assert(os_utils.split_extension("fubar.txt") == ("fubar", ".txt"))
 
 
 if __name__ == '__main__':
     debug.trace_current_context()
-    invoke_tests([__file__])
+    invoke_tests(__file__)
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.4.0.0/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_plot_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_python_ast.py` & `mezcla-1.4.0.0/mezcla/tests/test_python_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_randomize_lines.py` & `mezcla-1.4.0.0/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.4.0.0/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.4.0.0/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.4.0.0/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.4.0.0/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_simple_main_example.py` & `mezcla-1.4.0.0/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.4.0.0/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_spell.py` & `mezcla-1.4.0.0/mezcla/tests/test_spell.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 # Test(s) for ../spell.py
 #
 # Notes:
 # - For debugging the tested script, the ALLOW_SUBCOMMAND_TRACING environment
 #   option shows tracing output normally suppressed by  unittest_wrapper.py.
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_bing_search.py
+# - Spellcheck requires nltk and hunspell for multi-language support
+#   Language specific hunspell can be installed as hunspell-LANG_CODE (e.g. hunspell-ne -> Nepali)
+#   $ apt-get install hunspell-ne 
 #
 # TODO1:
 # - Rework tests following test_spell_EN
 # - Carefully review tests/template.py.
 # TODO3:
 # - Create test helpers to cut down on all the redundant code.
 #   ex: def check_spelling(self, lang, text, bad):
@@ -28,15 +31,15 @@
 import pytest
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla import system
 from mezcla.unittest_wrapper import TestWrapper
-from mezcla.unittest_wrapper import trap_exception
+## TODO: from mezcla.unittest_wrapper import trap_exception
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 #    TestIt.script_module:              path to file
 try:
     # note: requires enchant-2 library package under Ubuntu (besides pyenchant)
     import mezcla.spell as THE_MODULE
@@ -57,225 +60,266 @@
 ## elif (echo_PWD.endswith('/mezcla')):
 ##     SPELL_PATH = PATH1
 ## else:
 ##     SPELL_PATH = PATH3
 ##
 ## NOTE: the following is a temporary workaround for the bad tests
 ## TODO1: use run_script as in the template (and in most other tests elsewhere)!
-SPELL_PATH = gh.resolve_path("spell.py")
+SPELL_PATH = gh.resolve_path("../spell.py")
+
+## Environment Variables
+RUN_SLOW_TESTS = system.getenv_bool(
+    "RUN_SLOW_TESTS", 
+    False,
+    description="Run tests that can a while to run"
+    )
+
+# @pytest.mark.skipif(not THE_MODULE, reason="Problem loading spell.py: check requirements")
 
-@pytest.mark.skipif(not THE_MODULE, reason="Problem loading spell.py: check requirements")
 class SpellFiles(TestWrapper):
     """Class for testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     use_temp_base_dir = True    # treat TEMP_BASE as directory
-             
+         
     # NOTE 1: For test_phrase, song lyrics are used
     # NOTE 2: The content in test_phase error MUST be all lowercase
+    # NOTE 3: Standard assertion case: assert (output in test_phrase_error and len(output) != 0)
     # TODO 1: Find a method to not create any external filess when test_spell_query_LL functions used
     # TODO 2: A function for test_run_command replacement (optional)
 
+    # Function A: Helper Function reduces the amount of code to be written
+    @pytest.mark.skip
+    def test_helper(self, 
+                    lang_code:str="en_EN", 
+                    phrase:str="Hello World", 
+                    batch_file_path:str="-"
+                    ):
+        """Helper function for test_spell.py"""
+        debug.trace(4, f"\ntest_helper(); self={self}")
+
+        if batch_file_path == "-":
+            command = f'echo "{phrase}" | SPELL_LANG={lang_code} {SPELL_PATH} {batch_file_path}'
+        else:
+            command = f'SPELL_LANG={lang_code} {SPELL_PATH} {batch_file_path}'
+
+        output = gh.run(command)
+        debug.trace_expr(5, output, lang_code, phrase, batch_file_path)        
+        return output
+    
+    # Function B: Helper Function for query-like tests (skipped by defau)
+    @pytest.mark.skip
+    def test_helper_tempfile(self,
+                          lang_code:str="en_EN",
+                          phrase:str="Hello World"
+                          ):
+        """Helper function using tempfile"""
+        debug.trace(4, f"\ntest_helper_tempfile(); self={self}")
+
+        temp_phrase = f"{self.temp_file}.phrase"
+        test_run_command_1 = f'echo "{phrase}" > {temp_phrase}'
+        test_run_command_2 = f'SPELL_LANG={lang_code} {SPELL_PATH} {temp_phrase} > {self.temp_file}'
+        
+        gh.issue(test_run_command_1)
+        output = gh.run(test_run_command_2)
+        output = self.run_script(self.temp_file)
+        debug.trace_expr(5, output, lang_code, phrase)
+        return output
+    
+    # @pytest.mark.skip
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_default(self):
         """Ensure test_spell_default [English] works as expected"""
-        debug.trace(4, f"test_spell_default(); self={self}")
-        ## OLD: test_lang = "en_EN"
+        debug.trace(4, f"\ntest_spell_default(); self={self}")
+        
         test_phrase = "One kiss is all it tajkes"
-        ## ORGINAL: One kiss is all it takes (from One Kiss by Calvin Harris, Dua Lipa)
-        test_run_command = f'echo "{test_phrase}" | {SPELL_PATH} -'
-        output = gh.run(test_run_command)
-        assert (output != "" and len(output.split())==1)
-        return
+        test_phrase_error = "tajkes"
+        output = self.test_helper(phrase=test_phrase)
 
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output == test_phrase_error and len(output) != 0)
 
+    # @pytest.mark.xfail                   # TODO: remove xfail
+    # @trap_exception                      # TODO: remove when debugged
     @pytest.mark.xfail                   # TODO: remove xfail
-    @trap_exception                      # TODO: remove when debugged
     def test_spell_EN(self):
         """Ensure test_spell_EN [English] works as expected"""
-        debug.trace(4, f"test_spell_EN(); self={self}")
+        debug.trace(4, f"\ntest_spell_EN(); self={self}")
         
         test_lang = "en_EN"
-        test_phrase = "One kiss is all it takesqq"
-        test_phrase_error = "takesqq"
-        ## BAD: test_run_command = f'echo "{test_phrase}" | SPELL_LANG={test_lang} {SPELL_PATH} - > {self.temp_file}'
-        # LITERAL TRANSLATION: N/A  
-        system.write_file(self.temp_file, test_phrase)
-        output = self.run_script(env_options=f"SPELL_LANG={test_lang}", data_file=self.temp_file)
-        debug.trace_expr(5, output, test_phrase_error)
-        assert (output == test_phrase_error)
+        test_phrase = "You givc me that feeling"
+        test_phrase_error = "givc"
+
         ## TODO: maldito vs code so awkward to use!
+        output = self.test_helper(test_lang, test_phrase)
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output in test_phrase_error and len(output) != 0)
         return
 
+    ## OLD: @pytest.mark.xfail
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")               
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_ES(self):
         """Ensure test_spell_ES [Spanish] works as expected"""
-        debug.trace(4, f"test_spell_ES(); self={self}")
-
+        debug.trace(4, f"\ntest_spell_ES(); self={self}")
+        
         test_lang = "es_ES"
         test_phrase = "Yo te miro y se me corta la respiraciónqq"
         test_phrase_error = "respiraciónqq"
-        ## TODO1: rework using run_script
-        test_run_command = f'echo "{test_phrase}" | SPELL_LANG={test_lang} {SPELL_PATH} - > {self.temp_file}'
-        # LITERAL TRANSLATION: "I look at you and my breath catches"
-        test_run_command = f'echo "{test_phrase}" | SPELL_LANG={test_lang} {SPELL_PATH} -'
-        output = gh.run(test_run_command)
-
-        ## TODO2: output = self.run_script(self.temp_file)
-        assert (output == test_phrase_error)
+        output = self.test_helper(test_lang, test_phrase)
+        
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output in test_phrase and len(output) != 0)
         return
-    
+
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")               
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_NE(self):
         """Ensure test_spell_NE [Nepali] works as expected"""
+        debug.trace(4, f"\ntest_spell_NE(); self={self}")
         
         test_lang = "ne_NE"
-        test_phrase = "थाहा छैन तिमी को हो मेरोqq"
-        test_phrase_error = "मेरोqq"
-        test_run_command = f'echo "{test_phrase}" | SPELL_LANG={test_lang} {SPELL_PATH} - > {self.temp_file}'
-        # LITERAL TRANSLATION: "I don't know who you are"
-        # WARN: ne_NE dictionary may not have some words
-        output = gh.run(test_run_command)
-         
-        debug.trace(4, f"test_spell_NE(); self={self}")
-        ## TODO2: output = output = self.run_script(self.temp_file)
-        assert (output == test_phrase_error)
+        test_phrase = "थाहा छैन तिमीर को हो मेरो"
+        test_phrase_error = "तिमीर"
+        output = self.test_helper(lang_code=test_lang, phrase=test_phrase)
+        
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output in test_phrase and len(output) != 0)
         return
 
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_AR(self):
         """Ensure test_spell_AR [Arabic] works as expected"""
         debug.trace(4, f"test_spell_AR(); self={self}")
+
         test_lang = "ar_AR"
-        test_phrase = "وإنت معايا بشوفك أحلى النس"
-        ## ORIGINAL: وإنت معايا بشوفك أحلى الناس (from Bayen Habeit by Marshmello, Amr Diab)
-        ## Literal: When you are with me, I see you as the most beautiful person
-        test_run_command = f'echo "{test_phrase}" | SPELL_LANG={test_lang} {SPELL_PATH} -'
-        ## TODO2: output = output = self.run_script(self.temp_file)
-        output = gh.run(test_run_command)
-        assert (output != "" and len(output.split())==2)
+        test_phrase = "سعلينا الهوى وغنّا"
+        output = self.test_helper(test_lang, test_phrase)
+        
+        debug.trace_expr(5, output, test_phrase)
+        assert (output in test_phrase and len(output)!=0)
         return
     
-    @pytest.mark.skip                   # TODO: remove xfail
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
+    @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_RU(self):
         """Ensure test_spell_RU [Russian] works as expected"""
         debug.trace(4, f"test_spell_RU(); self={self}")
+        
         test_lang = "ru_RU"
         test_phrase = "Поплыли туманыны над рекой"
-        ## ORIGINAL: Поплыли туманы над рекой (from Катюша by M. Blanter)
-        ## Literal: Fogs floated over the river
-        test_run_command = f'echo "{test_phrase}" | SPELL_LANG={test_lang} {SPELL_PATH} -'
-        ## TODO2: output = output = self.run_script(self.temp_file)
-        output = gh.run(test_run_command)
-        assert (output != "" and len(output.split())==1)
+        output = self.test_helper(test_lang, test_phrase)
+        
+        debug.trace_expr(5, output, test_phrase)
+        assert (output in test_phrase and len(output) != 0)
         return
     
+    # Marked as slow test (takes a lot of time on pytest)
+    @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_query_EN(self):
         """Ensure test_spell_query_EN works as expected"""
-        
+        debug.trace(4, f"test_spell_query_EN(); self={self}")
+
         test_lang = "en_EN"
-        test_phrase = "Because I am lost in the way you moveqq"
-        # LITERAL TRANSLATION: N/A
-        ## BAD: temp_phrase = None
-        temp_phrase = f"{self.temp_file}.phrase"
-        test_run_command_1 = f'echo "{test_phrase}" > {temp_phrase}'
-        test_run_command_2 = f'SPELL_LANG={test_lang} {SPELL_PATH} {temp_phrase} > {self.temp_file}'
+        test_phrase = "Because I am lostr in the way you move"
+        test_phrase_error = "lostr"
+        output = self.test_helper_tempfile(test_lang, test_phrase)
 
-        test_phrase_error = "moveqq"
-         
-        debug.trace(4, f"test_spell_query_EN(); self={self}")
-        gh.issue(test_run_command_1)
-        output = gh.run(test_run_command_2)
-        ## TODO: output = self.run_script(self.temp_file)
-        assert (output == test_phrase_error)
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output == test_phrase_error and len(output) != 0)
         return
-    
+
+    # Marked as slow test (takes a lot of time on pytest)
+    @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_query_ES(self):
         """Ensure test_spell_query_ES works as expected"""
+        debug.trace(4, f"test_spell_query_ES(); self={self}")
+
         
         test_lang = "es_ES"
-        test_phrase = "Me dijeron que te estás casandoxx"
-        # LITERAL TRANSLATION: "They told me that you are getting married"
-        ## BAD: temp_phrase = None
-        temp_phrase = f"{self.temp_file}.phrase"
-        test_run_command_1 = f'echo "{test_phrase}" > {temp_phrase}'
-        test_run_command_2 = f'SPELL_LANG={test_lang} {SPELL_PATH} {temp_phrase} > {self.temp_file}'
-        test_phrase_error = "casandoxx"
-         
-        debug.trace(4, f"test_spell_query_ES(); self={self}")
-        gh.issue(test_run_command_1)
-        output = gh.run(test_run_command_2)
-        output = self.run_script(self.temp_file)
-        assert (output == test_phrase_error)
+        test_phrase = "Me dijeron que te estás casandoi"
+        test_phrase_error = "casandoi"
+        output = self.test_helper_tempfile(test_lang, test_phrase)
+        
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output == test_phrase_error and len(output) != 0)
         return
 
+    # Marked as slow test (takes a lot of time on pytest)
+    @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_query_NE(self):
         """Ensure test_spell_query_NE works as expected"""
-        
+        debug.trace(4, f"test_spell_query_NE(); self={self}")
+
         test_lang = "ne_NE"
-        test_phrase = "तिमी नै अब मेरो झुल्केको बिहानीxx"
-        # LITERAL TRANSLATION: You are now my rising dawn
-        ## BAD: temp_phrase = None
-        temp_phrase = f"{self.temp_file}.phrase"
-        test_run_command_1 = f'echo "{test_phrase}" > {temp_phrase}'
-        test_run_command_2 = f'SPELL_LANG={test_lang} {SPELL_PATH} {temp_phrase} > {self.temp_file}'
+        test_phrase = "तिमी नै अबप मेरो झुल्केको बिहानी"
+        test_phrase_error = "अबप"
+        output = self.test_helper_tempfile(test_lang, test_phrase)
 
-        test_phrase_error = "बिहानीxx"
-         
-        debug.trace(4, f"test_spell_query_NE(); self={self}")
-        gh.issue(test_run_command_1)
-        output = gh.run(test_run_command_2)
-        output = self.run_script(self.temp_file)
-        assert (output == test_phrase_error)
+        debug.trace_expr(5, output, test_phrase_error)
+        assert (output in test_phrase and len(output) != 0)
         return
 
+    # Marked as slow test (takes a lot of time on pytest)
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_default_batch(self):
         """Ensure test_spell_default_batch [English] works as expected"""
         debug.trace(4, f"test_spell_default_branch(); self={self}")
+        
         testfile_path = gh.resolve_path("./resources/spell-py-en.list")
-        test_run_command = f'python3 {SPELL_PATH} {testfile_path}'
-        output = gh.run(test_run_command).split("\n")
-        ## TODO2: make the tests more flexible (e.g., don't test for specific length)
-        assert (output != "" and len(output)==10)    # Error Message contains large amount of characters
+        output = (self.test_helper(batch_file_path=testfile_path)).split("\n")
+        
+        debug.trace_expr(5, output)
+        assert (output != [] and len(output) > 5)
         return
     
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_ES_batch(self):
         """Ensure test_spell_ES_batch [Spanish] works as expected"""
         debug.trace(4, f"test_spell_ES_batch(); self={self}")
+        
         test_lang = "es_ES"
         testfile_path = gh.resolve_path("./resources/spell-py-es.list")
-        test_run_command = f'SPELL_LANG={test_lang} python3 {SPELL_PATH} {testfile_path}'
-        output = gh.run(test_run_command).split("\n")
-        assert (output != "" and len(output)==10)    # Error Message contains large amount of characters
+        output = (self.test_helper(lang_code=test_lang, batch_file_path=testfile_path)).split("\n")
+        
+        debug.trace_expr(5, output)
+        assert (output != [] and len(output) > 3)
         return
     
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_RU_batch(self):
         """Ensure test_spell_RU_batch [Russian] works as expected"""
         debug.trace(4, f"test_spell_RU_batch(); self={self}")
+        
         test_lang = "ru_RU"
         testfile_path = gh.resolve_path("./resources/spell-py-ru.list")
-        test_run_command = f'SPELL_LANG={test_lang} python3 {SPELL_PATH} {testfile_path}'
-        output = gh.run(test_run_command).split("\n")
-        assert (output != "" and len(output)==5)    # Error Message contains large amount of characters
+        output = (self.test_helper(lang_code=test_lang, batch_file_path=testfile_path)).split("\n")
+        
+        debug.trace_expr(5, output)
+        assert (output != [] and len(output) > 3)
         return
     
+    # @pytest.mark.skipif(not RUN_SLOW_TESTS, reason="This test can take some time or may have missing libraries")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_AR_batch(self):
         """Ensure test_spell_AR_batch [Arabic] works as expected"""
         debug.trace(4, f"test_spell_AR_batch(); self={self}")
+        
         test_lang = "ar_AR"
         testfile_path = gh.resolve_path("./resources/spell-py-ar.list")
-        test_run_command = f'SPELL_LANG={test_lang} python3 {SPELL_PATH} {testfile_path}'
-        output = gh.run(test_run_command).split("\n")
-        assert (output != "" and len(output)==17)    # Error Message contains large amount of characters
+        output = (self.test_helper(lang_code=test_lang, batch_file_path=testfile_path)).split("\n")
+        
+        debug.trace_expr(5, output)
+        assert (output != "" and len(output)>5)
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_spell_LANG_suggest(self):
         """Ensure test_spell_LANG_suggest works as expected"""
         debug.trace(4, f"test_suggest_LANG(); self={self}")
         self.do_assert(False, "TODO: code test")
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.4.0.0/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_system.py` & `mezcla-1.4.0.0/mezcla/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_template.py` & `mezcla-1.4.0.0/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_text_categorizer.py` & `mezcla-1.4.0.0/mezcla/tests/test_text_categorizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,22 @@
 from mezcla.my_regex import my_re
 from mezcla import system
 from mezcla import misc_utils
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 system.setenv("USE_XGB", "1")
-import mezcla.text_categorizer as THE_MODULE
+THE_MODULE = None
+try:
+    ## TEMP: fails if xgboost not available (workaround for stupid docker issue)
+    import xgboost
+    debug.trace_expr(5, xgboost.XGBClassifier)
+    import mezcla.text_categorizer as THE_MODULE
+except:
+    system.print_exception_info("text_categorizer import")
 
 # Environment options
 TEST_TBD = system.getenv_bool("TEST_TBD", False,
                               description="Test features to be designed: TBD")
 
 
 class TestTextCategorizerUtils(TestWrapper):
@@ -51,14 +58,15 @@
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_read_categorization_data(self):
         """Ensure read_categorization_data works as expected"""
         debug.trace(4, "test_read_categorization_data()")
         assert(False)
 
+    @pytest.mark.xfail                   # TODO: remove xfail
     def test_int_if_whole(self):
         """Ensure int_if_whole works as expected"""
         debug.trace(4, "test_int_if_whole()")
         assert THE_MODULE.int_if_whole(2.0) == 2
         assert THE_MODULE.int_if_whole(2.999) == 2.999
 
     @pytest.mark.xfail                   # TODO: remove xfail
@@ -107,28 +115,26 @@
     def test_usage(self):
         """Test usage statement"""
         # Current usage:
         #   Usage: ./text_categorizer.py model
         usage = self.run_script(options="--help")
         assert "model" in usage
     
-    @trap_exception
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_test_untrained(self):
         """Make sure accuracy 0 if untrained (TODO: trap stderr)"""
         debug.trace(4, "test_test_untrained()")
         tc = THE_MODULE.TextCategorizer()
         ## OLD: accuracy = tc.test(__file__)
         test_data = ["cat1\ta b c d e",
                      "cat2\tf g h i j"]
         gh.write_lines(self.temp_file, test_data)
         accuracy = tc.test(self.temp_file)
         assert(accuracy == 0)
 
-    @trap_exception
     @pytest.mark.xfail
     def test_train(self):
         """Make sure training works"""
         debug.trace(4, "test_train()")
         data_file = gh.form_path(self.resources, "random-10pct-tweet-emotions.tsv")
         data = system.read_lines(data_file)
         tc = THE_MODULE.TextCategorizer(use_xgb=True)
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_text_processing.py` & `mezcla-1.4.0.0/mezcla/tests/test_text_processing.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,55 +8,64 @@
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_text_processing.py
 #
 
 """Tests for text_processing module"""
 
 # Standard packages
-## NOTE: this is empty for now
-
-# Installed packages
 import pytest
+import re
+# Installed packages
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla import system
+from mezcla.my_regex import my_re
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla.unittest_wrapper import trap_exception
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.text_processing as THE_MODULE
 
 # Constants
 RESOURCES = f'{gh.dir_path(__file__)}/resources'
 TEXT_EXAMPLE = f'{RESOURCES}/example_text.txt'
 TEXT_EXAMPLE_TAGS = f'{RESOURCES}/example_text_tags.txt'
 WORD_POS_FREQ_FILE = f'{RESOURCES}/word-POS.freq'
+WORD_FREQ_FILE = f'{RESOURCES}/word.freq'
 
-class TestTextProcessing:
+class TestTextProcessing(TestWrapper):
     """Class for testcase definition"""
 
     def test_split_sentences(self):
         """Ensure split_sentences works as expected"""
         debug.trace(4, "test_split_sentences()")
         assert THE_MODULE.split_sentences("I came. I saw. I conquered!") == ["I came.", "I saw.", "I conquered!"]
         assert THE_MODULE.split_sentences("Dr. Watson, it's elementary. But why?") == ["Dr. Watson, it's elementary.", "But why?"]
 
     def test_split_word_tokens(self):
         """Ensure split_word_tokens works as expected"""
         debug.trace(4, "test_split_word_tokens()")
         assert THE_MODULE.split_word_tokens("How now, brown cow?") == ['How', 'now', ',', 'brown', 'cow', '?']
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_label_for_tag(self):
         """Ensure label_for_tag works as expected"""
         debug.trace(4, "test_label_for_tag()")
-        assert False, "TODO: code test"
+        previous_value = THE_MODULE.KEEP_PUNCT
+        
+        self.monkeypatch.setattr(THE_MODULE, 'KEEP_PUNCT', True)
+        assert THE_MODULE.label_for_tag("SYM", ',') == ','
+        assert THE_MODULE.label_for_tag("SYM", '?') == '?'
+        self.monkeypatch.setattr(THE_MODULE, 'KEEP_PUNCT', False)
+        assert THE_MODULE.label_for_tag("SYM", ',') == 'SYM'
+        assert THE_MODULE.label_for_tag("SYM", '?') == 'SYM'
+        self.monkeypatch.setattr(THE_MODULE, 'KEEP_PUNCT', previous_value)
+        
 
     def test_class_for_tag(self):
         """Ensure class_for_tag works as expected"""
         debug.trace(4, "test_class_for_tag()")
         assert THE_MODULE.class_for_tag("NNS") == "noun"
         assert THE_MODULE.class_for_tag("VBG") == "verb"
         assert THE_MODULE.class_for_tag("VBG", previous="MD") == "verb"
@@ -67,49 +76,69 @@
         debug.trace(4, "test_tag_part_of_speech()")
         # NOTE:
         #   'brown' tagged as IN is wrong, should be JJ, this is a problem related to NLTK
         #   not the module being tested, so we are ignoring it for now.
         #   Related: https://stackoverflow.com/a/30823202
         assert THE_MODULE.tag_part_of_speech(['How', 'now', ',', 'brown', 'cow', '?']) == [('How', 'WRB'), ('now', 'RB'), (',', ','), ('brown', 'IN'), ('cow', 'NN'), ('?', '.')]
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_tokenize_and_tag(self):
         """Ensure tokenize_and_tag works as expected"""
         debug.trace(4, "test_tokenize_and_tag()")
-        assert False, "TODO: code test"
+        # NOTE:
+        #   'brown' tagged as IN is wrong, should be JJ, this is a problem related to NLTK
+        #   not the module being tested, so we are ignoring it for now.
+        #   Related: https://stackoverflow.com/a/30823202
+        assert THE_MODULE.tokenize_and_tag("How now, brown cow ?") == [('How', 'WRB'), ('now', 'RB'), (',', ','), ('brown', 'IN'), ('cow', 'NN'), ('?', '.')]
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_tokenize_text(self):
         """Ensure tokenize_text works as expected"""
         debug.trace(4, "test_tokenize_text()")
-        assert False, "TODO: code test"
+        assert THE_MODULE.tokenize_text("I came. I saw. I conquered!") == [['I', 'came', '.'], ['I', 'saw', '.'], ['I', 'conquered', '!']]
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_is_stopword(self):
         """Ensure is_stopword works as expected"""
         debug.trace(4, "test_is_stopword()")
-        assert False, "TODO: code test"
+        assert THE_MODULE.is_stopword('we')
+        assert THE_MODULE.is_stopword('i')
+        assert not THE_MODULE.is_stopword('cow')
 
-    @pytest.mark.xfail                   # TODO: remove xfail
+    @pytest.mark.xfail
     def test_has_spelling_mistake(self):
         """Ensure has_spelling_mistake works as expected"""
         debug.trace(4, "test_has_spelling_mistake()")
-        assert False, "TODO: code test"
+        previous_value = THE_MODULE.SKIP_ENCHANT
+        self.monkeypatch.setattr(THE_MODULE, 'SKIP_ENCHANT', True)
+        assert not THE_MODULE.has_spelling_mistake('the')
+        assert THE_MODULE.has_spelling_mistake('ai')
+        self.monkeypatch.setattr(THE_MODULE, 'SKIP_ENCHANT', False)
+        assert not THE_MODULE.SKIP_ENCHANT
+        assert THE_MODULE.has_spelling_mistake('sneik')
+        assert not THE_MODULE.has_spelling_mistake('snake')
+        
+        self.monkeypatch.setattr(THE_MODULE, 'SKIP_ENCHANT', previous_value)
+        
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_read_freq_data(self):
         """Ensure read_freq_data works as expected"""
         debug.trace(4, "test_read_freq_data()")
-        assert False, "TODO: code test"
+        lines = gh.read_lines(WORD_FREQ_FILE)
+        freq = THE_MODULE.read_freq_data(WORD_FREQ_FILE)
+        for line in lines[7:]:
+            token = re.match(r'^.+?(?=\s)', line).group(0).lower()
+            self.do_assert(freq[token])
+
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_read_word_POS_data(self): # pylint: disable=invalid-name
         """Ensure read_word_POS_data works as expected"""
         debug.trace(4, "test_read_word_POS_data()")
-        assert False, "TODO: code test"
+        lines = gh.read_lines(WORD_POS_FREQ_FILE)
+        freq_pos = THE_MODULE.read_word_POS_data(WORD_POS_FREQ_FILE)
+        for line in lines[6:]:
+            token = re.match(r'^.+?(?=\s)', line).group(0).lower()
+            self.do_assert(freq_pos[token])
 
     def test_get_most_common_POS(self): # pylint: disable=invalid-name
         """Ensure get_most_common_POS works as expected"""
         debug.trace(4, "test_get_most_common_POS()")
         # Testing if word_POS_hash is not none
         THE_MODULE.word_POS_hash = {
             'can': 'MD'
@@ -161,50 +190,61 @@
 
     def test_is_punct(self):
         """Ensure is_punct works as expected"""
         debug.trace(4, "test_is_punct()")
         assert THE_MODULE.is_punct('$', '$')
         assert not THE_MODULE.is_punct('can', 'MD')
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_usage(self):
         """Ensure usage works as expected"""
         debug.trace(4, "test_usage()")
-        assert False, "TODO: code test"
-
+        THE_MODULE.usage()
+        captured = self.get_stderr()
+        assert f"Usage: {THE_MODULE.__file__} [--help] [--just-tokenize] [--just-chunk] [--lowercase] file" in captured
+        assert f"echo \"My dawg has fleas.\" | {THE_MODULE.__file__} -" in captured
+        assert "- Intended more as a library module" in captured
+        assert "- In standalone mode it runs the text processing pipeline over the file:" in captured
+        assert "sentence splitting, word tokenization, and part-of-speech tagging" in captured
+        assert "- Set SKIP_NLTK environment variable to 1 to disable NLTK usage." in captured
 
 class TestTextProcessingScript(TestWrapper):
     """Class for testcase definition"""
     script_file = TestWrapper.get_module_file_path(__file__)
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
 
     def test_all(self):
         """Ensure text_processing without argument works as expected"""
         debug.trace(4, "test_all()")
         output = self.run_script(data_file=TEXT_EXAMPLE)
         assert output == gh.read_file(TEXT_EXAMPLE_TAGS)[:-1]
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_just_tokenize(self):
         """Ensure just_tokenize argument works as expected"""
         debug.trace(4, "test_just_tokenize()")
-        self.do_assert(False, "TODO: code test")
+        tokenized_text = self.run_script(data_file=TEXT_EXAMPLE,options="--just-tokenize")
+        non_tokenized_text = gh.read_file(TEXT_EXAMPLE)
+        # match every token except whitespaces, 
+        # that way tokenized and non-tokenized texts are equals 
+        matches_tokenized = my_re.match(r'\S', tokenized_text).groups()
+        matches_normal = my_re.match(r'\S', non_tokenized_text).groups()
+        assert matches_tokenized == matches_normal
+        assert not tokenized_text == non_tokenized_text
+        # self.do_assert(output == '', "TODO: code test")
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     def test_make_lowercase(self):
         """Ensure make_lowercase argument works as expected"""
         debug.trace(4, "test_make_lowercase()")
-        self.do_assert(False, "TODO: code test")
-
+        output_normal = self.run_script(data_file=TEXT_EXAMPLE,options="--just-tokenize")
+        output_lower = self.run_script(data_file=TEXT_EXAMPLE,options="--just-tokenize --lowercase")
+        self.do_assert(output_lower == output_normal.lower(), "TODO: code test")
 
 class TestTextProc(TestWrapper):
     """Test TextProc classes"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
 
-    @pytest.mark.xfail                   # TODO: remove xfail
     ## DEBUG:
     @trap_exception            # TODO: remove when debugged
     def test_chunk_noun_phrases(self):
         """Make sure sentences split into NPs properly"""
         sentence = "The cat is on the mat by the door"
         expected = ["The cat", "the mat", "the door"]
         min_overlap = 2
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_text_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_tpo_common.py` & `mezcla-1.4.0.0/mezcla/tests/test_tpo_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,37 +8,41 @@
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_tpo_common.py
 #
 # Warning:
 # - *** The tpo_common.py module is being phased out. Although there are
 #   a bunch of "work-in-progress" tests below, they are low priority because
 #   most are addressed by test_system.py or test_debug.py.
 #
+# TODO1: Make sure all work-in-progress tests issue Assert(False).
+#
 # TODO:
 # - Address commonly used debugging functions (e.g., debug_print) by redirecting output (via remapping sys.stderr to a file) and then checking file contents.
 # - add tests for normalize_unicode, ensure_unicode and other problematic functions
 #
 # Important:
 # - Most of the methods on tpo_common was moved to predecessors modules as system.py, debug.py etc.
 # - Using the predecessors module tests to these moved methods could be useful to avoid repeated tests but this could create conflicts with modified methods.
 #
 
 """Tests for tpo_common module"""
 
 # Standard modules
 import sys
 import re
+from datetime import datetime
 
 # Installed modules
 import pytest
 import pickle
 import trace
 
 # Local modules
 from mezcla import debug
 from mezcla import glue_helpers as gh
+from mezcla import system
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla.unittest_wrapper import trap_exception
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	                global module object
 #    TestIt.script_module:              path to file
 import mezcla.tpo_common as THE_MODULE
@@ -63,122 +67,166 @@
         debug.trace(4, "test_debugging_level()")
         THE_MODULE.set_debug_level(5)
         assert THE_MODULE.debugging_level() == 5
 
     def test_debug_trace_without_newline(self):
         """Ensure debug_trace_without_newline works as expected"""
         debug.trace(4, "test_debug_trace_without_newline()")
+        text = 'test debug trace withouht newline'
+        
+        # test underlying function is being called
         tracer = trace.Trace(countfuncs=1)
-        tracer.runfunc(THE_MODULE.debug_trace_without_newline, ('test debug trace withouht newline'))
+        tracer.runfunc(THE_MODULE.debug_trace_without_newline, (text))
         
         # redirect write_results to temp file
         temp = self.get_temp_file()
         tracer.results().write_results(coverdir=temp)
         
-        captured = self.get_stdout()
-        assert re.search(r'modulename: debug, funcname: trace', captured)
+        out, error = self.get_stdout_stderr()
+        assert re.search(r'modulename: debug, funcname: trace', out)
+
+        # test behaviour of functions
+        assert text in error
+        assert f'{text}\n' not in error
 
 
+    @pytest.mark.xfail
     def test_debug_trace(self):
         """Ensure debug_trace works as expected"""
         debug.trace(4, "test_debug_trace()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_debug_print(self):
         """Ensure debug_print works as expected"""
         debug.trace(4, "test_debug_print()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_debug_format(self):
         """Ensure debug_format works as expected"""
         debug.trace(4, "test_debug_format()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_debug_timestamp(self):
         """Ensure debug_timestamp works as expected"""
         debug.trace(4, "test_debug_timestamp()")
         tracer = trace.Trace(countfuncs=1)
         tracer.runfunc(THE_MODULE.debug_timestamp)
         
         # redirect write_results to temp file
         temp = self.get_temp_file()
         tracer.results().write_results(coverdir=temp)
         
         captured = self.get_stdout()
         assert re.search(r'modulename: debug, funcname: timestamp', captured)
+        
+        # test behaviour of function
+        actual, expected = THE_MODULE.debug_timestamp(), str(datetime.now())
+        # truncating the timestamp to eliminate milisecond difference in calculation
+        assert actual[:22] == expected[:22]
 
-    @trap_exception
     def test_debug_raise(self):
         """Ensure debug_raise works as expected"""
         debug.trace(4, "test_debug_raise()")
-        tracer = trace.Trace(countfuncs=1)
-        try:
-            raise RuntimeError
-        except RuntimeError:
-            with pytest.raises(RuntimeError):
-                tracer.runfunc(THE_MODULE.debug_raise)
         
+        tracer = trace.Trace(countfuncs=1)
+        with pytest.raises(RuntimeError):
+            tracer.runfunc(THE_MODULE.debug_raise)
+                
         # redirect write_results to temp file
         temp = self.get_temp_file()
         tracer.results().write_results(coverdir=temp)
         
         captured = self.get_stdout()
         assert re.search(r'modulename: debug, funcname: raise_exception', captured)
 
 
     def test_trace_array(self):
         """Ensure trace_array works as expected"""
         debug.trace(4, "test_trace_array()")
+        array = ['test', 'trace', 'array']
         tracer = trace.Trace(countfuncs=1)
-        tracer.runfunc(THE_MODULE.trace_array, (['test', 'trace', 'array']))
+        tracer.runfunc(THE_MODULE.trace_array, (array))
         
         # redirect write_results to temp file
         temp = self.get_temp_file()
         tracer.results().write_results(coverdir=temp)
         
-        captured = self.get_stdout()
-        assert re.search(r'modulename: debug, funcname: trace_values', captured)
+        out, error = self.get_stdout_stderr()
+        assert re.search(r'modulename: debug, funcname: trace_values', out)
+        
+        for i, item in enumerate(array):
+            assert f"{i}: {item}" in error
 
     def test_trace_object(self):
         """Ensure trace_object works as expected"""
         debug.trace(4, "test_trace_object()")
+        
+        class TestObj:
+            __var__ = 1
+            
+            def test_method():
+                pass
+        
+        obj = TestObj()
         tracer = trace.Trace(countfuncs=1)
-        tracer.runfunc(THE_MODULE.trace_object, ('test_trace_object'), show_methods_etc=True)
+        tracer.runfunc(THE_MODULE.trace_object, obj, show_methods_etc=True, show_private=True)
         
         # redirect write_results to temp file
         temp = self.get_temp_file()
         tracer.results().write_results(coverdir=temp)
         
-        captured = self.get_stdout()
-        assert re.search(r'modulename: debug, funcname: trace_object', captured)
+        out, error = self.get_stdout_stderr()
+        assert re.search(r'modulename: debug, funcname: trace_object', out)
+        
+        assert '__var__: 1' in error
+        assert 'test_method' in error
         
 
+    @pytest.mark.xfail
     def test_trace_value(self):
         """Ensure trace_value works as expected"""
         debug.trace(4, "test_trace_value()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_trace_current_context(self):
         """Ensure trace_current_context works as expected"""
         debug.trace(4, "test_trace_current_context()")
+        
+        test_var = 1
+        #assert local and global variables are traced
+        THE_MODULE.trace_current_context(level=8, label='TPO', show_methods_etc=True)
+        error = self.get_stderr()
+        assert 'TPO' in error
+        assert 'test_var' in error
+        assert 'FOOBAR' in error
+        
+        # assert debug function is being called
         tracer = trace.Trace(countfuncs=1)
-        tracer.runfunc(THE_MODULE.trace_current_context, show_methods_etc=True)
+        tracer.runfunc(THE_MODULE.trace_current_context, show_methods_etc=True, label='TPO')
         
         # redirect write_results to temp file
         temp = self.get_temp_file()
         tracer.results().write_results(coverdir=temp)
         
-        captured = self.get_stdout()
-        assert re.search(r'modulename: debug, funcname: trace_current_context', captured)
+        stdout = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: trace_current_context', stdout)
 
+    @pytest.mark.xfail
     def test_during_debugging(self):
         """Ensure during_debugging works as expected"""
         debug.trace(4, "test_during_debugging()")
-
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_debugging(self):
         """Ensure debugging works as expected"""
         debug.trace(4, "test_debugging()")
         THE_MODULE.set_debug_level(4)
         assert THE_MODULE.debugging(2)
         assert THE_MODULE.debugging(4)
@@ -228,25 +276,43 @@
         ## TODO: assert THE_MODULE.ensure_unicode(UTF8_BOM) == '\ufeff'
         ## TODO: add tests for sys.version_info.major < 3
         ## assert THE_MODULE.ensure_unicode('\xe1\x88\xb4') == '\u1234'
 
     def test_print_stderr(self):
         """Ensure print_stderr works as expected"""
         debug.trace(4, "test_print_stderr()")
-        ## TODO: WORK-IN-PROGRESS
+        # ensure stderr is not being redirected
+        self.monkeypatch.setattr(THE_MODULE, 'stderr', sys.stderr)
 
+        message = "this is error"
+        THE_MODULE.print_stderr(message)
+        error = self.get_stderr()
+        assert message in error
+
+    # @pytest.mark.xfail
     def test_redirect_stderr(self):
         """Ensure redirect_stderr works as expected"""
         debug.trace(4, "test_redirect_stderr()")
-        ## TODO: WORK-IN-PROGRESS
+        # ensure stderr is not being redirected
+        self.monkeypatch.setattr(THE_MODULE, 'stderr', sys.stderr)
+        
+        temp = self.get_temp_file()
+        THE_MODULE.redirect_stderr(temp)
+        THE_MODULE.print_stderr("stderr redirected")
+        THE_MODULE.restore_stderr()
+        assert "stderr redirected" in gh.read_file(temp)
 
+    @pytest.mark.xfail
     def test_restore_stderr(self):
         """Ensure restore_stderr works as expected"""
         debug.trace(4, "test_restore_stderr()")
-        ## TODO: WORK-IN-PROGRESS
+        # ensure stderr is already being redirected
+        self.monkeypatch.setattr(THE_MODULE, 'stderr', system.open_file(self.get_temp_file()))
+        THE_MODULE.restore_stderr()
+        assert sys.stderr == THE_MODULE.stderr
 
     def test_setenv(self):
         """Ensure setenv works as expected"""
         debug.trace(4, "test_setenv()")
         THE_MODULE.setenv('NEW_TEST_ENV_VAR', 'the gravity is 10, pi is 3')
         assert THE_MODULE.getenv('NEW_TEST_ENV_VAR') == 'the gravity is 10, pi is 3'
 
@@ -320,53 +386,63 @@
         debug.trace(4, "test_get_environment_option_descriptions()")
         set_test_env_var()
         result = THE_MODULE.get_environment_option_descriptions(include_default=True)
         self.do_assert(isinstance(result, list))
         self.do_assert("(2022)" in str(result), "default added")
         self.do_assert(len(result) == 2)
         
+    @pytest.mark.xfail
     def test_getenv_real(self):
         """Ensure getenv_real works as expected"""
         debug.trace(4, "test_getenv_real()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_getenv_float(self):
         """Ensure getenv_float works as expected"""
         debug.trace(4, "test_getenv_float()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_get_current_function_name(self):
         """Test(s) for get_current_function_name()"""
         assert THE_MODULE.get_current_function_name() == "test_get_current_function_name"
         return
 
+    @pytest.mark.xfail
     def test_get_property_value(self):
         """Ensure get_property_value works as expected"""
         debug.trace(4, "test_get_property_value()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_simple_format(self):
         """Ensure simple_format works as expected"""
         debug.trace(4, "test_simple_format()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_format(self):
         """Ensure format resolves from local and global namespace, and that local takes precedence"""
         fubar = 202
         assert THE_MODULE.format("{F} vs. {f}", F=FUBAR, f=fubar) == ("%s vs. %s" % (FUBAR, fubar))
         # pylint: disable=redefined-outer-name
         FOOBAR = 21
         assert THE_MODULE.format("{FOO}", FOO=FOOBAR) == str(FOOBAR)
         ## TODO: assert "Hey Jos\xc3\xa9" == THE_MODULE.format("Hey {j}", j=JOSE)
         return
 
+    @pytest.mark.xfail
     def test_init_logging(self):
         """Ensure init_logging works as expected"""
         debug.trace(4, "test_init_logging()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_load_object(self):
         """Ensure load_object works as expected"""
         debug.trace(4, "test_load_object()")
         test_dict = {
             1: 'first',
             2: 'second',
@@ -409,18 +485,20 @@
         THE_MODULE.store_object(test_filename, test_dict)
 
         test_file = open(test_filename, 'rb')
         actual_object = pickle.load(test_file)
         assert actual_object == test_dict
         test_file.close()
 
+    @pytest.mark.xfail
     def test_create_lookup_table(self):
         """Ensure create_lookup_table works as expected"""
         debug.trace(4, "test_create_lookup_table()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_lookup_key(self):
         """Ensure lookup_key works as expected"""
         debug.trace(4, "test_lookup_key()")
         test_table = {
             'first': '1st',
             'second': '2nd',
@@ -443,23 +521,27 @@
             'isbusiness - true': True,
         }
 
         temp_file = self.get_temp_file()
         gh.write_file(temp_file, content)
         assert THE_MODULE.create_boolean_lookup_table(temp_file) == expected
 
+    @pytest.mark.xfail
     def test_normalize_frequencies(self):
         """Ensure normalize_frequencies works as expected"""
         debug.trace(4, "test_normalize_frequencies()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_sort_frequencies(self):
         """Ensure sort_frequencies works as expected"""
         debug.trace(4, "test_sort_frequencies()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_sort_weighted_hash(self):
         """Ensure sort_weighted_hash works as expected"""
         debug.trace(4, "test_sort_weighted_hash()")
         test_hash = {
             'bananas': 3,
             'apples': 1411,
@@ -475,18 +557,20 @@
             ('peach', 43),
             ('bananas', 3),
         ]
         assert THE_MODULE.sort_weighted_hash(test_hash) == reversed_hash
         assert THE_MODULE.sort_weighted_hash(test_hash, reverse=False) == sorted_hash
         assert len(THE_MODULE.sort_weighted_hash(test_hash, max_num=2)) == 2
 
+    @pytest.mark.xfail
     def test_format_freq_hash(self):
         """Ensure format_freq_hash works as expected"""
         debug.trace(4, "test_format_freq_hash()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     def test_union(self):
         """Ensure union works as expected"""
         debug.trace(4, "test_union()")
         assert THE_MODULE.union([1, 2, 3], [2, 3, 4, 5]) == [1, 2, 3, 4, 5]
 
     def test_intersection(self):
@@ -563,30 +647,42 @@
         debug.trace(4, "test_is_numeric()")
         assert THE_MODULE.is_numeric("123")
         assert not THE_MODULE.is_numeric("one")
 
     def test_safe_int(self):
         """Ensure safe_int works as expected"""
         debug.trace(4, "test_safe_int()")
-        ## TODO: WORK-IN-PROGRESS
+        THE_MODULE.safe_int('1') == 1
+        THE_MODULE.safe_int(2.0) == 2
+        THE_MODULE.safe_int("F", base=16) == 16
+        THE_MODULE.safe_int("82", base=8) == 10
+        THE_MODULE.safe_int("four") == 0
 
+    # @pytest.mark.xfail
     def test_safe_float(self):
         """Ensure safe_float works as expected"""
         debug.trace(4, "test_safe_float()")
-        ## TODO: WORK-IN-PROGRESS
-
+        assert THE_MODULE.safe_float(5) == 5.0
+        assert THE_MODULE.safe_float("3") == 3.0
+        assert THE_MODULE.safe_float("three") == 0.0
+        
+        
+    @pytest.mark.xfail
     def test_reference_variables(self):
         """Ensure reference_variables works as expected"""
         debug.trace(4, "test_reference_variables()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
+    @pytest.mark.xfail
     def test_memodict(self):
         """Ensure memodict works as expected"""
         debug.trace(4, "test_memodict()")
         ## TODO: WORK-IN-PROGRESS
+        assert(False)
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_exit(self):
         """Ensure exit works as expected"""
         debug.trace(4, "test_exit()")
         def sys_exit_mock():
             return 'exit'
@@ -602,15 +698,14 @@
     def test_dummy_main(self):
         """Ensure dummy_main works as expected"""
         debug.trace(4, "test_dummy_main()")
         THE_MODULE.dummy_main()
         captured = self.get_stdout()
         assert 'Environment options' in captured
 
-    # @pytest.mark.xfail                   # TODO: remove xfail
     @trap_exception
     def test_getenv(self):
         """Ensure getenv works as expected"""
         debug.trace(4, "test_getenv()")
         self.monkeypatch.setenv('TEST_ENV_VAR', 'some value', prepend=False)
         assert THE_MODULE.getenv('TEST_ENV_VAR') == 'some value'
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_train_language_model.py` & `mezcla-1.4.0.0/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.4.0.0/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_transpose_data.py` & `mezcla-1.4.0.0/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_unittest_wrapper.py` & `mezcla-1.4.0.0/mezcla/tests/test_unittest_wrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,30 +18,36 @@
 
 """Tests for unittest_wrapper module"""
 
 # Installed packages
 import pytest
 
 # Local packages
+import os
+## TEST: os.environ["PRESERVE_TEMP_FILE"] = "1"
 from mezcla.unittest_wrapper import TestWrapper, invoke_tests, trap_exception
 from mezcla import debug
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                  global module object
 #    TestTemplate.script_module:  path to file
 import mezcla.unittest_wrapper as THE_MODULE
 
 
 ## TODO (use TestWrapper directly):
 
+# Globals
+last_self = None                        # Reserved for test_05_check_temp_part1/2
+
 class TestIt(TestWrapper):
     """Class for command-line based testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
+    last_temp_file = None               # Reserved for test_05_check_temp_part1/2
 
     def test_01_usage(self):
         """Make sure usage warns that not intended for command line and that no stdout"""
         debug.trace(4, f"TestIt.test_01_usage(); self={self}")
         log_file = self.temp_file + ".log"
         ## BAD: output = self.run_script(log_file=log_file)
         output = self.run_script(env_options="DEBUG_LEVEL=4", log_file=log_file)
@@ -133,12 +139,41 @@
         # example: "diff:\n< dog\'s bark\n…  ^\n> dawg\'s bark\n…  ^^\n\n"
         assert(my_re.search(r" \^\n.* \^\^\n", captured_trace, flags=my_re.DOTALL))
         
         # Make sure stuff properly stripped (i.e., message arg and comment)
         assert(not "sti.do_assert_equals" in captured_trace)
         return
 
+    @pytest.mark.xfail
+    def test_04_get_temp_dir(self):
+        """Tests get_temp_dir"""
+        debug.trace(4, f"TestIt.test_04_get_temp_dir(); self={self}")
+        assert False, "TODO: implement"
+
+    @pytest.mark.xfail
+    def test_05_check_temp_part1(self):
+        """Make sure self.temp setup OK"""
+        debug.trace(4, f"TestIt.test_05_check_temp_part1(); self={self!r}; id={id(self)}")
+        debug.trace_expr(5, self.last_temp_file, self.temp_file)
+        assert(self.last_temp_file is None)
+        self.last_temp_file = self.temp_file
+        global last_self                # TODO4 (use class member)
+        debug.assertion(last_self is None)
+        last_self = self
+
+    @pytest.mark.xfail
+    def test_06_check_temp_part2(self):
+        """Make sure self.temp unique"""
+        debug.trace(4, f"TestIt.test_06_check_temp_part2(); self={self!r}; id={id(self)}")
+        debug.trace_expr(5, self.last_temp_file, self.temp_file)
+        assert self.last_temp_file != self.temp_file
+        assert(self.last_temp_file is not None)
+        global last_self                # TODO4 (use class member)
+        # NOTE: The following will fail: apparently each test is run using
+        # a separate class instance.
+        debug.assertion(last_self == self)
+
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
-    invoke_tests([__file__])
+    invoke_tests(__file__)
```

### Comparing `mezcla-1.3.9.9/mezcla/tests/test_xml_utils.py` & `mezcla-1.4.0.0/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.4.0.0/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.4.0.0/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/tfidf/test_document.py` & `mezcla-1.4.0.0/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.4.0.0/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/text_categorizer.py` & `mezcla-1.4.0.0/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/text_processing.py` & `mezcla-1.4.0.0/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/text_utils.py` & `mezcla-1.4.0.0/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tfidf/config.py` & `mezcla-1.4.0.0/mezcla/tfidf/config.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tfidf/corpus.py` & `mezcla-1.4.0.0/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tfidf/dockeyword.py` & `mezcla-1.4.0.0/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tfidf/document.py` & `mezcla-1.4.0.0/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tfidf/preprocess.py` & `mezcla-1.4.0.0/mezcla/tfidf/preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tfidf/tests/misc_test.py` & `mezcla-1.4.0.0/mezcla/tfidf/tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/tpo_common.py` & `mezcla-1.4.0.0/mezcla/tpo_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 #   you shouldn't import using 'import *'.
 # - Debugging output and error messages are converted to UTF8 before output
 #   via s=unicode(s, "utf8"), which is same as s=codecs.encode(s, "utf8").
 # - Debugging code is "conditionally compiled" to avoid overhead of passing
 #   arguments to functions that do nothing in release code.
 # - Includes support for overriding stderr (e.g., for use with embedded apps as in adhoc/optimize_company_extraction.py's invocation of extract_company_info.py).
 #
+# TODO1:
+# - *** Make sure any function not mapping directly to debug or system traces out
+#   with "tpo" for grep purposes (e.g.,  tpo.debug_format in debug_format). ***
+#   This will help flag functions to be ported (e.g., redirect_stderr).
+#
 # TODO:
 # - Change all functions to using docstrings for comments already!!!
 # - Add support for using pprint module
 # - Put a version of assertion() here (i.e., from glue_helpers.py).
 # - Extend getenv support to indicate user-vs-devel options.
 # - Remove obsolete functions (e.g., get_current_function_name).
 # - Use debug_trace in place of debug_print in code run often.
@@ -475,14 +480,15 @@
     return debug_trace_without_newline(out_text, level=level)
 
 
 def debug_format(text, level=1, skip_newline=False, **namespace):
     """Version of debug_print that expands TEXT using format.
     Note: Exceptions are ignored (to encourage tracing, not discourage)."
     """
+    debug.trace(6, f"tpo.debug_format({text}, {skip_newline}, ...)")
     ## TODO: return debug.trace(no_eol=skip_newline, level, text, **namespace)
     # NOTE: String values from namespace need to be in UTF-8 format.
     # TODO: rename as debug_print_format as not just formatting the text
     assert(isinstance(level, int))
     if (debugging_level() >= level):
         ignore_exc = (debugging_level() < QUITE_DETAILED)
         debug_print(format(text, indirect_caller=True, 
@@ -1329,14 +1335,15 @@
 # This is implemented transparently via Python decorators. See
 #     http://stackoverflow.com/questions/739654/understanding-python-decorators
 #
 # usage example:
 #
 #    @memodict
 #    def fubar(word):
+#        """Fouled up"""
 #        result = ...
 #        return result
 #
 
 def memodict(f):
     """Memoization decorator for a function taking a single argument
     Warning: deprecated; uses version in system.py instead
```

### Comparing `mezcla-1.3.9.9/mezcla/train_language_model.py` & `mezcla-1.4.0.0/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/train_text_categorizer.py` & `mezcla-1.4.0.0/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/transpose_data.py` & `mezcla-1.4.0.0/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/mezcla/unittest_wrapper.py` & `mezcla-1.4.0.0/mezcla/unittest_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #   tests/test_extract_company_info.py for an example.
 # - It can be confusing debugging tests that use run_script, because the trace level
 #   is raised by default. To disable this, set the SUB_DEBUG_LEVEL as follows:
 #      l=5; DEBUG_LEVEL=$l SUB_DEBUG_LEVEL=$l pytest -s tests/test_spell.py
 #   See glue_helper.py for implementation along with related ALLOW_SUBCOMMAND_TRACING.
 # TODO:
 # - * Clarify TEMP_BASE vs. TEMP_FILE usage.
+# - Add TEMP_DIR for more direct specification.
 # - Clarify that this can co-exist with pytest-based tests (see tests/test_main.py).
 # TODO2:
 # - Clean up script_file usage (and unncessary settings in test scripts).
 #
 #-------------------------------------------------------------------------------
 # Sample test (streamlined version of test_simple_main_example.py):
 #
@@ -54,27 +55,31 @@
 import tempfile
 import unittest
 
 # Installed packages
 import pytest
 
 # Local packages
+# note: Disables TEMP_FILE default used by in glue_helpers.py.
+os.environ["PRESERVE_TEMP_FILE"] = "1"
 import mezcla
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.main import DISABLE_RECURSIVE_DELETE
 from mezcla.misc_utils import string_diff
 from mezcla.my_regex import my_re
 from mezcla import system
+## DEBUG: debug.trace_expr(6, __file__)
 
 # Constants (e.g., environment options)
 
 TL = debug.TL
-KEEP_TEMP = system.getenv_bool("KEEP_TEMP", debug.detailed_debugging(),
-                               "keep temporary files")
+KEEP_TEMP = system.getenv_bool(
+    "KEEP_TEMP", debug.detailed_debugging(),
+    desc="Keep temporary files")
 TODO_FILE = "TODO FILE"
 TODO_MODULE = "TODO MODULE"
 
 # Note: the following is for transparent resolution of dotted module names
 # for invocation of scripts via 'python -m package.module'. This is in support
 # of transitioning from the old way of importing packages via 'import module'
 # instead of 'import package.module'. (The former required that package be
@@ -85,29 +90,47 @@
 # Environment options
 VIA_UNITTEST = system.getenv_bool(
     "VIA_UNITTEST", False,
     description="Run tests via unittest instead of pytest")
 PROFILE_CODE = system.getenv_boolean(
     "PROFILE_CODE", False,
     description="Profile each test invocation")
+#
+# For use in tests
+RUN_SLOW_TESTS = system.getenv_bool(
+    "RUN_SLOW_TESTS", False,
+    description="Run tests that can a while to run")
+debug.reference_var(RUN_SLOW_TESTS)
 
 # Dynamic imports
 if PROFILE_CODE:
     import cProfile
     import pstats
 
 #-------------------------------------------------------------------------------
 
-def get_temp_dir(keep=None):
-    """Get temporary directory, omitting later deletion if KEEP"""
-    # NOTE: Unused function
+def get_temp_dir(keep=None, unique=None):
+    """Get temporary directory, omitting later deletion if KEEP
+    Note: Optionally returns UNIQUE dir
+    """
+    debug.assertion(not ((keep is False) and (unique is False)))
     if keep is None:
         keep = KEEP_TEMP
-    dir_path = tempfile.NamedTemporaryFile(delete=(not keep)).name
-    gh.full_mkdir(dir_path)
+    dir_base = gh.get_temp_file()
+    if unique:
+        # Note: creates parent temp dir if temp file regular file
+        if not system.is_directory(dir_base):
+            dir_base += "_temp_dir_"
+            gh.full_mkdir(dir_base)
+        dir_path = tempfile.NamedTemporaryFile(
+            delete=(not keep), dir=dir_base).name
+    else:
+        dir_path = dir_base
+    if not system.is_directory(dir_path):
+        gh.full_mkdir(dir_path)
     debug.trace(5, f"get_temp_dir() => {dir_path}")
     return dir_path
 
 
 def trap_exception(function):
     """Decorator to trap exception during function execution
     Note:
@@ -150,35 +173,46 @@
         """Wrapper around unary function f(x)"""   ## TODO: {function.__name__}
         debug.trace(7, f"in wrapper: x={x}")
         return function(x)
     #
     debug.trace(7, f"pytest_fixture_wrapper() => {gh.elide(wrapper)}")
     return wrapper
 
-def invoke_tests(filename, via_unittest=VIA_UNITTEST):
+def invoke_tests(filename: str, via_unittest: bool = VIA_UNITTEST):
     """Invoke TESTS defined in FILENAME, optionally VIA_UNITTEST"""
     if via_unittest:
         unittest.main()
     else:
-        pytest.main(filename)
+        pytest.main([filename])
 
 #-------------------------------------------------------------------------------
 
 class TestWrapper(unittest.TestCase):
     """Class for testcase definition
     Note:
     - script_module should be overriden to specify the module instance, such as via get_testing_module_name (see test/template.py)
     - set it to None to avoid command-line invocation checks
     """
+
+    # Re-initalize glue helper temp file settings
+    ## TODO?: system.setenv("PRESERVE_TEMP_FILE", "1")
+    debug.trace_expr(4, os.environ.get("PRESERVE_TEMP_FILE"))
+    ## TEST: os.environ["PRESERVE_TEMP_FILE"] = "1"
+    system.setenv("PRESERVE_TEMP_FILE", "1")
+    gh.init()
+    debug.trace_expr(4, os.environ.get("PRESERVE_TEMP_FILE"))
+
     script_file = TODO_FILE             # path for invocation via 'python -m coverage run ...' (n.b., usually set via get_module_file_path)
     script_module = TODO_MODULE         # name for invocation via 'python -m' (n.b., usually set via derive_tested_module_name)
-    temp_base = system.getenv_text("TEMP_BASE",
-                                   tempfile.NamedTemporaryFile().name)
-    check_coverage = system.getenv_bool("CHECK_COVERAGE", False,
-                                        "Check coverage during unit testing")
+    temp_base = system.getenv_text(
+        "TEMP_BASE", tempfile.NamedTemporaryFile().name,
+        desc="Override for basename of temporary files")
+    check_coverage = system.getenv_bool(
+        "CHECK_COVERAGE", False,
+        desc="Check coverage during unit testing")
     ## TODO: temp_file = None
     ## TEMP: initialize to unique value independent of temp_base
     temp_file = None
     use_temp_base_dir = system.is_directory(temp_base)
     ## OLD: test_num = 1
     test_num = 0
     temp_file_count = 0
@@ -216,15 +250,17 @@
             if (not ((my_re.search(r"warning:.*not intended", help_usage,
                                    flags=my_re.IGNORECASE))
                      or ("usage:" in help_usage.lower()))):
                 system.print_stderr("Warning: script should implement --help")
 
         # Optionally, setup temp-base directory (normally just a file)
         if cls.use_temp_base_dir is None:
-            cls.use_temp_base_dir = system.getenv_bool("USE_TEMP_BASE_DIR", False)
+            cls.use_temp_base_dir = system.getenv_bool(
+                "USE_TEMP_BASE_DIR", False,
+                desc="Treat TEMP_BASE as a directory")
             # TODO: temp_base_dir = system.getenv_text("TEMP_BASE_DIR", " "); cls.use_temp_base_dir = bool(temp_base_dir.strip()); ...
         if cls.use_temp_base_dir:
             ## TODO: pure python
             ## TODO: gh.full_mkdir
             gh.run("mkdir -p {dir}", dir=cls.temp_base)
 
         # Warn that coverage support is limited
@@ -284,15 +320,15 @@
     @staticmethod
     def get_module_file_path(test_filename):
         """Return absolute path of module being tested"""
         result = system.absolute_path(test_filename)
         ## TODO3: use os.path.delim instead of /
         result = my_re.sub(r'tests\/test_(.*\.py)', r'\1', result)
         debug.assertion(result.endswith(".py"))
-        debug.trace(7, f'get_module_file_path({test_filename}) => {result}')
+        debug.trace(6, f'get_module_file_path({test_filename}) => {result}')
         return result
 
     @classmethod
     def set_module_info(cls, test_filename, module_object=None):
         """Sets both script_module and script_path
         Note: normally invoked in setUpClass method
         Usage: cls.set_module_info(__file__, THE_MODULE)
@@ -318,18 +354,21 @@
         # Optionally, if can be a file in temp-base subdrectory.
         if self.use_temp_base_dir:
             default_temp_file = gh.form_path(self.temp_base, "test-")
         else:
             default_temp_file = self.temp_base + "-test-"
         TestWrapper.test_num += 1
         default_temp_file += str(TestWrapper.test_num)
+        debug.trace_expr(5, default_temp_file)
 
         # Get new temp file and delete existing file and variants based on temp_file_count,
         # such as /tmp/test-2, /tmp/test-2-1, and /tmp/test-2-2 (but not /tmp/test-[13]*).
-        self.temp_file = system.getenv_text("TEMP_FILE", default_temp_file)
+        self.temp_file = system.getenv_text(
+            "TEMP_FILE", default_temp_file,
+            desc="Override for temporary filename")
         gh.delete_existing_file(f"{self.temp_file}")
         for f in gh.get_matching_files(f"{self.temp_file}-[0-9]*"):
             gh.delete_existing_file(f)
 
         # Start the profiler
         if PROFILE_CODE:
             self.profiler.enable()
@@ -343,15 +382,17 @@
         OPTIONS and optional setting ENV_OPTIONS. If OUT_FILE and LOG_FILE are
         not specified, they  are derived from self.temp_file. The optional POST_OPTIONS
         go after the data file.
         Notes:
         - OPTIONS uses quotes around shell special characters used (e.g., '<', '>', '|')
         - issues warning if script invocation leads to error
         - if USES_STDIN, requires explicit empty string for DATA_FILE to avoid use of - (n.b., as a precaution against hangups)
-        - if SKIP_STDIN, then - omitted from command line"""
+        - if SKIP_STDIN, then - omitted from command line
+        - By default, stderr is not included in the output
+        """
         debug.trace_fmtd(trace_level + 1,
                          "TestWrapper.run_script(opts={opts!r}, data={df}, log={lf}, lvl={lvl}, out={of}, env={env}, stdin={stdin}, post={post}, back={back})",
                          opts=options, df=data_file, lf=log_file, lvl=trace_level, of=out_file,
                          env=env_options, stdin=uses_stdin, post=post_options, back=background)
         if options is None:
             options = ""
         if env_options is None:
@@ -503,15 +544,15 @@
     def get_stdout_stderr(self):
         """Get currently captured standard output and error
         Note: Clears both stdout and stderr captured afterwards. This might
         be needed beforehand to clear capsys buffer.
         """
         stdout, stderr = self.capsys.readouterr()
         ## TODO4: resolve issue with resolve_assertion call-stack tracing being clippped
-        debug.trace_expr(5, stdout, stderr, prefix="get_stdout_stderr:\n", delim="\n", maxlen=8192)
+        debug.trace_expr(5, stdout, stderr, prefix="get_stdout_stderr:\n", delim="\n", maxlen=16384)
         return stdout, stderr
         
     def get_stdout(self):
         """Get currently captured standard output (see get_stdout_stderr)
         Warning: You might need to invoke beforehand to clear buffer.
         """
         stdout, _stderr = self.get_stdout_stderr()
```

### Comparing `mezcla-1.3.9.9/mezcla/xml_utils.py` & `mezcla-1.4.0.0/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/pyproject.toml` & `mezcla-1.4.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## TODO: eliminate redundancy
 
 [tool.poetry]
 name = "mezcla"
-version = "1.3.9.9"
+version = "1.4.0.0"
 description = "Miscellaneous Python scripts developed over the course of several independent consulting projects. [Mezcla is Spanish for mixture.]"
 authors = ["Tom O'Hara <tomasohara@gmail.com>"]
 license = "LGPLv3"
 ## TODO:
 ## packages = ['mezcla', 'mezcla.tfidf']
 
 [tool.poetry.dependencies]
```

### Comparing `mezcla-1.3.9.9/required-packages.txt` & `mezcla-1.4.0.0/packages-required.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/requirements.txt` & `mezcla-1.4.0.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # - Usage examples:
 #   1. Usual
 #      pip install -r requirements.txt
 #   2. Optional (i.e., including most optional):
 #      pip install --verbose $(perl -pe 's/^#opt#\s*//;  s/\s*#.*//;' ~/Mezcla/requirements.txt | grep -v '^#')
 #   3. Full (i.e., including all optional):
 #      pip install --verbose $(perl -pe 's/^#(opt|full)#\s*//;  s/\s*#.*//;' ~/Mezcla/requirements.txt | grep -v '^#')
-#      # TODO2: --ignore-errors [maldito pip]
+#      # TODO2: --ignore-errors [maldito pip]; set pip-update check
 #      perl -pe 's/^#(opt|full)#\s*//;  s/\s*#.*//;' ~/Mezcla/requirements.txt | grep -v '^#' | xargs -I '{}' pip install '{}'
 # - use `pip freeze` to get current list of package specifications (n.b., >= better than == unless specific version needed)
 # - installing textract from PyPI fails https://github.com/deanmalmgren/textract/issues/461
 #
 # Installation:
 # - python -m nltk.downloader punkt averaged_perceptron_tagger stopwords
 #
@@ -28,24 +28,26 @@
 absl_py
 beautifulsoup4
 bs4
 cachetools
 cherrypy
 clip_interrogator
 datasets                      # Hugging Face (HF) data
-diffusers                     # Stale Diffusion
+#opt# diffusers               # Stale Diffusion; TEMP
 diskcache
 extcolors>=1.0.0
 flair
 flask
 git+https://github.com/tehabstract/textract.git
 gradio                        # UI support (e.g., HF-based apps)
 importlib_metadata
+langchain
+langchain_community
 #opt# kenlm                   # language model support (NOTE: problem with wheel)
-librosa>=0.10.0           
+## OLD: librosa>=0.10.0
 lxml
 mako
 matplotlib
 more_itertools
 nltk
 numpy>=1.18.5
 pandas>=1.3.0
@@ -53,24 +55,25 @@
 pyctcdecode                   # CTC beam search decoder for speech recognition
 pyenchant
 pysbd
 pytest
 requests
 scikit-learn
 scipy
-sentencepiece
+#opt# sentencepiece           # BERT tokenization; TEMP
 six
 stop_words
 #opt# tensorrt                # NVidia GPU support
 transformers                  # HF models
 torch
-torchaudio
+#opt# torchaudio
 webcolors
 wheel
-xgboost
+## NOTE: temporarily disabled due to stupid docker disk space constraints
+## TODO: xgboost
 #
 #...............................................................................
 # Optional requirements
 #
 # TODO:
 # - download Spacy model(s):
 #   python -m spacy download en_core_web_lg
@@ -94,14 +97,15 @@
 #opt# jupyter
 #opt# librosa
 #opt# pocketsphinx
 #opt# pylint
 #opt# pyyaml
 #opt# scispacy
 #opt# selenium
+#opt# Sphinx
 #
 ## OLD: #opt# spacy>=3.0.0
 ## TODO:
 ## note: See https://github.com/explosion/spacy-models/releases/tag/en_core_web_md-3.7.0
 spacy==3.7.0
 en_core_web_md@https://github.com/explosion/spacy-models/releases/download/en_core_web_md-3.7.0/en_core_web_md-3.7.0.tar.gz
 #
```

### Comparing `mezcla-1.3.9.9/setup.py` & `mezcla-1.4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla', 'mezcla.tfidf'],
       module="mezcla",
       ## TODO2: import mezcla; version=mezcla.VERSION
-      version="1.3.9.9",
+      version="1.4.0.0",
       ## BAD: description-file="README.txt",
       description_file="README.txt",
       ## BAD: dist-name="Mezcla",
       dist_name="Mezcla",
       author="Tom O'Hara",
       # TODO3: find out which email key is preferred
       email="tomasohara@gmail.com",
```

### Comparing `mezcla-1.3.9.9/temp/simple_batspp.py` & `mezcla-1.4.0.0/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/tools/_temp_test_settings.bash` & `mezcla-1.4.0.0/tools/_temp_test_settings.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/tools/local-workflows.sh` & `mezcla-1.4.0.0/tools/local-workflows.sh`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/tools/run_tests.bash` & `mezcla-1.4.0.0/tools/run_tests.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.9/tox.ini` & `mezcla-1.4.0.0/tox.ini`

 * *Files identical despite different names*

