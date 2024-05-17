# Comparing `tmp/pydra_fsl-0.0.9.tar.gz` & `tmp/pydra_fsl-0.1.0.tar.gz`

## Comparing `pydra_fsl-0.0.9.tar` & `pydra_fsl-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,505 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/.editorconfig
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/.github/dependabot.yaml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/.github/workflows/test.yaml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/__init__.py
--rw-r--r--   0        0        0    12486 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/eddy.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/fast.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/fnirt.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/fslmaths.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/fslmerge.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/fslreorient2std.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/fslroi.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/susan.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/bet/__init__.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/bet/bet.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/bet/robustfov.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/apply_xfm.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/concat_xfm.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/convert_xfm.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/flirt.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/invert_xfm.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/specs.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/LICENSE
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/hatch.toml
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 pydra_fsl-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.coveragerc
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.editorconfig
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.flake8
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.gitattributes
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/codecov.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/report_progress.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.github/workflows/ci-cd.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/source/index.rst
+-rwxr-xr-x   0        0        0     2504 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/generate
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/requirements.txt
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/accuracy_tester.yaml
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/accuracy_tester_callables.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_mask.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_mask_callables.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_topup.yaml
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_topup_callables.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_warp.yaml
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_warp_callables.py
+-rw-r--r--   0        0        0    10616 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_xfm.yaml
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_xfm_callables.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ar1_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ar1_image_callables.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/av_scale.yaml
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/av_scale_callables.py
+-rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/b0_calc.yaml
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/b0_calc_callables.py
+-rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bedpostx5.yaml
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bedpostx5_callables.py
+-rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bet.yaml
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bet_callables.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/binary_maths.yaml
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/binary_maths_callables.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/change_data_type.yaml
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/change_data_type_callables.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/classifier.yaml
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/classifier_callables.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cleaner.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cleaner_callables.py
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cluster.yaml
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cluster_callables.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/complex.yaml
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/complex_callables.py
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/contrast_mgr.yaml
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/contrast_mgr_callables.py
+-rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_warp.yaml
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_warp_callables.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_xfm.yaml
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_xfm_callables.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/copy_geom.yaml
+-rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/copy_geom_callables.py
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dilate_image.yaml
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dilate_image_callables.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/distance_map.yaml
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/distance_map_callables.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dti_fit.yaml
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dti_fit_callables.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dual_regression.yaml
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dual_regression_callables.py
+-rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy.yaml
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_callables.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_correct.yaml
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_correct_callables.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_quad.yaml
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_quad_callables.py
+-rw-r--r--   0        0        0     8763 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_de_warp.yaml
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_de_warp_callables.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_reg.yaml
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_reg_callables.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/erode_image.yaml
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/erode_image_callables.py
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/extract_roi.yaml
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/extract_roi_callables.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fast.yaml
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fast_callables.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat.yaml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_callables.py
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_model.yaml
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_model_callables.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feature_extractor.yaml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feature_extractor_callables.py
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filmgls.yaml
+-rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filmgls_callables.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filter_regressor.yaml
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filter_regressor_callables.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/find_the_biggest.yaml
+-rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/find_the_biggest_callables.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/first.yaml
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/first_callables.py
+-rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flameo.yaml
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flameo_callables.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flirt.yaml
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flirt_callables.py
+-rw-r--r--   0        0        0    14632 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fnirt.yaml
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fnirt_callables.py
+-rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fugue.yaml
+-rw-r--r--   0        0        0    10616 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fugue_callables.py
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/glm.yaml
+-rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/glm_callables.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ica__aroma.yaml
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ica__aroma_callables.py
+-rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_maths.yaml
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_maths_callables.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_meants.yaml
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_meants_callables.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_stats.yaml
+-rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_stats_callables.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/inv_warp.yaml
+-rw-r--r--   0        0        0     9982 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/inv_warp_callables.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/isotropic_smooth.yaml
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/isotropic_smooth_callables.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/l2_model.yaml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/l2_model_callables.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/level_1_design.yaml
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/level_1_design_callables.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/make_dyadic_vectors.yaml
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/make_dyadic_vectors_callables.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maths_command.yaml
+-rw-r--r--   0        0        0     9162 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maths_command_callables.py
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/max_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/max_image_callables.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maxn_image.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maxn_image_callables.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mcflirt.yaml
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mcflirt_callables.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mean_image.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mean_image_callables.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/median_image.yaml
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/median_image_callables.py
+-rw-r--r--   0        0        0    14386 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/melodic.yaml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/melodic_callables.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/merge.yaml
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/merge_callables.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/min_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/min_image_callables.py
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/motion_outliers.yaml
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/motion_outliers_callables.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multi_image_maths.yaml
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multi_image_maths_callables.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multiple_regress_design.yaml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multiple_regress_design_callables.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/overlay.yaml
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/overlay_callables.py
+-rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/percentile_image.yaml
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/percentile_image_callables.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_motion_params.yaml
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_motion_params_callables.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_time_series.yaml
+-rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_time_series_callables.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/power_spectrum.yaml
+-rw-r--r--   0        0        0     9443 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/power_spectrum_callables.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prelude.yaml
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prelude_callables.py
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prepare_fieldmap.yaml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prepare_fieldmap_callables.py
+-rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x.yaml
+-rw-r--r--   0        0        0    16132 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x2.yaml
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x2_callables.py
+-rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x_callables.py
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/proj_thresh.yaml
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/proj_thresh_callables.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/randomise.yaml
+-rw-r--r--   0        0        0    11553 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/randomise_callables.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/reorient_2_std.yaml
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/reorient_2_std_callables.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/robust_fov.yaml
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/robust_fov_callables.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/sig_loss.yaml
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/sig_loss_callables.py
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice.yaml
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_callables.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_timer.yaml
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_timer_callables.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slicer.yaml
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slicer_callables.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smm.yaml
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smm_callables.py
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth.yaml
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_callables.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_estimate.yaml
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_estimate_callables.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/spatial_filter.yaml
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/spatial_filter_callables.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/split.yaml
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/split_callables.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/std_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/std_image_callables.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/susan.yaml
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/susan_callables.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/swap_dimensions.yaml
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/swap_dimensions_callables.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/temporal_filter.yaml
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/temporal_filter_callables.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/text_2_vest.yaml
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/text_2_vest_callables.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/threshold.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/threshold_callables.py
+-rw-r--r--   0        0        0    12627 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/topup.yaml
+-rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/topup_callables.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/tract_skeleton.yaml
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/tract_skeleton_callables.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training.yaml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training_callables.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training_set_creator.yaml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training_set_creator_callables.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/unary_maths.yaml
+-rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/unary_maths_callables.py
+-rw-r--r--   0        0        0     9481 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vec_reg.yaml
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vec_reg_callables.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vest_2_text.yaml
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vest_2_text_callables.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points.yaml
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_callables.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_from_std.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_from_std_callables.py
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_to_std.yaml
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_to_std_callables.py
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_utils.yaml
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_utils_callables.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/x_fibres_5.yaml
+-rw-r--r--   0        0        0    12428 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/x_fibres_5_callables.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/_version.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/latest.py
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/_version.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/accuracy_tester.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_mask.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_topup.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_warp.py
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_xfm.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/ar1_image.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/av_scale.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/b0_calc.py
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/bedpostx5.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/bet.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/binary_maths.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/change_data_type.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/classifier.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/cleaner.py
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/cluster.py
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/complex.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/contrast_mgr.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/convert_warp.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/convert_xfm.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/copy_geom.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dilate_image.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/distance_map.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dti_fit.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dual_regression.py
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy_correct.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy_quad.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/epi_de_warp.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/epi_reg.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/erode_image.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/extract_roi.py
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fast.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feat.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feat_model.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feature_extractor.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/filmgls.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/filter_regressor.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/find_the_biggest.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/first.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/flameo.py
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/flirt.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fnirt.py
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fugue.py
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/glm.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/ica__aroma.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_maths.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_meants.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_stats.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/inv_warp.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/isotropic_smooth.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/l2_model.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/level_1_design.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/make_dyadic_vectors.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/maths_command.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/max_image.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/maxn_image.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/mcflirt.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/mean_image.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/median_image.py
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/melodic.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/merge.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/min_image.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/motion_outliers.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/multi_image_maths.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/multiple_regress_design.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/overlay.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/percentile_image.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/plot_motion_params.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/plot_time_series.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/power_spectrum.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prelude.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prepare_fieldmap.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prob_track_x.py
+-rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prob_track_x2.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/proj_thresh.py
+-rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/randomise.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/reorient_2_std.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/robust_fov.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/sig_loss.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice_timer.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slicer.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smm.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smooth.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smooth_estimate.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/spatial_filter.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/split.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/std_image.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/susan.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/swap_dimensions.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/temporal_filter.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/text_2_vest.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/threshold.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/topup.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tract_skeleton.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/training.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/training_set_creator.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/unary_maths.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/vec_reg.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/vest_2_text.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points_from_std.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points_to_std.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_utils.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/x_fibres_5.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/conftest.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_accuracytester.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applymask.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applytopup.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applywarp.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applyxfm.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_ar1image.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_avscale.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_b0calc.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_bedpostx5.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_bet.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_binarymaths.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_changedatatype.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_classifier.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_cleaner.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_cluster.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_complex.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_contrastmgr.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_convertwarp.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_convertxfm.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_copygeom.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dilateimage.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_distancemap.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dtifit.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dualregression.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddy.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddycorrect.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddyquad.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_epidewarp.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_epireg.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_erodeimage.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_extractroi.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fast.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_feat.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_featmodel.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_featureextractor.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_filmgls.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_filterregressor.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_findthebiggest.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_first.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_flameo.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_flirt.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fnirt.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fugue.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_glm.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_ica_aroma.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagemaths.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagemeants.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagestats.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_invwarp.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_isotropicsmooth.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_l2model.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_level1design.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_makedyadicvectors.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_mathscommand.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_maximage.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_maxnimage.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_mcflirt.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_meanimage.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_medianimage.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_melodic.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_merge.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_minimage.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_motionoutliers.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_multiimagemaths.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_multipleregressdesign.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_overlay.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_percentileimage.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_plotmotionparams.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_plottimeseries.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_powerspectrum.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_prelude.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_preparefieldmap.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_probtrackx.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_probtrackx2.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_projthresh.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_randomise.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_reorient2std.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_robustfov.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_sigloss.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slice.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slicer.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slicetimer.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smm.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smooth.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smoothestimate.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_spatialfilter.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_split.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_stdimage.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_susan.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_swapdimensions.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_temporalfilter.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_text2vest.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_threshold.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_topup.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_tractskeleton.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_training.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_trainingsetcreator.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_unarymaths.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_vecreg.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_vest2text.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppoints.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppointsfromstd.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppointstostd.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warputils.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_xfibres5.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/__init__.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fast.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/maths.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/susan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/__init__.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/bet.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/robustfov.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/__init__.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/applytopup.py
+-rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/eddy.py
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/topup.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/__init__.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/convertxfm.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/flirt.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/img2imgcoord.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/img2stdcoord.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/specs.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/std2imgcoord.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/applywarp.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/convertwarp.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirt.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirtfileutils.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/invwarp.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/specs.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/__init__.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/fugue.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/prelude.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/prepare_fieldmap.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/sigloss.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/__init__.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/chfiletype.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/fft.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/info.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/interleave.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/merge.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/orient.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/reorient2std.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/roi.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/selectvols.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/smoothfill.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/split.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/swapdim.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/conftest.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/fileformats/medimage_fsl/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/fileformats/extras/medimage_fsl/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/fileformats/extras/medimage_fsl/tests/test_generate_sample_data.py
+-rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/increment_tool_version.py
+-rwxr-xr-x   0        0        0     1368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/rename_template.py
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/report_progress.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/requirements.txt
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/LICENSE
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/NOTICE
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/README.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/PKG-INFO
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/eddy.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/eddy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,438 +1,429 @@
 """
-eddy
+Eddy
 ====
 
 Correct for artifacts induced by Eddy currents and subject motion.
+
+Examples
+--------
+
+>>> task = Eddy(
+...     input_image="input.nii",
+...     brain_mask="brain.nii",
+...     encoding_file="params.txt",
+...     index_file="index.txt",
+...     bvec_file="input.bvec",
+...     bval_file="input.bval",
+...     fieldmap_image="fieldmap.nii",
+... )
+>>> task.cmdline    # doctest: +ELLIPSIS
+'eddy --imain=input.nii --mask=brain.nii --acqp=params.txt --index=index.txt \
+--bvecs=input.bvec --bvals=input.bval --field=fieldmap.nii --out=eddy ...'
 """
 
 __all__ = ["Eddy"]
 
