# Comparing `tmp/osl-0.5.1.tar.gz` & `tmp/osl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osl-0.5.1.tar", last modified: Tue Sep 12 16:29:49 2023, max compression
+gzip compressed data, was "osl-0.6.0.tar", last modified: Fri Apr 12 15:17:52 2024, max compression
```

## Comparing `osl-0.5.1.tar` & `osl-0.6.0.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:49.498103 osl-0.5.1/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     1527 2022-11-17 15:59:38.000000 osl-0.5.1/LICENSE
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2049 2023-09-12 16:29:49.498103 osl-0.5.1/PKG-INFO
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     1251 2023-04-04 10:35:47.000000 osl-0.5.1/README.md
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.315102 osl-0.5.1/osl/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     1534 2023-09-12 16:25:18.000000 osl-0.5.1/osl/__init__.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.354102 osl-0.5.1/osl/glm/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)       55 2023-04-04 10:35:47.000000 osl-0.5.1/osl/glm/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     8088 2023-09-12 15:50:15.000000 osl-0.5.1/osl/glm/glm_base.py
--rw-r--r--   0 mvanes   (2914928) mwoolrichgrp (80002)     6577 2023-04-23 16:44:08.000000 osl-0.5.1/osl/glm/glm_epochs.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    32952 2023-09-12 15:50:15.000000 osl-0.5.1/osl/glm/glm_spectrum.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.364102 osl-0.5.1/osl/maxfilter/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      169 2022-09-07 09:21:47.000000 osl-0.5.1/osl/maxfilter/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    23018 2023-07-10 09:03:38.000000 osl-0.5.1/osl/maxfilter/maxfilter.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.386102 osl-0.5.1/osl/preprocessing/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      199 2022-11-18 13:14:30.000000 osl-0.5.1/osl/preprocessing/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    31416 2023-09-12 15:49:42.000000 osl-0.5.1/osl/preprocessing/batch.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    13843 2023-03-21 20:18:41.000000 osl-0.5.1/osl/preprocessing/mne_wrappers.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    13945 2023-07-10 09:03:38.000000 osl-0.5.1/osl/preprocessing/osl_wrappers.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    54662 2022-12-12 14:16:31.000000 osl-0.5.1/osl/preprocessing/plot_ica.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.413102 osl-0.5.1/osl/report/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      148 2022-11-18 13:14:30.000000 osl-0.5.1/osl/report/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     4049 2022-09-13 06:42:34.000000 osl-0.5.1/osl/report/phantom-report.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2541 2022-09-13 06:42:34.000000 osl-0.5.1/osl/report/phantom-trigger.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    42782 2023-09-12 15:49:42.000000 osl-0.5.1/osl/report/raw_report.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    13885 2023-09-12 15:49:42.000000 osl-0.5.1/osl/report/src_report.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.438102 osl-0.5.1/osl/report/templates/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     6601 2022-11-17 15:59:38.000000 osl-0.5.1/osl/report/templates/raw_subject_panel.html
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2174 2023-02-01 16:17:13.000000 osl-0.5.1/osl/report/templates/raw_summary_panel.html
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     5259 2023-09-12 15:49:42.000000 osl-0.5.1/osl/report/templates/src_subject_panel.html
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     3054 2023-02-14 13:03:16.000000 osl-0.5.1/osl/report/templates/src_summary_panel.html
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     4362 2022-11-17 15:59:38.000000 osl-0.5.1/osl/report/templates/subject_report.html
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2354 2022-11-17 15:59:38.000000 osl-0.5.1/osl/report/templates/summary_report.html
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.458102 osl-0.5.1/osl/source_recon/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      164 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     9650 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/batch.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    43926 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/beamforming.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.470102 osl-0.5.1/osl/source_recon/parcellation/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      138 2023-02-01 16:17:13.000000 osl-0.5.1/osl/source_recon/parcellation/__init__.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.976103 osl-0.5.1/osl/source_recon/parcellation/files/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    41373 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     9131 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    56930 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)   471175 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    45441 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d_ds8.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)   128653 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/HarvardOxford-sub-prob-bin-2mm.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)   414185 2023-02-01 16:17:13.000000 osl-0.5.1/osl/source_recon/parcellation/files/MNI152_T1_2mm_brain.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)     7241 2023-02-01 16:17:13.000000 osl-0.5.1/osl/source_recon/parcellation/files/MNI152_T1_8mm_brain.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    52328 2023-03-21 20:18:41.000000 osl-0.5.1/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)   417837 2023-02-01 16:17:13.000000 osl-0.5.1/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    42262 2023-02-01 16:17:13.000000 osl-0.5.1/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d_ds8.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)    37951 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds2mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)     1609 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds8mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)     6546 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/dk_cortical.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)     7695 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/dk_full.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)  2477647 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/fMRI_parcellation_ds2mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)    23705 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/fMRI_parcellation_ds8mm.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)  1165004 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)    23705 2022-09-13 06:46:47.000000 osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)  1651912 2022-09-13 06:46:48.000000 osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_2mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)    63185 2022-09-13 06:46:48.000000 osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)    63835 2022-09-13 06:46:48.000000 osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
--rwxrwxrwx   0 mvanes   (2914928) mwoolrichgrp (80002)     5233 2022-09-13 06:46:48.000000 osl-0.5.1/osl/source_recon/parcellation/files/giles_39_binary.nii.gz
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     5141 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/parcellation/nii.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    34882 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/parcellation/parcellation.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:49.014103 osl-0.5.1/osl/source_recon/rhino/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      330 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/rhino/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    49196 2023-09-12 15:49:42.000000 osl-0.5.1/osl/source_recon/rhino/coreg.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    11583 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/rhino/forward_model.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2433 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/rhino/fsl_utils.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     7133 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/rhino/polhemus.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    25915 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/rhino/surfaces.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    45871 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/rhino/utils.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    12297 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/sign_flipping.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    33543 2023-09-12 15:49:43.000000 osl-0.5.1/osl/source_recon/wrappers.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:49.042103 osl-0.5.1/osl/tests/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2022-09-07 09:21:48.000000 osl-0.5.1/osl/tests/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2727 2023-02-01 16:17:13.000000 osl-0.5.1/osl/tests/test_00_package_canary.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2445 2022-09-07 09:21:48.000000 osl-0.5.1/osl/tests/test_batch_api.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     3467 2022-10-03 10:17:09.000000 osl-0.5.1/osl/tests/test_batch_preproc.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     7523 2022-09-07 09:21:48.000000 osl-0.5.1/osl/tests/test_file_handling.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2659 2022-09-07 09:21:48.000000 osl-0.5.1/osl/tests/test_parallel.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:49.081103 osl-0.5.1/osl/utils/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      461 2022-12-12 14:16:31.000000 osl-0.5.1/osl/utils/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     9465 2022-09-30 13:14:45.000000 osl-0.5.1/osl/utils/create_neuromag306_info.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     7295 2022-11-18 13:14:30.000000 osl-0.5.1/osl/utils/file_handling.py
--rw-r--r--   0 mvanes   (2914928) mwoolrichgrp (80002)     3857 2023-04-23 16:44:08.000000 osl-0.5.1/osl/utils/logger.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    15519 2022-09-30 13:14:45.000000 osl-0.5.1/osl/utils/neuromag306_info.yml
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    11992 2022-12-12 14:16:31.000000 osl-0.5.1/osl/utils/opm.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     1435 2022-12-12 14:16:31.000000 osl-0.5.1/osl/utils/package.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     1865 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/parallel.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     5521 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulate.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:49.476103 osl-0.5.1/osl/utils/simulation_config/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)  6240010 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/megin_template_info.fif
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)   400128 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/reduced_mvar_params_grad.npy
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)   400128 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/reduced_mvar_params_mag.npy
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    81728 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/reduced_mvar_pcacomp_grad.npy
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    40928 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/reduced_mvar_pcacomp_mag.npy
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    20128 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/reduced_mvar_residcov_grad.npy
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)    20128 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/simulation_config/reduced_mvar_residcov_mag.npy
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:49.495103 osl-0.5.1/osl/utils/spmio/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)       29 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/spmio/__init__.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     4151 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/spmio/_data.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     4219 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/spmio/_events.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      419 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/spmio/_spmmeeg_utils.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     8834 2022-09-07 09:21:48.000000 osl-0.5.1/osl/utils/spmio/spmmeeg.py
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     1627 2023-07-10 09:03:38.000000 osl-0.5.1/osl/utils/study.py
-drwxrwsrwx   0 mvanes   (2914928) mwoolrichgrp (80002)        0 2023-09-12 16:29:48.341102 osl-0.5.1/osl.egg-info/
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     2049 2023-09-12 16:29:48.000000 osl-0.5.1/osl.egg-info/PKG-INFO
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     4241 2023-09-12 16:29:48.000000 osl-0.5.1/osl.egg-info/SOURCES.txt
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)        1 2023-09-12 16:29:48.000000 osl-0.5.1/osl.egg-info/dependency_links.txt
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      106 2023-09-12 16:29:48.000000 osl-0.5.1/osl.egg-info/entry_points.txt
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)        1 2022-09-07 09:23:35.000000 osl-0.5.1/osl.egg-info/not-zip-safe
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      412 2023-09-12 16:29:48.000000 osl-0.5.1/osl.egg-info/requires.txt
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)        4 2023-09-12 16:29:48.000000 osl-0.5.1/osl.egg-info/top_level.txt
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)      163 2023-09-12 16:29:49.501103 osl-0.5.1/setup.cfg
--rw-rw-rw-   0 mvanes   (2914928) mwoolrichgrp (80002)     3104 2023-09-12 16:25:28.000000 osl-0.5.1/setup.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.615092 osl-0.6.0/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1527 2023-09-21 07:51:38.000000 osl-0.6.0/LICENSE
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     3254 2024-04-12 15:17:52.615092 osl-0.6.0/PKG-INFO
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1192 2024-04-02 13:22:06.000000 osl-0.6.0/README.md
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.594092 osl-0.6.0/osl/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1534 2024-04-12 15:15:15.000000 osl-0.6.0/osl/__init__.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.595092 osl-0.6.0/osl/glm/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      153 2024-02-05 15:29:07.000000 osl-0.6.0/osl/glm/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    12188 2024-03-13 15:48:39.000000 osl-0.6.0/osl/glm/glm_base.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    10598 2024-02-05 15:29:07.000000 osl-0.6.0/osl/glm/glm_epochs.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    45100 2024-03-13 15:48:39.000000 osl-0.6.0/osl/glm/glm_spectrum.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.595092 osl-0.6.0/osl/maxfilter/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      268 2024-02-05 15:29:07.000000 osl-0.6.0/osl/maxfilter/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    25838 2024-02-05 15:29:07.000000 osl-0.6.0/osl/maxfilter/maxfilter.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.596092 osl-0.6.0/osl/preprocessing/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      297 2024-02-05 15:29:07.000000 osl-0.6.0/osl/preprocessing/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    34673 2024-03-05 09:28:23.000000 osl-0.6.0/osl/preprocessing/batch.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    31770 2024-02-05 15:29:07.000000 osl-0.6.0/osl/preprocessing/mne_wrappers.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    26509 2024-04-03 08:43:56.000000 osl-0.6.0/osl/preprocessing/osl_wrappers.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    55481 2024-02-05 15:29:07.000000 osl-0.6.0/osl/preprocessing/plot_ica.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.596092 osl-0.6.0/osl/report/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      250 2024-02-05 15:29:07.000000 osl-0.6.0/osl/report/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    48038 2024-03-28 10:46:16.000000 osl-0.6.0/osl/report/preproc_report.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    15000 2024-03-28 10:46:16.000000 osl-0.6.0/osl/report/src_report.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.597092 osl-0.6.0/osl/report/templates/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     6758 2024-02-13 09:06:50.000000 osl-0.6.0/osl/report/templates/raw_subject_panel.html
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2301 2024-02-13 09:06:50.000000 osl-0.6.0/osl/report/templates/raw_summary_panel.html
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     5259 2023-09-21 07:51:38.000000 osl-0.6.0/osl/report/templates/src_subject_panel.html
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     3177 2024-02-13 09:06:50.000000 osl-0.6.0/osl/report/templates/src_summary_panel.html
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4362 2023-09-21 07:51:38.000000 osl-0.6.0/osl/report/templates/subject_report.html
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2354 2023-09-21 07:51:38.000000 osl-0.6.0/osl/report/templates/summary_report.html
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.597092 osl-0.6.0/osl/source_recon/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      262 2024-02-05 15:29:07.000000 osl-0.6.0/osl/source_recon/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     9675 2024-02-13 09:06:50.000000 osl-0.6.0/osl/source_recon/batch.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    51435 2024-03-13 15:48:42.000000 osl-0.6.0/osl/source_recon/beamforming.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.598092 osl-0.6.0/osl/source_recon/parcellation/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      138 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/__init__.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.605092 osl-0.6.0/osl/source_recon/parcellation/files/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    41373 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     9131 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    56930 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)   471175 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    45441 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d_ds8.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)   128653 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/HarvardOxford-sub-prob-bin-2mm.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)   414185 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/MNI152_T1_2mm_brain.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)     7241 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/MNI152_T1_8mm_brain.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    52328 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)   417837 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    42262 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d_ds8.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)    37951 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds2mm.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)     1609 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    36166 2024-02-05 15:29:07.000000 osl-0.6.0/osl/source_recon/parcellation/files/aal_cortical_merged_8mm_stacked.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)     6546 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/dk_cortical.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)     7695 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/dk_full.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)  2477647 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fMRI_parcellation_ds2mm.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)    23705 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)  1165004 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)    23705 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)  1651912 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_2mm.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)    63185 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)    63835 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
+-rwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)     5233 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/files/giles_39_binary.nii.gz
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     5141 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/parcellation/nii.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    35048 2024-03-13 15:58:12.000000 osl-0.6.0/osl/source_recon/parcellation/parcellation.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.606092 osl-0.6.0/osl/source_recon/rhino/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      330 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/rhino/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    49485 2024-03-05 09:28:23.000000 osl-0.6.0/osl/source_recon/rhino/coreg.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    11765 2024-03-05 09:28:23.000000 osl-0.6.0/osl/source_recon/rhino/forward_model.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2433 2023-09-21 07:51:38.000000 osl-0.6.0/osl/source_recon/rhino/fsl_utils.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     7862 2024-02-05 15:29:07.000000 osl-0.6.0/osl/source_recon/rhino/polhemus.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    26467 2024-02-13 09:06:50.000000 osl-0.6.0/osl/source_recon/rhino/surfaces.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    46733 2024-02-13 09:06:50.000000 osl-0.6.0/osl/source_recon/rhino/utils.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    12267 2024-02-13 09:06:50.000000 osl-0.6.0/osl/source_recon/sign_flipping.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    33826 2024-03-28 10:46:16.000000 osl-0.6.0/osl/source_recon/wrappers.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.607092 osl-0.6.0/osl/tests/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)        0 2023-09-21 07:51:38.000000 osl-0.6.0/osl/tests/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2727 2023-09-21 07:51:38.000000 osl-0.6.0/osl/tests/test_00_package_canary.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2445 2023-09-21 07:51:38.000000 osl-0.6.0/osl/tests/test_batch_api.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4144 2024-03-05 09:28:23.000000 osl-0.6.0/osl/tests/test_batch_preproc.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     7523 2023-09-21 07:51:38.000000 osl-0.6.0/osl/tests/test_file_handling.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1034 2024-03-05 09:28:23.000000 osl-0.6.0/osl/tests/test_glm.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2659 2023-09-21 07:51:38.000000 osl-0.6.0/osl/tests/test_parallel.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.608092 osl-0.6.0/osl/utils/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      663 2024-03-05 09:28:23.000000 osl-0.6.0/osl/utils/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     9465 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/create_neuromag306_info.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     7277 2024-03-05 09:28:23.000000 osl-0.6.0/osl/utils/file_handling.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4339 2024-02-05 15:29:07.000000 osl-0.6.0/osl/utils/logger.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    15519 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/neuromag306_info.yml
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    13399 2024-03-05 09:28:23.000000 osl-0.6.0/osl/utils/opm.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1435 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/package.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     2392 2024-02-05 15:29:07.000000 osl-0.6.0/osl/utils/parallel.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1021 2024-02-05 15:29:07.000000 osl-0.6.0/osl/utils/run_func.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     7469 2024-03-05 09:28:23.000000 osl-0.6.0/osl/utils/simulate.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.612092 osl-0.6.0/osl/utils/simulation_config/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)  6240010 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/megin_template_info.fif
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)   400128 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/reduced_mvar_params_grad.npy
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)   400128 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/reduced_mvar_params_mag.npy
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    81728 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/reduced_mvar_pcacomp_grad.npy
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    40928 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/reduced_mvar_pcacomp_mag.npy
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    20128 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/reduced_mvar_residcov_grad.npy
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)    20128 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/simulation_config/reduced_mvar_residcov_mag.npy
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.613092 osl-0.6.0/osl/utils/spmio/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)       29 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/spmio/__init__.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4151 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/spmio/_data.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4219 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/spmio/_events.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      419 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/spmio/_spmmeeg_utils.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     8834 2023-09-21 07:51:38.000000 osl-0.6.0/osl/utils/spmio/spmmeeg.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4654 2024-02-05 15:29:07.000000 osl-0.6.0/osl/utils/study.py
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     1839 2024-03-05 09:28:23.000000 osl-0.6.0/osl/utils/version_utils.py
+drwxr-xr-x   0 cgohil   (2331127) wingrp   (80000)        0 2024-04-12 15:17:52.613092 osl-0.6.0/osl.egg-info/
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     3254 2024-04-12 15:17:52.000000 osl-0.6.0/osl.egg-info/PKG-INFO
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     4332 2024-04-12 15:17:52.000000 osl-0.6.0/osl.egg-info/SOURCES.txt
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)        1 2024-04-12 15:17:52.000000 osl-0.6.0/osl.egg-info/dependency_links.txt
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      141 2024-04-12 15:17:52.000000 osl-0.6.0/osl.egg-info/entry_points.txt
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)        1 2023-09-21 07:54:43.000000 osl-0.6.0/osl.egg-info/not-zip-safe
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      419 2024-04-12 15:17:52.000000 osl-0.6.0/osl.egg-info/requires.txt
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)        4 2024-04-12 15:17:52.000000 osl-0.6.0/osl.egg-info/top_level.txt
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)      163 2024-04-12 15:17:52.621092 osl-0.6.0/setup.cfg
+-rw-r--r--   0 cgohil   (2331127) wingrp   (80000)     3163 2024-04-12 15:14:05.000000 osl-0.6.0/setup.py
```

### Comparing `osl-0.5.1/LICENSE` & `osl-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/__init__.py` & `osl-0.6.0/osl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 from . import glm  # noqa: F401, F403
 
 # --------------------------------------------------------
 osl_logger = logging.getLogger(__name__)
 osl_logger.debug('osl main init complete')
 
 # --------------------------------------------------------
