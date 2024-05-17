# Comparing `tmp/smaht_submitr-0.8.2.1b4.tar.gz` & `tmp/smaht_submitr-0.8.2.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.2.1b4.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.2.1b5.tar", max compression
```

## Comparing `smaht_submitr-0.8.2.1b4.tar` & `smaht_submitr-0.8.2.1b5.tar`

### file list

```diff
@@ -1,66 +1,68 @@
--rw-r--r--   0        0        0     1098 2024-05-15 17:46:06.155018 smaht_submitr-0.8.2.1b4/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-05-15 17:46:06.155018 smaht_submitr-0.8.2.1b4/README.rst
--rw-r--r--   0        0        0     3466 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/base.py
--rw-r--r--   0        0        0      294 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/exceptions.py
--rw-r--r--   0        0        0    16784 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/file_for_upload.py
--rw-r--r--   0        0        0    11097 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/metadata_template.py
--rw-r--r--   0        0        0     2628 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/output.py
--rw-r--r--   0        0        0      377 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/__init__.py
--rw-r--r--   0        0        0    10830 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone.py
--rw-r--r--   0        0        0     8848 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_commands.py
--rw-r--r--   0        0        0     6750 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_config.py
--rw-r--r--   0        0        0     8002 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_config_amazon.py
--rw-r--r--   0        0        0     9757 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_config_google.py
--rw-r--r--   0        0        0     5152 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_installation.py
--rw-r--r--   0        0        0     2608 2024-05-15 17:46:06.195018 smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_utils.py
--rw-r--r--   0        0        0    18682 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
--rw-r--r--   0        0        0     7572 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/rclone/testing/rclone_utils_for_testing_google.py
--rw-r--r--   0        0        0    19785 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4779 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     9895 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     2824 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/get_metadata_template.py
--rw-r--r--   0        0        0     1822 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     4123 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/rcloner.py
--rw-r--r--   0        0        0     6303 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    21329 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   127817 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/submission.py
--rw-r--r--   0        0        0    14834 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/submission_uploads.py
--rw-r--r--   0        0        0        0 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0    11464 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_file_for_upload.py
--rw-r--r--   0        0        0     1620 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    34508 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_rclone_support.py
--rw-r--r--   0        0        0    11773 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0    37993 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     4353 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0     8667 2024-05-15 17:46:06.199018 smaht_submitr-0.8.2.1b4/submitr/utils.py
--rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-17 19:13:29.160236 smaht_submitr-0.8.2.1b5/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-05-17 19:13:29.160236 smaht_submitr-0.8.2.1b5/README.rst
+-rw-r--r--   0        0        0     3466 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/exceptions.py
+-rw-r--r--   0        0        0    17885 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/file_for_upload.py
+-rw-r--r--   0        0        0    11097 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/metadata_template.py
+-rw-r--r--   0        0        0     2628 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/output.py
+-rw-r--r--   0        0        0      353 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/__init__.py
+-rw-r--r--   0        0        0     6343 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_amazon.py
+-rw-r--r--   0        0        0     9291 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_commands.py
+-rw-r--r--   0        0        0     6986 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_config.py
+-rw-r--r--   0        0        0     9523 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_google.py
+-rw-r--r--   0        0        0     5152 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_installation.py
+-rw-r--r--   0        0        0     3187 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_utils.py
+-rw-r--r--   0        0        0    11817 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rcloner.py
+-rw-r--r--   0        0        0    19885 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
+-rw-r--r--   0        0        0     8157 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_google.py
+-rw-r--r--   0        0        0    17135 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/s3_upload.py
+-rw-r--r--   0        0        0     3512 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4779 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9895 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     2824 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/get_metadata_template.py
+-rw-r--r--   0        0        0     1822 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5107 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/rcloner.py
+-rw-r--r--   0        0        0     6455 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    21430 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   127795 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/submission.py
+-rw-r--r--   0        0        0    14817 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/submission_uploads.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0    12067 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_file_for_upload.py
+-rw-r--r--   0        0        0     1620 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    43766 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_rclone_support.py
+-rw-r--r--   0        0        0    11766 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0    37993 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     4353 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0     3863 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/testing_rclone_helpers.py
+-rw-r--r--   0        0        0     8677 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/utils.py
+-rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b5/PKG-INFO
```

### Comparing `smaht_submitr-0.8.2.1b4/LICENSE.txt` & `smaht_submitr-0.8.2.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/README.rst` & `smaht_submitr-0.8.2.1b5/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/pyproject.toml` & `smaht_submitr-0.8.2.1b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.2.1b4"  # TODO: To become 0.8.3
+version = "0.8.2.1b5"  # TODO: To become 0.8.3
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
@@ -45,15 +45,15 @@
 ]
 
 [tool.poetry.dependencies]
 
 python = ">=3.8.0,<3.13"
 awscli = ">=1.32.105"
 boto3 = "^1.34.105"
-dcicutils = "^8.8.4.1b32"
+dcicutils = "^8.8.4.1b33"
 PyYAML = "^6.0.1"
 requests = "^2.31.0"
 googleapi = "^0.1.0"
 
 [tool.poetry.dev-dependencies]
 
 # Coverage
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/base.py` & `smaht_submitr-0.8.2.1b5/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/file_for_upload.py` & `smaht_submitr-0.8.2.1b5/submitr/file_for_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pathlib
 from typing import Callable, List, Optional, Union
 from dcicutils.command_utils import yes_or_no
 from dcicutils.file_utils import compute_file_md5, get_file_size, normalize_path, search_for_file
 from dcicutils.misc_utils import format_size, normalize_string
 from dcicutils.structured_data import Portal, StructuredDataSet
-from submitr.rclone import RCloneConfigGoogle
+from submitr.rclone import RCloneGoogle
 
 # Unified the logic for looking for files to upload (to AWS S3), and storing
 # related info; whether or not the file is coming from the local file system
 # or from Google Cloud Storage (GCS), via rclone.
 
 
 class FileForUpload:
@@ -19,16 +19,16 @@
                  file: Union[dict, str, pathlib.Path],
                  type: Optional[str] = None,
                  accession: Optional[str] = None,
                  accession_name: Optional[str] = None,
                  uuid: Optional[str] = None,
                  main_search_directory: Optional[Union[str, pathlib.Path]] = None,
                  main_search_directory_recursively: bool = False,
-                 other_search_directories: Optional[List[Union[str, pathlib.Path]]] = None,
-                 config_google: Optional[RCloneConfigGoogle] = None) -> Optional[FileForUpload]:
+                 other_search_directories: Optional[Union[List[Union[str, pathlib.Path]], str, pathlib.Path]] = None,
+                 config_google: Optional[RCloneGoogle] = None) -> Optional[FileForUpload]:
 
         # Given file can be a dictionary (from structured_data.upload_files) like:
         # {"type": "ReferenceFile", "file": "first_file.fastq"}
         # Or a dictionary (from additional_data.upload_info of IngestionSubmission object) like:
         # {"uuid": "96f29020-7abd-4a42-b4c7-d342563b7074", "filename": "first_file.fastq"}
         # Or just a file name.
 
@@ -64,18 +64,20 @@
             # Only look at other search directories if we have no yet found the file within the main
             # search directory; and if multiple instances of the file exist within/among these other
             # directories it doesn't matter; we just take the first one we find, with no flagging of
             # multiple files found. Unlike the case (above) of searching the main search directory
             # where (if recursive is specified) we will flag any multiple file instances found.
             # In practice these other directories are the directory containing
             # the submission file, and the current directory.
+            if isinstance(other_search_directories, (str, pathlib.Path)) and other_search_directories:
+                other_search_directories = [other_search_directories]
             if (not main_search_directory and
                 not isinstance(other_search_directories, list) or not other_search_directories):  # noqa
-                # Only if no main search directory is specifed do we default the other search
-                # directories to the current directory (.), if it is not otherwise specified.
+                # Only if no main search directory is specifed do we make the default for other
+                # search directories the current directory (.), iff it is not otherwise specified.
                 other_search_directories = ["."]
             if isinstance(other_search_directories, list) and other_search_directories:
                 # Actually, other_search_directories can also be just a str and/or Path.
                 if file_path := search_for_file(self._name,
                                                 location=other_search_directories,
                                                 single=True, recursive=False):
                     file_paths = [file_path]
@@ -87,20 +89,20 @@
             if len(file_paths) > 1:
                 self._path_local_multiple = file_paths
 
         self._accession = normalize_string(accession) or None
         self._accession_name = normalize_string(accession_name) or None
         self._size_local = None
         self._checksum_local = None
-        self._config_google = config_google if isinstance(config_google, RCloneConfigGoogle) else None
+        self._config_google = config_google if isinstance(config_google, RCloneGoogle) else None
         self._path_google = None
         self._size_google = None
         self._checksum_google = None
         self._google_inaccessible = False
-        self._favor_local = True
+        self._favor_local = None
         self._ignore = False
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
@@ -117,51 +119,47 @@
 
     @property
     def uuid(self) -> Optional[str]:
         return self._uuid
 
     @property
     def from_local(self) -> bool:
-        return self.found_local and ((not self.found_google) or self.favor_local)
+        # Possible for this to return False if the file was found locally but was also found
+        # in Google Cloud Storage, and the favor_local property is None, meaning the review
+        # function has not yet been called, which resolves favor_local to True or False.
+        return self.found_local and ((not self.found_google) or (self.favor_local is True))
 
     @property
     def from_google(self) -> bool:
-        return self.found_google and ((not self.found_local) or (not self.favor_local))
+        # Same exact comment as from_local above applies here.
+        return self.found_google and ((not self.found_local) or (self.favor_local is False))
 
     @property
     def found(self) -> bool:
         return self.path_local is not None or self.path_google is not None
 
     @property
     def path(self) -> Optional[str]:
-        if self.found_local:
-            return self.path_local if not self.found_google or self.favor_local else self.path_google
-        return self.path_google if self.found_google else None
+        return self.path_local if self.from_local else (self.path_google if self.from_google else None)
 
     @property
     def display_path(self) -> Optional[str]:
-        if self.found_local:
-            return self.path_local if not self.found_google or self.favor_local else self.display_path_google
-        return self.display_path_google if self.found_google else None
+        return self.path_local if self.from_local else (self.display_path_google if self.from_google else None)
 
     @property
     def size(self) -> Optional[int]:
-        if self.found_local:
-            return self.size_local if not self.found_google or self.favor_local else self.size_google
-        return self.size_google if self.found_google else None
+        return self.size_local if self.from_local else (self.size_google if self.from_google else None)
 
     @property
     def checksum(self) -> Optional[str]:
-        if self.found_local:
-            return self.checksum_local if not self.found_google or self.favor_local else self.checksum_google
-        return self.checksum_google if self.found_google else None
+        return self.checksum_local if self.from_local else (self.checksum_google if self.from_google else None)
 
     @property
