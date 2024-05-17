# Comparing `tmp/timeseriesflattener-2.2.3.tar.gz` & `tmp/timeseriesflattener-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-2.2.3.tar", last modified: Tue May  7 13:21:51 2024, max compression
+gzip compressed data, was "timeseriesflattener-2.2.4.tar", last modified: Fri May 17 12:54:26 2024, max compression
```

## Comparing `timeseriesflattener-2.2.3.tar` & `timeseriesflattener-2.2.4.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.159999 timeseriesflattener-2.2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.095998 timeseriesflattener-2.2.3/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.devcontainer/post-start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.095998 timeseriesflattener-2.2.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.083998 timeseriesflattener-2.2.3/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.095998 timeseriesflattener-2.2.3/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.099998 timeseriesflattener-2.2.3/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.099998 timeseriesflattener-2.2.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/benchmark.yml
--rw-r--r--   0 root         (0) root         (0)      720 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)      849 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1939 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      788 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2885 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      697 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.python-version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.099998 timeseriesflattener-2.2.3/.vscode/
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.vscode/extensions.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     1373 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1286 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    74316 2024-05-07 13:21:45.000000 timeseriesflattener-2.2.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1031 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/Makefile
--rw-r--r--   0 root         (0) root         (0)    11525 2024-05-07 13:21:51.159999 timeseriesflattener-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7649 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.103998 timeseriesflattener-2.2.3/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.103998 timeseriesflattener-2.2.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   424821 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/aggregators.rst
--rw-r--r--   0 root         (0) root         (0)     4115 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/flattener.rst
--rw-r--r--   0 root         (0) root         (0)     5165 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.103998 timeseriesflattener-2.2.3/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   128585 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50850 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    29677 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/03_text.ipynb
--rw-r--r--   0 root         (0) root         (0)     5314 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/04_from_legacy.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.107998 timeseriesflattener-2.2.3/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)     1833 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/example.py
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/icon.png
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/lefthook.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.107998 timeseriesflattener-2.2.3/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4633 2024-05-07 13:21:45.000000 timeseriesflattener-2.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/requirements-dev.lock
--rw-r--r--   0 root         (0) root         (0)     1474 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/requirements.lock
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 13:21:51.159999 timeseriesflattener-2.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.107998 timeseriesflattener-2.2.3/src/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/test_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.107998 timeseriesflattener-2.2.3/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      776 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/_frame_validator.py
--rw-r--r--   0 root         (0) root         (0)     3924 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/_intermediary_frames.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/aggregators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.111998 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/default_column_names.py
--rw-r--r--   0 root         (0) root         (0)     3708 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     2978 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/meta.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/outcome.py
--rw-r--r--   0 root         (0) root         (0)     1899 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1434 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/static.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/test_from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/test_specs.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/timestamp_frame.py
--rw-r--r--   0 root         (0) root         (0)     6485 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.111998 timeseriesflattener-2.2.3/src/timeseriesflattener/frame_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/frame_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
--rw-r--r--   0 root         (0) root         (0)      644 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/process_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.115998 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/static.py
--rw-r--r--   0 root         (0) root         (0)    10309 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/temporal.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/test_static.py
--rw-r--r--   0 root         (0) root         (0)    10592 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/test_temporal.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     5057 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/test_aggregators.py
--rw-r--r--   0 root         (0) root         (0)    12858 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/test_flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.115998 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     1519 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.115998 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.087998 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.087998 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.115998 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.131998 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      754 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5511 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.135998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.135998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2016 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6160 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.135998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     5535 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     7823 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/logger.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.135998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/
--rw-r--r--   0 root         (0) root         (0)     2981 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.135998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2697 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.091998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.091998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.139998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.139998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1877 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.155998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      696 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5446 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.155998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.155998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3308 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.155998 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.159999 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23392 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2321 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.159999 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/utils/
--rw-r--r--   0 root         (0) root         (0)      984 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:21:51.159999 timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11525 2024-05-07 13:21:50.000000 timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8537 2024-05-07 13:21:51.000000 timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 13:21:50.000000 timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      650 2024-05-07 13:21:50.000000 timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-07 13:21:50.000000 timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8330 2024-05-07 13:21:44.000000 timeseriesflattener-2.2.3/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.301473 timeseriesflattener-2.2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.devcontainer/post-start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.225473 timeseriesflattener-2.2.4/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/benchmark.yml
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      788 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.python-version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.241473 timeseriesflattener-2.2.4/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.vscode/extensions.json
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    74868 2024-05-17 12:54:21.000000 timeseriesflattener-2.2.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-17 12:54:26.301473 timeseriesflattener-2.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7649 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.241473 timeseriesflattener-2.2.4/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.241473 timeseriesflattener-2.2.4/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   424821 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/aggregators.rst
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/flattener.rst
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   128585 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50850 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    29677 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/03_text.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5314 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/04_from_legacy.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/example.py
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/icon.png
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/lefthook.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-05-17 12:54:21.000000 timeseriesflattener-2.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/requirements-dev.lock
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/requirements.lock
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 12:54:26.301473 timeseriesflattener-2.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/src/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/test_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.249472 timeseriesflattener-2.2.4/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      776 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/_frame_validator.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/_intermediary_frames.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/aggregators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/default_column_names.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/static.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_specs.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timestamp_frame.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
+-rw-r--r--   0 root         (0) root         (0)      644 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/process_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/static.py
+-rw-r--r--   0 root         (0) root         (0)    10309 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_static.py
+-rw-r--r--   0 root         (0) root         (0)    10592 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/test_aggregators.py
+-rw-r--r--   0 root         (0) root         (0)    12858 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/test_flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.257473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.257473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      754 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     7823 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5446 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.297473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.297473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/utils/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.297473 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8330 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/tasks.py
```

### Comparing `timeseriesflattener-2.2.3/.devcontainer/devcontainer.json` & `timeseriesflattener-2.2.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/actions/test/action.yml` & `timeseriesflattener-2.2.4/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-2.2.4/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/dependabot.yml` & `timeseriesflattener-2.2.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/recommended_repo_setup.md` & `timeseriesflattener-2.2.4/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/benchmark.yml` & `timeseriesflattener-2.2.4/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/check_for_rej.yml` & `timeseriesflattener-2.2.4/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-2.2.4/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/documentation.yml` & `timeseriesflattener-2.2.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-2.2.4/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-2.2.4/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/pre-commit.yml` & `timeseriesflattener-2.2.4/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/stalebot.yml` & `timeseriesflattener-2.2.4/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.github/workflows/static_type_checks.yml` & `timeseriesflattener-2.2.4/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.gitignore` & `timeseriesflattener-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.pre-commit-config.yaml` & `timeseriesflattener-2.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.vscode/tasks.json` & `timeseriesflattener-2.2.4/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/.zenodo.json` & `timeseriesflattener-2.2.4/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/CHANGELOG.md` & `timeseriesflattener-2.2.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.2.4 (2024-05-17)
+
+### Fix
+
+* Don't mix types in HasValuesAggregator fallback ([`dfdf5dd`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/dfdf5dd1417639e76ec1639f7c689464c1012f05))
+
+### Documentation
+
+* Remove type hint in docstring ([`a4fe254`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a4fe254e87a0796bd1f63d803e35e57e86ae8e34))
+* Add docstring to flattener ([`64ee0b0`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/64ee0b09f8949cd85fa1345b371920ab5300749d))
+
 ## v2.2.3 (2024-05-07)
 
 ### Fix
 
 * Expose ValueSpecification ([`b670fc8`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/b670fc891a2cdfcb4eed01d82fd9b3f627a5b9b8))
 
 ## v2.2.2 (2024-05-03)