-__version__ = '0.5.1'
+__version__ = '0.6.0'
```

### Comparing `osl-0.5.1/osl/maxfilter/maxfilter.py` & `osl-0.6.0/osl/maxfilter/maxfilter.py`

 * *Files 10% similar despite different names*

```diff
@@ -302,22 +302,51 @@
     new_origin = np.loadtxt(tmp_fit)[:3] * 1000
     print('fitted origin is {0}'.format(new_origin))
 
     return new_origin
 
 
 def run_maxfilter(infif, outfif, args, logfile_tag=''):
+    """Wrapper for Elekta Maxfilter.
+
+    Parameters
+    ----------
+        infif : str
+            Path to input fif file (raw data).
+        outfif : str
+            Path to output fif file (maxfiltered).
+        args : dict
+            Dictionary of arguments to pass to maxfilter.  See ``help(osl.maxfilter)`` for all options, and 
+            Notes for recommendations.
+        logfile_tag : str, optional
+            Tag to append to logfile name. The default is ''. This is used to
+            differentiate between different stages of maxfiltering (e.g., ``'_trans'``, ``'_tsss'``).
+
+    Returns
+    -------
+        outfif : str
+            Path to output fif file (maxfiltered).
+        stdlog : str
+            Path to logfile.
+            
+    Notes
+    -----
+    The recommended use for maxfilter at OHBA is to run multistage maxfiltering, with the following options:
+    ``args = {'maxpath': '/neuro/bin/util/maxfilter', 'scanner': 'Neo', 'mode': 'multistage', 'tsss': {}, 'headpos': {}, 'movecomp': {}}``
+    """
 
     basecmd = '{maxpath} -f {infif} -o {outfif}'
 
     # --------------
     # Format Maxfilter options
 
     if ('tsss' in args) and args['tsss']:
         outfif = outfif.replace('.fif', 'tsss.fif')
+    elif ('trans' in args) and args['trans']:
+        outfif = outfif.replace('.fif', 'trans.fif')
     elif logfile_tag != '_trans':
         outfif = outfif.replace('.fif', 'sss.fif')
 
     # Create base command
     cmd = basecmd.format(maxpath=args['maxpath'], infif=infif, outfif=outfif)
 
     cmd = _add_headpos(cmd, args, outfif)
@@ -371,21 +400,49 @@
 
     return outfif, stdlog
 
 
 # -------------------------------------------------
 
 def run_multistage_maxfilter(infif, outbase, args):
-    """
+    """Wrapper for running :py:func:`run_maxfilter <osl.maxfilter.run_maxfilter>` in three sequential steps:
+         
+    1. Find Bad Channels
+         
+    2. Signal Space Separation
+         
+    3. Translate to reference file
+    
+    Parameters
+    ----------
+        infif : str
+            Path to input fif file (raw data).
+        outbase : str
+            output directory.
+        args : dict
+            Dictionary of arguments to pass to maxfilter. See ``help(osl.maxfilter)`` for all options.
+
+    
+    Notes
+    -----
+    All files are written to disk and the output of each stage is used as the input to the next. 
+    
+    General advice (from CBU):
+    
+    * don't use ``'trans'`` with ``'movecomp'``
+    
+    * don't use ``'autobad'`` with ``'headpos'`` or ``'movecomp'``
+    
+    * don't use ``'autobad'`` with ``'st'``
+    
+    References
+    ----------
+    
     https://imaging.mrc-cbu.cam.ac.uk/meg/Maxfilter
     https://imaging.mrc-cbu.cam.ac.uk/meg/maxbugs
-
-    Camb advice - don't use trans with movecomp
-                - don't use autobad with headpos or movecomp
-                - don't use autobad with st
     """
 
     # --------------------------------------
     # Stage 1 - Find Bad Channels
 
     outfif = outbase.format('autobad_.fif')
     outlog = outbase.format('autobad.log')
@@ -439,16 +496,16 @@
     outfif, outlog = run_maxfilter(infif, outfif, stage2_args)
 
     # --------------------------------------
     # Stage 3 - Translate to reference file
     if ('trans' in args) and args['trans'] is not None:
 
         infif = outfif  # input is output from previous stage
-        outfif = outbase.format('trans.fif')
-        outlog = outbase.format('trans.log')
+        outfif = outbase.format('.fif')
+        outlog = outbase.format('.log')
 
         if os.path.exists(outfif):
             os.remove(outfif)
 
         # Fixed Args
         stage3_args = {'autobad': None, 'force': True}
         # User args
@@ -457,17 +514,49 @@
             if key in args:
                 stage3_args[key] = args[key]
 
         outfif, outlog = run_maxfilter(infif, outfif, stage3_args)
 
 
 def run_cbu_3stage_maxfilter(infif, outbase, args):
+    """Wrapper for running :py:func:`run_maxfilter <osl.maxfilter.run_maxfilter>` in three 
+    sequential steps used by MRC Cognition and Brain Sciences Unit (CBU) in Cambridge:
+         
+    0. Fit Origin without nose
+         
+    1. Find Bad Channels
+         
+    2. Signal Space Separation
+    
+    3. Translate to default
+    
+    Parameters
+    ----------
+        infif : str
+            Path to input fif file (raw data).
+        outbase : str
+            output directory.
+        args : dict
+            Dictionary of arguments to pass to maxfilter.  See ``help(osl.maxfilter)`` for all options.
+
+    
+    Notes
+    -----
+    All files are written to disk and the output of each stage is used as the input to the next. 
 
+    
+    References
+    ----------
+    
+    https://imaging.mrc-cbu.cam.ac.uk/meg/Maxfilter
+    https://imaging.mrc-cbu.cam.ac.uk/meg/maxbugs
+    """
+    
     # --------------------------------------
-    # Stage 0 - Fit Origin without noce
+    # Stage 0 - Fit Origin without nose
     origin = fit_cbu_origin(infif, outbase, remove_nose=True)
 
     # --------------------------------------
     # Stage 1 - Find Bad Channels
 
     outfif = outbase.format('autobad_.fif')
     outlog = outbase.format('autobad.log')
@@ -524,16 +613,16 @@
 
     outfif, outlog = run_maxfilter(infif, outfif, stage2_args)
 
     # --------------------------------------
     # Stage 3 - Translate to default
 
     infif = outfif  # input is output from previous stage
-    outfif = outbase.format('trans.fif')
-    outlog = outbase.format('trans.log')
+    outfif = outbase.format('.fif')
+    outlog = outbase.format('.log')
 
     if os.path.exists(outfif):
         os.remove(outfif)
 
     # Fixed Args
     new_origin = [origin[0], origin[1] - 13, origin[2] + 6]
     stage3_args = {'autobad': None, 'trans': 'default',
@@ -547,30 +636,35 @@
 
 
 # -------------------------------------------------
 
 def run_maxfilter_batch(files, outdir, args=None):
     """Batch Maxfiltering.
 
