# Comparing `tmp/kappadata-1.4.8.tar.gz` & `tmp/kappadata-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.4.8.tar", last modified: Thu Dec 14 13:58:02 2023, max compression
+gzip compressed data, was "kappadata-1.4.9.tar", last modified: Thu Dec 14 14:40:48 2023, max compression
```

## Comparing `kappadata-1.4.8.tar` & `kappadata-1.4.9.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.042553 kappadata-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-14 13:56:10.000000 kappadata-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2023-12-14 13:58:02.042553 kappadata-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2023-12-14 13:56:10.000000 kappadata-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.006553 kappadata-1.4.8/kappadata/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-14 13:57:48.000000 kappadata-1.4.8/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.006553 kappadata-1.4.8/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.010553 kappadata-1.4.8/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.010553 kappadata-1.4.8/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/base/kd_single_collator_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/kd_dino_mask_collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/kd_ijepa_mask_collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9500 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.010553 kappadata-1.4.8/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.010553 kappadata-1.4.8/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.010553 kappadata-1.4.8/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.010553 kappadata-1.4.8/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/mae_finetune_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/mugs_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.014553 kappadata-1.4.8/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_audioset_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_esc50_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_image_net_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_sid_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_speech_ccommands_v1_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/transforms/norm/kd_speech_ccommands_v2_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.014553 kappadata-1.4.8/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.014553 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/mugs_multi_view_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.014553 kappadata-1.4.8/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/copying/copying_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/copying/create_zips.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/copying/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.014553 kappadata-1.4.8/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.014553 kappadata-1.4.8/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.018553 kappadata-1.4.8/kappadata/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.018553 kappadata-1.4.8/kappadata/mock/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/mock/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/mock/datasets/audioset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/mock/datasets/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/mock/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.018553 kappadata-1.4.8/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.018553 kappadata-1.4.8/kappadata/samplers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/base/sampler_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/class_balanced_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/interleaved_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/semi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/sequential_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/samplers/weighted_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.026553 kappadata-1.4.8/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.026553 kappadata-1.4.8/kappadata/transforms/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/audio/kd_fbank.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/audio/kd_magnitude_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/audio/kd_roll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/audio/kd_spec_augment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.026553 kappadata-1.4.8/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_additive_uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_binarize.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_columnwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_minsize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_random_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_simple_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_solarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_three_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_transform_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/kd_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.030553 kappadata-1.4.8/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/norm/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/patchify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/patchwise_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/save_state_to_context_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.030553 kappadata-1.4.8/kappadata/transforms/semseg/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/semseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_random_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/unpatchify.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.034553 kappadata-1.4.8/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/getall_as_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/global_rng.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.034553 kappadata-1.4.8/kappadata/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_dataset_imgsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_mae_schematic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_masked_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/visualization/visualize_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.034553 kappadata-1.4.8/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.038553 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/allgather_class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/class_groups_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/intra_class_shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/kd_pseudo_label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/random_superclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/sort_by_class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/swap_label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.038553 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.038553 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/kd_random_class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/semi_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-14 13:56:10.000000 kappadata-1.4.8/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.042553 kappadata-1.4.8/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2023-12-14 13:58:01.000000 kappadata-1.4.8/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9391 2023-12-14 13:58:01.000000 kappadata-1.4.8/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 13:58:01.000000 kappadata-1.4.8/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-14 13:58:01.000000 kappadata-1.4.8/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-14 13:58:01.000000 kappadata-1.4.8/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-14 13:56:10.000000 kappadata-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-14 13:58:02.042553 kappadata-1.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.038553 kappadata-1.4.8/test_unit_long/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/test_unit_long/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2023-12-14 13:56:10.000000 kappadata-1.4.8/test_unit_long/test_stochastic_transform_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:58:02.038553 kappadata-1.4.8/tests_external_sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 13:56:10.000000 kappadata-1.4.8/tests_external_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2023-12-14 13:56:10.000000 kappadata-1.4.8/tests_external_sources/dinov2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-12-14 13:56:10.000000 kappadata-1.4.8/tests_external_sources/ijepa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.799449 kappadata-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-14 14:39:00.000000 kappadata-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10809 2023-12-14 14:40:48.799449 kappadata-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2023-12-14 14:39:00.000000 kappadata-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.763449 kappadata-1.4.9/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-14 14:40:35.000000 kappadata-1.4.9/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.763449 kappadata-1.4.9/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.767449 kappadata-1.4.9/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.767449 kappadata-1.4.9/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/base/kd_single_collator_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/kd_dino_mask_collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/kd_ijepa_mask_collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9500 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.767449 kappadata-1.4.9/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.767449 kappadata-1.4.9/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.767449 kappadata-1.4.9/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.767449 kappadata-1.4.9/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/mae_finetune_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/mugs_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_audioset_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_esc50_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_image_net_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_sid_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_speech_ccommands_v1_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/transforms/norm/kd_speech_ccommands_v2_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/mugs_multi_view_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/copying/copying_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/copying/create_zips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/copying/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.771449 kappadata-1.4.9/kappadata/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.775449 kappadata-1.4.9/kappadata/mock/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/mock/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/mock/datasets/audioset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/mock/datasets/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/mock/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.775449 kappadata-1.4.9/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.775449 kappadata-1.4.9/kappadata/samplers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/base/sampler_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/class_balanced_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/interleaved_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/semi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/sequential_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/samplers/weighted_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.783449 kappadata-1.4.9/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.783449 kappadata-1.4.9/kappadata/transforms/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/audio/kd_fbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/audio/kd_magnitude_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/audio/kd_roll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/audio/kd_spec_augment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.783449 kappadata-1.4.9/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_additive_uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_binarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_columnwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_minsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_random_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_simple_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_three_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_transform_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/kd_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.787449 kappadata-1.4.9/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/norm/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/patchify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/patchwise_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/save_state_to_context_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.787449 kappadata-1.4.9/kappadata/transforms/semseg/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/semseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/unpatchify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.791449 kappadata-1.4.9/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/getall_as_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/global_rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.791449 kappadata-1.4.9/kappadata/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_dataset_imgsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_mae_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_masked_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/visualization/visualize_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.791449 kappadata-1.4.9/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.795449 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/allgather_class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/class_groups_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/intra_class_shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/kd_pseudo_label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/random_superclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/sort_by_class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/swap_label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.795449 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.795449 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/kd_random_class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/semi_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-14 14:39:00.000000 kappadata-1.4.9/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.799449 kappadata-1.4.9/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10809 2023-12-14 14:40:48.000000 kappadata-1.4.9/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9391 2023-12-14 14:40:48.000000 kappadata-1.4.9/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 14:40:48.000000 kappadata-1.4.9/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-14 14:40:48.000000 kappadata-1.4.9/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-14 14:40:48.000000 kappadata-1.4.9/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-14 14:39:00.000000 kappadata-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-14 14:40:48.799449 kappadata-1.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.795449 kappadata-1.4.9/test_unit_long/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/test_unit_long/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2023-12-14 14:39:00.000000 kappadata-1.4.9/test_unit_long/test_stochastic_transform_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 14:40:48.795449 kappadata-1.4.9/tests_external_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 14:39:00.000000 kappadata-1.4.9/tests_external_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2023-12-14 14:39:00.000000 kappadata-1.4.9/tests_external_sources/dinov2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-12-14 14:39:00.000000 kappadata-1.4.9/tests_external_sources/ijepa.py
```

### Comparing `kappadata-1.4.8/LICENSE` & `kappadata-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/PKG-INFO` & `kappadata-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.4.8
+Version: 1.4.9
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.4.8/README.md` & `kappadata-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/__init__.py` & `kappadata-1.4.9/kappadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 
 import kappadata.caching
 import kappadata.collators
 import kappadata.common
 import kappadata.copying
 import kappadata.datasets
 import kappadata.loading