-    def favor_local(self) -> bool:
-        return self._favor_local
+    def favor_local(self) -> Optional[bool]:
+        return self._favor_local if self.found_google else True
 
     @property
     def ignore(self) -> bool:
         return self._ignore
 
     def resume_upload_command(self, env: Optional[str] = None) -> Optional[str]:
         return (f"resume-uploads{f' --env {env}' if isinstance(env, str) else ''}"
@@ -192,15 +190,15 @@
     @property
     def checksum_local(self) -> Optional[str]:
         if self._checksum_local is None and (path_local := self._path_local):
             self._checksum_local = compute_file_md5(path_local)
         return self._checksum_local
 
     @property
-    def config_google(self) -> Optional[RCloneConfigGoogle]:
+    def config_google(self) -> Optional[RCloneGoogle]:
         return self._config_google
 
     @property
     def found_google(self) -> bool:
         return self.path_google is not None
 
     @property
@@ -219,40 +217,51 @@
         if path_google := self.path_google:
             return f"gs://{path_google}"
         return None
 
     @property
     def size_google(self) -> Optional[int]:
         if self._size_google is None:
-            _ = self.path_google  # Initialize Google related info.
+            _ = self.path_google  # Initializes size as part of checking existence.
         return self._size_google
 
     @property
     def checksum_google(self) -> Optional[str]:
         if self._checksum_google is None:
-            _ = self.path_google  # Initialize Google related info.
+            if (config_google := self.config_google) and (not self._google_inaccessible):
+                if checksum_google := config_google.file_checksum(self.name):
+                    self._checksum_google = checksum_google
+                else:
+                    self._google_inaccessible = True
         return self._checksum_google
 
     def review(self, portal: Optional[Portal] = None, review_only: bool = False,
                verbose: bool = False, printf: Optional[Callable] = None) -> bool:
+        """
+        Reviews, possibly confirming interactively the file for upload. If the file
+        was found both locally (on the filesystem) and in Google Cloud Storage, we
+        will prompt the user as to which they want to use. If the file is found
+        locally multiple times (due to recursive directory search) then gives a
+        warning and skips (return False). Otherwise just returns True.
+        """
 
         if not callable(printf):
             printf = print
 
         file_identifier = self.name
         if self.uuid:
             if self.accession:
                 file_identifier += f" ({self.uuid} | {self.accession})"
             else:
                 file_identifier += f" ({self.uuid})"
         elif self.accession:
             file_identifier += f" ({self.accession})"
 
         if not self.found:
-            printf(f"- WARNING ▶ File for upload NOT FOUND: {file_identifier}")
+            printf(f"- WARNING: File for upload NOT FOUND: {file_identifier}")
             if isinstance(portal, Portal):
                 printf(f"  - Use --directory to specify a directory where the file can be found.")
                 if not review_only:
                     printf(f"  - Upload later with:"
                            f" {self.resume_upload_command(env=portal.env if portal else None)}")
             self._ignore = True
             return False
@@ -261,21 +270,22 @@
 
         if self.found_local:
             if self.found_google:
                 found_local_and_google = True
                 printf(f"- File for upload found BOTH locally AND in Google Cloud Storage: {file_identifier}")
                 printf(f"  - Google Cloud Storage: {self.display_path_google}"
                        f"{f' ({format_size(self.size_google)})' if self.size_google else ''}")
-            if self.found_local_multiple and self.favor_local:
-                # TODO
-                # Could prompt for an option to choose one of them or something.
-                # Probably not worth it; doubt it will come up much if at all.
+            if self.found_local_multiple and (not self.found_google or self._favor_local is True):
+                # Here there are multiple local files found (due to recursive directory lookup),
+                # and there was either no Google file found or if there was we are favoring local.
+                # Could prompt the user to choose which of the multiple local files to use or
+                # something; but probably not worth it; doubt it will come up much if at all.
                 if not review_only:
                     indent = ""
-                    printf(f"- WARNING ▶ Ignoring file for upload"
+                    printf(f"- WARNING: Ignoring file for upload"
                            f" as multiple/ambiguous local instances found: {file_identifier}")
                 else:
                     if found_local_and_google:
                         indent = "  "
                         printf(f"{indent}- Local file AMBIGUITY (multiple local instances found): {file_identifier}")
                     else:
                         indent = ""
@@ -330,15 +340,15 @@
 class FilesForUpload:
 
     @staticmethod
     def assemble(files: Union[StructuredDataSet, List[dict], List[Union[str, pathlib.Path]], str, pathlib.Path],
                  main_search_directory: Optional[Union[str, pathlib.Path]] = None,
                  main_search_directory_recursively: bool = False,
                  other_search_directories: Optional[List[Union[str, pathlib.Path]]] = None,
-                 config_google: Optional[RCloneConfigGoogle] = None) -> List[FileForUpload]:
+                 config_google: Optional[RCloneGoogle] = None) -> List[FileForUpload]:
 
         if isinstance(files, StructuredDataSet):
             files = files.upload_files
         elif isinstance(files, (str, pathlib.Path)):
             files = [files]
         if not isinstance(files, list):
             return []
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/metadata_template.py` & `smaht_submitr-0.8.2.1b5/submitr/metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/output.py` & `smaht_submitr-0.8.2.1b5/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/rclone.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/rcloner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from contextlib import contextmanager
 import os
 from shutil import copy as copy_file
 from typing import Callable, List, Optional, Tuple, Union
 from dcicutils.file_utils import normalize_path
 from dcicutils.tmpfile_utils import create_temporary_file_name, temporary_file
 from submitr.rclone.rclone_config import RCloneConfig
-from submitr.rclone.rclone_config_amazon import RCloneConfigAmazon
+from submitr.rclone.rclone_amazon import RCloneAmazon
 from submitr.rclone.rclone_commands import RCloneCommands
 from submitr.rclone.rclone_installation import RCloneInstallation
 from submitr.rclone.rclone_utils import cloud_path
+from submitr.utils import DEBUGGING
 
 
-class RClone(RCloneCommands, RCloneInstallation):
+class RCloner(RCloneCommands, RCloneInstallation):
 
     def __init__(self, source: Optional[RCloneConfig] = None, destination: Optional[RCloneConfig] = None) -> None:
         self._source_config = source if isinstance(source, RCloneConfig) else None
         self._destination_config = destination if isinstance(destination, RCloneConfig) else None
 
     @property
     def source(self) -> Optional[RCloneConfig]:
@@ -49,15 +50,15 @@
         return lines
 
     @contextmanager
     def config_file(self, persist: bool = False) -> str:
         with temporary_file(suffix=".conf") as temporary_config_file_name:
             os.chmod(temporary_config_file_name, 0o600)  # for security
             RCloneConfig.write_config_file(temporary_config_file_name, self.config_lines)
-            if persist is True:
+            if (persist is True) or DEBUGGING():
                 # This is just for dryrun for testing/troubleshooting.
                 persistent_config_file_name = create_temporary_file_name(suffix=".conf")
                 copy_file(temporary_config_file_name, persistent_config_file_name)
                 os.chmod(persistent_config_file_name, 0o600)  # for security
                 yield persistent_config_file_name
             else:
                 yield temporary_config_file_name
@@ -83,48 +84,56 @@
         Can force to use 'copy' by passing False as the copyto argument.
         """
         # Just FYI WRT copy/copyto:
         # - Using 'copy' when the cloud destination is a file gives error: "is a file not a directory".
         # - Using 'copyto' when the cloud destination is a "directory" creates a *file* of that name;
         #   along side the "directory" of the same name (which is odd and alomst certainly undesireble).
         if isinstance(destination_config := self.destination, RCloneConfig):
-            # Here a destination cloud configuration has been defined for this RClone object;
+            # Here a destination cloud configuration has been defined for this RCloner object;
             # meaning we are copying to some cloud destination (and not to a local file destination).
             if not (destination := destination_config.path(destination)):
                 raise Exception(f"No cloud destination specified.")
             if isinstance(source_config := self.source, RCloneConfig):
-                # Here both a source and destination cloud configuration have been defined for this RClone
+                # Here both a source and destination cloud configuration have been defined for this RCloner
                 # object; meaning we are copying from one cloud source to another cloud destination; i.e. e.g.
                 # from either Amazon S3 or Google Cloud Storage to either Amazon S3 or Google Cloud Storage.
                 if not (source := source_config.path(source)):
                     raise Exception(f"No cloud source specified.")
                 with self.config_file(persist=dryrun is True) as source_and_destination_config_file:  # noqa
                     command_args = [f"{source_config.name}:{source}", f"{destination_config.name}:{destination}"]
-                    destination_s3 = isinstance(destination_config, RCloneConfigAmazon)
+                    destination_s3 = isinstance(destination_config, RCloneAmazon)
                     return RCloneCommands.copy_command(command_args,
                                                        config=source_and_destination_config_file,
                                                        copyto=copyto, destination_s3=destination_s3,
                                                        progress=progress, dryrun=dryrun,
                                                        return_output=return_output)
             else:
-                # Here only a destination config cloud configuration has been defined for this RClone
+                # Here only a destination config cloud configuration has been defined for this RCloner
                 # object; meaning we are copying from a local file source to some cloud destination;
                 # i.e. e.g. from a local file to either Amazon S3 or Google Cloud Storage.
                 if not (source := normalize_path(source)):
                     raise Exception(f"No file source specified.")
+                elif not os.path.isfile(source):
+                    raise Exception(f"Source file not found: {source}")
+                if not cloud_path.has_separator(destination):
+                    # If the destination has no path separator then (assume) it must be just the (root)
+                    # bucket, meaning we want to do a copy rather than a copyto; though FYI not that in
+                    # general we cannot (straightforwardly) tell if the destination is a sub-folder,
+                    # such as they are in the cloud, so the caller would have to explicitly specify this.
+                    copyto = False
                 with destination_config.config_file(persist=dryrun is True) as destination_config_file:
                     command_args = [source, f"{destination_config.name}:{destination}"]
-                    destination_s3 = isinstance(destination_config, RCloneConfigAmazon)
+                    destination_s3 = isinstance(destination_config, RCloneAmazon)
                     return RCloneCommands.copy_command(command_args,
                                                        config=destination_config_file,
                                                        copyto=copyto, destination_s3=destination_s3,
                                                        progress=progress, dryrun=dryrun,
                                                        return_output=return_output)
         elif isinstance(source_config := self.source, RCloneConfig):
-            # Here only a source cloud configuration has been defined for this RClone object;
+            # Here only a source cloud configuration has been defined for this RCloner object;
             # meaning we are copying from some cloud source to a local file destination;
             # i.e. e.g. from either Amazon S3 or Google Cloud Storage to a local file.
             if source_config.bucket:
                 # A path/bucket in the source RCloneConfig is nothing more than an alternative
                 # way of manually placing it at the beginning of the given source argument.
                 source = cloud_path.join(source_config.bucket, source)
             if not (source := cloud_path.normalize(source)):
@@ -147,20 +156,28 @@
                 command_args = [f"{source_config.name}:{source}", destination]
                 return RCloneCommands.copy_command(command_args,
                                                    config=source_config_file,
                                                    copyto=True,
                                                    progress=progress, dryrun=dryrun,
                                                    return_output=return_output)
         else:
-            # Here not source or destination cloud configuration has been defined for this RClone;
+            # Here not source or destination cloud configuration has been defined for this RCloner;
             # object; meaning this is (degenerate case of a) simple local file to file copy.
             if not (source := normalize_path(source)):
                 raise Exception(f"No file source specified.")
             if not (destination := normalize_path(destination)):
                 raise Exception(f"No file destination specified.")
             if not os.path.isdir(destination):
                 copyto = True
             command_args = [source, destination]
             return RCloneCommands.copy_command(command_args,
                                                copyto=copyto,
                                                progress=progress, dryrun=dryrun,
                                                return_output=return_output)
+
+    def copy_to_bucket(self, *args, **kwargs) -> Union[bool, Tuple[bool, List[str]]]:
+        kwargs["copyto"] = False
+        return self.copy(*args, **kwargs)
+
+    def copy_to_key(self, *args, **kwargs) -> Union[bool, Tuple[bool, List[str]]]:
+        kwargs["copyto"] = True
+        return self.copy(*args, **kwargs)
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_commands.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import subprocess
 from typing import Callable, List, Optional, Tuple, Union
 from dcicutils.misc_utils import normalize_string
 from submitr.rclone.rclone_installation import RCloneInstallation
+from submitr.utils import DEBUG
 
 
 class RCloneCommands:
 
     @staticmethod
     def copy_command(args: List[str], config: Optional[str] = None, copyto: bool = False,
                      progress: Optional[Callable] = None,
@@ -30,25 +31,28 @@
         if not callable(progress):
             progress = None
         try:
             if dryrun is True:
                 if " " in command[0]:
                     command[0] = f"\"{command[0]}\""
                 return " ".join(command)
+            DEBUG(f"RCLONE-COPY-COMMAND: {' '.join(command)}")
             process = subprocess.Popen(command, universal_newlines=True,
                                        stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
             if return_output is True:
                 lines = []
             for line in process.stdout:
+                DEBUG(f"RCLONE-COPY-OUTPUT: {normalize_string(line)}")
                 if progress and (nbytes := RCloneCommands._parse_rclone_progress_bytes(line)):
                     progress(nbytes)
                 if (return_output is True) and (line := normalize_string(line)):
                     lines.append(line)
             process.stdout.close()
             result = process.wait()
+            DEBUG(f"RCLONE-COPY-RESULT: {process.returncode}")
             result = True if (result == 0) else False
             return result if not (return_output is True) else (result, lines)
         except Exception as e:
             if raise_exception is True:
                 raise e
             return False if not (return_output is True) else (False, [])
 
@@ -131,15 +135,19 @@
         if result.returncode == 0:
             if not (some_output_required is True) or (len(result.stdout) > 0):
                 return True
         return False
 
     @staticmethod
     def _execute(command: List[str]) -> subprocess.CompletedProcess:
-        return subprocess.run(command, capture_output=True, universal_newlines=True)
+        DEBUG(f"RCLONE-COMMAND: {' '.join(command)}")
+        result = subprocess.run(command, capture_output=True, universal_newlines=True)
+        DEBUG(f"RCLONE-COMMAND-OUTPUT: {normalize_string(result.stdout)}")
+        DEBUG(f"RCLONE-COMMAND-RESULT: {result.returncode}")
+        return result
 
     _RCLONE_PROGRESS_UNITS = {"KiB": 2**10, "MiB": 2**20, "GiB": 2**30, "TiB": 2**40, "PiB": 2**50, "B": 1}
     _RCLONE_PROGRESS_PATTERN = rf".*Transferred:\s*(\d+(?:\.\d+)?)\s*({'|'.join(_RCLONE_PROGRESS_UNITS.keys())}).*"
     _RCLONE_PROGRESS_REGEX = re.compile(_RCLONE_PROGRESS_PATTERN)
     _RCLONE_SIZE_PATERN = r".*\((\d+) Byte\)"
     _RCLONE_SIZE_REGEX = re.compile(_RCLONE_SIZE_PATERN)
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_config.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 from abc import ABC as AbstractBaseClass, abstractproperty
 from contextlib import contextmanager
+import os
 from shutil import copy as copy_file
 from typing import List, Optional
 from dcicutils.tmpfile_utils import create_temporary_file_name, temporary_file
 from dcicutils.misc_utils import create_uuid, normalize_string
 from submitr.rclone.rclone_commands import RCloneCommands
 from submitr.rclone.rclone_utils import cloud_path
+from submitr.utils import DEBUGGING
 
 
 class RCloneConfig(AbstractBaseClass):
 
     def __init__(self,
                  name: Optional[str] = None,
                  credentials: Optional[RCloneCredentials] = None,
                  bucket: Optional[str] = None) -> None:
         self._name = normalize_string(name) or create_uuid()
         self._credentials = credentials if isinstance(credentials, RCloneCredentials) else None
         # Here we allow not just a bucket name but any "path", such as they are (i.e. path-like),
         # beginning with a bucket name, within the cloud (S3, GCP) storage system. If set then
         # this will be prepended (via cloud_path.path/join) to any path which is operated upon,
-        # e.g. for the path_exists, file_size, file_checksum, and RClone.copy functions.
+        # e.g. for the path_exists, file_size, file_checksum, and RCloner.copy functions.
         self._bucket = cloud_path.normalize(bucket)
 
     @property
     def name(self) -> str:
         if not self._name:
             self._name = create_uuid()
         return self._name
@@ -78,18 +80,20 @@
                 if config[key] is not None:
                     lines.append(f"{key} = {config[key]}")
         return lines
 
     @contextmanager
     def config_file(self, persist: bool = False) -> str:
         with temporary_file(suffix=".conf") as temporary_config_file_name:
+            os.chmod(temporary_config_file_name, 0o600)  # for security
             self.write_config_file(temporary_config_file_name, self.config_lines)
-            if persist is True:
+            if (persist is True) or DEBUGGING():
                 persistent_config_file_name = create_temporary_file_name(suffix=".conf")
                 copy_file(temporary_config_file_name, persistent_config_file_name)
+                os.chmod(persistent_config_file_name, 0o600)  # for security
                 yield persistent_config_file_name
             else:
                 yield temporary_config_file_name
 
     @staticmethod
     def write_config_file(file: str, lines: List[str]) -> None:
         if (file := normalize_string(file)) is None:
@@ -107,49 +111,49 @@
             return cloud_path.join(self.bucket, path)
         return None
 
     def path_exists(self, path: str) -> Optional[bool]:
         # N.B. For AWS S3 rclone ls requires policies s3:GetObject and s3:ListBucket
         # for the bucket/key. So for our main use case (using Portal-granted temporary
         # credentials to copy to AWS S3, which only have s3:PutObject and s3:GetObject
-        # policies) we cannot use this. See submitr.s3_utils for special handling.
+        # policies) this will NOT work. See submitr.s3_upload for special handling.
         if path := self.path(path):
             with self.config_file() as config_file:
                 return RCloneCommands.exists_command(source=f"{self.name}:{path}", config=config_file)
         return False
 
     def file_size(self, path: str) -> Optional[int]:
         # N.B. For AWS S3 rclone size requires policies s3:GetObject and s3:ListBucket
         # for the bucket/key. So for our main use case (using Portal-granted temporary
         # credentials to copy to AWS S3, which only have s3:PutObject and s3:GetObject
-        # policies) we cannot use this. See submitr.s3_utils for special handling.
+        # policies) this will NOT work. See submitr.s3_upload for special handling.
         if path := self.path(path):
             with self.config_file() as config_file:
                 return RCloneCommands.size_command(source=f"{self.name}:{path}", config=config_file)
         return None
 
     def file_checksum(self, path: str) -> Optional[str]:
         # N.B. For AWS S3 rclone hashsum requires policies s3:GetObject and s3:ListBucket
         # for the bucket/key. So for our main use case (using Portal-granted temporary
         # credentials to copy to AWS S3, which only have s3:PutObject and s3:GetObject
-        # policies) we cannot use this. See submitr.s3_utils for special handling.
+        # policies) this will NOT work. See submitr.s3_upload for special handling.
         if path := self.path(path):
             with self.config_file() as config_file:
                 return RCloneCommands.checksum_command(source=f"{self.name}:{path}", config=config_file)
 
     def ping(self) -> bool:
         # For some reason with this command we need the project_number in the config for Google.
         with self.config_file() as config_file:
             return RCloneCommands.ping_command(source=f"{self.name}:", config=config_file)
 
-    def __eq__(self, other: RCloneConfig) -> bool:
+    def __eq__(self, other: Optional[RCloneConfig]) -> bool:
         return (isinstance(other, RCloneConfig) and
                 (self.name == other.name) and
                 (self.bucket == other.bucket) and
                 (self.credentials == other.credentials))
 
-    def __ne__(self, other: RCloneConfig) -> bool:
+    def __ne__(self, other: Optional[RCloneConfig]) -> bool:
         return not self.__eq__(other)
 
 
 class RCloneCredentials(AbstractBaseClass):
     pass
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_config_google.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_google.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,46 +8,45 @@
 from dcicutils.misc_utils import create_dict, normalize_string, PRINT
 from submitr.rclone.rclone_commands import RCloneCommands
 from submitr.rclone.rclone_config import RCloneConfig, RCloneCredentials
 from submitr.rclone.rclone_installation import RCloneInstallation
 from submitr.rclone.rclone_utils import cloud_path
 
 
-class RCloneConfigGoogle(RCloneConfig):
+class RCloneGoogle(RCloneConfig):
 
     def __init__(self,
-                 credentials_or_config: Optional[Union[GoogleCredentials, RCloneConfigGoogle]] = None,
+                 credentials_or_config: Optional[Union[GoogleCredentials, RCloneGoogle]] = None,
                  service_account_file: Optional[str] = None,
                  location: Optional[str] = None,  # analagous to AWS region
                  name: Optional[str] = None,
                  bucket: Optional[str] = None) -> None:
 
-        if isinstance(credentials_or_config, RCloneConfigGoogle):
+        if isinstance(credentials_or_config, RCloneGoogle):
+            if isinstance(credentials_or_config.credentials, GoogleCredentials):
+                credentials = GoogleCredentials(credentials=credentials_or_config.credentials, location=location)
+            else:
+                # No credentials allowed/works when running on a GCE instance.
+                credentials = None
             name = normalize_string(name) or credentials_or_config.name
             bucket = cloud_path.normalize(bucket) or credentials_or_config.bucket
-            credentials = credentials_or_config.credentials
         elif isinstance(credentials_or_config, GoogleCredentials):
-            credentials = credentials_or_config
+            credentials = GoogleCredentials(credentials=credentials_or_config, location=location)
+        elif service_account_file := normalize_path(service_account_file):
+            credentials = GoogleCredentials(service_account_file=service_account_file, location=location)
         else:
+            # No credentials allowed/works when running on a GCE instance.
             credentials = None
-        credentials = GoogleCredentials(credentials=credentials,
-                                        location=location,
-                                        service_account_file=service_account_file)
         super().__init__(name=name, bucket=bucket, credentials=credentials)
         self._project = None
 
     @property
-    def credentials(self) -> GoogleCredentials:
+    def credentials(self) -> Optional[GoogleCredentials]:
         return super().credentials
 
-    @credentials.setter
-    def credentials(self, value: GoogleCredentials) -> None:
-        if isinstance(value, GoogleCredentials):
-            super().credentials = value
-
     @property
     def config(self) -> dict:
         # The bucket_policy_only=true option indicates that rclone should enforce a bucket-only access policy,
         # meaning that object-level ACLs are not used to control access to objects within the bucket.
         return create_dict(type="google cloud storage",
                            location=self.location,
                            bucket_policy_only=True,
@@ -58,27 +57,19 @@
         # for which we actually use rclone lsd, we need to specify the project_number for Google.
         args = ["--gcs-project-number", project] if (project := self.project) else None
         with self.config_file() as config_file:
             return RCloneCommands.ping_command(source=f"{self.name}:", config=config_file, args=args)
 
     @property
     def location(self) -> Optional[str]:
-        return self._credentials.location
-
-    @location.setter
-    def location(self, value: str) -> None:
-        self._credentials.location = value
+        return self.credentials.location if self.credentials else None
 
     @property
     def service_account_file(self) -> Optional[str]:
-        return self._credentials.service_account_file
-
-    @service_account_file.setter
-    def service_account_file(self, value: str) -> None:
-        self._credentials.service_account_file = value
+        return self.credentials.service_account_file if self.credentials else None
 
     @property
     def project(self) -> Optional[str]:
         """
         Returns the Google project name (or number - either) associated with the account identified
         by the service account file (if any) or with the system (e.g. if running on a GCE instance).
         FYI only place needed was for rclone lsd comment which we use as a ping.
@@ -91,22 +82,24 @@
                     service_account_json = json.load(f)
                     if isinstance(project := service_account_json.get("project_id"), str) and project:
                         self._project = project
                         return self._project
         except Exception:
             pass
         # If no service account file specified then maybe we are on a GCE instance.
-        return RCloneConfigGoogle._get_project_name_assuming_google_compute_engine
+        if project := RCloneGoogle._get_project_name_if_google_compute_engine():
+            self._project = project
+            return self._project
 
     @staticmethod
     def is_google_compute_engine() -> Optional[str]:
-        return RCloneConfigGoogle._get_project_name_assuming_google_compute_engine() is not None
+        return RCloneGoogle._get_project_name_if_google_compute_engine() is not None
 
     @staticmethod
-    def _get_project_name_assuming_google_compute_engine() -> Optional[str]:
+    def _get_project_name_if_google_compute_engine() -> Optional[str]:
         """
         Returns the name of the Google Compute Engine (GCE) that this code is running on,
         if indeed we are running on a GCE instance; otherwise None.
         """
         try:
             # Just FYI this URL also yields more info on a GCE instance (with proper header below):
             # - http://metadata.google.internal/computeMetadata/v1/instance/?alt=json&recursive=true
@@ -122,55 +115,53 @@
             pass
         return None
 
     @staticmethod
     def from_command_args(rclone_google_source: Optional[str],
                           rclone_google_credentials: Optional[str] = None,
                           verify_installation: bool = True,
-                          printf: Optional[Callable] = None) -> Optional[RCloneConfigGoogle]:
+                          printf: Optional[Callable] = None) -> Optional[RCloneGoogle]:
         """
         Assumed to be called at the start of command-line utility (i.e. e.g. submit-metadata-bundle).
         """
         if not isinstance(rclone_google_source, str) or not rclone_google_source:
             return None
         if not callable(printf):
             printf = PRINT
         if not RCloneInstallation.verify_installation():
             printf(f"ERROR: Cannot install rclone for some reason (contact support).")
             exit(1)
         if not isinstance(rclone_google_credentials, str):
             rclone_google_credentials = None