-    Example use:
-    run_maxfilter_batch(files="/path/to/fif", outdir="/path/to/outdir",
-    args="--maxpath /neuro/bin/util/maxfilter --scanner Neo --tsss --mode
-    multistage --headpos --movecomp")
-
     Parameters
     ----------
     files : str or list of str
         Path(s) to raw fif files to maxfilter.
     outdir : str
         Path to directory to save output to.
     args : str
-        List of additional optional arguments to pass to osl_maxfilter.
+        List of additional optional arguments to pass to osl_maxfilter.  See ``help(osl.maxfilter)`` for all options.
         If a string is passed it it split input a list (delimited by spaces).
-        E.g. args="--maxpath /neuro/bin/util/maxfilter"
-        is equivalent to args=["--maxpath", "/neuro/bin/util/maxfilter"].
+        E.g. ``args="--maxpath /neuro/bin/util/maxfilter"``
+        is equivalent to ``args=["--maxpath", "/neuro/bin/util/maxfilter"]``.
+        
+    Notes
+    -----
+    Example use:
+    
+    
+    >>> run_maxfilter_batch(files="/path/to/fif", outdir="/path/to/outdir",
+        args="--maxpath /neuro/bin/util/maxfilter --scanner Neo --tsss --mode
+        multistage --headpos --movecomp")
+    
     """
 
     if args is None:
         args = []
     if isinstance(args, str):
         args = args.split(" ")
     argv = [files] + [outdir] + args
```

### Comparing `osl-0.5.1/osl/preprocessing/batch.py` & `osl-0.6.0/osl/preprocessing/batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 import re
 import logging
 from pathlib import Path
 from copy import deepcopy
 from functools import partial, wraps
 from time import localtime, strftime
 from datetime import datetime
+import inspect
 
 import mne
 import numpy as np
 import yaml
 
 from . import mne_wrappers, osl_wrappers
 from ..utils import find_run_id, validate_outdir, process_file_inputs, add_subdir
 from ..utils import logger as osl_logger
 from ..utils.parallel import dask_parallel_bag
+from ..utils.version_utils import check_version
 
 logger = logging.getLogger(__name__)
 
 
 # --------------------------------------------------------------
 # Decorators
 
@@ -74,15 +76,15 @@
     infile : str
         Path to file to read. File can be bti, fif, ds, meg4 or vhdr.
     preload : bool
         Should we load the data in the file?
 
     Returns
     -------
-    raw : mne.Raw
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
         Data as an MNE Raw object.
     """
     if not isinstance(infile, str):
         raise ValueError(
             "infile must be a str. Got type(infile)={0}.".format(type(infile))
         )
     if " " in infile:
@@ -102,15 +104,15 @@
         )
 
     # FIF file
     elif os.path.splitext(infile)[1] == ".fif":
         logger.info("Detected fif file format, using: mne.io.read_raw_fif")
         raw = mne.io.read_raw_fif(infile, preload=preload)
     # EDF file
-    elif os.path.splitext(infile)[1] == ".edf":
+    elif os.path.splitext(infile)[1].lower() == ".edf":
         logger.info("Detected edf file format, using: mne.io.read_raw_edf")
         raw = mne.io.read_raw_edf(infile, preload=preload)
     # CTF data in ds directory
     elif os.path.splitext(infile)[1] == ".ds":
         logger.info("Detected CTF file format, using: mne.io.read_raw_ctf")
         raw = mne.io.read_raw_ctf(infile, preload=preload)
     elif os.path.splitext(infile)[1] == ".meg4":
@@ -144,24 +146,27 @@
 # Batch processing utilities
 
 
 def find_func(method, target="raw", extra_funcs=None):
     """Find a preprocessing function.
 
     Function priority:
-    1) User custom function
-    2) MNE/OSL wrapper
-    3) MNE method on Raw or Epochs (specified by target)
+
+    1. User custom function
+    
+    2. MNE/OSL wrapper
+    
+    3. MNE method on Raw or Epochs (specified by target)
 
     Parameters
     ----------
     method : str
         Function name.
     target : str
-        Type of MNE object to preprocess. Can be 'raw', 'epochs', 'power' or 'itc'.
+        Type of MNE object to preprocess. Can be ``'raw'``, ``'epochs'``, ``'evoked'``, ``'power'`` or ``'itc'``.
     extra_funcs : list
         List of user-defined functions.
 
     Returns
     -------
     function
         Function to preprocess an MNE object.
@@ -232,14 +237,16 @@
             config = yaml.load(config, Loader=yaml.FullLoader)
 
     # Initialise missing values in config
     if "meta" not in config:
         config["meta"] = {"event_codes": None}
     elif "event_codes" not in config["meta"]:
         config["meta"]["event_codes"] = None
+    elif "versions" not in config['meta']:
+        config["meta"]["versions"] = None
 
     if "preproc" not in config:
         raise KeyError("Please specify preprocessing steps in config.")
 
     for stage in config["preproc"]:
         # Check each stage is a dictionary with a single key
         if not isinstance(stage, dict):
@@ -264,65 +271,104 @@
             raise KeyError(
                 "event_codes must be passed in config if we are finding events."
             )
 
     return config
 
 
-def get_config_from_fif(data):
+def check_config_versions(config):
     """Get config from a preprocessed fif file.
 
     Parameters
     ----------
-    data : mne.Raw
-        Preprocessing data.
+    config : dictionary or yaml string
+        Preprocessing configuration to check.
 
-    Return
+    Raises
     ------
+    AssertionError
+        Raised if package version mismatch found in 'version_assert'
+
+    WARNING
+        Raised if package version mismatch found in 'version_warn'
+
+    """
+    config = load_config(config)
+
+    # Check for version and raise an error if mismatch found
+    if 'version_assert' in config['meta']:
+        for vers in config['meta']['version_assert']:
+            check_version(vers, mode='assert')
+
+    # Check for version and raise a warning if mismatch found
+    if 'version_warn' in config['meta']:
+        for vers in config['meta']['version_warn']:
+            check_version(vers, mode='warn')
+
+
+def get_config_from_fif(inst):
+    """Get config from a preprocessed fif file.
+
+    Reads the ``inst.info['description']`` field of a fif file to get the
+    preprocessing config.
+    
+    Parameters
+    ----------
+    inst : :py:class:`mne.io.Raw <mne.io.Raw>`, :py:class:`mne.Epochs <mne.Epochs>`, :py:class:`mne.Evoked <mne.Evoked>`
+        Preprocessed MNE object.
+
+    Returns
+    -------
     dict
         Preprocessing config.
     """
     config_list = re.findall(
         "%% config start %%(.*?)%% config end %%",
-        data.info["description"],
+        inst.info["description"],
         flags=re.DOTALL,
     )
     config = []
     for config_text in config_list:
         config.append(load_config(config_text))
 
     return config
 
 
-def append_preproc_info(dataset, config):
-    """Add to the config of already preprocessed data.
+def append_preproc_info(dataset, config, extra_funcs=None):
+    """Add to the config of already preprocessed data to ``inst.info['description']``.
 
     Parameters
     ----------
     dataset : dict
         Preprocessed dataset.
     config : dict
         Preprocessing config.
 
     Returns
     -------
     dict
-        Dataset dict containing the preprocessed data.
+        Dataset dict containing the preprocessed data edited in place.
     """
     from .. import __version__  # here to avoid circular import
 
     if dataset["raw"].info["description"] == None:
         dataset["raw"].info["description"] = ""
 
     preproc_info = (
         "\n\nOSL BATCH PROCESSING APPLIED ON "
         + f"{datetime.today().strftime('%d/%m/%Y %H:%M:%S')} \n"
         + f"VERSION: {__version__}\n"
         + f"%% config start %% \n{config} \n%% config end %%"
     )
+    
+    if extra_funcs is not None:
+        preproc_info += "\n\nCUSTOM FUNCTIONS USED:\n"
+        for func in extra_funcs:
+            preproc_info += f"%% extra_funcs start %% \n{inspect.getsource(func)}\n%% extra_funcs end %%"
+    
     dataset["raw"].info["description"] = (
         dataset["raw"].info["description"] + preproc_info
     )
 
     if dataset["epochs"] is not None:
         if dataset["epochs"].info["description"] == None:
             dataset["epochs"].info["description"] = ""
@@ -332,24 +378,26 @@
 
     return dataset
 
 
 def write_dataset(dataset, outbase, run_id, ftype='preproc_raw', overwrite=False):
     """Write preprocessed data to a file.
 
+    Will write all keys in the dataset dict to disk with corresponding extensions.
+
     Parameters
     ----------
     dataset : dict
         Preprocessed dataset.
     outbase : str
         Path to directory to write to.
     run_id : str
         ID for the output file.
     ftype: str
-        Extension for the fif file (default "preproc_raw")
+        Extension for the fif file (default ``preproc_raw``)
     overwrite : bool
         Should we overwrite if the file already exists?
 
     Output
     ------
     fif_outname : str
         The saved fif file name
@@ -363,51 +411,55 @@
     fif_outname = outbase.format(run_id=run_id, ftype=ftype, fext="fif")
     if Path(fif_outname).exists() and not overwrite:
         raise ValueError(
             "{} already exists. Please delete or do use overwrite=True.".format(fif_outname)
         )
     dataset["raw"].save(fif_outname, overwrite=overwrite)
 
-    if dataset["events"] is not None:
+    if "events" in dataset and dataset['events'] is not None:
         outname = outbase.format(run_id=run_id, ftype="events", fext="npy")
         np.save(outname, dataset["events"])
 
-    if dataset["event_id"] is not None:
+    if "event_id" in dataset and dataset['event_id'] is not None:
         outname = outbase.format(run_id=run_id, ftype="event-id", fext="yml")
         yaml.dump(dataset["event_id"], open(outname, "w"))
 
-    if dataset["epochs"] is not None:
+    if "epochs" in dataset and dataset['epochs'] is not None:
         outname = outbase.format(run_id=run_id, ftype="epo", fext="fif")
         dataset["epochs"].save(outname, overwrite=overwrite)
 
-    if dataset["ica"] is not None:
+    if "ica" in dataset and dataset['ica'] is not None:
         outname = outbase.format(run_id=run_id, ftype="ica", fext="fif")
         dataset["ica"].save(outname, overwrite=overwrite)
 
+    if "tfr" in dataset and dataset['tfr'] is not None:
+        outname = outbase.format(run_id=run_id, ftype="tfr", fext="fif")
+        dataset["tfr"].save(outname, overwrite=overwrite)
+
     return fif_outname
 
 def read_dataset(fif, preload=False, ftype=None):
-    """Reads fif/npy/yml files associated with a dataset.
+    """Reads ``fif``/``npy``/``yml`` files associated with a dataset.
 
     Parameters
     ----------
     fif : str
         Path to raw fif file (can be preprocessed).
     preload : bool
         Should we load the raw fif data?
     ftype : str
-        Extension for the fif file (will be replaced for e.g. "_events.npy" or 
-        "_ica.fif"). If None, we assume the fif file is preprocessed with 
-        OSL and has the extension "preproc_raw". If this fails, we guess 
-        the extension as whatever comes after the last "_".
+        Extension for the fif file (will be replaced for e.g. ``'_events.npy'`` or 
+        ``'_ica.fif'``). If ``None``, we assume the fif file is preprocessed with 
+        OSL and has the extension ``'_preproc_raw'``. If this fails, we guess 
+        the extension as whatever comes after the last ``'_'``.
 
     Returns
     -------
     dataset : dict
-        Contains keys: 'raw', 'events', 'epochs', 'ica'.
+        Contains keys: ``'raw'``, ``'events'``, ``'event_id'``, ``'epochs'``, ``'ica'``.
     """
     print("Loading dataset:")
 
     print("Reading", fif)
     raw = mne.io.read_raw_fif(fif, preload=preload)
 
     # Guess extension
@@ -489,23 +541,23 @@
         Should we show the plot?
     stagecol : str
         Stage colour.
     startcol : str
         Start colour.
     fig : matplotlib.figure
         Matplotlib figure to plot on.
-    ax : matplotlib.axes
+    ax : :py:class:`matplotlib.axes <matplotlib.axes>`
         Matplotlib axes to plot on.
     title : str
         Title for the plot.
 
     Returns
     -------
-    fig : matplotlib.figure
-    ax : matplotlib.axes
+    fig : :py:class:`matplotlib.figure <matplotlib.figure>`
+    ax : :py:class:`matplotlib.axes <matplotlib.axes>`
     """
     config = load_config(config)
 
     if np.logical_or(ax == None, fig == None):
         fig = plt.figure(figsize=(8, 12))
         plt.subplots_adjust(top=0.95, bottom=0.05)
         ax = plt.subplot(111, frame_on=False)
@@ -594,50 +646,50 @@
     config : str or dict
         Preprocessing config.
     infile : str
         Path to input file.
     outname : str
         Output filename.
     ftype: str
-        Extension for the fif file (default "preproc_raw")
+        Extension for the fif file (default ``preproc_raw``)
     outdir : str
         Output directory. If processing multiple files, they can
-        be put in unique sub directories by including {x:0} at 
-        the end of the outdir, where x is the pattern which
-        precedes the unique identifier and 0 is the length of 
+        be put in unique sub directories by including ``{x:0}`` at 
+        the end of the outdir, where ``x`` is the pattern which
+        precedes the unique identifier and ``0`` is the length of 
         the unique identifier. For example: if the outdir is
-        ../../{sub-:3} and each is like 
-        /sub-001_task-rest.fif, the outdir for the file will be
-        ../../sub-001/
+        ``../../{sub-:3}`` and each is like 
+        ``/sub-001_task-rest.fif``, the outdir for the file will be
+        ``../../sub-001/``.
     logsdir : str
         Directory to save log files to.
     reportdir : str
         Directory to save report files to.
     ret_dataset : bool
         Should we return a dataset dict?
     gen_report : bool
         Should we generate a report?
     overwrite : bool
         Should we overwrite the output file if it already exists?
     extra_funcs : list
         User-defined functions.
     verbose : str
         Level of info to print.
-        Can be: CRITICAL, ERROR, WARNING, INFO, DEBUG or NOTSET.
+        Can be: ``'CRITICAL'``, ``'ERROR'``, ``'WARNING'``, ``'INFO'``, ``'DEBUG'`` or ``'NOTSET'``.
     mneverbose : str
         Level of info from MNE to print.
-        Can be: CRITICAL, ERROR, WARNING, INFO, DEBUG or NOTSET.
+        Can be: ``'CRITICAL'``, ``'ERROR'``, ``'WARNING'``, ``'INFO'``, ``'DEBUG'`` or ``'NOTSET'``.
 
     Returns
     -------
     dict or bool
-        If ret_dataset=True, a dict containing the preprocessed dataset with the
-        following keys: raw, ica, epochs, events, event_id. An empty dict is returned
-        if preprocessing fail. If return an empty dict. if ret_dataset=False, we
-        return a flag indicating whether preprocessing was successful.
+        If ``ret_dataset=True``, a dict containing the preprocessed dataset with the
+        following keys: ``raw``, ``ica``, ``epochs``, ``events``, ``event_id``. An empty dict is returned
+        if preprocessing fails. If ``ret_dataset=False``, we return a flag indicating whether 
+        preprocessing was successful.
     """
 
     # Generate a run ID
     if outname is None:
         run_id = find_run_id(infile)
     else:
         run_id = os.path.splitext(outname)[0]
@@ -733,15 +785,15 @@
             method, userargs = next(iter(stage.items()))
             target = userargs.get("target", "raw")  # Raw is default
             func = find_func(method, target=target, extra_funcs=extra_funcs)
             # Actual function call
             dataset = func(dataset, userargs)
 
         # Add preprocessing info to dataset dict
-        dataset = append_preproc_info(dataset, config)
+        dataset = append_preproc_info(dataset, config, extra_funcs)
 
         fif_outname = None
         if outdir is not None:
             fif_outname = write_dataset(dataset, outbase, run_id, overwrite=overwrite)
 
         # Generate report data
         if gen_report:
@@ -808,72 +860,81 @@
     else:
         return True
 
 
 def run_proc_batch(
     config,
     files,
+    outnames=None,
+    ftype=None,
     outdir=None,
     logsdir=None,
     reportdir=None,
     gen_report=True,
     overwrite=False,
     extra_funcs=None,
     verbose="INFO",
     mneverbose="WARNING",
     strictrun=False,
     dask_client=False,
-    ftype=None,
 ):
     """Run batched preprocessing.
 
     This function will write output to disk (i.e. will not return the preprocessed
     data).
 
     Parameters
     ----------
     config : str or dict
         Preprocessing config.
     files : str or list or mne.Raw
-        Can be a list of Raw objects or a list of filenames (or .ds dir names if CTF data)
-        or a path to a textfile list of filenames (or .ds dir names if CTF data).
+        Can be a list of Raw objects or a list of filenames (or ``.ds`` dir names if CTF data)
+        or a path to a textfile list of filenames (or ``.ds`` dir names if CTF data).
     outdir : str
         Output directory. If processing multiple files, they can
-        be put in unique sub directories by including {x:0} at 
-        the end of the outdir, where x is the pattern which
-        precedes the unique identifier and 0 is the length of 
+        be put in unique sub directories by including ``{x:0}`` at 
+        the end of the outdir, where ``x`` is the pattern which
+        precedes the unique identifier and ``0`` is the length of 
         the unique identifier. For example: if the outdir is
-        ../../{sub-:3} and each is like /sub-001_task-rest.fif, 
-        the outdir for the file will be ../../sub-001/
+        ``../../{sub-:3}`` and each is like ``/sub-001_task-rest.fif``, 
+        the outdir for the file will be ``../../sub-001/``.
     logsdir : str
         Directory to save log files to.
     reportdir : str
         Directory to save report files to.
     gen_report : bool
         Should we generate a report?
     overwrite : bool
         Should we overwrite the output file if it exists?
     extra_funcs : list
         User-defined functions.
     verbose : str
         Level of info to print.
-        Can be: CRITICAL, ERROR, WARNING, INFO, DEBUG or NOTSET.
+        Can be: ``'CRITICAL'``, ``'ERROR'``, ``'WARNING'``, ``'INFO'``, ``'DEBUG'`` or ``'NOTSET'``.
     mneverbose : str
         Level of info from MNE to print.
-        Can be: CRITICAL, ERROR, WARNING, INFO, DEBUG or NOTSET.
+        Can be: ``'CRITICAL'``, ``'ERROR'``, ``'WARNING'``, ``'INFO'``, ``'DEBUG'`` or ``'NOTSET'``.
     strictrun : bool
         Should we ask for confirmation of user inputs before starting?
     dask_client : bool
-        Indicate whether to use a previously initialised dask.distributed.Client
-        instance.
+        Indicate whether to use a previously initialised :py:class:`dask.distributed.Client <distributed.Client>`
+        instance. 
 
     Returns
     -------
     list of bool
         Flags indicating whether preprocessing was successful for each input file.
+        
+    Notes
+    -----
+    If you are using a :py:class:`dask.distributed.Client <distributed.Client>` instance, you must initialise it
+    before calling this function. For example:
+    
+    >>> from dask.distributed import Client
+    >>> client = Client(threads_per_worker=1, n_workers=4)
     """
 
     if outdir is None:
         # Use the current working directory
         outdir = os.getcwd()
 
     # Validate the parent outdir - later do so for each subdirectory
@@ -888,15 +949,27 @@
         verobse = 'INFO'
     logfile = os.path.join(logsdir, 'osl_batch.log')
     osl_logger.set_up(log_file=logfile, level=verbose, startup=False)
 
     logger.info('Starting OSL Batch Processing')
 
     # Check through inputs and parameters
-    infiles, outnames, good_files = process_file_inputs(files)
+    infiles, good_files_outnames, good_files = process_file_inputs(files)
+
+    # Specify filenames for the output data
+    if outnames is None:
+        outnames = good_files_outnames
+    else:
+        if len(outnames) != len(good_files_outnames):
+            logger.critical(
+                f"Number of outnames ({len(outnames)}) does not match "
+                f"number of good files {len(good_files_outnames)}. "
+                "Fix outnames or use outnames=None."
+            )
+
     if strictrun and click.confirm('Is this correct set of inputs?') is False:
         logger.critical('Stopping : User indicated incorrect number of input files')
         sys.exit(1)
     else:
         if strictrun:
             logger.info('User confirms input files')
 
@@ -928,15 +1001,14 @@
         gen_report=gen_report,
         overwrite=overwrite,
         extra_funcs=extra_funcs,
     )
 
     # Loop through input files to generate arguments for run_proc_chain
     args = []
-
     for infile, outname in zip(infiles, outnames):
         args.append((config, infile, outname))
 
     # Actually run the processes
     if dask_client:
         proc_flags = dask_parallel_bag(pool_func, args)
     else:
@@ -947,30 +1019,37 @@
         "Processed {0}/{1} files successfully".format(
             np.sum(proc_flags), len(proc_flags)
         )
     )
 
     # Generate a report
     if gen_report and len(infiles) > 0:
-        from ..report import raw_report # avoids circular import
-        raw_report.gen_html_page(reportdir)
-        if raw_report.gen_html_summary(reportdir):
+        from ..report import preproc_report # avoids circular import
+        preproc_report.gen_html_page(reportdir)
+        if preproc_report.gen_html_summary(reportdir):
             logger.info("******************************" + "*" * len(str(reportdir)))
             logger.info(f"* REMEMBER TO CHECK REPORT: {reportdir} *")
             logger.info("******************************" + "*" * len(str(reportdir)))
 
     # Return flags
     return proc_flags
 
 
 # ----------------------------------------------------------
 # Main CLI user function
 
 
 def main(argv=None):
+    """Main function for command line interface.
+    
+    Parameters
+    ----------
+    argv : list
+        Command line arguments.
+    """    
     if argv is None:
         argv = sys.argv[1:]
 
     parser = argparse.ArgumentParser(description="Batch preprocess some fif files.")
     parser.add_argument("config", type=str, help="yaml defining preproc")
     parser.add_argument(
         "files",
```

### Comparing `osl-0.5.1/osl/preprocessing/plot_ica.py` & `osl-0.6.0/osl/preprocessing/plot_ica.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,53 +17,55 @@
     block=False,
     show_first_samp=False,
     show_scrollbars=True,
     time_format="float",
     n_channels=10,
     bad_labels_list=["eog", "ecg", "emg", "hardware", "other"],
 ):
-    """Plot estimated latent sources given the unmixing matrix.
+    """OSL adaptation of MNE's :py:meth:`mne.preprocessing.ICA.plot_sources <mne.preprocessing.ICA.plot_sources>` function to 
+    plot estimated latent sources given the unmixing matrix.
 
     Typical usecases:
 
     1. plot evolution of latent sources over time based on (Raw input)
     2. plot latent source around event related time windows (Epochs input)
     3. plot time-locking in ICA space (Evoked input)
 
     Parameters
     ----------
-    ica : instance of mne.preprocessing.ICA
+    ica : :py:class:`mne.preprocessing.ICA <mne.preprocessing.ICA>`.
         The ICA solution.
-    inst : instance of mne.io.Raw, mne.Epochs, mne.Evoked
+    inst : :py:class:`mne.io.Raw <mne.io.Raw>`, :py:class:`mne.Epochs <mne.Epochs>`, or :py:class:`mne.Evoked <mne.Evoked>`.
         The object to plot the sources from.
-    %(picks_base)s all sources in the order as fitted.
+    picks : str
+        Channel types to pick.
     start, stop : float | int | None
-       If ``inst`` is a `~mne.io.Raw` or an `~mne.Evoked` object, the first and
-       last time point (in seconds) of the data to plot. If ``inst`` is a
-       `~mne.io.Raw` object, ``start=None`` and ``stop=None`` will be
-       translated into ``start=0.`` and ``stop=3.``, respectively. For
-       `~mne.Evoked`, ``None`` refers to the beginning and end of the evoked
-       signal. If ``inst`` is an `~mne.Epochs` object, specifies the index of
-       the first and last epoch to show.
+        If ``inst`` is a :py:class:`mne.io.Raw <mne.io.Raw>` or an  :py:class:`mne.Evoked <mne.Evoked>` object, the first and
+        last time point (in seconds) of the data to plot. If ``inst`` is a
+        :py:class:`mne.io.Raw <mne.io.Raw>` object, ``start=None`` and ``stop=None`` will be
+        translated into ``start=0.`` and ``stop=3.``, respectively. For
+        :py:class:`mne.Evoked <mne.Evoked>`, ``None`` refers to the beginning and end of the evoked
+        signal. If ``inst`` is an  :py:class:`mne.Epochs <mne.Epochs>` object, specifies the index of
+        the first and last epoch to show.
     title : str | None
         The window title. If None a default is provided.
     show : bool
         Show figure if True.
     block : bool
         Whether to halt program execution until the figure is closed.
         Useful for interactive selection of components in raw and epoch
         plotter. For evoked, this parameter has no effect. Defaults to False.
     show_first_samp : bool
         If True, show time axis relative to the ``raw.first_samp``.
     n_channels : int
-        OSL ADDITION - Number of channels to show at the same time
+        Number of channels to show at the same time (default: 10)
     bad_labels_list : list of str
-        OSL ADDITION -
-    %(show_scrollbars)s
-    %(time_format)s
+        list of bad labels to show in the bad labels list that can be used to mark the type of 
+        bad component. Defaults to ``["eog", "ecg", "emg", "hardware", "other"]``.
+ 
 
     Returns
     -------
     fig : instance of Figure
         The figure.
 
     Notes
@@ -132,14 +134,16 @@
     block,
     show_scrollbars,
     show_first_samp,
     time_format,
     n_channels,
     bad_labels_list,
 ):
+    """Adaptation of MNE's `mne.preprocessing.ica._plot_sources` function to allow for OSL additions.
+    """    
     """Plot the ICA components as a RawArray or EpochsArray."""
     # from mne.viz._figure import _get_browser
     from mne.viz.utils import _compute_scalings, _make_event_color_dict, plt_show
     from mne import EpochsArray, BaseEpochs
     from mne.io import RawArray, BaseRaw
     from mne.io.meas_info import create_info
     from mne.io.pick import pick_types
@@ -325,15 +329,18 @@
 
 from mne.viz._mpl_figure import MNEBrowseFigure
 
 backend = None
 
 
 def _get_browser(**kwargs):
