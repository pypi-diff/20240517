# Comparing `tmp/pz_rail_astro_tools-1.0.0.tar.gz` & `tmp/pz_rail_astro_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_astro_tools-1.0.0.tar", last modified: Mon May 13 19:53:42 2024, max compression
+gzip compressed data, was "pz_rail_astro_tools-1.0.1.tar", last modified: Fri May 17 18:43:56 2024, max compression
```

## Comparing `pz_rail_astro_tools-1.0.0.tar` & `pz_rail_astro_tools-1.0.1.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.802474 pz_rail_astro_tools-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/astro_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/rail/astro_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.802474 pz_rail_astro_tools-1.0.0/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/grid_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/observing_condition_degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/photometric_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_selections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/engines/gcr_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.802474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.834474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/tools/photometry_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/tests/astro_tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/test_gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/astro_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 18:43:55.000000 pz_rail_astro_tools-1.0.1/src/rail/astro_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/grid_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/observing_condition_degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/photometric_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_selections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/engines/gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.292702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    25884 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/testdata/rubin_dm_dc2_example2.pq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/tools/photometry_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/tests/astro_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/test_gcr_engine.py
```

### Comparing `pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.github/pull_request_template.md` & `pz_rail_astro_tools-1.0.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.github/workflows/linting.yml` & `pz_rail_astro_tools-1.0.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.github/workflows/publish-to-pypi.yml` & `pz_rail_astro_tools-1.0.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.github/workflows/smoke-test.yml` & `pz_rail_astro_tools-1.0.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.github/workflows/testing-and-coverage.yml` & `pz_rail_astro_tools-1.0.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.gitignore` & `pz_rail_astro_tools-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/.pre-commit-config.yaml` & `pz_rail_astro_tools-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/LICENSE` & `pz_rail_astro_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/PKG-INFO` & `pz_rail_astro_tools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 1.0.0
+Version: 1.0.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_astro_tools-1.0.0/README.md` & `pz_rail_astro_tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/pyproject.toml` & `pz_rail_astro_tools-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/PKG-INFO` & `pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 1.0.0
+Version: 1.0.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/SOURCES.txt` & `pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,13 +31,14 @@
 src/rail/creation/engines/gcr_engine.py
 src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
 src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
 src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
 src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+src/rail/examples_data/testdata/rubin_dm_dc2_example2.pq
 src/rail/tools/photometry_tools.py
 tests/astro_tools/test_core.py
 tests/astro_tools/test_degraders.py
 tests/astro_tools/test_gcr_engine.py
 tests/astro_tools/gcr_test_data/schema.yaml
 tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