```

### Comparing `kappadata-1.4.8/kappadata/caching/cached_dataset.py` & `kappadata-1.4.9/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.4.9/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.4.9/kappadata/collators/base/kd_collator_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.4.9/kappadata/collators/base/kd_compose_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.4.9/kappadata/collators/base/kd_single_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/base/kd_single_collator_wrapper.py` & `kappadata-1.4.9/kappadata/collators/base/kd_single_collator_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/kd_dino_mask_collator.py` & `kappadata-1.4.9/kappadata/collators/kd_dino_mask_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/kd_ijepa_mask_collator.py` & `kappadata-1.4.9/kappadata/collators/kd_ijepa_mask_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/kd_mix_collator.py` & `kappadata-1.4.9/kappadata/collators/kd_mix_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.4.9/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.4.9/kappadata/common/datasets/kd_image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/transforms/byol_transforms.py` & `kappadata-1.4.9/kappadata/common/transforms/byol_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.4.9/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.4.9/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.4.9/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/transforms/mugs_transforms.py` & `kappadata-1.4.9/kappadata/common/transforms/mugs_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/transforms/norm/__init__.py` & `kappadata-1.4.9/kappadata/common/transforms/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/common/wrappers/sample_wrappers/mugs_multi_view_wrapper.py` & `kappadata-1.4.9/kappadata/common/wrappers/sample_wrappers/mugs_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/copying/copying_utils.py` & `kappadata-1.4.9/kappadata/copying/copying_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/copying/create_zips.py` & `kappadata-1.4.9/kappadata/copying/create_zips.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/copying/folder.py` & `kappadata-1.4.9/kappadata/copying/folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/copying/image_folder.py` & `kappadata-1.4.9/kappadata/copying/image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.4.9/kappadata/datasets/kd_concat_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/datasets/kd_dataset.py` & `kappadata-1.4.9/kappadata/datasets/kd_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/datasets/kd_subset.py` & `kappadata-1.4.9/kappadata/datasets/kd_subset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/datasets/kd_wrapper.py` & `kappadata-1.4.9/kappadata/datasets/kd_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/factory.py` & `kappadata-1.4.9/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/mock/datasets/audioset.py` & `kappadata-1.4.9/kappadata/mock/datasets/audioset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/mock/datasets/imagenet.py` & `kappadata-1.4.9/kappadata/mock/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/base/sampler_base.py` & `kappadata-1.4.9/kappadata/samplers/base/sampler_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/class_balanced_sampler.py` & `kappadata-1.4.9/kappadata/samplers/class_balanced_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/distributed_sampler.py` & `kappadata-1.4.9/kappadata/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.4.9/kappadata/samplers/infinite_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.4.9/kappadata/samplers/interleaved_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/random_sampler.py` & `kappadata-1.4.9/kappadata/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/semi_sampler.py` & `kappadata-1.4.9/kappadata/samplers/semi_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/samplers/weighted_sampler.py` & `kappadata-1.4.9/kappadata/samplers/weighted_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/__init__.py` & `kappadata-1.4.9/kappadata/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/audio/kd_fbank.py` & `kappadata-1.4.9/kappadata/transforms/audio/kd_fbank.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/audio/kd_magnitude_jitter.py` & `kappadata-1.4.9/kappadata/transforms/audio/kd_magnitude_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/audio/kd_spec_augment.py` & `kappadata-1.4.9/kappadata/transforms/audio/kd_spec_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.4.9/kappadata/transforms/base/kd_compose_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.4.9/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.4.9/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/base/kd_transform.py` & `kappadata-1.4.9/kappadata/transforms/base/kd_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.4.9/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.4.9/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_additive_gaussian_noise.py` & `kappadata-1.4.9/kappadata/transforms/kd_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_additive_uniform_noise.py` & `kappadata-1.4.9/kappadata/transforms/kd_additive_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_bucketize.py` & `kappadata-1.4.9/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.4.9/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_columnwise_norm.py` & `kappadata-1.4.9/kappadata/transforms/kd_columnwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.4.9/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.4.9/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_minsize.py` & `kappadata-1.4.9/kappadata/transforms/kd_minsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.4.9/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_additive_gaussian_noise.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_apply.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_apply.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_crop.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_grayscale.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_random_threshold.py` & `kappadata-1.4.9/kappadata/transforms/kd_random_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_resize.py` & `kappadata-1.4.9/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_simple_random_crop.py` & `kappadata-1.4.9/kappadata/transforms/kd_simple_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_solarize.py` & `kappadata-1.4.9/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_three_augment.py` & `kappadata-1.4.9/kappadata/transforms/kd_three_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_threshold.py` & `kappadata-1.4.9/kappadata/transforms/kd_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_transform_choice.py` & `kappadata-1.4.9/kappadata/transforms/kd_transform_choice.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/kd_two_random_crop.py` & `kappadata-1.4.9/kappadata/transforms/kd_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.4.9/kappadata/transforms/norm/kd_image_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.4.9/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/norm/kd_norm_base.py` & `kappadata-1.4.9/kappadata/transforms/norm/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/patchify.py` & `kappadata-1.4.9/kappadata/transforms/patchify.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/patchify_image.py` & `kappadata-1.4.9/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/patchwise_norm.py` & `kappadata-1.4.9/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.4.9/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/patchwise_transform.py` & `kappadata-1.4.9/kappadata/transforms/patchwise_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_pad.py` & `kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_pad.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_random_crop.py` & `kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_random_resize.py` & `kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_random_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/transforms/semseg/kd_semseg_resize.py` & `kappadata-1.4.9/kappadata/transforms/semseg/kd_semseg_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/bounding_box_utils.py` & `kappadata-1.4.9/kappadata/utils/bounding_box_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/class_counts.py` & `kappadata-1.4.9/kappadata/utils/class_counts.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/color_histogram.py` & `kappadata-1.4.9/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/getall_as_tensor.py` & `kappadata-1.4.9/kappadata/utils/getall_as_tensor.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/hash_utils.py` & `kappadata-1.4.9/kappadata/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/magnitude_sampler.py` & `kappadata-1.4.9/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/multi_crop_utils.py` & `kappadata-1.4.9/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/pos_embed.py` & `kappadata-1.4.9/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/random.py` & `kappadata-1.4.9/kappadata/utils/random.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/save_image.py` & `kappadata-1.4.9/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/utils/transform_utils.py` & `kappadata-1.4.9/kappadata/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_dataset_imgsize.py` & `kappadata-1.4.9/kappadata/visualization/visualize_dataset_imgsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_interpolation.py` & `kappadata-1.4.9/kappadata/visualization/visualize_interpolation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_jigsaw.py` & `kappadata-1.4.9/kappadata/visualization/visualize_jigsaw.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_mae_schematic.py` & `kappadata-1.4.9/kappadata/visualization/visualize_mae_schematic.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_masked_image.py` & `kappadata-1.4.9/kappadata/visualization/visualize_masked_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_transform.py` & `kappadata-1.4.9/kappadata/visualization/visualize_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/visualization/visualize_two_random_crop.py` & `kappadata-1.4.9/kappadata/visualization/visualize_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/__init__.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/allgather_class_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/allgather_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/class_groups_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/class_groups_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/intra_class_shuffle_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/intra_class_shuffle_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/kd_pseudo_label_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/kd_pseudo_label_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,16 +76,14 @@
 
     # noinspection PyUnusedLocal
     def getitem_confidence(self, idx, ctx=None):
         assert self.topk is None and self.tau is None, "geitem_confidence requires static pseudo labels"
         assert self.threshold is None
         assert self.confidences is not None
         confidence = self.confidences[idx]