-    """Instantiate a new MNE browse-style figure."""
+    """OSL Adaptation of MNE's `mne.viz._figure._get_browser` function 
+    that instantiate a new MNE browse-style figure.
+
+    """    
     from mne.viz.utils import _get_figsize_from_config
     from mne.viz._figure import _init_browser_backend
     import numpy as np
 
     figsize = kwargs.setdefault("figsize", _get_figsize_from_config())
     if figsize is None or np.any(np.array(figsize) < 8):
         kwargs["figsize"] = (8, 8)
@@ -346,16 +353,18 @@
     )  # OSL ADDITION IN ORDER TO USE OSL'S FIGURE CLASS FROM _INIT_BROWSER
 
     return browser
 
 
 def _init_browser(backend, **kwargs):  # OSL ADDITION IN ORDER TO USE OSL'S FIGURE CLASS
     from mne.viz._mpl_figure import _figure
-
-    """Instantiate a new MNE browse-style figure."""
+    """OSL's adaptation of MNE's `mne.viz._mpl_figure._init_browser` that 
+    instantiate a new MNE browse-style figure.
+    """
+    
     fig = _figure(toolbar=False, FigureClass=osl_MNEBrowseFigure, **kwargs)
 
     # initialize zen mode
     # (can't do in __init__ due to get_position() calls)
     fig.canvas.draw()
     fig._update_zen_mode_offsets()
     fig._resize(None)  # needed for MPL >=3.4
@@ -366,15 +375,17 @@
         fig.mne.scrollbars_visible = True
         fig._toggle_scrollbars()
 
     return fig
 
 
 class osl_MNEBrowseFigure(MNEBrowseFigure):
-    """Interactive figure with scrollbars, for data browsing."""
+    """OSL's adaptatation of MNE's `mne.viz._mpl_figure.MNEBrowseFigure` that
+    creates an interactive figure with scrollbars, for data browsing."""
+    
 
     def __init__(self, inst, figsize, ica=None,
                  xlabel='Time (s)', **kwargs):
         from matplotlib.colors import to_rgba_array
         from matplotlib.patches import Rectangle
         from matplotlib.ticker import (FixedFormatter, FixedLocator,
                                        FuncFormatter, NullFormatter)
@@ -659,14 +670,15 @@
             vline=vline,
             vline_hscroll=vline_hscroll,
             vline_text=vline_text,
         )
 
     def _draw_traces(self):
         """Draw (or redraw) the channel data."""
+        
         from matplotlib.colors import to_rgba_array
         from matplotlib.patches import Rectangle
 
         # OSL ADDITION
         from mne import pick_types
         from mne.io.pick import channel_type
         import numpy as np
```

### Comparing `osl-0.5.1/osl/report/raw_report.py` & `osl-0.6.0/osl/report/preproc_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 import sys
 import yaml
 import sails
 import argparse
 import tempfile
 import pickle
 import pathlib
+import re
 
 import numpy as np
 import matplotlib.pyplot as plt
 from jinja2 import Template
 from tabulate import tabulate
 from mne.channels.channels import channel_type
-from scipy.ndimage.filters import uniform_filter1d
 from matplotlib.lines import Line2D
 from matplotlib.patches import Rectangle
 from pathlib import Path
 
