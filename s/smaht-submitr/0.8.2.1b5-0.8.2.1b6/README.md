# Comparing `tmp/smaht_submitr-0.8.2.1b5.tar.gz` & `tmp/smaht_submitr-0.8.2.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.2.1b5.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.2.1b6.tar", max compression
```

## Comparing `smaht_submitr-0.8.2.1b5.tar` & `smaht_submitr-0.8.2.1b6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1098 2024-05-17 19:13:29.160236 smaht_submitr-0.8.2.1b5/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-05-17 19:13:29.160236 smaht_submitr-0.8.2.1b5/README.rst
--rw-r--r--   0        0        0     3466 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/base.py
--rw-r--r--   0        0        0      294 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/exceptions.py
--rw-r--r--   0        0        0    17885 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/file_for_upload.py
--rw-r--r--   0        0        0    11097 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/metadata_template.py
--rw-r--r--   0        0        0     2628 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/output.py
--rw-r--r--   0        0        0      353 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/__init__.py
--rw-r--r--   0        0        0     6343 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_amazon.py
--rw-r--r--   0        0        0     9291 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_commands.py
--rw-r--r--   0        0        0     6986 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_config.py
--rw-r--r--   0        0        0     9523 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_google.py
--rw-r--r--   0        0        0     5152 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_installation.py
--rw-r--r--   0        0        0     3187 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_utils.py
--rw-r--r--   0        0        0    11817 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/rcloner.py
--rw-r--r--   0        0        0    19885 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
--rw-r--r--   0        0        0     8157 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_google.py
--rw-r--r--   0        0        0    17135 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/s3_upload.py
--rw-r--r--   0        0        0     3512 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4779 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     9895 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     2824 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/get_metadata_template.py
--rw-r--r--   0        0        0     1822 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5107 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/rcloner.py
--rw-r--r--   0        0        0     6455 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    21430 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-05-17 19:13:29.200235 smaht_submitr-0.8.2.1b5/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   127795 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/submission.py
--rw-r--r--   0        0        0    14817 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/submission_uploads.py
--rw-r--r--   0        0        0        0 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0    12067 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_file_for_upload.py
--rw-r--r--   0        0        0     1620 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    43766 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_rclone_support.py
--rw-r--r--   0        0        0    11766 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0    37993 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     4353 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0     3863 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/tests/testing_rclone_helpers.py
--rw-r--r--   0        0        0     8677 2024-05-17 19:13:29.204235 smaht_submitr-0.8.2.1b5/submitr/utils.py
--rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-17 20:16:01.931087 smaht_submitr-0.8.2.1b6/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-05-17 20:16:01.931087 smaht_submitr-0.8.2.1b6/README.rst
+-rw-r--r--   0        0        0     3466 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/exceptions.py
+-rw-r--r--   0        0        0    17885 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/file_for_upload.py
+-rw-r--r--   0        0        0    11097 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/metadata_template.py
+-rw-r--r--   0        0        0     2628 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/output.py
+-rw-r--r--   0        0        0      353 2024-05-17 20:16:01.967087 smaht_submitr-0.8.2.1b6/submitr/rclone/__init__.py
+-rw-r--r--   0        0        0     6343 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_amazon.py
+-rw-r--r--   0        0        0     9291 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_commands.py
+-rw-r--r--   0        0        0     6986 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_config.py
+-rw-r--r--   0        0        0     9916 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_google.py
+-rw-r--r--   0        0        0     5152 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_installation.py
+-rw-r--r--   0        0        0     3187 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_utils.py
+-rw-r--r--   0        0        0    11817 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/rcloner.py
+-rw-r--r--   0        0        0    19885 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
+-rw-r--r--   0        0        0     8157 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/rclone/testing/rclone_utils_for_testing_google.py
+-rw-r--r--   0        0        0    17135 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/s3_upload.py
+-rw-r--r--   0        0        0     3512 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4779 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9895 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     2824 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/get_metadata_template.py
+-rw-r--r--   0        0        0     1822 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5483 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/rcloner.py
+-rw-r--r--   0        0        0     7143 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    21810 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   127795 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/submission.py
+-rw-r--r--   0        0        0    14817 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/submission_uploads.py
+-rw-r--r--   0        0        0        0 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0    12067 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_file_for_upload.py
+-rw-r--r--   0        0        0     1620 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    43766 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_rclone_support.py
+-rw-r--r--   0        0        0    11766 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0    37993 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     4353 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0     3863 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/tests/testing_rclone_helpers.py
+-rw-r--r--   0        0        0     8677 2024-05-17 20:16:01.971087 smaht_submitr-0.8.2.1b6/submitr/utils.py
+-rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b6/PKG-INFO
```

### Comparing `smaht_submitr-0.8.2.1b5/LICENSE.txt` & `smaht_submitr-0.8.2.1b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/README.rst` & `smaht_submitr-0.8.2.1b6/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/pyproject.toml` & `smaht_submitr-0.8.2.1b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.2.1b5"  # TODO: To become 0.8.3
+version = "0.8.2.1b6"  # TODO: To become 0.8.3
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.8.2.1b5/submitr/base.py` & `smaht_submitr-0.8.2.1b6/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/file_for_upload.py` & `smaht_submitr-0.8.2.1b6/submitr/file_for_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/metadata_template.py` & `smaht_submitr-0.8.2.1b6/submitr/metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/output.py` & `smaht_submitr-0.8.2.1b6/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_amazon.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_amazon.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_commands.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_commands.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_config.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_config.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_google.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_google.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,36 @@
         except Exception:
             pass
         # If no service account file specified then maybe we are on a GCE instance.
         if project := RCloneGoogle._get_project_name_if_google_compute_engine():
             self._project = project
             return self._project
 
