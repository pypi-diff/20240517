# Comparing `tmp/nostr_dvm-0.4.1.tar.gz` & `tmp/nostr_dvm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.4.1.tar", last modified: Fri May 17 08:36:20 2024, max compression
+gzip compressed data, was "nostr_dvm-0.4.2.tar", last modified: Fri May 17 08:54:26 2024, max compression
```

## Comparing `nostr_dvm-0.4.1.tar` & `nostr_dvm-0.4.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.023416 nostr_dvm-0.4.1/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.027416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39785 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.031416 nostr_dvm-0.4.1/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.039416 nostr_dvm-0.4.1/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13177 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.039416 nostr_dvm-0.4.1/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.039416 nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 08:36:20.000000 nostr_dvm-0.4.1/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:20.043416 nostr_dvm-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-17 08:36:14.000000 nostr_dvm-0.4.1/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.446890 nostr_dvm-0.4.2/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.446890 nostr_dvm-0.4.2/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.446890 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.446890 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.446890 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39785 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.450890 nostr_dvm-0.4.2/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13177 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 08:54:26.000000 nostr_dvm-0.4.2/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-17 08:54:26.000000 nostr_dvm-0.4.2/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:54:26.000000 nostr_dvm-0.4.2/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 08:54:26.000000 nostr_dvm-0.4.2/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 08:54:26.000000 nostr_dvm-0.4.2/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:54:26.458890 nostr_dvm-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-17 08:54:17.000000 nostr_dvm-0.4.2/tests/test_events.py
```

### Comparing `nostr_dvm-0.4.1/LICENSE` & `nostr_dvm-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/PKG-INFO` & `nostr_dvm-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.4.1
+Version: 0.4.2
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.4.1/README.md` & `nostr_dvm-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.4.2/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/bot.py` & `nostr_dvm-0.4.2/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/dvm.py` & `nostr_dvm-0.4.2/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.4.2/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/subscription.py` & `nostr_dvm-0.4.2/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,21 +40,26 @@
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
         print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
+        max_results = 200
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
+            elif tag.as_vec()[0] == 'param':
+                param = tag.as_vec()[1]
+                if param == "max_results":  # check for param type
+                    max_results = int(tag.as_vec()[2])
 
         options = {
-
+            "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         options = DVMTaskInterface.set_options(request_form)
 
@@ -65,15 +70,15 @@
             response = requests.get(url)
             response_json = response.json()
             result_list = []
             i = 0
             if len(response_json["notes"]) > 0:
                 for note in response_json["notes"]:
                     i += 1
-                    if i < 20:
+                    if i < int(options["max_results"]):
                         e_tag = Tag.parse(["e", note["id"]])
                         #print(e_tag.as_vec())
                         result_list.append(e_tag.as_vec())
                     else:
                         break
 
             return json.dumps(result_list)
```

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.4.2/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.4.2/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.4.2/nostr_dvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.4.1
+Version: 0.4.2
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.4.1/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.4.2/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/setup.py` & `nostr_dvm-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.1'
+VERSION = '0.4.2'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.4.1/tests/test_dvm_client.py` & `nostr_dvm-0.4.2/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.1/tests/test_events.py` & `nostr_dvm-0.4.2/tests/test_events.py`

 * *Files identical despite different names*