-        if not callable(printf):
-            printf = print
         if rclone_google_credentials and not os.path.isfile(rclone_google_credentials):
             printf(f"ERROR: Google service account file does not exist: {rclone_google_credentials}")
             exit(1)
         # TODO: Allow "location" to be passed in (?); not in service account file.
-        return RCloneConfigGoogle(service_account_file=rclone_google_credentials, bucket=rclone_google_source)
+        return RCloneGoogle(service_account_file=rclone_google_credentials, bucket=rclone_google_source)
 
     def verify_connectivity(self, printf: Optional[Callable] = None) -> bool:
         if not callable(printf):
             printf = print
         if self.ping():
             printf(f"Google Cloud Storage project"
                    f"{f' ({self.project})' if self.project else ''}"
                    f" connectivity appears to be OK ✓")
             if self.bucket_exists() is False:
                 printf(f"WARNING: Google Cloud Storage bucket NOT FOUND: {self.bucket}")
             return False
         else:
             printf(f"Google Cloud Storage project"
-                   f"{f' ({self.project()})' if self.project() else ''}"
+                   f"{f' ({self.project})' if self.project else ''}"
                    f" connectivity appears to be problematic ✗")
             return True
 
-    def __eq__(self, other: RCloneConfigGoogle) -> bool:
-        return isinstance(other, RCloneConfigGoogle) and super().__eq__(other)
+    def __eq__(self, other: Optional[RCloneGoogle]) -> bool:
+        return isinstance(other, RCloneGoogle) and super().__eq__(other)
 