+    def verify_connectivity(self, printf: Optional[Callable] = None) -> bool:
+        if not callable(printf):
+            printf = print
+        if self.ping():
+            printf(f"Google Cloud Storage project"
+                   f"{f' ({self.project})' if self.project else ''}"
+                   f" connectivity appears to be OK ✓")
+            if self.bucket_exists() is False:
+                printf(f"WARNING: Google Cloud Storage bucket NOT FOUND: {self.bucket}")
+            return False
+        else:
+            printf(f"Google Cloud Storage project"
+                   f"{f' ({self.project})' if self.project else ''}"
+                   f" connectivity appears to be problematic ✗")
+            return True
+
+    def __eq__(self, other: Optional[RCloneGoogle]) -> bool:
+        return isinstance(other, RCloneGoogle) and super().__eq__(other)
+
+    def __ne__(self, other: Optional[RCloneGoogle]) -> bool:
+        return not self.__eq__(other)
+
     @staticmethod
     def is_google_compute_engine() -> Optional[str]:
         return RCloneGoogle._get_project_name_if_google_compute_engine() is not None
 
     @staticmethod
     def _get_project_name_if_google_compute_engine() -> Optional[str]:
         """
@@ -114,55 +136,39 @@
         except Exception:
             pass
         return None
 
     @staticmethod
     def from_command_args(rclone_google_source: Optional[str],
                           rclone_google_credentials: Optional[str] = None,
+                          rclone_google_location: Optional[str] = None,
                           verify_installation: bool = True,
                           printf: Optional[Callable] = None) -> Optional[RCloneGoogle]:
         """
         Assumed to be called at the start of command-line utility (i.e. e.g. submit-metadata-bundle).
+        The rclone_google_source should be the Google bucket (or bucket/sub-folder is also allowed),
+        where the files to be copied can be found. The rclone_google_credentials should be the full path
+        to the Google (GCP) service account file; or this can be omitted if running on a GCE instance.
+        The rclone_google_location is the location (aka region) to be used for the copy.
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
         if rclone_google_credentials and not os.path.isfile(rclone_google_credentials):
             printf(f"ERROR: Google service account file does not exist: {rclone_google_credentials}")
             exit(1)