+try:
+    from scipy.ndimage import uniform_filter1d
+except ImportError:
+    from scipy.ndimage.filters import uniform_filter1d
+
 from ..utils import process_file_inputs, validate_outdir
 from ..utils.logger import log_or_print
 from ..preprocessing import (
     read_dataset,
     load_config,
     get_config_from_fif,
     plot_preproc_flowchart,
@@ -46,15 +51,15 @@
     Parameters
     ----------
     infiles : list of str
         List of paths to fif files.
     outdir : str
         Directory to save HTML report and figures to.
     ftype : str
-        Type of fif file, e.g., 'raw' or 'preproc_raw'.
+        Type of fif file, e.g., ``'raw'`` or ``'preproc_raw'``.
         
     """
 
     # Validate input files and directory to save html file and plots to
     infiles, outnames, good_files = process_file_inputs(infiles)
     outdir = validate_outdir(outdir)
 
@@ -71,28 +76,40 @@
 
     print("************" + "*" * len(str(outdir)))
     print(f"* REPORT: {outdir} *")
     print("************" + "*" * len(str(outdir)))
 
 
 def get_header_id(raw):
-    """Extract scan name from MNE data object."""
+    """Extract scan name from MNE data object.
+    
+    Parameters
+    ----------
+    raw : mne.io.:py:class:`mne.io.Raw <mne.io.Raw>`.
+        MNE Raw object.
+        
+    Returns
+    -------
+    id : str
+        Scan name.
+    
+    """
     return raw.filenames[0].split('/')[-1].strip('.fif')
 
 
 def gen_html_data(raw, outdir, ica=None, preproc_fif_filename=None):
     """Generate HTML web-report for an MNE data object.
 
     Parameters
     ----------
-    raw : mne.Raw
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
         MNE Raw object.
     outdir : string
         Directory to write HTML data and plots to.
-    ica : mne.preprocessing.ICA
+    ica : :py:class:`mne.preprocessing.ICA <mne.preprocessing.ICA>`
         ICA object.
     preproc_fif_filename : str
         Filename of file output by preprocessing
     """
 
     data = {}
     data['filename'] = raw.filenames[0]
@@ -176,14 +193,16 @@
     data['bad_chan_num'] = len(bad_chans)
 
     # Path to save plots
     savebase = str(outdir / '{0}.png')
     
     # Generate plots for the report
     data["plt_config"] = plot_flowchart(raw, savebase)
+    data["txt_extra_funcs"] = save_extra_funcs(raw, savebase.replace('.png', '.txt'))
+    data["plt_rawdata"] = plot_rawdata(raw, savebase)
     data['plt_temporalsumsq'] = plot_channel_time_series(raw, savebase, exclude_bads=False)
     data['plt_temporalsumsq_exclude_bads'] = plot_channel_time_series(raw, savebase, exclude_bads=True)
     data['plt_badchans'] = plot_sensors(raw, savebase)
     data['plt_channeldev'] = plot_channel_dists(raw, savebase, exclude_bads=False)
     data['plt_channeldev_exclude_bads'] = plot_channel_dists(raw, savebase, exclude_bads=True)
     data['plt_spectra'], data['plt_zoomspectra'] = plot_spectra(raw, savebase)
     data['plt_digitisation'] = plot_digitisation_2d(raw, savebase)
@@ -205,14 +224,19 @@
 def gen_html_page(outdir):
     """Generate an HTML page from a report directory.
 
     Parameters
     ----------
     outdir : str
         Directory to generate HTML report with.
+        
+    Returns
+    -------
+    success : bool
+        Whether the report was successfully generated.
     """
     outdir = pathlib.Path(outdir)
 
     # Subdirectories which contains plots for each fif file
     subdirs = sorted(
         [d.stem for d in pathlib.Path(outdir).iterdir() if d.is_dir()]
     )
@@ -296,14 +320,15 @@
     data = {}
     data["total"] = total
 
     # Create plots
     os.makedirs(f"{reportdir}/summary", exist_ok=True)
 
     data["plt_config"] = subject_data[0]["plt_config"]
+    data["txt_extra_funcs"] = subject_data[0]["txt_extra_funcs"]
     data["plt_summary_bad_segs"] = plot_summary_bad_segs(subject_data, reportdir)
     data["plt_summary_bad_chans"] = plot_summary_bad_chans(subject_data, reportdir)
 
     # Create panel
     panel_template = load_template('raw_summary_panel')
     panel = panel_template.render(data=data)
 
@@ -322,26 +347,52 @@
     with open(outpath, 'w') as f:
         f.write(page)
 
     return True
 
 
 def load_template(tname):
+    """Load an HTML template from the templates directory.
+
+    Parameters
+    ----------
+    tname : str
+        Name of the template to load.
+        
+    Returns
+    -------
+    template : jinja2.Template
+        The loaded template.
+    """
     basedir = os.path.dirname(os.path.realpath(__file__))
     fname = os.path.join(basedir, 'templates', '{0}.html'.format(tname))
     with open(fname, 'r') as file:
         template = Template(file.read())
     return template
 
 
 # ----------------------------------------------------------------------------------
 # Scan stats and figures
 
 def plot_flowchart(raw, savebase=None):
-    """Plots preprocessing flowchart(s)"""
+    """Plots preprocessing flowchart(s)
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.    
+    
+    """
     
     # Get config info from raw.info['description']
     config_list = get_config_from_fif(raw)
 
     # Number of subplots, i.e. the number of times osl preprocessing was applied
     nrows = len(config_list)
 
@@ -372,16 +423,98 @@
         savebase = pathlib.Path(savebase)
         filebase = savebase.parent.name + "/" + savebase.name
         fpath = filebase.format('flowchart')
     else:
         fpath = None
     return fpath
 
+
+def save_extra_funcs(raw, savebase=None):
+    """ Saves extra functions from the raw.info['description'] to a text file.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved text file.
+    
+    """
+    extra_funcs = re.findall(
+        "%% extra_funcs start %%(.*?)%% extra_funcs end %%",
+        raw.info["description"],
+        flags=re.DOTALL,
+    )
+    
+    if savebase is not None:
+        fpath = savebase.format(f"extra_funcs")
+        with(open(fpath, 'w')) as file:
+            [print(func, file=file) for func in extra_funcs]
+        return fpath
+    else:
+        return None
+    
+        
+
+def plot_rawdata(raw, savebase):
+    """Plots raw data.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.      
+    
+    """
+
+    fig = raw.pick(['meg', 'eeg']).plot(n_channels=np.inf, duration=raw.times[-1])
+
+    if savebase is not None:
+        figname = savebase.format('rawdata')
+        fig.savefig(figname, dpi=150, transparent=True)
+        plt.close(fig)
+
+        # Return the filename
+        savebase = pathlib.Path(savebase)
+        filebase = savebase.parent.name + "/" + savebase.name
+        fpath = filebase.format('rawdata')
+    else:
+        fpath = None
+    return fpath
+
+
 def plot_channel_time_series(raw, savebase=None, exclude_bads=False):
-    """Plots sum-square time courses."""
+    """Plots sum-square time courses.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+    exclude_bads : bool
+        Whether to exclude bad channels and bad segments.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.    
+    
+    """
 
     if exclude_bads:
         # excludes bad channels and bad segments
         exclude = 'bads'
     else:
         # includes bad channels and bad segments
         exclude = []
@@ -482,15 +615,29 @@
         fpath = filebase.format(plot_name)
     else:
         fpath = None
     return fpath
 
 
 def plot_sensors(raw, savebase=None):
-    """Plots sensors with bad channels highlighted."""
+    """Plots sensors with bad channels highlighted.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.    
+    
+    """
     # plot channel types seperately for neuromag306 (3 coils in same location)
 
     if 3012 in np.unique([i['coil_type'] for i in raw.info['chs']]):
         with open(str(Path(__file__).parent.parent) + "/utils/neuromag306_info.yml", 'r') as f:
             channels = yaml.safe_load(f)
         if 3024 in np.unique([i['coil_type'] for i in raw.info['chs']]):
             coil_types = ['mag', 'grad_longitude', 'grad_lattitude']
@@ -518,15 +665,30 @@
         fpath = filebase.format('bad_chans')
     else:
         fpath = None
     return fpath
 
 
 def plot_channel_dists(raw, savebase=None, exclude_bads=True):
-    """Plot distributions of temporal standard deviation."""
+    """Plot distributions of temporal standard deviation.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str 
+        Base string for saving figures.
+    exclude_bads : bool
+        Whether to exclude bad channels and bad segments.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.    
+    """
 
     if exclude_bads:
         # excludes bad channels and bad segments
         exclude = 'bads'
         reject_by_annotation = 'omit'
     else:
         # includes bad channels and bad segments
@@ -600,15 +762,30 @@
         fpath = filebase.format(plot_name)
     else:
         fpath = None
     return fpath
 
 
 def plot_spectra(raw, savebase=None):
-    """Plot power spectra for each sensor modality."""
+    """Plot power spectra for each sensor modality.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`   
+        MNE Raw object.
+    savebase : str  
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath1 : str
+        Path to saved figure (full spectra).
+    fpath2 : str
+        Path to saved figure (zoomed in spectra).
+    """
 
     is_ctf = raw.info["dev_ctf_t"] is not None
     if is_ctf:
         # Note that with CTF mne.pick_types will return:
         # ~274 axial grads (as magnetometers) if {picks: 'mag', ref_meg: False}
         # ~28 reference axial grads if {picks: 'grad'}
         channel_types = {
@@ -637,21 +814,20 @@
     row = 0
 
     for name, chan_inds in sorted(channel_types.items()):
         if len(chan_inds) == 0:
             continue
 
         # Plot spectra
-        raw.plot_psd(
-            show=False,
-            picks=chan_inds,
-            ax=ax[row],
+        raw.compute_psd(
+            picks=chan_inds, 
             n_fft=int(raw.info['sfreq']*2),
-            verbose=0,
-        )
+            verbose=0).plot(
+                        axes=ax[row],
+                        show=False)
 
         ax[row].set_title(name, fontsize=12)
 
         row += 1
 
     # Save full spectra
     if savebase is not None:
@@ -666,23 +842,22 @@
     row = 0
 
     for name, chan_inds in sorted(channel_types.items()):
         if len(chan_inds) == 0:
             continue
 
         # Plot zoomed in spectra
-        raw.plot_psd(
-            show=False,
-            picks=chan_inds,
-            ax=ax[row],
-            fmin=1,
-            fmax=48,
-            n_fft=int(raw.info['sfreq']*2),
-            verbose=0,
-        )
+        raw.compute_psd(
+        picks=chan_inds, 
+        fmin=1,
+        fmax=48,
+        n_fft=int(raw.info['sfreq']*2),
+        verbose=0).plot(
+                    axes=ax[row],
+                    show=False)
 
         ax[row].set_title(name, fontsize=12)
 
         row += 1
 
     # Save zoomed in spectra
     if savebase is not None:
@@ -698,15 +873,28 @@
     else:
         fpath1 = None
         fpath2 = None
     return fpath1, fpath2
 
 
 def plot_digitisation_2d(raw, savebase=None):
-    """Plots the digitisation and headshape."""
+    """Plots the digitisation and headshape.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.
+    """
 
     # Return if no digitisation available
     if not raw.info['dig']:
         return None
 
     # Make plot
     fig = plt.figure(figsize=(16, 4))
@@ -814,15 +1002,28 @@
         fpath = filebase.format('EOG')
     else:
         fpath = None
     return fpath
 
 
 def plot_ecg_summary(raw, savebase=None):
-    """Plot ECG summary."""
+    """Plot ECG summary.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.
+    """
 
     # Get the raw ECG data
     chan_inds = mne.pick_types(raw.info, ecg=True)
     if len(chan_inds) == 0:
         return None
     t = raw.times
     x = raw.get_data(chan_inds).T
@@ -845,15 +1046,31 @@
         fpath = filebase.format('ECG')
     else:
         fpath = None
     return fpath
 
 
 def plot_bad_ica(raw, ica, savebase):
-    """Plot ICA characteristics for rejected components."""
+    """Plot ICA characteristics for rejected components.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    ica : :py:class:`mne.preprocessing.ICA <mne.preprocessing.ICA>` 
+        MNE ICA object.
+    savebase : str  
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.
+    
+    """
 
     exclude_uniq = np.sort(np.unique(ica.exclude))[::-1]
     nbad = len(exclude_uniq)
 
     # Handle the case when ica.labels_ and ica.exclude don't match
     if len(ica.labels_) != nbad:
         # Make a dummy labels_ dict
@@ -1014,15 +1231,28 @@
     ax.set_xlabel("Subject")
     ax.set_ylabel("Number of bad channels")
     fig.savefig(output_file, dpi=300)
     plt.close(fig)
     return f"summary/bad_chans.png"
 
 def plot_artefact_scan(raw, savebase=None):
-
+    """Plot artefact scan.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.
+    savebase : str
+        Base string for saving figures.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved figure.
+    """
     events = mne.find_events(raw, min_duration=2/raw.info['sfreq'])
     modalities = ['mag', 'grad']
 
     # Plot eye movements
     event_dict = {'moves': 1}
     epochs = mne.Epochs(raw, events, event_id=event_dict, tmin=-1, tmax=16.5,
                         preload=True)
@@ -1183,15 +1413,21 @@
         'plt_buttonpress_grad': filebase.format('buttonpress_grad'),
         'plt_buttonpress_mag': filebase.format('buttonpress_mag'),
     }
     return filenames
 
 
 def print_scan_summary(raw):
-    """Print a text summary of an MNE file."""
+    """Print a text summary of an MNE file.
+    
+    Parameters
+    ----------
+    raw : :py:class:`mne.io.Raw <mne.io.Raw>`
+        MNE Raw object.    
+    """
     print('Datafile : {0}'.format(raw.filenames))
 
     # Project name - set by user during acquisition
     print('Project name: {0}'.format(raw.info['proj_name']))
     print('Experimenter: {0}'.format(raw.info['experimenter']))
 
     date = raw.info['meas_date']
```

### Comparing `osl-0.5.1/osl/report/src_report.py` & `osl-0.6.0/osl/report/src_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """Reporting tool for source reconstruction.
 
 """
 
 # Authors: Chetan Gohil <chetan.gohil@psych.ox.ac.uk>
+# Mats van Es <mats.vanes@psych.ox.ac.uk>
 
 import os
 import os.path as op
 from pathlib import Path
 from shutil import copy
 
 import pickle
 import numpy as np
 import matplotlib.pyplot as plt
 from tabulate import tabulate
+import inspect
 
-from . import raw_report
+from . import preproc_report
 from ..source_recon import parcellation
 
 
-def gen_html_data(config, src_dir, subject, reportdir, logger=None):
+def gen_html_data(config, src_dir, subject, reportdir, logger=None, extra_funcs=None):
     """Generate data for HTML report.
 
     Parameters
     ----------
     config : dict
         Source reconstruction config.
     src_dir : str
         Source reconstruction directory.
     subject : str
         Subject name.
     reportdir : str
         Report directory.
     logger : logging.getLogger
         Logger.
+    extra_funcs : list
+        List of extra functions to run
     """
     src_dir = Path(src_dir)
     reportdir = Path(reportdir)
 
     # Make directory for plots contained in the report
     os.makedirs(reportdir, exist_ok=True)
     os.makedirs(reportdir / subject, exist_ok=True)
@@ -59,14 +63,16 @@
 
     # Otherwise, this is the first time this has been called
     else:
         # Data for the report
         data = {}
         data["config"] = config
 
+    data['extra_funcs'] = save_extra_funcs(extra_funcs, reportdir / subject)
+    
     data["fif_id"] = subject
     data["filename"] = subject
 
     # What have we done for this subject?
     data["compute_surfaces"] = subject_data.pop("compute_surfaces", False)
     data["coregister"] = subject_data.pop("coregister", False)
     data["beamform"] = subject_data.pop("beamform", False)
@@ -112,21 +118,50 @@
         data["plt_parc_corr"] = f"{subject}/parc_corr.png"
         copy("{}/{}".format(src_dir, subject_data["parc_corr_plot"]), "{}/{}/parc_corr.png".format(reportdir, subject))
 
     # Save data in the report directory
     pickle.dump(data, open(f"{reportdir}/{subject}/data.pkl", "wb"))
 
 
+def save_extra_funcs(extra_funcs, reportdir):
+    """ Saves extra functions to a text file.
+    
+    Parameters
+    ----------
+    extra_funcs : list
+        List of extra functions to save.
+    reportdir : str
+        Subject report directory.
+        
+    Returns
+    -------
+    fpath : str
+        Path to saved text file.
+    """
+    if reportdir is not None and extra_funcs is not None:
+        fpath = reportdir / 'extra_funcs.txt'
+        with(open(fpath, 'w')) as file:
+            [print(f"{inspect.getsource(func)}\n\n", file=file) for func in extra_funcs]
+        return fpath
+    else:
+        return None
+
+
 def gen_html_page(reportdir):
     """Generate an HTML page from a report directory.
 
     Parameters
     ----------
     reportdir : str
         Directory to generate HTML report with.
+        
+    Returns
+    -------
+    bool
+        Whether the report was generated successfully.    
     """
     reportdir = Path(reportdir)
 
     # Subdirectories which contains plots for each fif file
     subdirs = sorted([d.stem for d in Path(reportdir).iterdir() if d.is_dir()])
 
     # Load HTML data
@@ -147,27 +182,27 @@
     # and an id for each file
     for i in range(total):
         data[i]["num"] = i + 1
         data[i]["total"] = total
 
     # Create panels
     panels = []
-    panel_template = raw_report.load_template('src_subject_panel')
+    panel_template = preproc_report.load_template('src_subject_panel')
 
     for i in range(total):
         panels.append(panel_template.render(data=data[i]))
 
     # Hyperlink to each panel on the page
     filenames = ""
     for i in range(total):
         filename = Path(data[i]["filename"]).name
         filenames += "{0}. {1}<br>".format(i + 1, filename)
 
     # Render the full page
-    page_template = raw_report.load_template('subject_report')
+    page_template = preproc_report.load_template('subject_report')
     page = page_template.render(panels=panels, filenames=filenames)
 
     # Write the output file
     outpath = Path(reportdir) / 'subject_report.html'
     with open(outpath, 'w') as f:
         f.write(page)
 
@@ -177,14 +212,19 @@
 def gen_html_summary(reportdir):
     """Generate an HTML summary from a report directory.
 
     Parameters
     ----------
     reportdir : str
         Directory to generate HTML summary report with.
+        
+    Returns
+    -------
+    bool
+        Whether the report was generated successfully.
     """
     reportdir = Path(reportdir)
 
     # Subdirectories which contains plots for each fif file
     subdirs = sorted([d.stem for d in Path(reportdir).iterdir() if d.is_dir()])
 
     # Load HTML data
@@ -201,14 +241,15 @@
     if total == 0:
         return False
 
     # Data used in the summary report
     data = {}
     data["total"] = total
     data["config"] = subject_data[0]["config"]
+    data["extra_funcs"] = subject_data[0]["extra_funcs"]
     data["coregister"] = subject_data[0]["coregister"]
     data["beamform"] = subject_data[0]["beamform"]
     data["beamform_and_parcellate"] = subject_data[0]["beamform_and_parcellate"]
     data["fix_sign_ambiguity"] = subject_data[0]["fix_sign_ambiguity"]
 
     if data["coregister"]:
         subjects = np.array([d["filename"] for d in subject_data])
@@ -247,25 +288,25 @@
 
     if data["fix_sign_ambiguity"]:
         data["template"] = subject_data[0]["template"]
         metrics = np.array([d["metrics"] for d in subject_data if "metrics" in d])
         data["plt_sflip"] = plot_sign_flipping_results(metrics, reportdir)
 
     # Create panel
-    panel_template = raw_report.load_template('src_summary_panel')
+    panel_template = preproc_report.load_template('src_summary_panel')
     panel = panel_template.render(data=data)
 
     # List of filenames
     filenames = ""
     for i in range(total):
         filename = Path(subject_data[i]["filename"]).name
         filenames += "{0}. {1}<br>".format(i + 1, filename)
 
     # Render the full page
-    page_template = raw_report.load_template('summary_report')
+    page_template = preproc_report.load_template('summary_report')
     page = page_template.render(panel=panel, filenames=filenames)
 
     # Write the output file
     outpath = Path(reportdir) / 'summary_report.html'
     with open(outpath, 'w') as f:
         f.write(page)
```

### Comparing `osl-0.5.1/osl/report/templates/raw_subject_panel.html` & `osl-0.6.0/osl/report/templates/raw_subject_panel.html`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
                     {{ data.eventtable }}
                 </div>
             </div>
         </div>
     </div>
     
     <div class="tabpage" style="width: 100%; display: none" id={{ data.fif_id }}_timeseries>
+        <div style="width: 100%">
+            <h4>Raw data</h4>
+            <img src="{{ data.plt_rawdata }}" alt="" style='max-width: 60%'/>
+        </div>
         {% if data.bad_seg != [] %}
             <div style="width: 100%">
                 <h4>Bad segments</h4>
                 <span>{{ '<br/>'.join(data.bad_seg[::-1]) }}</span>
             </div>
         {% endif %}
         <div style="width: 100%">
```

### Comparing `osl-0.5.1/osl/report/templates/raw_summary_panel.html` & `osl-0.6.0/osl/report/templates/raw_summary_panel.html`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,16 @@
   </div>
 
   <div class="flex-child" style="flex: 5; padding-left: 25px">
 
     <div class="tabpage" style='width: 100%' id='config'>
         <h3>Config</h3>
         <img src="{{ data.plt_config }}" alt="" style='max-width: 60%'/>
+        <h3>Extra functions</h3>
+        <iframe src="{{ data.txt_extra_funcs }}" style="width: 80%; height: 200px;"></iframe>
     </div>
 
     <div class="tabpage" style='width: 100%' id='time'>
         <h3>Time Series</h3>
         {% if data.plt_summary_bad_segs != [] %}
             <h4>Bad segments</h4>
             <img src="{{ data.plt_summary_bad_segs }}" alt="" style='max-width: 60%'/>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 Config Time Series Channels
 ******** CCoonnffiigg ********
+******** EExxttrraa ffuunnccttiioonnss ********
 ******** TTiimmee SSeerriieess ********
 {% if data.plt_summary_bad_segs != [] %}
 ****** BBaadd sseeggmmeennttss ******
 {% else %} No summary. {% endif %}
 ******** CChhaannnneellss ********
 {% if data.plt_summary_bad_chans != [] %}
 ****** BBaadd cchhaannnneellss ******
```

### Comparing `osl-0.5.1/osl/report/templates/src_subject_panel.html` & `osl-0.6.0/osl/report/templates/src_subject_panel.html`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/report/templates/src_summary_panel.html` & `osl-0.6.0/osl/report/templates/src_summary_panel.html`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
   </div>
 
   <div class="flex-child" style="flex: 5; padding-left: 25px">
 
     <div class="tabpage" style='width: 100%' id='config'>
         <h3>Config</h3>
         <img src="{{ data.plt_config }}" alt="" style='max-width: 60%'/>
+        <h3>Extra functions</h3>
+        <iframe src="{{ data.extra_funcs }}" style="width: 80%; height: 200px;"></iframe>
     </div>
 
     {% if data.coregister %}
         <div class="tabpage" style='width: 100%' id='coregistration'>
             <h3>Coregistration</h3>
             {% if data.coreg_table is defined %}
                 Distance between polhemus and structural MRI fiducials in cm.</br></br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 Config {% if data.coregister %} Coregistration {% endif %} {% if
 data.beamform_and_parcellate %} Parcellation {% endif %} {% if
 data.fix_sign_ambiguity %} Sign Flipping {% endif %}
 ******** CCoonnffiigg ********
+******** EExxttrraa ffuunnccttiioonnss ********
 {% if data.coregister %}
 ******** CCoorreeggiissttrraattiioonn ********
 {% if data.coreg_table is defined %} Distance between polhemus and structural
 MRI fiducials in cm. {{ data.coreg_table }} {% else %} No fiducials were used
 in coregistration. {% endif %}
 {% endif %} {% if data.beamform_and_parcellate %}
 ******** PPaarrcceellllaattiioonn ********
```

### Comparing `osl-0.5.1/osl/report/templates/subject_report.html` & `osl-0.6.0/osl/report/templates/subject_report.html`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/report/templates/summary_report.html` & `osl-0.6.0/osl/report/templates/summary_report.html`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/batch.py` & `osl-0.6.0/osl/source_recon/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             f.write(str(ex_value))
             f.write("\n")
             traceback.print_tb(ex_traceback, file=f)
 
         return False
 
     # Generate HTML data for the report
-    src_report.gen_html_data(config, src_dir, subject, reportdir)
+    src_report.gen_html_data(config, src_dir, subject, reportdir, extra_funcs=extra_funcs)
 
     return True
 
 
 def run_src_batch(
     config,
     src_dir,
```

### Comparing `osl-0.5.1/osl/source_recon/beamforming.py` & `osl-0.6.0/osl/source_recon/beamforming.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 import os
 import os.path as op
 
 import numpy as np
 import matplotlib.pyplot as plt
 import mne
 from mne import read_forward_solution, Covariance, compute_covariance, compute_raw_covariance
-from mne.io.meas_info import _simplify_info
-from mne.io.pick import pick_channels_cov, pick_info
-from mne.io.proj import make_projector
 from mne.rank import compute_rank
 from mne.minimum_norm.inverse import _check_depth, _prepare_forward, _get_vertno
 from mne.source_estimate import _get_src_type
 from mne.forward import _subject_from_forward
 from mne.forward.forward import is_fixed_orient
 from mne.beamformer import read_beamformer
 from mne.beamformer._lcmv import _apply_lcmv
@@ -35,14 +32,24 @@
     _check_src_normal,
     check_version,
     verbose,
     warn,
 )
 from mne.utils import logger as mne_logger
 
+try:
+    from mne._fiff.meas_info import _simplify_info
+    from mne._fiff.pick import pick_channels_cov, pick_info
+    from mne._fiff.proj import make_projector
+except ImportError:
+    # Depreciated in mne 1.6
+    from mne.io.meas_info import _simplify_info
+    from mne.io.pick import pick_channels_cov, pick_info
+    from mne.io.proj import make_projector
+
 from osl.source_recon import rhino
 from osl.source_recon.rhino import utils as rhino_utils
 from osl.utils.logger import log_or_print
 
 
 def get_beamforming_filenames(subjects_dir, subject):
     """Get beamforming filenames.
@@ -243,24 +250,57 @@
     """
     filenames = get_beamforming_filenames(subjects_dir, subject)
     log_or_print(f"loading {filenames['filters_file']}")
     return read_beamformer(filenames["filters_file"])
 
 
 def apply_lcmv(data, filters, reject_by_annotation="omit"):
-    """Apply a LCMV filter to an MNE Raw or Epochs object."""
+    """Apply a LCMV filter to an MNE Raw or Epochs object.
+    
+    Parameters
+    ----------
+    data : instance of :py:class:`mne.io.Raw` or :py:class:`mne.Epochs`
+        The data to apply the LCMV filter to.
+    filters : instance of :py:class:`mne.beamformer.Beamformer`
+        The LCMV filter to apply.
+    reject_by_annotation : str | list of str | None
+        If string, the annotation description to use to reject epochs.
+        If list of str, the annotation descriptions to use to reject epochs.
+        If None, do not reject epochs.
+        
+    Returns
+    -------
+    :py:class:`mne.SourceEstimate`
+    """
     log_or_print("beamforming.apply_lcmv")
     if isinstance(data, mne.io.Raw):
         return apply_lcmv_raw(data, filters, reject_by_annotation)
     else:
         return mne.beamformer.apply_lcmv_epochs(data, filters)
 
 
 def apply_lcmv_raw(raw, filters, reject_by_annotation="omit"):
-    """Modified version of mne.beamformer.apply_lcmv_raw."""
+    """Modified version of mne.beamformer.apply_lcmv_raw.
+    
+    Parameters
+    ----------
+    raw : instance of :py:class:`mne.io.Raw`
+        The raw data to apply the LCMV filter to.
+    filters : instance of :py:class:`mne.beamformer.Beamformer`
+        The LCMV filter to apply.
+    reject_by_annotation : str | list of str | None
+        If string, the annotation description to use to reject epochs.
+        If list of str, the annotation descriptions to use to reject epochs.
+        If None, do not reject epochs.
+        
+    Returns
+    -------
+    :py:class:`mne.SourceEstimate`
+    
+    """
 
     _check_reference(raw)
 
     # Get data from the mne.Raw object
     data, times = raw.get_data(return_times=True, reject_by_annotation=reject_by_annotation)
 
     # Select channels
@@ -289,15 +329,15 @@
 
     Returns
     -------
     recon_timeseries : numpy.ndarray
         The timecourse in recon_timeseries_head nearest to coord_mni.
     """
 
-    rhino_files = rhino_utils.get_rhino_files(subjects_dir, subjects)
+    rhino_files = rhino_utils.get_rhino_files(subjects_dir, subject)
     surfaces_filenames = rhino_files["surf"]
     coreg_filenames = rhino_files["coreg"]
 
     # Get coord_mni in mri space
     mni_mri_t = rhino_utils.read_trans(surfaces_filenames["mni_mri_t_file"])
     coord_mri = rhino_utils.xform_points(mni_mri_t["trans"], coord_mni)
 
@@ -471,15 +511,17 @@
     spatial_resolution : int
         Resolution to use for the reference brain in mm (must be an integer, or will be cast to nearest int). If None, then the gridstep used in rhino_files['fwd_model'] is used.
     reference_brain : string
         'mni' indicates that the reference_brain is the stdbrain in MNI space.
         'mri' indicates that the reference_brain is the subject's sMRI in the scaled native/mri space.
         'unscaled_mri' indicates that the reference_brain is the subject's sMRI in unscaled native/mri space.
         Note that Scaled/unscaled relates to the allow_smri_scaling option in coreg. If allow_scaling was False, then the unscaled MRI will be the same as the scaled MRI.
-
+    verbose : bool
+        If True, print out more information.
+    
     Returns
     -------
     leadfield_out : numpy.ndarray
         (nsensors, ndipoles) np.array of lead fields resampled on the reference brain grid.
     """
 
     rhino_files = rhino_utils.get_rhino_files(subjects_dir, subject)
@@ -591,14 +633,67 @@
     depth=None,
     inversion="matrix",
     verbose=None,
 ):
     """Compute LCMV spatial filter.
 
     Modified version of mne.beamformer._make_lcmv.
+    
+    Parameters
+    ----------
+    info : instance of :py:class:`mne.Info`
+        The measurement info to specify the channels to include.
+    forward : instance of :py:class:`mne.Forward`
+        The forward solution.
+    data_cov : instance of :py:class:`mne.Covariance`
+        The data covariance object.
+    reg : float
+        The regularization for the whitened data covariance.
+    noise_cov : instance of :py:class:`mne.Covariance`
+        The noise covariance object.
+    label : instance of :py:class:`mne.Label`
+        Restricts the LCMV solution to a given label.
+    pick_ori : None | 'normal' | 'max-power' | max-power-pre-weight-norm
+        The source orientation to compute the beamformer in.
+    rank : dict | None | 'full' | 'info'
+        This controls the rank computation that can be read from the measurement info or estimated from the data. When a noise covariance is used for whitening, this should reflect the rank of that covariance, otherwise amplification of noise components can occur in whitening (e.g., often during source localization).
+    
+        ``None``
+            The rank will be estimated from the data after proper scaling of different channel types. 
+        
+        ``'info'``
+            The rank is inferred from info. If data have been processed with Maxwell filtering, the Maxwell filtering header is used. Otherwise, the channel counts themselves are used. In both cases, the number of projectors is subtracted from the (effective) number of channels in the data. For example, if Maxwell filtering reduces the rank to 68, with two projectors the returned value will be 66. 
+        
+        ``'full'``
+            The rank is assumed to be full, i.e. equal to the number of good channels. If a Covariance is passed, this can make sense if it has been (possibly improperly) regularized without taking into account the true data rank. 
+        
+        dict
+            Calculate the rank only for a subset of channel types, and explicitly specify the rank for the remaining channel types. This can be extremely useful if you already know the rank of (part of) your data, for instance in case you have calculated it earlier.
+            This parameter must be a dictionary whose keys correspond to channel types in the data (e.g. 'meg', 'mag', 'grad', 'eeg'), and whose values are integers representing the respective ranks. For example, {'mag': 90, 'eeg': 45} will assume a rank of 90 and 45 for magnetometer data and EEG data, respectively.
+            The ranks for all channel types present in the data, but not specified in the dictionary will be estimated empirically. That is, if you passed a dataset containing magnetometer, gradiometer, and EEG data together with the dictionary from the previous example, only the gradiometer rank would be determined, while the specified magnetometer and EEG ranks would be taken for granted. 
+
+        The default is ``'info'``. 
+    noise_rank : dict | None | 'full' | 'info'
+        This controls the rank computation that can be read from the measurement info or estimated from the data. When a noise covariance is used for whitening, this should reflect the rank of that covariance, otherwise amplification of noise components can occur in whitening (e.g., often during source localization).
+    weight_norm : None | 'unit-noise-gain' | 'nai'
+        The weight normalization scheme to use.
+    reduce_rank : bool
+        Whether to reduce the rank by one during computation of the filter.
+    depth : None | float | dict
+        How to weight (or normalize) the forward using a depth prior (see Notes).
+    inversion : 'matrix' | 'single'
+        The inversion scheme to compute the weights.
+    verbose : bool, str, int, or None
+        If not None, override default verbose level (see mne.verbose).
+        
+    Returns
+    -------
+    filters : instance of :py:class:`mne.beamformer.Beamformer`
+        Dictionary containing filter weights from LCMV beamformer. See MNE docs.
+        
     """
     # Code that is different to mne.beamformer.make_lcmv is labelled with MWW
 
     # Check number of sensor types present in the data and ensure a noise cov
     info = _simplify_info(info)
     noise_cov, _, allow_mismatch = _check_one_ch_type("lcmv", info, forward, data_cov, noise_cov)
 
@@ -968,14 +1063,62 @@
     limit=None,
     allow_fixed_depth=True,
     limit_depth_chs=False,
 ):
     """Input preparation common for LCMV, DICS, and RAP-MUSIC.
 
     Modified version of mne.beamformer._prepare_beamformer_input.
+    
+    Parameters
+    ----------
+    info : instance of :py:class:`mne.Info`
+        Measurement info
+    forward : instance of :py:class:`mne.Forward`
+        The forward solution.
+    label : instance of :py:class:`mne.Label` | None
+        Restricts the forward solution to a given label.
+    pick_ori : None | 'normal' | 'max-power' | 'vector' | 'max-power-pre-weight-norm'
+        The source orientation to compute the beamformer in.
+    noise_cov : instance of :py:class:`mne.Covariance` | None
+        The noise covariance.
+    rank : dict | None | 'full' | 'info'
+        See :py:func:`mne.compute_rank`.
+    pca : bool
+        If True, the rank of the forward is reduced to match the rank of the noise covariance matrix.
+    loose : float | None
+        Value that weights the source variances of the dipole components defining the tangent space of the cortical surfaces. If ``None``, no loose orientation constraint is applied.
+    combine_xyz : str
+        How to combine the dipoles in the same locations of the forward model when picking normals. See :py:func:`mne.forward._pick_ori`.
+    exp : float | None
+        Exponent for the depth weighting. If None, no depth weighting is performed.
+    limit : float | None
+        Limit on depth weighting factors. If None, no upper limit is applied.
+    allow_fixed_depth : bool
+        If True, fixed depth weighting is allowed.
+    limit_depth_chs : bool
+        If True, use only grad channels for depth weighting. 
+        
+    Returns
+    -------
+    is_free_ori : bool
+        Whether the forward operator is free orientation.
+    info : instance of :py:class:`mne.Info`
+        Measurement info restricted to selected channels.
+    proj : array
+        The SSP/PCA projector.
+    vertno : array
+        The indices of the vertices corresponding to the source space.
+    G : array
+        The forward operator restricted to selected channels.
+    whitener : array  
+        The whitener for the selected channels.
+    nn : array
+        The normals of the source space.
+    orient_std : array
+        The standard deviation of the orientation prior.
     """
     # Lines marked MWW are where code has been changed.
 
     # MWW
     # _check_option('pick_ori', pick_ori, ('normal', 'max-power', 'vector', None))
     _check_option("pick_ori", pick_ori, ("normal", "max-power", "vector", "max-power-pre-weight-norm", None))
```

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d_ds8.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/HarvOxf-sub-Schaefer100-combined-2mm_4d_ds8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/HarvardOxford-sub-prob-bin-2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/HarvardOxford-sub-prob-bin-2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/MNI152_T1_2mm_brain.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/MNI152_T1_2mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/MNI152_T1_8mm_brain.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/MNI152_T1_8mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d_ds8.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d_ds8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds8mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/dk_cortical.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/dk_cortical.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/dk_full.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/dk_full.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fMRI_parcellation_ds2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fMRI_parcellation_ds2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fMRI_parcellation_ds8mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_2mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/files/giles_39_binary.nii.gz` & `osl-0.6.0/osl/source_recon/parcellation/files/giles_39_binary.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/nii.py` & `osl-0.6.0/osl/source_recon/parcellation/nii.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/parcellation/parcellation.py` & `osl-0.6.0/osl/source_recon/parcellation/parcellation.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         Parcellation file (or path to parcellation file).
     voxel_timeseries : numpy.ndarray
         (nvoxels x ntpts) or (nvoxels x ntpts x ntrials) data to be parcellated.
         Data is assumed to be in same space as the parcellation (e.g. typically corresponds to the output from beamforming.transform_recon_timeseries).
     voxel_coords : numpy.ndarray
         (nvoxels x 3) coordinates of voxel_timeseries in mm in same space as parcellation (e.g. typically corresponds to the output from beamforming.transform_recon_timeseries).
     method : str
-        'pca' - take 1st PC in each parcel
-        'spatial_basis' - The parcel time-course for each spatial map is the 1st PC from all voxels, weighted by the spatial map.
+        ``'pca'`` - take 1st PC in each parcel
+        ``'spatial_basis'`` - The parcel time-course for each spatial map is the 1st PC from all voxels, weighted by the spatial map.
         If the parcellation is unweighted and non-overlapping, 'spatialBasis' will give the same result as 'PCA' except with a different normalization.
     working_dir : str
         Directory to put temporary file in. If None, attempt to use same directory as passed in parcellation.
 
     Returns
     -------
     parcel_timeseries : numpy.ndarray
@@ -101,16 +101,16 @@
     Parameters
     ----------
     voxel_timeseries : numpy.ndarray
         (nvoxels x ntpts) or (nvoxels x ntpts x ntrials) and is assumed to be on the same grid as parcellation (typically output by beamforming.transform_recon_timeseries).
     parcellation_asmatrix: numpy.ndarray
         (nvoxels x nparcels) and is assumed to be on the same grid as voxel_timeseries.
     method : str
-        'pca' - take 1st PC of voxels
-        'spatial_basis' - The parcel time-course for each spatial map is the 1st PC from all voxels, weighted by the spatial map.
+        ``'pca'`` - take 1st PC of voxels
+        ``'spatial_basis'`` - The parcel time-course for each spatial map is the 1st PC from all voxels, weighted by the spatial map.
         If the parcellation is unweighted and non-overlapping, 'spatialBasis' will give the same result as 'PCA' except with a different normalization.
 
     Returns
     -------
     parcel_timeseries : numpy.ndarray
         nparcels x ntpts, or nparcels x ntpts x ntrials
     voxel_weightings : numpy.ndarray
@@ -353,16 +353,16 @@
     Returns
     -------
     ortho_timeseries : numpy.ndarray
         (nparcels x ntpts) or (nparcels x ntpts x ntrials) orthoganalised data
     weights : numpy.ndarray
         (optional output depending on compute_weights flag) weighting matrix such that, ortho_timeseries = timeseries * weights
 
-    Notes
-    -----
+    References
+    ----------
     Colclough, G. L., Brookes, M., Smith, S. M. and Woolrich, M. W., "A symmetric multivariate leakage correction for MEG connectomes," NeuroImage 117, pp. 439-448 (2015)
     """
 
     if len(timeseries.shape) == 2:
         # add dim for trials:
         timeseries = np.expand_dims(timeseries, axis=2)
         added_dim = True
@@ -472,20 +472,24 @@
         Low and high frequency in Hz.
     parcellation_file : str
         Path to parcellation file.
     filename : str
         Output filename.
     """
     if parc_ts.ndim == 3:
-        # (parcels, time, epochs) -> (parcels, time)
-        shape = parc_ts.shape
-        parc_ts = parc_ts.reshape(shape[0], shape[1] * shape[2])
+        # Calculate PSD for each epoch individually and average
+        psd = []
+        for i in range(parc_ts.shape[-1]):
+            f, p = welch(parc_ts[..., i], fs=fs)
+            psd.append(p)
+        psd = np.mean(psd, axis=0)
+    else:
+        # Calcualte PSD of continuous data
+        f, psd = welch(parc_ts, fs=fs)
 
-    # Calculate PSD
-    f, psd = welch(parc_ts, fs=fs)
     n_parcels = psd.shape[0]
 
     # Re-order to use colour to indicate anterior->posterior location
     parc_centers = parcel_centers(parcellation_file)
     order = np.argsort(parc_centers[:, 1])
     parc_centers = parc_centers[order]
     psd = psd[order]
@@ -809,23 +813,23 @@
         mne.io.raw object that produced parc_data via source recon and parcellation. Info such as timings and bad segments will be copied from this to parc_raw.
     parcel_names : list of str
         List of strings indicating names of parcels. If None then names are set to be parcel_0,...,parcel_{n_parcels-1}.
 
     Returns
     -------
     parc_epo : mne.Epochs
-        Generated parcellation in mne.Epochs format.
+        Generated parcellation in :py:class: mne.Epochs` format.
     """
 
     # Epochs info
     info = epochs.info
 
     # Create parc info
     if parcel_names is None:
-        parcel_names = [f"parcel_{i}" for i in range(data.shape[0])]
+        parcel_names = [f"parcel_{i}" for i in range(parc_data.shape[0])]
 
     parc_info = mne.create_info(ch_names=parcel_names, ch_types="misc", sfreq=info["sfreq"])
     parc_events = epochs.events
 
     # Parcellated data Epochs object
     parc_epo = mne.EpochsArray(np.swapaxes(parc_data.T, 1, 2), parc_info, parc_events)
```

### Comparing `osl-0.5.1/osl/source_recon/rhino/coreg.py` & `osl-0.6.0/osl/source_recon/rhino/coreg.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,27 @@
 import matplotlib.pyplot as plt
 
 from mne import read_epochs, read_forward_solution
 from mne.viz._3d import _sensor_shape
 from mne.viz.backends.renderer import _get_renderer
 from mne.transforms import write_trans, read_trans, apply_trans, _get_trans, combine_transforms, Transform, rotation, invert_transform
 from mne.forward import _create_meg_coils
-from mne.io import _loc_to_coil_trans, read_info, read_raw, RawArray
-from mne.io.pick import pick_types
+from mne.io import read_info, read_raw, RawArray
+
+try:
+    from mne import pick_types
+except ImportError:
+    # Depreciated in mne 1.6
+    from mne.io.pick import pick_types
+
+try:
+    from mne._fiff.tag import _loc_to_coil_trans
+except ImportError:
+    # Depreciated in mne 1.6
+    from mne.io import _loc_to_coil_trans
 
 from fsl import wrappers as fsl_wrappers
 
 import osl.source_recon.rhino.utils as rhino_utils
 from osl.source_recon.rhino.surfaces import get_surfaces_filenames
 from osl.utils.logger import log_or_print
 
@@ -60,36 +71,44 @@
     use_dev_ctf_t=True,
     already_coregistered=False,
     allow_smri_scaling=False,
     n_init=1,
 ):
     """Coregistration.
 
-    Calculates a linear, affine transform from native sMRI space to polhemus (head) space, using headshape points that include the nose (if useheadshape = True).
-
-    Requires rhino.compute_surfaces to have been run.
-
-    This is based on the OSL Matlab version of RHINO.
-
-    Call get_coreg_filenames(subjects_dir, subject) to get a file list of generated files.
-
-    RHINO firsts registers the polhemus-derived fiducials (nasion, rpa, lpa) in polhemus space to the sMRI-derived fiducials in native sMRI space.
-
-    RHINO then refines this by making use of polhemus-derived headshape points that trace out the surface of the head (scalp), and ideally include the nose.
+    Calculates a linear, affine transform from native sMRI space to 
+    polhemus (head) space, using headshape points that include the 
+    nose (if useheadshape = True). Requires ``rhino.compute_surfaces``
+    to have been run. This is based on the OSL Matlab version of 
+    RHINO.
+    Call ``get_coreg_filenames(subjects_dir, subject)`` to get a file 
+    list of generated files. RHINO firsts registers the polhemus-
+    derived fiducials (nasion, rpa, lpa) in polhemus space to the 
+    sMRI-derived fiducials in native sMRI space.
+
+    RHINO then refines this by making use of polhemus-derived headshape 
+    points that trace out the surface of the head (scalp), and ideally 
+    include the nose.
 
-    Finally, these polhemus-derived headshape points in polhemus space are registered to the sMRI-derived scalp surface in native sMRI space.
+    Finally, these polhemus-derived headshape points in polhemus space 
+    are registered to the sMRI-derived scalp surface in native sMRI space.
 
     In more detail:
+    
     1)  Map location of fiducials in MNI standard space brain to native sMRI space. These are then used as the location of the sMRI-derived fiducials in native sMRI space.
+    
     2a) We have polhemus-derived fids in polhemus space and sMRI-derived fids in native sMRI space. Use these to estimate the affine xform from native sMRI space to polhemus
         (head) space.
+        
     2b) We can also optionally learn the best scaling to add to this affine xform, such that the sMRI-derived fids are scaled in size to better match the polhemus-derived fids.
         This assumes that we trust the size (e.g. in mm) of the polhemus-derived fids, but not the size of sMRI-derived fids. E.g. this might be the case if we do not trust
         the size (e.g. in mm) of the sMRI, or if we are using a template sMRI that would has not come from this subject.
+        
     3)  If a scaling is learnt in step 2, we apply it to sMRI, and to anything derived from sMRI
+    
     4)  Transform sMRI-derived headshape pnts into polhemus space 5)  We have the polhemus-derived headshape points in polhemus space and the sMRI-derived headshape (scalp
         surface) in native sMRI space.  Use these to estimate the affine xform from native sMRI space using the ICP algorithm initilaised using the xform estimate in step 2.
 
     Parameters
     ----------
     fif_file : string
         Full path to MNE-derived fif file.
@@ -592,15 +611,15 @@
     # -----------------
     # Setup MEG sensors
 
     if display_sensors or display_sensor_oris:
 
         meg_picks = pick_types(info, meg=True, ref_meg=False, exclude=())
 
-        coil_transs = [_loc_to_coil_trans(info["chs"][pick]["loc"]) for pick in meg_picks ]
+        coil_transs = [_loc_to_coil_trans(info["chs"][pick]["loc"]) for pick in meg_picks]
         coils = _create_meg_coils([info["chs"][pick] for pick in meg_picks], acc="normal")
 
         meg_rrs, meg_tris, meg_sensor_locs, meg_sensor_oris = (list(), list(), list(), list())
         offset = 0
         for coil, coil_trans in zip(coils, coil_transs):
             rrs, tris = _sensor_shape(coil)
             rrs = apply_trans(coil_trans, rrs)
```

### Comparing `osl-0.5.1/osl/source_recon/rhino/forward_model.py` & `osl-0.6.0/osl/source_recon/rhino/forward_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 
 from mne import make_bem_model, make_bem_solution, make_forward_solution, write_forward_solution
 from mne.bem import ConductorModel, read_bem_solution
 from mne.transforms import read_trans, Transform
 from mne.io import read_info
 from mne.io.constants import FIFF
 from mne.surface import read_surface, write_surface
-from mne.source_space import _make_volume_source_space, _complete_vol_src
+
+try:
+    from mne.source_space import _make_volume_source_space, _complete_vol_src
+except ImportError:
+    # Depreciated in mne 1.6
+    from mne.source_space._source_space import _make_volume_source_space, _complete_vol_src
 
 import osl.source_recon.rhino.utils as rhino_utils
 from osl.source_recon.rhino import get_coreg_filenames
 from osl.utils.logger import log_or_print
 
 
 def forward_model(
@@ -118,21 +123,21 @@
 
     Notes
     -----
     Forward modelling is done in head space.
 
     The coords of points to reconstruct to can be found in the output here:
 
-        fwd['src'][0]['rr'][fwd['src'][0]['vertno']]
+    >>> fwd['src'][0]['rr'][fwd['src'][0]['vertno']]
 
     where they are in head space in metres.
 
     The same coords of points to reconstruct to can be found in the input here:
 
-        src[0]['rr'][src[0]['vertno']]
+    >>> src[0]['rr'][src[0]['vertno']]
 
     where they are in native MRI space in metres.
     """
     filenames = get_coreg_filenames(subjects_dir, subject)
 
     # src should be in MRI space. Let's just check that is the case
     if src[0]["coord_frame"] != FIFF.FIFFV_COORD_MRI:
