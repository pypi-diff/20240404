# Comparing `tmp/nostr-dvm-0.3.0.tar.gz` & `tmp/nostr-dvm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr-dvm-0.3.0.tar", last modified: Fri Mar 22 16:08:21 2024, max compression
+gzip compressed data, was "nostr-dvm-0.3.1.tar", last modified: Wed Apr  3 21:58:17 2024, max compression
```

## Comparing `nostr-dvm-0.3.0.tar` & `nostr-dvm-0.3.1.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.466750 nostr-dvm-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-22 16:08:21.466750 nostr-dvm-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39271 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.458751 nostr-dvm-0.3.0/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_relevant_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 16:08:21.466750 nostr-dvm-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.467745 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39387 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.471746 nostr-dvm-0.3.1/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.479745 nostr-dvm-0.3.1/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.479745 nostr-dvm-0.3.1/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 21:58:17.000000 nostr-dvm-0.3.1/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:58:17.483746 nostr-dvm-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-03 21:58:13.000000 nostr-dvm-0.3.1/tests/test_events.py
```

### Comparing `nostr-dvm-0.3.0/LICENSE` & `nostr-dvm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/PKG-INFO` & `nostr-dvm-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.0
+Version: 0.3.1
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr-dvm-0.3.0/README.md` & `nostr-dvm-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/utils.py` & `nostr-dvm-0.3.1/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/bot.py` & `nostr-dvm-0.3.1/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/dvm.py` & `nostr-dvm-0.3.1/nostr_dvm/dvm.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         signer = NostrSigner.keys(self.keys)
         self.client = Client.with_opts(signer, opts)
 
         self.job_list = []
         self.jobs_on_hold_list = []
         pk = self.keys.public_key()
 
-        print("Nostr DVM public key: " + str(pk.to_bech32()) + " Hex: " + str(pk.to_hex()) + "\n")
+        print("Nostr DVM public key: " + str(pk.to_bech32()) + " Hex: " + str(pk.to_hex()) + " Supported DVM tasks: " +
+              ', '.join(p.NAME + ":" + p.TASK for p in self.dvm_config.SUPPORTED_DVMS) + "\n")
 
         for relay in self.dvm_config.RELAY_LIST:
             self.client.add_relay(relay)
         self.client.connect()
 
         zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         kinds = [EventDefinitions.KIND_NIP90_GENERIC]
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr-dvm-0.3.1/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/subscription.py` & `nostr-dvm-0.3.1/nostr_dvm/subscription.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,321 +1,388 @@
 import json
-import math
 import os
 import signal
 import time
 from datetime import timedelta
 
-from nostr_sdk import (Keys, Client, Timestamp, Filter, nip04_decrypt, HandleNotification, EventBuilder, PublicKey,
-                       Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Nip19Event, nip44_decrypt, Kind)
+from nostr_sdk import (
+    Keys, Client, Timestamp, Filter, nip04_decrypt, HandleNotification, EventBuilder,
+    PublicKey, Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Kind
+)
 
 from nostr_dvm.utils.database_utils import fetch_user_metadata
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.nip88_utils import nip88_has_active_subscription
 from nostr_dvm.utils.nip89_utils import NIP89Config
+from nostr_dvm.utils.nostr_utils import send_event
 from nostr_dvm.utils.nwc_tools import nwc_zap
-from nostr_dvm.utils.subscription_utils import create_subscription_sql_table, add_to_subscription_sql_table, \
-    get_from_subscription_sql_table, update_subscription_sql_table, get_all_subscriptions_from_sql_table, \
-    delete_from_subscription_sql_table
+from nostr_dvm.utils.subscription_utils import (
+    create_subscription_sql_table, add_to_subscription_sql_table, get_from_subscription_sql_table,
+    update_subscription_sql_table, get_all_subscriptions_from_sql_table, delete_from_subscription_sql_table
+)
 from nostr_dvm.utils.zap_utils import create_bolt11_lud16, zaprequest
 
 
 class Subscription:
-    job_list: list
-
-    # This is a simple list just to keep track which events we created and manage, so we don't pay for other requests
     def __init__(self, dvm_config, admin_config=None):
         self.NAME = "Subscription Handler"
-        dvm_config.DB = "db/" + "subscriptions" + ".db"
+        dvm_config.DB = "db/subscriptions.db"
         self.dvm_config = dvm_config
         nip89config = NIP89Config()
         nip89config.NAME = self.NAME
         self.dvm_config.NIP89 = nip89config
         self.admin_config = admin_config
         self.keys = Keys.parse(dvm_config.PRIVATE_KEY)
         wait_for_send = False
         skip_disconnected_relays = True
         opts = (Options().wait_for_send(wait_for_send).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
                 .skip_disconnected_relays(skip_disconnected_relays))
         signer = NostrSigner.keys(self.keys)
         self.client = Client.with_opts(signer, opts)
 
-        pk = self.keys.public_key()
+        public_key = self.keys.public_key()
 
         self.job_list = []
 
-        print("Nostr Subscription Handler public key: " + str(pk.to_bech32()) + " Hex: " + str(
-            pk.to_hex()) + "\n")
+        print(f"Nostr Subscription Handler public key: {public_key.to_bech32()} Hex: {public_key.to_hex()}\n")
 
         for relay in self.dvm_config.RELAY_LIST:
             self.client.add_relay(relay)
         self.client.connect()
 
-        zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
+        zap_filter = Filter().pubkey(public_key).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         cancel_subscription_filter = Filter().kinds([EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT]).since(
             Timestamp.now())
         authors = []
         if admin_config is not None:
             for key in admin_config.USERNPUBS:
                 authors.append(PublicKey.parse(key))
-        dm_filter = Filter().authors(authors).pubkey(pk).kinds([EventDefinitions.KIND_DM]).since(Timestamp.now())
+        dvm_filter = Filter().authors(authors).pubkey(public_key).kinds([EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION]).since(Timestamp.now())
 
-        self.client.subscribe([zap_filter, dm_filter, cancel_subscription_filter], None)
+        self.client.subscribe([zap_filter, dvm_filter, cancel_subscription_filter], None)
 
         create_subscription_sql_table(dvm_config.DB)
 
+        self.client.handle_notifications(self.NotificationHandler(self))
 