```

### Comparing `timeseriesflattener-2.2.3/CODE_OF_CONDUCT.md` & `timeseriesflattener-2.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/CONTRIBUTING.md` & `timeseriesflattener-2.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/Dockerfile` & `timeseriesflattener-2.2.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/LICENSE` & `timeseriesflattener-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/PKG-INFO` & `timeseriesflattener-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.3
+Version: 2.2.4
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.3 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.4 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.2.3/README.md` & `timeseriesflattener-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/citation.cff` & `timeseriesflattener-2.2.4/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/Makefile` & `timeseriesflattener-2.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/_static/favicon.ico` & `timeseriesflattener-2.2.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/_static/icon.png` & `timeseriesflattener-2.2.4/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/_static/icon_dark.png` & `timeseriesflattener-2.2.4/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/_static/terminology_figure.png` & `timeseriesflattener-2.2.4/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/conf.py` & `timeseriesflattener-2.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/faq.rst` & `timeseriesflattener-2.2.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/feature_specifications.rst` & `timeseriesflattener-2.2.4/docs/feature_specifications.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/index.rst` & `timeseriesflattener-2.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-2.2.4/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-2.2.4/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/03_text.ipynb` & `timeseriesflattener-2.2.4/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/04_from_legacy.ipynb` & `timeseriesflattener-2.2.4/docs/tutorials/04_from_legacy.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/img/term_a.png` & `timeseriesflattener-2.2.4/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/img/term_b.png` & `timeseriesflattener-2.2.4/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/img/term_c.png` & `timeseriesflattener-2.2.4/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/docs/tutorials/img/term_d.png` & `timeseriesflattener-2.2.4/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/example.py` & `timeseriesflattener-2.2.4/example.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/icon.png` & `timeseriesflattener-2.2.4/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/paper/paper.bib` & `timeseriesflattener-2.2.4/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/paper/paper.md` & `timeseriesflattener-2.2.4/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/pyproject.toml` & `timeseriesflattener-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "2.2.3"
+version = "2.2.4"
 authors = [
   { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
   { name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com" },
   { name = "Kenneth Enevoldsen" },
   { name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" },
 ]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
```

### Comparing `timeseriesflattener-2.2.3/requirements-dev.lock` & `timeseriesflattener-2.2.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/requirements.lock` & `timeseriesflattener-2.2.4/requirements.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/conftest.py` & `timeseriesflattener-2.2.4/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/test_benchmark.py` & `timeseriesflattener-2.2.4/src/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/__init__.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/_frame_validator.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/_frame_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/_intermediary_frames.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/_intermediary_frames.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/aggregators.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/from_legacy.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/meta.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/meta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/outcome.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/prediction_times.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/predictor.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/predictor.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/static.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/test_from_legacy.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/test_specs.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/timedelta.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/feature_specs/timestamp_frame.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timestamp_frame.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/flattener.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/flattener.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,18 +93,33 @@
 
 
 @dataclass
 class Flattener:
     predictiontime_frame: PredictionTimeFrame
     compute_lazily: bool = False
     n_workers: int | None = None
+    """Flatten multiple irregular time series to a static feature set.
+    
+    Args:
+        predictiontime_frame: A frame that contains the prediction times.
+        compute_lazily: If True, the computation will be done lazily.
+        n_workers: The number of workers to use for multiprocessing. 
+            If None, multiprocessing will be handled entirely by polars, otherwise, 
+            specify the number of workers to use with joblib. """
 
     def aggregate_timeseries(
         self, specs: Sequence[ValueSpecification], step_size: dt.timedelta | None = None
     ) -> AggregatedFrame:
+        """Perform the aggregation/flattening.
+        
+        Args:
+            specs: The specifications for the features to be created.
+            step_size: The step size for the aggregation. 
+                If not None, will aggregate prediction times in chunks of step_size. 
+                Reduce if you encounter memory issues."""
         if self.compute_lazily:
             print(
                 "We have encountered performance issues on Windows when using lazy evaluation. If you encounter performance issues, try setting lazy=False."
             )
 
         # Check for conflicts in the specs
         conflicting_specs = _get_spec_conflicts(specs)
```

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/process_spec.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/process_spec.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/static.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/temporal.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/test_static.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/test_temporal.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/spec_processors/timedelta.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/test_aggregators.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/test_aggregators.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 
 @dataclass(frozen=True)
 class SingleVarAggregatorExample:
     aggregator: Aggregator
     input_values: Sequence[float | None]
     expected_output_values: Sequence[float]
+    fallback_str: str = "nan"
 
     @property
     def input_frame(self) -> pl.LazyFrame:
         return pl.LazyFrame(
             {
                 "prediction_time_uuid": [1] * len(self.input_values),
                 "value": self.input_values,
@@ -54,15 +55,15 @@
         )
 
     @property
     def expected_output(self) -> pl.DataFrame:
         return pl.DataFrame(
             {
                 "prediction_time_uuid": [1],
-                f"value_{self.aggregator.name}_fallback_nan": self.expected_output_values,
+                f"value_{self.aggregator.name}_fallback_{self.fallback_str}": self.expected_output_values,
             }
         )
 
 
 AggregatorExampleType = Union[ComplexAggregatorExample, SingleVarAggregatorExample]
 
 # TODO: Write integration tests with Earliest and Latest aggregators, since they will depend on sorting
@@ -86,20 +87,21 @@
         SingleVarAggregatorExample(
             aggregator=SumAggregator(), input_values=[1, 2], expected_output_values=[3]
         ),
         SingleVarAggregatorExample(
             aggregator=VarianceAggregator(), input_values=[1, 2], expected_output_values=[0.5]
         ),
         SingleVarAggregatorExample(
-            aggregator=HasValuesAggregator(), input_values=[1, 2], expected_output_values=[1]
+            aggregator=HasValuesAggregator(), input_values=[1, 2], expected_output_values=[1], fallback_str="False"
         ),
         SingleVarAggregatorExample(
             aggregator=HasValuesAggregator(),
             input_values=[None],  # type: ignore
             expected_output_values=[0],
+            fallback_str="False",
         ),
         ComplexAggregatorExample(
             aggregator=SlopeAggregator(timestamp_col_name="timestamp"),
             input_frame=str_to_pl_df(
                 """prediction_time_uuid,timestamp,value
 1,2013-01-01,1
 1,2013-01-02,3
@@ -149,11 +151,11 @@
         masked_frame=TimeMaskedFrame(
             init_df=example.input_frame,
             value_col_names=["value"],
             prediction_time_uuid_col_name="prediction_time_uuid",
             timestamp_col_name="timestamp",
         ),
         aggregators=[example.aggregator],
-        fallback=np.nan,
+        fallback=np.nan if example.aggregator.name != "bool" else False,
     )
 
     assert_frame_equal(result.collect(), example.expected_output)
```

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/test_flattener.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/test_flattener.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/aggregation_fns.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/df_transforms.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_specs/group_specs.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/feature_specs/single_specs.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/flattened_dataset.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/flattened_ds_validator.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/logger.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/misc_utils.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/load_synth_data.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/testing/utils_for_testing.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener/v1/utils/pydantic_basemodel.py` & `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.3
+Version: 2.2.4
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.3 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.4 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.3/tasks.py` & `timeseriesflattener-2.2.4/tasks.py`

 * *Files identical despite different names*