@@ -207,43 +212,44 @@
     mindist : float
         Exclude points closer than this distance (mm) to the bounding surface.
     exclude : float
         Exclude points closer than this distance (mm) from the center of mass of the bounding surface.
 
     Returns
     -------
-    src : SourceSpaces
+    src : :py:class:`mne.SourceSpaces`
         A single source space object.
 
     See Also
     --------
-    mne.setup_volume_source_space
+    :py:func:`mne.setup_volume_source_space`
+
 
     Notes
     -----
     This is a RHINO specific version of mne.setup_volume_source_space, which can handle smri's that are niftii files.
     This specifically uses the inner skull surface in:
 
-        get_coreg_filenames(subjects_dir, subject)['bet_inskull_surf_file']
+    >>> get_coreg_filenames(subjects_dir, subject)['bet_inskull_surf_file']
 
     to define the source space grid.
 
     This will also copy the:
 
-        get_coreg_filenames(subjects_dir, subject)['bet_inskull_surf_file']
+    >>> get_coreg_filenames(subjects_dir, subject)['bet_inskull_surf_file']
 
     file to:
 
-        subjects_dir/subject/bem/inner_skull.surf
+        ``subjects_dir/subject/bem/inner_skull.surf`
 
     since this is where mne expects to find it when mne.make_bem_model is called.
 
     The coords of points to reconstruct to can be found in the output here:
 
-        src[0]['rr'][src[0]['vertno']]
+    >>> src[0]['rr'][src[0]['vertno']]
 
     where they are in native MRI space in metres.
     """
     filenames = get_coreg_filenames(subjects_dir, subject)
 
     # Note that due to the unusal naming conventions used by BET and MNE:
     # - bet_inskull_*_file is actually the brain surface
```

