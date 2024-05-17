# Comparing `tmp/nostr_dvm-0.4.0.tar.gz` & `tmp/nostr_dvm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.4.0.tar", last modified: Thu May 16 10:47:46 2024, max compression
+gzip compressed data, was "nostr_dvm-0.4.1.tar", last modified: Fri May 17 08:36:20 2024, max compression
```

## Comparing `nostr_dvm-0.4.0.tar` & `nostr_dvm-0.4.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.584154 nostr_dvm-0.4.0/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.584154 nostr_dvm-0.4.0/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.584154 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.584154 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.588154 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39785 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.592154 nostr_dvm-0.4.0/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.596154 nostr_dvm-0.4.0/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 10:47:46.000000 nostr_dvm-0.4.0/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-16 10:47:46.000000 nostr_dvm-0.4.0/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:47:46.000000 nostr_dvm-0.4.0/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 10:47:46.000000 nostr_dvm-0.4.0/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 10:47:46.000000 nostr_dvm-0.4.0/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:47:46.600154 nostr_dvm-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 10:47:43.000000 nostr_dvm-0.4.0/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.023416 nostr_dvm-0.4.1/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39785 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.039416 nostr_dvm-0.4.1/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13177 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.039416 nostr_dvm-0.4.1/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.039416 nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/tests/test_events.py
```

### Comparing `nostr_dvm-0.4.0/LICENSE` & `nostr_dvm-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/PKG-INFO` & `nostr_dvm-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.4.0
+Version: 0.4.1
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.4.0/README.md` & `nostr_dvm-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/bot.py` & `nostr_dvm-0.4.1/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/dvm.py` & `nostr_dvm-0.4.1/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.4.1/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/subscription.py` & `nostr_dvm-0.4.1/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,19 +43,27 @@
         opts = {
             "max_results": 200,
         }
         self.request_form['options'] = json.dumps(opts)
 
         self.last_schedule = Timestamp.now().as_secs()
 
+        if self.options.get("db_name"):
+            self.db_name = self.options.get("db_name")
+        if self.options.get("db_since"):
+            self.db_since = int(self.options.get("db_since"))
+
+
         use_logger = False
         if use_logger:
             init_logger(LogLevel.DEBUG)
 
-        self.sync_db()
+        if self.dvm_config.UPDATE_DATABASE:
+            self.sync_db()
+
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
@@ -113,24 +121,24 @@
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
         # Negentropy reconciliation
         # Query events from database
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
-        lasthour = Timestamp.from_secs(timestamp_hour_ago)
+        since = Timestamp.from_secs(timestamp_hour_ago)
 
-        filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(lasthour)
+        filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
         events = cli.database().query([filter1])
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
                 filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
                                        definitions.EventDefinitions.KIND_REACTION,
-                                       definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
+                                       definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
                 reactions = cli.database().query([filt])
                 if len(reactions) >= self.min_reactions:
                     ns.finallist[event.id().to_hex()] = len(reactions)
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
@@ -152,15 +160,16 @@
         return result
 
     def schedule(self, dvm_config):
         if dvm_config.SCHEDULE_UPDATES_SECONDS == 0:
             return 0
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
-                self.sync_db()
+                if self.dvm_config.UPDATE_DATABASE:
+                    self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
                 self.result = self.calculate_result(self.request_form)
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
@@ -189,19 +198,20 @@
         print(
             "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, processing_msg=None):
+def build_example(name, identifier, admin_config, options, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
@@ -230,22 +240,23 @@
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     #admin_config.UPDATE_PROFILE = False
     #admin_config.REBROADCAST_NIP89 = False
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                          admin_config=admin_config)
+                                          admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, processing_msg=None):
+def build_example_subscription(name, identifier, admin_config, options, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
-    dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.SCHEDULE_UPDATES_SECONDS = 180  # Every 3 minutes
+    dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
 
@@ -291,13 +302,13 @@
     #admin_config.REBROADCAST_NIP88 = False
 
     # admin_config.FETCH_NIP88 = True
     # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
     # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                          nip88config=nip88config,
+                                          nip88config=nip88config, options=options,
                                           admin_config=admin_config)
 
 
 if __name__ == '__main__':
     process_venv(DicoverContentCurrentlyPopular)