```

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/grid_selection.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/grid_selection.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/lsst_error_model.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/observing_condition_degrader.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/observing_condition_degrader.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/photometric_errors.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/photometric_errors.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_degraders.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_selections.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/creation/engines/gcr_engine.py` & `pz_rail_astro_tools-1.0.1/src/rail/creation/engines/gcr_engine.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5` & `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits` & `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits` & `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/src/rail/tools/photometry_tools.py` & `pz_rail_astro_tools-1.0.1/src/rail/tools/photometry_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 
 import hyperbolic  # https://github.com/jlvdb/hyperbolic
 
 dustmaps_config = tables_io.lazy_modules.lazyImport('dustmaps.config')
 dustmaps_sfd = tables_io.lazy_modules.lazyImport('dustmaps.sfd')
 
 
-
-
 # default column names in DC2
 LSST_BANDS = 'ugrizy'
 DEFAULT_MAG_COLS = [f"mag_{band}_lsst" for band in LSST_BANDS]
 DEFAULT_MAGERR_COLS = [f"mag_err_{band}_lsst" for band in LSST_BANDS]
 
 
 def _compute_flux(magnitude, zeropoint):
@@ -408,85 +406,89 @@
             The converted version of the table
         """
         self.set_data('input', data)
         self.run()
         return self.get_handle('output')
 
 
-class Dereddener(RailStage):
+class DustMapBase(RailStage):
     """Utility stage that does dereddening
     
     Note: set copy_all_cols=True to copy all 
     columns in data, copy_cols will be ignored
     """
-    name = 'Dereddener'
+    name = 'DustMapBase'
 
     config_options = RailStage.config_options.copy()
     config_options.update(bands='ugrizy')
     config_options.update(mag_name="mag_{band}_lsst")
     config_options.update(band_a_env=[4.81,3.64,2.70,2.06,1.58,1.31])
     config_options.update(dustmap_name='sfd')
     config_options.update(dustmap_dir=str)
     config_options.update(copy_cols=[])
     config_options.update(copy_all_cols=False)
 
-    inputs = [('input', Hdf5Handle)]
-    outputs = [('output', Hdf5Handle)]
+    inputs = [('input', PqHandle)]
+    outputs = [('output', PqHandle)]
 
     def fetch_map(self):
         dust_map_dict = dict(sfd=dustmaps_sfd)
         try:
             dust_map_submod = dust_map_dict[self.config.dustmap_name]
         except KeyError as msg:  # pragma: no cover
             raise KeyError(f"Unknown dustmap {self.config.dustmap_name}, options are {list(dust_map_dict.keys())}") from msg
 
-        if os.path.exists(os.path.join(self.config.dustmap_dir, self.config.dustmap_name)):  # pragma: no cover
+        dustmap_dir = os.path.expandvars(self.config.dustmap_dir)
+        dustmap_path = os.path.join(dustmap_dir, self.config.dustmap_name)
+        if os.path.exists(dustmap_path):  # pragma: no cover
             # already downloaded, return
             return
         
         dust_map_config = dustmaps_config.config
-        dust_map_config['data_dir'] = self.config.dustmap_dir
+        # dust_map_config['data_dir'] = self.config.dustmap_dir
+        dust_map_config['data_dir'] = dustmap_dir
         fetch_func = dust_map_submod.fetch
         fetch_func()
         
             
     def __init__(self, args, comm=None):
         RailStage.__init__(self, args, comm=comm)
 
     def run(self):
         data = self.get_data('input', allow_missing=True)
         out_data = {}
-        coords = SkyCoord(data['ra'], data['decl'], unit = 'deg',frame='fk5')
+        coords = SkyCoord(data['ra'], data['dec'], unit = 'deg',frame='fk5')
         dust_map_dict = dict(sfd=dustmaps_sfd.SFDQuery)
         try:
             dust_map_class = dust_map_dict[self.config.dustmap_name]
             dust_map_config = dustmaps_config.config
             dust_map_config['data_dir'] = self.config.dustmap_dir
             dust_map = dust_map_class()
         except KeyError as msg:  # pragma: no cover
             raise KeyError(f"Unknown dustmap {self.config.dustmap_name}, options are {list(dust_map_dict.keys())}") from msg
         ebvvec = dust_map(coords)
         band_mag_name_list=[]
         for i, band_ in enumerate(self.config.bands):
             band_mag_name = self.config.mag_name.format(band=band_)
             mag_vals = data[band_mag_name]
-            out_data[band_mag_name] = mag_vals - ebvvec*self.config.band_a_env[i]
+            out_data[band_mag_name] = self._calc_values(mag_vals, ebvvec, self.config.band_a_env[i])
             band_mag_name_list.append(band_mag_name)
        
         # check if copy_all_cols set to true:
         if self.config.copy_all_cols==False: # pragma: no cover
             for col_ in self.config.copy_cols:  # pragma: no cover
                 out_data[col_] = data[col_]
         elif self.config.copy_all_cols==True: # pragma: no cover
             for col_ in data:
                 # make sure we do not overwrite the photometry columns
                 if col_ not in band_mag_name_list:
                     out_data[col_] = data[col_]
 
-        self.add_data('output', out_data)
+        out_data_pd = pd.DataFrame(out_data)
+        self.add_data('output', out_data_pd)
 
     def __call__(self, data):
         """Return a converted table
 
         Parameters
         ----------
         data : table-like
@@ -496,7 +498,27 @@
         -------
         out_data : table-like
             The converted version of the table
         """
         self.set_data('input', data)
         self.run()
         return self.get_handle('output')
+
+
+class Dereddener(DustMapBase):
+    """Utility stage that does dereddening
+    
+    """
+    name = 'Dereddener'
+
+    def _calc_values(self, mag_vals, ebvvec, band_a_env):
+        return mag_vals - ebvvec*band_a_env
+    
+
+class Reddener(DustMapBase):
+    """Utility stage that does reddening
+    
+    """
+    name = 'Reddener'
+
+    def _calc_values(self, mag_vals, ebvvec, band_a_env):
+        return mag_vals + ebvvec*band_a_env
```