### Comparing `osl-0.5.1/osl/source_recon/rhino/fsl_utils.py` & `osl-0.6.0/osl/source_recon/rhino/fsl_utils.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/source_recon/rhino/polhemus.py` & `osl-0.6.0/osl/source_recon/rhino/polhemus.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functions related to polhemus fiducials.
 
 """
 
 # Authors: Mark Woolrich <mark.woolrich@ohba.ox.ac.uk>
 #          Chetan Gohil <chetan.gohil@psych.ox.ac.uk>
+#          Mats van Es <mats.vanes@psych.ox.ac.uk>
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from mne.io import read_info
 from mne.io.constants import FIFF
 
@@ -79,14 +80,29 @@
     np.savetxt(nasion_outfile, polhemus_nasion * 1000)
     np.savetxt(rpa_outfile, polhemus_rpa * 1000)
     np.savetxt(lpa_outfile, polhemus_lpa * 1000)
     np.savetxt(headshape_outfile, np.array(polhemus_headshape).T * 1000)
 
 
 def plot_polhemus_points(txt_fnames, colors=None, scales=None, markers=None, alphas=None):
+    """Plot polhemus points.
+    
+    Parameters
+    ----------
+    txt_fnames : list of strings
+        List of filenames containing polhemus points.
+    colors : list of tuples
+        List of colors for each set of points.
+    scales : list of floats
+        List of scales for each set of points.
+    markers : list of strings
+        List of markers for each set of points.
+    alphas : list of floats
+        List of alphas for each set of points.
+    """
     plt.figure()
     ax = plt.axes(projection="3d")
     for ss in range(len(txt_fnames)):
         if alphas is None:
             alpha = 1
         else:
             alpha = alphas[ss]
@@ -138,22 +154,24 @@
     '''
 
     if recon_dir is not None and subject is not None:
         coreg_filenames = get_coreg_filenames(recon_dir, subject)
         polhemus_headshape_file = coreg_filenames["polhemus_headshape_file"]
     elif polhemus_headshape_file is not None:
         polhemus_headshape_file = polhemus_headshape_file
+        coreg_filenames = {'polhemus_headshape_file': polhemus_headshape_file}
     else:
         ValueError('Invalid inputs. See function\'s documentation.')
       
     polhemus_headshape_polhemus = np.loadtxt(polhemus_headshape_file)
 
     print("Num headshape points={}".format(polhemus_headshape_polhemus.shape[1]))
     print('Click on points to delete them.')
     print('Press "w" to write changes to the file')
+    print('Press "q" to close the figure')
     sys.stdout.flush()
 
     def scatter_headshapes(ax, x, y, z):
         # Polhemus-derived headshape points
         color, scale, alpha, marker = "red", 8, 0.7, "o"
         ax.scatter(x, y, z, color=color, marker=marker, s=scale, alpha=alpha, picker=5)
         plt.draw()
@@ -186,13 +204,16 @@
 
     def on_press(event):
         if event.key == 'w':
             polhemus_headshape_polhemus_new = np.array([x, y, z])
             print("Num headshape points remaining={}".format(polhemus_headshape_polhemus_new.shape[1]))
             np.savetxt(coreg_filenames["polhemus_headshape_file"], polhemus_headshape_polhemus_new)
             print('Changes saved to file {}'.format(coreg_filenames["polhemus_headshape_file"]))
+        elif event.key == 'q':
+            print('Closing figure')
+            plt.close(fig)
                     
     # Connect click event to function
     fig.canvas.mpl_connect('pick_event', on_click)
     fig.canvas.mpl_connect('key_press_event', on_press)
 
     plt.show()
```

### Comparing `osl-0.5.1/osl/source_recon/rhino/surfaces.py` & `osl-0.6.0/osl/source_recon/rhino/surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         log_or_print("The nose is not going to be added to the outer skin (scalp) surface")
 
     # Check smri_file
     smri_ext = "".join(Path(smri_file).suffixes)
     if smri_ext not in [".nii", ".nii.gz"]:
         raise ValueError("smri_file needs to be a niftii file with a .nii or .nii.gz extension")
 
-    # Copy smri to new file for modification
+    # Copy sMRI to new file for modification
     img = nib.load(smri_file)
     nib.save(img, filenames["smri_file"])
 
     # RHINO will always use the sform, and so we will set the qform to be same as sform for sMRI,
     # to stop the original qform from being used by mistake (e.g. by flirt)
     #
     # Command: fslorient -copysform2qform <smri_file>
@@ -230,14 +230,22 @@
             "Try running the following from a cmd line: \n   fsleyes {} {} \nAnd see if the standard space brain is shown in the same postcode as the structural.\n"
             "If it is not, then the sformcode in the structural image needs setting correctly.\n".format(filenames["smri_file"], filenames["std_brain"], filenames["smri_file"])
         )
 
     # -------------------------------------------------------
     # 2) Use BET to skull strip sMRI so that flirt works well
 
+    # Check sMRI doesn't contain nans (this can cause segmentation faults with FSL's bet)
+    if rhino_utils._check_nii_for_nan(filenames["smri_file"]):
+        log_or_print("WARNING: nan found in sMRI file. This might cause issues with BET.")
+        old_smri_file = Path(smri_file)
+        new_smri_file = old_smri_file.with_name(old_smri_file.stem + '_fixed' + old_smri_file.suffix)
+        log_or_print("If you encounter an error, it might be possible to fix the file with:")
+        log_or_print(f"fslmaths {old_smri_file} -nan {new_smri_file}")
+
     log_or_print("Running BET pre-FLIRT...")
 
     # Command: bet <flirt_smri_mniaxes_file> <flirt_smri_mniaxes_bet_file>
     flirt_smri_mniaxes_bet_file = op.join(filenames["basedir"], "flirt_smri_mniaxes_bet")
     fsl_wrappers.bet(flirt_smri_mniaxes_file, flirt_smri_mniaxes_bet_file)
 
     # ---------------------------------------------------------
```

### Comparing `osl-0.5.1/osl/source_recon/rhino/utils.py` & `osl-0.6.0/osl/source_recon/rhino/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,23 @@
     # All RHINO files
     files = {"surf": surf_files, "coreg": coreg_files, "fwd_model": op.join(rhino_dir, "model-fwd.fif")}
 
     return files
 
 
 def system_call(cmd, verbose=False):
+    """ Run a system call.
+    
+    Parameters
+    ----------
+    cmd : string
+        Command to run.
+    verbose : bool
+        Print command before running.
+    """
     if verbose:
         log_or_print(cmd)
     subprocess.call(cmd, shell=True)
 
 
 def get_gridstep(coords):
     """Get gridstep (i.e. spatial resolution of dipole grid) in mm.
@@ -268,15 +277,18 @@
     """
 
     sformcode = int(nib.load(nii_file).header["sform_code"])
 
     if sformcode == 1 or sformcode == 4:
         sform = nib.load(nii_file).header.get_sform()
     else:
-        raise ValueError("sform code for {} is {}, and needs to be 4 or 1".format(nii_file, sformcode))
+        raise ValueError(
+            f"sform code for {nii_file} is {sformcode}, and needs to be 4 or 1.\n"
+            "To fix see: https://github.com/OHBA-analysis/osl/blob/main/examples/fix_smri_files.py"
+        )
 
     sform = Transform("mri_voxel", "mri", sform)
     return sform
 
 
 def _get_mni_sform(nii_file):
     """
@@ -286,15 +298,18 @@
     """
 
     sformcode = int(nib.load(nii_file).header["sform_code"])
 
     if sformcode == 1 or sformcode == 4:
         sform = nib.load(nii_file).header.get_sform()
     else:
-        raise ValueError("sform code for {} is {}, and needs to be 4 or 1".format(nii_file, sformcode))
+        raise ValueError(
+            f"sform code for {nii_file} is {sformcode}, and needs to be 4 or 1.\n"
+            "To fix see: https://github.com/OHBA-analysis/osl/blob/main/examples/fix_smri_files.py"
+        )
 
     sform = Transform("unknown", "mni_tal", sform)
     return sform
 
 
 def _get_orient(nii_file):
     cmd = "fslorient -getorient {}".format(nii_file)
@@ -302,14 +317,20 @@
     # use os.popen rather than os.system as we want to return a value, note that this will wait until the read() works before continuing.
     # Without the read() the code will continue without waiting for the system call to finish
     orient = os.popen(cmd).read().strip()
 
     return orient
 
 
+def _check_nii_for_nan(filename):
+    img = nib.load(filename)
+    data = img.get_fdata()
+    return np.isnan(data).any()
+
+
 @cfunc(intc(CPointer(float64), intp, CPointer(float64), voidptr))
 def majority(values_ptr, len_values, result, data):
     """
     def _majority(buffer, required_majority):
        return buffer.sum() >= required_majority
 
     See: https://ilovesymposia.com/2017/03/12/scipys-new-lowlevelcallable-is-a-game-changer/
@@ -1069,15 +1090,28 @@
         write_surface(surf_outfile, rrs_native, tris_native, file_format="freesurfer", overwrite=True)
 
     else:
         raise ValueError("Invalid infile. Needs to be a .nii.gz or .vtk file")
 
 
 def _transform_bet_surfaces(flirt_xform_file, mne_xform_file, filenames, smri_file):
-
+    """Transforms bet surfaces into mne space.
+    
+    Parameters
+    ----------
+    flirt_xform_file : string
+        Path to flirt xform file.
+    mne_xform_file : string
+        Path to mne xform file.
+    filenames : dict
+        Dictionary containing filenames.
+    smri_file : string
+        Path to structural MRI file.
+    """
+    
     # Transform betsurf mask/mesh using passed in flirt transform and mne transform
     for mesh_name in {"outskin_mesh", "inskull_mesh", "outskull_mesh"}:
         # xform mask
         # Command: flirt -in <flirt_mesh_file> -ref <smri_file> -interp nearestneighbour -applyxfm -init <flirt_xform_file> -out <out_file>
         fsl_wrappers.flirt(
             op.join(filenames["basedir"], "flirt_" + mesh_name + ".nii.gz"),
             smri_file,
```

### Comparing `osl-0.5.1/osl/source_recon/sign_flipping.py` & `osl-0.6.0/osl/source_recon/sign_flipping.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         metric = covariance_matrix_correlation(cov, template_cov, n_embeddings)
         if n == 0:
             metrics.append(metric)
             log_or_print(f"init {n}, unflipped metric: {metric}")
 
         # Randomly permute the sign of different channels and calculate the metric
         if use_tqdm:
-            iterator = trange(n_iter, desc="sign flipping", ncols=98)
+            iterator = trange(n_iter, desc="sign flipping")
         else:
             iterator = range(n_iter)
         for j in iterator:
             new_flips = randomly_flip(flips, max_flips)
             new_cov = apply_flips_to_covariance(cov, new_flips, n_embeddings)
             new_metric = covariance_matrix_correlation(new_cov, template_cov, n_embeddings)
             if new_metric > metric:
@@ -138,15 +138,15 @@
     Returns
     -------
     covs : numpy.ndarray
         Covariance matrices.
     """
     covs = []
     if use_tqdm:
-        iterator = trange(len(parc_files), desc="Calculating covariances", ncols=98)
+        iterator = trange(len(parc_files), desc="Calculating covariances")
     else:
         iterator = range(len(parc_files))
     for i in iterator:
         # Load data
         if loader is not None:
             # Use the loader that has been passed
             x = loader(parc_files[i])
@@ -191,15 +191,15 @@
     -------
     index : int
         Index for the template subject.
     """
     # Calculate the similarity between subjects
     n_subjects = len(covs)
     metric = np.zeros([n_subjects, n_subjects])
-    for i in trange(n_subjects, desc="Comparing subjects", ncols=98):
+    for i in trange(n_subjects, desc="Comparing subjects"):
         for j in range(i + 1, n_subjects):
             metric[i, j] = covariance_matrix_correlation(covs[i], covs[j], diag_offset, mode="abs")
             metric[j, i] = metric[i, j]
 
     # Get the median subject
     metric_sum = np.sum(metric, axis=1)
     argmedian = np.argsort(metric_sum)[len(metric_sum) // 2]
```

### Comparing `osl-0.5.1/osl/source_recon/wrappers.py` & `osl-0.6.0/osl/source_recon/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,14 +407,15 @@
     subject,
     preproc_file,
     smri_file,
     epoch_file,
     freq_range,
     chantypes,
     rank,
+    reg=0,
 ):
     """Wrapper function for beamforming.
 
     Parameters
     ----------
     src_dir : str
         Path to where to output the source reconstruction files.
@@ -429,14 +430,16 @@
     freq_range : list
         Lower and upper band to bandpass filter before beamforming. If None,
         no filtering is done.
     chantypes : str or list of str
         Channel types to use in beamforming.
     rank : dict
         Keys should be the channel types and the value should be the rank to use.
+    reg : float
+        The regularization for the whitened data covariance.
     """
     logger.info("beamforming")
 
     if isinstance(chantypes, str):
         chantypes = [chantypes]
 
     # Load sensor-level data
@@ -466,14 +469,15 @@
     filters = beamforming.make_lcmv(
         subjects_dir=src_dir,
         subject=subject,
         data=data,
         chantypes=chantypes,
         weight_norm="nai",
         rank=rank,
+        reg=reg,
         save_filters=True,
     )
 
     # Make plots
     filters_cov_plot, filters_svd_plot = beamforming.make_plots(src_dir, subject, filters, data)
     filters_cov_plot = filters_cov_plot.replace(f"{src_dir}/", "")
     filters_svd_plot = filters_svd_plot.replace(f"{src_dir}/", "")
@@ -481,14 +485,15 @@
     # Save info for the report
     src_report.add_to_data(
         f"{src_dir}/{subject}/report_data.pkl",
         {
             "beamform": True,
             "chantypes": chantypes,
             "rank": rank,
+            "reg": reg,
             "freq_range": freq_range,
             "filters_cov_plot": filters_cov_plot,
             "filters_svd_plot": filters_svd_plot,
         },
     )
 
 
@@ -661,14 +666,15 @@
     freq_range,
     parcellation_file,
     method,
     orthogonalisation,
     spatial_resolution=None,
     reference_brain="mni",
     extra_chans="stim",
+    reg=0,
 ):
     """Wrapper function for beamforming and parcellation.
 
     Parameters
     ----------
     src_dir : str
         Path to where to output the source reconstruction files.
@@ -700,14 +706,16 @@
         'mri' indicates that the reference_brain is the subject's sMRI in the scaled native/mri space.
         'unscaled_mri' indicates that the reference_brain is the subject's sMRI in unscaled native/mri space.
         Note that Scaled/unscaled relates to the allow_smri_scaling option in coreg.
         If allow_scaling was False, then the unscaled MRI will be the same as the scaled MRI.
     extra_chans : str or list of str
         Extra channels to include in the parc-raw.fif file. Defaults to 'stim'.
         Stim channels are always added to parc-raw.fif in addition to extra_chans.
+    reg : float
+        The regularization for the whitened data covariance in the beamforming stage.
     """
     logger.info("beamform_and_parcellate")
 
     if isinstance(chantypes, str):
         chantypes = [chantypes]
 
     # Load sensor-level data