-        class NotificationHandler(HandleNotification):
-            client = self.client
-            dvm_config = self.dvm_config
-            keys = self.keys
-
-            def handle(self, relay_url, subscription_id, nostr_event: Event):
-                if nostr_event.kind().as_u64() == EventDefinitions.KIND_DM.as_u64():
-                    print(nostr_event.as_json())
-                    handle_dm(nostr_event)
-                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT.as_u64():
-                    handle_cancel(nostr_event)
-
-            def handle_msg(self, relay_url, msg):
-                return
-
-        def handle_cancel(nostr_event):
-            print(nostr_event.as_json())
-            sender = nostr_event.author().to_hex()
-            kind7001eventid = ""
-            recipient = ""
-            if sender == self.keys.public_key().to_hex():
-                return
-
-            for tag in nostr_event.tags():
-                if tag.as_vec()[0] == "p":
-                    recipient = tag.as_vec()[1]
-                elif tag.as_vec()[0] == "e":
-                    kind7001eventid = tag.as_vec()[1]
-
-            if kind7001eventid != "":
-                subscription = get_from_subscription_sql_table(dvm_config.DB, kind7001eventid)
-
-                if subscription is not None:
-                    update_subscription_sql_table(dvm_config.DB, kind7001eventid, recipient,
-                                                  subscription.subscriber, subscription.nwc, subscription.cadence,
-                                                  subscription.amount, subscription.begin, subscription.end,
-                                                  subscription.tier_dtag, subscription.zaps, subscription.recipe,
-                                                  False, Timestamp.now().as_secs())
-
-        def infer_subscription_end_time(start, cadence):
-            end = start
-            if cadence == "daily":
-                end = start + 60 * 60 * 24
-            elif cadence == "weekly":
-                end = start + 60 * 60 * 24 * 7
-            elif cadence == "monthly":
-                # TODO check days of month -.-
-                end = start + 60 * 60 * 24 * 31
-            elif cadence == "yearly":
-                # TODO check extra day every 4 years
-                end = start + 60 * 60 * 24 * 356
-            return end
-
-        def pay_zap_split(nwc, overall_amount, zaps):
-            overallsplit = 0
-
-            for zap in zaps:
-                overallsplit += int(zap['split'])
-
-            zapped_amount = 0
-            for zap in zaps:
-                name, nip05, lud16 = fetch_user_metadata(zap['key'], self.client)
-                splitted_amount = math.floor(
-                    (int(zap['split']) / overallsplit) * int(overall_amount) / 1000)
-                # invoice = create_bolt11_lud16(lud16, splitted_amount)
-                # TODO add details about DVM in message
-                invoice = zaprequest(lud16, splitted_amount, "DVM subscription", None,
-                                     PublicKey.parse(zap['key']), self.keys, DVMConfig.RELAY_LIST)
-                print(invoice)
-                if invoice is not None:
-                    nwc_event_id = nwc_zap(nwc, invoice, self.keys, zap['relay'])
-                    if nwc_event_id is None:
-                        print("error zapping " + lud16)
-                    else:
-                        zapped_amount = zapped_amount + (splitted_amount * 1000)
-                        print(str(zapped_amount) + "/" + str(overall_amount))
+        try:
+            while True:
+                time.sleep(60.0)
+                self.check_subscriptions()
 
-            if zapped_amount < overall_amount * 0.8:  # TODO how do we handle failed zaps for some addresses? we are ok with 80% for now
-                success = False
-            else:
-                print("Zapped successfully")
-                success = True
-                # if no active subscription exists OR the subscription ended, pay
-
-            return success
-
-        def make_subscription_zap_recipe(event7001, recipient, subscriber, start, end, tier_dtag):
-            message = "payed by subscription service"
-            pTag = Tag.parse(["p", recipient])
-            PTag = Tag.parse(["P", subscriber])
-            eTag = Tag.parse(["e", event7001])
-            validTag = Tag.parse(["valid", str(start), str(end)])
-            tierTag = Tag.parse(["tier", tier_dtag])
-            alttag = Tag.parse(["alt", "This is a NIP90 DVM Subscription Payment Recipe"])
-
-            tags = [pTag, PTag, eTag, validTag, tierTag, alttag]
-
-            event = EventBuilder(EventDefinitions.KIND_NIP88_PAYMENT_RECIPE,
-                                 message, tags).to_event(self.keys)
-
-            dvmconfig = DVMConfig()
-            signer = NostrSigner.keys(self.keys)
-            client = Client(signer)
-            for relay in dvmconfig.RELAY_LIST:
-                client.add_relay(relay)
-            client.connect()
-            recipeid = client.send_event(event)
-            recipe = recipeid.to_hex()
-            return recipe
-
-        def handle_dm(nostr_event):
-
-            sender = nostr_event.author().to_hex()
-            if sender == self.keys.public_key().to_hex():
-                return
+        except KeyboardInterrupt:
+            print('Stay weird!')
+            os.kill(os.getpid(), signal.SIGTERM)
 
-            try:
-                decrypted_text = nip04_decrypt(self.keys.secret_key(), nostr_event.author(), nostr_event.content())
-                try:
-                    jsonevent = json.loads(decrypted_text)
-                    print(jsonevent)
-                    nwc = nip44_decrypt(self.keys.secret_key(), nostr_event.author(), jsonevent['nwc'])
-                    event7001 = jsonevent['subscribe_event']
-                    cadence = jsonevent['cadence']
-                    recipient = jsonevent['recipient']
-                    subscriber = jsonevent['subscriber']
-                    overall_amount = int(jsonevent['overall_amount'])
-                    tier_dtag = jsonevent['tier_dtag']
-
-                    start = Timestamp.now().as_secs()
-
-                    isactivesubscription = False
-                    recipe = ""
-
-                    subscription = get_from_subscription_sql_table(dvm_config.DB, event7001)
-                    #if subscription is not None and subscription.end > start:
-                    #    start = subscription.end
-                    #    isactivesubscription = True
-
-
-
-                    zapsstr = json.dumps(jsonevent['zaps'])
-                    print(zapsstr)
-                    success = True
-                    if subscription is None or subscription.end <= Timestamp.now().as_secs():
-                        #rather check nostr if our db is right
-                        subscription_status = nip88_has_active_subscription(
-                            PublicKey.parse(subscriber),
-                            tier_dtag, self.client, recipient, checkCanceled=False)
-
-                        if not subscription_status["isActive"]:
-                            success = pay_zap_split(nwc, overall_amount, jsonevent['zaps'])
-                            start = Timestamp.now().as_secs()
-                            end = infer_subscription_end_time(start, cadence)
-                        else:
-                            start = Timestamp.now().as_secs()
-                            end = subscription_status["validUntil"]
-                    else:
-                        start = subscription.begin
-                        end = subscription.end
-
-
-                    if success:
-                        recipe = make_subscription_zap_recipe(event7001, recipient, subscriber, start, end, tier_dtag)
-                        print("RECIPE " + recipe)
-                        isactivesubscription = True
-
-                    if subscription is None:
-                        add_to_subscription_sql_table(dvm_config.DB, event7001, recipient, subscriber, nwc,
-                                                      cadence, overall_amount, start, end, tier_dtag,
-                                                      zapsstr, recipe, isactivesubscription, Timestamp.now().as_secs())
-                        print("new subscription entry")
-                    else:
-                        update_subscription_sql_table(dvm_config.DB, event7001, recipient, subscriber, nwc,
-                                                      cadence, overall_amount, start, end,
-                                                      tier_dtag, zapsstr, recipe, isactivesubscription,
-                                                      Timestamp.now().as_secs())
-                        print("updated subscription entry")
+    def check_subscriptions(self):
+        subscriptions = get_all_subscriptions_from_sql_table(self.dvm_config.DB)
 
+        for subscription in subscriptions:
+            if subscription.active:
+                if subscription.end < Timestamp.now().as_secs():
+                    self.handle_subscription_renewal(subscription)
+            else:
+                self.handle_expired_subscription(subscription)
 