-        if torch.is_tensor(confidence):
-            confidence = confidence.item()
         return confidence
 
     def _getitem_class(self, idx):
         if self.seed is not None:
             # static pseudo labels (they dont change from epoch to epoch)
             rng = np.random.default_rng(seed=self.seed + idx)
         else:
```

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/random_superclass_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/random_superclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/dataset_wrappers/swap_label_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/dataset_wrappers/swap_label_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/mode_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/mode_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/__init__.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/kd_random_class_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/kd_random_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/semi_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/semi_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.4.9/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/kappadata.egg-info/PKG-INFO` & `kappadata-1.4.9/kappadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.4.8
+Version: 1.4.9
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.4.8/kappadata.egg-info/SOURCES.txt` & `kappadata-1.4.9/kappadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/setup.cfg` & `kappadata-1.4.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.4.8
+version = 1.4.9
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

### Comparing `kappadata-1.4.8/test_unit_long/test_stochastic_transform_seed.py` & `kappadata-1.4.9/test_unit_long/test_stochastic_transform_seed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/tests_external_sources/dinov2.py` & `kappadata-1.4.9/tests_external_sources/dinov2.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.4.8/tests_external_sources/ijepa.py` & `kappadata-1.4.9/tests_external_sources/ijepa.py`

 * *Files identical despite different names*