@@ -737,14 +745,15 @@
     filters = beamforming.make_lcmv(
         subjects_dir=src_dir,
         subject=subject,
         data=chantype_data,
         chantypes=chantypes,
         weight_norm="nai",
         rank=rank,
+        reg=reg,
         save_filters=True,
     )
 
     # Make plots
     filters_cov_plot, filters_svd_plot = beamforming.make_plots(src_dir, subject, filters, chantype_data)
     filters_cov_plot = filters_cov_plot.replace(f"{src_dir}/", "")
     filters_svd_plot = filters_svd_plot.replace(f"{src_dir}/", "")
@@ -819,14 +828,15 @@
         f"{src_dir}/{subject}/report_data.pkl",
         {
             "beamform_and_parcellate": True,
             "beamform": True,
             "parcellate": True,
             "chantypes": chantypes,
             "rank": rank,
+            "reg": reg,
             "freq_range": freq_range,
             "filters_cov_plot": filters_cov_plot,
             "filters_svd_plot": filters_svd_plot,
             "parcellation_file": parcellation_file,
             "method": method,
             "orthogonalisation": orthogonalisation,
             "parc_fif_file": str(parc_fif_file),
```

### Comparing `osl-0.5.1/osl/tests/test_00_package_canary.py` & `osl-0.6.0/osl/tests/test_00_package_canary.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/tests/test_batch_api.py` & `osl-0.6.0/osl/tests/test_batch_api.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/tests/test_batch_preproc.py` & `osl-0.6.0/osl/tests/test_batch_preproc.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,14 +45,37 @@
 
         dataset = run_proc_chain(cfg, self.fpath)
 
         # Just testing that things run not that the outputs are sensible...
         assert(isinstance(dataset["raw"], mne.io.fiff.raw.Raw))
 
 
+class TestVersions(unittest.TestCase):
+    def test_simple_chain(self):
+        from ..preprocessing import load_config, check_config_versions
+
+        cfg = """
+        meta:
+          event_codes:
+          version_assert: 
+          version_warn: 
+        preproc:
+          - filter:         {l_freq: 1, h_freq: 30}
+          - notch_filter:   {freqs: 50}
+          - bad_channels:   {picks: 'grad'}
+          - bad_segments:   {segment_len: 800, picks: 'grad'}
+        """
+        config = load_config(cfg)
+
+        config['meta']['version_assert'] = ['numpy>1.0', 'scipy>1.0']
+        config['meta']['version_warn'] = ['mne>1.0']
+
+        check_config_versions(config)
+
+
 class TestPreprocessingBatch(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         from ..utils import simulate_raw_from_template
 
         cls.infiles = []
```

### Comparing `osl-0.5.1/osl/tests/test_file_handling.py` & `osl-0.6.0/osl/tests/test_file_handling.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/tests/test_parallel.py` & `osl-0.6.0/osl/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/create_neuromag306_info.py` & `osl-0.6.0/osl/utils/create_neuromag306_info.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/file_handling.py` & `osl-0.6.0/osl/utils/file_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 infiles = [sanitise_filepath(f) for f in inputs]
                 outnames = [find_run_id(f) for f in infiles]
             elif isinstance(inputs[0], (list, tuple)):
                 # We have a list containing files and output names
                 for row in inputs:
                     infiles.append(sanitise_filepath(row[0]))
                     outnames.append(row[1])
-            elif isinstance(inputs[0], mne.io.fiff.raw.Raw):
+            elif isinstance(inputs[0], mne.io.Raw):
                 # We have a list of MNE objects
                 infiles = infiles
                 check_paths = False
         else:
             raise ValueError("Input type is invalid")
 
     # Check that files actually exist if we've been passed filenames rather
@@ -121,15 +121,15 @@
 
 def find_run_id(infile, preload=True):
 
     # TODO: This is perhaps more complex than it needs to be - could just use
     # the fif option for everything except BTI scans? They're basically the
     # same now.
 
-    if isinstance(infile, mne.io.fiff.raw.Raw):
+    if isinstance(infile, mne.io.Raw):
         infile = infile.filenames[0]
 
     if os.path.split(infile)[1] == 'c,rfDC':
         # We have a BTI scan
         runname = os.path.basename(os.path.dirname(infile))
     elif os.path.splitext(infile)[1] == '.fif':
         # We have a FIF file
```

### Comparing `osl-0.5.1/osl/utils/logger.py` & `osl-0.6.0/osl/utils/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,25 +102,45 @@
         osl_logger.info('logging to file: {0}'.format(log_file))
 
     # Attribute to let us know if we have setup the OSL logger
     osl_logger.already_setup = True
 
 
 def set_level(level, handler='console'):
-    """Set new logging level for OSL module."""
+    """Set new logging level for OSL module.
+    
+    Parameters
+    ----------
+    level : {'CRITICAL', 'WARNING', 'INFO', 'DEBUG'}
+        String indicating new logging level
+    handler : str
+        The handler to set the level for. Defaults to 'console'.
+    """
     osl_logger = logging.getLogger('osl')
     for handler in osl_logger.handlers:
         if handler.get_name() == 'console':
             if level in ['INFO', 'DEBUG']:
                 osl_logger.info("OSL osl_logger: handler '{0}' level set to '{1}'".format(handler.get_name(), level))
             handler.setLevel(getattr(logging, level))
 
 
 def get_level(handler='console'):
-    """Return current logging level for OSL module."""
+    """Return current logging level for OSL module.
+    
+    Parameters
+    ----------
+    handler : str
+        The handler to get the level for. Defaults to 'console'.
+        
+    Returns
+    -------
+    level : {'CRITICAL', 'WARNING', 'INFO', 'DEBUG'}
+        String indicating current logging level
+    
+    """
     osl_logger = logging.getLogger('osl')
     for handler in osl_logger.handlers:
         if handler.get_name() == 'console':
             return handler.level
 
 
 def log_or_print(msg, warning=False):
```

### Comparing `osl-0.5.1/osl/utils/neuromag306_info.yml` & `osl-0.6.0/osl/utils/neuromag306_info.yml`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/opm.py` & `osl-0.6.0/osl/utils/opm.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,56 @@
 import os.path
 from shutil import copyfile
 import nibabel as nib
 
 import numpy as np
 
 import mne
-from mne.io import _coil_trans_to_loc
 from mne.io.constants import FIFF
 from mne.transforms import Transform, apply_trans
 
+try:
+    from mne._fiff.tag import _coil_trans_to_loc
+except ImportError:
+    # Depreciated in mne 1.6
+    from mne.io import _coil_trans_to_loc
+
 import pandas as pd
 import scipy
 
 # -------------------------------------------------------------
 # %% Get sensor locations and orientations from tsv file
 
 def convert_notts(notts_opm_mat_file, smri_file, tsv_file, fif_file, smri_fixed_file):
-
+    """ Convert Nottingham OPM data from matlab file to fif file.
+    
+    Parameters
+    ----------
+    notts_opm_mat_file : str
+        The matlab file containing the OPM data.
+    smri_file : str
+        The structural MRI file.
+    tsv_file : str
+        The tsv file containing the sensor locations and orientations.
+    fif_file : str
+        The output fif file.
+    smri_fixed_file : str
+        The output structural MRI file with corrected sform.
+        
+    Notes
+    -----
+    The matlab file is assumed to contain a variable called 'data' which is
+    a matrix of size nSamples x nChannels.
+    The matlab file is assumed to contain a variable called 'fs' which is
+    the sampling frequency.
+    The tsv file is assumed to contain a header row, and the following columns:
+    name, type, bad, x, y, z, qx, qy, qz
+    The x,y,z columns are the sensor locations in metres.
+    The qx,qy,qz columns are the sensor orientations in metres.
+    """
     # correct sform for smri
     sform_std_fixed = correct_mri(smri_file, smri_fixed_file)
 
     # Note that later in this function, we will also apply this sform to
     # the sensor coordinates and orientations.
     # This is because, with the OPM Notts data, coregistration on the sensor coordinates
     # has already been carried out, and so the sensor coordinates need to stay matching 
@@ -166,15 +196,34 @@
 
     # FINALLY put data and info together and save to fif_file
     data = scipy.io.loadmat(notts_opm_mat_file)['data'].T * 1e-15  # fT
     raw = mne.io.RawArray(data, info)
     raw.save(fif_file, overwrite=True)
 
 def correct_mri(smri_file, smri_fixed_file):
+    """Correct the sform in the structural MRI file.
+
+    Parameters
+    ----------
+    smri_file : str
+        The structural MRI file.
+    smri_fixed_file : str
+        The output structural MRI file with corrected sform.
+        
+        
+    Returns
+    -------
+    sform_std : ndarray
+        The new sform.
+        
+    Notes
+    -----
+    The sform is corrected so that it is in standard orientation.
 
+    """
     # Copy smri_name to new file for modification
     copyfile(smri_file, smri_fixed_file)
 
     smri = nib.load(smri_fixed_file)
     sform = smri.header.get_sform()
     sform_std = np.copy(sform)
 
@@ -186,18 +235,17 @@
     sform_std[1, 0:4] = [0, -1, 0, 126]
     sform_std[2, 0:4] = [0, 0, -1, 72]
     
     os.system('fslorient -setsform {} {}'.format(' '.join(map(str, sform_std.flatten())), smri_fixed_file))
 
     return sform_std
 
-#########################################################################
-
 # -------------------------------------------------------------
 # %% Debug and plotting code for checking sensor locs and oris
+
 if False:
 
     from mne.io.pick import pick_types
     from mne.io import _loc_to_coil_trans
     from mne.viz._3d import _sensor_shape
     from mne.forward import _create_meg_coils
     from mne.transforms import apply_trans, read_trans, combine_transforms, _get_trans, invert_transform
```

### Comparing `osl-0.5.1/osl/utils/package.py` & `osl-0.6.0/osl/utils/package.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/parallel.py` & `osl-0.6.0/osl/utils/parallel.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,37 @@
 # Housekeeping for logging
 import logging
 osl_logger = logging.getLogger(__name__)
 
 
 def dask_parallel_bag(func, iter_args,
                       func_args=None, func_kwargs=None):
-    """A maybe more consistent alternative to dask_parallel."""
+    """A maybe more consistent alternative to ``dask_parallel``.
+    
+    Parameters
+    ---------
+    func : function
+        The function to run in parallel.
+    iter_args : list
+        A list of iterables to pass to func.
+    func_args : list, optional
+        A list of positional arguments to pass to func.
+    func_kwargs : dict, optional
+        A dictionary of keyword arguments to pass to func.
+    
+    Returns
+    -------
+    flags : list
+        A list of return values from func.
+        
+    References
+    ----------
+    https://docs.dask.org/en/stable/bag.html
+    
+    """
 
     func_args = [] if func_args is None else func_args
     func_kwargs = {} if func_kwargs is None else func_kwargs
 
     # Get connection to currently active cluster
     client = default_client()
```

### Comparing `osl-0.5.1/osl/utils/simulation_config/megin_template_info.fif` & `osl-0.6.0/osl/utils/simulation_config/megin_template_info.fif`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/simulation_config/reduced_mvar_params_grad.npy` & `osl-0.6.0/osl/utils/simulation_config/reduced_mvar_params_grad.npy`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/simulation_config/reduced_mvar_params_mag.npy` & `osl-0.6.0/osl/utils/simulation_config/reduced_mvar_params_mag.npy`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/simulation_config/reduced_mvar_pcacomp_grad.npy` & `osl-0.6.0/osl/utils/simulation_config/reduced_mvar_pcacomp_grad.npy`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/simulation_config/reduced_mvar_pcacomp_mag.npy` & `osl-0.6.0/osl/utils/simulation_config/reduced_mvar_pcacomp_mag.npy`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/simulation_config/reduced_mvar_residcov_grad.npy` & `osl-0.6.0/osl/utils/simulation_config/reduced_mvar_residcov_grad.npy`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/simulation_config/reduced_mvar_residcov_mag.npy` & `osl-0.6.0/osl/utils/simulation_config/reduced_mvar_residcov_mag.npy`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/spmio/_data.py` & `osl-0.6.0/osl/utils/spmio/_data.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/spmio/_events.py` & `osl-0.6.0/osl/utils/spmio/_events.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl/utils/spmio/spmmeeg.py` & `osl-0.6.0/osl/utils/spmio/spmmeeg.py`

 * *Files identical despite different names*

### Comparing `osl-0.5.1/osl.egg-info/SOURCES.txt` & `osl-0.6.0/osl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 osl/maxfilter/maxfilter.py
 osl/preprocessing/__init__.py
 osl/preprocessing/batch.py
 osl/preprocessing/mne_wrappers.py
 osl/preprocessing/osl_wrappers.py
 osl/preprocessing/plot_ica.py
 osl/report/__init__.py
-osl/report/phantom-report.py
-osl/report/phantom-trigger.py
-osl/report/raw_report.py
+osl/report/preproc_report.py
 osl/report/src_report.py
 osl/report/templates/raw_subject_panel.html
 osl/report/templates/raw_summary_panel.html
 osl/report/templates/src_subject_panel.html
 osl/report/templates/src_summary_panel.html
 osl/report/templates/subject_report.html
 osl/report/templates/summary_report.html
@@ -49,14 +47,15 @@
 osl/source_recon/parcellation/files/MNI152_T1_2mm_brain.nii.gz
 osl/source_recon/parcellation/files/MNI152_T1_8mm_brain.nii.gz
 osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm.nii.gz
 osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d.nii.gz
 osl/source_recon/parcellation/files/Schaefer2018_100Parcels_7Networks_order_FSLMNI152_2mm_4d_ds8.nii.gz
 osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds2mm.nii.gz
 osl/source_recon/parcellation/files/WTA_fMRI_parcellation_ds8mm.nii.gz
+osl/source_recon/parcellation/files/aal_cortical_merged_8mm_stacked.nii.gz
 osl/source_recon/parcellation/files/dk_cortical.nii.gz
 osl/source_recon/parcellation/files/dk_full.nii.gz
 osl/source_recon/parcellation/files/fMRI_parcellation_ds2mm.nii.gz
 osl/source_recon/parcellation/files/fMRI_parcellation_ds8mm.nii.gz
 osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm.nii.gz
 osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
 osl/source_recon/parcellation/files/fmri_d100_parcellation_with_PCC_tighterMay15_v2_2mm.nii.gz
@@ -71,25 +70,28 @@
 osl/source_recon/rhino/surfaces.py
 osl/source_recon/rhino/utils.py
 osl/tests/__init__.py
 osl/tests/test_00_package_canary.py
 osl/tests/test_batch_api.py
 osl/tests/test_batch_preproc.py
 osl/tests/test_file_handling.py
+osl/tests/test_glm.py
 osl/tests/test_parallel.py
 osl/utils/__init__.py
 osl/utils/create_neuromag306_info.py
 osl/utils/file_handling.py
 osl/utils/logger.py
 osl/utils/neuromag306_info.yml
 osl/utils/opm.py
 osl/utils/package.py
 osl/utils/parallel.py
+osl/utils/run_func.py
 osl/utils/simulate.py
 osl/utils/study.py
+osl/utils/version_utils.py
 osl/utils/simulation_config/megin_template_info.fif
 osl/utils/simulation_config/reduced_mvar_params_grad.npy
 osl/utils/simulation_config/reduced_mvar_params_mag.npy
 osl/utils/simulation_config/reduced_mvar_pcacomp_grad.npy
 osl/utils/simulation_config/reduced_mvar_pcacomp_mag.npy
 osl/utils/simulation_config/reduced_mvar_residcov_grad.npy
 osl/utils/simulation_config/reduced_mvar_residcov_mag.npy
```

### Comparing `osl-0.5.1/setup.py` & `osl-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # Requirement categories
-reqs = ['numpy', 'scipy', 'matplotlib', 'mne>=1.0.0', 'scikit-learn', 'fslpy',
-        'sails', 'tabulate', 'pyyaml>=5.1', 'neurokit2', 'jinja2',
+reqs = ['numpy', 'scipy', 'matplotlib', 'mne~=1.3.1', 'scikit-learn', 'fslpy',
+        'sails', 'tabulate', 'pyyaml>=5.1', 'neurokit2', 'jinja2==3.0.3',
         'glmtools', 'numba', 'nilearn', 'dask', 'distributed', 'parse',
         'opencv-python', 'panel', 'h5io']
 doc_reqs = ['sphinx==4.0.2', 'numpydoc', 'sphinx_gallery', 'pydata-sphinx-theme']
 dev_reqs = ['setuptools>=41.0.1', 'pytest', 'pytest-cov', 'coverage', 'flake8']
 
 name = 'osl'
 
 setup(name=name,
-      version='0.5.1',
+      version='0.6.0',
       description='OHBA Software Library',
       long_description=README,
       long_description_content_type="text/markdown",
       author='OHBA Analysis Group',
       license='MIT',
 
       # Choose your license
@@ -55,14 +55,15 @@
       },
 
       zip_safe=False,
       entry_points={
           'console_scripts': [
               'osl_maxfilter = osl.maxfilter.maxfilter:main',
               'osl_preproc = osl.preprocessing.batch:main',
+              'osl_func = osl.utils.run_func:main',
           ]},
 
       packages=['osl', 'osl.tests', 'osl.report', 'osl.maxfilter',
                 'osl.preprocessing', 'osl.utils', 'osl.utils.spmio',
                 'osl.source_recon', 'osl.source_recon.rhino',
                 'osl.source_recon.parcellation', 'osl.glm'],
```