-import os
-
-import attrs
+from os import PathLike
+from pathlib import PurePath
 
-import pydra
+from attrs import define, field
+from pydra.engine.specs import File, ShellOutSpec, ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
 
 
-@attrs.define(slots=False, kw_only=True)
-class EddySpec(pydra.specs.ShellSpec):
+@define(slots=False, kw_only=True)
+class EddySpec(ShellSpec):
     """Specifications for eddy."""
 
     # Parameters that specify input files.
-    input_image: os.PathLike = attrs.field(
+    input_image: PathLike = field(
         metadata={
-            "help_string": (
-                "input image as a 4D volume of all images acquired in the diffusion protocol"
-            ),
+            "help_string": "input image as a 4D volume",
             "mandatory": True,
-            "argstr": "--imain",
+            "argstr": "--imain={input_image}",
         }
     )
 
-    mask_image: os.PathLike = attrs.field(
+    brain_mask: PathLike = field(
         metadata={
             "help_string": "brain mask as a single volume image",
             "mandatory": True,
-            "argstr": "--mask",
+            "argstr": "--mask={brain_mask}",
         }
     )
 
-    acquisition_parameters_file: os.PathLike = attrs.field(
+    encoding_file: PathLike = field(
         metadata={
             "help_string": "acquisition parameters for the diffusion protocol",
             "mandatory": True,
-            "argstr": "--acqp",
+            "argstr": "--acqp={encoding_file}",
         }
     )
 
-    index_file: os.PathLike = attrs.field(
+    index_file: PathLike = field(
         metadata={
-            "help_string": "mapping from volume index to acquisition parameters",
+            "help_string": "mapping from volume index to encoding parameters",
             "mandatory": True,
-            "argstr": "--index",
+            "argstr": "--index={index_file}",
         }
     )
 
-    bvec_file: os.PathLike = attrs.field(
+    bvec_file: PathLike = field(
         metadata={
             "help_string": "diffusion directions",
             "mandatory": True,
-            "argstr": "--bvecs",
+            "argstr": "--bvecs={bvec_file}",
         }
     )
 
-    bval_file: os.PathLike = attrs.field(
+    bval_file: PathLike = field(
         metadata={
             "help_string": "diffusion weighting",
             "mandatory": True,
-            "argstr": "--bvals",
+            "argstr": "--bvals={bval_file}",
         }
     )
 
-    topup_file: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "topup output file",
-            "mandatory": True,
-            "argstr": "--topup",
-            "xor": {"fieldmap_image"},
-        }
+    fieldmap_image: PathLike = field(
+        metadata={"help_string": "fieldmap image", "argstr": "--field={fieldmap_image}"}
     )
 
-    fieldmap_image: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "fieldmap file",
-            "mandatory": True,
-            "argstr": "--field",
-            "xor": {"topup_file"},
-        }
-    )
-
-    fieldmap_matrix: os.PathLike = attrs.field(
+    fieldmap_matrix: PathLike = field(
         metadata={
             "help_string": "rigid-body transformation matrix from fieldmap to first input volume",
-            "argstr": "--field_mat",
+            "argstr": "--field_mat={fieldmap_matrix}",
             "requires": {"fieldmap_image"},
         }
     )
 
-    no_peas: bool = attrs.field(
+    no_peas: bool = field(
         metadata={
             "help_string": "do not perform post-Eddy alignment of shells",
             "argstr": "--dont_peas",
         }
     )
 
     # Parameters specifying names of output-files.
-    output_basename: str = attrs.field(
+    output_basename: str = field(
         default="eddy",
         metadata={
             "help_string": "basename for output files",
-            "argstr": "--out",
+            "argstr": "--out={output_basename}",
         },
     )
 
     # Parameters specifying how eddy should be run.
-    first_level_model: str = attrs.field(
+    first_level_model: str = field(
         default="quadratic",
         metadata={
             "help_string": "model for the magnetic field generated by Eddy currents",
-            "argstr": "--flm",
+            "argstr": "--flm={first_level_model}",
             "allowed_values": {"movement", "linear", "quadratic", "cubic"},
         },
     )
 
-    second_level_model: str = attrs.field(
+    second_level_model: str = field(
         default="none",
         metadata={
             "help_string": "model for how diffusion gradients generate Eddy currents",
-            "argstr": "--slm",
+            "argstr": "--slm={second_level_model}",
             "allowed_values": {"none", "linear", "quadratic"},
         },
     )
 
-    fwhm: float = attrs.field(
+    fwhm: float = field(
         default=0,
         metadata={
-            "help_string": (
-                "filter width used for pre-conditionning data prior to estimating distortions"
-            ),
-            "argstr": "--fwhm",
+            "help_string": "filter width used for pre-conditioning data prior to estimating distortions",
+            "argstr": "--fwhm={fwhm}",
         },
     )
 
-    num_iterations: int = attrs.field(
+    num_iterations: int = field(
         default=5,
         metadata={
             "help_string": "number of iterations for eddy",
-            "argstr": "--niter",
+            "argstr": "--niter={num_iterations}",
         },
     )
 
-    fill_empty_planes: bool = attrs.field(
-        metadata={
-            "help_string": "detect and fill empty planes",
-            "argstr": "--fep",
-        }
+    fill_empty_planes: bool = field(
+        metadata={"help_string": "detect and fill empty planes", "argstr": "--fep"}
     )
 
-    interpolation: str = attrs.field(
+    interpolation: str = field(
         default="spline",
         metadata={
             "help_string": "interpolation method for the estimation phase",
-            "argstr": "--interp",
+            "argstr": "--interp={interpolation}",
             "allowed_values": {"spline", "trilinear"},
         },
     )
 
-    resampling: str = attrs.field(
+    resampling: str = field(
         default="jac",
         metadata={
             "help_string": "final resampling strategy",
-            "argstr": "--resamp",
+            "argstr": "--resamp={resampling}",
             "allowed_values": {"jac", "lsr"},
         },
     )
 
-    num_voxels: int = attrs.field(
+    num_voxels: int = field(
         default=1000,
         metadata={
             "help_string": "number of voxels to use for GP hyperparameter estimation",
-            "argstr": "--nvoxhp",
+            "argstr": "--nvoxhp={num_voxels}",
         },
     )
 
-    fudge_factor: int = attrs.field(
+    fudge_factor: int = field(
         default=10,
         metadata={
             "help_string": "fudge factor for Q-space smoothing during estimation",
-            "argstr": "--ff",
+            "argstr": "--ff={fudge_factor}",
         },
     )
 
     # Parameters for outlier replacement (ol)
-    replace_outliers: bool = attrs.field(
+    replace_outliers: bool = field(
         metadata={"help_string": "replace outliers", "argstr": "--repol"}
     )
 
-    outlier_num_stdevs: int = attrs.field(
+    outlier_num_stdevs: int = field(
         metadata={
             "help_string": "number of times off the standard deviation to qualify as outlier",
-            "argstr": "--ol_nstd",
+            "argstr": "--ol_nstd={outlier_num_stdevs}",
             "requires": {"replace_outliers"},
         }
     )
 
-    outlier_num_voxels: int = attrs.field(
+    outlier_num_voxels: int = field(
         metadata={
             "help_string": "minimum number of voxels in a slice to qualify for outlier detection",
-            "argstr": "--ol_nvox",
+            "argstr": "--ol_nvox={outlier_num_voxels}",
             "requires": {"replace_outliers"},
         }
     )
 
-    outlier_type: str = attrs.field(
+    outlier_type: str = field(
         metadata={
             "help_string": "type of outliers detected",
-            "argstr": "--ol_type",
+            "argstr": "--ol_type={outlier_type}",
             "allowed_values": {"both", "gw", "sw"},
             "requires": {"replace_outliers"},
         }
     )
 
-    multiband_factor: int = attrs.field(
+    multiband_factor: int = field(
         metadata={
             "help_string": "multiband factor",
-            "argstr": "--mb",
+            "argstr": "--mb={multiband_factor}",
         }
     )
 
-    multiband_offset: int = attrs.field(
+    multiband_offset: int = field(
         metadata={
             "help_string": "multiband slice offset",
-            "argstr": "--mb_offs",
+            "argstr": "--mb_offs={multiband_offset}",
             "requires": {"multiband_factor"},
         }
     )
 
     # Parameters for intra-volume movement correction (s2v)
-    movement_prediction_order: int = attrs.field(
+    movement_prediction_order: int = field(
         default=0,
         metadata={
             "help_string": "order of movement prediction model",
-            "argstr": "--mporder",
+            "argstr": "--mporder={movement_prediction_order}",
         },
     )
 
-    s2v_num_iterations: int = attrs.field(
+    s2v_num_iterations: int = field(
         metadata={
             "help_string": "number of iterations for s2v movement estimation",
-            "argstr": "--s2v_niter",
+            "argstr": "--s2v_niter={s2v_num_iterations}",
         }
     )
 
-    s2v_lambda: float = attrs.field(
+    s2v_lambda: float = field(
         metadata={
             "help_string": "weighting of regularization for s2v movement estimation",
-            "argstr": "--s2v_lambda",
+            "argstr": "--s2v_lambda={s2v_lambda}",
         }
     )
 
-    s2v_interpolation: str = attrs.field(
+    s2v_interpolation: str = field(
         metadata={
             "help_string": "interpolation method for s2v movement estimation.",
-            "argstr": "--s2v_interp",
+            "argstr": "--s2v_interp={s2v_interpolation}",
             "allowed_values": {"spline", "trilinear"},
         }
     )
 
-    slice_grouping_file: os.PathLike = attrs.field(
+    slice_grouping_file: PathLike = field(
         metadata={
             "help_string": "file containing slice grouping information",
-            "argstr": "--slspec",
+            "argstr": "--slspec={slice_grouping_file}",
             "xor": {"slice_timing_file"},
         }
     )
 
-    slice_timing_file: os.PathLike = attrs.field(
+    slice_timing_file: PathLike = field(
         metadata={
             "help_string": "file containing slice timing information",
-            "argstr": "--json",
+            "argstr": "--json={slice_timing_file}",
             "xor": {"slice_grouping_file"},
         }
     )
 
     # Parameters for move-by-susceptibility correction (mbs)
-    estimate_move_by_susceptibility: bool = attrs.field(
+    estimate_move_by_susceptibility: bool = field(
         metadata={
             "help_string": "estimate susceptibility-induced field changes due to subject motion",
             "argstr": "--estimate_move_by_susceptibility",
         }
     )
 
-    mbs_num_iterations: int = attrs.field(
+    mbs_num_iterations: int = field(
         metadata={
             "help_string": "number of iterations for MBS field estimation",
-            "argstr": "--mbs_niter",
+            "argstr": "--mbs_niter={mbs_num_iterations}",
             "requires": {"estimate_move_by_susceptibility"},
         }
     )
 
-    mbs_lambda: int = attrs.field(
+    mbs_lambda: int = field(
         metadata={
             "help_string": "weighting of regularization for MBS field estimation",
-            "argstr": "--mbs_lambda",
+            "argstr": "--mbs_lambda={mbs_lambda}",
             "requires": {"estimate_move_by_susceptibility"},
         }
     )
 
-    mbs_knot_spacing: int = attrs.field(
+    mbs_knot_spacing: int = field(
         metadata={
             "help_string": "knot-spacing for MBS field estimation",
-            "argstr": "--mbs_ksp",
+            "argstr": "--mbs_ksp={mbs_knot_spacing}",
             "requires": {"estimate_move_by_susceptibility"},
         }
     )
 
     # Miscellaneous parameters.
-    data_is_shelled: bool = attrs.field(
+    data_is_shelled: bool = field(
         metadata={
             "help_string": "bypass checks for data shelling",
             "argstr": "--data_is_shelled",
         }
     )
 
-    random_seed: int = attrs.field(
+    random_seed: int = field(
         metadata={
             "help_string": "random seed for voxel selection",
-            "argstr": "--initrand",
+            "argstr": "--initrand={random_seed}",
         }
     )
 
-    save_cnr_maps: bool = attrs.field(
-        metadata={
-            "help_string": "save shell-wise CNR maps",
-            "argstr": "--cnr_maps",
-        }
+    save_cnr_maps: bool = field(
+        metadata={"help_string": "save shell-wise CNR maps", "argstr": "--cnr_maps"}
     )
 
-    save_residuals: bool = attrs.field(
+    save_residuals: bool = field(
         metadata={
             "help_string": "save residuals for all scans",
             "argstr": "--residuals",
         }
     )
 
-    verbose: bool = attrs.field(
-        metadata={
-            "help_string": "enable verbose logging",
-            "argstr": "-v",
-        }
+    verbose: bool = field(
+        metadata={"help_string": "enable verbose logging", "argstr": "--verbose"}
     )
 
 
-class EddyOutSpec(pydra.specs.ShellOutSpec):
+@define(slots=False, kw_only=True)
+class EddyOutSpec(ShellOutSpec):
     """Output specification for eddy."""
 
-    corrected_image: pydra.specs.File = attrs.field(
+    corrected_image: File = field(
         metadata={
             "help_string": "input image corrected for distortions",
             "output_file_template": "{output_basename}.nii.gz",
         }
     )
 
-    parameters_file: pydra.specs.File = attrs.field(
+    parameters_file: File = field(
         metadata={
             "help_string": "registration parameters for movement and EC",
             "output_file_template": "{output_basename}.eddy_parameters",
         }
     )
 
-    rotated_bvec_file: pydra.specs.File = attrs.field(
+    rotated_bvec_file: File = field(
         metadata={
             "help_string": "rotated b-vecs",
             "output_file_template": "{output_basename}.eddy_rotated_bvecs",
         }
     )
 
-    movement_rms_matrix: pydra.specs.File = attrs.field(
+    movement_rms_matrix: File = field(
         metadata={
             "help_string": "movement induced RMS",
             "output_file_template": "{output_basename}.eddy_movement_rms",
         }
     )
 
-    restricted_movement_rms_matrix: pydra.specs.File = attrs.field(
+    restricted_movement_rms_matrix: File = field(
         metadata={
             "help_string": "movement induced RMS without translation in the PE direction",
             "output_file_template": "{output_basename}.eddy_restricted_movement_rms",
         }
     )
 
-    displacement_fields_image: pydra.specs.File = attrs.field(
+    displacement_fields_image: File = field(
         metadata={
             "help_string": "displacement fields in millimeters",
             "output_file_template": "{output_basename}.eddy_displacement_fields",
         }
     )
 
-    outlier_free_image: pydra.specs.File = attrs.field(
+    outlier_free_image: File = field(
         metadata={
             "help_string": "input image with outliers replaced by predictions",
             "output_file_template": "{output_basename}.eddy_outlier_free_data",
             "requires": ["replace_outliers"],
         }
     )
 
-    movement_over_time_file: pydra.specs.File = attrs.field(
+    movement_over_time_file: File = field(
         metadata={
             "help_string": "movement parameters per time-point (slice or group)",
             "output_file_template": "{output_basename}.eddy_movement_over_time",
             "requires": ["movement_prediction_order"],
         }
     )
 
-    cnr_maps_image: pydra.specs.File = attrs.field(
+    cnr_maps_image: File = field(
         metadata={
             "help_string": "path to optional CNR maps image",
             "output_file_template": "{output_basename}.eddy_cnr_maps",
             "requires": ["save_cnr_maps"],
         }
     )
 
-    residuals_image: pydra.specs.File = attrs.field(
+    residuals_image: File = field(
         metadata={
             "help_string": "path to optional residuals image",
             "output_file_template": "{output_basename}.eddy_residuals",
             "requires": ["save_residuals"],
         }
     )
 
 
-class Eddy(pydra.engine.ShellCommandTask):
+class Eddy(ShellCommandTask):
     """Task definition for eddy."""
 
     executable = "eddy"
 
-    input_spec = pydra.specs.SpecInfo(name="EddyInput", bases=(EddySpec,))
+    input_spec = SpecInfo(name="Input", bases=(EddySpec,))
 
-    output_spec = pydra.specs.SpecInfo(name="EddyOutput", bases=(EddyOutSpec,))
+    output_spec = SpecInfo(name="Output", bases=(EddyOutSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/fast.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
-FMRIB's Automated Segmentation Tool (FAST)
-==========================================
+FAST
+====
 
-FAST performs automtic segmentation of 3D images of the brain
-using hidden Markov random field model and the expectation-maximization algorithm.
+Automatic segmentation of 3D images of the brain.
 """
 
 __all__ = ["FAST"]
 
 import os
 
 import attrs
@@ -25,20 +24,23 @@
             "help_string": "input image (single-channel mode)",
             "mandatory": True,
             "argstr": "",
             "position": -1,
         }
     )
 
-    image_type: int = attrs.field(
-        default=1,
+    image_type: str = attrs.field(
+        default="T1",
         metadata={
-            "help_string": "type of input image(s) (1: T1, 2: T2, 3: PD)",
+            "help_string": "type of input image (T1, T2 or PD)",
             "argstr": "-t",
-            "allowed_values": {1, 2, 3},
+            "allowed_values": {"T1", "T2", "PD"},
+            "formatter": lambda image_type: "-t {:d}".format(
+                {"T1": 1, "T2": 2, "PD": 3}.get(image_type)
+            ),
         },
     )
 
     # Output parameters.
     output_basename: str = attrs.field(
         default="fast",
         metadata={
@@ -168,15 +170,15 @@
             "requires": ["save_segmentation_masks"],
             "callable": get_segmentation_masks,
         }
     )
 
     probability_maps: pydra.specs.MultiOutputFile = attrs.field(
         metadata={
-            "help_string": "posterior probablity mapping for each class",
+            "help_string": "posterior probability mapping for each class",
             "requires": ["save_probability_maps"],
             "callable": get_probability_maps,
         }
     )
 
     partial_volume_maps: pydra.specs.MultiOutputFile = attrs.field(
         metadata={
@@ -204,10 +206,10 @@
 
 
 class FAST(pydra.engine.ShellCommandTask):
     """Task definition for FAST."""
 
     executable = "fast"
 
-    input_spec = pydra.specs.SpecInfo(name="FASTInput", bases=(FASTSpec,))
+    input_spec = pydra.specs.SpecInfo(name="Input", bases=(FASTSpec,))
 
-    output_spec = pydra.specs.SpecInfo(name="FASTOuput", bases=(FASTOutSpec,))
+    output_spec = pydra.specs.SpecInfo(name="Ouput", bases=(FASTOutSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/fnirt.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirtfileutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,120 @@
 """
-FSL Non-linear Image Registration Tool (FNIRT)
-==============================================
-
-FNIRT performs non-linear registration of brain images.
+FNIRTFileUtils
+==============
 
 Examples
 --------
 
-Register two images together:
+>>> task = FNIRTFileUtils(
+...     input_image="input.nii",
+...     reference_image="reference.nii",
+... )
+>>> task.cmdline  # doctest: +ELLIPSIS
+'fnirtfileutils --in input.nii --ref reference.nii --out ...input_field.nii \
+--outformat field ...'
 
->>> task = FNIRT(
-...     reference_image="template.nii",
+>>> task = FNIRTFileUtils(
 ...     input_image="input.nii",
+...     reference_image="reference.nii",
+...     output_jacobian_image="jacobian.nii",
+...     with_affine_transform=True,
 ... )
 >>> task.cmdline  # doctest: +ELLIPSIS
-'fnirt --ref template.nii --in input.nii --cout .../input_fnirt_coeff \
---iout .../input_fnirt.nii --fout .../input_fnirt_field.nii'
+'fnirtfileutils --in input.nii --ref reference.nii ... --jac jacobian.nii \
+... --withaff'
 """
 
-__all__ = ["FNIRT"]
+__all__ = ["FNIRTFileUtils"]
 
 import os
 
 import attrs
 
 import pydra
 
+from . import specs
 
-@attrs.define(slots=False, kw_only=True)
-class FNIRTSpec(pydra.specs.ShellSpec):
-    """Task specifications for FNIRT."""
 
-    reference_image: os.PathLike = attrs.field(
-        metadata={"help_string": "reference image", "argstr": "--ref"}
-    )
+@attrs.define(slots=False, kw_only=True)
+class FNIRTFileUtilsSpec(pydra.specs.ShellSpec):
+    """Specifications for fnirtfileutils."""
 
     input_image: os.PathLike = attrs.field(
-        metadata={"help_string": "input image", "argstr": "--in"}
+        metadata={
+            "help_string": "input image with FNIRT coefficients",
+            "argstr": "--in",
+        }
     )
 
-    output_field_coefficients_file: str = attrs.field(
+    reference_image: os.PathLike = attrs.field(
         metadata={
-            "help_string": "output file containing the field coefficients",
-            "argstr": "--cout",
-            "output_file_template": "{input_image}_fnirt_coeff",
-            "keep_extension": False,
+            "help_string": "reference image",
+            "argstr": "--ref",
         }
     )
 
     output_image: str = attrs.field(
         metadata={
-            "help_string": "output image",
-            "argstr": "--iout",
-            "output_file_template": "{input_image}_fnirt",
+            "help_string": "output field or coefficient image",
+            "argstr": "--out",
+            "output_file_template": "{input_image}_{output_format}",
         }
     )
 
-    output_field_image: str = attrs.field(
+    output_format: str = attrs.field(
+        default="field",
         metadata={
-            "help_string": "output deformation field",
-            "argstr": "--fout",
-            "output_file_template": "{input_image}_fnirt_field",
+            "help_string": "output format (field or spline)",
+            "argstr": "--outformat",
+            "allowed_values": {"field", "spline"},
+        },
+    )
+
+    warp_resolution: float = attrs.field(
+        metadata={
+            "help_string": "warp resolution in millimeters",
+            "argstr": "--warpres",
+            # "requires": {("output_format", "spline")},  # TODO
         }
     )
 
-    reference_mask: os.PathLike = attrs.field(
+    knot_spacing: float = attrs.field(
         metadata={
-            "help_string": "mask in reference space",
-            "argstr": "--applyrefmask --refmask",
+            "help_string": "knot spacing in voxels",
+            "argstr": "--knotspace",
+            # "requires": {("output_format", "spline")},  # TODO
         }
     )
 
-    input_mask: os.PathLike = attrs.field(
+    output_jacobian_image: str = attrs.field(
         metadata={
-            "help_string": "mask in input image space",
-            "argstr": "--applyinmask --inmask",
+            "help_string": "output Jacobian determinant map",
+            "argstr": "--jac",
+            "output_file_template": "{input_image}_jac",
         }
     )
 
-    verbose: bool = attrs.field(
+    output_jacobian_matrix: str = attrs.field(
         metadata={
-            "help_string": "enable verbose logging",
-            "argstr": "-v",
+            "help_string": "output Jacobian matrix map",
+            "argstr": "--matjac",
+            "output_file_template": "{input_image}_matjac",
         }
     )
 
+    with_affine_transform: bool = attrs.field(
+        metadata={
+            "help_string": "include affine transform in field and jacobian images",
+            "argstr": "--withaff",
+        }
+    )
 
-class FNIRT(pydra.engine.ShellCommandTask):
-    """Task definition for FNIRT."""
 
-    executable = "fnirt"
+class FNIRTFileUtils(pydra.engine.ShellCommandTask):
+    """Task definition for fnirtfileutils."""
 
-    input_spec = pydra.specs.SpecInfo(name="FNIRTInput", bases=(FNIRTSpec,))
+    executable = "fnirtfileutils"
+
+    input_spec = pydra.specs.SpecInfo(
+        name="Input", bases=(FNIRTFileUtilsSpec, specs.VerboseSpec)
+    )
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/fslmaths.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/maths.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,128 @@
 """
 fslmaths
 ========
 
+Mathematical manipulation of images.
+
 Examples
 --------
 
 Convert input image to float:
 
->>> task = FSLMaths(input_image="input.nii")
->>> task.cmdline  # doctest: +ELLIPSIS
-'fslmaths input.nii .../input_fslmaths.nii -odt float'
-
-Apply mask to input image:
-
->>> task = Mul(
-...     input_image="input.nii",
-...     other_image="mask.nii",
-...     output_image="output.nii",
-... )
+>>> task = Maths(input_image="input.nii")
+>>> task.cmdline    # doctest: +ELLIPSIS
+'fslmaths input.nii .../input_fslmaths.nii'
+
+Multiply input image with a binary mask:
+
+>>> task = Mul(input_image="input.nii", other_image="mask.nii", output_image="output.nii")
 >>> task.cmdline
-'fslmaths input.nii -mul mask.nii output.nii -odt float'
-"""
+'fslmaths input.nii -mul mask.nii output.nii'
 
-__all__ = ["FSLMaths", "Mul"]
+>>> task = Threshold(input_image="input.nii", threshold=0.3, output_image="output.nii")
+>>> task.cmdline
+'fslmaths input.nii -thr 0.3 output.nii'
+"""
 
-import os
+__all__ = ["Maths", "MathsSpec", "Mul", "Threshold"]
 
-import attrs
+from os import PathLike
 
-import pydra
+from attrs import define, field
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
 
 
-@attrs.define(slots=False, kw_only=True)
-class FSLMathsSpec(pydra.specs.ShellSpec):
+@define(kw_only=True)
+class MathsSpec(ShellSpec):
     """Specifications for fslmaths."""
 
-    _ALLOWED_DATATYPES = {"char", "short", "int", "float", "double", "input"}
+    _datatypes = {"char", "short", "int", "float", "double", "input"}
 
-    datatype: str = attrs.field(
+    internal_datatype: str = field(
         metadata={
-            "help_string": "datatype used for internal computation",
+            "help_string": "internal datatype",
             "argstr": "-dt",
             "position": 1,
-            "allowed_values": _ALLOWED_DATATYPES,
+            "allowed_values": _datatypes,
         }
     )
 
-    input_image: os.PathLike = attrs.field(
+    input_image: PathLike = field(
         metadata={
             "help_string": "input image",
             "mandatory": True,
             "argstr": "",
             "position": 2,
         }
     )
 
-    output_image: str = attrs.field(
+    output_image: str = field(
         metadata={
             "help_string": "output image",
             "argstr": "",
             "position": -2,
             "output_file_template": "{input_image}_fslmaths",
         }
     )
 
-    output_datatype: str = attrs.field(
-        default="float",
+    output_datatype: str = field(
         metadata={
-            "help_string": "datatype used for output serialization",
+            "help_string": "output datatype",
             "argstr": "-odt",
             "position": -1,
-            "allowed_values": _ALLOWED_DATATYPES,
-        },
+            "allowed_values": _datatypes,
+        }
     )
 
 
-class FSLMaths(pydra.engine.ShellCommandTask):
+class Maths(ShellCommandTask):
     """Task definition for fslmaths."""
 
     executable = "fslmaths"
 
-    input_spec = pydra.specs.SpecInfo(name="Input", bases=(FSLMathsSpec,))
+    input_spec = SpecInfo(name="Input", bases=(MathsSpec,))
 
 
-@attrs.define(slots=False, kw_only=True)
-class MulSpec(pydra.specs.ShellSpec):
+@define(kw_only=True)
+class MulSpec(MathsSpec):
     """Specifications for fslmaths' mul."""
 
-    other_image: os.PathLike = attrs.field(
+    other_image: PathLike = field(
         metadata={
             "help_string": "multiply input with other image",
+            "mandatory": True,
             "argstr": "-mul",
         }
     )
 
 
-class Mul(FSLMaths):
+class Mul(Maths):
     """Task definition for fslmaths' mul."""
 
-    input_spec = pydra.specs.SpecInfo(name="Input", bases=(FSLMathsSpec, MulSpec))
+    input_spec = SpecInfo(name="Input", bases=(MulSpec,))
+
+
+@define(kw_only=True)
+class ThresholdSpec(MathsSpec):
+    """Specifications for fslmaths' threshold."""
+
+    threshold: float = field(
+        metadata={
+            "help_string": "value for thresholding the image",
+            "mandatory": True,
+            "argstr": "-thr",
+        }
+    )
+
+
+class Threshold(Maths):
+    """Task definition for fslmaths' threshold."""
+
+    input_spec = SpecInfo(name="Input", bases=(ThresholdSpec,))
+
+
+# TODO: Drop compatibility alias for 0.x
+FSLMaths = Maths
+FSLMathsSpec = MathsSpec
+__all__ += ["FSLMaths", "FSLMathsSpec"]
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/fslmerge.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/sigloss.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,68 @@
 """
-FSLMerge
-========
+SigLoss
+=======
+
+Estimate signal loss from a B0 map.
 
 Examples
 --------
 
->>> task = FSLMerge(
-...     dimension="t",
-...     input_images=["vol1.nii", "vol2.nii"],
-... )
+>>> task = SigLoss(input_image="b0map.nii", input_mask="mask.nii", output_image="sigloss.nii")
 >>> task.cmdline  # doctest: +ELLIPSIS
-'fslmerge -t ...merged vol1.nii vol2.nii'
+'sigloss ... --in b0map.nii --mask mask.nii --sigloss sigloss.nii'
 """
 
-__all__ = ["FSLMerge"]
+__all__ = ["SigLoss"]
 
 import os
-import typing as ty
 
 import attrs
 
 import pydra
 
 
 @attrs.define(slots=False, kw_only=True)
-class FSLMergeSpec(pydra.specs.ShellSpec):
-    """Specifications for fslmerge."""
+class SigLossSpec(pydra.specs.ShellSpec):
+    """Specifications for sigloss."""
 
-    dimension: str = attrs.field(
-        metadata={
-            "help_string": "merge dimension",
-            "mandatory": True,
-            "argstr": "-{dimension}",
-            "allowed_values": {"t", "x", "y", "z", "a", "tr"},
-            "xor": {"volume_index"},
-        }
+    echo_time: float = attrs.field(
+        default=1.0,
+        metadata={"help_string": "echo time in seconds", "argstr": "--te"},
     )
 
-    volume_index: int = attrs.field(
+    slice_direction: str = attrs.field(
+        default="z",
         metadata={
-            "help_string": "merge volume N from each input file",
-            "mandatory": True,
-            "argstr": "-n",
-            "xor": {"dimension"},
-        }
+            "help_string": "slice direction",
+            "argstr": "--slicedir",
+            "allowed_values": {"x", "y", "z"},
+        },
     )
 
-    output_image: str = attrs.field(
+    input_image: os.PathLike = attrs.field(
         metadata={
-            "help_string": "output image",
-            "argstr": "",
-            "output_file_template": "merged",
+            "help_string": "input B0-map image in rad/s",
+            "mandatory": True,
+            "argstr": "--in",
         }
     )
 
-    input_images: ty.Iterable[os.PathLike] = attrs.field(
-        metadata={
-            "help_string": "input image",
-            "mandatory": True,
-            "argstr": "...",
-        }
+    input_mask: os.PathLike = attrs.field(
+        metadata={"help_string": "input mask", "argstr": "--mask"}
     )
 
-    repetition_time: float = attrs.field(
+    output_image: str = attrs.field(
         metadata={
-            "help_string": "specify TR value in seconds (default is 1.0)",
-            "argstr": "",
+            "help_string": "output signal-loss image",
+            "argstr": "--sigloss",
+            "output_file_template": "{input_image}_sigloss",
         }
     )
 
 
-class FSLMerge(pydra.engine.ShellCommandTask):
-    """Task definition for fslmerge."""
+class SigLoss(pydra.engine.ShellCommandTask):
+    """Task definition for sigloss."""
 
-    executable = "fslmerge"
+    executable = "sigloss"
 
-    input_spec = pydra.specs.SpecInfo(name="FSLMergeInput", bases=(FSLMergeSpec,))
+    input_spec = pydra.specs.SpecInfo(name="Input", bases=(SigLossSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/fslreorient2std.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/reorient2std.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 """
-FSLReorient2Std
-===============
+Reorient2Std
+============
 
 Change orientation of the image to match the one used
 for standard template images (MNI152).
 
 Examples
 --------
 
->>> task = FSLReorient2Std(input_image="image.nii")
+>>> task = Reorient2Std(input_image="image.nii")
 >>> task.cmdline  # doctest: +ELLIPSIS
 'fslreorient2std -m ...image_r2std.mat image.nii ...image_r2std.nii'
 """
 
-__all__ = ["FSLReorient2Std"]
+__all__ = ["Reorient2Std"]
 
-import os
+from os import PathLike
 
-import attrs
+from attrs import define, field
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
 
-import pydra
 
+@define(kw_only=True)
+class Reorient2StdSpec(ShellSpec):
+    """Specifications for fslreorient2std."""
 
-@attrs.define(slots=False, kw_only=True)
-class FSLReorient2StdSpec(pydra.specs.ShellSpec):
-    """Specificiations for fslreorient2std."""
-
-    input_image: os.PathLike = attrs.field(
+    input_image: PathLike = field(
         metadata={
             "help_string": "input image",
             "mandatory": True,
             "argstr": "",
             "position": -2,
         }
     )
 
-    output_image: str = attrs.field(
+    output_image: str = field(
         metadata={
             "help_string": "output reoriented image",
             "argstr": "",
             "position": -1,
             "output_file_template": "{input_image}_r2std",
         }
     )
 
-    output_matrix: str = attrs.field(
+    output_matrix: str = field(
         metadata={
             "help_string": "output transformation matrix",
             "argstr": "-m",
             "output_file_template": "{input_image}_r2std.mat",
             "keep_extension": False,
         }
     )
 
 
-class FSLReorient2Std(pydra.engine.ShellCommandTask):
+class Reorient2Std(ShellCommandTask):
     """Task definition for fslreorient2std."""
 
     executable = "fslreorient2std"
 
-    input_spec = pydra.specs.SpecInfo(
-        name="FSLReorient2StdInput", bases=(FSLReorient2StdSpec,)
-    )
+    input_spec = SpecInfo(name="Input", bases=(Reorient2StdSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/fslroi.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice_timer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,98 @@
-"""
-FSLROI
-======
-
-Manual cropping to a region-of-interest (ROI) for structural brain images.
-
-Examples
---------
-
-Extract a 16-voxel cube starting at position (10, 20, 30):
->>> task = FSLROI(
-...    input_image="image.nii",
-...    min_x=10,
-...    min_y=20,
-...    min_z=30,
-...    size_x=16,
-...    size_y=16,
-...    size_z=16,
-... )
->>> task.cmdline  # doctest: +ELLIPSIS
-'fslroi image.nii ...image_roi.nii 10 16 20 16 30 16'
-
-Extract a temporal window starting at 5 onwards:
->>> task = FSLROI(
-...     input_image="input.nii",
-...     output_image="output.nii",
-...     min_t=5,
-...     size_t=-1,
-... )
->>> task.cmdline
-'fslroi input.nii output.nii 5 -1'
-"""
-
-__all__ = ["FSLROI"]
-
-import os
-
-import attrs
-
-import pydra
-
-
-@attrs.define(slots=False, kw_only=True)
-class FSLROISpec(pydra.specs.ShellSpec):
-    """Specifications for fslroi."""
-
-    input_image: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "input image",
+from fileformats.generic.file import File
+from pathlib import Path
+from pydra.engine import ShellCommandTask
+from pydra.engine import specs
+import typing as ty
+
+input_fields = [
+    (
+        "in_file",
+        File,
+        {
+            "help_string": "filename of input timeseries",
+            "argstr": "--in={in_file}",
             "mandatory": True,
-            "argstr": "",
-        }
-    )
-
-    output_image: str = attrs.field(
-        metadata={
-            "help_string": "output image",
-            "argstr": "",
-            "output_file_template": "{input_image}_roi",
-        }
-    )
-
-    min_x: int = attrs.field(
-        metadata={
-            "help_string": "start of ROI in x-dimension (0-based indexing)",
-            "argstr": "",
-        }
-    )
-
-    size_x: int = attrs.field(
-        # default=-1,
-        metadata={
-            "help_string": "size of ROI in x-dimension (-1 for maximum)",
-            "argstr": "",
-            "requires": {"min_x"},
-        }
-    )
-
-    min_y: int = attrs.field(
-        metadata={
-            "help_string": "start of ROI in y-dimension (0-based indexing)",
-            "argstr": "",
-            "requires": {"min_x"},
-        }
-    )
-
-    size_y: int = attrs.field(
-        # default=-1,
-        metadata={
-            "help_string": "size of ROI in y-dimension (-1 for maximum)",
-            "argstr": "",
-            "requires": {"min_y"},
-        }
-    )
-
-    min_z: int = attrs.field(
-        metadata={
-            "help_string": "start of ROI in z-dimension (0-based indexing)",
-            "argstr": "",
-            "requires": {"min_x"},
-        }
-    )
-
-    size_z: int = attrs.field(
-        # default=-1,
-        metadata={
-            "help_string": "size of ROI in z-dimension (-1 for maximum)",
-            "argstr": "",
-            "requires": {"min_z"},
-        }
-    )
-
-    min_t: int = attrs.field(
-        metadata={
-            "help_string": "start of ROI in t-dimension (0-based indexing)",
-            "argstr": "",
-        }
-    )
-
-    size_t: int = attrs.field(
-        # default=-1,
-        metadata={
-            "help_string": "size of ROI in t-dimension (-1 for maximum)",
-            "argstr": "",
-            "requires": {"min_t"},
-        },
-    )
-
-
-class FSLROI(pydra.engine.ShellCommandTask):
-    """Task definition for fslroi."""
-
-    executable = "fslroi"
-
-    input_spec = pydra.engine.specs.SpecInfo(name="FSLROIInput", bases=(FSLROISpec,))
+            "position": 0,
+        },
+    ),
+    (
+        "out_file",
+        Path,
+        {"help_string": "filename of output timeseries", "argstr": "--out={out_file}"},
+    ),
+    (
+        "index_dir",
+        bool,
+        {"help_string": "slice indexing from top to bottom", "argstr": "--down"},
+    ),
+    (
+        "time_repetition",
+        float,
+        {
+            "help_string": "Specify TR of data - default is 3s",
+            "argstr": "--repeat={time_repetition}",
+        },
+    ),
+    (
+        "slice_direction",
+        ty.Any,
+        {
+            "help_string": "direction of slice acquisition (x=1, y=2, z=3) - default is z",
+            "argstr": "--direction={slice_direction}",
+        },
+    ),
+    (
+        "interleaved",
+        bool,
+        {"help_string": "use interleaved acquisition", "argstr": "--odd"},
+    ),
+    (
+        "custom_timings",
+        File,
+        {
+            "help_string": "slice timings, in fractions of TR, range 0:1 (default is 0.5 = no shift)",
+            "argstr": "--tcustom={custom_timings}",
+        },
+    ),
+    (
+        "global_shift",
+        float,
+        {
+            "help_string": "shift in fraction of TR, range 0:1 (default is 0.5 = no shift)",
+            "argstr": "--tglobal",
+        },
+    ),
+    (
+        "custom_order",
+        File,
+        {
+            "help_string": "filename of single-column custom interleave order file (first slice is referred to as 1 not 0)",
+            "argstr": "--ocustom={custom_order}",
+        },
+    ),
+]
+SliceTimer_input_spec = specs.SpecInfo(
+    name="Input", fields=input_fields, bases=(specs.ShellSpec,)
+)
+
+output_fields = [
+    ("slice_time_corrected_file", File, {"help_string": "slice time corrected file"})
+]
+SliceTimer_output_spec = specs.SpecInfo(
+    name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
+)
+
+
+class SliceTimer(ShellCommandTask):
+    """
+    Examples
+    -------
+
+    >>> from fileformats.generic.file import File
+    >>> from pydra.tasks.fsl.auto.slice_timer import SliceTimer
+
+    """
+
+    input_spec = SliceTimer_input_spec
+    output_spec = SliceTimer_output_spec
+    executable = "slicetimer"
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/susan.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/susan.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,8 +99,8 @@
 
 
 class SUSAN(pydra.engine.ShellCommandTask):
     """Task definition for SUSAN."""
 
     executable = "susan"
 
-    input_spec = pydra.specs.SpecInfo(name="SUSANInput", bases=(SUSANSpec,))
+    input_spec = pydra.specs.SpecInfo(name="Input", bases=(SUSANSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/bet/bet.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/bet.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,27 +74,23 @@
             ),
             "argstr": "-g",
         }
     )
 
     head_radius: float = attrs.field(
         metadata={
-            "help_string": (
-                "Head radius (in millimeters)."
-                " Initial surface sphere is set to half of this value."
-            ),
+            "help_string": "Head radius (in millimeters)."
+            " Initial surface sphere is set to half of this value.",
             "argstr": "-r",
         }
     )
 
     center_of_gravity: ty.Tuple[int, int, int] = attrs.field(
         metadata={
-            "help_string": (
-                "centre-of-gravity (in voxel coordinates) of initial mesh surface"
-            ),
+            "help_string": "centre-of-gravity (in voxel coordinates) of initial mesh surface",
             "argstr": "-c",
         }
     )
 
     apply_thresholding: bool = attrs.field(
         metadata={
             "help_string": "apply thresholding to segmented brain image and mask",
@@ -202,12 +198,10 @@
 
 
 class BET(pydra.engine.ShellCommandTask):
     """Task definition for BET."""
 
     executable = "bet"
 
-    input_spec = pydra.specs.SpecInfo(
-        name="BETInput", bases=(BETSpec, BETVariationsSpec)
-    )
+    input_spec = pydra.specs.SpecInfo(name="Input", bases=(BETSpec, BETVariationsSpec))
 
-    output_spec = pydra.specs.SpecInfo(name="BETOutput", bases=(BETOutSpec,))
+    output_spec = pydra.specs.SpecInfo(name="Output", bases=(BETOutSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/bet/robustfov.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/robustfov.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 
 
 class RobustFOV(pydra.engine.ShellCommandTask):
     """Task definition for robustfov."""
 
     executable = "robustfov"
 
-    input_spec = pydra.specs.SpecInfo(name="RobustFOVInput", bases=(RobustFOVSpec,))
+    input_spec = pydra.specs.SpecInfo(name="Input", bases=(RobustFOVSpec,))
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/apply_xfm.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/applywarp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,152 @@
 """
-ApplyXFM
-========
+ApplyWarp
+=========
 
 Examples
 --------
 
->>> task = ApplyXFM(
-...     input_image="input.nii",
-...     reference_image="reference.nii",
-...     input_matrix="affine.mat",
+>>> task = ApplyWarp(
+...     input_image="invol.nii",
+...     reference_image="refvol.nii",
+...     input_warpfield="warpvol.nii",
+...     warpfield_as="abs",
 ... )
 >>> task.cmdline  # doctest: +ELLIPSIS
-'flirt -in input.nii -ref reference.nii -init affine.mat -out .../input_axfm.nii \
--applyxfm -interp trilinear'
+'applywarp --in invol.nii --ref refvol.nii --out ...invol_warped.nii \
+--warp warpvol.nii --abs ...'
 
->>> task = ApplyXFM(
-...     input_image="input.nii",
-...     reference_image="reference.nii",
-...     input_matrix="affine.mat",
-...     isotropic_resolution=1,
-...     padding_size=5,
+>>> task = ApplyWarp(
+...     input_image="invol.nii",
+...     reference_image="refvol.nii",
+...     output_image="outvol.nii",
+...     use_sqform=True,
 ... )
 >>> task.cmdline  # doctest: +ELLIPSIS
-'flirt -in input.nii -ref reference.nii -init affine.mat -out .../input_axfm.nii \
--applyisoxfm 1 -paddingsize 5 -interp trilinear'
-
+'applywarp --in invol.nii --ref refvol.nii --out outvol.nii ... --usesqform'
 """
 
-__all__ = ["ApplyXFM"]
+__all__ = ["ApplyWarp"]
 
 import os
+import typing as ty
 
 import attrs
 
 import pydra
 
 from . import specs
-from .flirt import FLIRT
 
 
 @attrs.define(slots=False, kw_only=True)
-class ApplyXFMSpec(pydra.specs.ShellSpec):
-    """Specifications for ApplyXFM."""
+class ApplyWarpSpec(pydra.specs.ShellSpec):
+    """Specifications for applywarp."""
 
     input_image: os.PathLike = attrs.field(
         metadata={
             "help_string": "input image",
             "mandatory": True,
-            "argstr": "-in",
+            "argstr": "--in",
         }
     )
 
     reference_image: os.PathLike = attrs.field(
         metadata={
             "help_string": "reference image",
             "mandatory": True,
-            "argstr": "-ref",
+            "argstr": "--ref",
         }
     )
 
-    input_matrix: os.PathLike = attrs.field(
+    output_image: str = attrs.field(
         metadata={
-            "help_string": "input transformation matrix",
-            "mandatory": True,
-            "argstr": "-init",
+            "help_string": "output image",
+            "argstr": "--out",
+            "output_file_template": "{input_image}_warped",
         }
     )
 
-    output_image: str = attrs.field(
+    input_warpfield: os.PathLike = attrs.field(
         metadata={
-            "help_string": "output image",
-            "argstr": "-out",
-            "output_file_template": "{input_image}_axfm",
+            "help_string": "deformation field or coefficients",
+            "argstr": "--warp",
+        }
+    )
+
+    warpfield_as: str = attrs.field(
+        metadata={
+            "help_string": "treat deformation field as absolute (abs) or relative (rel)",
+            "argstr": "--{warpfield_as}",
+            "allowed_values": {"abs", "rel"},
+            "requires": {"input_warpfield"},
         }
     )
 
     output_datatype: str = attrs.field(
         metadata={
-            "help_string": "output datatype",
-            "argstr": "-datatype",
-            "allowed_values": {
-                "char",
-                "short",
-                "int",
-                "float",
-                "double",
-            },
+            "help_string": "force output datatype",
+            "argstr": "--datatype",
+            "allowed_values": {"char", "short", "int", "float", "double"},
+        }
+    )
+
+    supersampling_level: ty.Union[str, int] = attrs.field(
+        metadata={
+            "help_string": "level of intermediate supersampling",
+            "argstr": "--super --superlevel",
+        }
+    )
+
+    pre_affine_matrix: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "pre-affine matrix",
+            "argstr": "--premat",
+        }
+    )
+
+    post_affine_matrix: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "post-affine matrix",
+            "argstr": "--postmat",
+        }
+    )
+
+    reference_mask: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "mask image in reference space",
+            "argstr": "--mask",
         }
     )
 
-    isotropic_resolution: float = attrs.field(
-        default=0.0,
-        metadata={
-            "help_string": "force resampling to isotropic resolution",
-            "formatter": lambda isotropic_resolution: (
-                f"-applyisoxfm {isotropic_resolution}"
-                if isotropic_resolution
-                else "-applyxfm"
-            ),
+    interpolation: str = attrs.field(
+        default="trilinear",
+        metadata={
+            "help_string": "interpolation method",
+            "argstr": "--interp",
+            "allowed_values": {"nn", "trilinear", "sinc", "spline"},
         },
     )
 
     padding_size: float = attrs.field(
         metadata={
             "help_string": "padding size in voxels",
-            "argstr": "-paddingsize",
+            "argstr": "--paddingsize",
+        }
+    )
+
+    use_sqform: bool = attrs.field(
+        metadata={
+            "help_string": "use sform and qform from reference and input images",
+            "argstr": "--usesqform",
+            "requires": {"input_image", "reference_image"},
         }
     )
 
 
-class ApplyXFM(FLIRT):
-    """Task definition for ApplyXFM."""
+class ApplyWarp(pydra.engine.ShellCommandTask):
+    """Task definition for applywarp."""
+
+    executable = "applywarp"
 
     input_spec = pydra.specs.SpecInfo(
-        name="ApplyXFMInput",
-        bases=(ApplyXFMSpec, specs.InterpolationSpec),
+        name="Input", bases=(ApplyWarpSpec, specs.VerboseSpec)
     )
```

### Comparing `pydra_fsl-0.0.9/pydra/tasks/fsl/flirt/specs.py` & `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/specs.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "CostFunctionSpec",
     "InterpolationSpec",
     "SearchSpec",
     "WeightingSpec",
 ]
 
 import os
+import pathlib
 import typing as ty
 
 import attrs
 
 import pydra
 
 
@@ -112,7 +113,78 @@
 
     input_weighting_image: os.PathLike = attrs.field(
         metadata={
             "help_string": "weights for input image",
             "argstr": "-inweight",
         }
     )
+
+
+@attrs.define(slots=False, kw_only=True)
+class VerboseSpec(pydra.specs.ShellSpec):
+    verbose: bool = attrs.field(
+        metadata={
+            "help_string": "enable verbose logging",
+            "argstr": "-v",
+        }
+    )
+
+
+@attrs.define(slots=False, kw_only=True)
+class BaseCoordSpec(pydra.specs.ShellSpec):
+    input_coordinates: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "input coordinates",
+            "mandatory": True,
+            "argstr": "",
+            "position": -1,
+        }
+    )
+
+    output_coordinates: str = attrs.field(
+        metadata={
+            "help_string": "output coordinates",
+            "output_file_template": "{input_coordinates}_out",
+        }
+    )
+
+    affine_matrix: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "affine transformation matrix",
+            "argstr": "-xfm",
+        }
+    )
+
+    input_warpfield: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "input warpfield image",
+            "argstr": "-warp",
+        }
+    )
+
+    unit: str = attrs.field(
+        default="vox",
+        metadata={
+            "help_string": "unit of coordinates: voxels (vox) or millimeters (mm)",
+            "argstr": "-{unit}",
+            "allowed_values": {"vox", "mm"},
+        },
+    )
+
+
+def _get_output_coordinates(output_coordinates: str, stdout):
+    output_coordinates = pathlib.Path.cwd() / output_coordinates
+
+    with open(output_coordinates, mode="w") as f:
+        f.write(stdout)
+
+    return output_coordinates
+
+
+@attrs.define(slots=False, kw_only=True)
+class CoordOutSpec(pydra.specs.ShellOutSpec):
+    output_coordinates: os.PathLike = attrs.field(
+        metadata={
+            "help_string": "output coordinates",
+            "callable": _get_output_coordinates,
+        }
+    )
```

### Comparing `pydra_fsl-0.0.9/LICENSE` & `pydra_fsl-0.1.0/LICENSE`

 * *Files identical despite different names*