-                except Exception as e:
-                    print(e)
+        print(f"{Timestamp.now().as_secs()}: Checking {len(subscriptions)} Subscription entries..")
 
-            except Exception as e:
-                print("Error in Subscriber " + str(e))
+    def handle_subscription_renewal(self, subscription):
+        subscription_status = nip88_has_active_subscription(
+            PublicKey.parse(subscription.subscriber),
+            subscription.tier_dtag, self.client, subscription.recipent)
+
+        if subscription_status["expires"]:
+            update_subscription_sql_table(self.dvm_config.DB, subscription_status["subscriptionId"],
+                                          subscription.recipent,
+                                          subscription.subscriber, subscription.nwc,
+                                          subscription.cadence, subscription.amount, subscription.unit,
+                                          subscription.begin, subscription.end,
+                                          subscription.tier_dtag, subscription.zaps,
+                                          subscription.recipe,
+                                          False,
+                                          Timestamp.now().as_secs(), subscription.tier)
+        else:
+            zaps = json.loads(subscription.zaps)
+            success = self.pay_zap_split(subscription.nwc, subscription.amount, zaps, subscription.tier,
+                                         subscription.unit)
+            if success:
+                end = self.infer_subscription_end_time(Timestamp.now().as_secs(), subscription.cadence)
+                recipe = self.make_subscription_zap_recipe(subscription.id, subscription.recipent,
+                                                           subscription.subscriber, subscription.begin,
+                                                           end, subscription.tier_dtag)
+            else:
+                end = Timestamp.now().as_secs()
+                recipe = subscription.recipe
 
-        self.client.handle_notifications(NotificationHandler())
+            update_subscription_sql_table(self.dvm_config.DB, subscription.id,
+                                          subscription.recipent,
+                                          subscription.subscriber, subscription.nwc,
+                                          subscription.cadence, subscription.amount, subscription.unit,
+                                          subscription.begin, end,
+                                          subscription.tier_dtag, subscription.zaps, recipe,
+                                          success,
+                                          Timestamp.now().as_secs(), subscription.tier)
+
+            print("Updated subscription entry")
+
+            message = (f"Renewed Subscription to DVM {subscription.tier}. "
+                       f"Next renewal: {Timestamp.from_secs(end).to_human_datetime().replace('Z', ' ').replace('T', ' ')}")
+            self.send_direct_message(subscription.subscriber, message)
+
+    def handle_expired_subscription(self, subscription):
+        delete_threshold = 60 * 60 * 24 * 365
+        if subscription.cadence == "daily":
+            delete_threshold = 60 * 60 * 24 * 3  # After 3 days, delete the subscription, user can make a new one
+        elif subscription.cadence == "weekly":
+            delete_threshold = 60 * 60 * 24 * 21  # After 21 days, delete the subscription, user can make a new one
+        elif subscription.cadence == "monthly":
+            delete_threshold = 60 * 60 * 24 * 60  # After 60 days, delete the subscription, user can make a new one
+        elif subscription.cadence == "yearly":
+            delete_threshold = 60 * 60 * 24 * 500  # After 500 days, delete the subscription, user can make a new one
+
+        if subscription.end < (Timestamp.now().as_secs() - delete_threshold):
+            delete_from_subscription_sql_table(self.dvm_config.DB, subscription.id)
+            print("Deleted expired subscription")
+
+    def pay_zap_split(self, nwc, overall_amount, zaps, tier, unit="msats"):
+        overallsplit = sum(int(zap[3]) for zap in zaps)
+        zapped_amount = 0
+
+        for zap in zaps:
+            if zap[1] == "":
+                zap[1] = self.keys.public_key().to_hex()
+
+            name, nip05, lud16 = fetch_user_metadata(zap[1], self.client)
+            splitted_amount = int((int(zap[3]) / overallsplit) * int(overall_amount) / 1000)
+
+            invoice = zaprequest(lud16, splitted_amount, tier, None,
+                                 PublicKey.parse(zap[1]), self.keys, DVMConfig.RELAY_LIST)
+
+            if invoice is not None:
+                nwc_event_id = nwc_zap(nwc, invoice, self.keys, zap[2])
+                if nwc_event_id is None:
+                    print(f"Error zapping {lud16}")
+                else:
+                    zapped_amount += splitted_amount * 1000
+                    print(f"{zapped_amount}/{overall_amount}")
+
+        return zapped_amount >= overall_amount * 0.8
+
+    def make_subscription_zap_recipe(self, event7001, recipient, subscriber, start, end, tier_dtag):
+        message = "Paid by subscription service"
+        p_tag = Tag.parse(["p", recipient])
+        p_subscriber_tag = Tag.parse(["P", subscriber])
+        e_tag = Tag.parse(["e", event7001])
+        valid_tag = Tag.parse(["valid", str(start), str(end)])
+        tier_tag = Tag.parse(["tier", tier_dtag])
+        alt_tag = Tag.parse(["alt", "This is a NIP90 DVM Subscription Payment Recipe"])
+
+        tags = [p_tag, p_subscriber_tag, e_tag, valid_tag, tier_tag, alt_tag]
+
+        event = EventBuilder(EventDefinitions.KIND_NIP88_PAYMENT_RECIPE,
+                             message, tags).to_event(self.keys)
+
+        recipeid = self.client.send_event(event)
+        recipe = recipeid.to_hex()
+        return recipe
+
+    def infer_subscription_end_time(self, start, cadence):
+        end = start
+        if cadence == "daily":
+            end = start + 60 * 60 * 24
+        elif cadence == "weekly":
+            end = start + 60 * 60 * 24 * 7
+        elif cadence == "monthly":
+            end = start + 60 * 60 * 24 * 31
+        elif cadence == "yearly":
+            end = start + 60 * 60 * 24 * 356
+        return end
+
+    def send_direct_message(self, recipient, message):
+        evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.parse(recipient), message, None).to_event(
+            self.keys)
+        send_event(evt, client=self.client, dvm_config=self.dvm_config)
+
+    class NotificationHandler(HandleNotification):
+        def __init__(self, subscription):
+            self.subscription = subscription
+
+        def handle(self, relay_url, subscription_id, nostr_event: Event):
+            if nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION.as_u64():
+                self.subscription.handle_nwc_request(nostr_event)
+            elif nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT.as_u64():
+                self.subscription.handle_cancel(nostr_event)
+
+        def handle_msg(self, relay_url, msg):
+            pass
+
+    def send_status_success(self, original_event, domain):
+
+        e_tag = Tag.parse(["e", original_event.id().to_hex()])
+        p_tag = Tag.parse(["p", original_event.author().to_hex()])
+        status_tag = Tag.parse(["status", "success", "Job has been scheduled, you can manage it on " + domain])
+        reply_tags = [status_tag]
+        encryption_tags = []
+
+        encrypted_tag = Tag.parse(["encrypted"])
+        encryption_tags.append(encrypted_tag)
+        encryption_tags.append(p_tag)
+        encryption_tags.append(e_tag)
+
+        str_tags = []
+        for element in reply_tags:
+            str_tags.append(element.as_vec())
+
+        content = json.dumps(str_tags)
+        content = nip04_encrypt(self.keys.secret_key(), PublicKey.from_hex(original_event.author().to_hex()),
+                                content)
+        reply_tags = encryption_tags
+
+        keys = Keys.parse(self.dvm_config.PRIVATE_KEY)
+        reaction_event = EventBuilder(EventDefinitions.KIND_FEEDBACK, str(content), reply_tags).to_event(keys)
+        send_event(reaction_event, client=self.client, dvm_config=self.dvm_config)
+
+    def handle_cancel(self, nostr_event):
+        print(nostr_event.as_json())
+        sender = nostr_event.author().to_hex()
+        if sender == self.keys.public_key().to_hex():
+            return
+
+        kind7001eventid = ""
+        recipient = ""
+        for tag in nostr_event.tags():
+            if tag.as_vec()[0] == "p":
+                recipient = tag.as_vec()[1]
+            elif tag.as_vec()[0] == "e":
+                kind7001eventid = tag.as_vec()[1]
+
+        if kind7001eventid != "":
+            subscription = get_from_subscription_sql_table(self.dvm_config.DB, kind7001eventid)
+
+            if subscription is not None:
+                update_subscription_sql_table(self.dvm_config.DB, kind7001eventid, recipient,
+                                              subscription.subscriber, subscription.nwc, subscription.cadence,
+                                              subscription.amount, subscription.unit, subscription.begin,
+                                              subscription.end,
+                                              subscription.tier_dtag, subscription.zaps, subscription.recipe,
+                                              False, Timestamp.now().as_secs(), subscription.tier)
+
+    def handle_nwc_request(self, nostr_event):
+        print(nostr_event.as_json())
+        sender = nostr_event.author().to_hex()
+        if sender == self.keys.public_key().to_hex():
+            return
 
         try:
-            while True:
-                time.sleep(60.0)
-                subscriptions = get_all_subscriptions_from_sql_table(dvm_config.DB)
-
-                for subscription in subscriptions:
-                    if subscription.active:
-                        if subscription.end < Timestamp.now().as_secs():
-                            # We could directly zap, but let's make another check if our subscription expired
-                            subscription_status = nip88_has_active_subscription(
-                                PublicKey.parse(subscription.subscriber),
-                                subscription.tier_dtag, self.client, subscription.recipent)
-
-                            if not subscription_status["isActive"] or subscription_status["expires"]:
-                                update_subscription_sql_table(dvm_config.DB, subscription.id,
-                                                              subscription.recipent,
-                                                              subscription.subscriber, subscription.nwc,
-                                                              subscription.cadence, subscription.amount,
-                                                              subscription.begin, subscription.end,
-                                                              subscription.tier_dtag, subscription.zaps,
-                                                              subscription.recipe,
-                                                              False,
-                                                              Timestamp.now().as_secs())
-                            else:
-                                zaps = json.loads(subscription.zaps)
-                                success = pay_zap_split(subscription.nwc, subscription.amount, zaps)
-                                if success:
-                                    end = infer_subscription_end_time(Timestamp.now().as_secs(), subscription.cadence)
-                                    recipe = make_subscription_zap_recipe(subscription.id, subscription.recipent,
-                                                                          subscription.subscriber, subscription.begin,
-                                                                          end, subscription.tier_dtag)
-                                else:
-                                    end = Timestamp.now().as_secs()
-                                    recipe = subscription.recipe
-
-                                update_subscription_sql_table(dvm_config.DB, subscription.id,
-                                                              subscription.recipent,
-                                                              subscription.subscriber, subscription.nwc,
-                                                              subscription.cadence, subscription.amount,
-                                                              subscription.begin, end,
-                                                              subscription.tier_dtag, subscription.zaps, recipe,
-                                                              success,
-                                                              Timestamp.now().as_secs())
-                                print("updated subscription entry")
-
-
-                    else:
-                        delete_threshold = 60 * 60 * 24 * 365
-                        if subscription.cadence == "daily":
-                            delete_threshold = 60 * 60 * 24 * 3  # After 3 days, delete the subscription, user can make a new one
-                        elif subscription.cadence == "weekly":
-                            delete_threshold = 60 * 60 * 24 * 21  # After 21 days, delete the subscription, user can make a new one
-                        elif subscription.cadence == "monthly":
-                            delete_threshold = 60 * 60 * 24 * 60  # After 60 days, delete the subscription, user can make a new one
-                        elif subscription.cadence == "yearly":
-                            delete_threshold = 60 * 60 * 24 * 500  # After 500 days, delete the subscription, user can make a new one
-
-                        if subscription.end < (Timestamp.now().as_secs() - delete_threshold):
-                            delete_from_subscription_sql_table(dvm_config.DB, subscription.id)
-                            print("Delete expired subscription")
-
-                print(str(Timestamp.now().as_secs()) + ": Checking " + str(len(subscriptions)) + " Subscription entries..")
+            decrypted_text = nip04_decrypt(self.keys.secret_key(), nostr_event.author(), nostr_event.content())
+            try:
+                jsonevent = json.loads(decrypted_text)
+                nwc = ""
+                subscriber = ""
+                for entry in jsonevent:
+                    if entry[1] == "nwc":
+                        nwc = entry[2]
+                    elif entry[1] == "p":
+                        subscriber = entry[2]
+
+                subscriptionfilter = Filter().kind(EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT).author(
+                    PublicKey.parse(subscriber)).limit(1)
+                evts = self.client.get_events_of([subscriptionfilter], timedelta(seconds=3))
 