### Comparing `pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/schema.yaml` & `pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/schema.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5` & `pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/tests/astro_tools/test_core.py` & `pz_rail_astro_tools-1.0.1/tests/astro_tools/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     Hdf5Handle,
     ModelHandle,
     PqHandle,
     QPHandle,
     TableHandle,
 )
 from rail.core.stage import RailStage
-from rail.tools.photometry_tools import HyperbolicMagnitudes, HyperbolicSmoothing, PhotometryManipulator, LSSTFluxToMagConverter, Dereddener
-from rail.utils.path_utils import RAILDIR
+from rail.tools.photometry_tools import HyperbolicMagnitudes, HyperbolicSmoothing, PhotometryManipulator, LSSTFluxToMagConverter, Dereddener, Reddener
+from rail.utils.path_utils import RAILDIR, find_rail_file
 #from rail.tools.util_stages import (
 #    LSSTFluxToMagConverter,
 #    Dereddener,
 #)
 
 
 # def test_data_file():
@@ -33,43 +33,45 @@
 #        df = DataFile('dummy', 'x')
 
 
 def test_flux2mag():
     DS = RailStage.data_store
     DS.clear()
 
-    testFile = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "rubin_dm_dc2_example.pq")
+    testFile = find_rail_file(os.path.join("examples_data", "testdata", "rubin_dm_dc2_example2.pq"))
     test_data = DS.read_file("test_data", TableHandle, testFile)
 
     fluxToMag = LSSTFluxToMagConverter.make_stage(name='flux2mag')
     out_data = fluxToMag(test_data)
 
 
 @pytest.mark.slow
 def test_dereddener():
     DS = RailStage.data_store
     DS.clear()
 
-    testFile = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "rubin_dm_dc2_example.pq")
+    testFile = find_rail_file(os.path.join("examples_data", "testdata", "rubin_dm_dc2_example2.pq"))
     test_data = DS.read_file("test_data", TableHandle, testFile)
 
-    fluxToMag = LSSTFluxToMagConverter.make_stage(name='flux2mag', copy_cols=dict(ra='ra', decl='decl'))
+    fluxToMag = LSSTFluxToMagConverter.make_stage(name='flux2mag', copy_cols=dict(ra='ra', dec='decl'))
 
     is_temp_dir = False
     dustmap_dir = os.environ.get('RAIL_DUSTMAP_DIR')
     if dustmap_dir is None:
         tmp_dustmap_dir = tempfile.TemporaryDirectory()
         dustmap_dir = tmp_dustmap_dir.name
         is_temp_dir = True
 
     dereddener = Dereddener.make_stage(name='dereddner', dustmap_dir=dustmap_dir)
+    reddener = Reddener.make_stage(name='reddner', dustmap_dir=dustmap_dir)
     dereddener.fetch_map()
 
     flux_data = fluxToMag(test_data)
     dered_data = dereddener(flux_data)
+    red_data = reddener(flux_data)
 
     if is_temp_dir:
         tmp_dustmap_dir.cleanup()
 
 
 
 @pytest.fixture
```

### Comparing `pz_rail_astro_tools-1.0.0/tests/astro_tools/test_degraders.py` & `pz_rail_astro_tools-1.0.1/tests/astro_tools/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.0/tests/astro_tools/test_gcr_engine.py` & `pz_rail_astro_tools-1.0.1/tests/astro_tools/test_gcr_engine.py`

 * *Files identical despite different names*