```

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,25 @@
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
         self.last_schedule = Timestamp.now().as_secs()
 
+        if self.options.get("db_name"):
+            self.db_name = self.options.get("db_name")
+        if self.options.get("db_since"):
+            self.db_since = int(self.options.get("db_since"))
+
         use_logger = False
         if use_logger:
             init_logger(LogLevel.DEBUG)
 
-        self.sync_db()
+        if self.dvm_config.UPDATE_DATABASE:
+            self.sync_db()
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
@@ -97,30 +103,30 @@
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
         database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
         cli.add_relay("wss://relay.damus.io")
         cli.add_relay("wss://nos.lol")
-        cli.add_relay("wss://pablof7z.nostr1.com")
+        cli.add_relay("wss://nostr.mom")
 
         ropts = RelayOptions().ping(False)
         cli.add_relay_with_opts("wss://nostr.band", ropts)
 
         cli.connect()
 
         user = PublicKey.parse(options["user"])
         followers_filter = Filter().author(user).kinds([Kind(3)])
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
         #print(followers)
 
         # Negentropy reconciliation
         # Query events from database
-        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
-        lasthour = Timestamp.from_secs(timestamp_hour_ago)
+        timestamp_since = Timestamp.now().as_secs() - self.db_since
+        since = Timestamp.from_secs(timestamp_since)
 
 
         result_list = []
 
         if len(followers) > 0:
             newest = 0
             best_entry = followers[0]
@@ -132,26 +138,26 @@
             #print(best_entry.as_json())
             followings = []
             for tag in best_entry.tags():
                 if tag.as_vec()[0] == "p":
                     following = PublicKey.parse(tag.as_vec()[1])
                     followings.append(following)
 
-            filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).authors(followings).since(lasthour)
+            filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).authors(followings).since(since)
             events = cli.database().query([filter1])
 
             ns.finallist = {}
             for event in events:
-                if event.created_at().as_secs() > timestamp_hour_ago:
-                    filt = Filter().kinds(
-                        [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_REPOST,
-                         definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
-                    reactions = cli.database().query([filt])
-                    if len(reactions) >= self.min_reactions:
-                        ns.finallist[event.id().to_hex()] = len(reactions)
+                #if event.created_at().as_secs() > timestamp_since:
+                filt = Filter().kinds(
+                    [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_REPOST,
+                     definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
+                reactions = cli.database().query([filt])
+                if len(reactions) >= self.min_reactions:
+                    ns.finallist[event.id().to_hex()] = len(reactions)
 
 
 
             finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
             for entry in finallist_sorted:
                 # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
                 e_tag = Tag.parse(["e", entry[0]])
@@ -173,15 +179,16 @@
     def schedule(self, dvm_config):
         if dvm_config.SCHEDULE_UPDATES_SECONDS == 0:
             return 0
         # We simply use the db from the other dvm that contains all notes
 
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
-                self.sync_db()
+                if self.dvm_config.UPDATE_DATABASE:
+                    self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
@@ -207,19 +214,20 @@
 
         print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, processing_msg=None):
+def build_example(name, identifier, admin_config, options, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
@@ -246,23 +254,24 @@
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     # admin_config.UPDATE_PROFILE = False
     # admin_config.REBROADCAST_NIP89 = False
 
-    return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
+    return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config, options=options,
                                                    admin_config=admin_config)
 
 
-def build_example_subscription(name, identifier, admin_config, processing_msg=None):
+def build_example_subscription(name, identifier, admin_config, options, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
-    dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.SCHEDULE_UPDATES_SECONDS = 180  # Every 3 minutes
+    dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
 
     # Add NIP89
     nip89info = {
@@ -301,13 +310,13 @@
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
     # admin_config.FETCH_NIP88 = True
     # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
     # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
     return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                                   nip88config=nip88config,
+                                                   nip88config=nip88config, options=options,
                                                    admin_config=admin_config)
 
 
 if __name__ == '__main__':
     process_venv(DicoverContentCurrentlyPopularFollowers)
```

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             self.db_since = int(self.options.get("db_since"))
 
 
         use_logger = False
         if use_logger:
             init_logger(LogLevel.DEBUG)
 
-        self.sync_db()
+        if self.dvm_config.UPDATE_DATABASE:
+            self.sync_db()
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
@@ -145,29 +146,32 @@
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
         # Negentropy reconciliation
         # Query events from database
+        timestamp_since = Timestamp.now().as_secs() - self.db_since
+        since = Timestamp.from_secs(timestamp_since)
 
-        filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE)
+        filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
 
         events = cli.database().query([filter1])
         print(len(events))
         ns.finallist = {}
 
         for event in events:
             if all(ele in event.content().lower() for ele in self.must_list):
                 if any(ele in event.content().lower() for ele in self.search_list):
                     if not any(ele in event.content().lower() for ele in self.avoid_list):