-        except KeyboardInterrupt:
-            print('Stay weird!')
-            os.kill(os.getpid(), signal.SIGTERM)
+                if len(evts) > 0:
+                    self.process_subscription_event(evts[0], nwc, subscriber)
+            except Exception as e:
+                print(f"Error processing JSON event: {e}")
+        except Exception as e:
+            print(f"Error decrypting event content: {e}")
+
+    def process_subscription_event(self, subscription_event, nwc, subscriber):
+        event7001id = subscription_event.id().to_hex()
+        tier_dtag = ""
+        recipient = ""
+        cadence = ""
+        unit = "msats"
+        zaps = []
+        tier = "DVM"
+        overall_amount = 0
+        subscription_event_id = ""
+
+        for tag in subscription_event.tags():
+            if tag.as_vec()[0] == "amount":
+                overall_amount = int(tag.as_vec()[1])
+                unit = tag.as_vec()[2]
+                cadence = tag.as_vec()[3]
+                print(f"{overall_amount} {unit} {cadence}")
+            elif tag.as_vec()[0] == "p":
+                recipient = tag.as_vec()[1]
+            elif tag.as_vec()[0] == "e":
+                subscription_event_id = tag.as_vec()[1]
+            elif tag.as_vec()[0] == "event":
+                jsonevent = json.loads(tag.as_vec()[1])
+                subscription_event = Event.from_json(jsonevent)
+
+                for tag in subscription_event.tags():
+                    if tag.as_vec()[0] == "d":
+                        tier_dtag = tag.as_vec()[1]
+                    elif tag.as_vec()[0] == "zap":
+                        zaps.append(tag.as_vec())
+                    elif tag.as_vec()[0] == "title":
+                        tier = tag.as_vec()[1]
+
+        if tier_dtag == "" or len(zaps) == 0:
+            tierfilter = Filter().id(EventId.parse(subscription_event_id))
+            evts = self.client.get_events_of([tierfilter], timedelta(seconds=3))
+            if len(evts) > 0:
+                for tag in evts[0].tags():
+                    if tag.as_vec()[0] == "d":
+                        tier_dtag = tag.as_vec()[0]
+
+        isactivesubscription = False
+        recipe = ""
+
+        subscription = get_from_subscription_sql_table(self.dvm_config.DB, event7001id)
+        zapsstr = json.dumps(zaps)
+        print(zapsstr)
+        success = True
+        if subscription is None or subscription.end <= Timestamp.now().as_secs():
+            # rather check nostr if our db is right
+            subscription_status = nip88_has_active_subscription(
+                PublicKey.parse(subscriber),
+                tier_dtag, self.client, recipient, checkCanceled=False)
+
+            if not subscription_status["isActive"]:
+
+                success = self.pay_zap_split(nwc, overall_amount, zaps, tier, unit)
+                start = Timestamp.now().as_secs()
+                end = self.infer_subscription_end_time(start, cadence)
+            else:
+                start = Timestamp.now().as_secs()
+                end = subscription_status["validUntil"]
+        else:
+            start = subscription.begin
+            end = subscription.end
+
+        if success:
+            recipe = self.make_subscription_zap_recipe(event7001id, recipient, subscriber, start, end,
+                                                       tier_dtag)
+            print("RECIPE " + recipe)
+            isactivesubscription = True
+
+        if subscription is None:
+            add_to_subscription_sql_table(self.dvm_config.DB, event7001id, recipient, subscriber, nwc,
+                                          cadence, overall_amount, unit, start, end, tier_dtag,
+                                          zapsstr, recipe, isactivesubscription,
+                                          Timestamp.now().as_secs(), tier)
+            print("new subscription entry")
+        else:
+            update_subscription_sql_table(self.dvm_config.DB, event7001id, recipient, subscriber, nwc,
+                                          cadence, overall_amount, unit, start, end,
+                                          tier_dtag, zapsstr, recipe, isactivesubscription,
+                                          Timestamp.now().as_secs(), tier)
+            print("updated subscription entry")
+
+        self.send_status_success(subscription_event, "noogle.lol")
+
+        message = ("Subscribed to DVM " + tier + ". Renewing on: " + str(
+            Timestamp.from_secs(end).to_human_datetime().replace("Z", " ").replace("T", " ")))
+        self.send_direct_message(subscriber, message)
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search_wine.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
-        "about": "I show notes that are currently popular, just like the free DVM, I'm also used for testing subscriptions. (beta)",
+        "about": "I show notes that are currently popular all over Nostr. I'm also used for testing subscriptions.",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "subscription": True,
         "nip90Params": {
             "max_results": {
                 "required": False,
@@ -246,15 +246,15 @@
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
     admin_config.UPDATE_PROFILE = False
-    admin_config.REBROADCAST_NIP89 = False
+    admin_config.REBROADCAST_NIP89 = True
     admin_config.REBROADCAST_NIP88 = False
 
    # admin_config.FETCH_NIP88 = True
    # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
    # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/convert_media.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imageinterrogator.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/imageupscale.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/search_users.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/search_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class SearchUser(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_USER_SEARCH
     TASK: str = "search-user"
     FIX_COST: float = 0
     dvm_config: DVMConfig
-    last_schedule: int
+    last_schedule: int = 0
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import re
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
@@ -62,15 +63,15 @@
                                                             EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
                                                             EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY],
                                                      dvm_config=dvm_config)
                     if evt is None:
                         print("Event not found")
                         raise Exception
                     
-                    if evt.kind() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
+                    if evt.kind().as_u64() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
                         result_list = json.loads(evt.content())
                         prompt = ""
                         for tag in result_list:
                             e_tag = Tag.parse(tag)
                             evt = get_event_by_id(e_tag.as_vec()[1], client=client, config=dvm_config)
                             prompt += evt.content() + "\n"
 
@@ -102,15 +103,17 @@
             sign.saveCookiesToDir(cookie_path_dir)
 
 
         options = DVMTaskInterface.set_options(request_form)
 
         try:
             chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
-            query_result = chatbot.query("Summarize the following notes: " + options["prompt"])
+            text = re.sub(r'^https?:\/\/.*[\r\n]*', '', str(options["prompt"]), flags=re.MULTILINE)
+
+            query_result = chatbot.query("Summarize the following notes: " + text[:3500])
             print(query_result["text"])  # or query_result.text or query_result["text"]
             return str(query_result["text"]).lstrip()
 
         except Exception as e:
             print("Error in Module: " + str(e))
             raise Exception(e)
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                                                             EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
                                                             EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY],
                                                      dvm_config=dvm_config)
                     if evt is None:
                         print("Event not found")
                         raise Exception
 
-                    if evt.kind() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
+                    if evt.kind().as_u64() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
                         result_list = json.loads(evt.content())
                         prompt = ""
                         for tag in result_list:
                             e_tag = Tag.parse(tag)
                             evt = get_event_by_id(e_tag.as_vec()[1], client=client, config=dvm_config)
                             prompt += evt.content() + "\n"
 
@@ -104,16 +104,17 @@
                 base_url='https://unleashed.chat/api/v1',
             )
 
             print('Models:\n')
 
             for model in client.models.list():
                 print('- ' + model.id)
+            text = re.sub(r'^https?:\/\/.*[\r\n]*', '', str(options["prompt"]), flags=re.MULTILINE)
 
-            content = "Summarize the following notes: " + str(options["prompt"])[:3500]
+            content = "Summarize the following notes: " + text[:3500]
             normal_stream = client.chat.completions.create(
                 messages=[
                     {
                         'role': 'user',
                         'content':content,
                     }
                 ],
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_google.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_pdf.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/texttospeech.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/translation_google.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/translation_libretranslate.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_svd.py` & `nostr-dvm-0.3.1/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/admin_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/backend_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/cashu_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/database_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/database_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,24 +209,14 @@
 
         update_sql_table(dvm_config.DB, npub, user.balance, user.iswhitelisted, user.isblacklisted, user.nip05,
                          user.lud16,
                          user.name,
                          Timestamp.now().as_secs(), subscribed_until)
         print("Updated user subscription for: " + str(user.name))
 
-        if dvm_config is not None:
-            keys = Keys.parse(dvm_config.PRIVATE_KEY)
-            # time.sleep(1.0)
-
-            message = ("Subscribed to DVM " + dvm_config.NIP89.NAME + " until: " + str(
-                Timestamp.from_secs(subscribed_until).to_human_datetime().replace("Z", " ").replace("T", " ")))
-
-            evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.from_hex(npub), message,
-                                                    None).to_event(keys)
-            send_event(evt, client=client, dvm_config=dvm_config)
 
 
 def get_or_add_user(db, npub, client, config, update=False, skip_meta = False):
     user = get_from_sql_table(db, npub)
     if user is None:
         try:
             if skip_meta:
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/definitions.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     KIND_NIP90_RESULT_CONTENT_DISCOVERY = Kind(6300)
     KIND_NIP90_PEOPLE_DISCOVERY = Kind(5301)
     KIND_NIP90_RESULT_PEOPLE_DISCOVERY = Kind(6301)
     KIND_NIP90_CONTENT_SEARCH = Kind(5302)
     KIND_NIP90_RESULTS_CONTENT_SEARCH = Kind(6302)
     KIND_NIP90_USER_SEARCH = Kind(5303)
     KIND_NIP90_RESULTS_USER_SEARCH = Kind(6303)