-        # TODO: Allow "location" to be passed in (?); not in service account file.
-        return RCloneGoogle(service_account_file=rclone_google_credentials, bucket=rclone_google_source)
-
-    def verify_connectivity(self, printf: Optional[Callable] = None) -> bool:
-        if not callable(printf):
-            printf = print
-        if self.ping():
-            printf(f"Google Cloud Storage project"
-                   f"{f' ({self.project})' if self.project else ''}"
-                   f" connectivity appears to be OK ✓")
-            if self.bucket_exists() is False:
-                printf(f"WARNING: Google Cloud Storage bucket NOT FOUND: {self.bucket}")
-            return False
-        else:
-            printf(f"Google Cloud Storage project"
-                   f"{f' ({self.project})' if self.project else ''}"
-                   f" connectivity appears to be problematic ✗")
-            return True
-
-    def __eq__(self, other: Optional[RCloneGoogle]) -> bool:
-        return isinstance(other, RCloneGoogle) and super().__eq__(other)
-
-    def __ne__(self, other: Optional[RCloneGoogle]) -> bool:
-        return not self.__eq__(other)
+        return RCloneGoogle(service_account_file=rclone_google_credentials,
+                            location=rclone_google_location,
+                            bucket=rclone_google_source)
 
 
 class GoogleCredentials(RCloneCredentials):
 
     def __init__(self,
                  credentials: Optional[GoogleCredentials] = None,
                  service_account_file: Optional[str] = None,
@@ -171,15 +177,14 @@
         if isinstance(credentials, GoogleCredentials):
             self._location = credentials.location
             self._service_account_file = credentials.service_account_file
         else:
             self._location = None
             self._service_account_file = None
 
-        # TODO: maybe exception if no service-account-file AND not running on GCE.
         if service_account_file := normalize_path(service_account_file, expand_home=True):
             if not os.path.isfile(service_account_file):
                 raise Exception(f"GoogleCredentials service account file not found: {service_account_file}")
             self._service_account_file = service_account_file
 
         if location := normalize_string(location):
             self._location = location
```

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_installation.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_installation.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rclone_utils.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rclone_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/rcloner.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/rcloner.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_amazon.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/testing/rclone_utils_for_testing_amazon.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/rclone/testing/rclone_utils_for_testing_google.py` & `smaht_submitr-0.8.2.1b6/submitr/rclone/testing/rclone_utils_for_testing_google.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/s3_upload.py` & `smaht_submitr-0.8.2.1b6/submitr/s3_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/s3_utils.py` & `smaht_submitr-0.8.2.1b6/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/get_metadata_template.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/get_metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/rcloner.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/rcloner.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,37 +46,45 @@
         if not credentials_amazon:
             usage("No AWS credentials specified or found (in environment).")
         source_config = RCloneAmazon(credentials_amazon)
     elif args.source.lower().startswith("gs://"):
         source = args.source[5:]
         if not credentials_google:
             if not RCloneGoogle.is_google_compute_engine():
+                # No Google credentials AND NOT running on a GCE instance.
                 usage("No GCP credentials specified.")
-            elif args.verbose:
-                google_project = RCloneGoogle._get_project_name_if_google_compute_engine()
-                print(f"Running from Google Cloud Engine{f': {google_project} ✓' if google_project else '.'}")
-        source_config = RCloneGoogle(credentials_google)
+            # OK to create RCloneGoogle with no credentials on a GCE instance.
+            source_config = RCloneGoogle()
+            if args.verbose:
+                google_project = source_config.project
+                print(f"Running from Google Cloud Engine (GCE){f': {google_project} ✓' if google_project else '.'}")
+        else:
+            source_config = RCloneGoogle(credentials_google)
     else:
         source = args.source
         source_config = None
 
     if args.destination.lower().startswith("s3://"):
         destination = args.destination[5:]
         if not credentials_amazon:
             usage("No AWS credentials specified or found (in environment).")
         destination_config = RCloneAmazon(credentials_amazon)
     elif args.destination.lower().startswith("gs://"):
         destination = args.destination[5:]
         if not credentials_google:
             if not RCloneGoogle.is_google_compute_engine():
+                # No Google credentials AND NOT running on a GCE instance.
                 usage("No GCP credentials specified.")
-            elif args.verbose:
-                google_project = RCloneGoogle._get_project_name_if_google_compute_engine()
-                print(f"Running from Google Cloud Engine{f': {google_project} ✓' if google_project else '.'}")
-        destination_config = RCloneGoogle(credentials_google)
+            # OK to create RCloneGoogle with no credentials on a GCE instance.
+            destination_config = RCloneGoogle()
+            if args.verbose:
+                google_project = destination_config.project
+                print(f"Running from Google Cloud Engine (GCE){f': {google_project} ✓' if google_project else '.'}")
+        else:
+            destination_config = RCloneGoogle(credentials_google)
     else:
         destination = args.destination
         destination_config = None
 
     rcloner = RCloner(source=source_config, destination=destination_config)
     result, output = rcloner.copy(source, destination, return_output=True)
     if result is True:
```

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/resume_uploads.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,23 @@
   To specifiy the path to your metatdata file;
   only the directory of this is used to locate your upload files.
 --directory DIRECTORY
   To specify a directory containing the files to upload;
   this directory will be search, recursively.
 --directory-only
   Same as --directory but does NOT search recursively.
+--rclone-google-source GOOGLE-CLOUD-STORAGE-SOURCE
+  A Google Cloud Storage (GCS) bucket or bucket/sub-folder
+  from where the upload file(s) should be copied.
+--rclone-google-credentials GCS-SERVICE-ACCOUNT-FILE
+  GCS credentials to use for --rclone-google-source;
+  e.g. full path to your GCP service account file.
+  May be omitted if running on a GCE instance.
+--rclone-google-location LOCATION
+  The Google Cloud Storage (GCS) location (aka "region").
 --help
   Prints this documentation.
 --help-advanced
   Prints this plus more advanced documentation.
 --help-web
   Opens your browser to the Web based documentation.
   {CustomArgumentParser.HELP_URL}
@@ -75,14 +84,15 @@
     parser.add_argument('--bundle', help="location of the original Excel submission file")
     parser.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
     parser.add_argument('--directory', help="Directory of the upload files.")
     parser.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
     parser.add_argument('--upload_folder', help="Synonym for --directory.")
     parser.add_argument('--rclone-google-source', help="Use rlcone to copy upload files from GCS.", default=None)
     parser.add_argument('--rclone-google-credentials', help="GCS credentials (service account file).", default=None)
+    parser.add_argument('--rclone-google-location', help="GCS location (aka region).", default=None)
     parser.add_argument('--output', help="Output file for results.", default=False)
     parser.add_argument('--verbose', action="store_true", default=False)
     parser.add_argument('--yes', action="store_true",
                         help="Suppress (yes/no) requests for user input.", default=False)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
@@ -121,15 +131,17 @@
     if not args.upload_folder and args.directory:
         args.upload_folder = args.directory
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Specified upload directory not found: {args.upload_folder}")
         exit(1)
 
-    config_google = RCloneGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
+    config_google = RCloneGoogle.from_command_args(args.rclone_google_source,
+                                                   args.rclone_google_credentials,
+                                                   args.rclone_google_location)
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
         if args.env:
             env_from_env = True
```

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/submit_metadata_bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,22 @@
   To specify your submission center.
   Default is to use the submission center associated with your account.
 --directory DIRECTORY
   To specify a directory containing the files to upload; in addition
   to the default of using the directory containing the submitted file;
   this directory will be searched recursively.
 --rclone-google-source GOOGLE-CLOUD-STORAGE-SOURCE
-  A Google Cloud Storage (GCS) bucket or bucket/key (foldrer)
-  from where the upload file(s) should be read.
+  A Google Cloud Storage (GCS) bucket or bucket/sub-folder
+  from where the upload file(s) should be copied.
 --rclone-google-credentials GCS-SERVICE-ACCOUNT-FILE
   GCS credentials to use for --rclone-google-source;
-  e.g. a path to a service account file.
+  e.g. full path to your GCP service account file.
+  May be omitted if running on a GCE instance.
+--rclone-google-location LOCATION
+  The Google Cloud Storage (GCS) location (aka "region").
 --output OUTPUT-FILE
   Writes all logging output to the specified file;
   and refrains from printing lengthy content to output/stdout.
 --info
   Displays ONLY info about the specified metadata file; nothing else.
   Add --refs or --files to see (linkTo) references or (upload) files.
 --verbose
@@ -223,14 +226,15 @@
     parser.add_argument('--verbose', action="store_true", help="Debug output.", default=False)
     parser.add_argument('--timeout', help="Wait timeout for server validation/submission.")
     parser.add_argument('--debug', action="store_true", help="Debug output.", default=False)
     parser.add_argument('--debug-sleep', help="Sleep on each row read for troubleshooting/testing.", default=False)
     parser.add_argument('--ping', action="store_true", help="Ping server.", default=False)
     parser.add_argument('--rclone-google-source', help="Use rlcone to copy upload files from GCS.", default=None)
     parser.add_argument('--rclone-google-credentials', help="GCS credentials (service account file).", default=None)
+    parser.add_argument('--rclone-google-location', help="GCS location (aka region).", default=None)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
     if args.directory:
         if args.directory_only:
             PRINT("May not specify both --directory and --directory-only")
             exit(1)
@@ -242,15 +246,17 @@
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
         if args.env:
             env_from_env = True
 
-    config_google = RCloneGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
+    config_google = RCloneGoogle.from_command_args(args.rclone_google_source,
+                                                   args.rclone_google_credentials,
+                                                   args.rclone_google_location)
 
     if args.ping or (args.bundle_filename and args.bundle_filename.lower() == "ping"):
         if args.env or os.environ.get("SMAHT_ENV"):
             ping_okay = _ping(env=args.env or os.environ.get("SMAHT_ENV"), env_from_env=env_from_env,
                               server=args.server, app=args.app, keys_file=args.keys, verbose=True)
             if ping_okay:
                 PRINT("Portal connectivity appears to be OK ✓")
```

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.2.1b6/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/submission.py` & `smaht_submitr-0.8.2.1b6/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/submission_uploads.py` & `smaht_submitr-0.8.2.1b6/submitr/submission_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.2.1b6/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_base.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_file_for_upload.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_file_for_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_misc.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_rclone_support.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_rclone_support.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_submission.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/test_utils.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/tests/testing_rclone_helpers.py` & `smaht_submitr-0.8.2.1b6/submitr/tests/testing_rclone_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/submitr/utils.py` & `smaht_submitr-0.8.2.1b6/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b5/PKG-INFO` & `smaht_submitr-0.8.2.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.2.1b5
+Version: 0.8.2.1b6
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.13
```