+
                         filt = Filter().kinds(
                             [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION,
                              definitions.EventDefinitions.KIND_REPOST,
-                             definitions.EventDefinitions.KIND_NOTE]).event(event.id())
+                             definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
                         reactions = cli.database().query([filt])
                         if len(reactions) >= self.min_reactions:
                             ns.finallist[event.id().to_hex()] = len(reactions)
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
@@ -179,54 +183,66 @@
 
 
     def schedule(self, dvm_config):
         if dvm_config.SCHEDULE_UPDATES_SECONDS == 0:
             return 0
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
-                self.sync_db()
+                if self.dvm_config.UPDATE_DATABASE:
+                    self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
                 self.result = self.calculate_result(self.request_form)
                 #print(self.result)
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
+        cli.add_relay("wss://nostr.oxtr.dev")
+        cli.add_relay("wss://relay.nostr.net")
+        cli.add_relay("wss://relay.nostr.bg")
+        cli.add_relay("wss://nostr.wine")
+        cli.add_relay("wss://nostr21.com")
+
+        #RELAY_LIST = [ "wss://nostr.wine",
+        #              , "wss://relay.nostr.bg",
+        #              , "wss://relay.nostr.net"
+        #              ]
         cli.connect()
 
-        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
-        lasthour = Timestamp.from_secs(timestamp_hour_ago)
+        timestamp_since = Timestamp.now().as_secs() - self.db_since
+        since = Timestamp.from_secs(timestamp_since)
 
-        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
+        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_ZAP]).since(since)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
         print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
         database.delete(Filter().until(Timestamp.from_secs(
             Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesn't get too full.
 
         print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options, image, description, processing_msg=None):
+def build_example(name, identifier, admin_config, options, image, description, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
@@ -254,19 +270,20 @@
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, options, image, description, processing_msg=None):
+def build_example_subscription(name, identifier, admin_config, options, image, description, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
 
     # Add NIP89
```

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/dvmconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PRIVATE_KEY: str = ""
     PUBLIC_KEY: str = ""
     FIX_COST: float = None
     PER_UNIT_COST: float = None
 
     RELAY_LIST = ["wss://relay.damus.io", "wss://nos.lol", "wss://nostr.wine",
                   "wss://nostr.mom", "wss://nostr.oxtr.dev", "wss://relay.nostr.bg",
-                  "wss://relay.f7z.io", "wss://pablof7z.nostr1.com", "wss://relay.nostr.net", "wss://140.f7z.io",
+                  "wss://relay.f7z.io", "wss://relay.nostr.net"
                   ]
 
     RELAY_TIMEOUT = 5
     EXTERNAL_POST_PROCESS_TYPE = PostProcessFunctionType.NONE  # Leave this on None, except the DVM is external
     LNBITS_INVOICE_KEY = ''  # Will all automatically generated by default, or read from .env
     LNBITS_ADMIN_KEY = ''  # In order to pay invoices, e.g. from the bot to DVMs, or reimburse users.
     LNBITS_URL = 'https://lnbits.com'
@@ -34,14 +34,15 @@
     NEW_USER_BALANCE: int = 0  # Free credits for new users
     SUBSCRIPTION_MANAGEMENT = 'https://noogle.lol/discovery'
     NIP88: NIP88Config
     NIP89: NIP89Config
     SEND_FEEDBACK_EVENTS = True
     SHOW_RESULT_BEFORE_PAYMENT: bool = False  # if this is true show results even when not paid right after autoprocess
     SCHEDULE_UPDATES_SECONDS = 0
+    UPDATE_DATABASE = True  # DVMs that use a db manage their db by default. If a dvm should use the same db as another DVM, deactive it for those who do.
     CUSTOM_PROCESSING_MESSAGE = None
 
 
 def build_default_config(identifier):
     dvm_config = DVMConfig()
     dvm_config.PRIVATE_KEY = check_and_set_private_key(identifier)
     dvm_config.IDENTIFIER = identifier
```

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.4.1/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.4.1/nostr_dvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.4.0
+Version: 0.4.1
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.4.0/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.4.1/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/setup.py` & `nostr_dvm-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.4.0/tests/test_dvm_client.py` & `nostr_dvm-0.4.1/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.0/tests/test_events.py` & `nostr_dvm-0.4.1/tests/test_events.py`

 * *Files identical despite different names*