+    KIND_NIP90_DVM_SUBSCRIPTION = Kind(5906)
+    KIND_NIP90_RESULT_DVM_SUBSCRIPTION = Kind(6906)
+
     KIND_NIP90_GENERIC = Kind(5999)
     KIND_NIP90_RESULT_GENERIC = Kind(6999)
 
     KIND_NIP88_SUBSCRIBE_EVENT = Kind(7001)
     KIND_NIP88_STOP_SUBSCRIPTION_EVENT = Kind(7002)
     KIND_NIP88_PAYMENT_RECIPE = Kind(7003)
     KIND_NIP88_TIER_EVENT = Kind(37001)
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/dvmconfig.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/external_dvm_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/mediasource_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/nip88_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/nip89_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/nostr_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/nwc_tools.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/output_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/subscription_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/subscription_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 class Subscription:
     id: str
     recipent: str
     subscriber: str
     nwc: str
     cadence: str
     amount: int
+    unit: str
     begin: int
     end: int
     tier_dtag: str
     zaps: str
     recipe: str
     active: bool
     lastupdate: int
+    tier: str
 
 
 def create_subscription_sql_table(db):
     try:
         import os
         if not os.path.exists(r'db'):
             os.makedirs(r'db')
@@ -32,42 +34,44 @@
         cur.execute(""" CREATE TABLE IF NOT EXISTS subscriptions (
                                             id text PRIMARY KEY,
                                             recipient text,
                                             subscriber  text,
                                             nwc text NOT NULL,
                                             cadence text,
                                             amount int,
+                                            unit text,
                                             begin int,
                                             end int,
                                             tier_dtag text,
                                             zaps text,
                                             recipe text,
                                             active boolean,
-                                            lastupdate int
+                                            lastupdate int,
+                                            tier text
                                             
                                           
                                         ); """)
         cur.execute("SELECT name FROM sqlite_master")
         con.close()
 
     except Error as e:
         print(e)
 
 
-def add_to_subscription_sql_table(db, id, recipient, subscriber, nwc, cadence, amount, begin, end, tier_dtag, zaps,
-                                  recipe, active, lastupdate):
+def add_to_subscription_sql_table(db, id, recipient, subscriber, nwc, cadence, amount, unit, begin, end, tier_dtag, zaps,
+                                  recipe, active, lastupdate, tier):
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
-        data = (id, recipient, subscriber, nwc, cadence, amount, begin, end, tier_dtag, zaps, recipe, active, lastupdate)
+        data = (id, recipient, subscriber, nwc, cadence, amount, unit, begin, end, tier_dtag, zaps, recipe, active, lastupdate, tier)
         print(id)
         print(recipient)
         print(subscriber)
         print(nwc)
-        cur.execute("INSERT or IGNORE INTO subscriptions VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", data)
+        cur.execute("INSERT or IGNORE INTO subscriptions VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", data)
         con.commit()
         con.close()
     except Error as e:
         print("Error when Adding to DB: " + str(e))
 
 
 def get_from_subscription_sql_table(db, id):
@@ -83,21 +87,23 @@
             subscription = Subscription
             subscription.id = row[0]
             subscription.recipent = row[1]
             subscription.subscriber = row[2]
             subscription.nwc = row[3]
             subscription.cadence = row[4]
             subscription.amount = row[5]
-            subscription.begin = row[6]
-            subscription.end = row[7]
-            subscription.tier_dtag = row[8]
-            subscription.zaps = row[9]
-            subscription.recipe = row[10]
-            subscription.active = row[11]
-            subscription.lastupdate = row[12]
+            subscription.unit = row[6]
+            subscription.begin = row[7]
+            subscription.end = row[8]
+            subscription.tier_dtag = row[9]
+            subscription.zaps = row[10]
+            subscription.recipe = row[11]
+            subscription.active = row[12]
+            subscription.lastupdate = row[13]
+            subscription.tier = row[14]
 
             return subscription
 
     except Error as e:
         print("Error Getting from DB: " + str(e))
         return None
 
@@ -108,15 +114,15 @@
         cursor = con.cursor()
 
         sqlite_select_query = """SELECT * from subscriptions"""
         cursor.execute(sqlite_select_query)
         records = cursor.fetchall()
         subscriptions = []
         for row in records:
-            subscriptions.append(Subscription(row[0], row[1], row[2], row[3], row[4], row[5], row[6], row[7], row[8], row[9], row[10], row[11], row[12]))
+            subscriptions.append(Subscription(row[0], row[1], row[2], row[3], row[4], row[5], row[6], row[7], row[8], row[9], row[10], row[11], row[12], row[13], row[14]))
         cursor.close()
         return subscriptions
 
     except sqlite3.Error as error:
         print("Failed to read data from sqlite table", error)
     finally:
         if con:
@@ -129,34 +135,36 @@
         cur = con.cursor()
         cur.execute("DELETE FROM subscriptions WHERE id=?", (id,))
         con.commit()
         con.close()
     except Error as e:
         print(e)
 
-def update_subscription_sql_table(db, id, recipient, subscriber, nwc, cadence, amount, begin, end, tier_dtag, zaps,
-                                  recipe, active, lastupdate):
+def update_subscription_sql_table(db, id, recipient, subscriber, nwc, cadence, amount, unit, begin, end, tier_dtag, zaps,
+                                  recipe, active, lastupdate, tier):
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
-        data = (recipient, subscriber, nwc, cadence, amount, begin, end, tier_dtag, zaps, recipe, active, lastupdate, id)
+        data = (recipient, subscriber, nwc, cadence, amount, unit, begin, end, tier_dtag, zaps, recipe, active, lastupdate, tier, id)
 
         cur.execute(""" UPDATE subscriptions
                   SET recipient = ? ,
                       subscriber = ? ,
                       nwc = ? ,
                       cadence = ? ,
                       amount = ? ,
+                      unit = ? ,
                       begin = ? ,
                       end = ?,
                       tier_dtag = ?,
                       zaps = ?,
                       recipe = ?,
                       active = ?,
-                      lastupdate = ?
+                      lastupdate = ?,
+                      tier = ?
 
                   WHERE id = ?""", data)
         con.commit()
         con.close()
     except Error as e:
         print("Error Updating DB: " + str(e))
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm/utils/zap_utils.py` & `nostr-dvm-0.3.1/nostr_dvm/utils/zap_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import urllib.parse
 from pathlib import Path
 
 import requests
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 from bech32 import bech32_decode, convertbits, bech32_encode
-from nostr_sdk import nostr_sdk, PublicKey, SecretKey, Event, EventBuilder, Tag, Keys, generate_shared_key, Kind
+from nostr_sdk import nostr_sdk, PublicKey, SecretKey, Event, EventBuilder, Tag, Keys, generate_shared_key, Kind, \
+    Timestamp
 
 from nostr_dvm.utils.nostr_utils import get_event_by_id, check_and_decrypt_own_tags
 import lnurl
 from hashlib import sha256
 import dotenv
 
 # TODO tor connection to lnbits