-    def __ne__(self, other: RCloneConfigGoogle) -> bool:
+    def __ne__(self, other: Optional[RCloneGoogle]) -> bool:
         return not self.__eq__(other)
 
 
 class GoogleCredentials(RCloneCredentials):
 
     def __init__(self,
                  credentials: Optional[GoogleCredentials] = None,
@@ -180,39 +171,31 @@
         if isinstance(credentials, GoogleCredentials):
             self._location = credentials.location
             self._service_account_file = credentials.service_account_file
         else:
             self._location = None
             self._service_account_file = None
 
+        # TODO: maybe exception if no service-account-file AND not running on GCE.
         if service_account_file := normalize_path(service_account_file, expand_home=True):
             if not os.path.isfile(service_account_file):
-                raise Exception(f"GCS service account file not found: {service_account_file}")
+                raise Exception(f"GoogleCredentials service account file not found: {service_account_file}")
             self._service_account_file = service_account_file
 
         if location := normalize_string(location):
             self._location = location
 
     @property
     def service_account_file(self) -> Optional[str]:
         return self._service_account_file
 
-    @service_account_file.setter
-    def service_account_file(self, value: str) -> None:
-        if (value := normalize_path(value)) is not None:
-            self._service_account_file = value or None
-
     @property
     def location(self) -> Optional[str]:
         return self._location
 
-    @location.setter
-    def location(self, value: str) -> None:
-        if (value := normalize_string(value)) is not None:
-            self._location = value or None
-
-    def __eq__(self, other: GoogleCredentials) -> bool:
-        return ((self.location == other.location) and
+    def __eq__(self, other: Optional[GoogleCredentials]) -> bool:
+        return (isinstance(other, GoogleCredentials) and
+                (self.location == other.location) and
                 (self.service_account_file == other.service_account_file))
 
-    def __ne__(self, other: GoogleCredentials) -> bool:
+    def __ne__(self, other: Optional[GoogleCredentials]) -> bool:
         return not self.__eq__(other)
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_installation.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_installation.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/rclone_utils.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from re import compile as re_compile, escape as re_escape
 import os
+from re import compile as re_compile, escape as re_escape
+from typing import Optional, Tuple
 
 
 class cloud_path:
 
     separator = "/"
 
     @staticmethod
@@ -43,14 +44,15 @@
     def to_file_path(value: str) -> str:
         if not (value := cloud_path.normalize(value)):
             return ""
         return value.replace(cloud_path.separator, os.sep)
 
     @staticmethod
     def basename(value: str) -> str:
+        # Returns the basename of the given cloud path (just like os.path.basename).
         if not (value := cloud_path.normalize(value)):
             return ""
         return os.path.basename(cloud_path.to_file_path(value))
 
     @staticmethod
     def bucket(value: str) -> str:
         # Returns the bucket portion of the given cloud path assuming it consists of
@@ -67,7 +69,18 @@
         # Returns the key portion of the given cloud path assuming it consists of
         # a bucket (a single name followed by a separator, i.e. a slash) followed
         # by an optional key. If no key is found then returns and empty string.
         if value := cloud_path.normalize(value):
             if (separator_index := value.find(cloud_path.separator)) > 0:
                 return value[separator_index + 1:]
         return ""
+
+    @staticmethod
+    def bucket_and_key(bucket: str, key: Optional[str] = None) -> Tuple[Optional[str], Optional[str]]:
+        if not (bucket_and_key := cloud_path.join(bucket, key)):
+            return None, None
+        if cloud_path.has_separator(bucket_and_key):
+            bucket = cloud_path.bucket(bucket_and_key)
+            key = cloud_path.key(bucket_and_key)
+            return bucket, key
+        else:
+            return bucket_and_key, None
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/testing/rclone_utils_for_testing_amazon.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_amazon.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,40 +6,34 @@
 from json import dumps as dump_json
 import os
 from typing import List, Optional, Union
 from dcicutils.file_utils import are_files_equal, normalize_path
 from dcicutils.misc_utils import create_short_uuid, normalize_string
 from dcicutils.tmpfile_utils import temporary_file
 from dcicutils.datetime_utils import format_datetime
-from submitr.rclone.rclone_config_amazon import AmazonCredentials
+from submitr.rclone.rclone_amazon import AmazonCredentials
 from submitr.rclone.rclone_utils import cloud_path
 
 
 # Module with class/functions to aid in integration testing of smaht-submitr rclone support.
 
 class AwsS3:
 
     @staticmethod
     def create(*args, **kwargs) -> AwsS3:
         return AwsS3(*args, **kwargs)
 
     def __init__(self, credentials: AmazonCredentials) -> None:
-        self._credentials = AmazonCredentials(credentials)
+        self._credentials = credentials
         self._client = None
 
     @property
     def credentials(self) -> AmazonCredentials:
         return self._credentials
 
-    @credentials.setter
-    def credentials(self, value: AmazonCredentials) -> None:
-        if isinstance(value, AmazonCredentials) and value != self._credentials:
-            self._credentials = value
-            self._client = None
-
     @property
     def client(self) -> BotoClient:
         if not self._client:
             self._client = BotoClient(
                 "s3",
                 region_name=self.credentials.region,
                 aws_access_key_id=self.credentials.access_key_id,
@@ -95,15 +89,19 @@
         except Exception as e:
             if hasattr(e, "response") and e.response.get("Error", {}).get("Code") == "404":
                 return False
             if raise_exception is True:
                 raise e
             return False
 
-    def delete_file(self, bucket: str, key: str, check: bool = False, raise_exception: bool = True) -> bool:
+    def delete_file(self, bucket: str, key: Optional[str] = None,
+                    check: bool = False, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return False
         try:
             if not (check is True) or self.file_exists(bucket, key):
                 self.client.delete_object(Bucket=bucket, Key=key)
                 return True
         except Exception as e:
             if raise_exception is True:
                 raise e
@@ -116,54 +114,69 @@
         except Exception as e:
             if hasattr(e, "response") and e.response.get("Error", {}).get("Code") == "404":
                 return False
             if raise_exception is True:
                 raise e
             return False
 
-    def file_exists(self, bucket: str, key: str, raise_exception: bool = True) -> bool:
+    def file_exists(self, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return False
         if self._file_head(bucket, key, raise_exception=raise_exception):
             return True
         return False
 
-    def file_equals(self, bucket: str, key: str, file: str, raise_exception: bool = True) -> bool:
+    def file_equals(self, file: str, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return None
         try:
             with temporary_file() as temporary_downloaded_file_name:
                 if self.download_file(bucket, key, temporary_downloaded_file_name):
                     return are_files_equal(file, temporary_downloaded_file_name)
         except Exception as e:
             if hasattr(e, "response") and e.response.get("Error", {}).get("Code") == "404":
                 return False
             if raise_exception is True:
                 raise e
         return False
 
-    def file_size(self, bucket: str, key: str, raise_exception: bool = True) -> Optional[int]:
+    def file_size(self, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> Optional[int]:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return None
         if file_head := self._file_head(bucket, key, raise_exception=raise_exception):
             return file_head.get("ContentLength", None)
         return None
 
-    def file_checksum(self, bucket: str, key: str, raise_exception: bool = True) -> Optional[str]:
+    def file_checksum(self, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> Optional[str]:
         # N.B. When using rclone to copy a file to AWS S3, it writes checksum (md5) for the file
         # to the metadata associated with the target key; it seems to put it in two places, in
         # x-amz-meta-md5chksum in the HTTPHeaders and also in md5chksum in the Metadata; see below.
         # But this is (possibly/plausibly) only for smaller sized files; see rclone.py for more
         # comments on checksums; in any case this code here is only for testing and is fine for
         # our purposes of testing the basic functioning of the rclone copy/copyto commands.
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return None
         if file_head := self._file_head(bucket, key, raise_exception=raise_exception):
             if isinstance(md5 := file_head.get("Metadata", {}).get("md5chksum"), str):
                 return base64_decode(md5).hex()
             md5 = file_head.get("ResponseMetadata", {}).get("HTTPHeaders", {}).get("x-amz-meta-md5chksum")
             if isinstance(md5, str):
                 return base64_decode(md5).hex()
             return file_head.get("ETag").strip("\"")
         return None
 
-    def file_kms_encrypted(self, bucket: str, key: str,
+    def file_kms_encrypted(self, bucket: str, key: Optional[str] = None,
                            kms_key_id: Optional[str] = None, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return None
         if file_head := self._file_head(bucket, key, raise_exception=raise_exception):
             if file_kms_key_id := file_head.get("SSEKMSKeyId"):
                 if isinstance(kms_key_id, str) and (kms_key_id := kms_key_id.strip()):
                     return True if (kms_key_id in file_kms_key_id) else False
                 return True
         return False
 
@@ -233,19 +246,18 @@
             # aws), unless these temporary (session) credentials are targetted specifically for the bucket/key.
             # actions = actions + ["s3:PutObject", "s3:DeleteObject", "s3:CreateBucket"]
             actions = actions + ["s3:PutObject"]
         statements.append({"Effect": "Allow", "Action": actions, "Resource": resources})
         if deny:
             statements.append({"Effect": "Deny", "Action": actions, "NotResource": resources})
         policy = {"Version": "2012-10-17", "Statement": statements}
-        credentials = AwsS3._generate_temporary_credentials(generating_credentials=self.credentials,
-                                                            policy=policy,
-                                                            kms_key_id=kms_key_id,
-                                                            duration=duration)
-        return AmazonCredentials(credentials) if credentials else None
+        return AwsS3._generate_temporary_credentials(generating_credentials=self.credentials,
+                                                     policy=policy,
+                                                     kms_key_id=kms_key_id,
+                                                     duration=duration)
 
     def _generate_temporary_credentials(generating_credentials: AmazonCredentials,
                                         policy: Optional[dict] = None,
                                         kms_key_id: Optional[str] = None,
                                         duration: Optional[Union[int, timedelta]] = None,
                                         raise_exception: bool = True) -> Optional[AmazonCredentials]:
         """
@@ -274,18 +286,18 @@
         try:
             sts = BotoClient("sts",
                              aws_access_key_id=generating_credentials.access_key_id,
                              aws_secret_access_key=generating_credentials.secret_access_key,
                              aws_session_token=generating_credentials.session_token)
             response = sts.get_federation_token(Name=name, Policy=policy, DurationSeconds=duration)
             if isinstance(credentials := response.get("Credentials"), dict):
-                return AmazonCredentials(access_key_id=credentials.get("AccessKeyId"),
-                                         secret_access_key=credentials.get("SecretAccessKey"),
-                                         session_token=credentials.get("SessionToken"),
-                                         kms_key_id=kms_key_id)
+                return AwsCredentials(access_key_id=credentials.get("AccessKeyId"),
+                                      secret_access_key=credentials.get("SecretAccessKey"),
+                                      session_token=credentials.get("SessionToken"),
+                                      kms_key_id=kms_key_id)
         except Exception as e:
             if raise_exception is True:
                 raise e
         return None
 
     def _file_head(self, bucket: str, key: str, raise_exception: bool = True) -> Optional[dict]:
         try:
@@ -302,54 +314,68 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def generate_temporary_credentials(self, *args, **kwargs) -> Optional[AmazonCredentials]:
         return AwsS3(self).generate_temporary_credentials(*args, **kwargs)
 
-    def to_dict(self) -> dict:
-        return {
-            "region_name": self.region,
-            "aws_access_key_id": self.access_key_id,
-            "aws_secret_access_key": self.secret_access_key,
-            "aws_session_token": self.session_token
-        }
+    def to_dictionary(self, environment_names: bool = True) -> dict:
+        # FYI used in test_rclone_support to pass into s3_upload.upload_file_to_aws_s3.
+        if environment_names is True:
+            return {
+                "AWS_DEFAULT_REGION_NAME": self.region,
+                "AWS_ACCESS_KEY_ID": self.access_key_id,
+                "AWS_SECRET_ACCESS_KEY": self.secret_access_key,
+                "AWS_SESSION_TOKEN": self.session_token
+            }
+        else:
+            return {
+                "region_name": self.region,
+                "aws_access_key_id": self.access_key_id,
+                "aws_secret_access_key": self.secret_access_key,
+                "aws_session_token": self.session_token
+            }
 
     @staticmethod
     def from_file(credentials_file: str, credentials_section: str = None,
                   kms_key_id: Optional[str] = None) -> Optional[AwsCredentials]:
         if not credentials_section:
             credentials_section = "default"
         try:
-            credentials_file = os.path.expanduser(credentials_file)
+            credentials_file = normalize_path(credentials_file, expand_home=True)
             if not os.path.isfile(credentials_file):
                 if os.path.isdir(credentials_file):
                     credentials_file = os.path.join(credentials_file, "credentials")
                 else:
                     credentials_file = os.path.join("~", f".aws_test.{credentials_file}", "credentials")
+                    credentials_file = normalize_path(credentials_file, expand_home=True)
+                if not os.path.isfile(credentials_file):
+                    return None
             config = configparser.ConfigParser()
             config.read(os.path.expanduser(credentials_file))
             section = config[credentials_section]
             region = (section.get("region", None) or
                       section.get("region_name", None) or
                       section.get("aws_default_region", None))
             access_key_id = (section.get("aws_access_key_id", None) or
                              section.get("access_key_id", None))
             secret_access_key = (section.get("aws_secret_access_key", None) or
                                  section.get("secret_access_key", None))
             session_token = (section.get("aws_session_token", None) or
                              section.get("session_token", None))
+            if not (access_key_id and secret_access_key):
+                return None
             return AwsCredentials(region=region,
                                   access_key_id=access_key_id,
                                   secret_access_key=secret_access_key,
                                   session_token=session_token,
                                   kms_key_id=kms_key_id)
         except Exception:
             pass
-        return AwsCredentials()
+        return None
 
     @staticmethod
     def from_environment_variables() -> Optional[AwsCredentials]:
         region = os.environ.get("AWS_DEFAULT_REGION", None)
         access_key_id = os.environ.get("AWS_ACCESS_KEY_ID", None)
         secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY", None)
         session_token = os.environ.get("AWS_SESSION_TOKEN", None)
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/rclone/testing/rclone_utils_for_testing_google.py` & `smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_google.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from __future__ import annotations
 import base64
 from google.cloud.storage import Client as GcsClient
 import os
 from typing import List, Optional
 from dcicutils.file_utils import are_files_equal, normalize_path
 from dcicutils.tmpfile_utils import temporary_file
-from submitr.rclone.rclone_config_google import GoogleCredentials
+from submitr.rclone.rclone_google import GoogleCredentials, RCloneGoogle
 from submitr.rclone.rclone_utils import cloud_path
 
 
 # Module with class/functions to aid in integration testing of smaht-submitr rclone support.
 
 class Gcs:
 
     def __init__(self, credentials: GoogleCredentials) -> None:
-        self._credentials = GoogleCredentials(credentials)
+        self._credentials = credentials
         self._client = None
 
     @property
     def credentials(self) -> GoogleCredentials:
         return self._credentials
 
-    @credentials.setter
-    def credentials(self, value: GoogleCredentials) -> None:
-        if isinstance(value, GoogleCredentials) and value != self._credentials:
-            self._credentials = value
-
     @property
     def client(self) -> GcsClient:
         if not self._client:
-            self._client = GcsClient.from_service_account_json(self.credentials.service_account_file)
+            if not RCloneGoogle.is_google_compute_engine():
+                self._client = GcsClient.from_service_account_json(self.credentials.service_account_file)
+            else:
+                # Credentials are implicit on a GCE.
+                self._client = GcsClient()
         return self._client
 
     def upload_file(self, file: str, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> bool:
         try:
             if not isinstance(file, str) or not file:
                 return False
             if not (bucket := cloud_path.normalize(bucket)):
@@ -82,15 +81,19 @@
             self.client.get_bucket(bucket).blob(key).download_to_filename(file)
             return True
         except Exception as e:
             if raise_exception is True:
                 raise e
             return False
 
-    def delete_file(self, bucket: str, key: str, check: bool = False, raise_exception: bool = True) -> bool:
+    def delete_file(self, bucket: str, key: Optional[str] = None,
+                    check: bool = False, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return False
         try:
             if not (check is True) or self.file_exists(bucket, key):
                 self.client.get_bucket(bucket).blob(key).delete()
                 return True
         except Exception as e:
             if raise_exception is True:
                 raise e
@@ -102,56 +105,60 @@
                 return False
             return self.client.get_bucket(bucket).exists()
         except Exception as e:
             if raise_exception is True:
                 raise e
             return False
 
-    def file_exists(self, bucket: str, key: str, raise_exception: bool = True) -> bool:
+    def file_exists(self, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return None
         try:
             if not (bucket := cloud_path.normalize(bucket)):
                 return False
             if not (key := cloud_path.normalize(key)):
                 return False
             return self.client.get_bucket(bucket).blob(key).exists()
         except Exception as e:
             if raise_exception is True:
                 raise e
             return False
 
-    def file_equals(self, bucket: str, key: str, file: str, raise_exception: bool = True) -> bool:
+    def file_equals(self, file: str, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> bool:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key or not isinstance(file, str) or not file:
+            return False
         try:
             with temporary_file() as temporary_downloaded_file_name:
                 if self.download_file(bucket, key, temporary_downloaded_file_name):
                     return are_files_equal(file, temporary_downloaded_file_name)
         except Exception as e:
             if raise_exception is True:
                 raise e
         return False
 
-    def file_size(self, bucket: str, key: str, raise_exception: bool = True) -> Optional[int]:
+    def file_size(self, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> Optional[int]:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
+            return None
         try:
-            if not (bucket := cloud_path.normalize(bucket)):
-                return None
-            if not (key := cloud_path.normalize(key)):
-                return None
             # Using list_blobs with the exact key as prefix because when just
             # using the blob directly the size is None; for some reason.
             # return self.client.get_bucket(bucket).blob(key).size
             for blob in self.client.get_bucket(bucket).list_blobs(prefix=key):
                 return blob.size
         except Exception as e:
             if raise_exception is True:
                 raise e
             return None
 
-    def file_checksum(self, bucket: str, key: str, raise_exception: bool = True) -> Optional[str]:
-        if not (bucket := cloud_path.normalize(bucket)):
-            return None
-        if not (key := cloud_path.normalize(key)):
+    def file_checksum(self, bucket: str, key: Optional[str] = None, raise_exception: bool = True) -> Optional[str]:
+        bucket, key = cloud_path.bucket_and_key(bucket, key)
+        if not bucket or not key:
             return None
         try:
             # Using list_blobs with the exact key as prefix because when just
             # using the blob directly the md5_hash is None; for some reason.
             # return self.client.get_bucket(bucket).blob(key).md5_hash
             for blob in self.client.get_bucket(bucket).list_blobs(prefix=key):
                 return base64.b64decode(blob.md5_hash).hex()
@@ -170,9 +177,13 @@
 
 class GcpCredentials(GoogleCredentials):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @staticmethod
-    def from_file(service_account_file: str, location: Optional[str] = None) -> GoogleCredentials:
+    def from_file(service_account_file: str, location: Optional[str] = None) -> Optional[GoogleCredentials]:
+        if not (service_account_file := normalize_path(service_account_file, expand_home=True)):
+            return None
+        if not os.path.isfile(service_account_file):
+            return None
         return GcpCredentials(service_account_file=service_account_file, location=location)
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/s3_utils.py` & `smaht_submitr-0.8.2.1b5/submitr/s3_upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from base64 import b64decode as base64_decode
-# import boto3
 from boto3 import client as BotoClient
 from collections import namedtuple
 import threading
 from time import time as current_timestamp
 from typing import Callable, Optional
 from dcicutils.command_utils import yes_or_no
 from dcicutils.file_utils import compute_file_md5
 from dcicutils.misc_utils import format_duration, format_size
 from dcicutils.progress_bar import ProgressBar
 from submitr.file_for_upload import FileForUpload
-from submitr.rclone import RClone, RCloneConfigAmazon, cloud_path
-from submitr.utils import get_s3_bucket_and_key_from_s3_uri, format_datetime
+from submitr.rclone import RCloner, RCloneAmazon, cloud_path
+from submitr.s3_utils import get_s3_bucket_and_key_from_s3_uri, get_s3_key_metadata
 
 # Module to upload a given file, with the given AWS credentials to AWS S3.
 # Displays progress bar and other info; checks if file already exists; verifies
 # upload; catches interrupts; et cetera. Circa May 2024 added support for upload,
 # or transfer rather, from Google Cloud Storage (GCS) directly to S3 via rclone.
 
 # Notes on checksums:
@@ -41,15 +39,15 @@
 # the uploaded S3 file/object. For local file uploads we just compute this md5 directly. For files
 # being uploaded from GCS we (trust and) take/use the md5 value stored in GCS for the file/object.
 # Then when we need the md5 of an already existing file in S3 we read this metadata rather than
 # using rclone (or boto3 for that matter) to do it.
 
 # This is to control whether or not we first prompt the user to take the time
 # to do a checksum on the local file to see if it appears to be exactly the
-# the same as an already exisiting file in AWS S3.
+# the same (based on size) as an already exisiting file in AWS S3.
 _BIG_FILE_SIZE = 1024 * 1024 * 500  # 500 MB
 
 
 def upload_file_to_aws_s3(file: FileForUpload,
                           s3_uri: str,
                           aws_credentials: Optional[dict] = None,
                           aws_kms_key_id: Optional[str] = None,
@@ -80,36 +78,36 @@
     print_preamble = print_preamble is True
     verify_upload = verify_upload is True
     catch_interrupt = catch_interrupt is True
     if not callable(printf):
         printf = print
 
     if file.from_local:
-        rclone = None
+        rcloner = None
         file_size = file.size_local
         file_checksum = None
         file_checksum_timestamp = None
 
     elif file.from_google:
-        rclone_config_google = file.config_google
-        rclone_amazon_config = RCloneConfigAmazon(region=aws_credentials.get("region_name"),
-                                                  access_key_id=aws_credentials.get("aws_access_key_id"),
-                                                  secret_access_key=aws_credentials.get("aws_secret_access_key"),
-                                                  session_token=aws_credentials.get("aws_session_token"),
-                                                  kms_key_id=aws_kms_key_id)
-        rclone = RClone(source=rclone_config_google, destination=rclone_amazon_config)
-        if not rclone_config_google.path_exists(file.name):
+        rclone_google = file.config_google
+        rclone_amazon_config = RCloneAmazon(region=aws_credentials.get("region_name"),
+                                            access_key_id=aws_credentials.get("aws_access_key_id"),
+                                            secret_access_key=aws_credentials.get("aws_secret_access_key"),
+                                            session_token=aws_credentials.get("aws_session_token"),
+                                            kms_key_id=aws_kms_key_id)
+        rcloner = RCloner(source=rclone_google, destination=rclone_amazon_config)
+        if not rclone_google.path_exists(file.name):
             printf(f"ERROR: Cannot find Google Cloud Storage object: {file.path_google}")
             return False
         file_size = file.size_google
         file_checksum = None
         # Note that it is known to be the case that calling rclone hashsum to get the checksum
         # of a file in Google Cloud Storage (GCS) merely retrieves the checksum from GCS,
         # which had previously been computed/stored by GCS for the file within GCS.
-        file_checksum = rclone_config_google.file_checksum(file.name)
+        file_checksum = rclone_google.file_checksum(file.name)
         file_checksum_timestamp = current_timestamp()
 
     else:
         raise Exception("File for upload not found; should not happen at this point!")
 
     def define_upload_file_callback(progress_total_nbytes: bool = False) -> None:
         nonlocal file_size
@@ -180,53 +178,17 @@
         upload_done = None
         should_abort = False
         threads_aborted = set()
         thread_lock = threading.Lock()
         upload_file_callback_type = namedtuple("upload_file_callback", ["function", "done", "abort_upload"])
         return upload_file_callback_type(upload_file_callback, done, abort_upload)
 
-    def get_uploaded_file_info() -> Optional[dict]:
+    def get_uploaded_file_info(strings: bool = False) -> Optional[dict]:
         nonlocal aws_credentials, s3_bucket, s3_key
-        try:
-            # Note that we do not need to use any KMS key for head_object.
-            s3 = BotoClient("s3", **aws_credentials)
-            if not isinstance(s3_file_head := s3.head_object(Bucket=s3_bucket, Key=s3_key), dict):
-                return None
-            result = {
-                "modified": format_datetime(s3_file_head.get("LastModified")),
-                "size": s3_file_head.get("ContentLength")
-            }
-            # Try getting the md5 that we ourselves wrote if/when uploading via this module.
-            if isinstance(s3_file_metadata := s3_file_head.get("Metadata"), dict):
-                if isinstance(s3_file_md5 := s3_file_metadata.get("md5"), str):
-                    result["md5"] = s3_file_md5
-                    if isinstance(s3_file_md5_timestamp := s3_file_metadata.get("md5-timestamp"), str):
-                        result["md5_timestamp"] = s3_file_md5_timestamp
-                    if isinstance(s3_file_md5_source := s3_file_metadata.get("md5-source"), str):
-                        result["md5_source"] = s3_file_md5_source
-            # As a backup check if there is an md5 written directly by rclone copy.
-            if not result.get("md5") and isinstance(s3_file_metadata, dict):
-                if s3_file_md5 := s3_file_metadata.get("md5chksum"):
-                    result["md5"] = base64_decode(s3_file_md5).hex()
-                    if isinstance(s3_file_md5_timestamp := s3_file_metadata.get("mtime"), str):
-                        result["md5_timestamp"] = s3_file_md5_timestamp
-            if not result.get("md5") and isinstance(s3_file_metadata := s3_file_head.get("ResponseMetadata"), dict):
-                if isinstance(s3_file_http_headers := s3_file_metadata.get("HTTPHeaders"), dict):
-                    if isinstance(s3_file_md5 := s3_file_http_headers.get("x-amz-meta-md5chksum"), str):
-                        result["md5"] = base64_decode(s3_file_md5).hex()
-                        if isinstance(s3_file_md5_timestamp := s3_file_http_headers.get("x-amz-meta-mtime"), str):
-                            result["md5_timestamp"] = s3_file_md5_timestamp
-            # Just for completeness and FYI get get the etag (not actually needed/used right now).
-            if isinstance(s3_file_etag := s3_file_head.get("ETag", ""), str):
-                result["etag"] = s3_file_etag.strip("\"")
-            return result
-        except Exception:
-            # Ignore error for now because (1) verification usage not absolutely necessary,
-            # and (2) portal permission change for this not yet deployed everywhere.
-            return None
+        return get_s3_key_metadata(aws_credentials, s3_bucket, s3_key, strings=strings)
 
     def verify_with_any_already_uploaded_file() -> None:
         nonlocal file, file_size, file_checksum, file_checksum_timestamp
         if existing_file_info := get_uploaded_file_info():
             existing_file_modified = existing_file_info["modified"]
             existing_file_size = existing_file_info["size"]
             existing_file_md5 = existing_file_info.get("md5")  # might not be set
@@ -264,39 +226,38 @@
             if not yes_or_no("Do you want to continue with this upload anyways?"):
                 printf(f"Skipping upload of {file.name} ({format_size(file_size)}) to: {s3_uri}")
                 return False
         return True
 
     def verify_uploaded_file() -> bool:
         nonlocal file, file_size
-        if file_info := get_uploaded_file_info():
-            printf(f"Verifying upload: {file.name} ... ", end="")
-            if file_info["size"] != file_size:
-                printf(f"WARNING: File size mismatch ▶ {file_size} vs {file_info['size']}")
-                return False
-            if file_checksum and file_info.get("md5") and (file_checksum != file_info["md5"]):
-                printf(f"WARNING: File checksum mismatch ▶ {file_checksum} vs {file_info['md5']}")
-                return False
-            printf("OK")
-            return True
-        return False
-
-    def create_metadata_for_uploading_file() -> dict:
-        nonlocal aws_credentials, s3_bucket, s3_key, file_checksum, file_checksum_timestamp
         try:
-            s3 = BotoClient("s3", **aws_credentials)
-            if isinstance(s3_file_head := s3.head_object(Bucket=s3_bucket, Key=s3_key), dict):
-                if isinstance(metadata := s3_file_head.get("Metadata"), dict):
-                    if file_checksum:
-                        metadata["md5"] = file_checksum
-                        metadata["md5-timestamp"] = str(file_checksum_timestamp)
-                        metadata["md5-source"] = "google-cloud-storage" if file.found_google else "file-system"
-                    return metadata
+            if file_info := get_uploaded_file_info():
+                printf(f"Verifying upload: {file.name} ... ", end="")
+                if file_info["size"] != file_size:
+                    printf(f"WARNING: File size mismatch ▶ {file_size} vs {file_info['size']}")
+                    return False
+                if file_checksum and file_info.get("md5") and (file_checksum != file_info["md5"]):
+                    printf(f"WARNING: File checksum mismatch ▶ {file_checksum} vs {file_info['md5']}")
+                    return False
+                printf("OK")
+                return True
         except Exception:
             pass
+        printf(f"WARNING: Could not verify upload: {file.name}")
+        return False
+
+    def create_metadata_for_uploading_file() -> dict:
+        nonlocal file, file_checksum, file_checksum_timestamp
+        if metadata := get_uploaded_file_info(strings=True):
+            if file_checksum:
+                metadata["md5"] = file_checksum
+                metadata["md5-timestamp"] = str(file_checksum_timestamp)
+                metadata["md5-source"] = "google-cloud-storage" if file.found_google else "file-system"
+            return metadata
         return {}
 
     def update_metadata_for_uploaded_file() -> bool:
         # Only need in the GCS case, as this metadata is set (via ExtraArgs) on the actual upload for S3.
         nonlocal aws_credentials, s3_bucket, s3_key
         if metadata := create_metadata_for_uploading_file():
             try:
@@ -313,36 +274,35 @@
         printf(f"▶ Upload: {file.name} ({format_size(file.size)}) ...")
         printf(f"  - From: {file.display_path}")
         printf(f"  -   To: {s3_uri}")
 
     if verify_upload and not verify_with_any_already_uploaded_file():
         return False
 
-    metadata = create_metadata_for_uploading_file()
     upload_aborted = False
-
-    if rclone:
+    if rcloner:
         upload_file_callback = define_upload_file_callback(progress_total_nbytes=True)
         try:
             # Note that the source is just file.name, which is just the base name of the file,
             # from the metadata file); the bucket (or bucket/path; whatever was passed in via
-            # --rclone-google-source) is stored in RCloneConfigGoogle (from file.config_google),
-            # and RClone.copy (which has this RCloneConfigGoogle, by virtue of RClone being
+            # --rclone-google-source) is stored in RCloneGoogle (from file.config_google),
+            # and RCloner.copy (which has this RCloneGoogle, by virtue of RCloner being
             # created with it as a source), resolves/expands this to the full Google path name.
-            rclone.copy(file.name, cloud_path.join(s3_bucket, s3_key), progress=upload_file_callback.function)
+            rcloner.copy_to_key(file.name, cloud_path.join(s3_bucket, s3_key), progress=upload_file_callback.function)
+            # Unlike non-rlone (boto) based copy, we have to set the metadata separately, after rlcone copy.
             update_metadata_for_uploaded_file()
         except Exception:
             printf(f"Upload ABORTED: {file.path_google} ◀")  # TODO: test
             upload_aborted = True
             pass
     else:
         upload_file_callback = define_upload_file_callback(progress_total_nbytes=False)
         s3 = BotoClient("s3", **aws_credentials)
         aws_extra_args = {"ServerSideEncryption": "aws:kms", "SSEKMSKeyId": aws_kms_key_id} if aws_kms_key_id else {}
-        if metadata:
+        if metadata := create_metadata_for_uploading_file():
             aws_extra_args["Metadata"] = metadata
         with open(file.path_local, "rb") as f:
             try:
                 if aws_extra_args:
                     s3.upload_fileobj(f, s3_bucket, s3_key,
                                       ExtraArgs=aws_extra_args,
                                       Callback=upload_file_callback.function)
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/get_metadata_template.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/get_metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/resume_uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from dcicutils.command_utils import script_catch_errors
 from dcicutils.misc_utils import PRINT
 from submitr.base import DEFAULT_APP
-from submitr.rclone import RCloneConfigGoogle
+from submitr.rclone import RCloneGoogle
 from submitr.submission import resume_uploads
 from submitr.scripts.cli_utils import CustomArgumentParser
 
 
 _HELP = f"""
 ===
 resume-uploads [VERSION]
@@ -83,14 +83,18 @@
     parser.add_argument('--verbose', action="store_true", default=False)
     parser.add_argument('--yes', action="store_true",
                         help="Suppress (yes/no) requests for user input.", default=False)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
     if args.directory:
+        if args.directory_only:
+            PRINT("May not specify both --directory and --directory-only")
+            exit(1)
+        args.upload_folder = args.directory
         args.upload_folder = args.directory
         directory_only = False
     if args.directory_only:
         args.upload_folder = args.directory_only
         directory_only = True
 
     if args.yes:
@@ -117,15 +121,15 @@
     if not args.upload_folder and args.directory:
         args.upload_folder = args.directory
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Specified upload directory not found: {args.upload_folder}")
         exit(1)
 
-    config_google = RCloneConfigGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
+    config_google = RCloneGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
         if args.env:
             env_from_env = True
 
@@ -136,15 +140,15 @@
                        env_from_env=env_from_env,
                        keys_file=args.keys,
                        bundle_filename=args.bundle,
                        server=args.server,
                        upload_folder=args.upload_folder,
                        no_query=args.yes,
                        subfolders=not directory_only,
-                       rclone_config_google=config_google,
+                       rclone_google=config_google,
                        output_file=args.output,
                        app=args.app,
                        verbose=args.verbose)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/submit_metadata_bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     _define_portal,
     _get_consortia,
     _get_submission_centers,
     _ping,
     _print_metadata_file_info,
     _pytesting
 )
-from submitr.rclone import RCloneConfigGoogle
+from submitr.rclone import RCloneGoogle
 
 _HELP = f"""
 ===
 submit-metadata-bundle [VERSION]
 ===
 Tool to submit submission metadata and files to SMaHT Portal.
 See: {CustomArgumentParser.HELP_URL}
@@ -227,27 +227,30 @@
     parser.add_argument('--ping', action="store_true", help="Ping server.", default=False)
     parser.add_argument('--rclone-google-source', help="Use rlcone to copy upload files from GCS.", default=None)
     parser.add_argument('--rclone-google-credentials', help="GCS credentials (service account file).", default=None)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
     if args.directory:
+        if args.directory_only:
+            PRINT("May not specify both --directory and --directory-only")
+            exit(1)
         args.upload_folder = args.directory
         directory_only = False
     if args.directory_only:
         args.upload_folder = args.directory_only
         directory_only = True
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
         if args.env:
             env_from_env = True
 
-    config_google = RCloneConfigGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
+    config_google = RCloneGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
 
     if args.ping or (args.bundle_filename and args.bundle_filename.lower() == "ping"):
         if args.env or os.environ.get("SMAHT_ENV"):
             ping_okay = _ping(env=args.env or os.environ.get("SMAHT_ENV"), env_from_env=env_from_env,
                               server=args.server, app=args.app, keys_file=args.keys, verbose=True)
             if ping_okay:
                 PRINT("Portal connectivity appears to be OK ✓")
@@ -313,15 +316,15 @@
         if not os.path.exists(args.bundle_filename):
             PRINT(f"File does not exist: {args.bundle_filename}")
             exit(1)
         _print_metadata_file_info(args.bundle_filename, env=args.env,
                                   refs=args.refs, files=args.files,
                                   subfolders=not directory_only,
                                   upload_folder=args.upload_folder,
-                                  rclone_config_google=config_google,
+                                  rclone_google=config_google,
                                   output_file=args.output,
                                   verbose=args.verbose)
         exit(0)
 
     with script_catch_errors():
 
         if not _sanity_check_submitted_file(args.bundle_filename):
@@ -339,15 +342,15 @@
                              app=args.app,
                              submission_protocol=args.submission_protocol,
                              upload_folder=args.upload_folder,
                              show_details=args.details,
                              post_only=args.post_only,
                              patch_only=args.patch_only,
                              submit=args.submit,
-                             rclone_config_google=config_google,
+                             rclone_google=config_google,
                              validate_local_only=args.validate_local_only,
                              validate_remote_only=args.validate_remote_only,
                              validate_local_skip=args.validate_local_skip,
                              validate_remote_skip=args.validate_remote_skip,
                              noanalyze=args.noanalyze,
                              json_only=args.json_only,
                              ref_nocache=args.ref_nocache,
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.2.1b5/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/submission.py` & `smaht_submitr-0.8.2.1b5/submitr/submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from dcicutils.submitr.progress_constants import PROGRESS_INGESTER, PROGRESS_LOADXL, PROGRESS_PARSE
 from dcicutils.submitr.ref_lookup_strategy import ref_lookup_strategy
 from submitr.base import DEFAULT_APP
 from submitr.exceptions import PortalPermissionError
 from submitr.file_for_upload import FilesForUpload
 from submitr.metadata_template import check_metadata_version, print_metadata_version_warning
 from submitr.output import PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW, get_output_file, setup_for_output_file_option
-from submitr.rclone import RCloneConfigGoogle
+from submitr.rclone import RCloneGoogle
 from submitr.scripts.cli_utils import get_version
 from submitr.submission_uploads import do_any_uploads
 from submitr.utils import format_path, get_health_page, is_excel_file_name, print_boxed, tobool
 
 
 def set_output_file(output_file):
     if output_file:
@@ -599,15 +599,15 @@
                          add_submission_center=None,
                          app: OrchestratedApp = None,
                          upload_folder=None,
                          no_query=False,
                          subfolders=False,
                          submission_protocol=DEFAULT_SUBMISSION_PROTOCOL,
                          submit=False,
-                         rclone_config_google=None,
+                         rclone_google=None,
                          validate_local_only=False,
                          validate_remote_only=False,
                          validate_local_skip=False,
                          validate_remote_skip=False,
                          post_only=False,
                          patch_only=False,
                          keys_file=None,
@@ -730,25 +730,26 @@
                 PRINT(f"- {known_submission_center.get('name')} ({known_submission_center.get('uuid')})")
             exit(1)
         add_submission_center = f"/submission-centers/{found_submission_centers[0]['uuid']}/"
 
     if verbose:
         SHOW(f"Metadata bundle upload bucket: {metadata_bundles_bucket}")
 
-    if rclone_config_google:
-        rclone_config_google.verify_connectivity()
+    if rclone_google:
+        rclone_google.verify_connectivity()
 
     if not noversion:
         check_metadata_version(ingestion_filename, portal=portal)
 
     if not validate_remote_only and not validate_local_skip:
         structured_data = _validate_locally(ingestion_filename, portal,
                                             validation=validation,
                                             validate_local_only=validate_local_only,
                                             autoadd=autoadd, upload_folder=upload_folder, subfolders=subfolders,
+                                            rclone_google=rclone_google,
                                             exit_immediately_on_errors=exit_immediately_on_errors,
                                             ref_nocache=ref_nocache, output_file=output_file, noprogress=noprogress,
                                             noanalyze=noanalyze, json_only=json_only, verbose_json=verbose_json,
                                             verbose=verbose, debug=debug, debug_sleep=debug_sleep)
         if validate_local_only:
             # We actually do exit from _validate_locally if validate_local_only is True.
             # This return is just emphasize that fact.
@@ -791,15 +792,15 @@
 
         SHOW(f"Validation tracking ID: {validation_uuid}")
 
         server_validation_done, server_validation_status, server_validation_response = _monitor_ingestion_process(
                 validation_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
                 show_details=show_details, report=False, messages=True,
                 validation=True,
-                rclone_config_google=rclone_config_google,
+                rclone_google=rclone_google,
                 nofiles=True, noprogress=noprogress, timeout=timeout,
                 verbose=verbose, debug=debug, debug_sleep=debug_sleep)
 
         if server_validation_status != "success":
             exit(1)
 
         PRINT("Validation results (server): OK")
@@ -810,15 +811,15 @@
               f" {'--validate-local-only' if validate_local_only else '--validate-remote-skip'}).")
 
     if validation:
         do_any_uploads(structured_data,
                        metadata_file=ingestion_filename,
                        main_search_directory=upload_folder,
                        main_search_directory_recursively=subfolders,
-                       config_google=rclone_config_google,
+                       config_google=rclone_google,
                        portal=portal,
                        verbose=True,
                        review_only=True)
         exit(0)
 
     # Server submission.
 
@@ -845,15 +846,15 @@
         debug_sleep=debug_sleep)
 
     SHOW(f"Submission tracking ID: {submission_uuid}")
 
     submission_done, submission_status, submission_response = _monitor_ingestion_process(
             submission_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
             show_details=show_details, report=False, messages=True,
-            rclone_config_google=rclone_config_google,
+            rclone_google=rclone_google,
             validation=False,
             nofiles=True, noprogress=noprogress, timeout=timeout,
             verbose=verbose, debug=debug, debug_sleep=debug_sleep)
 
     if submission_status != "success":
         exit(1)
 
@@ -861,15 +862,15 @@
 
     # Now that submission has successfully complete, review the files to upload and then do it.
 
     do_any_uploads(submission_response,
                    metadata_file=ingestion_filename,
                    main_search_directory=upload_folder,
                    main_search_directory_recursively=subfolders,
-                   config_google=rclone_config_google,
+                   config_google=rclone_google,
                    portal=portal,
                    verbose=verbose)
 
 
 def _get_recent_submissions(portal: Portal, count: int = 30, name: Optional[str] = None) -> List[dict]:
     url = f"/search/?type=IngestionSubmission&sort=-date_created&from=0&limit={count}"
     if name:
@@ -961,15 +962,15 @@
                                validation: bool = False,
                                env_from_env: bool = False,
                                report: bool = True, messages: bool = False,
                                nofiles: bool = False, noprogress: bool = False,
                                check_submission_script: bool = False,
                                upload_directory: Optional[str] = None,
                                upload_directory_recursive: bool = False,
-                               rclone_config_google: Optional[RCloneConfigGoogle] = None,
+                               rclone_google: Optional[RCloneGoogle] = None,
                                timeout: Optional[int] = None,
                                verbose: bool = False, debug: bool = False,
                                note: Optional[str] = None,
                                output_file: Optional[str] = None,
                                debug_sleep: Optional[int] = None) -> Tuple[bool, str, dict]:
 
     if output_file:
@@ -1291,15 +1292,15 @@
                 verbose=verbose, debug=debug, debug_sleep=debug_sleep)
         if submission_status != "success":
             exit(1)
         PRINT("Submission complete!")
         do_any_uploads(submission_response,
                        main_search_directory=upload_directory,
                        main_search_directory_recursively=upload_directory_recursive,
-                       config_google=rclone_config_google,
+                       config_google=rclone_google,
                        portal=portal,
                        verbose=verbose)
         return
 
     if check_submission_script or verbose or debug:  # or not validation
         PRINT(f"Details for this server {'validation' if validation else 'submission'} ({uuid}) below:")
         _print_submission_summary(portal, check_response,
@@ -1716,32 +1717,32 @@
         return upload_file_accession_based_name, upload_file_type
     except Exception:
         return None
 
 
 def resume_uploads(uuid, server=None, env=None, bundle_filename=None, keydict=None,
                    upload_folder=None, no_query=False, subfolders=False,
-                   rclone_config_google=None,
+                   rclone_google=None,
                    output_file=None, app=None, keys_file=None, env_from_env=False, verbose=False):
 
     if output_file:
         global PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW
         PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW = setup_for_output_file_option(output_file)
 
     portal = _define_portal(key=keydict, keys_file=keys_file, env=env,
                             server=server, app=app, env_from_env=env_from_env,
                             report=True, note="Resuming File Upload")
-    if rclone_config_google:
-        rclone_config_google.verify_connectivity()
+    if rclone_google:
+        rclone_google.verify_connectivity()
 
     do_any_uploads(uuid,
                    metadata_file=bundle_filename,
                    main_search_directory=upload_folder,
                    main_search_directory_recursively=subfolders,
-                   config_google=rclone_config_google,
+                   config_google=rclone_google,
                    portal=portal,
                    verbose=verbose)
 
 
 def get_metadata_bundles_bucket_from_health_path(key: dict) -> str:
     return get_health_page(key=key).get("metadata_bundles_bucket")
 
@@ -1774,16 +1775,17 @@
         if hasattr(e, "response") and e.response.get("Error", {}).get("Code", "").lower() == "accessdenied":
             PRINT(f"Access denied fetching: {results_location}")
         return (results_location, None)
 
 
 def _validate_locally(ingestion_filename: str, portal: Portal, autoadd: Optional[dict] = None,
                       validation: bool = False, validate_local_only: bool = False,
-                      upload_folder: Optional[str] = None,
-                      subfolders: bool = False, exit_immediately_on_errors: bool = False,
+                      upload_folder: Optional[str] = None, subfolders: bool = False,
+                      rclone_google: Optional[RCloneGoogle] = None,
+                      exit_immediately_on_errors: bool = False,
                       ref_nocache: bool = False, output_file: Optional[str] = None,
                       noanalyze: bool = False, json_only: bool = False, noprogress: bool = False,
                       verbose_json: bool = False, verbose: bool = False, quiet: bool = False,
                       debug: bool = False, debug_sleep: Optional[str] = None) -> StructuredDataSet:
 
     if json_only:
         noprogress = True
@@ -1897,27 +1899,30 @@
     validation_okay = _validate_data(structured_data, portal, ingestion_filename,
                                      upload_folder, recursive=subfolders, verbose=verbose, debug=debug)
     if validation_okay:
         PRINT("Validation results (preliminary): OK")
     elif exit_immediately_on_errors:
         if verbose:
             _print_structured_data_verbose(portal, structured_data, ingestion_filename, upload_folder=upload_folder,
-                                           recursive=subfolders, validation=validation, noanalyze=True, verbose=verbose)
+                                           recursive=subfolders, rclone_google=rclone_google,
+                                           validation=validation, noanalyze=True, verbose=verbose)
         if output_file:
             PRINT_STDOUT(f"Exiting with preliminary validation errors; see your output file: {output_file}")
         else:
             if not verbose:
                 PRINT_STDOUT()
             PRINT_STDOUT(f"Exiting with preliminary validation errors.")
             PRINT_STDOUT("Use the --output FILE option to write errors to a file.")
         exit(1)
 
     if verbose:
-        _print_structured_data_verbose(portal, structured_data, ingestion_filename, upload_folder=upload_folder,
-                                       recursive=subfolders, validation=validation, verbose=verbose)
+        _print_structured_data_verbose(portal, structured_data, ingestion_filename,
+                                       upload_folder=upload_folder, recursive=subfolders,
+                                       rclone_google=rclone_google,
+                                       validation=validation, verbose=verbose)
     elif not quiet:
         if not noanalyze:
             _print_structured_data_status(portal, structured_data, validation=validation,
                                           report_updates_only=True, noprogress=noprogress, verbose=verbose, debug=debug)
         else:
             PRINT("Skipping analysis of metadata wrt creates/updates to be done (per --noanalyze).")
     if not validation_okay:
@@ -2083,43 +2088,39 @@
                                 initial_validation_errors.append(
                                     f"Missing required property ({missing_required_property})"
                                     f" for type: {schema_name}")
     return initial_validation_errors
 
 
 def _print_structured_data_verbose(portal: Portal, structured_data: StructuredDataSet, ingestion_filename: str,
-                                   upload_folder: str, recursive: bool, validation: bool = False,
+                                   upload_folder: str, recursive: bool,
+                                   rclone_google: Optional[RCloneGoogle] = None,
+                                   validation: bool = False,
                                    noanalyze: bool = False, noprogress: bool = False, verbose: bool = False) -> None:
     if (reader_warnings := structured_data.reader_warnings):
         PRINT_OUTPUT(f"\n> Parser warnings:")
         for reader_warning in reader_warnings:
             PRINT_OUTPUT(f"  - {_format_issue(reader_warning, ingestion_filename)}")
     if structured_data.data:
         PRINT_OUTPUT(f"\n> Types submitting:")
         for type_name in sorted(structured_data.data):
             PRINT_OUTPUT(f"  - {type_name}: {len(structured_data.data[type_name])}"
                          f" object{'s' if len(structured_data.data[type_name]) != 1 else ''}")
     if resolved_refs := structured_data.resolved_refs:
         PRINT_OUTPUT(f"\n> Resolved object (linkTo) references:")
         for resolved_ref in sorted(resolved_refs):
             PRINT_OUTPUT(f"  - {resolved_ref}")
-    # TODO: replace with FilesForUpload
-    if files := structured_data.upload_files_located(location=[upload_folder,
-                                                               os.path.dirname(ingestion_filename) or "."],
-                                                     recursive=recursive):
-        printed_header = False
-        if files_found := [file for file in files if file.get("path")]:
-            for file in files_found:
-                path = file.get("path")
-                if not printed_header:
-                    PRINT_OUTPUT(f"\n> Resolved file references:")
-                    printed_header = True
-                PRINT_OUTPUT(f"  - {file.get('type')}: {file.get('file')} -> {path}"
-                             f" [{format_size(get_file_size(path))}]")
-    PRINT_OUTPUT()
+    files_for_upload = FilesForUpload.assemble(structured_data.upload_files,
+                                               main_search_directory=upload_folder,
+                                               main_search_directory_recursively=recursive,
+                                               config_google=rclone_google)
+    if files_for_upload:
+        PRINT_OUTPUT()
+        FilesForUpload.review(files_for_upload, review_only=True, verbose=verbose)
+        PRINT_OUTPUT()
     if not noanalyze:
         _print_structured_data_status(portal, structured_data,
                                       validation=validation,
                                       report_updates_only=True, noprogress=noprogress, verbose=verbose)
     else:
         PRINT("Skipping analysis of metadata wrt creates/updates to be done (per --noanalyze).")
 
@@ -2436,15 +2437,15 @@
     return results
 
 
 def _print_metadata_file_info(file: str, env: str,
                               refs: bool = False, files: bool = False,
                               upload_folder: Optional[str] = None,
                               subfolders: bool = False,
-                              rclone_config_google: Optional[RCloneConfigGoogle] = None,
+                              rclone_google: Optional[RCloneGoogle] = None,
                               output_file: Optional[str] = None,
                               verbose: bool = False) -> None:
     if output_file:
         set_output_file(output_file)
     PRINT(f"Metadata File: {os.path.basename(file)}")
     if size := get_file_size(file):
         PRINT(f"Size: {format_size(size)} ({size})")
@@ -2493,15 +2494,15 @@
             unchecked_refs = structured_data.unchecked_refs
             PRINT(f"References: {len(unchecked_refs)}")
             print_refs(unchecked_refs, max_output=max_output, output_file=output_file, verbose=verbose)
         if files is True:
             files_for_upload = FilesForUpload.assemble(structured_data,
                                                        main_search_directory=upload_folder,
                                                        main_search_directory_recursively=subfolders,
-                                                       config_google=rclone_config_google)
+                                                       config_google=rclone_google)
             FilesForUpload.review(files_for_upload, portal=portal, review_only=True, verbose=True, printf=PRINT)
     if not (refs is True):
         if not (files is True):
             PRINT("Note: Use --refs to view references; and --files to view files for upload.")
         else:
             PRINT("Note: Use --refs to view references (linkTo) paths.")
     elif not (files is True):
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/submission_uploads.py` & `smaht_submitr-0.8.2.1b5/submitr/submission_uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import re
 from typing import List, Optional, Tuple, Union
 from dcicutils.command_utils import yes_or_no
 from dcicutils.s3_utils import HealthPageKey
 from dcicutils.structured_data import Portal, StructuredDataSet
 from submitr.file_for_upload import FileForUpload, FilesForUpload
 from submitr.output import PRINT
-from submitr.rclone import RCloneConfigGoogle
-from submitr.s3_utils import upload_file_to_aws_s3
+from submitr.rclone import RCloneGoogle
+from submitr.s3_upload import upload_file_to_aws_s3
 from submitr.utils import tobool
 
 
 def do_any_uploads(arg: Union[str, dict, StructuredDataSet],
                    metadata_file: Optional[str] = None,
                    main_search_directory: Optional[Union[str, pathlib.PosixPath]] = None,
                    main_search_directory_recursively: bool = False,
-                   config_google: Optional[RCloneConfigGoogle] = None,
+                   config_google: Optional[RCloneGoogle] = None,
                    portal: Optional[Portal] = None,
                    review_only: bool = False,
                    verbose: bool = False) -> None:
 
     files_for_upload = assemble_files_for_upload(
         arg,
         main_search_directory=main_search_directory,
@@ -36,15 +36,15 @@
 
 
 def assemble_files_for_upload(arg: Union[str, dict, StructuredDataSet],
                               main_search_directory: Optional[Union[str, pathlib.PosixPath]] = None,
                               main_search_directory_recursively: bool = False,
                               other_search_directories: Optional[List[Union[str, pathlib.PosixPath]]] = None,
                               metadata_file: Optional[str] = None,
-                              config_google: Optional[RCloneConfigGoogle] = None,
+                              config_google: Optional[RCloneGoogle] = None,
                               portal: Optional[Portal] = None,
                               review: bool = True,
                               review_only: bool = True,
                               verbose: bool = False,
                               _recursive: bool = False) -> Optional[List[FileForUpload]]:
 
     # Returns a list of FileForUpload from the given argument; the given argument can be any of:
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_base.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_misc.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_rclone_support.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_rclone_support.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,33 @@
 import pytest
 from typing import Optional, Tuple
 from dcicutils.file_utils import are_files_equal, compute_file_md5, normalize_path
 from dcicutils.misc_utils import create_short_uuid
 from dcicutils.tmpfile_utils import (
     create_temporary_file_name, remove_temporary_file,
     temporary_directory, temporary_file, temporary_random_file)
-from submitr.rclone.rclone import RClone
+from submitr.file_for_upload import FilesForUpload
+from submitr.rclone.rcloner import RCloner
 from submitr.rclone.rclone_config import RCloneConfig
-from submitr.rclone.rclone_config_amazon import AmazonCredentials, RCloneConfigAmazon
-from submitr.rclone.rclone_config_google import GoogleCredentials, RCloneConfigGoogle
+from submitr.rclone.rclone_amazon import AmazonCredentials, RCloneAmazon
+from submitr.rclone.rclone_google import GoogleCredentials, RCloneGoogle
 from submitr.rclone.rclone_utils import cloud_path
 from submitr.rclone.testing.rclone_utils_for_testing_amazon import AwsCredentials, AwsS3
 from submitr.rclone.testing.rclone_utils_for_testing_google import GcpCredentials, Gcs
 from submitr.rclone.rclone_installation import RCloneInstallation
+from submitr.s3_upload import upload_file_to_aws_s3
+from submitr.s3_utils import get_s3_key_metadata
+from submitr.tests.testing_rclone_helpers import (
+    setup_module as rclone_setup_module, teardown_module as rclone_teardown_module, Mock_LocalStorage)
+
 
 pytestmark = pytest.mark.integration
 
-# Integration tests for RClone related functionality within smaht-submitr.
+
+# Integration tests for RCloner related functionality within smaht-submitr.
 # Need valid AWS credentials (currently for: smaht-wolf).
 # Need valid Google Cloud credentials (currently for: smaht-dac).
 # With these to variables set to True to default to getting credentials
 # from environment variables (as is done in GA), these are the environment
 # variables that need to be set:
 # - AWS_ACCESS_KEY_ID (required)
 # - AWS_SECRET_ACCESS_KEY (required)
@@ -47,66 +54,14 @@
 AMAZON_TEST_BUCKET_NAME = "smaht-unit-testing-files"
 AMAZON_KMS_KEY_ID = "27d040a3-ead1-4f5a-94ce-0fa6e7f84a95"  # not secret fyi
 GOOGLE_ACCOUNT_NAME = "smaht-dac"
 GOOGLE_TEST_BUCKET_NAME = "smaht-submitr-rclone-testing"
 GOOGLE_LOCATION = "us-east1"
 
 
-def setup_module():
-
-    global AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES
-    global GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES
-    global AMAZON_CREDENTIALS_FILE_PATH
-    global GOOGLE_SERVICE_ACCOUNT_FILE_PATH
-
-    assert RCloneInstallation.install() is not None
-    assert RCloneInstallation.is_installed() is True
-
-    if AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
-        amazon_credentials_file_path = create_temporary_file_name()
-        region = os.environ.get("AWS_DEFAULT_REGION", None)
-        access_key_id = os.environ.get("AWS_ACCESS_KEY_ID", None)
-        secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY", None)
-        session_token = os.environ.get("AWS_SESSION_TOKEN", None)
-        if access_key_id and secret_access_key:
-            with open(amazon_credentials_file_path, "w") as f:
-                f.write(f"[default]\n")
-                f.write(f"aws_default_region={region}\n") if region else None
-                f.write(f"aws_access_key_id={access_key_id}\n")
-                f.write(f"aws_secret_access_key={secret_access_key}\n")
-                f.write(f"aws_session_token={session_token}\n") if session_token else None
-            os.chmod(amazon_credentials_file_path, 0o600)  # for security
-            AMAZON_CREDENTIALS_FILE_PATH = amazon_credentials_file_path
-    if not (AMAZON_CREDENTIALS_FILE_PATH and
-            os.path.isfile(normalize_path(AMAZON_CREDENTIALS_FILE_PATH, expand_home=True))):
-        print("No Amazon credentials file defined. Skippping this test module: test_rclone_support")
-        pytest.skip()
-
-    if GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
-        if service_account_json_string := os.environ.get("GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON"):
-            service_account_json = json.loads(service_account_json_string)
-            google_service_account_file_path = create_temporary_file_name(suffix=".json")
-            with open(google_service_account_file_path, "w") as f:
-                json.dump(service_account_json, f)
-            os.chmod(google_service_account_file_path, 0o600)  # for security
-            GOOGLE_SERVICE_ACCOUNT_FILE_PATH = google_service_account_file_path
-    if not (GOOGLE_SERVICE_ACCOUNT_FILE_PATH and
-            os.path.isfile(normalize_path(GOOGLE_SERVICE_ACCOUNT_FILE_PATH, expand_home=True))):
-        print("No Google credentials file defined. Skippping this test module: test_rclone_support")
-        pytest.skip()
-
-
-def teardown_module():
-    if AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
-        remove_temporary_file(AMAZON_CREDENTIALS_FILE_PATH)
-    if GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
-        remove_temporary_file(GOOGLE_SERVICE_ACCOUNT_FILE_PATH)
-    pass
-
-
 class Env:
 
     test_file_prefix = "test-smaht-submitr-"
     test_file_suffix = ".txt"
     test_file_size = 2048
 
     def __init__(self, use_cloud_subfolder_key: bool = False):
@@ -171,91 +126,171 @@
         self.location = GOOGLE_LOCATION
         self.service_account_file = GOOGLE_SERVICE_ACCOUNT_FILE_PATH
         self.project_id = GOOGLE_ACCOUNT_NAME
         self.bucket = GOOGLE_TEST_BUCKET_NAME
 
     def credentials(self) -> GoogleCredentials:
         credentials = GcpCredentials.from_file(self.service_account_file, location=self.location)
-        assert credentials.location == self.location
-        assert credentials.service_account_file == normalize_path(self.service_account_file, expand_home=True)
-        assert os.path.isfile(credentials.service_account_file)
+        assert (credentials is not None) or RCloneGoogle.is_google_compute_engine()
+        if credentials is not None:
+            assert credentials.location == self.location
+            assert credentials.service_account_file == normalize_path(self.service_account_file, expand_home=True)
+            assert os.path.isfile(credentials.service_account_file)
         return credentials
 
     def gcs_non_rclone(self):
         return Gcs(self.credentials())
 
 
-def test_all():
-    _test_cloud_variations(use_cloud_subfolder_key=True)
-    _test_cloud_variations(use_cloud_subfolder_key=False)
-    _test_rclone_local_to_local()
+def setup_module():
+
+    rclone_setup_module()
+
+    global AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES
+    global GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES
+    global AMAZON_CREDENTIALS_FILE_PATH
+    global GOOGLE_SERVICE_ACCOUNT_FILE_PATH
+
+    assert RCloneInstallation.install() is not None
+    assert RCloneInstallation.is_installed() is True
+
+    if AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
+        amazon_credentials_file_path = create_temporary_file_name()
+        region = os.environ.get("AWS_DEFAULT_REGION", None)
+        access_key_id = os.environ.get("AWS_ACCESS_KEY_ID", None)
+        secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY", None)
+        session_token = os.environ.get("AWS_SESSION_TOKEN", None)
+        if access_key_id and secret_access_key:
+            with open(amazon_credentials_file_path, "w") as f:
+                f.write(f"[default]\n")
+                f.write(f"aws_default_region={region}\n") if region else None
+                f.write(f"aws_access_key_id={access_key_id}\n")
+                f.write(f"aws_secret_access_key={secret_access_key}\n")
+                f.write(f"aws_session_token={session_token}\n") if session_token else None
+            os.chmod(amazon_credentials_file_path, 0o600)  # for security
+            AMAZON_CREDENTIALS_FILE_PATH = amazon_credentials_file_path
+    if not (AMAZON_CREDENTIALS_FILE_PATH and
+            os.path.isfile(normalize_path(AMAZON_CREDENTIALS_FILE_PATH, expand_home=True))):
+        print("No Amazon credentials file defined. Skippping this test module: test_rclone_support")
+        pytest.skip()
+
+    if GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
+        if service_account_json_string := os.environ.get("GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON"):
+            service_account_json = json.loads(service_account_json_string)
+            google_service_account_file_path = create_temporary_file_name(suffix=".json")
+            with open(google_service_account_file_path, "w") as f:
+                json.dump(service_account_json, f)
+            os.chmod(google_service_account_file_path, 0o600)  # for security
+            GOOGLE_SERVICE_ACCOUNT_FILE_PATH = google_service_account_file_path
+    if not (GOOGLE_SERVICE_ACCOUNT_FILE_PATH and
+            os.path.isfile(normalize_path(GOOGLE_SERVICE_ACCOUNT_FILE_PATH, expand_home=True))):
+        if not RCloneGoogle.is_google_compute_engine():
+            print("No Google credentials file defined. Skippping this test module: test_rclone_support")
+            pytest.skip()
+            return
+        # Google credentials can be None on a GCE instance; i.e. no service account file needed.
+        GOOGLE_SERVICE_ACCOUNT_FILE_PATH = None
+
+    initial_setup_and_sanity_checking(env_amazon=EnvAmazon(), env_google=EnvGoogle())
+
+
+def teardown_module():
+    if AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
+        remove_temporary_file(AMAZON_CREDENTIALS_FILE_PATH)
+    if GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
+        remove_temporary_file(GOOGLE_SERVICE_ACCOUNT_FILE_PATH)
+    rclone_teardown_module()
 
 
 def initial_setup_and_sanity_checking(env_amazon: EnvAmazon, env_google: EnvGoogle) -> None:
 
     AwsCredentials.remove_credentials_from_environment_variables()
     assert os.environ.get("AWS_DEFAULT_REGION", None) is None
     assert os.environ.get("AWS_ACCESS_KEY_ID", None) is None
     assert os.environ.get("AWS_SECRET_ACCESS_KEY", None) is None
     assert os.environ.get("AWS_SESSION_TOKEN", None) is None
 
-    s3 = env_amazon.s3_non_rclone()
-    assert s3.bucket_exists(env_amazon.bucket) is True
+    assert env_amazon.s3_non_rclone().bucket_exists(env_amazon.bucket) is True
 
     credentials_google = env_google.credentials()
-    assert os.path.isfile(credentials_google.service_account_file)
-    gcs = env_google.gcs_non_rclone()
-    assert gcs.bucket_exists(env_google.bucket) is True
+    if not RCloneGoogle.is_google_compute_engine():
+        assert os.path.isfile(credentials_google.service_account_file)
+    assert env_google.gcs_non_rclone().bucket_exists(env_google.bucket) is True
+
+
+def test_all():
+    # TODO
+    # Split the _test function into separate real test_ functions;
+    # originally developed as non-pytest module.
+    _test_cloud_variations(use_cloud_subfolder_key=True)
+    _test_cloud_variations(use_cloud_subfolder_key=False)
+    _test_rclone_local_to_local()
+
+
+def _test_cloud_variations(use_cloud_subfolder_key: bool = False):
+
+    env_amazon = EnvAmazon(use_cloud_subfolder_key=use_cloud_subfolder_key)
+    env_google = EnvGoogle(use_cloud_subfolder_key=use_cloud_subfolder_key)
+    _test_utils_for_testing(env_amazon=env_amazon)
+    _test_rclone_between_amazon_and_local(env_amazon=env_amazon)
+    _test_rclone_between_google_and_local(env_google=env_google)
+    _test_rclone_google_to_amazon(env_amazon=env_amazon, env_google=env_google)
+    _test_rclone_amazon_to_google(env_amazon=env_amazon, env_google=env_google)
 
 
 def create_rclone_config_amazon(credentials: AmazonCredentials) -> RCloneConfig:
-    config = RCloneConfigAmazon(credentials)
+    config = RCloneAmazon(credentials)
     assert config.credentials == credentials
     assert config.access_key_id == credentials.access_key_id
     assert config.secret_access_key == credentials.secret_access_key
     assert config.session_token == credentials.session_token
     assert config.kms_key_id == credentials.kms_key_id
-    assert RCloneConfigAmazon(config) == config  # checking equals override
-    assert RCloneConfigAmazon(config, bucket="mismatch") != config  # checking equals override
+    assert config == config
+    assert not (config != config)
+    assert RCloneAmazon(config, bucket="mismatch") != config  # checking equals override
     return config
 
 
 def create_rclone_config_google(credentials: GoogleCredentials, env_google: EnvGoogle) -> RCloneConfig:
-    config = RCloneConfigGoogle(credentials)
+    config = RCloneGoogle(credentials)
+    # Google credentials can be None on a GCE instance.
     assert config.credentials == credentials
-    assert config.location == credentials.location
-    assert config.service_account_file == credentials.service_account_file
-    assert RCloneConfigGoogle(config) == config  # checking equals override
-    assert RCloneConfigGoogle(config, bucket="mismatch") != config  # checking equals override
+    if credentials:
+        # Google credentials can be None on a GCE instance.
+        assert config.location == credentials.location
+        assert config.service_account_file == credentials.service_account_file
+    assert config == config
+    assert not (config != config)
+    assert RCloneGoogle(config, bucket="mismatch") != config  # checking equals override
     assert config.project == env_google.project_id
     return config
 
 
-def create_rclone(source: Optional[RCloneConfig] = None, destination: Optional[RCloneConfig] = None) -> RClone:
-    rclone = RClone(source=source, destination=destination)
-    assert rclone.source == source
-    assert rclone.destination == destination
-    return rclone
+def create_rclone(source: Optional[RCloneConfig] = None, destination: Optional[RCloneConfig] = None) -> RCloner:
+    rcloner = RCloner(source=source, destination=destination)
+    assert rcloner.source == source
+    assert rcloner.destination == destination
+    return rcloner
 
 
 def sanity_check_amazon_file(env_amazon: EnvAmazon,
                              credentials: AmazonCredentials, bucket: str, key: str, file: str) -> None:
     s3 = env_amazon.s3_non_rclone()
     assert s3.file_exists(bucket, key) is True
-    assert s3.file_equals(bucket, key, file) is True
+    assert s3.file_equals(file, bucket, key) is True
     if kms_key_id := credentials.kms_key_id:
         assert s3.file_kms_encrypted(bucket, key) is True
         assert s3.file_kms_encrypted(bucket, key, kms_key_id) is True
 
 
 def sanity_check_google_file(env_google: EnvGoogle,
                              credentials: GoogleCredentials, bucket: str, key: str, file: str) -> None:
     gcs = env_google.gcs_non_rclone()
     assert gcs.file_exists(bucket, key) is True
-    assert gcs.file_equals(bucket, key, file) is True
+    assert gcs.file_equals(file, bucket, key) is True
 
 
 def cleanup_amazon_file(env_amazon: EnvAmazon, bucket: str, key: str) -> None:
     s3 = env_amazon.s3_non_rclone()
     assert s3.delete_file(bucket, key) is True
     assert s3.file_exists(bucket, key) is False
 
@@ -265,16 +300,16 @@
     assert gcs.delete_file(bucket, key) is True
     assert gcs.file_exists(bucket, key) is False
 
 
 def _test_utils_for_testing(env_amazon: EnvAmazon) -> None:
 
     # First of all, test the test code, i.e. the Amazon/Google code which uploads,
-    # downloads, verifies, et cetera - WITHOUT using RClone - in furtherance of the
-    # testing of the various RClone features.
+    # downloads, verifies, et cetera - WITHOUT using RCloner - in furtherance of the
+    # testing of the various RCloner features.
 
     credentials = env_amazon.credentials()
     _test_utils_for_testing_amazon(env_amazon=env_amazon, credentials=credentials)
 
     temporary_credentials = env_amazon.temporary_credentials()
     _test_utils_for_testing_amazon(env_amazon=env_amazon, credentials=temporary_credentials)
 
@@ -294,33 +329,33 @@
             # will specify the key explicitly, otherwise it will use just the basename of the
             # file (i.e. tmp_test_file_name); we can do this also even if the key does not have
             # a slash, but good to test specifying no key at all, i.e. in the else clause below.
             assert s3.upload_file(tmp_test_file_path, env_amazon.bucket, key) is True
         else:
             assert s3.upload_file(tmp_test_file_path, env_amazon.bucket) is True
         assert s3.file_exists(env_amazon.bucket, key) is True
-        assert s3.file_equals(env_amazon.bucket, key, tmp_test_file_path) is True
+        assert s3.file_equals(tmp_test_file_path, env_amazon.bucket, key) is True
         assert s3.file_exists(env_amazon.bucket, key + "-junk-suffix") is False
         assert len(s3_test_files := s3.list_files(env_amazon.bucket, prefix=Env.test_file_prefix)) > 0
         assert len(s3_test_files_found := [f for f in s3_test_files if f["key"] == key]) == 1
         assert s3_test_files_found[0]["key"] == key
         assert len(s3.list_files(env_amazon.bucket, prefix=key)) == 1
         with temporary_random_file() as some_random_file_path:
-            assert s3.file_equals(env_amazon.bucket, key, some_random_file_path) is False
+            assert s3.file_equals(some_random_file_path, env_amazon.bucket, key) is False
         with temporary_file() as tmp_downloaded_file_path:
             assert s3.download_file(env_amazon.bucket, key, tmp_downloaded_file_path) is True
             assert s3.download_file(env_amazon.bucket, key, "/dev/null") is True
             assert are_files_equal(tmp_test_file_path, tmp_downloaded_file_path) is True
             assert are_files_equal(tmp_test_file_path, "/dev/null") is False
         with temporary_directory() as tmp_download_directory:
             assert s3.download_file(env_amazon.bucket, key, tmp_download_directory) is True
             assert are_files_equal(tmp_test_file_path, f"{tmp_download_directory}/{key}") is True
         assert s3.delete_file(env_amazon.bucket, key) is True
         assert s3.file_exists(env_amazon.bucket, key) is False
-        assert s3.file_equals(env_amazon.bucket, key, "/dev/null") is False
+        assert s3.file_equals("/dev/null", env_amazon.bucket, key) is False
         assert s3.download_file(env_amazon.bucket, key, "/dev/null") is False
 
 
 def _test_rclone_between_amazon_and_local(env_amazon: EnvAmazon) -> None:
 
     __test_rclone_between_amazon_and_local(env_amazon=env_amazon,
                                            credentials_type_amazon=None,
@@ -353,62 +388,63 @@
         if credentials_type_amazon == EnvAmazon.CredentialsType.TEMPORARY:
             credentials_amazon = env_amazon.temporary_credentials(nokms=nokms)
         elif credentials_type_amazon == EnvAmazon.CredentialsType.TEMPORARY_KEY_SPECIFIC:
             credentials_amazon = env_amazon.temporary_credentials(bucket=env_amazon.bucket, key=key_amazon, nokms=nokms)
         else:
             credentials_amazon = env_amazon.credentials(nokms=nokms)
         config = create_rclone_config_amazon(credentials_amazon)
-        # Upload the local test file to AWS S3 using RClone;
+        # Upload the local test file to AWS S3 using RCloner;
         # we upload tmp_test_file_path to the key (tmp_test_file_name) key in env_amazon.bucket.
-        rclone = create_rclone(destination=config)
+        rcloner = create_rclone(destination=config)
         if cloud_path.has_separator(key_amazon):
             # If we are uploading to a key which has a slash (i.e. a folder-like key) then we
             # will specify the key explicitly, otherwise it will use just the basename of the
             # file (i.e. tmp_test_file_name); we can do this also even if the key does not have
             # a slash, but good to test specifying no key at all, i.e. in the else clause below.
-            assert rclone.copy(tmp_test_file_path, cloud_path.join(env_amazon.bucket, key_amazon)) is True
+            assert rcloner.copy(tmp_test_file_path, cloud_path.join(env_amazon.bucket, key_amazon)) is True
         else:
-            assert rclone.copy(tmp_test_file_path, env_amazon.bucket, copyto=False) is True
-        # Sanity check the uploaded file using non-RClone methods (via AwS3 which uses boto3).
+            assert rcloner.copy(tmp_test_file_path, env_amazon.bucket, copyto=False) is True
+        # Sanity check the uploaded file using non-rclone methods (via AwS3 which uses boto3).
         sanity_check_amazon_file(env_amazon, credentials_amazon, env_amazon.bucket, key_amazon, tmp_test_file_path)
-        # Now try to download the test file (which was uploaded above to AWS S3 using RClone) to the local file system
-        # using RClone; use the same RClone configuration as for upload, but as the source rather than the destination.
-        rclone = create_rclone(source=config)
+        # Now try to download the test file (which was uploaded above to AWS S3 using RCloner)
+        # to the local file system using RCloner; use the same RCloner configuration as for
+        # upload, but as the source rather than the destination.
+        rcloner = create_rclone(source=config)
         with temporary_directory() as tmp_download_directory:
-            rclone.copy(cloud_path.join(env_amazon.bucket, key_amazon), tmp_download_directory, copyto=False)
+            rcloner.copy(cloud_path.join(env_amazon.bucket, key_amazon), tmp_download_directory, copyto=False)
             assert are_files_equal(tmp_test_file_path,
                                    os.path.join(tmp_download_directory, cloud_path.basename(key_amazon))) is True
         # Cleanup (delete) the test file in AWS S3.
         cleanup_amazon_file(env_amazon, env_amazon.bucket, key_amazon)
 
 
 def _test_rclone_between_google_and_local(env_google: EnvGoogle) -> None:
     credentials = env_google.credentials()
     config = create_rclone_config_google(credentials, env_google)
     with Env.temporary_test_file() as (tmp_test_file_path, tmp_test_file_name):
         key_google = env_google.file_name_to_key_name(tmp_test_file_name)
         # Here we have a local test file to upload to Google Cloud Storage.
-        rclone = create_rclone(destination=config)
-        # Upload the local test file to Google Cloud Storage using RClone; we upload
+        rcloner = create_rclone(destination=config)
+        # Upload the local test file to Google Cloud Storage using RCloner; we upload
         # tmp_test_file_path to the key (tmp_test_file_name) key in env_google.bucket.
         if cloud_path.has_separator(key_google):
             # If we are uploading to a key which has a slash (i.e. a folder-like key) then we
             # will specify the key explicitly, otherwise it will use just the basename of the
             # file (i.e. tmp_test_file_name); we can do this also even if the key does not have
             # a slash, but good to test specifying no key at all, i.e. in the else clause below.
-            rclone.copy(tmp_test_file_path, cloud_path.join(env_google.bucket, key_google))
+            rcloner.copy(tmp_test_file_path, cloud_path.join(env_google.bucket, key_google))
         else:
-            rclone.copy(tmp_test_file_path, env_google.bucket, copyto=False)
-        # Sanity check the uploaded file using non-RClone methods (via Gcs which uses google.cloud.storage).
+            rcloner.copy(tmp_test_file_path, env_google.bucket, copyto=False)
+        # Sanity check the uploaded file using non-rclone methods (via Gcs which uses google.cloud.storage).
         sanity_check_google_file(env_google, credentials, env_google.bucket, key_google, tmp_test_file_path)
-        # Now try to download the uploaded test file in Google Cloud Storage using RClone;
-        # use the same RClone configuration as for upload but as the source rather than destination.
-        rclone = create_rclone(source=config)
+        # Now try to download the uploaded test file in Google Cloud Storage using RCloner;
+        # use the same RCloner configuration as for upload but as the source rather than destination.
+        rcloner = create_rclone(source=config)
         with temporary_directory() as tmp_download_directory:
-            rclone.copy(cloud_path.join(env_google.bucket, key_google), tmp_download_directory, copyto=False)
+            rcloner.copy(cloud_path.join(env_google.bucket, key_google), tmp_download_directory, copyto=False)
             assert are_files_equal(tmp_test_file_path,
                                    os.path.join(tmp_download_directory, cloud_path.basename(key_google))) is True
         # Cleanup (delete) the test file in Google Cloud Storage.
         cleanup_google_file(env_google, env_google.bucket, key_google)
 
 
 def _test_rclone_google_to_amazon(env_amazon: EnvAmazon, env_google: EnvGoogle) -> None:
@@ -437,79 +473,79 @@
 
 def __test_rclone_google_to_amazon(env_amazon: EnvAmazon,
                                    env_google: EnvGoogle,
                                    credentials_type_amazon: Optional[EnvAmazon.CredentialsType] = None,
                                    nokms: bool = False) -> None:
 
     credentials_google = env_google.credentials()
-    rclone_config_google = create_rclone_config_google(credentials_google, env_google)
+    rclone_google = create_rclone_config_google(credentials_google, env_google)
     # First upload a test file to Google Cloud Storage.
     with Env.temporary_test_file() as (tmp_test_file_path, tmp_test_file_name):
         key_amazon = env_amazon.file_name_to_key_name(tmp_test_file_name)
         key_google = env_google.file_name_to_key_name(tmp_test_file_name)
         if credentials_type_amazon == EnvAmazon.CredentialsType.TEMPORARY:
             credentials_amazon = env_amazon.temporary_credentials(nokms=nokms)
         elif credentials_type_amazon == EnvAmazon.CredentialsType.TEMPORARY_KEY_SPECIFIC:
             credentials_amazon = env_amazon.temporary_credentials(bucket=env_amazon.bucket, key=key_amazon, nokms=nokms)
         else:
             credentials_amazon = env_amazon.credentials(nokms=nokms)
-        rclone_config_amazon = create_rclone_config_amazon(credentials_amazon)
+        rclone_amazon = create_rclone_config_amazon(credentials_amazon)
         # Here we have a local test file to upload to Google Cloud Storage;
-        # which we will then copy directly to AWS S3 via RClone.
-        # So first upload our local test file to Google Cloud Storage (via RClone - why not).
-        rclone = create_rclone(destination=rclone_config_google)
+        # which we will then copy directly to AWS S3 via RCloner.
+        # So first upload our local test file to Google Cloud Storage (via RCloner - why not).
+        rcloner = create_rclone(destination=rclone_google)
         if cloud_path.has_separator(key_google):
             # If we are uploading to a key which has a slash (i.e. a folder-like key) then we
             # will specify the key explicitly, otherwise it will use just the basename of the
             # file (i.e. tmp_test_file_name); we can do this also even if the key does not have
             # a slash, but good to test specifying no key at all, i.e. in the else clause below.
-            rclone.copy(tmp_test_file_path, cloud_path.join(env_google.bucket, key_google))
+            rcloner.copy(tmp_test_file_path, cloud_path.join(env_google.bucket, key_google))
         else:
-            rclone.copy(tmp_test_file_path, env_google.bucket, copyto=False)
+            rcloner.copy(tmp_test_file_path, env_google.bucket, copyto=False)
         # Make sure it made it there.
         sanity_check_google_file(env_google, credentials_google, env_google.bucket, key_google, tmp_test_file_path)
         # Now try to copy directly from Google Cloud Storage to AWS S3 (THIS is really the MAIN event).
-        rclone = create_rclone(source=rclone_config_google, destination=rclone_config_amazon)
+        rcloner = create_rclone(source=rclone_google, destination=rclone_amazon)
         if cloud_path.has_separator(key_amazon):
             # If we are uploading to a key which has a slash (i.e. a folder-like key) then we
             # will specify the key explicitly, otherwise it will use just the basename of the
             # file (i.e. tmp_test_file_name); we can do this also even if the key does not have
             # a slash, but good to test specifying no key at all, i.e. in the else clause below.
-            rclone.copy(cloud_path.join(env_google.bucket, key_google),
-                        cloud_path.join(env_amazon.bucket, key_amazon))
+            rcloner.copy(cloud_path.join(env_google.bucket, key_google),
+                         cloud_path.join(env_amazon.bucket, key_amazon))
         else:
-            rclone.copy(cloud_path.join(env_google.bucket, key_google), env_amazon.bucket, copyto=False)
+            rcloner.copy(cloud_path.join(env_google.bucket, key_google), env_amazon.bucket, copyto=False)
         # Sanity check the file in AWS S3 which was copied directly from Google Cloud Storage.
         sanity_check_amazon_file(env_amazon, credentials_amazon, env_amazon.bucket, key_amazon, tmp_test_file_path)
         # Exercise the RCloneConfig rclone commands (path_exists, file_size, file_checksum) for Google file.
         path_google = cloud_path.join(env_google.bucket, key_google)
-        assert rclone_config_google.file_size(path_google) == Env.test_file_size
-        assert rclone_config_google.path_exists(path_google) is True
-        assert rclone_config_google.file_checksum(path_google) == compute_file_md5(tmp_test_file_path)
-        assert rclone_config_google.ping() is True
+        assert rclone_google.file_size(path_google) == Env.test_file_size
+        assert rclone_google.path_exists(path_google) is True
+        assert rclone_google.file_checksum(path_google) == compute_file_md5(tmp_test_file_path)
+        assert rclone_google.ping() is True
         # Exercise the RCloneConfig rclone commands (path_exists, file_size, file_checksum) for Amazon file.
         assert env_amazon.s3_non_rclone().file_size(env_amazon.bucket, key_amazon) == Env.test_file_size
         assert env_amazon.s3_non_rclone().file_exists(env_amazon.bucket, key_amazon) is True
         assert (env_amazon.s3_non_rclone().file_checksum(env_amazon.bucket, key_amazon) ==
                 compute_file_md5(tmp_test_file_path))
         # Do the above copy again but this time with the destination
-        # bucket specified within the RCloneConfigGoogle object (new: 2024-05-10).
+        # bucket specified within the RCloneGoogle object (new: 2024-05-10).
         cleanup_amazon_file(env_amazon, env_amazon.bucket, key_amazon)
-        rclone_config_amazon.bucket = env_amazon.bucket
-        assert rclone_config_amazon.bucket == env_amazon.bucket
-        assert rclone_config_amazon.path("testing-path-function") == f"{env_amazon.bucket}/testing-path-function"
-        assert rclone_config_amazon.path_exists(key_amazon) is False
+        rclone_amazon.bucket = env_amazon.bucket
+        assert rclone_amazon.bucket == env_amazon.bucket
+        assert rclone_amazon.path("testing-path-function") == f"{env_amazon.bucket}/testing-path-function"
+        assert rclone_amazon.path_exists(key_amazon) is False
         if cloud_path.has_separator(key_amazon):
             # If we are uploading to a key which has a slash (i.e. a folder-like key) then we
             # will specify the key explicitly, otherwise it will use just the basename of the
             # file (i.e. tmp_test_file_name); we can do this also even if the key does not have
             # a slash, but good to test specifying no key at all, i.e. in the else clause below.
-            rclone.copy(cloud_path.join(env_google.bucket, key_google), key_amazon)
+            rcloner.copy(cloud_path.join(env_google.bucket, key_google), key_amazon)
         else:
-            rclone.copy(cloud_path.join(env_google.bucket, key_google), None, copyto=False)
+            rcloner.copy(cloud_path.join(env_google.bucket, key_google), None, copyto=False)
         # Sanity check the file in AWS S3 which was copied directly from Google Cloud Storage.
         sanity_check_amazon_file(env_amazon, credentials_amazon, env_amazon.bucket, key_amazon, tmp_test_file_path)
         # Re-exercise the RCloneConfig rclone commands (path_exists, file_size, file_checksum) for Amazon file.
         assert env_amazon.s3_non_rclone().file_size(env_amazon.bucket, key_amazon) == Env.test_file_size
         assert env_amazon.s3_non_rclone().file_exists(env_amazon.bucket, key_amazon) is True
         assert (env_amazon.s3_non_rclone().file_checksum(env_amazon.bucket, key_amazon) ==
                 compute_file_md5(tmp_test_file_path))
@@ -518,73 +554,191 @@
         # Cleanup (delete) the test source file in Google Cloud Storage.
         cleanup_google_file(env_google, env_google.bucket, key_google)
 
 
 def _test_rclone_amazon_to_google(env_amazon: EnvAmazon, env_google: EnvGoogle) -> None:
     credentials_amazon = env_amazon.credentials()
     credentials_google = env_google.credentials()
-    rclone_config_amazon = create_rclone_config_amazon(credentials_amazon)
-    rclone_config_google = create_rclone_config_google(credentials_google, env_google)
+    rclone_amazon = create_rclone_config_amazon(credentials_amazon)
+    rclone_google = create_rclone_config_google(credentials_google, env_google)
     # First upload a test file to AWS S3.
     with Env.temporary_test_file() as (tmp_test_file_path, tmp_test_file_name):
         key_amazon = env_amazon.file_name_to_key_name(tmp_test_file_name)
         key_google = env_google.file_name_to_key_name(tmp_test_file_name)
         # Here we have a local test file to upload to AWS S3;
-        # which we will then copy directly to Google Cloud Storage via RClone.
-        # So first upload our local test file to AWS S3 (via RClone - why not).
-        rclone = create_rclone(destination=rclone_config_amazon)
+        # which we will then copy directly to Google Cloud Storage via RCloner.
+        # So first upload our local test file to AWS S3 (via RCloner - why not).
+        rcloner = create_rclone(destination=rclone_amazon)
         if cloud_path.has_separator(key_google):
-            rclone.copy(tmp_test_file_path, cloud_path.join(env_amazon.bucket, key_amazon))
+            rcloner.copy(tmp_test_file_path, cloud_path.join(env_amazon.bucket, key_amazon))
         else:
-            rclone.copy(tmp_test_file_path, env_amazon.bucket, copyto=False)
+            rcloner.copy(tmp_test_file_path, env_amazon.bucket, copyto=False)
         # Make sure it made it there.
         sanity_check_amazon_file(env_amazon, credentials_amazon, env_amazon.bucket, key_amazon, tmp_test_file_path)
         # Now try to copy directly from AWS S3 to Google Cloud Storage.
-        rclone = create_rclone(source=rclone_config_amazon, destination=rclone_config_google)
+        rcloner = create_rclone(source=rclone_amazon, destination=rclone_google)
         if cloud_path.has_separator(key_google):
-            rclone.copy(cloud_path.join(env_amazon.bucket, key_amazon),
-                        cloud_path.join(env_google.bucket, key_google))
+            rcloner.copy(cloud_path.join(env_amazon.bucket, key_amazon),
+                         cloud_path.join(env_google.bucket, key_google))
         else:
-            rclone.copy(cloud_path.join(env_amazon.bucket, key_amazon), env_google.bucket, copyto=False)
+            rcloner.copy(cloud_path.join(env_amazon.bucket, key_amazon), env_google.bucket, copyto=False)
         # Sanity check the file in Google Cloud Storage which was copied directly from AWS S3.
         sanity_check_google_file(env_google, credentials_google, env_google.bucket, key_google, tmp_test_file_path)
         # Cleanup (delete) the test destination file in Google Cloud Storage.
         # Do the above copy again but this time with the destination
-        # bucket specified within the RCloneConfigGoogle object (new: 2024-05-10).
+        # bucket specified within the RCloneGoogle object (new: 2024-05-10).
         cleanup_google_file(env_google, env_google.bucket, key_google)
-        rclone_config_google.bucket = env_google.bucket
-        rclone = create_rclone(source=rclone_config_amazon, destination=rclone_config_google)
+        rclone_google.bucket = env_google.bucket
+        rcloner = create_rclone(source=rclone_amazon, destination=rclone_google)
         if cloud_path.has_separator(key_google):
-            rclone.copy(cloud_path.join(env_amazon.bucket, key_amazon), key_google)
+            rcloner.copy(cloud_path.join(env_amazon.bucket, key_amazon), key_google)
         else:
-            rclone.copy(cloud_path.join(env_amazon.bucket, key_amazon), None, copyto=False)
+            rcloner.copy(cloud_path.join(env_amazon.bucket, key_amazon), None, copyto=False)
         # Sanity check the file in Google Cloud Storage which was copied directly from AWS S3.
         sanity_check_google_file(env_google, credentials_google, env_google.bucket, key_google, tmp_test_file_path)
         # Cleanup (delete) the test destination file in Google Cloud Storage.
         cleanup_google_file(env_google, env_google.bucket, key_google)
         # Cleanup (delete) the test source file in AWS S3.
         cleanup_amazon_file(env_amazon, env_amazon.bucket, key_amazon)
 
 
 def _test_rclone_local_to_local() -> None:
     # Just for completeness, and pretty much falls out, we
     # support the degenerate case of local file to file copy via rclone.
     with Env.temporary_test_file() as (tmp_test_file_path, tmp_test_file_name):
         with temporary_file() as tmp_destination_file:
-            RClone().copy(tmp_test_file_path, tmp_destination_file)
+            RCloner().copy(tmp_test_file_path, tmp_destination_file)
             assert are_files_equal(tmp_test_file_path, tmp_destination_file)
         with temporary_directory() as tmp_destination_directory:
-            RClone().copy(tmp_test_file_path, tmp_destination_directory, copyto=False)
+            RCloner().copy(tmp_test_file_path, tmp_destination_directory, copyto=False)
             assert are_files_equal(tmp_test_file_path,
                                    os.path.join(tmp_destination_directory, os.path.basename(tmp_test_file_path)))
 
 
-def _test_cloud_variations(use_cloud_subfolder_key: bool = False):
+def test_rclone_google_to_amazon_more() -> None:
 
-    env_amazon = EnvAmazon(use_cloud_subfolder_key=use_cloud_subfolder_key)
-    env_google = EnvGoogle(use_cloud_subfolder_key=use_cloud_subfolder_key)
-    initial_setup_and_sanity_checking(env_amazon=env_amazon, env_google=env_google)
-    _test_utils_for_testing(env_amazon=env_amazon)
-    _test_rclone_between_amazon_and_local(env_amazon=env_amazon)
-    _test_rclone_between_google_and_local(env_google=env_google)
-    _test_rclone_google_to_amazon(env_amazon=env_amazon, env_google=env_google)
-    _test_rclone_amazon_to_google(env_amazon=env_amazon, env_google=env_google)
+    filesize = 1235
+    filesystem = Mock_LocalStorage()
+    file_one = "subdir/test_file_one.fastq"
+    file_two = "test_file_two.fastq"
+    filesystem.create_files(file_one, nbytes=filesize)
+    # env_amazon = EnvAmazon(use_cloud_subfolder_key=True)
+    env_google = EnvGoogle(use_cloud_subfolder_key=True)
+    bucket_google = f"{env_google.bucket}/test-{create_short_uuid(31)}"
+    credentials_google = env_google.credentials()
+    rclone_google = RCloneGoogle(credentials_google, bucket=bucket_google)
+    rcloner = RCloner(destination=rclone_google)
+    # Note that the second destination argument to RCloner.copy can be
+    # unspecified meaning that it will be the *bucket* ("bucket" - can be
+    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
+    assert env_google.gcs_non_rclone().file_size(cloud_path.join(bucket_google, os.path.basename(file_one))) == filesize
+    assert env_google.gcs_non_rclone().file_size(bucket_google, os.path.basename(file_one)) == filesize
+    files = [{"filename": file_one},
+             {"filename": file_two}]
+    files_for_upload = FilesForUpload.assemble(files,
+                                               main_search_directory=filesystem.root,
+                                               main_search_directory_recursively=True,
+                                               config_google=rclone_google)
+    assert len(files_for_upload) == 2
+    assert files_for_upload[0].found is True
+    assert files_for_upload[0].found_local is True
+    assert files_for_upload[0].found_google is True
+    assert files_for_upload[0].path_local == os.path.join(filesystem.root, file_one)
+    assert files_for_upload[0].size_local == filesize
+    assert len(files_for_upload[0].checksum_local) > 0
+    assert files_for_upload[0].path_google == cloud_path.join(bucket_google, files_for_upload[0].name)
+    assert files_for_upload[0].size_google == filesize
+    assert len(files_for_upload[0].checksum_google) > 0
+    # Found both locally and in Google; ambiguous, as favor_local starts as None;
+    # so these return False/None; favor_local normally gets resolved in review function.
+    assert files_for_upload[0].favor_local is None
+    assert files_for_upload[0].from_local is False
+    assert files_for_upload[0].from_google is False
+    assert files_for_upload[0].path is None
+    assert files_for_upload[0].size is None
+    assert files_for_upload[0].checksum is None
+    files_for_upload[0]._favor_local = True  # normally resolved by FileForUpload.review
+    assert files_for_upload[0].favor_local is True
+    assert files_for_upload[0].from_local is True
+    assert files_for_upload[0].from_google is False
+    assert files_for_upload[0].path == os.path.join(filesystem.root, file_one)
+    assert files_for_upload[0].size == filesize
+    assert len(files_for_upload[0].checksum) > 0
+    files_for_upload[0]._favor_local = False  # normally resolved by FileForUpload.review
+    assert files_for_upload[0].favor_local is False
+    assert files_for_upload[0].from_local is False
+    assert files_for_upload[0].from_google is True
+    assert files_for_upload[0].path == cloud_path.join(rclone_google.bucket, files_for_upload[0].name)
+    assert files_for_upload[0].size == filesize
+    assert len(files_for_upload[0].checksum) > 0
+
+    env_amazon = EnvAmazon()
+    s3_key = f"test-{create_short_uuid(31)}/SMAFIPIGC8NG.fastq"
+    s3_uri = f"s3://{env_amazon.bucket}/{s3_key}"
+    credentials_amazon = env_amazon.temporary_credentials(env_amazon.bucket, s3_key)
+    # FYI the output of this looks something like this (but not specifically checking for now):
+    # ▶ Upload: test_file_one.fastq (1.21 KB) ...
+    #   - From: gs://smaht-submitr-rclone-testing/test_file_one.fastq
+    #   -   To: s3://smaht-unit-testing-files/test-9eFJ8iZHG5ayrTEuSvz7G4upKVJdtpJ/SMAFIPIGC8NG.fastq
+    # ▶ Upload progress ✓ 100% ◀|###########| 1234/1235 | 1.16 MB/s | 00:00 | ETA: 00:00
+    # ▶ Upload progress ✓ 100% ◀|###########| 1235/1235 | 3.53 KB/s | 00:00 | ETA: 00:00
+    # Verifying upload: test_file_one.fastq ... OK
+    upload_file_to_aws_s3(file=files_for_upload[0],
+                          s3_uri=s3_uri,
+                          aws_credentials=credentials_amazon.to_dictionary())
+    assert env_amazon.s3_non_rclone().file_exists(env_amazon.bucket, s3_key) is True
+    assert env_amazon.s3_non_rclone().file_size(env_amazon.bucket, s3_key) == filesize
+    assert (env_amazon.s3_non_rclone().file_checksum(env_amazon.bucket, s3_key) ==
+            compute_file_md5(os.path.join(filesystem.root, file_one)))
+    s3_key_metadata = get_s3_key_metadata(credentials_amazon.to_dictionary(environment_names=False),
+                                          env_amazon.bucket, s3_key)
+    assert isinstance(s3_key_metadata, dict)
+    assert s3_key_metadata["size"] == filesize
+    assert s3_key_metadata["size"] == filesize
+    assert s3_key_metadata["md5"] == compute_file_md5(os.path.join(filesystem.root, file_one))
+    assert s3_key_metadata["md5_source"] == "google-cloud-storage"
+    assert env_amazon.s3_non_rclone().delete_file(env_amazon.bucket, s3_key)
+    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, files_for_upload[0].name)
+
+
+def test_rclone_local_to_google_copy_to_bucket() -> None:
+    # Just an aside (ran across while testing); make sure copyto=False works for sub-folder.
+    filesize = 1234
+    env_google = EnvGoogle(use_cloud_subfolder_key=True)
+    filesystem = Mock_LocalStorage()
+    filesystem.create_files(file_one := "subdir/test_file_one.fastq", nbytes=filesize)
+    # Bucket is really "bucket" - bucket plus optional sub-folder, which RCloneConfig is designed to handle.
+    subfolder = f"test-{create_short_uuid(31)}"
+    bucket_google = cloud_path.join(env_google.bucket, subfolder)
+    credentials_google = env_google.credentials()
+    rclone_google = RCloneGoogle(credentials_google, bucket=bucket_google)
+    rcloner = RCloner(destination=rclone_google)
+    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
+    assert env_google.gcs_non_rclone().file_exists(cloud_path.join(bucket_google, os.path.basename(file_one))) is True
+    assert env_google.gcs_non_rclone().file_exists(bucket_google, os.path.basename(file_one)) is True
+    assert env_google.gcs_non_rclone().file_size(cloud_path.join(bucket_google, os.path.basename(file_one))) == filesize
+    assert env_google.gcs_non_rclone().file_size(bucket_google, os.path.basename(file_one)) == filesize
+    assert (env_google.gcs_non_rclone().file_checksum(cloud_path.join(bucket_google, os.path.basename(file_one))) ==
+            compute_file_md5(os.path.join(filesystem.root, file_one)))
+    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, os.path.basename(file_one))
+
+
+def test_rclone_local_to_amazon_copy_to_bucket() -> None:
+    # Just an aside (ran across while testing); make sure copyto=False works for sub-folder.
+    filesize = 1236
+    env_amazon = EnvAmazon(use_cloud_subfolder_key=True)
+    filesystem = Mock_LocalStorage()
+    filesystem.create_files(file_one := "subdir/test_file_one.fastq", nbytes=filesize)
+    # Bucket is really "bucket" - bucket plus optional sub-folder, which RCloneConfig is designed to handle.
+    subfolder = f"test-{create_short_uuid(31)}"
+    bucket_amazon = cloud_path.join(env_amazon.bucket, subfolder)
+    credentials_amazon = env_amazon.credentials()
+    rclone_amazon = RCloneAmazon(credentials_amazon, bucket=bucket_amazon)
+    rcloner = RCloner(destination=rclone_amazon)
+    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
+    assert env_amazon.s3_non_rclone().file_exists(cloud_path.join(bucket_amazon, os.path.basename(file_one))) is True
+    assert env_amazon.s3_non_rclone().file_exists(bucket_amazon, os.path.basename(file_one)) is True
+    assert env_amazon.s3_non_rclone().file_size(cloud_path.join(bucket_amazon, os.path.basename(file_one))) == filesize
+    assert env_amazon.s3_non_rclone().file_size(bucket_amazon, os.path.basename(file_one)) == filesize
+    assert (env_amazon.s3_non_rclone().file_checksum(cloud_path.join(bucket_amazon, os.path.basename(file_one))) ==
+            compute_file_md5(os.path.join(filesystem.root, file_one)))
+    assert env_amazon.s3_non_rclone().delete_file(bucket_amazon, os.path.basename(file_one))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_resume_uploads.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,10 +226,10 @@
                                         joined_filename = os.path.join(current_dir, SAMPLE_UPLOAD_INFO[-1]['filename'])
                                         # Make sure this is doing what we expect.
                                         assert current_dir + "/" in joined_filename
                                         # Make sure the inner upload actually uploads to the current dir.
                                         mock_upload_file_to_uuid.assert_called_with(auth=fake_keydict,
                                                                                     filename=joined_filename,
                                                                                     uuid=SAMPLE_UPLOAD_INFO[-1]['uuid'],
-                                                                                    rclone_config_google=None,
+                                                                                    rclone_google=None,
                                                                                     first_time=False, portal=mock.ANY)
                                         assert output == []
```

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_submission.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/test_utils.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.2.1b5/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b4/submitr/utils.py` & `smaht_submitr-0.8.2.1b5/submitr/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from datetime import datetime
 from functools import lru_cache
 import io
 from json import dumps as json_dumps, loads as json_loads
 import os
 from pathlib import Path
 import pkg_resources
-import re
 import requests
 from signal import signal, SIGINT
 import string
 from typing import Any, Callable, List, Optional, Tuple
 from dcicutils.datetime_utils import format_datetime, parse_datetime
 from dcicutils.function_cache_decorator import function_cache
 from dcicutils.misc_utils import PRINT, str_to_bool
@@ -85,20 +84,14 @@
         return json_loads(self.content)
 
     def raise_for_status(self):
         if self.status_code >= 300:
             raise Exception(f"{self} raised for status.")
 
 
-def get_s3_bucket_and_key_from_s3_uri(uri: str) -> Tuple[str, str]:
-    if match := re.match(r"s3://([^/]+)/(.+)", uri):
-        return (match.group(1), match.group(2))
-    return None, None
-
-
 def tobool(value: Any, fallback: bool = False) -> bool:
     if isinstance(value, bool):
         return value
     elif isinstance(value, str):
         try:
             return str_to_bool(value)
         except Exception:
@@ -221,7 +214,16 @@
     finally:
         signal(SIGINT, previous_interrupt_handler)
 
 
 @function_cache(serialize_key=True)
 def get_health_page(key: dict) -> dict:
     return Portal(key).get_health().json()
+
+
+def DEBUGGING():
+    return isinstance(debug := os.environ.get("SMAHT_DEBUG"), str) and (debug.lower() == "true" or debug == "1")
+
+
+def DEBUG(*args, **kwargs):
+    if DEBUGGING():
+        PRINT(*args, **kwargs)
```

### Comparing `smaht_submitr-0.8.2.1b4/PKG-INFO` & `smaht_submitr-0.8.2.1b5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.2.1b4
+Version: 0.8.2.1b5
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.13
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: awscli (>=1.32.105)
 Requires-Dist: boto3 (>=1.34.105,<2.0.0)
-Requires-Dist: dcicutils (>=8.8.4.1b32,<9.0.0.0)
+Requires-Dist: dcicutils (>=8.8.4.1b33,<9.0.0.0)
 Requires-Dist: googleapi (>=0.1.0,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/smaht-dac/submitr.git
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://staging.smaht.org/static/img/docs/submitr_logo.png
```