@@ -264,35 +265,47 @@
             e_tag = Tag.parse(['e', zapped_event.id().to_hex()])
             tags = [amount_tag, relays_tag, p_tag, e_tag, lnurl_tag]
         else:
             p_tag = Tag.parse(['p', zapped_user.to_hex()])
             tags = [amount_tag, relays_tag, p_tag, lnurl_tag]
 
         if zaptype == "private":
-            key_str = keys.secret_key().to_hex() + zapped_event.id().to_hex() + str(zapped_event.created_at().as_secs())
-            encryption_key = sha256(key_str.encode('utf-8')).hexdigest()
+            if zapped_event is not None:
+                key_str = keys.secret_key().to_hex() + zapped_event.id().to_hex() + str(
+                    zapped_event.created_at().as_secs())
+
+            else:
+                key_str = keys.secret_key().to_hex() + str(Timestamp.now().as_secs())
 
+            encryption_key = sha256(key_str.encode('utf-8')).hexdigest()
+            tags = [p_tag]
+            if zapped_event is not None:
+                tags.append(e_tag)
             zap_request = EventBuilder(Kind(9733), content,
-                                       [p_tag, e_tag]).to_event(keys).as_json()
+                                       tags).to_event(keys).as_json()
             keys = Keys.parse(encryption_key)
-            encrypted_content = enrypt_private_zap_message(zap_request, keys.secret_key(), zapped_event.author())
+            if zapped_event is not None:
+                encrypted_content = enrypt_private_zap_message(zap_request, keys.secret_key(), zapped_event.author())
+            else:
+                encrypted_content = enrypt_private_zap_message(zap_request, keys.secret_key(), zapped_user)
+
             anon_tag = Tag.parse(['anon', encrypted_content])
             tags.append(anon_tag)
             content = ""
 
         zap_request = EventBuilder(Kind(9734), content,
                                    tags).to_event(keys).as_json()
 
         response = requests.get(callback + "?amount=" + str(int(amount) * 1000) + "&nostr=" + urllib.parse.quote_plus(
             zap_request) + "&lnurl=" + encoded_lnurl)
         ob = json.loads(response.content)
         return ob["pr"]
 
     except Exception as e:
-        print("ZAP REQUEST: " + e)
+        print("ZAP REQUEST: " + str(e))
         return None
 
 
 def get_price_per_sat(currency):
     import requests
 
     url = "https://openapiv1.coinstats.app/coins/bitcoin"
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm.egg-info/PKG-INFO` & `nostr-dvm-0.3.1/nostr_dvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.0
+Version: 0.3.1
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr-dvm-0.3.0/nostr_dvm.egg-info/SOURCES.txt` & `nostr-dvm-0.3.1/nostr_dvm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
 nostr_dvm/interfaces/__init__.py
 nostr_dvm/interfaces/dvmtaskinterface.py
 nostr_dvm/tasks/__init__.py
 nostr_dvm/tasks/advanced_search.py
 nostr_dvm/tasks/advanced_search_wine.py
 nostr_dvm/tasks/content_discovery_currently_popular.py
+nostr_dvm/tasks/content_discovery_currently_popular_followers.py
 nostr_dvm/tasks/convert_media.py
+nostr_dvm/tasks/discovery_censor_wot.py
 nostr_dvm/tasks/discovery_inactive_follows.py
 nostr_dvm/tasks/discovery_nonfollowers.py
-nostr_dvm/tasks/discovery_relevant_notes.py
 nostr_dvm/tasks/discovery_trending_notes_nostrband.py
 nostr_dvm/tasks/imagegeneration_openai_dalle.py
 nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
 nostr_dvm/tasks/imagegeneration_sd21_mlx.py
 nostr_dvm/tasks/imagegeneration_sdxl.py
 nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
 nostr_dvm/tasks/imageinterrogator.py
```

### Comparing `nostr-dvm-0.3.0/setup.py` & `nostr-dvm-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. '
                     'This is an early stage release. Interfaces might change/brick')
 
 # Setting up
 setup(
     name="nostr-dvm",
```

### Comparing `nostr-dvm-0.3.0/tests/test_dvm_client.py` & `nostr-dvm-0.3.1/tests/test_dvm_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import time
 from pathlib import Path
 from threading import Thread
 
 import dotenv
 from nostr_sdk import Keys, Client, Tag, EventBuilder, Filter, HandleNotification, Timestamp, nip04_decrypt, \
-    nip04_encrypt, NostrSigner
+    nip04_encrypt, NostrSigner, PublicKey, Event
 
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.nostr_utils import send_event, check_and_set_private_key
 from nostr_dvm.utils.definitions import EventDefinitions
 
 
 # TODO HINT: Best use this path with a previously whitelisted privkey, as zapping events is not implemented in the lib/code
@@ -36,21 +36,21 @@
 
     for relay in relay_list:
         client.add_relay(relay)
     client.connect()
     config = DVMConfig
     send_event(event, client=client, dvm_config=config)
     return event.as_json()
+
+
 def nostr_client_test_search_profile(input):
     keys = Keys.parse(check_and_set_private_key("test_client"))
 
     iTag = Tag.parse(["i", input, "text"])
 
-
-
     relaysTag = Tag.parse(['relays', "wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
                            "wss://nostr-pub.wellorder.net"])
     alttag = Tag.parse(["alt", "This is a NIP90 DVM AI task to translate a given Input"])
     event = EventBuilder(EventDefinitions.KIND_NIP90_USER_SEARCH, str("Search for user"),
                          [iTag, relaysTag, alttag]).to_event(keys)
 
     relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
@@ -62,14 +62,15 @@
     for relay in relay_list:
         client.add_relay(relay)
     client.connect()
     config = DVMConfig
     send_event(event, client=client, dvm_config=config)
     return event.as_json()
 
+
 def nostr_client_test_image(prompt):
     keys = Keys.parse(check_and_set_private_key("test_client"))
 
     iTag = Tag.parse(["i", prompt, "text"])
     outTag = Tag.parse(["output", "image/png;format=url"])
     paramTag1 = Tag.parse(["param", "size", "1024x1024"])
     tTag = Tag.parse(["t", "bitcoin"])
@@ -90,29 +91,56 @@
         client.add_relay(relay)
     client.connect()
     config = DVMConfig
     send_event(event, client=client, dvm_config=config)
     return event.as_json()
 
 
+def nostr_client_test_censor_filter(users):
+    keys = Keys.parse(check_and_set_private_key("test_client"))
+
+    relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
+                  ]
+
+    relaysTag = Tag.parse(relay_list)
+    alttag = Tag.parse(["alt", "This is a NIP90 DVM AI task to find people to ignore based on people the user trusts"])
+    # pTag = Tag.parse(["p", user, "text"])
+    tags = [relaysTag, alttag]
+    for user in users:
+        iTag = Tag.parse(["i", user, "text"])
+        tags.append(iTag)
+
+    event = EventBuilder(EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY, str("Give me bad actors"),
+                         tags).to_event(keys)
+
+    signer = NostrSigner.keys(keys)
+    client = Client(signer)
+    for relay in relay_list:
+        client.add_relay(relay)
+    client.connect()
+    config = DVMConfig
+    send_event(event, client=client, dvm_config=config)
+    return event.as_json()
+
+
 def nostr_client_test_tts(prompt):
     keys = Keys.parse(check_and_set_private_key("test_client"))
 
     iTag = Tag.parse(["i", prompt, "text"])
     paramTag1 = Tag.parse(["param", "language", "en"])
 
     bidTag = Tag.parse(['bid', str(1000 * 1000), str(1000 * 1000)])
     relaysTag = Tag.parse(['relays', "wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
                            "wss://nostr-pub.wellorder.net"])
     alttag = Tag.parse(["alt", "This is a NIP90 DVM AI task to generate TTSt"])
     event = EventBuilder(EventDefinitions.KIND_NIP90_TEXT_TO_SPEECH, str("Generate an Audio File."),
                          [iTag, paramTag1, bidTag, relaysTag, alttag]).to_event(keys)
 
     relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
-                  "wss://nostr-pub.wellorder.net"]
+                  ]
 
     signer = NostrSigner.keys(keys)
     client = Client(signer)
     for relay in relay_list:
         client.add_relay(relay)
     client.connect()
     config = DVMConfig
@@ -120,16 +148,14 @@
     return event.as_json()
 
 
 def nostr_client_test_image_private(prompt, cashutoken):
     keys = Keys.parse(check_and_set_private_key("test_client"))
     receiver_keys = Keys.parse(check_and_set_private_key("replicate_sdxl"))
 
-    # TODO more advanced logic, more parsing, params etc, just very basic test functions for now
-
     relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
                   "wss://nostr-pub.wellorder.net"]
     i_tag = Tag.parse(["i", prompt, "text"])
     outTag = Tag.parse(["output", "image/png;format=url"])
     paramTag1 = Tag.parse(["param", "size", "1024x1024"])
     pTag = Tag.parse(["p", receiver_keys.public_key().to_hex()])
 
@@ -173,39 +199,42 @@
     client.connect()
 
     dm_zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_DM,
                                                EventDefinitions.KIND_ZAP]).since(
         Timestamp.now())  # events to us specific
     dvm_filter = (Filter().kinds([EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
                                   EventDefinitions.KIND_FEEDBACK]).since(Timestamp.now()))  # public events
-    client.subscribe([dm_zap_filter, dvm_filter])
+    client.subscribe([dm_zap_filter, dvm_filter], None)
 
     # nostr_client_test_translation("This is the result of the DVM in spanish", "text", "es", 20, 20)
     # nostr_client_test_translation("note1p8cx2dz5ss5gnk7c59zjydcncx6a754c0hsyakjvnw8xwlm5hymsnc23rs", "event", "es", 20,20)
     # nostr_client_test_translation("44a0a8b395ade39d46b9d20038b3f0c8a11168e67c442e3ece95e4a1703e2beb", "event", "zh", 20, 20)
-    #nostr_client_test_image("a beautiful purple ostrich watching the sunset")
-    nostr_client_test_search_profile("dontbelievew")
+    # nostr_client_test_image("a beautiful purple ostrich watching the sunset")
+    # nostr_client_test_search_profile("dontbelieve")
+    wot = ["99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64"]
+    nostr_client_test_censor_filter(wot)
+
     # nostr_client_test_tts("Hello, this is a test. Mic check one, two.")
 
     # cashutoken = "cashuAeyJ0b2tlbiI6W3sicHJvb2ZzIjpbeyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6MSwiQyI6IjAyNWU3ODZhOGFkMmExYTg0N2YxMzNiNGRhM2VhMGIyYWRhZGFkOTRiYzA4M2E2NWJjYjFlOTgwYTE1NGIyMDA2NCIsInNlY3JldCI6InQ1WnphMTZKMGY4UElQZ2FKTEg4V3pPck5rUjhESWhGa291LzVzZFd4S0U9In0seyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6NCwiQyI6IjAyOTQxNmZmMTY2MzU5ZWY5ZDc3MDc2MGNjZmY0YzliNTMzMzVmZTA2ZGI5YjBiZDg2Njg5Y2ZiZTIzMjVhYWUwYiIsInNlY3JldCI6IlRPNHB5WE43WlZqaFRQbnBkQ1BldWhncm44UHdUdE5WRUNYWk9MTzZtQXM9In0seyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6MTYsIkMiOiIwMmRiZTA3ZjgwYmMzNzE0N2YyMDJkNTZiMGI3ZTIzZTdiNWNkYTBhNmI3Yjg3NDExZWYyOGRiZDg2NjAzNzBlMWIiLCJzZWNyZXQiOiJHYUNIdHhzeG9HM3J2WWNCc0N3V0YxbU1NVXczK0dDN1RKRnVwOHg1cURzPSJ9XSwibWludCI6Imh0dHBzOi8vbG5iaXRzLmJpdGNvaW5maXhlc3RoaXMub3JnL2Nhc2h1L2FwaS92MS9ScDlXZGdKZjlxck51a3M1eVQ2SG5rIn1dfQ=="
     # nostr_client_test_image_private("a beautiful ostrich watching the sunset")
     class NotificationHandler(HandleNotification):
-        def handle(self, relay_url, event):
+        def handle(self, relay_url, subscription_id, event: Event):
             print(f"Received new event from {relay_url}: {event.as_json()}")
-            if event.kind() == 7000:
+            if event.kind().as_u64() == 7000:
                 print("[Nostr Client]: " + event.as_json())
-            elif 6000 < event.kind() < 6999:
+            elif 6000 < event.kind().as_u64() < 6999:
                 print("[Nostr Client]: " + event.as_json())
                 print("[Nostr Client]: " + event.content())
 
-            elif event.kind() == 4:
+            elif event.kind().as_u64() == 4:
                 dec_text = nip04_decrypt(sk, event.author(), event.content())
                 print("[Nostr Client]: " + f"Received new msg: {dec_text}")
 
-            elif event.kind() == 9735:
+            elif event.kind().as_u64() == 9735:
                 print("[Nostr Client]: " + f"Received new zap:")
                 print(event.as_json())
 
         def handle_msg(self, relay_url, msg):
             return
 
     client.handle_notifications(NotificationHandler())
```

### Comparing `nostr-dvm-0.3.0/tests/test_events.py` & `nostr-dvm-0.3.1/tests/test_events.py`

 * *Files identical despite different names*

