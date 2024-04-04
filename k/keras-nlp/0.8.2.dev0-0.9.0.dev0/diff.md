# Comparing `tmp/keras-nlp-0.8.2.dev0.tar.gz` & `tmp/keras-nlp-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nlp-0.8.2.dev0.tar", last modified: Tue Feb 27 21:16:08 2024, max compression
+gzip compressed data, was "keras-nlp-0.9.0.dev0.tar", last modified: Thu Apr  4 19:59:38 2024, max compression
```

## Comparing `keras-nlp-0.8.2.dev0.tar` & `keras-nlp-0.9.0.dev0.tar`

### file list

```diff
@@ -1,267 +1,286 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.102891 keras-nlp-0.8.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-27 21:16:08.102891 keras-nlp-0.8.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.058891 keras-nlp-0.8.2.dev0/keras_nlp/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.058891 keras-nlp-0.8.2.dev0/keras_nlp/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.058891 keras-nlp-0.8.2.dev0/keras_nlp/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.058891 keras-nlp-0.8.2.dev0/keras_nlp/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.058891 keras-nlp-0.8.2.dev0/keras_nlp/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.058891 keras-nlp-0.8.2.dev0/keras_nlp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.062891 keras-nlp-0.8.2.dev0/keras_nlp/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/backend/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/backend/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/backend/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.062891 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.062891 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/alibi_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/reversible_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/rotary_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.066891 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/random_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.066891 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/rouge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/rouge_l.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/rouge_n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.066891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.070891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.070891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.070891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.074891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.074891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.078891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.078891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/electra/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/electra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/electra/electra_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/electra/electra_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.078891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.082891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)    17362 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_decoder_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/rms_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/generative_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.082891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.082891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.086891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.086891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_transformer_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.090891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.090891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.090891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.094891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_cached_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.094891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.094891 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/relative_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/xlnet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/xlnet_content_and_query_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/xlnet_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.098891 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/beam_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/contrastive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/greedy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/top_k_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/top_p_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.098891 keras-nlp-0.8.2.dev0/keras_nlp/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19031 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.098891 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25973 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11672 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19732 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.102891 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/keras_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/preset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-02-27 21:15:57.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/utils/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/src/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.102891 keras-nlp-0.8.2.dev0/keras_nlp/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-27 21:16:02.000000 keras-nlp-0.8.2.dev0/keras_nlp/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:16:08.102891 keras-nlp-0.8.2.dev0/keras_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-27 21:16:08.000000 keras-nlp-0.8.2.dev0/keras_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-02-27 21:16:08.000000 keras-nlp-0.8.2.dev0/keras_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 21:16:08.000000 keras-nlp-0.8.2.dev0/keras_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-27 21:16:08.000000 keras-nlp-0.8.2.dev0/keras_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 21:16:08.000000 keras-nlp-0.8.2.dev0/keras_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-27 21:16:08.102891 keras-nlp-0.8.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-27 21:15:56.000000 keras-nlp-0.8.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.231090 keras-nlp-0.9.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-04 19:59:38.231090 keras-nlp-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.187090 keras-nlp-0.9.0.dev0/keras_nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.187090 keras-nlp-0.9.0.dev0/keras_nlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.187090 keras-nlp-0.9.0.dev0/keras_nlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.187090 keras-nlp-0.9.0.dev0/keras_nlp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.187090 keras-nlp-0.9.0.dev0/keras_nlp/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.187090 keras-nlp-0.9.0.dev0/keras_nlp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.191090 keras-nlp-0.9.0.dev0/keras_nlp/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/backend/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/backend/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/backend/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.191090 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.191090 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/alibi_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/reversible_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/rotary_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21998 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.195090 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/random_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.195090 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/rouge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/rouge_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/rouge_n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.195090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.199090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.199090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19926 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.199090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.203091 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.203091 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.203091 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.207090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/electra_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/electra_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/electra_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/electra_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.207090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.207090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_transformer_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.211090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17399 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_decoder_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/rms_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.211090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.211090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.215090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/masked_lm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.215090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_transformer_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.219090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.219090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/seq_2_seq_lm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.219090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.223090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.223090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.223090 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/relative_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/xlnet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/xlnet_content_and_query_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/xlnet_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.227090 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/beam_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/contrastive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/greedy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/top_k_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/top_p_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.227090 keras-nlp-0.9.0.dev0/keras_nlp/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18984 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.227090 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23749 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.227090 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/keras_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/preset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/utils/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/src/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.227090 keras-nlp-0.9.0.dev0/keras_nlp/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 19:59:36.000000 keras-nlp-0.9.0.dev0/keras_nlp/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:38.227090 keras-nlp-0.9.0.dev0/keras_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-04 19:59:38.000000 keras-nlp-0.9.0.dev0/keras_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-04 19:59:38.000000 keras-nlp-0.9.0.dev0/keras_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:59:38.000000 keras-nlp-0.9.0.dev0/keras_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 19:59:38.000000 keras-nlp-0.9.0.dev0/keras_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:59:38.000000 keras-nlp-0.9.0.dev0/keras_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-04 19:59:38.231090 keras-nlp-0.9.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-04 19:59:32.000000 keras-nlp-0.9.0.dev0/setup.py
```

### Comparing `keras-nlp-0.8.2.dev0/PKG-INFO` & `keras-nlp-0.9.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.8.2.dev0
+Version: 0.9.0.dev0
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nlp-0.8.2.dev0/README.md` & `keras-nlp-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/layers/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/models/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,69 +7,93 @@
 
 from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
 from keras_nlp.src.models.albert.albert_classifier import AlbertClassifier
 from keras_nlp.src.models.albert.albert_masked_lm import AlbertMaskedLM
 from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import AlbertMaskedLMPreprocessor
 from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
 from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.bart.bart_backbone import BartBackbone
 from keras_nlp.src.models.bart.bart_preprocessor import BartPreprocessor
 from keras_nlp.src.models.bart.bart_seq_2_seq_lm import BartSeq2SeqLM
 from keras_nlp.src.models.bart.bart_seq_2_seq_lm_preprocessor import BartSeq2SeqLMPreprocessor
 from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 from keras_nlp.src.models.bert.bert_backbone import BertBackbone
 from keras_nlp.src.models.bert.bert_classifier import BertClassifier
 from keras_nlp.src.models.bert.bert_masked_lm import BertMaskedLM
 from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import BertMaskedLMPreprocessor
 from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
 from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bloom.bloom_backbone import BloomBackbone
+from keras_nlp.src.models.bloom.bloom_causal_lm import BloomCausalLM
+from keras_nlp.src.models.bloom.bloom_causal_lm_preprocessor import BloomCausalLMPreprocessor
+from keras_nlp.src.models.bloom.bloom_preprocessor import BloomPreprocessor
+from keras_nlp.src.models.bloom.bloom_tokenizer import BloomTokenizer
+from keras_nlp.src.models.causal_lm import CausalLM
+from keras_nlp.src.models.classifier import Classifier
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.src.models.deberta_v3.deberta_v3_classifier import DebertaV3Classifier
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import DebertaV3MaskedLMPreprocessor
 from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import DebertaV3Preprocessor
 from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.src.models.distil_bert.distil_bert_classifier import DistilBertClassifier
 from keras_nlp.src.models.distil_bert.distil_bert_masked_lm import DistilBertMaskedLM
 from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import DistilBertMaskedLMPreprocessor
 from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import DistilBertPreprocessor
 from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import DistilBertTokenizer
+from keras_nlp.src.models.electra.electra_backbone import ElectraBackbone
+from keras_nlp.src.models.electra.electra_preprocessor import ElectraPreprocessor
+from keras_nlp.src.models.electra.electra_tokenizer import ElectraTokenizer
 from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
 from keras_nlp.src.models.f_net.f_net_masked_lm import FNetMaskedLM
 from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import FNetMaskedLMPreprocessor
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.falcon.falcon_backbone import FalconBackbone
+from keras_nlp.src.models.falcon.falcon_causal_lm_preprocessor import FalconCausalLMPreprocessor
+from keras_nlp.src.models.falcon.falcon_preprocessor import FalconPreprocessor
+from keras_nlp.src.models.falcon.falcon_tokenizer import FalconTokenizer
 from keras_nlp.src.models.gemma.gemma_backbone import GemmaBackbone
 from keras_nlp.src.models.gemma.gemma_causal_lm import GemmaCausalLM
 from keras_nlp.src.models.gemma.gemma_causal_lm_preprocessor import GemmaCausalLMPreprocessor
 from keras_nlp.src.models.gemma.gemma_preprocessor import GemmaPreprocessor
 from keras_nlp.src.models.gemma.gemma_tokenizer import GemmaTokenizer
 from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
 from keras_nlp.src.models.gpt2.gpt2_causal_lm import GPT2CausalLM
 from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import GPT2CausalLMPreprocessor
 from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
 from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.llama.llama_backbone import LlamaBackbone
+from keras_nlp.src.models.llama.llama_causal_lm import LlamaCausalLM
+from keras_nlp.src.models.llama.llama_causal_lm_preprocessor import LlamaCausalLMPreprocessor
+from keras_nlp.src.models.llama.llama_preprocessor import LlamaPreprocessor
 from keras_nlp.src.models.llama.llama_tokenizer import LlamaTokenizer
+from keras_nlp.src.models.masked_lm import MaskedLM
 from keras_nlp.src.models.mistral.mistral_backbone import MistralBackbone
 from keras_nlp.src.models.mistral.mistral_causal_lm import MistralCausalLM
 from keras_nlp.src.models.mistral.mistral_causal_lm_preprocessor import MistralCausalLMPreprocessor
 from keras_nlp.src.models.mistral.mistral_preprocessor import MistralPreprocessor
 from keras_nlp.src.models.mistral.mistral_tokenizer import MistralTokenizer
 from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
 from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import OPTCausalLMPreprocessor
 from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
 from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
 from keras_nlp.src.models.roberta.roberta_masked_lm import RobertaMaskedLM
 from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import RobertaMaskedLMPreprocessor
 from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
 from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.seq_2_seq_lm import Seq2SeqLM
+from keras_nlp.src.models.task import Task
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_classifier import XLMRobertaClassifier
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm import XLMRobertaMaskedLM
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import XLMRobertaMaskedLMPreprocessor
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import XLMRobertaPreprocessor
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import XLMRobertaTokenizer
+from keras_nlp.src.tokenizers.tokenizer import Tokenizer
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/samplers/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,10 +22,11 @@
 
 from keras_nlp.src import layers
 from keras_nlp.src import metrics
 from keras_nlp.src import models
 from keras_nlp.src import samplers
 from keras_nlp.src import tokenizers
 from keras_nlp.src import utils
+from keras_nlp.src.utils.preset_utils import upload_preset
 from keras_nlp.src.version_utils import __version__
 from keras_nlp.src.version_utils import version
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/api_export.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/backend/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/backend/config.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/backend/keras.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/backend/keras.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/backend/ops.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/backend/ops.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/backend/random.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/backend/random.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/conftest.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+
 import pytest
 import tensorflow as tf
 
 from keras_nlp.src.backend import config as backend_config
 from keras_nlp.src.backend import keras
 
 
@@ -79,14 +81,18 @@
         "markers",
         "tf_only: mark test as a tf only test",
     )
     config.addinivalue_line(
         "markers",
         "keras_3_only: mark test as a keras 3 only test",
     )
+    config.addinivalue_line(
+        "markers",
+        "kaggle_key_required: mark test needing a kaggle key",
+    )
 
 
 def pytest_collection_modifyitems(config, items):
     run_extra_large_tests = config.getoption("--run_extra_large")
     # Run large tests for --run_extra_large or --run_large.
     run_large_tests = config.getoption("--run_large") or run_extra_large_tests
 
@@ -103,23 +109,35 @@
         not backend_config.backend() == "tensorflow",
         reason="tests only run on tf backend",
     )
     keras_3_only = pytest.mark.skipif(
         not backend_config.keras_3(),
         reason="tests only run on with multi-backend keras",
     )
+    found_kaggle_key = all(
+        [
+            os.environ.get("KAGGLE_USERNAME", None),
+            os.environ.get("KAGGLE_KEY", None),
+        ]
+    )
+    kaggle_key_required = pytest.mark.skipif(
+        not found_kaggle_key,
+        reason="tests only run with a kaggle api key",
+    )
     for item in items:
         if "large" in item.keywords:
             item.add_marker(skip_large)
         if "extra_large" in item.keywords:
             item.add_marker(skip_extra_large)
         if "tf_only" in item.keywords:
             item.add_marker(tf_only)
         if "keras_3_only" in item.keywords:
             item.add_marker(keras_3_only)
+        if "kaggle_key_required" in item.keywords:
+            item.add_marker(kaggle_key_required)
 
 
 # Disable traceback filtering for quicker debugging of tests failures.
 tf.debugging.disable_traceback_filtering()
 if backend_config.keras_3():
     keras.config.disable_traceback_filtering()
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/alibi_bias.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/alibi_bias.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,23 @@
     shape as the input.
 
     Args:
         alibi_bias_max: int. This value will be used to compute the slope of
             each head. The heads' slopes are a geometric sequence that starts at
             `2**(-alibi_bias_max/num_heads)` and uses that same value as its
             ratio. Defaults to 8.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
+
     Call arguments:
         attention_scores: The result of multipying the query and the key of the
             multi-head attention layer of the transformer to add alibi bias to
             it. With shape `(batch_size, num_heads, query_length, key_length)`.
 
-    Examples:
+    Example:
     ```python
     query_length = 10
     key_length = 10
     num_heads = 4
     batch_size = 2
     hidden_dim = 8
 
@@ -90,15 +93,17 @@
 
     def _get_alibi_bias(self, num_heads, key_length):
         slopes = ops.convert_to_tensor(
             self._get_slopes(num_heads), dtype=self.compute_dtype
         )
         slopes = ops.expand_dims(slopes, 1)
 
-        seq_range = ops.expand_dims(ops.arange(1 - key_length, 1), 0)
+        seq_range = ops.expand_dims(
+            ops.arange(1 - key_length, 1, dtype="int32"), 0
+        )
         seq_range = ops.cast(seq_range, dtype=self.compute_dtype)
 
         alibi_bias = ops.multiply(slopes, seq_range)
         alibi_bias = ops.expand_dims(alibi_bias, 1)
 
         # return shape is `(1, num_heads, 1, key_length)`
         return ops.expand_dims(alibi_bias, 0)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/cached_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/f_net_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
             normalization components. Defaults to `1e-5`.
         kernel_initializer: `str` or `keras.initializers` initializer.
             The kernel initializer for the dense layers.
             Defaults to `"glorot_uniform"`.
         bias_initializer: "string" or `keras.initializers` initializer.
             The bias initializer for the dense layers.
             Defaults to `"zeros"`.
-        name: string. The name of the layer. Defaults to `None`.
-        **kwargs: other keyword arguments.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
-    Examples:
+    Example:
 
     ```python
     # Create a single FNet encoder layer.
     encoder = keras_nlp.layers.FNetEncoder(
         intermediate_dim=64)
 
     # Create a simple model containing the encoder.
@@ -75,18 +75,17 @@
         self,
         intermediate_dim,
         dropout=0,
         activation="relu",
         layer_norm_epsilon=1e-5,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
-        name=None,
         **kwargs
     ):
-        super().__init__(name=name, **kwargs)
+        super().__init__(**kwargs)
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
         self.activation = keras.activations.get(activation)
         self.layer_norm_epsilon = layer_norm_epsilon
         self.kernel_initializer = keras.initializers.get(kernel_initializer)
         self.bias_initializer = keras.initializers.get(bias_initializer)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/masked_lm_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,18 @@
             normalization components. Defaults to `1e-5`.
         kernel_initializer: string or `keras.initializers` initializer.
             The kernel initializer for the dense and multiheaded
             attention layers. Defaults to `"glorot_uniform"`.
         bias_initializer: string or `keras.initializers` initializer.
             The bias initializer for the dense and multiheaded
             attention layers. Defaults to `"zeros"`.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
-    Examples:
+    Example:
 
     ```python
     batch_size = 16
     vocab_size = 100
     hidden_dim = 32
     seq_length = 50
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/position_embedding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/position_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,27 @@
     `keras.layers.Embedding` for padding mask support.
 
     Args:
         sequence_length: The maximum length of the dynamic sequence.
         initializer: The initializer to use for the embedding weights. Defaults
             to `"glorot_uniform"`.
         seq_axis: The axis of the input tensor where we add the embeddings.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
     Call arguments:
         inputs: The tensor inputs to compute an embedding for, with shape
             `(batch_size, sequence_length, hidden_dim)`. Only the input shape
             will be used, as the position embedding does not depend on the
             input sequence content.
         start_index: An integer or integer tensor. The starting position to
             compute the position embedding from. This is useful during cached
             decoding, where each position is predicted separately in a loop.
 
-    Examples:
+    Example:
 
     Called directly on input.
     >>> layer = keras_nlp.layers.PositionEmbedding(sequence_length=10)
     >>> layer(np.zeros((8, 10, 16)))
 
     Combine with a token embedding.
     ```python
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/reversible_embedding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/reversible_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,38 @@
         embeddings_constraint: Constraint function applied to
             the `embeddings` matrix (see `keras.constraints`).
         mask_zero: Boolean, whether or not the input value 0 is a special
             "padding" value that should be masked out.
         reverse_dtype: The dtype for the reverse projection computation.
             For stability, it is usually best to use full precision even when
             working with half or mixed precision training.
+        **kwargs: other keyword arguments passed to `keras.layers.Embedding`,
+            including `name`, `trainable`, `dtype` etc.
 
     Call arguments:
         inputs: The tensor inputs to the layer.
         reverse: Boolean. If `True` the layer will perform a linear projection
             from `output_dim` to `input_dim`, instead of a normal embedding
             call. Default to `False`.
 
-    Examples:
+    Example:
     ```python
     batch_size = 16
     vocab_size = 100
     hidden_dim = 32
     seq_length = 50
 
     # Generate random inputs.
     token_ids = np.random.randint(vocab_size, size=(batch_size, seq_length))
 
     embedding = keras_nlp.layers.ReversibleEmbedding(vocab_size, hidden_dim)
     # Embed tokens to shape `(batch_size, seq_length, hidden_dim)`.
     hidden_states = embedding(token_ids)
     # Project hidden states to shape `(batch_size, seq_length, vocab_size)`.
-    logits = embedding(hidden_state, reverse=True)
+    logits = embedding(hidden_states, reverse=True)
     ```
 
     References:
     - [Vaswani et al., 2017](https://arxiv.org/abs/1706.03762)
     - [Press and Wolf, 2016](https://arxiv.org/abs/1608.05859)
     """
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/rotary_embedding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/rotary_embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     Args:
         max_wavelength: int. The maximum angular wavelength of the sine/cosine
             curves.
         scaling_factor: float. The scaling factor used to scale frequency range.
         sequence_axis: int. Sequence axis in the input tensor.
         feature_axis: int. Feature axis in the input tensor.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
     Call arguments:
         inputs: The tensor inputs to apply the embedding to. This can have
             any shape, but must contain both a sequence and feature axis. The
             rotary embedding will be applied to `inputs` and returned.
         start_index: An integer or integer tensor. The starting position to
             compute the rotary embedding from. This is useful during cached
@@ -81,57 +83,68 @@
         self.max_wavelength = max_wavelength
         self.sequence_axis = sequence_axis
         self.feature_axis = feature_axis
         self.scaling_factor = scaling_factor
         self.built = True
 
     def call(self, inputs, start_index=0):
+        inputs = ops.moveaxis(
+            inputs, (self.feature_axis, self.sequence_axis), (-1, 1)
+        )
         cos_emb, sin_emb = self._compute_cos_sin_embedding(inputs, start_index)
-        return self._apply_rotary_pos_emb(inputs, cos_emb, sin_emb)
+        output = self._apply_rotary_pos_emb(inputs, cos_emb, sin_emb)
+        return ops.moveaxis(
+            output, (-1, 1), (self.feature_axis, self.sequence_axis)
+        )
 
     def _apply_rotary_pos_emb(self, tensor, cos_emb, sin_emb):
-        x1, x2 = ops.split(tensor, 2, axis=self.feature_axis)
-        half_rot_tensor = ops.concatenate((-x2, x1), axis=self.feature_axis)
+        x1, x2 = ops.split(tensor, 2, axis=-1)
+        # Avoid `ops.concatenate` for now, to avoid a obscure bug with XLA
+        # compilation on jax. We should be able to remove this once the
+        # following PR is in all jax releases we care about:
+        # https://github.com/openxla/xla/pull/7875
+        half_rot_tensor = ops.stack((-x2, x1), axis=-2)
+        half_rot_tensor = ops.reshape(half_rot_tensor, ops.shape(tensor))
         return (tensor * cos_emb) + (half_rot_tensor * sin_emb)
 
     def _compute_cos_sin_embedding(self, inputs, start_index=0):
-        def get_axis(axis):
-            return axis if axis > 0 else len(inputs.shape) + axis
+        start_index = ops.cast(start_index, dtype="float32")
 
-        feature_axis = get_axis(self.feature_axis)
-        sequence_axis = get_axis(self.sequence_axis)
+        feature_axis = len(inputs.shape) - 1
+        sequence_axis = 1
 
         rotary_dim = ops.shape(inputs)[feature_axis]
         inverse_freq = self._get_inverse_freq(rotary_dim)
 
-        seq_len = ops.shape(inputs)[self.sequence_axis]
-        tensor = ops.cast(ops.arange(seq_len), self.compute_dtype) + start_index
+        seq_len = ops.shape(inputs)[sequence_axis]
+        tensor = ops.arange(seq_len, dtype="float32") + start_index
 
-        tensor = ops.cast(tensor, dtype=inverse_freq.dtype)
         freq = ops.einsum("i,j->ij", tensor, inverse_freq)
-        embedding = ops.concatenate((freq, freq), axis=-1)
+        embedding = ops.stack((freq, freq), axis=-2)
+        embedding = ops.reshape(
+            embedding, (*ops.shape(freq)[:-1], ops.shape(freq)[-1] * 2)
+        )
 
         # Reshape the embedding to be broadcastable with input shape.
         if feature_axis < sequence_axis:
             embedding = ops.transpose(embedding)
         for axis in range(len(inputs.shape)):
             if axis != sequence_axis and axis != feature_axis:
                 embedding = ops.expand_dims(embedding, axis)
 
-        return ops.cos(embedding), ops.sin(embedding)
+        cos_emb = ops.cast(ops.cos(embedding), self.compute_dtype)
+        sin_emb = ops.cast(ops.sin(embedding), self.compute_dtype)
+        return cos_emb, sin_emb
 
     def _get_inverse_freq(self, rotary_dim):
-        freq_range = ops.arange(0, rotary_dim, 2)
-        freq_range = ops.cast(freq_range, self.compute_dtype)
-        freq_range = freq_range / ops.cast(
-            self.scaling_factor, self.compute_dtype
-        )
+        freq_range = ops.arange(0, rotary_dim, 2, dtype="float32")
+        freq_range = freq_range / ops.cast(self.scaling_factor, "float32")
         inverse_freq = 1.0 / (
             self.max_wavelength
-            ** (freq_range / ops.cast(rotary_dim, self.compute_dtype))
+            ** (freq_range / ops.cast(rotary_dim, "float32"))
         )
         return inverse_freq
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/sine_position_encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,25 @@
     positional encoding the same size as the embedded token tensor, which
     can be added directly to the embedded token tensor.
 
     Args:
         max_wavelength: The maximum angular wavelength of the sine/cosine
             curves, as described in Attention is All You Need. Defaults to
             `10000`.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
     Call arguments:
         inputs: The tensor inputs to compute an embedding for, with shape
             `(batch_size, sequence_length, hidden_dim)`.
         start_index: An integer or integer tensor. The starting position to
             compute the encoding from. This is useful during cached decoding,
             where each position is predicted separately in a loop.
 
-    Examples:
+    Example:
     ```python
     # create a simple embedding layer with sinusoidal positional encoding
     seq_len = 100
     vocab_size = 1000
     embedding_dim = 32
     inputs = keras.Input((seq_len,), dtype="float32")
     embedding = keras.layers.Embedding(
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/token_and_position_embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,26 +29,31 @@
     output when called. This layer assumes that the last dimension in the input
     corresponds to the sequence dimension.
 
     Args:
         vocabulary_size: The size of the vocabulary.
         sequence_length: The maximum length of input sequence
         embedding_dim: The output dimension of the embedding layer
+        tie_weights: Boolean, whether or not the matrix for embedding and
+            the matrix for the `reverse` projection should share the same
+            weights.
         embeddings_initializer: The initializer to use for the Embedding
             Layers
         mask_zero: Boolean, whether or not the input value 0 is a special
             "padding" value that should be masked out.
             This is useful when using recurrent layers which may take variable
             length input. If this is True, then all subsequent layers in the
             model need to support masking or an exception will be raised.
             If mask_zero` is set to True, as a consequence, index 0 cannot be
             used in the vocabulary
             (input_dim should equal size of vocabulary + 1).
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
-    Examples:
+    Example:
     ```python
     inputs = np.ones(shape=(1, 50), dtype="int32")
     embedding_layer = keras_nlp.layers.TokenAndPositionEmbedding(
         vocabulary_size=10_000,
         sequence_length=50,
         embedding_dim=128,
     )
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/transformer_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,17 @@
 class TransformerDecoder(keras.layers.Layer):
     """Transformer decoder.
 
     This class follows the architecture of the transformer decoder layer in the
     paper [Attention is All You Need](https://arxiv.org/abs/1706.03762). Users
     can instantiate multiple instances of this class to stack up a decoder.
 
-    By default, this layer will apply a causal mask to the decoder attention layer.
-    This layer will correctly compute an attention mask from an implicit
-    Keras padding mask (for example, by passing `mask_zero=True` to a
-    `keras.layers.Embedding` layer). See the Masking and Padding
-    [guide](https://keras.io/guides/understanding_masking_and_padding/)
-    for more details.
+    By default, this layer will apply a causal mask to the decoder attention
+    layer. You can also pass padding or attention masks directly to the layer
+    during call, e.g. with `decoder_padding_mask` or `decoder_attention_mask`.
 
     This layer can be called with either one or two inputs. The number of inputs
     must be consistent across all calls. The options are as follows:
         `layer(decoder_sequence)`: no cross-attention will be built into the
             decoder block. This is useful when building a "decoder-only"
             transformer such as GPT-2.
         `layer(decoder_sequence, encoder_sequence)`: cross-attention will be
@@ -68,18 +65,18 @@
             The bias initializer for the dense and multiheaded
             attention layers. Defaults to `"zeros"`.
         normalize_first: bool. If True, the inputs to the
             attention layer(s) and the intermediate dense layer are normalized
             (similar to GPT-2). If set to False, outputs of attention layer and
             intermediate dense layer are normalized (similar to BERT).
             Defaults to `False`.
-        name: string. The name of the layer. Defaults to `None`.
-        **kwargs: other keyword arguments.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
-    Examples:
+    Example:
     ```python
     # Create a single transformer decoder layer.
     decoder = keras_nlp.layers.TransformerDecoder(
         intermediate_dim=64, num_heads=8)
 
     # Create a simple model containing the decoder.
     decoder_input = keras.Input(shape=(10, 64))
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/transformer_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
             The bias initializer for the dense and multiheaded
             attention layers. Defaults to `"zeros"`.
         normalize_first: bool. If True, the inputs to the
             attention layer and the intermediate dense layer  are normalized
             (similar to GPT-2). If set to False, outputs of attention layer and
             intermediate dense layer are normalized (similar to BERT).
             Defaults to `False`.
-        name: string. The name of the layer. Defaults to `None`.
-        **kwargs: other keyword arguments.
+        **kwargs: other keyword arguments passed to `keras.layers.Layer`,
+            including `name`, `trainable`, `dtype` etc.
 
-    Examples:
+    Example:
 
     ```python
     # Create a single transformer encoder layer.
     encoder = keras_nlp.layers.TransformerEncoder(
         intermediate_dim=64, num_heads=8)
 
     # Create a simple model containing the encoder.
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/modeling/transformer_layer_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/masked_lm_mask_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/multi_segment_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/preprocessing_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/random_deletion.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/random_swap.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/random_swap.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/layers/preprocessing/start_end_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/bleu.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/edit_distance.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/edit_distance.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/perplexity.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/perplexity.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/rouge_base.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/rouge_base.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/rouge_l.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/rouge_l.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/metrics/rouge_n.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/metrics/rouge_n.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from keras_nlp.src.models.albert.albert_classifier import AlbertClassifier
 from keras_nlp.src.models.albert.albert_masked_lm import AlbertMaskedLM
 from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
 from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
 from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.bart.bart_backbone import BartBackbone
 from keras_nlp.src.models.bart.bart_preprocessor import BartPreprocessor
 from keras_nlp.src.models.bart.bart_seq_2_seq_lm import BartSeq2SeqLM
 from keras_nlp.src.models.bart.bart_seq_2_seq_lm_preprocessor import (
     BartSeq2SeqLMPreprocessor,
 )
 from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
@@ -32,15 +33,22 @@
 from keras_nlp.src.models.bert.bert_masked_lm import BertMaskedLM
 from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
     BertMaskedLMPreprocessor,
 )
 from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
 from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.src.models.bloom.bloom_backbone import BloomBackbone
+from keras_nlp.src.models.bloom.bloom_causal_lm import BloomCausalLM
+from keras_nlp.src.models.bloom.bloom_causal_lm_preprocessor import (
+    BloomCausalLMPreprocessor,
+)
+from keras_nlp.src.models.bloom.bloom_preprocessor import BloomPreprocessor
 from keras_nlp.src.models.bloom.bloom_tokenizer import BloomTokenizer
+from keras_nlp.src.models.causal_lm import CausalLM
+from keras_nlp.src.models.classifier import Classifier
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.src.models.deberta_v3.deberta_v3_classifier import (
     DebertaV3Classifier,
 )
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
@@ -62,23 +70,26 @@
 from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
 from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 from keras_nlp.src.models.electra.electra_backbone import ElectraBackbone
+from keras_nlp.src.models.electra.electra_preprocessor import ElectraPreprocessor
 from keras_nlp.src.models.electra.electra_tokenizer import ElectraTokenizer
 from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
 from keras_nlp.src.models.f_net.f_net_masked_lm import FNetMaskedLM
 from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
     FNetMaskedLMPreprocessor,
 )
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.falcon.falcon_backbone import FalconBackbone
+from keras_nlp.src.models.falcon.falcon_tokenizer import FalconTokenizer
 from keras_nlp.src.models.gemma.gemma_backbone import GemmaBackbone
 from keras_nlp.src.models.gemma.gemma_causal_lm import GemmaCausalLM
 from keras_nlp.src.models.gemma.gemma_causal_lm_preprocessor import (
     GemmaCausalLMPreprocessor,
 )
 from keras_nlp.src.models.gemma.gemma_preprocessor import GemmaPreprocessor
 from keras_nlp.src.models.gemma.gemma_tokenizer import GemmaTokenizer
@@ -95,38 +106,48 @@
     GPTNeoXCausalLMPreprocessor,
 )
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_preprocessor import (
     GPTNeoXPreprocessor,
 )
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
 from keras_nlp.src.models.llama.llama_backbone import LlamaBackbone
+from keras_nlp.src.models.llama.llama_causal_lm import LlamaCausalLM
+from keras_nlp.src.models.llama.llama_causal_lm_preprocessor import (
+    LlamaCausalLMPreprocessor,
+)
+from keras_nlp.src.models.llama.llama_preprocessor import LlamaPreprocessor
+from keras_nlp.src.models.llama.llama_tokenizer import LlamaTokenizer
+from keras_nlp.src.models.masked_lm import MaskedLM
 from keras_nlp.src.models.mistral.mistral_backbone import MistralBackbone
 from keras_nlp.src.models.mistral.mistral_causal_lm import MistralCausalLM
 from keras_nlp.src.models.mistral.mistral_causal_lm_preprocessor import (
     MistralCausalLMPreprocessor,
 )
 from keras_nlp.src.models.mistral.mistral_preprocessor import MistralPreprocessor
 from keras_nlp.src.models.mistral.mistral_tokenizer import MistralTokenizer
 from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
 from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
     OPTCausalLMPreprocessor,
 )
 from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
 from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
 from keras_nlp.src.models.roberta.roberta_masked_lm import RobertaMaskedLM
 from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
 from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
 from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.seq_2_seq_lm import Seq2SeqLM
 from keras_nlp.src.models.t5.t5_backbone import T5Backbone
 from keras_nlp.src.models.t5.t5_tokenizer import T5Tokenizer
+from keras_nlp.src.models.task import Task
 from keras_nlp.src.models.whisper.whisper_audio_feature_extractor import (
     WhisperAudioFeatureExtractor,
 )
 from keras_nlp.src.models.whisper.whisper_backbone import WhisperBackbone
 from keras_nlp.src.models.whisper.whisper_preprocessor import WhisperPreprocessor
 from keras_nlp.src.models.whisper.whisper_tokenizer import WhisperTokenizer
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
@@ -142,8 +163,9 @@
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
 from keras_nlp.src.models.xlnet.xlnet_backbone import XLNetBackbone
+from keras_nlp.src.tokenizers.tokenizer import Tokenizer
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
-from keras_nlp.src.models.albert.albert_presets import backbone_presets
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.utils.keras_utils import gelu_approximate
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def albert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.AlbertBackbone")
@@ -73,15 +69,15 @@
         num_segments: int. The number of types that the 'segment_ids' input can
             take.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
             for model computations and weights. Note that some computations,
             such as softmax and layer normalization, will always be done at
             float32 precision regardless of dtype.
 
-    Examples:
+    Example:
     ```python
     input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
         "segment_ids": np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]]),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
     }
 
@@ -226,14 +222,15 @@
                 "segment_ids": segment_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs={
                 "sequence_output": sequence_output,
                 "pooled_output": pooled_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
@@ -262,11 +259,7 @@
                 "dropout": self.dropout,
                 "max_sequence_length": self.max_sequence_length,
                 "num_segments": self.num_segments,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_classifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.src.models.albert.albert_backbone import albert_kernel_initializer
-from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.src.models.albert.albert_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
-
-
-@keras_nlp_export("keras_nlp.models.AlbertClassifier")
-class AlbertClassifier(Task):
-    """An end-to-end ALBERT model for classification tasks
-
-    This model attaches a classification head to a `keras_nlp.model.AlbertBackbone`
-    backbone, mapping from the backbone outputs to logit output suitable for
-    a classification task. For usage of this model with pre-trained weights, see
-    the `from_preset()` method.
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_backbone import bert_kernel_initializer
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.classifier import Classifier
+
+
+@keras_nlp_export("keras_nlp.models.BertClassifier")
+class BertClassifier(Classifier):
+    """An end-to-end BERT model for classification tasks.
+
+    This model attaches a classification head to a
+    `keras_nlp.model.BertBackbone` instance, mapping from the backbone outputs
+    to logits suitable for a classification task. For usage of this model with
+    pre-trained weights, use the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind.
 
     Args:
-        backbone: A `keras_nlp.models.AlertBackbone` instance.
+        backbone: A `keras_nlp.models.BertBackbone` instance.
         num_classes: int. Number of classes to predict.
-        preprocessor: A `keras_nlp.models.AlbertPreprocessor` or `None`. If
+        preprocessor: A `keras_nlp.models.BertPreprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
         activation: Optional `str` or callable. The
             activation function to use on the model outputs. Set
             `activation="softmax"` to return output probabilities.
             Defaults to `None`.
         dropout: float. The dropout probability value, applied after the dense
             layer.
 
     Examples:
 
-     Raw string data.
+    Raw string data.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     labels = [0, 3]
 
     # Pretrained classifier.
-    classifier = keras_nlp.models.AlbertClassifier.from_preset(
-        "albert_base_en_uncased",
+    classifier = keras_nlp.models.BertClassifier.from_preset(
+        "bert_base_en_uncased",
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     classifier.predict(x=features, batch_size=2)
 
     # Re-compile (e.g., with a new learning rate).
     classifier.compile(
@@ -87,93 +83,80 @@
         "token_ids": np.ones(shape=(2, 12), dtype="int32"),
         "segment_ids": np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2),
     }
     labels = [0, 3]
 
     # Pretrained classifier without preprocessing.
-    classifier = keras_nlp.models.AlbertClassifier.from_preset(
-        "albert_base_en_uncased",
+    classifier = keras_nlp.models.BertClassifier.from_preset(
+        "bert_base_en_uncased",
         num_classes=4,
         preprocessor=None,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
     Custom backbone and vocabulary.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     labels = [0, 3]
 
-    bytes_io = io.BytesIO()
-    ds = tf.data.Dataset.from_tensor_slices(features)
-    sentencepiece.SentencePieceTrainer.train(
-        sentence_iterator=ds.as_numpy_iterator(),
-        model_writer=bytes_io,
-        vocab_size=10,
-        model_type="WORD",
-        pad_id=0,
-        unk_id=1,
-        bos_id=2,
-        eos_id=3,
-        pad_piece="<pad>",
-        unk_piece="<unk>",
-        bos_piece="[CLS]",
-        eos_piece="[SEP]",
-        user_defined_symbols="[MASK]",
+    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
+    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
+    tokenizer = keras_nlp.models.BertTokenizer(
+        vocabulary=vocab,
     )
-    tokenizer = keras_nlp.models.AlbertTokenizer(
-        proto=bytes_io.getvalue(),
-    )
-    preprocessor = keras_nlp.models.AlbertPreprocessor(
+    preprocessor = keras_nlp.models.BertPreprocessor(
         tokenizer=tokenizer,
         sequence_length=128,
     )
-    backbone = keras_nlp.models.AlbertBackbone(
-        vocabulary_size=tokenizer.vocabulary_size(),
+    backbone = keras_nlp.models.BertBackbone(
+        vocabulary_size=30552,
         num_layers=4,
         num_heads=4,
         hidden_dim=256,
-        embedding_dim=128,
         intermediate_dim=512,
         max_sequence_length=128,
     )
-    classifier = keras_nlp.models.AlbertClassifier(
+    classifier = keras_nlp.models.BertClassifier(
         backbone=backbone,
         preprocessor=preprocessor,
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = BertBackbone
+    preprocessor_cls = BertPreprocessor
+
     def __init__(
         self,
         backbone,
         num_classes,
         preprocessor=None,
         activation=None,
         dropout=0.1,
         **kwargs,
     ):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
+        self.output_dropout = keras.layers.Dropout(
+            dropout,
+            dtype=backbone.dtype_policy,
+            name="classifier_dropout",
+        )
         self.output_dense = keras.layers.Dense(
             num_classes,
-            kernel_initializer=albert_kernel_initializer(),
+            kernel_initializer=bert_kernel_initializer(),
             activation=activation,
             dtype=backbone.dtype_policy,
             name="logits",
         )
-        self.output_dropout = keras.layers.Dropout(
-            dropout,
-            dtype=backbone.dtype_policy,
-            name="output_dropout",
-        )
 
         # === Functional Model ===
         inputs = backbone.input
         pooled = backbone(inputs)["pooled_output"]
         pooled = self.output_dropout(pooled)
         outputs = self.output_dense(pooled)
         super().__init__(
@@ -183,42 +166,18 @@
         )
 
         # === Config ===
         self.num_classes = num_classes
         self.activation = keras.activations.get(activation)
         self.dropout = dropout
 
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "activation": keras.activations.serialize(self.activation),
                 "dropout": self.dropout,
             }
         )
-
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return AlbertBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return AlbertPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy({**backbone_presets})
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_masked_lm.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,32 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
 from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
 from keras_nlp.src.models.albert.albert_backbone import albert_kernel_initializer
 from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.albert.albert_presets import backbone_presets
-from keras_nlp.src.models.task import Task
+from keras_nlp.src.models.masked_lm import MaskedLM
 from keras_nlp.src.utils.keras_utils import gelu_approximate
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertMaskedLM")
-class AlbertMaskedLM(Task):
+class AlbertMaskedLM(MaskedLM):
     """An end-to-end ALBERT model for the masked language modeling task.
 
     This model will train ALBERT on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` method.
 
@@ -48,15 +44,15 @@
 
     Args:
         backbone: A `keras_nlp.models.AlbertBackbone` instance.
         preprocessor: A `keras_nlp.models.AlbertMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
-    Example usage:
+    Examples:
 
     Raw string data.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
     # Pretrained language model.
     masked_lm = keras_nlp.models.AlbertMaskedLM.from_preset(
@@ -92,14 +88,17 @@
         "albert_base_en_uncased",
         preprocessor=None,
     )
     masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = AlbertBackbone
+    preprocessor_cls = AlbertMaskedLMPreprocessor
+
     def __init__(self, backbone, preprocessor=None, **kwargs):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.masked_lm_head = MaskedLMHead(
             vocabulary_size=backbone.vocabulary_size,
             token_embedding=backbone.token_embedding,
@@ -122,27 +121,7 @@
         )
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return AlbertBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return AlbertMaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
-from keras_nlp.src.models.albert.albert_presets import backbone_presets
 from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertPreprocessor")
 class AlbertPreprocessor(Preprocessor):
     """An ALBERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -145,14 +141,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = AlbertTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -202,15 +200,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return AlbertTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/albert/albert_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.albert.albert_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertTokenizer")
 class AlbertTokenizer(SentencePieceTokenizer):
     """ALBERT tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -116,11 +112,7 @@
             self.mask_token_id = self.token_to_id(self.mask_token)
         else:
             self.cls_token_id = None
             self.sep_token_id = None
             self.pad_token_id = None
             self.mask_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_backbone.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.layers.modeling.transformer_decoder import TransformerDecoder
 from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.bart.bart_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def bart_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.BartBackbone")
@@ -228,14 +224,15 @@
                 "decoder_token_ids": decoder_token_id_input,
                 "decoder_padding_mask": decoder_padding_mask_input,
             },
             outputs={
                 "encoder_sequence_output": encoder_output,
                 "decoder_sequence_output": decoder_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
@@ -256,11 +253,7 @@
                 "dropout": self.dropout,
                 "max_sequence_length": self.max_sequence_length,
             }
         )
 
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
-from keras_nlp.src.models.bart.bart_presets import backbone_presets
 from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.BartPreprocessor")
 class BartPreprocessor(Preprocessor):
     """A BART preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -127,14 +124,16 @@
         )
     }
     ds = tf.data.Dataset.from_tensor_slices(features)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
+    tokenizer_cls = BartTokenizer
+
     def __init__(
         self,
         tokenizer,
         encoder_sequence_length=1024,
         decoder_sequence_length=1024,
         **kwargs,
     ):
@@ -271,15 +270,7 @@
         """Alias for `decoder_sequence_length`."""
         return self.decoder_sequence_length
 
     @sequence_length.setter
     def sequence_length(self, value):
         self.decoder_sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return BartTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.bart.bart_backbone import BartBackbone
-from keras_nlp.src.models.bart.bart_presets import backbone_presets
 from keras_nlp.src.models.bart.bart_seq_2_seq_lm_preprocessor import (
     BartSeq2SeqLMPreprocessor,
 )
-from keras_nlp.src.models.generative_task import GenerativeTask
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.seq_2_seq_lm import Seq2SeqLM
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
 @keras_nlp_export("keras_nlp.models.BartSeq2SeqLM")
-class BartSeq2SeqLM(GenerativeTask):
+class BartSeq2SeqLM(Seq2SeqLM):
     """An end-to-end BART model for seq2seq language modeling.
 
     A seq2seq language model (LM) is an encoder-decoder model which is used for
     conditional text generation. The encoder is given a "context" text (fed to
     the encoder), and the decoder predicts the next token based on both the
     encoder inputs and the previous tokens. You can finetune `BartSeq2SeqLM` to
     generate text for any seq2seq task (e.g., translation or summarization).
@@ -175,14 +172,17 @@
         backbone=backbone,
         preprocessor=preprocessor,
     )
     bart_lm.fit(x=features, batch_size=2)
     ```
     """
 
+    backbone_cls = BartBackbone
+    preprocessor_cls = BartSeq2SeqLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -195,34 +195,14 @@
         outputs = backbone.token_embedding(hidden_states, reverse=True)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def backbone_cls(cls):
-        return BartBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return BartSeq2SeqLMPreprocessor
-
     def call_decoder_with_cache(
         self,
         encoder_hidden_states,
         encoder_padding_mask,
         decoder_token_ids,
         self_attention_cache=None,
         self_attention_cache_update_index=None,
@@ -394,30 +374,30 @@
             self_attention_cache,
             cross_attention_cache,
         )
 
     def generate_step(
         self,
         inputs,
-        end_token_id=None,
+        stop_token_ids=None,
     ):
         """A compilable generation function for a batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
         for a single batch of inputs. Inputs should have the same structure as
         model inputs, a dictionary with keys `"encoder_token_ids"`,
         `"encoder_padding_mask"`, `"decoder_token_ids"` and
         `"decoder_padding_mask"`.
 
         Args:
             inputs: A dictionary with four keys - `"encoder_token_ids"`,
                 `"encoder_padding_mask"`, `"decoder_token_ids"` and
                 `"decoder_padding_mask"`, with batched tensor values.
-            end_token_id: The id of the end token to stop on. If all
-                sequences have produced a new `end_token_id`, generation
+            stop_token_ids: Tuple of id's of end token's to stop on. If all
+                sequences have produced a new stop token, generation
                 will stop.
         """
         (
             encoder_token_ids,
             encoder_padding_mask,
             decoder_token_ids,
             decoder_padding_mask,
@@ -467,31 +447,32 @@
             )
             return (
                 ops.squeeze(logits, axis=1),
                 ops.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        decoder_token_ids = self._sampler(
+        decoder_token_ids = self.sampler(
             next=next,
             prompt=decoder_token_ids,
             cache=self_attention_cache,
             index=index,
             mask=decoder_padding_mask,
-            end_token_id=end_token_id,
+            stop_token_ids=stop_token_ids,
             hidden_states=hidden_states,
             model=self,
         )
 
         # Compute an output padding mask with the token ids we updated.
-        if end_token_id is not None:
-            # Build a mask of `end_token_id` locations not in the original
+        if stop_token_ids is not None:
+            # Build a mask of `stop_token_ids` locations not in the original
             # prompt (not in locations where `decoder_padding_mask` is True).
-            end_locations = ops.logical_and(
-                ops.equal(decoder_token_ids, end_token_id),
+            end_locations = any_equal(
+                decoder_token_ids,
+                stop_token_ids,
                 ops.logical_not(decoder_padding_mask),
             )
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after `end_locations`.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 import tensorflow as tf
 from absl import logging
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.bart.bart_preprocessor import BartPreprocessor
-from keras_nlp.src.models.bart.bart_presets import backbone_presets
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.BartSeq2SeqLMPreprocessor")
 class BartSeq2SeqLMPreprocessor(BartPreprocessor):
     """BART Seq2Seq LM preprocessor.
 
     This layer is used as preprocessor for seq2seq tasks using the BART model.
@@ -263,11 +260,7 @@
             & (decoder_token_ids != self.tokenizer.start_token_id)
         )
         decoder_token_ids = tf.ragged.boolean_mask(
             decoder_token_ids, decoder_padding_mask
         )
         return self.tokenizer.detokenize(decoder_token_ids)
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bart/bart_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bart/bart_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.bart.bart_presets import backbone_presets
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.BartTokenizer")
 class BartTokenizer(BytePairTokenizer):
     """A BART tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -114,18 +111,14 @@
             self.pad_token_id = self.token_to_id(self.pad_token)
             self.end_token_id = self.token_to_id(self.end_token)
         else:
             self.start_token_id = None
             self.pad_token_id = None
             self.end_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_backbone.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.bert.bert_presets import backbone_presets
 from keras_nlp.src.utils.keras_utils import gelu_approximate
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def bert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.BertBackbone")
@@ -192,14 +188,15 @@
                 "segment_ids": segment_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs={
                 "sequence_output": sequence_output,
                 "pooled_output": pooled_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
@@ -222,11 +219,7 @@
                 "dropout": self.dropout,
                 "max_sequence_length": self.max_sequence_length,
                 "num_segments": self.num_segments,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,67 +8,67 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.bert.bert_backbone import BertBackbone
-from keras_nlp.src.models.bert.bert_backbone import bert_kernel_initializer
-from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.src.models.bert.bert_presets import backbone_presets
-from keras_nlp.src.models.bert.bert_presets import classifier_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.classifier import Classifier
+from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
+    XLMRobertaPreprocessor,
+)
 
 
-@keras_nlp_export("keras_nlp.models.BertClassifier")
-class BertClassifier(Task):
-    """An end-to-end BERT model for classification tasks.
+@keras_nlp_export("keras_nlp.models.XLMRobertaClassifier")
+class XLMRobertaClassifier(Classifier):
+    """An end-to-end XLM-RoBERTa model for classification tasks.
 
     This model attaches a classification head to a
-    `keras_nlp.model.BertBackbone` instance, mapping from the backbone outputs
-    to logits suitable for a classification task. For usage of this model with
-    pre-trained weights, use the `from_preset()` constructor.
+    `keras_nlp.model.XLMRobertaBackbone` instance, mapping from the backbone
+    outputs to logits suitable for a classification task. For usage of
+    this model with pre-trained weights, see the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind.
+    warranties or conditions of any kind. The underlying model is provided by a
+    third party and subject to a separate license, available
+    [here](https://github.com/facebookresearch/fairseq).
 
     Args:
-        backbone: A `keras_nlp.models.BertBackbone` instance.
+        backbone: A `keras_nlp.models.XLMRobertaBackbone` instance.
         num_classes: int. Number of classes to predict.
-        preprocessor: A `keras_nlp.models.BertPreprocessor` or `None`. If
+        preprocessor: A `keras_nlp.models.XLMRobertaPreprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
-        activation: Optional `str` or callable. The
-            activation function to use on the model outputs. Set
-            `activation="softmax"` to return output probabilities.
-            Defaults to `None`.
-        dropout: float. The dropout probability value, applied after the dense
-            layer.
+        activation: Optional `str` or callable. The activation function to use
+            on the model outputs. Set `activation="softmax"` to return output
+            probabilities. Defaults to `None`.
+        hidden_dim: int. The size of the pooler layer.
+        dropout: float. The dropout probability value, applied to the pooled
+            output, and after the first dense layer.
 
     Examples:
 
     Raw string data.
     ```python
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    features = ["The quick brown fox jumped.", "نسيت الواجب"]
     labels = [0, 3]
 
     # Pretrained classifier.
-    classifier = keras_nlp.models.BertClassifier.from_preset(
-        "bert_base_en_uncased",
+    classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
+        "xlm_roberta_base_multi",
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     classifier.predict(x=features, batch_size=2)
 
     # Re-compile (e.g., with a new learning rate).
     classifier.compile(
@@ -82,127 +82,140 @@
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
     Preprocessed integer data.
     ```python
     features = {
         "token_ids": np.ones(shape=(2, 12), dtype="int32"),
-        "segment_ids": np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2),
     }
     labels = [0, 3]
 
     # Pretrained classifier without preprocessing.
-    classifier = keras_nlp.models.BertClassifier.from_preset(
-        "bert_base_en_uncased",
+    classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
+        "xlm_roberta_base_multi",
         num_classes=4,
         preprocessor=None,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
     Custom backbone and vocabulary.
     ```python
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    features = ["The quick brown fox jumped.", "نسيت الواجب"]
     labels = [0, 3]
 
-    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
-    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
-    tokenizer = keras_nlp.models.BertTokenizer(
-        vocabulary=vocab,
+    def train_sentencepiece(ds, vocab_size):
+        bytes_io = io.BytesIO()
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=ds.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=vocab_size,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        return bytes_io.getvalue()
+    ds = tf.data.Dataset.from_tensor_slices(
+        ["the quick brown fox", "the earth is round"]
+    )
+    proto = train_sentencepiece(ds, vocab_size=10)
+    tokenizer = keras_nlp.models.XLMRobertaTokenizer(
+        proto=proto
     )
-    preprocessor = keras_nlp.models.BertPreprocessor(
-        tokenizer=tokenizer,
+    preprocessor = keras_nlp.models.XLMRobertaPreprocessor(
+        tokenizer,
         sequence_length=128,
     )
-    backbone = keras_nlp.models.BertBackbone(
-        vocabulary_size=30552,
+    backbone = keras_nlp.models.XLMRobertaBackbone(
+        vocabulary_size=250002,
         num_layers=4,
         num_heads=4,
         hidden_dim=256,
         intermediate_dim=512,
         max_sequence_length=128,
     )
-    classifier = keras_nlp.models.BertClassifier(
+    classifier = keras_nlp.models.XLMRobertaClassifier(
         backbone=backbone,
         preprocessor=preprocessor,
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = XLMRobertaBackbone
+    preprocessor_cls = XLMRobertaPreprocessor
+
     def __init__(
         self,
         backbone,
         num_classes,
         preprocessor=None,
         activation=None,
-        dropout=0.1,
+        hidden_dim=None,
+        dropout=0.0,
         **kwargs,
     ):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
+        self.pooled_dropout = keras.layers.Dropout(
+            dropout,
+            dtype=backbone.dtype_policy,
+            name="pooled_dropout",
+        )
+        hidden_dim = hidden_dim or backbone.hidden_dim
+        self.pooled_dense = keras.layers.Dense(
+            hidden_dim,
+            activation="tanh",
+            dtype=backbone.dtype_policy,
+            name="pooled_dense",
+        )
         self.output_dropout = keras.layers.Dropout(
             dropout,
             dtype=backbone.dtype_policy,
-            name="classifier_dropout",
+            name="output_dropout",
         )
         self.output_dense = keras.layers.Dense(
             num_classes,
-            kernel_initializer=bert_kernel_initializer(),
+            kernel_initializer=roberta_kernel_initializer(),
             activation=activation,
             dtype=backbone.dtype_policy,
             name="logits",
         )
 
         # === Functional Model ===
         inputs = backbone.input
-        pooled = backbone(inputs)["pooled_output"]
-        pooled = self.output_dropout(pooled)
-        outputs = self.output_dense(pooled)
+        x = backbone(inputs)[:, backbone.start_token_index, :]
+        x = self.pooled_dropout(x)
+        x = self.pooled_dense(x)
+        x = self.output_dropout(x)
+        outputs = self.output_dense(x)
+        # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
         # === Config ===
+        self.backbone = backbone
+        self.preprocessor = preprocessor
         self.num_classes = num_classes
         self.activation = keras.activations.get(activation)
+        self.hidden_dim = hidden_dim
         self.dropout = dropout
 
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "activation": keras.activations.serialize(self.activation),
+                "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return BertBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return BertPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy({**backbone_presets, **classifier_presets})
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_masked_lm.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
 from keras_nlp.src.models.bert.bert_backbone import BertBackbone
 from keras_nlp.src.models.bert.bert_backbone import bert_kernel_initializer
 from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
     BertMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.bert.bert_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.masked_lm import MaskedLM
 
 
 @keras_nlp_export("keras_nlp.models.BertMaskedLM")
-class BertMaskedLM(Task):
+class BertMaskedLM(MaskedLM):
     """An end-to-end BERT model for the masked language modeling task.
 
     This model will train BERT on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` constructor.
 
@@ -47,15 +43,15 @@
 
     Args:
         backbone: A `keras_nlp.models.BertBackbone` instance.
         preprocessor: A `keras_nlp.models.BertMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
-    Example usage:
+    Examples:
 
     Raw string data.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
     # Pretrained language model.
     masked_lm = keras_nlp.models.BertMaskedLM.from_preset(
@@ -91,14 +87,17 @@
         "bert_base_en_uncased",
         preprocessor=None,
     )
     masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = BertBackbone
+    preprocessor_cls = BertMaskedLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -126,29 +125,7 @@
         )
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.backbone = backbone
-        self.preprocessor = preprocessor
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return BertBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return BertMaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,31 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
-from keras_nlp.src.models.bert.bert_presets import backbone_presets
-from keras_nlp.src.models.bert.bert_presets import classifier_presets
 from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
-
-PRESET_NAMES = ", ".join(list(backbone_presets) + list(classifier_presets))
 
 
 @keras_nlp_export("keras_nlp.models.BertPreprocessor")
 class BertPreprocessor(Preprocessor):
     """A BERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -126,14 +119,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = BertTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -183,15 +178,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return BertTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy({**backbone_presets, **classifier_presets})
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bert/bert_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,110 +8,126 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.bert.bert_presets import backbone_presets
-from keras_nlp.src.models.bert.bert_presets import classifier_presets
-from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 
-PRESET_NAMES = ", ".join(list(backbone_presets) + list(classifier_presets))
 
-
-@keras_nlp_export("keras_nlp.models.BertTokenizer")
-class BertTokenizer(WordPieceTokenizer):
-    """A BERT tokenizer using WordPiece subword segmentation.
+@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
+class RobertaTokenizer(BytePairTokenizer):
+    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
-    is based on `keras_nlp.tokenizers.WordPieceTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by BERT
+    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by RoBERTa
     models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a BERT preset.
+    a matching vocabulary for a RoBERTa preset.
 
     This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.BertPreprocessor` layer for input packing.
+    combined with a `keras_nlp.models.RobertaPreprocessor` layer for input
+    packing.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
-        vocabulary: A list of strings or a string filename path. If
-            passing a list, each element of the list should be a single word
-            piece token string. If passing a filename, the file should be a
-            plain text file containing a single word piece token per line.
-        lowercase: If `True`, the input text will be first lowered before
-            tokenization.
+        vocabulary: A dictionary mapping tokens to integer ids, or file path
+            to a json file containing the token to id mapping.
+        merges: A list of merge rules or a string file path, If passing a file
+            path. the file should have one merge rule per line. Every merge
+            rule contains merge entities separated by a space.
 
     Examples:
     ```python
     # Unbatched input.
-    tokenizer = keras_nlp.models.BertTokenizer.from_preset(
-        "bert_base_en_uncased",
+    tokenizer = keras_nlp.models.RobertaTokenizer.from_preset(
+        "roberta_base_en",
     )
     tokenizer("The quick brown fox jumped.")
 
     # Batched input.
     tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
     tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
 
     # Custom vocabulary.
-    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
-    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
-    tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
-    tokenizer("The quick brown fox jumped.")
+    # Note: 'Ġ' is space
+    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
+    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.RobertaTokenizer(
+        vocabulary=vocab,
+        merges=merges
+    )
+    tokenizer(["a quick fox", "a fox quick"])
     ```
     """
 
     def __init__(
         self,
         vocabulary=None,
-        lowercase=False,
+        merges=None,
         **kwargs,
     ):
-        self.cls_token = "[CLS]"
-        self.sep_token = "[SEP]"
-        self.pad_token = "[PAD]"
-        self.mask_token = "[MASK]"
+        self.start_token = "<s>"
+        self.pad_token = "<pad>"
+        self.end_token = "</s>"
+        self.mask_token = "<mask>"
+
         super().__init__(
             vocabulary=vocabulary,
-            lowercase=lowercase,
+            merges=merges,
+            unsplittable_tokens=[
+                self.start_token,
+                self.pad_token,
+                self.end_token,
+                self.mask_token,
+            ],
             **kwargs,
         )
 
-    def set_vocabulary(self, vocabulary):
-        super().set_vocabulary(vocabulary)
+    def set_vocabulary_and_merges(self, vocabulary, merges):
+        super().set_vocabulary_and_merges(vocabulary, merges)
 
         if vocabulary is not None:
             # Check for necessary special tokens.
-            for token in [self.cls_token, self.pad_token, self.sep_token]:
+            for token in [
+                self.start_token,
+                self.pad_token,
+                self.end_token,
+                self.mask_token,
+            ]:
                 if token not in self.vocabulary:
                     raise ValueError(
                         f"Cannot find token `'{token}'` in the provided "
                         f"`vocabulary`. Please provide `'{token}'` in your "
                         "`vocabulary` or use a pretrained `vocabulary` name."
                     )
 
-            self.cls_token_id = self.token_to_id(self.cls_token)
-            self.sep_token_id = self.token_to_id(self.sep_token)
+            self.start_token_id = self.token_to_id(self.start_token)
             self.pad_token_id = self.token_to_id(self.pad_token)
+            self.end_token_id = self.token_to_id(self.end_token)
             self.mask_token_id = self.token_to_id(self.mask_token)
         else:
-            self.cls_token_id = None
-            self.sep_token_id = None
+            self.start_token_id = None
             self.pad_token_id = None
+            self.end_token_id = None
             self.mask_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy({**backbone_presets, **classifier_presets})
+    def get_config(self):
+        config = super().get_config()
+        # In the constructor, we pass the list of special tokens to the
+        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
+        # delete it from the config here.
+        del config["unsplittable_tokens"]
+        return config
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,177 +7,191 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 
+
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
+from keras_nlp.src.layers.modeling.transformer_decoder import TransformerDecoder
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.bloom.bloom_decoder import BloomDecoder
-from keras_nlp.src.models.bloom.bloom_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import gelu_approximate
 
 
-def _bloom_kernel_initializer(stddev=0.02):
+def _gpt_2_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
-class BloomBackbone(Backbone):
-    """A BLOOM decoder network.
-
-    This network implements a Transformer-based decoder network, BigScience
-    Language Open-science Open-access Multilingual (BLOOM), as descriped in
-    ["BLOOM: A 176B-Parameter Open-Access Multilingual Language Model"](https://arxiv.org/pdf/2211.05100.pdf).
+@keras_nlp_export("keras_nlp.models.GPT2Backbone")
+class GPT2Backbone(Backbone):
+    """GPT-2 core network with hyperparameters.
+
+    This network implements a Transformer-based decoder network,
+    Generative Pretrained Transformer-2 (GPT-2), as described in
+    ["Language Models are Unsupervised Multitask Learners"](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf).
+    It includes the embedding lookups and transformer layers.
 
     The default constructor gives a fully customizable, randomly initialized
-    Bloom model with any number of layers, heads, and embedding dimensions. To
-    load preset architectures and weights, use the `from_preset()` constructor.
+    GPT-2 model with any number of layers, heads, and embedding
+    dimensions. To load preset architectures and weights, use the `from_preset`
+    constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available [here](https://huggingface.co/spaces/bigscience/license).
+    third party and subject to a separate license, available
+    [here](https://github.com/openai/gpt-2).
 
     Args:
         vocabulary_size: int. The size of the token vocabulary.
         num_layers: int. The number of transformer layers.
         num_heads: int. The number of attention heads for each transformer.
             The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The dimensionality of the embeddings and hidden states.
+        hidden_dim: int. The size of the transformer encoding and pooler layers.
         intermediate_dim: int. The output dimension of the first Dense layer in
-            the MLP network of each transformer.
-        dropout: float. Dropout probability for the Transformer decoder.
-        layer_norm_epsilon: float. Epsilon for the layer normalization layers in
-            the transformer decoder.
-        max_sequence_length: int. The maximum sequence length that this decoder
-            can consume.
+            a two-layer feedforward network for each transformer.
+        dropout: float. Dropout probability for the Transformer encoder.
+        max_sequence_length: int. The maximum sequence length that this encoder
+            can consume. If `None`, `max_sequence_length` uses the value from
+            sequence length. This determines the variable shape for positional
+            embeddings.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
-            for model computations and weights. Note that some computations,
-            such as softmax and layer normalization, will always be done at
-            float32 precision regardless of dtype.
+            for the models computations and weights. Note that some
+            computations, such as softmax and layer normalization will always
+            be done a float32 precision regardless of dtype.
 
-    Examples:
+    Example:
     ```python
     input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
     }
 
-    # Pretrained BLOOM decoder.
-    model = keras_nlp.models.BloomBackbone.from_preset("bloom_560m_multi")
+    # Pretrained GPT-2 decoder.
+    model = keras_nlp.models.GPT2Backbone.from_preset("gpt2_base_en")
     model(input_data)
 
-    # Randomly initialized BLOOM decoder with a custom config.
-    model = keras_nlp.models.BloomBackbone(
-        vocabulary_size=10,
-        num_layers=2,
-        num_heads=2,
-        hidden_dim=32,
-        intermediate_dim=32*4,
-        dropout=0.0,
-        layer_norm_epsilon=1e-5,
-        max_sequence_length=128,
+    # Randomly initialized GPT-2 decoder with custom config.
+    model = keras_nlp.models.GPT2Backbone(
+        vocabulary_size=50257,
+        num_layers=12,
+        num_heads=12,
+        hidden_dim=768,
+        intermediate_dim=3072,
+        max_sequence_length=1024,
     )
     model(input_data)
     ```
-
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
         num_heads,
         hidden_dim,
         intermediate_dim,
-        dropout=0.0,
-        layer_norm_epsilon=1e-5,
-        max_sequence_length=2048,
+        dropout=0.1,
+        max_sequence_length=1024,
         dtype=None,
         **kwargs,
     ):
         # === Layers ===
         self.token_embedding = ReversibleEmbedding(
             input_dim=vocabulary_size,
             output_dim=hidden_dim,
-            embeddings_initializer=_bloom_kernel_initializer(stddev=0.02),
-            tie_weights=False,
+            embeddings_initializer=_gpt_2_kernel_initializer(stddev=0.01),
             dtype=dtype,
             name="token_embedding",
         )
-        self.embeddings_layer_norm = keras.layers.LayerNormalization(
-            epsilon=layer_norm_epsilon,
+        self.position_embedding = PositionEmbedding(
+            initializer=_gpt_2_kernel_initializer(stddev=0.02),
+            sequence_length=max_sequence_length,
+            dtype=dtype,
+            name="position_embedding",
+        )
+        self.embeddings_add = keras.layers.Add(
             dtype=dtype,
-            name="token_embedding_layernorm",
+            name="embeddings_add",
+        )
+        self.embeddings_dropout = keras.layers.Dropout(
+            dropout,
+            dtype=dtype,
+            name="embeddings_dropout",
         )
         self.transformer_layers = []
         for i in range(num_layers):
-            layer = BloomDecoder(
-                num_heads=num_heads,
-                intermediate_dim=intermediate_dim,
-                dropout=dropout,
-                layer_norm_epsilon=layer_norm_epsilon,
-                dtype=dtype,
-                name=f"transformer_layer_{i}",
+            self.transformer_layers.append(
+                TransformerDecoder(
+                    intermediate_dim=intermediate_dim,
+                    num_heads=num_heads,
+                    dropout=dropout,
+                    layer_norm_epsilon=1e-05,
+                    activation=gelu_approximate,
+                    kernel_initializer=_gpt_2_kernel_initializer(stddev=0.02),
+                    normalize_first=True,
+                    dtype=dtype,
+                    name=f"transformer_layer_{i}",
+                )
             )
-            self.transformer_layers.append(layer)
         self.layer_norm = keras.layers.LayerNormalization(
-            epsilon=layer_norm_epsilon,
+            axis=-1,
+            epsilon=1e-05,
             dtype=dtype,
-            name="final_layernorm",
+            name="layer_norm",
         )
 
         # === Functional Model ===
         token_id_input = keras.Input(
             shape=(None,), dtype="int32", name="token_ids"
         )
         padding_mask_input = keras.Input(
             shape=(None,), dtype="int32", name="padding_mask"
         )
-        x = self.token_embedding(token_id_input)
-        x = self.embeddings_layer_norm(x)
+        # Embed inputs.
+        tokens = self.token_embedding(token_id_input)
+        positions = self.position_embedding(tokens)
+        x = self.embeddings_add((tokens, positions))
+        x = self.embeddings_dropout(x)
+        # Apply transformer layers.
         for transformer_layer in self.transformer_layers:
             x = transformer_layer(x, decoder_padding_mask=padding_mask_input)
         sequence_output = self.layer_norm(x)
+        # Instantiate using the Functional constructor.
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=sequence_output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
-        self.layer_norm_epsilon = layer_norm_epsilon
         self.max_sequence_length = max_sequence_length
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "vocabulary_size": self.vocabulary_size,
                 "num_layers": self.num_layers,
                 "num_heads": self.num_heads,
                 "hidden_dim": self.hidden_dim,
                 "intermediate_dim": self.intermediate_dim,
                 "dropout": self.dropout,
-                "layer_norm_epsilon": self.layer_norm_epsilon,
                 "max_sequence_length": self.max_sequence_length,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_causal_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_causal_lm_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 from absl import logging
 
-from keras_nlp.src.backend import keras
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import ops
 from keras_nlp.src.models.bloom.bloom_preprocessor import BloomPreprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.BloomCausalLMPreprocessor")
 class BloomCausalLMPreprocessor(BloomPreprocessor):
     """BLOOM Causal LM preprocessor.
 
     This preprocessing layer is meant for use with
     `keras_nlp.models.BloomCausalLM`. By default, it will take in batches of
     strings, and return outputs in a `(x, y, sample_weight)` format, where the
     `y` label is the next token id in the `x` sequence.
@@ -127,15 +127,15 @@
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     def generate_preprocess(
         self,
         x,
         sequence_length=None,
     ):
-        """Covert strings to integer token input for generation.
+        """Convert strings to integer token input for generation.
 
         Similar to calling the layer for training, this method takes in strings
         or tensor strings, tokenizes and packs the input, and computes a padding
         mask masking all inputs not filled in with a padded value.
 
         Unlike calling the layer for training, this method does not compute
         labels and will never append a `tokenizer.end_token_id` to the end of
@@ -155,15 +155,15 @@
             "padding_mask": padding_mask,
         }
 
     def generate_postprocess(
         self,
         x,
     ):
-        """Covert integer token output to strings for generation.
+        """Convert integer token output to strings for generation.
 
         This method reverses `generate_preprocess()`, by first removing all
         padding and start/end tokens, and then converting the integer sequence
         back to a string.
         """
         if not self.built:
             self.build(None)
@@ -171,13 +171,13 @@
         token_ids, padding_mask = x["token_ids"], x["padding_mask"]
         token_ids = ops.convert_to_numpy(token_ids)
         padding_mask = ops.convert_to_numpy(padding_mask)
         # Strip any special tokens during detokenization (e.g. the start and
         # end markers). In the future we could make this configurable.
         padding_mask = (
             padding_mask
-            & (token_ids != self.tokenizer.eos_token_id)
-            & (token_ids != self.tokenizer.bos_token_id)
+            & (token_ids != self.tokenizer.start_token_id)
+            & (token_ids != self.tokenizer.end_token_id)
         )
         token_ids = tf.ragged.boolean_mask(token_ids, padding_mask)
         return self.tokenizer.detokenize(token_ids)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_decoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_transformer_decoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,210 +1,255 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2024 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# from keras_nlp.src.backend import keras
-# from keras_nlp.src.backend import ops
+import math
+
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.transformer_layer_utils import (
     compute_causal_mask,
 )
 from keras_nlp.src.layers.modeling.transformer_layer_utils import (
     merge_padding_and_attention_mask,
 )
-from keras_nlp.src.models.bloom.bloom_attention import BloomAttention
-from keras_nlp.src.utils.keras_utils import clone_initializer
+from keras_nlp.src.models.falcon.falcon_attention import FalconAttention
 
 
-class BloomDecoder(keras.layers.Layer):
+class FalconTransformerDecoder(keras.layers.Layer):
     def __init__(
         self,
-        num_heads,
+        num_attention_heads,
         intermediate_dim,
-        dropout=0.0,
         layer_norm_epsilon=1e-5,
-        kernel_initializer="glorot_uniform",
-        bias_initializer="zeros",
+        attention_dropout_rate=0,
+        feedforward_dropout_rate=0,
         **kwargs,
     ):
         super().__init__(**kwargs)
-
-        self.num_heads = num_heads
+        self.num_attention_heads = num_attention_heads
         self.intermediate_dim = intermediate_dim
-        self.dropout = dropout
         self.layer_norm_epsilon = layer_norm_epsilon
-        self.kernel_initializer = keras.initializers.get(kernel_initializer)
-        self.bias_initializer = keras.initializers.get(bias_initializer)
+        self.attention_dropout_rate = attention_dropout_rate
+        self.feedforward_dropout_rate = feedforward_dropout_rate
 
     def build(self, decoder_sequence_shape):
-        hidden_dim = decoder_sequence_shape[-1]
-        head_dim = int(hidden_dim // self.num_heads)
-
-        if head_dim * self.num_heads != hidden_dim:
-            raise ValueError(
-                f"`hidden_dim` must be divisible by num_heads (got `hidden_dim`"
-                f": {hidden_dim} and `num_heads`: {self.num_heads})."
-            )
-
-        self._pre_attention_layernorm = keras.layers.LayerNormalization(
+        self.hidden_dim = decoder_sequence_shape[-1]
+        self.input_layernorm = keras.layers.LayerNormalization(
             epsilon=self.layer_norm_epsilon,
             dtype=self.dtype_policy,
-            name="pre_attention_layernorm",
+            name="input_layernorm",
+        )
+        self.input_layernorm.build(decoder_sequence_shape)
+
+        # Attention layers.
+        self.key_dim = self.hidden_dim // self.num_attention_heads
+        self.attention_layer = FalconAttention(
+            num_heads=self.num_attention_heads,
+            attention_dropout_rate=self.attention_dropout_rate,
+            dtype=self.dtype_policy,
+            name="attention",
+        )
+        self.attention_layer.build(
+            decoder_sequence_shape,
         )
-        self._pre_attention_layernorm.build(decoder_sequence_shape)
 
-        self._self_attention_layer = BloomAttention(
-            num_heads=self.num_heads,
-            dropout=self.dropout,
-            kernel_initializer=clone_initializer(self.kernel_initializer),
-            bias_initializer=clone_initializer(self.bias_initializer),
+        self.attention_dropout = keras.layers.Dropout(
+            rate=self.attention_dropout_rate,
             dtype=self.dtype_policy,
-            name="self_attention",
+            name="attention_dropout",
         )
-        self._self_attention_layer.build(decoder_sequence_shape)
 
-        self._post_attention_layernorm = keras.layers.LayerNormalization(
+        self.post_attention_layernorm = keras.layers.LayerNormalization(
             epsilon=self.layer_norm_epsilon,
             dtype=self.dtype_policy,
             name="post_attention_layernorm",
         )
-        self._post_attention_layernorm.build(decoder_sequence_shape)
+        self.post_attention_layernorm.build(decoder_sequence_shape)
 
-        self._mlp_intermediate_dense = keras.layers.Dense(
+        # Feedforward layers.
+        # TODO: use_bias should be an argument to the transformer to support
+        # other sizes of models, e.g. 7B, that don't use bias.
+        self.dense_h_to_4h = keras.layers.Dense(
             self.intermediate_dim,
-            kernel_initializer=clone_initializer(self.kernel_initializer),
-            bias_initializer=clone_initializer(self.bias_initializer),
+            activation=keras.activations.gelu,
+            use_bias=True,
             dtype=self.dtype_policy,
-            name="mlp_intermediate_dense",
+            name="dense_h_to_4h",
         )
-        self._mlp_intermediate_dense.build(decoder_sequence_shape)
+        self.dense_h_to_4h.build(decoder_sequence_shape)
 
-        self._mlp_output_dense = keras.layers.Dense(
-            hidden_dim,
-            kernel_initializer=clone_initializer(self.kernel_initializer),
-            bias_initializer=clone_initializer(self.bias_initializer),
+        self.dense_4h_to_h = keras.layers.Dense(
+            self.hidden_dim,
+            use_bias=True,
             dtype=self.dtype_policy,
-            name="mlp_output_dense",
+            name="dense_4h_to_h",
+        )
+        self.dense_4h_to_h.build(
+            (
+                decoder_sequence_shape[0],
+                decoder_sequence_shape[1],
+                self.intermediate_dim,
+            )
         )
-        intermediate_shape = list(decoder_sequence_shape)
-        intermediate_shape[-1] = self.intermediate_dim
-        self._mlp_output_dense.build(tuple(intermediate_shape))
 
-        self._dropout_layer = keras.layers.Dropout(
-            rate=self.dropout, dtype=self.dtype_policy, name="dropout"
+        self.feedforward_dropout = keras.layers.Dropout(
+            rate=self.feedforward_dropout_rate,
+            dtype=self.dtype_policy,
+            name="feedforward_dropout",
         )
 
         self.built = True
 
     def call(
         self,
-        decoder_sequence,
+        inputs,
         decoder_padding_mask=None,
         decoder_attention_mask=None,
         attention_cache=None,
         attention_cache_update_index=None,
-        use_causal_mask=True,
+        training=None,
     ):
-        self_attention_mask = self._compute_attention_mask(
-            decoder_sequence=decoder_sequence,
+        attention_mask = self._compute_attention_mask(
+            decoder_sequence=inputs,
             decoder_padding_mask=decoder_padding_mask,
             decoder_attention_mask=decoder_attention_mask,
-            use_causal_mask=use_causal_mask,
             attention_cache=attention_cache,
             attention_cache_update_index=attention_cache_update_index,
         )
 
-        residual = decoder_sequence
-        x = self._pre_attention_layernorm(decoder_sequence)
+        residual = inputs
+
+        x = self.input_layernorm(inputs)
 
-        attention_output = self._self_attention_layer(
-            hidden_states=x,
-            attention_mask=self_attention_mask,
+        alibi = self._build_alibi_tensor(
+            self.num_attention_heads, decoder_padding_mask
+        )
+
+        # Attention block.
+        attention_output = self.attention_layer(
+            inputs=x,
+            alibi=alibi,
+            attention_mask=attention_mask,
             cache=attention_cache,
             cache_update_index=attention_cache_update_index,
         )
 
         if attention_cache is None:
             x = attention_output
         else:
             x, attention_cache = attention_output
 
+        x = self.attention_dropout(x, training=training)
+
         x = x + residual
         residual = x
-        x = self._post_attention_layernorm(x)
-        x = self._mlp_intermediate_dense(x)
-        x = keras.activations.gelu(x, approximate=True)
-        x = self._mlp_output_dense(x)
-        x = self._dropout_layer(x)
+
+        x = self.post_attention_layernorm(x)
+
+        x = self.dense_h_to_4h(x)
+        x = self.dense_4h_to_h(x)
+
+        x = self.feedforward_dropout(x, training=training)
+
         x = x + residual
 
         if attention_cache is not None:
             return x, attention_cache
         else:
             return x
 
-    def _compute_attention_mask(
-        self,
-        decoder_sequence,
-        decoder_padding_mask,
-        decoder_attention_mask,
-        use_causal_mask,
-        attention_cache,
-        attention_cache_update_index,
-    ):
-        decoder_mask = merge_padding_and_attention_mask(
-            decoder_sequence, decoder_padding_mask, decoder_attention_mask
-        )
-        if use_causal_mask:
-            batch_size = ops.shape(decoder_sequence)[0]
-            input_length = output_length = ops.shape(decoder_sequence)[1]
-            if attention_cache is not None:
-                input_length = ops.shape(attention_cache)[2]
-
-            causal_mask = compute_causal_mask(
-                batch_size,
-                input_length,
-                output_length,
-                (
-                    0
-                    if attention_cache_update_index is None
-                    else attention_cache_update_index
-                ),
-            )
-            return (
-                ops.minimum(decoder_mask, causal_mask)
-                if decoder_mask is not None
-                else causal_mask
-            )
-        return decoder_mask
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "num_heads": self.num_heads,
+                "num_attention_heads": self.num_attention_heads,
                 "intermediate_dim": self.intermediate_dim,
-                "dropout": self.dropout,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
-                "kernel_initializer": keras.initializers.serialize(
-                    self.kernel_initializer
-                ),
-                "bias_initializer": keras.initializers.serialize(
-                    self.bias_initializer
-                ),
+                "attention_dropout_rate": self.attention_dropout_rate,
+                "feedforward_dropout_rate": self.feedforward_dropout_rate,
             }
         )
         return config
 
     def compute_output_shape(self, decoder_sequence_shape):
         return decoder_sequence_shape
 
+    def _compute_attention_mask(
+        self,
+        decoder_sequence,
+        decoder_padding_mask,
+        decoder_attention_mask,
+        attention_cache=None,
+        attention_cache_update_index=None,
+    ):
+        decoder_mask = merge_padding_and_attention_mask(
+            decoder_sequence, decoder_padding_mask, decoder_attention_mask
+        )
+        batch_size = ops.shape(decoder_sequence)[0]
+        input_length = output_length = ops.shape(decoder_sequence)[1]
+        # We need to handle a rectangular causal mask when doing cached
+        # decoding. For generative inference, `decoder_sequence` will
+        # generally be length 1, and `cache` will be the full generation length.
+        if attention_cache is not None:
+            input_length = ops.shape(attention_cache)[2]
+
+        causal_mask = compute_causal_mask(
+            batch_size,
+            input_length,
+            output_length,
+            (
+                0
+                if attention_cache_update_index is None
+                else attention_cache_update_index
+            ),
+        )
+        return (
+            ops.minimum(decoder_mask, causal_mask)
+            if decoder_mask is not None
+            else causal_mask
+        )
+
+    def _build_alibi_tensor(self, num_heads, attention_mask):
+        batch_size, seq_length = attention_mask.shape
+        slopes = ops.convert_to_tensor(
+            self._get_slopes(num_heads),
+            dtype=self.compute_dtype,
+        )  # num_heads
+        arange_tensor = (
+            (
+                ops.cast(ops.cumsum(attention_mask, axis=-1) - 1, dtype="int32")
+                * attention_mask
+            )
+        )[:, None, :]
+        alibi = slopes[..., None] * ops.cast(arange_tensor, self.compute_dtype)
+        alibi = ops.expand_dims(
+            alibi, 0
+        )  # [None, batch_size, num_heads, seq_length]
+        return ops.transpose(alibi, [1, 2, 0, 3])
+
+    def _get_slopes(self, num_heads):
+        def get_slopes_power_of_2(n):
+            start = 2 ** (-(2 ** -(math.log2(n) - 3)))
+            ratio = start
+            return [start * ratio**i for i in range(n)]
+
+        if math.log2(num_heads).is_integer():
+            return get_slopes_power_of_2(num_heads)
+        else:
+            closest_power_of_2 = 2 ** math.floor(math.log2(num_heads))
+            return (
+                get_slopes_power_of_2(closest_power_of_2)
+                + self._get_slopes(2 * closest_power_of_2)[0::2][
+                    : num_heads - closest_power_of_2
+                ]
+            )
+
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
-from keras_nlp.src.backend import keras
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
-from keras_nlp.src.models.bloom.bloom_presets import backbone_presets
 from keras_nlp.src.models.bloom.bloom_tokenizer import BloomTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.BloomPreprocessor")
 class BloomPreprocessor(Preprocessor):
     """BLOOM preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
 
     - Tokenize the inputs using the `tokenizer`.
     - Construct a dictionary with keys `"token_ids"`, `"padding_mask"`, that can
@@ -103,14 +100,16 @@
 
     # Map unlabeled single sentences.
     ds = tf.data.Dataset.from_tensor_slices(text)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
+    tokenizer_cls = BloomTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=2048,
         add_start_token=True,
         add_end_token=True,
         **kwargs,
@@ -122,16 +121,16 @@
         self.add_start_token = add_start_token
         self.add_end_token = add_end_token
 
     def build(self, input_shape):
         # Defer packer creation to `build()` so that we can be sure tokenizer
         # assets have loaded when restoring a saved model.
         self.packer = StartEndPacker(
-            start_value=self.tokenizer.bos_token_id,
-            end_value=self.tokenizer.eos_token_id,
+            start_value=self.tokenizer.start_token_id,
+            end_value=self.tokenizer.end_token_id,
             pad_value=self.tokenizer.pad_token_id,
             sequence_length=self.sequence_length,
             return_padding_mask=True,
         )
         self.built = True
 
     def call(
@@ -180,15 +179,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def tokenizer_cls(cls):
-        return BloomTokenizer
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/bloom/bloom_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/falcon/falcon_tokenizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2024 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
-from keras_nlp.src.backend import keras
-from keras_nlp.src.models.bloom.bloom_presets import backbone_presets
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
-class BloomTokenizer(BytePairTokenizer):
-    """A BLOOM tokenizer using Byte-Pair Encoding subword segmentation.
+@keras_nlp_export("keras_nlp.models.FalconTokenizer")
+class FalconTokenizer(BytePairTokenizer):
+    """Falcon tokenizer based on BytePairTokenizer.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by BLOOM
+    underlying tokenizer, it will check for all special tokens needed by Falcon
     models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a BLOOM preset.
+    a matching vocabulary for a Falcon preset.
 
     This tokenizer does not provide truncation or padding of inputs.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
@@ -46,78 +43,68 @@
             should have one merge rule per line. Every merge rule contains
             merge entities separated by a space.
 
     Examples:
 
     ```python
     # Unbatched input.
-    tokenizer = keras_nlp.models.BloomTokenizer.from_preset("bloom_560m_multi")
+    tokenizer = keras_nlp.models.FalconTokenizer.from_preset("falcon_refinedweb_1b_en")
     tokenizer("The quick brown fox jumped.")
 
     # Batched input.
     tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
     tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
 
     # Custom vocabulary.
-    vocab = {"<s>": 0, "</s>": 1, "<pad>": 2, "a": 3, "Ġquick": 4, "Ġfox": 5}
+    vocab = {"<|endoftext|>": 0, "a": 4, "Ġquick": 5, "Ġfox": 6}
     merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
     merges += ["Ġ f", "o x", "Ġf ox"]
-    tokenizer = keras_nlp.models.BloomTokenizer(vocabulary=vocab, merges=merges)
+    tokenizer = keras_nlp.models.FalconTokenizer(vocabulary=vocab, merges=merges)
     tokenizer("a quick fox.")
     ```
     """
 
     def __init__(
         self,
         vocabulary=None,
         merges=None,
         **kwargs,
     ):
-        self.bos_token = "<s>"
-        self.eos_token = "</s>"
-        self.pad_token = "<pad>"
+        # Falcon uses the same start as end token, i.e., "<|endoftext|>".
+        self.end_token = self.start_token = "<|endoftext|>"
 
         super().__init__(
             vocabulary=vocabulary,
             merges=merges,
-            unsplittable_tokens=[
-                self.bos_token,
-                self.eos_token,
-                self.pad_token,
-            ],
+            unsplittable_tokens=[self.end_token],
             **kwargs,
         )
 
     def set_vocabulary_and_merges(self, vocabulary, merges):
         super().set_vocabulary_and_merges(vocabulary, merges)
 
         if vocabulary is not None:
             # Check for necessary special tokens.
-            for token in [self.bos_token, self.eos_token, self.pad_token]:
-                if token not in self.get_vocabulary():
-                    raise ValueError(
-                        f"Cannot find token `'{token}'` in the provided "
-                        f"`vocabulary`. Please provide `'{token}'` in "
-                        "your `vocabulary` or use a pretrained `vocabulary` name."
-                    )
-
-            self.bos_token_id = self.token_to_id(self.bos_token)
-            self.eos_token_id = self.token_to_id(self.eos_token)
-            self.pad_token_id = self.token_to_id(self.pad_token)
+            if self.end_token not in self.get_vocabulary():
+                raise ValueError(
+                    f"Cannot find token `'{self.end_token}'` in the provided "
+                    f"`vocabulary`. Please provide `'{self.end_token}'` in "
+                    "your `vocabulary` or use a pretrained `vocabulary` name."
+                )
+
+            self.end_token_id = self.token_to_id(self.end_token)
+            self.start_token_id = self.end_token_id
+            self.pad_token_id = 0
         else:
-            self.bos_token_id = None
-            self.eos_token_id = None
+            self.end_token_id = None
+            self.start_token_id = None
             self.pad_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,7 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.utils.preset_utils import register_presets
+
+register_presets(backbone_presets, (FNetBackbone, FNetTokenizer))
+
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
 from keras_nlp.src.models.deberta_v3.disentangled_attention_encoder import (
     DisentangledAttentionEncoder,
 )
 from keras_nlp.src.models.deberta_v3.relative_embedding import RelativeEmbedding
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def deberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Backbone")
@@ -174,14 +171,15 @@
             )
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=x,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
@@ -204,11 +202,7 @@
                 "dropout": self.dropout,
                 "max_sequence_length": self.max_sequence_length,
                 "bucket_size": self.bucket_size,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.models.classifier import Classifier
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import (
     deberta_kernel_initializer,
 )
 from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Classifier")
-class DebertaV3Classifier(Task):
+class DebertaV3Classifier(Classifier):
     """An end-to-end DeBERTa model for classification tasks.
 
     This model attaches a classification head to a
     `keras_nlp.model.DebertaV3Backbone` model, mapping from the backbone
     outputs to logit output suitable for a classification task. For usage of
     this model with pre-trained weights, see the `from_preset()` method.
 
@@ -149,14 +146,17 @@
         preprocessor=preprocessor,
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = DebertaV3Backbone
+    preprocessor_cls = DebertaV3Preprocessor
+
     def __init__(
         self,
         backbone,
         num_classes,
         preprocessor=None,
         activation=None,
         hidden_dim=None,
@@ -208,42 +208,19 @@
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.num_classes = num_classes
         self.activation = keras.activations.get(activation)
         self.hidden_dim = hidden_dim
         self.dropout = dropout
 
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "activation": keras.activations.serialize(self.activation),
                 "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return DebertaV3Backbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return DebertaV3Preprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import (
     deberta_kernel_initializer,
 )
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
-from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.masked_lm import MaskedLM
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3MaskedLM")
-class DebertaV3MaskedLM(Task):
+class DebertaV3MaskedLM(MaskedLM):
     """An end-to-end DeBERTaV3 model for the masked language modeling task.
 
     This model will train DeBERTaV3 on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` method.
 
@@ -51,15 +48,15 @@
 
     Args:
         backbone: A `keras_nlp.models.DebertaV3Backbone` instance.
         preprocessor: A `keras_nlp.models.DebertaV3MaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
-    Example usage:
+    Examples:
 
     Raw string data.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
     # Pretrained language model.
     masked_lm = keras_nlp.models.DebertaV3MaskedLM.from_preset(
@@ -94,14 +91,17 @@
         "deberta_v3_base_en",
         preprocessor=None,
     )
     masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = DebertaV3Backbone
+    preprocessor_cls = DebertaV3MaskedLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -127,27 +127,7 @@
         outputs = self.masked_lm_head(x, inputs["mask_positions"])
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return DebertaV3Backbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return DebertaV3MaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
-from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
 from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Preprocessor")
 class DebertaV3Preprocessor(Preprocessor):
     """A DeBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -143,14 +140,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = DebertaV3Tokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -199,15 +198,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return DebertaV3Tokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Tokenizer")
 class DebertaV3Tokenizer(SentencePieceTokenizer):
     """DeBERTa tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -148,11 +145,7 @@
             return self.mask_token_id
         return super().token_to_id(token)
 
     def detokenize(self, ids):
         ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
         return super().detokenize(ids)
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/deberta_v3/relative_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
 from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def distilbert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertBackbone")
@@ -155,14 +152,15 @@
             x = transformer_layer(x, padding_mask=padding_mask_input)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=x,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
@@ -183,11 +181,7 @@
                 "intermediate_dim": self.intermediate_dim,
                 "dropout": self.dropout,
                 "max_sequence_length": self.max_sequence_length,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_classifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,32 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.models.classifier import Classifier
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import (
     distilbert_kernel_initializer,
 )
 from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertClassifier")
-class DistilBertClassifier(Task):
+class DistilBertClassifier(Classifier):
     """An end-to-end DistilBERT model for classification tasks.
 
     This model attaches a classification head to a
     `keras_nlp.model.DistilBertBackbone` instance, mapping from the backbone
     outputs to logits suitable for a classification task. For usage of
     this model with pre-trained weights, see the `from_preset()` constructor.
 
@@ -136,14 +133,17 @@
         preprocessor=preprocessor,
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = DistilBertBackbone
+    preprocessor_cls = DistilBertPreprocessor
+
     def __init__(
         self,
         backbone,
         num_classes,
         preprocessor=None,
         activation=None,
         hidden_dim=None,
@@ -188,42 +188,19 @@
 
         # === Config ===
         self.num_classes = num_classes
         self.activation = keras.activations.get(activation)
         self.hidden_dim = hidden_dim
         self.dropout = dropout
 
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "activation": keras.activations.serialize(self.activation),
                 "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return DistilBertBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return DistilBertPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import (
     distilbert_kernel_initializer,
 )
 from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import (
     DistilBertMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.masked_lm import MaskedLM
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertMaskedLM")
-class DistilBertMaskedLM(Task):
+class DistilBertMaskedLM(MaskedLM):
     """An end-to-end DistilBERT model for the masked language modeling task.
 
     This model will train DistilBERT on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` constructor.
 
@@ -51,15 +48,15 @@
 
     Args:
         backbone: A `keras_nlp.models.DistilBertBackbone` instance.
         preprocessor: A `keras_nlp.models.DistilBertMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
-    Example usage:
+    Examples:
 
     Raw string data.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
     # Pretrained language model.
     masked_lm = keras_nlp.models.DistilBertMaskedLM.from_preset(
@@ -94,14 +91,17 @@
         "distil_bert_base_en_uncased",
         preprocessor=None,
     )
     masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = DistilBertBackbone
+    preprocessor_cls = DistilBertMaskedLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -129,27 +129,7 @@
         )
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return DistilBertBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return DistilBertMaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
-from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
 from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertPreprocessor")
 class DistilBertPreprocessor(Preprocessor):
     """A DistilBERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -114,14 +111,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = DistilBertTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -170,15 +169,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return DistilBertTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/distil_bert/distil_bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bert/bert_tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,108 +8,106 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
 from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras_nlp_export("keras_nlp.models.DistilBertTokenizer")
-class DistilBertTokenizer(WordPieceTokenizer):
-    """A DistilBERT tokenizer using WordPiece subword segmentation.
+@keras_nlp_export("keras_nlp.models.BertTokenizer")
+class BertTokenizer(WordPieceTokenizer):
+    """A BERT tokenizer using WordPiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.WordPieceTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by DistilBERT
+    underlying tokenizer, it will check for all special tokens needed by BERT
     models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a DistilBERT preset.
+    a matching vocabulary for a BERT preset.
 
     This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.DistilBertPreprocessor` layer for input packing.
+    combined with a `keras_nlp.models.BertPreprocessor` layer for input packing.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
         vocabulary: A list of strings or a string filename path. If
             passing a list, each element of the list should be a single word
             piece token string. If passing a filename, the file should be a
             plain text file containing a single word piece token per line.
         lowercase: If `True`, the input text will be first lowered before
             tokenization.
+        special_tokens_in_strings: bool. A bool to indicate if the tokenizer
+            should expect special tokens in input strings that should be
+            tokenized and mapped correctly to their ids. Defaults to False.
 
     Examples:
-
     ```python
     # Unbatched input.
-    tokenizer = keras_nlp.models.DistilBertTokenizer.from_preset(
-        "distil_bert_base_en_uncased",
+    tokenizer = keras_nlp.models.BertTokenizer.from_preset(
+        "bert_base_en_uncased",
     )
     tokenizer("The quick brown fox jumped.")
 
     # Batched input.
     tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
     tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
 
     # Custom vocabulary.
     vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
     vocab += ["The", "quick", "brown", "fox", "jumped", "."]
-    tokenizer = keras_nlp.models.DistilBertTokenizer(vocabulary=vocab)
+    tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
     tokenizer("The quick brown fox jumped.")
     ```
     """
 
     def __init__(
         self,
-        vocabulary,
+        vocabulary=None,
         lowercase=False,
+        special_tokens_in_strings=False,
         **kwargs,
     ):
         self.cls_token = "[CLS]"
         self.sep_token = "[SEP]"
         self.pad_token = "[PAD]"
         self.mask_token = "[MASK]"
         super().__init__(
             vocabulary=vocabulary,
             lowercase=lowercase,
+            special_tokens=[
+                self.cls_token,
+                self.sep_token,
+                self.pad_token,
+                self.mask_token,
+            ],
+            special_tokens_in_strings=special_tokens_in_strings,
             **kwargs,
         )
 
     def set_vocabulary(self, vocabulary):
         super().set_vocabulary(vocabulary)
 
         if vocabulary is not None:
-            # Check for necessary special tokens.
-            for token in [self.cls_token, self.pad_token, self.sep_token]:
-                if token not in self.vocabulary:
-                    raise ValueError(
-                        f"Cannot find token `'{token}'` in the provided "
-                        f"`vocabulary`. Please provide `'{token}'` in your "
-                        "`vocabulary` or use a pretrained `vocabulary` name."
-                    )
-
             self.cls_token_id = self.token_to_id(self.cls_token)
             self.sep_token_id = self.token_to_id(self.sep_token)
             self.pad_token_id = self.token_to_id(self.pad_token)
             self.mask_token_id = self.token_to_id(self.mask_token)
         else:
             self.cls_token_id = None
             self.sep_token_id = None
             self.pad_token_id = None
             self.mask_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+    def get_config(self):
+        config = super().get_config()
+        del config["special_tokens"]  # Not configurable; set in __init__.
+        return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/electra/electra_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/electra_backbone.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.utils.keras_utils import gelu_approximate
 
 
 def electra_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.ElectraBackbone")
 class ElectraBackbone(Backbone):
     """A Electra encoder network.
 
     This network implements a bidirectional Transformer-based encoder as
     described in ["Electra: Pre-training Text Encoders as Discriminators Rather
     Than Generators"](https://arxiv.org/abs/2003.10555). It includes the
     embedding lookups and transformer layers, but not the masked language model
     or classification task networks.
 
     The default constructor gives a fully customizable, randomly initialized
-    Electra encoder with any number of layers, heads, and embedding
-    dimensions.
+    ELECTRA encoder with any number of layers, heads, and embedding
+    dimensions. To load preset architectures and weights, use the
+    `from_preset()` constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://huggingface.co/docs/transformers/model_doc/electra#overview).
 
     Args:
@@ -58,21 +60,28 @@
             sequence length. This determines the variable shape for positional
             embeddings.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
             for model computations and weights. Note that some computations,
             such as softmax and layer normalization, will always be done at
             float32 precision regardless of dtype.
 
-    Examples:
+    Example:
         ```python
         input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
         "segment_ids": np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]]),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
         }
+
+        # Pre-trained ELECTRA encoder.
+        model = keras_nlp.models.ElectraBackbone.from_preset(
+            "electra_base_discriminator_en"
+        )
+        model(input_data)
+
         # Randomly initialized Electra encoder
         backbone = keras_nlp.models.ElectraBackbone(
             vocabulary_size=1000,
             num_layers=2,
             num_heads=2,
             hidden_dim=32,
             intermediate_dim=64,
@@ -197,14 +206,15 @@
                 "segment_ids": segment_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs={
                 "sequence_output": sequence_output,
                 "pooled_output": pooled_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocab_size = vocab_size
         self.num_layers = num_layers
         self.num_heads = num_heads
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/electra/electra_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/electra/electra_tokenizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_nlp.src.backend import keras
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.tokenizers import WordPieceTokenizer
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.ElectraTokenizer")
 class ElectraTokenizer(WordPieceTokenizer):
     """A ELECTRA tokenizer using WordPiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.WordPieceTokenizer`.
 
     If input is a batch of strings (rank > 0), the layer will output a
@@ -32,14 +32,17 @@
     Args:
         vocabulary: A list of strings or a string filename path. If
             passing a list, each element of the list should be a single word
             piece token string. If passing a filename, the file should be a
             plain text file containing a single word piece token per line.
         lowercase: If `True`, the input text will be first lowered before
             tokenization.
+        special_tokens_in_strings: bool. A bool to indicate if the tokenizer
+            should expect special tokens in input strings that should be
+            tokenized and mapped correctly to their ids. Defaults to False.
 
     Examples:
     ```python
     # Custom Vocabulary.
     vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
     vocab += ["The", "quick", "brown", "fox", "jumped", "."]
 
@@ -53,37 +56,50 @@
     tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
     tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
     ```
     """
 
-    def __init__(self, vocabulary, lowercase=False, **kwargs):
+    def __init__(
+        self,
+        vocabulary,
+        lowercase=False,
+        special_tokens_in_strings=False,
+        **kwargs,
+    ):
         self.cls_token = "[CLS]"
         self.sep_token = "[SEP]"
         self.pad_token = "[PAD]"
         self.mask_token = "[MASK]"
-        super().__init__(vocabulary=vocabulary, lowercase=lowercase, **kwargs)
+        super().__init__(
+            vocabulary=vocabulary,
+            lowercase=lowercase,
+            special_tokens=[
+                self.cls_token,
+                self.sep_token,
+                self.pad_token,
+                self.mask_token,
+            ],
+            special_tokens_in_strings=special_tokens_in_strings,
+            **kwargs,
+        )
 
     def set_vocabulary(self, vocabulary):
         super().set_vocabulary(vocabulary)
 
         if vocabulary is not None:
-            # Check for necessary special tokens.
-            for token in [self.cls_token, self.pad_token, self.sep_token]:
-                if token not in self.vocabulary:
-                    raise ValueError(
-                        f"Cannot find token `'{token}'` in the provided "
-                        f"`vocabulary`. Please provide `'{token}'` in your "
-                        "`vocabulary` or use a pretrained `vocabulary` name."
-                    )
-
             self.cls_token_id = self.token_to_id(self.cls_token)
             self.sep_token_id = self.token_to_id(self.sep_token)
             self.pad_token_id = self.token_to_id(self.pad_token)
             self.mask_token_id = self.token_to_id(self.mask_token)
         else:
             self.cls_token_id = None
             self.sep_token_id = None
             self.pad_token_id = None
             self.mask_token_id = None
 
+    def get_config(self):
+        config = super().get_config()
+        del config["special_tokens"]  # Not configurable; set in __init__.
+        return config
+
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.f_net_encoder import FNetEncoder
 from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.src.utils.keras_utils import gelu_approximate
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def f_net_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
 def f_net_bias_initializer(stddev=0.02):
@@ -202,14 +199,15 @@
                 "token_ids": token_id_input,
                 "segment_ids": segment_id_input,
             },
             outputs={
                 "sequence_output": sequence_output,
                 "pooled_output": pooled_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.hidden_dim = hidden_dim
@@ -230,11 +228,7 @@
                 "dropout": self.dropout,
                 "max_sequence_length": self.max_sequence_length,
                 "num_segments": self.num_segments,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.models.classifier import Classifier
 from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.src.models.f_net.f_net_backbone import f_net_kernel_initializer
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.FNetClassifier")
-class FNetClassifier(Task):
+class FNetClassifier(Classifier):
     """An end-to-end f_net model for classification tasks.
 
     This model attaches a classification head to a
     `keras_nlp.model.FNetBackbone` instance, mapping from the backbone outputs
     to logits suitable for a classification task. For usage of this model with
     pre-trained weights, use the `from_preset()` constructor.
 
@@ -96,14 +93,17 @@
         num_classes=4,
         preprocessor=None,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = FNetBackbone
+    preprocessor_cls = FNetPreprocessor
+
     def __init__(
         self,
         backbone,
         num_classes,
         preprocessor=None,
         activation=None,
         dropout=0.1,
@@ -137,41 +137,18 @@
         )
 
         # === Config ===
         self.num_classes = num_classes
         self.activation = keras.activations.get(activation)
         self.dropout = dropout
 
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "dropout": self.dropout,
                 "activation": keras.activations.serialize(self.activation),
             }
         )
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return FNetBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return FNetPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,68 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
-from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.src.models.f_net.f_net_backbone import f_net_kernel_initializer
-from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
-    FNetMaskedLMPreprocessor,
+from keras_nlp.src.models.masked_lm import MaskedLM
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
+    RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras_nlp_export("keras_nlp.models.FNetMaskedLM")
-class FNetMaskedLM(Task):
-    """An end-to-end FNet model for the masked language modeling task.
+@keras_nlp_export("keras_nlp.models.RobertaMaskedLM")
+class RobertaMaskedLM(MaskedLM):
+    """An end-to-end RoBERTa model for the masked language modeling task.
 
-    This model will train FNet on a masked language modeling task.
+    This model will train RoBERTa on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
-    `from_preset()` constructor.
+    `from_preset()` method.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case inputs can be raw string features during `fit()`, `predict()`,
     and `evaluate()`. Inputs will be tokenized and dynamically masked during
     training and evaluation. This is done by default when creating the model
     with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind.
+    warranties or conditions of any kind. The underlying model is provided by a
+    third party and subject to a separate license, available
+    [here](https://github.com/facebookresearch/fairseq).
 
     Args:
-        backbone: A `keras_nlp.models.FNetBackbone` instance.
-        preprocessor: A `keras_nlp.models.FNetMaskedLMPreprocessor` or
+        backbone: A `keras_nlp.models.RobertaBackbone` instance.
+        preprocessor: A `keras_nlp.models.RobertaMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
-    Example usage:
+    Examples:
 
     Raw string data.
     ```python
-
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
     # Pretrained language model.
-    masked_lm = keras_nlp.models.FNetMaskedLM.from_preset(
-        "f_net_base_en",
+    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
+        "roberta_base_en",
     )
     masked_lm.fit(x=features, batch_size=2)
 
     # Re-compile (e.g., with a new learning rate).
     masked_lm.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
         optimizer=keras.optimizers.Adam(5e-5),
@@ -77,76 +75,60 @@
     ```
 
     Preprocessed integer data.
     ```python
     # Create a preprocessed dataset where 0 is the mask token.
     features = {
         "token_ids": np.array([[1, 2, 0, 4, 0, 6, 7, 8]] * 2),
-        "segment_ids": np.array([[0, 0, 0, 1, 1, 1, 0, 0]] * 2),
+        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1]] * 2),
         "mask_positions": np.array([[2, 4]] * 2)
     }
     # Labels are the original masked values.
     labels = [[3, 5]] * 2
 
-    masked_lm = keras_nlp.models.FNetMaskedLM.from_preset(
-        "f_net_base_en",
+    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
+        "roberta_base_en",
         preprocessor=None,
     )
+
     masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = RobertaBackbone
+    preprocessor_cls = RobertaMaskedLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.masked_lm_head = MaskedLMHead(
             vocabulary_size=backbone.vocabulary_size,
             token_embedding=backbone.token_embedding,
             intermediate_activation="gelu",
-            kernel_initializer=f_net_kernel_initializer(),
+            kernel_initializer=roberta_kernel_initializer(),
             dtype=backbone.dtype_policy,
             name="mlm_head",
         )
 
         # === Functional Model ===
         inputs = {
             **backbone.input,
             "mask_positions": keras.Input(
                 shape=(None,), dtype="int32", name="mask_positions"
             ),
         }
         backbone_outputs = backbone(backbone.input)
         outputs = self.masked_lm_head(
-            backbone_outputs["sequence_output"], inputs["mask_positions"]
+            backbone_outputs, inputs["mask_positions"]
         )
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return FNetBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return FNetMaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_preprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
-from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.FNetPreprocessor")
 class FNetPreprocessor(Preprocessor):
     """An FNet preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -116,14 +113,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = FNetTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -172,15 +171,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return FNetTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/f_net/f_net_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.FNetTokenizer")
 class FNetTokenizer(SentencePieceTokenizer):
     """FNet tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -91,11 +88,7 @@
             self.mask_token_id = self.token_to_id(self.mask_token)
         else:
             self.cls_token_id = None
             self.sep_token_id = None
             self.pad_token_id = None
             self.mask_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_attention.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
+from keras_nlp.src.layers.modeling.rotary_embedding import RotaryEmbedding
 from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
 class CachedGemmaAttention(keras.layers.Layer):
     """A cached grouped query attention layer."""
 
     def __init__(
@@ -83,35 +84,31 @@
             dtype=self.dtype_policy,
             name="attention_output",
         )
         self.output_dense.build(
             (None, None, self.num_query_heads, self.head_dim)
         )
         self.softmax = keras.layers.Softmax(dtype="float32")
+
+        self.rope_layer = RotaryEmbedding(
+            max_wavelength=10_000.0, dtype=self.dtype_policy
+        )
+
         self.built = True
 
-    def _apply_rope(self, x, positions):
+    def _apply_rope(self, x, start_index):
         """Rope rotate q or k."""
-        # TODO: refactor to use RotaryEmbedding layer?
-        max_wavelength = 10000
-        x_shape = ops.shape(x)
-        freq_exponents = (2.0 / x_shape[-1]) * ops.cast(
-            ops.arange(x_shape[-1] // 2, dtype="float32"), self.compute_dtype
-        )
-        timescale = max_wavelength**freq_exponents
-        radians = positions[..., None] / timescale[None, None, :]
-        radians = radians[..., None, :]
-        sin, cos = ops.sin(radians), ops.cos(radians)
-        x1, x2 = ops.split(x, 2, axis=-1)
-        # Avoid `ops.concatenate` for now, to avoid a obscure bug with XLA
-        # compilation on jax. We should be able to remove this once the
-        # following PR is in all jax releases we care about:
-        # https://github.com/openxla/xla/pull/7875
-        output = ops.stack([x1 * cos - x2 * sin, x2 * cos + x1 * sin], axis=-1)
-        return ops.reshape(output, x_shape)
+        x = self.rope_layer(x, start_index=start_index)
+        # Gemma uses a different layout for positional embeddings.
+        # The transformation below ensures the embeddings are numerically
+        # equivalent to the original gemma implementation.
+        x = ops.reshape(
+            ops.stack(ops.split(x, 2, axis=-1), axis=-1), ops.shape(x)
+        )
+        return x
 
     def _compute_attention(
         self,
         q,
         k,
         v,
         attention_mask,
@@ -150,36 +147,30 @@
         self,
         x,
         attention_mask=None,
         cache=None,
         cache_update_index=0,
         training=False,
     ):
-        seq_len = ops.shape(x)[1]
-        start_index = cache_update_index
-        positions = ops.cast(
-            ops.arange(seq_len, dtype="float32"), self.compute_dtype
-        )
-        positions = positions + ops.cast(start_index, self.compute_dtype)
         query = self.query_dense(x)
-        query = self._apply_rope(query, positions)
+        query = self._apply_rope(query, cache_update_index)
 
         if cache is not None:
             key_cache = cache[:, 0, ...]
             value_cache = cache[:, 1, ...]
             key_update = self.key_dense(x)
-            key_update = self._apply_rope(key_update, positions)
+            key_update = self._apply_rope(key_update, cache_update_index)
             value_update = self.value_dense(x)
             start = [0, cache_update_index, 0, 0]
             key = ops.slice_update(key_cache, start, key_update)
             value = ops.slice_update(value_cache, start, value_update)
             cache = ops.stack((key, value), axis=1)
         else:
             key = self.key_dense(x)
-            key = self._apply_rope(key, positions)
+            key = self._apply_rope(key, cache_update_index)
             value = self.value_dense(x)
 
         attention_vec = self._compute_attention(
             query, key, value, attention_mask, training=training
         )
 
         # Wipe attn vec if there are no attended tokens.
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import config
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.gemma.gemma_decoder_block import GemmaDecoderBlock
-from keras_nlp.src.models.gemma.gemma_presets import backbone_presets
 from keras_nlp.src.models.gemma.rms_normalization import RMSNormalization
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GemmaBackbone")
 class GemmaBackbone(Backbone):
     """Gemma core network with hyperparameters.
 
     This backbone implements the base Transformer network for the Gemma model.
@@ -56,15 +53,15 @@
             in the transformer model.
         dropout: float. Dropout probability for the Transformer encoder.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
             for the models computations and weights. Note that some
             computations, such as softmax and layer normalization will always
             be done a float32 precision regardless of dtype.
 
-    Example usage:
+    Example:
     ```python
     input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
     }
 
     # Pretrained Gemma decoder.
@@ -153,14 +150,15 @@
         sequence_output = self.layer_norm(x)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=sequence_output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_query_heads = num_query_heads
@@ -184,27 +182,27 @@
                 "head_dim": self.head_dim,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
                 "dropout": self.dropout,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
     @staticmethod
-    def get_layout_map(device_mesh, model_parallel_dim_name="model"):
+    def get_layout_map(
+        device_mesh,
+        model_parallel_dim_name="model",
+        data_parallel_dim_name="batch",
+    ):
         """Get a `keras.distribution.LayoutMap` for model parallel distribution.
 
         The returned `LayoutMap` contains the sharding spec for the gemma
         backbone weights, so that you can use it to distribute weights across
         the accelerators.
 
-        Sample usage:
+        Example:
         ```
         # Feel free to change the mesh shape to balance data and model parallel
         mesh = keras.distribution.DeviceMesh(
             shape=(1, 8), axis_names=('batch', 'model'),
             devices=keras.distribution.list_devices())
         layout_map = GemmaBackbone.get_layout_map(
             mesh, model_parallel_dim_name="model")
@@ -216,14 +214,16 @@
         ```
 
         Args:
             device_mesh: The `keras.distribution.DeviceMesh` instance for
                 distribution.
             model_parallel_dim_name: The axis name of the device mesh, where
                 the weights should be partition on.
+            data_parallel_dim_name: The axis name of the device mesh, where
+                the data should be partition on.
         Return:
             `keras.distribution.LayoutMap` that contains the sharding spec
             of all the model weights.
         """
         # The weight path and shape of the Gemma backbone is like below (for 2G)
         # token_embedding/embeddings,  (256128, 2048), 524550144
         # repeat block for decoder
@@ -243,26 +243,35 @@
                 f" got {type(device_mesh)}"
             )
         if model_parallel_dim_name not in device_mesh.axis_names:
             raise ValueError(
                 f"{model_parallel_dim_name} is not found in the "
                 f"device_mesh.axis_names. {device_mesh.axis_name=}"
             )
+        if data_parallel_dim_name not in device_mesh.axis_names:
+            raise ValueError(
+                f"{data_parallel_dim_name} is not found in the "
+                f"device_mesh.axis_names. {device_mesh.axis_name=}"
+            )
+        # Note that it is possible to further config the mesh to be 3D, eg
+        # (data, seq, model). We leave it as 2D for now for simplicity.
+        data_dim = data_parallel_dim_name
         model_dim = model_parallel_dim_name
-        # The sharding is partition for the hidden_dim of the model.
+        # The sharding config is based on the Gemma team training config.
+        # See https://arxiv.org/abs/2403.08295
         layout_map = keras.distribution.LayoutMap(device_mesh)
-        layout_map["token_embedding/embeddings"] = (None, model_dim)
+        layout_map["token_embedding/embeddings"] = (model_dim, data_dim)
         layout_map["decoder_block.*attention.*(query|key|value).*kernel"] = (
-            None,
             model_dim,
+            data_dim,
             None,
         )
         layout_map["decoder_block.*attention_output.*kernel"] = (
-            None,
-            None,
             model_dim,
+            None,
+            data_dim,
         )
-        layout_map["decoder_block.*ffw_gating.*kernel"] = (model_dim, None)
-        layout_map["decoder_block.*ffw_linear.*kernel"] = (None, model_dim)
+        layout_map["decoder_block.*ffw_gating.*kernel"] = (data_dim, model_dim)
+        layout_map["decoder_block.*ffw_linear.*kernel"] = (model_dim, data_dim)
 
         return layout_map
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_causal_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_causal_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
+from keras_nlp.src.models.causal_lm import CausalLM
 from keras_nlp.src.models.gemma.gemma_backbone import GemmaBackbone
 from keras_nlp.src.models.gemma.gemma_causal_lm_preprocessor import (
     GemmaCausalLMPreprocessor,
 )
-from keras_nlp.src.models.gemma.gemma_presets import backbone_presets
-from keras_nlp.src.models.generative_task import GenerativeTask
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
 @keras_nlp_export("keras_nlp.models.GemmaCausalLM")
-class GemmaCausalLM(GenerativeTask):
+class GemmaCausalLM(CausalLM):
     """An end-to-end Gemma model for causal language modeling.
 
     A causal language model (LM) predicts the next token based on previous
     tokens. This task setup can be used to train the model unsupervised on
     plain text input, or to autoregressively generate plain text similar to
     the data used for training. This task can be used for pre-training or
     fine-tuning a Gemma model, simply by calling `fit()`.
@@ -93,14 +91,22 @@
     Call `fit()` on a single batch.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     gemma_lm = keras_nlp.models.GemmaCausalLM.from_preset("gemma_2b_en")
     gemma_lm.fit(x=features, batch_size=2)
     ```
 
+    Call `fit()` with LoRA fine-tuning enabled.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    gemma_lm = keras_nlp.models.GemmaCausalLM.from_preset("gemma_2b_en")
+    gemma.backbone.enable_lora(rank=4)
+    gemma_lm.fit(x=features, batch_size=2)
+    ```
+
     Call `fit()` without preprocessing.
     ```python
     x = {
         # Token ids for "<bos> Keras is deep learning library<eos>"
         "token_ids": np.array([[2, 214064, 603, 5271, 6044, 9581, 1, 0]] * 2),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 0]] * 2),
     }
@@ -135,14 +141,17 @@
         backbone=backbone,
         preprocessor=preprocessor,
     )
     gemma_lm.fit(x=features, batch_size=2)
     ```
     """
 
+    backbone_cls = GemmaBackbone
+    preprocessor_cls = GemmaCausalLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -155,35 +164,31 @@
         outputs = backbone.token_embedding(hidden_states, reverse=True)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            sampler="greedy",
-            jit_compile=True,
+    def compile(
+        self,
+        optimizer="auto",
+        loss="auto",
+        *,
+        weighted_metrics="auto",
+        sampler="greedy",
+        **kwargs,
+    ):
+        super().compile(
+            optimizer=optimizer,
+            loss=loss,
+            weighted_metrics=weighted_metrics,
+            sampler=sampler,
+            **kwargs,
         )
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def backbone_cls(cls):
-        return GemmaBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return GemmaCausalLMPreprocessor
-
     def call_with_cache(
         self,
         token_ids,
         cache,
         cache_update_index,
     ):
         """Forward pass of `GemmaCausalLM` with cache.
@@ -234,27 +239,27 @@
         # Seed the cache.
         _, hidden_states, cache = self.call_with_cache(token_ids, cache, 0)
         return hidden_states, cache
 
     def generate_step(
         self,
         inputs,
-        end_token_id=None,
+        stop_token_ids=None,
     ):
         """A compilable generation function for a single batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
         for a single batch of inputs. Inputs should have the same structure as
         model inputs, a dictionary with keys `"token_ids"` and `"padding_mask"`.
 
         Args:
             inputs: A dictionary with two keys `"token_ids"` and
                 `"padding_mask"` and batched tensor values.
-            end_token_id: The id of the end token to stop on. If all
-                sequences have produced a new `end_token_id`, generation
+            stop_token_ids: Tuple of id's of end token's to stop on. If all
+                sequences have produced a new stop token, generation
                 will stop.
         """
         token_ids, padding_mask = inputs["token_ids"], inputs["padding_mask"]
         # Create and seed cache with a single forward pass.
         hidden_states, cache = self._build_cache(token_ids)
         # Compute the lengths of all user inputted tokens ids.
         row_lengths = ops.sum(ops.cast(padding_mask, "int32"), axis=-1)
@@ -273,33 +278,33 @@
             )
             return (
                 ops.squeeze(logits, axis=1),
                 ops.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        token_ids = self._sampler(
+        token_ids = self.sampler(
             next=next,
             prompt=token_ids,
             cache=cache,
             index=index,
             mask=padding_mask,
-            end_token_id=end_token_id,
+            stop_token_ids=stop_token_ids,
             hidden_states=hidden_states,
             model=self,
         )
 
         # Compute an output padding mask with the token ids we updated.
-        if end_token_id is not None:
-            # Build a mask of `end_token_id` locations not in the original
+        if stop_token_ids is not None:
+            # Build a mask of `stop_token_ids` locations not in the original
             # prompt (not in locations where `padding_mask` is True).
-            end_locations = ops.logical_and(
-                ops.equal(token_ids, end_token_id),
-                ops.logical_not(padding_mask),
+            end_locations = any_equal(
+                token_ids, stop_token_ids, ops.logical_not(padding_mask)
             )
+
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
         else:
@@ -355,15 +360,15 @@
                 target_ids are not provided when using ScoringMode.LOSS.
 
         Returns:
             The per-token scores as a tensor of size
             <float>[batch_size, num_tokens, vocab_size] in "logits" mode, or
             <float>[batch_size, num_tokens] in "loss" mode.
 
-        Examples:
+        Example:
 
         Compute gradients between embeddings and loss scores with TensorFlow:
         ```python
         gemma_lm = keras_nlp.models.GemmaCausalLM.from_preset(
             "gemma_2b_en"
         )
         generations = gemma_lm.generate(
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_causal_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_causal_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     def generate_preprocess(
         self,
         x,
         sequence_length=None,
     ):
-        """Covert strings to integer token input for generation.
+        """Convert strings to integer token input for generation.
 
         Similar to calling the layer for training, this method takes in strings
         or tensor strings, tokenizes and packs the input, and computes a padding
         mask masking all inputs not filled in with a padded value.
 
         Unlike calling the layer for training, this method does not compute
         labels and will never append a `tokenizer.end_token_id` to the end of
@@ -144,19 +144,16 @@
             x, sequence_length=sequence_length, add_end_value=False
         )
         return {
             "token_ids": token_ids,
             "padding_mask": padding_mask,
         }
 
-    def generate_postprocess(
-        self,
-        x,
-    ):
-        """Covert integer token output to strings for generation.
+    def generate_postprocess(self, x):
+        """Convert integer token output to strings for generation.
 
         This method reverses `generate_preprocess()`, by first removing all
         padding and start/end tokens, and then converting the integer sequence
         back to a string.
         """
         if not self.built:
             self.build(None)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_decoder_block.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_decoder_block.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
-from keras_nlp.src.models.gemma.gemma_presets import backbone_presets
 from keras_nlp.src.models.gemma.gemma_tokenizer import GemmaTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GemmaPreprocessor")
 class GemmaPreprocessor(Preprocessor):
     """Gemma preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
@@ -120,14 +117,16 @@
 
     # Map unlabeled single sentences.
     ds = tf.data.Dataset.from_tensor_slices(text)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
+    tokenizer_cls = GemmaTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=8192,
         add_start_token=True,
         add_end_token=True,
         **kwargs,
@@ -186,15 +185,7 @@
                 "sequence_length": self.sequence_length,
                 "add_start_token": self.add_start_token,
                 "add_end_token": self.add_end_token,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def tokenizer_cls(cls):
-        return GemmaTokenizer
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/gemma_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gemma/gemma_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.gemma.gemma_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GemmaTokenizer")
 class GemmaTokenizer(SentencePieceTokenizer):
     """Gemma tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -99,11 +96,7 @@
             self.end_token_id = self.token_to_id(self.end_token)
             self.pad_token_id = self.token_to_id(self.pad_token)
         else:
             self.start_token_id = None
             self.end_token_id = None
             self.pad_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gemma/rms_normalization.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_layernorm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-# Copyright 2024 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 
 
-class RMSNormalization(keras.layers.Layer):
+# TODO: Deprecate this in favor of
+# `keras.layers.LayerNormalization(rms_scaling=True)` once Keras 2 support is
+# removed.
+class LlamaLayerNorm(keras.layers.Layer):
+    """A normalization layer for Llama that implements RMS normalization."""
+
     def __init__(self, epsilon=1e-6, **kwargs):
         super().__init__(**kwargs)
         self.epsilon = epsilon
 
     def build(self, input_shape):
+        dim = input_shape[-1]
         self.scale = self.add_weight(
             name="scale",
             trainable=True,
-            shape=(input_shape[-1],),
-            initializer="zeros",
+            shape=(dim,),
+            initializer="ones",
+            dtype=self.variable_dtype,
         )
         self.built = True
 
     def call(self, x):
-        # Always compute normalization in float32.
         x = ops.cast(x, "float32")
-        scale = ops.cast(self.scale, "float32")
-        var = ops.mean(ops.square(x), axis=-1, keepdims=True)
-        normed_inputs = x * ops.reciprocal(ops.sqrt(var + 1e-06))
-        normed_inputs = normed_inputs * (1 + scale)
-        return ops.cast(normed_inputs, self.compute_dtype)
+        var = ops.mean(ops.power(x, 2), axis=-1, keepdims=True)
+        x = x * ops.rsqrt(var + self.epsilon)
+        return ops.cast(x, self.compute_dtype) * self.scale
+
+    def get_config(self):
+        config = super().get_config()
+        config.update({"epsilon": self.epsilon})
+        return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/generative_task.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/utils/pipeline_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,268 +8,284 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import itertools
+import functools
+import math
 
 import tensorflow as tf
 import tree
 
-from keras_nlp.src.backend import config
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.samplers.serialization import get as get_sampler
-from keras_nlp.src.utils.tensor_utils import tensor_to_list
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.tensor_utils import is_tensor_type
+
+
+def _convert_inputs_to_dataset(
+    x=None,
+    y=None,
+    sample_weight=None,
+    batch_size=None,
+):
+    """Convert inputs to a `tf.data.Dataset`.
+
+    This is a stand in for the `TensorLikeDataAdapter` in core Keras.
+    """
+    if isinstance(x, tf.data.Dataset):
+        if y is not None:
+            raise ValueError(
+                "When `x` is a `tf.data.Dataset`, please do not provide "
+                f"`y`. Received: `type(y)={type(y)}`."
+            )
+        if sample_weight is not None:
+            raise ValueError(
+                "When `x` is a `tf.data.Dataset`, please do not provide "
+                "`sample_weight`. Received: "
+                f"`type(sample_weight)={type(sample_weight)}`."
+            )
+        if batch_size is not None:
+            raise ValueError(
+                "When `x` is a `tf.data.Dataset`, please do not provide "
+                "`batch_size`. Received: "
+                f"`type(batch_size)={type(batch_size)}`."
+            )
+        return x
+
+    inputs = pack_x_y_sample_weight(x, y, sample_weight)
+    try:
+
+        def convert(x):
+            if isinstance(x, (tf.Tensor, tf.RaggedTensor)):
+                return x
+            if hasattr(x, "__array__"):
+                return ops.convert_to_numpy(x)
+            return x
+
+        inputs = tree.map_structure(convert, inputs)
+        ds = tf.data.Dataset.from_tensor_slices(inputs)
+    except ValueError as e:
+        # If our inputs are unbatched, re-raise with a more friendly error
+        # message the default from tf.data. We expect this to come up with
+        # some frequency, so it's important to have a good sign post here.
+        if "only supported for rank >= 1" in str(e):
+            raise ValueError(
+                "`x`, `y`, and `sample_weight` must have a batch dimension "
+                "when calling `fit()`, `evaluate()`, and `predict()`. Received "
+                "an input with rank 0. Please add an outer dimension to your "
+                "input, e.g., wrap it in a list."
+            ) from e
+        raise e
+
+    return ds.batch(batch_size or 32)
+
+
+def _train_validation_split(arrays, validation_split):
+    """Split arrays into train and validation subsets in deterministic order.
+
+    This is copied directly from core Keras.
+    """
+
+    def _can_split(t):
+        return is_tensor_type(t) or t is None
+
+    flat_arrays = tree.flatten(arrays)
+    unsplitable = [type(t) for t in flat_arrays if not _can_split(t)]
+    if unsplitable:
+        raise ValueError(
+            "`validation_split` is only supported for Tensors or NumPy "
+            "arrays, found following types in the input: {}".format(unsplitable)
+        )
+
+    if all(t is None for t in flat_arrays):
+        return arrays, arrays
+
+    first_non_none = None
+    for t in flat_arrays:
+        if t is not None:
+            first_non_none = t
+            break
+
+    # Assumes all arrays have the same batch shape or are `None`.
+    batch_dim = int(first_non_none.shape[0])
+    split_at = int(math.floor(batch_dim * (1.0 - validation_split)))
+
+    if split_at == 0 or split_at == batch_dim:
+        raise ValueError(
+            "Training data contains {batch_dim} samples, which is not "
+            "sufficient to split it into a validation and training set as "
+            "specified by `validation_split={validation_split}`. Either "
+            "provide more data, or a different value for the "
+            "`validation_split` argument.".format(
+                batch_dim=batch_dim, validation_split=validation_split
+            )
+        )
+
+    def _split(t, start, end):
+        if t is None:
+            return t
+        return t[start:end]
+
+    train_arrays = tree.map_structure(
+        functools.partial(_split, start=0, end=split_at), arrays
+    )
+    val_arrays = tree.map_structure(
+        functools.partial(_split, start=split_at, end=batch_dim), arrays
+    )
+
+    return train_arrays, val_arrays
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
-class GenerativeTask(Task):
-    """Base class for Generative Task models."""
+class PipelineModel(keras.Model):
+    """A model which allows automatically applying preprocessing."""
 
-    def compile(
+    def __init__(self, *args, **kwargs):
+        # Workaround for https://github.com/keras-team/keras/issues/17270
+        # Reset any attempt to overwrite this classes base class to this class
+        # can continue to be used for functional and non-functional models.
+        PipelineModel.__bases__ = (keras.Model,)
+        super().__init__(*args, **kwargs)
+
+    def preprocess_samples(self, x, y=None, sample_weight=None):
+        """An overridable function which preprocesses entire samples."""
+        return pack_x_y_sample_weight(x, y, sample_weight)
+
+    # ========================================================================
+    # Below are overrides to keras.Model methods to apply the functions above.
+    # ========================================================================
+    def fit(
         self,
-        *args,
-        run_eagerly=False,
-        jit_compile=True,
-        sampler="top_k",
+        x=None,
+        y=None,
+        batch_size=None,
+        sample_weight=None,
+        validation_data=None,
+        validation_split=None,
         **kwargs,
     ):
-        xla_compatible = True
-        super().compile(
-            *args,
-            run_eagerly=run_eagerly,
-            # Only `jit_compile` if not eager and in a compatible environment.
-            jit_compile=jit_compile and xla_compatible and not run_eagerly,
-            **kwargs,
-        )
-        self._sampler = get_sampler(sampler)
-        # Clear the compiled generate function.
-        self.generate_function = None
-
-    def generate_step(self):
-        """Run generation on a single batch of input."""
-        raise NotImplementedError
-
-    def make_generate_function(self):
-        """Create or return the compiled generation function."""
-        if self.generate_function is not None:
-            return self.generate_function
-
-        self.generate_function = self.generate_step
-        if config.backend() == "torch":
-            import torch
-
-            def wrapped_generate_function(
-                inputs,
-                end_token_id=None,
-            ):
-                with torch.no_grad():
-                    return self.generate_step(inputs, end_token_id)
-
-            self.generate_function = wrapped_generate_function
-        elif config.backend() == "tensorflow" and not self.run_eagerly:
-            # `jit_compile` is a property of keras.Model after TF 2.12.
-            # Use `getattr()` for backwards compatibility.
-            jit_compile = getattr(self, "jit_compile", True)
-            self.generate_function = tf.function(
-                self.generate_step, jit_compile=jit_compile
+        if validation_split and validation_data is None:
+            (x, y, sample_weight), validation_data = _train_validation_split(
+                (x, y, sample_weight), validation_split=validation_split
             )
-        elif config.backend() == "jax" and not self.run_eagerly:
-            import jax
 
-            @jax.jit
-            def compiled_generate_function(inputs, end_token_id, state):
-                (
-                    sampler_variables,
-                    trainable_variables,
-                    non_trainable_variables,
-                ) = state
-                mapping = itertools.chain(
-                    zip(self._sampler.variables, sampler_variables),
-                    zip(self.trainable_variables, trainable_variables),
-                    zip(self.non_trainable_variables, non_trainable_variables),
+        x = _convert_inputs_to_dataset(x, y, sample_weight, batch_size)
+        x = x.map(
+            self.preprocess_samples, num_parallel_calls=tf.data.AUTOTUNE
+        ).prefetch(tf.data.AUTOTUNE)
+
+        if validation_data is not None:
+            if not isinstance(validation_data, tf.data.Dataset):
+                (vx, vy, vsw) = keras.utils.unpack_x_y_sample_weight(
+                    validation_data
                 )
-
-                with keras.StatelessScope(state_mapping=mapping) as scope:
-                    outputs = self.generate_step(inputs, end_token_id)
-
-                # Get updated sampler variables from the stateless scope.
-                sampler_variables = []
-                for v in self._sampler.variables:
-                    new_v = scope.get_current_value(v)
-                    sampler_variables.append(new_v if new_v is not None else v)
-                return outputs, sampler_variables
-
-            def wrapped_generate_function(
-                inputs,
-                end_token_id=None,
-            ):
-                # Create an explicit tuple of all variable state.
-                state = (
-                    self._sampler.variables,
-                    # Use the explicit variable.value to preserve the
-                    # sharding spec of distribution.
-                    [v.value for v in self.trainable_variables],
-                    [v.value for v in self.non_trainable_variables],
-                )
-                inputs = tree.map_structure(ops.convert_to_tensor, inputs)
-                outputs, sampler_variables = compiled_generate_function(
-                    inputs,
-                    end_token_id,
-                    state,
+                validation_data = _convert_inputs_to_dataset(
+                    vx, vy, vsw, batch_size
                 )
-                # Only assign the sampler variables (random seeds), as other
-                # model variables should never be updated in generation.
-                for ref_v, v in zip(self._sampler.variables, sampler_variables):
-                    ref_v.assign(v)
-                return outputs
-
-            self.generate_function = wrapped_generate_function
 
-        return self.generate_function
+        return super().fit(
+            x=x,
+            y=None,
+            batch_size=None,
+            sample_weight=None,
+            validation_data=validation_data,
+            **kwargs,
+        )
 
-    def _normalize_generate_inputs(
+    def evaluate(
         self,
-        inputs,
+        x=None,
+        y=None,
+        batch_size=None,
+        sample_weight=None,
+        **kwargs,
     ):
-        """Normalize user input to the generate function.
-
-        This function coverts all inputs to tensors, adds a batch dimension if
-        necessary, and returns a iterable "dataset like" object (either an
-        actual `tf.data.Dataset` or a list with a single batch element).
-        """
-        input_is_scalar = False
-
-        if isinstance(inputs, tf.data.Dataset):
-            return inputs, input_is_scalar
-
-        def normalize(x):
-            x_is_scalar = False
-            if isinstance(x, str) or isinstance(x, list):
-                x = tf.convert_to_tensor(x)
-
-            if isinstance(x, tf.Tensor) and x.shape.rank == 0:
-                x_is_scalar = True
-                x = x[tf.newaxis]
-
-            return x, x_is_scalar
-
-        if isinstance(inputs, dict):
-            for key in inputs:
-                inputs[key], input_is_scalar = normalize(inputs[key])
-        else:
-            inputs, input_is_scalar = normalize(inputs)
-
-        # We avoid converting to a dataset purely for speed, for a single batch
-        # of input, creating a dataset would add significant overhead.
-        return [inputs], input_is_scalar
+        # During `fit()`, `keras.Model` attempts to cache the validation
+        # dataset and ignores the values for `x`, `y`, and `sample_weight`.
+        # We don't want that behavior here, as the validation dataset still
+        # needs preprocessing.
+        kwargs.pop("_use_cached_eval_dataset", None)
+        x = _convert_inputs_to_dataset(x, y, sample_weight, batch_size)
+        x = x.map(
+            self.preprocess_samples, num_parallel_calls=tf.data.AUTOTUNE
+        ).prefetch(tf.data.AUTOTUNE)
+        return super().evaluate(
+            x=x,
+            y=None,
+            batch_size=None,
+            **kwargs,
+        )
 
-    def _normalize_generate_outputs(
+    def predict(
         self,
-        outputs,
-        input_is_scalar,
+        x=None,
+        batch_size=None,
+        **kwargs,
     ):
-        """Normalize user output from the generate function.
-
-        This function converts all output to numpy (for integer output), or
-        python strings (for string output). If a batch dimension was added to
-        the input, it is removed from the output (so generate can be string in,
-        string out).
-        """
-
-        def normalize(x):
-            if isinstance(x[0], list):
-                outputs = []
-                for batch in x:
-                    for e in batch:
-                        outputs.append(e)
-                return outputs[0] if input_is_scalar else outputs
-            if isinstance(x[0], tf.Tensor) and x[0].dtype == tf.string:
-                outputs = tf.concat(x, axis=0)
-                outputs = tf.squeeze(outputs, 0) if input_is_scalar else outputs
-                return tensor_to_list(outputs)
-            outputs = ops.concatenate(x, axis=0)
-            outputs = ops.squeeze(outputs, 0) if input_is_scalar else outputs
-            return ops.convert_to_numpy(outputs)
-
-        if isinstance(outputs[0], dict):
-            normalized = {}
-            for key in outputs[0]:
-                normalized[key] = normalize([x[key] for x in outputs])
-            return normalized
-        return normalize([x for x in outputs])
+        x = _convert_inputs_to_dataset(x, None, None, batch_size)
+        x = x.map(
+            self.preprocess_samples, num_parallel_calls=tf.data.AUTOTUNE
+        ).prefetch(tf.data.AUTOTUNE)
+        return super().predict(
+            x=x,
+            batch_size=None,
+            **kwargs,
+        )
 
-    def generate(
+    def train_on_batch(
         self,
-        inputs,
-        max_length=None,
+        x,
+        y=None,
+        sample_weight=None,
+        **kwargs,
     ):
-        """Generate text given prompt `inputs`.
-
-        This method generates text based on given `inputs`. The sampling method
-        used for generation can be set via the `compile()` method.
-
-        If `inputs` are a `tf.data.Dataset`, outputs will be generated
-        "batch-by-batch" and concatenated. Otherwise, all inputs will be handled
-        as a single batch.
-
-        If a `preprocessor` is attached to the model, `inputs` will be
-        preprocessed inside the `generate()` function and should match the
-        structure expected by the `preprocessor` layer (usually raw strings).
-        If a `preprocessor` is not attached, inputs should match the structure
-        expected by the `backbone`. See the example usage above for a
-        demonstration of each.
-
-        Args:
-            inputs: python data, tensor data, or a `tf.data.Dataset`. If a
-                `preprocessor` is attached to the model, `inputs` should match
-                the structure expected by the `preprocessor` layer. If a
-                `preprocessor` is not attached, `inputs` should match the
-                structure expected the `backbone` model.
-            max_length: Optional. int. The max length of the generated sequence.
-                Will default to the max configured `sequence_length` of the
-                `preprocessor`. If `preprocessor` is `None`, `inputs` should be
-                should be padded to the desired maximum length and this argument
-                will be ignored.
-        """
-        # Setup our three main passes.
-        # 1. Optionally preprocessing strings to dense integer tensors.
-        # 2. Generate new tokens via a compiled function on dense tensors.
-        # 3. Optionally postprocess dense integer tensors back to string.
-        generate_function = self.make_generate_function()
-        end_token_id = None
-        if self.preprocessor is not None:
-            end_token_id = self.preprocessor.tokenizer.end_token_id
-
-        def preprocess(x):
-            return self.preprocessor.generate_preprocess(
-                x, sequence_length=max_length
-            )
-
-        def generate(x):
-            return generate_function(x, end_token_id=end_token_id)
-
-        def postprocess(x):
-            return self.preprocessor.generate_postprocess(x)
-
-        # Normalize inputs, apply our three passes, and normalize outputs.
-        inputs, input_is_scalar = self._normalize_generate_inputs(inputs)
-
-        if self.preprocessor is not None:
-            if isinstance(inputs, tf.data.Dataset):
-                inputs = inputs.map(preprocess, tf.data.AUTOTUNE)
-                inputs = inputs.prefetch(tf.data.AUTOTUNE)
-            else:
-                # Fast path for non-dataset, single-batch input.
-                inputs = [preprocess(x) for x in inputs]
-
-        outputs = [generate(x) for x in inputs]
+        data = self.preprocess_samples(x, y, sample_weight)
+        x, y, sample_weight = keras.utils.unpack_x_y_sample_weight(data)
+        x = ops.convert_to_tensor(x)
+        if y is not None:
+            y = ops.convert_to_tensor(y)
+        if sample_weight is not None:
+            sample_weight = ops.convert_to_tensor(sample_weight)
+        return super().train_on_batch(
+            x=x,
+            y=y,
+            sample_weight=sample_weight,
+            **kwargs,
+        )
 
-        if self.preprocessor is not None:
-            outputs = [postprocess(x) for x in outputs]
+    def test_on_batch(
+        self,
+        x,
+        y=None,
+        sample_weight=None,
+        **kwargs,
+    ):
+        data = self.preprocess_samples(x, y, sample_weight)
+        x, y, sample_weight = keras.utils.unpack_x_y_sample_weight(data)
+        x = ops.convert_to_tensor(x)
+        if y is not None:
+            y = ops.convert_to_tensor(y)
+        if sample_weight is not None:
+            sample_weight = ops.convert_to_tensor(sample_weight)
+        return super().test_on_batch(
+            x=x,
+            y=y,
+            sample_weight=sample_weight,
+            **kwargs,
+        )
 
-        return self._normalize_generate_outputs(outputs, input_is_scalar)
+    def predict_on_batch(
+        self,
+        x,
+        **kwargs,
+    ):
+        data = self.preprocess_samples(x)
+        x, _, _ = keras.utils.unpack_x_y_sample_weight(data)
+        x = ops.convert_to_tensor(x)
+        return super().predict_on_batch(
+            x=x,
+            **kwargs,
+        )
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_backbone.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,203 +1,169 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
-from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
+from keras_nlp.src.layers.modeling.token_and_position_embedding import (
+    TokenAndPositionEmbedding,
+)
 from keras_nlp.src.layers.modeling.transformer_decoder import TransformerDecoder
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.src.utils.keras_utils import gelu_approximate
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-def _gpt_2_kernel_initializer(stddev=0.02):
-    return keras.initializers.RandomNormal(stddev=stddev)
+def opt_kernel_initializer(stddev=0.02):
+    return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras_nlp_export("keras_nlp.models.GPT2Backbone")
-class GPT2Backbone(Backbone):
-    """GPT-2 core network with hyperparameters.
-
-    This network implements a Transformer-based decoder network,
-    Generative Pretrained Transformer-2 (GPT-2), as described in
-    ["Language Models are Unsupervised Multitask Learners"](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf).
-    It includes the embedding lookups and transformer layers.
-
-    The default constructor gives a fully customizable, randomly initialized
-    GPT-2 model with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset`
-    constructor.
+@keras_nlp_export("keras_nlp.models.OPTBackbone")
+class OPTBackbone(Backbone):
+    """An OPT decoder network.
+
+    This class implements a Transformer-based decoder model as described in
+    ["OPT: Open Pre-trained Transformer Language Models"](https://arxiv.org/abs/2205.01068).
+    The default constructor gives a fully customizable, randomly initialized OPT
+    model with any number of layers, heads, and embedding dimensions. To load
+    preset architectures and weights, use the `from_preset()` constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
-    [here](https://github.com/openai/gpt-2).
+    [here](https://github.com/facebookresearch/fairseq/).
 
     Args:
         vocabulary_size: int. The size of the token vocabulary.
-        num_layers: int. The number of transformer layers.
+        num_layers: int. The number of transformer decoder layers.
         num_heads: int. The number of attention heads for each transformer.
             The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The size of the transformer encoding and pooler layers.
+        hidden_dim: int. The hidden size of the transformer decoder layers.
         intermediate_dim: int. The output dimension of the first Dense layer in
-            a two-layer feedforward network for each transformer.
-        dropout: float. Dropout probability for the Transformer encoder.
-        max_sequence_length: int. The maximum sequence length that this encoder
+            a two-layer feedforward network for each transformer decoder layer.
+        dropout: float. Dropout probability for the Transformer decoder.
+        max_sequence_length: int. The maximum sequence length that this decoder
             can consume. If `None`, `max_sequence_length` uses the value from
             sequence length. This determines the variable shape for positional
             embeddings.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
-            for the models computations and weights. Note that some
-            computations, such as softmax and layer normalization will always
-            be done a float32 precision regardless of dtype.
+            for model computations and weights. Note that some computations,
+            such as softmax and layer normalization, will always be done at
+            float32 precision regardless of dtype.
 
-    Example:
+    Examples:
     ```python
     input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
     }
 
-    # Pretrained GPT-2 decoder.
-    model = keras_nlp.models.GPT2Backbone.from_preset("gpt2_base_en")
+    # Pretrained OPT decoder
+    model = keras_nlp.models.OPTBackbone.from_preset("opt_125m_en")
     model(input_data)
 
-    # Randomly initialized GPT-2 decoder with custom config.
-    model = keras_nlp.models.GPT2Backbone(
-        vocabulary_size=50257,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=1024,
+    # Randomly initialized OPT decoder model with a custom config
+    model = keras_nlp.models.OPTBackbone(
+        vocabulary_size=50265,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
     model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
         num_heads,
         hidden_dim,
         intermediate_dim,
         dropout=0.1,
-        max_sequence_length=1024,
+        max_sequence_length=2048,
         dtype=None,
         **kwargs,
     ):
         # === Layers ===
-        self.token_embedding = ReversibleEmbedding(
-            input_dim=vocabulary_size,
-            output_dim=hidden_dim,
-            embeddings_initializer=_gpt_2_kernel_initializer(stddev=0.01),
-            dtype=dtype,
-            name="token_embedding",
-        )
-        self.position_embedding = PositionEmbedding(
-            initializer=_gpt_2_kernel_initializer(stddev=0.02),
+        self.embeddings = TokenAndPositionEmbedding(
+            vocabulary_size=vocabulary_size,
             sequence_length=max_sequence_length,
+            embedding_dim=hidden_dim,
+            embeddings_initializer=opt_kernel_initializer(),
             dtype=dtype,
-            name="position_embedding",
-        )
-        self.embeddings_add = keras.layers.Add(
-            dtype=dtype,
-            name="embeddings_add",
-        )
-        self.embeddings_dropout = keras.layers.Dropout(
-            dropout,
-            dtype=dtype,
-            name="embeddings_dropout",
+            name="embeddings",
         )
+        self.token_embedding = self.embeddings.token_embedding
         self.transformer_layers = []
         for i in range(num_layers):
-            self.transformer_layers.append(
-                TransformerDecoder(
-                    intermediate_dim=intermediate_dim,
-                    num_heads=num_heads,
-                    dropout=dropout,
-                    layer_norm_epsilon=1e-05,
-                    activation=gelu_approximate,
-                    kernel_initializer=_gpt_2_kernel_initializer(stddev=0.02),
-                    normalize_first=True,
-                    dtype=dtype,
-                    name=f"transformer_layer_{i}",
-                )
+            layer = TransformerDecoder(
+                intermediate_dim=intermediate_dim,
+                num_heads=num_heads,
+                dropout=dropout,
+                activation="relu",
+                layer_norm_epsilon=1e-5,
+                normalize_first=True,
+                kernel_initializer=opt_kernel_initializer(),
+                dtype=dtype,
+                name=f"transformer_layer_{i}",
             )
+            self.transformer_layers.append(layer)
         self.layer_norm = keras.layers.LayerNormalization(
             axis=-1,
-            epsilon=1e-05,
+            epsilon=1e-5,
             dtype=dtype,
             name="layer_norm",
         )
 
         # === Functional Model ===
         token_id_input = keras.Input(
             shape=(None,), dtype="int32", name="token_ids"
         )
         padding_mask_input = keras.Input(
             shape=(None,), dtype="int32", name="padding_mask"
         )
-        # Embed inputs.
-        tokens = self.token_embedding(token_id_input)
-        positions = self.position_embedding(tokens)
-        x = self.embeddings_add((tokens, positions))
-        x = self.embeddings_dropout(x)
-        # Apply transformer layers.
+        x = self.embeddings(token_id_input)
         for transformer_layer in self.transformer_layers:
             x = transformer_layer(x, decoder_padding_mask=padding_mask_input)
-        sequence_output = self.layer_norm(x)
-        # Instantiate using the Functional constructor.
+        x = self.layer_norm(x)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
-            outputs=sequence_output,
+            outputs=x,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
         self.max_sequence_length = max_sequence_length
 
     def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "vocabulary_size": self.vocabulary_size,
-                "num_layers": self.num_layers,
-                "num_heads": self.num_heads,
-                "hidden_dim": self.hidden_dim,
-                "intermediate_dim": self.intermediate_dim,
-                "dropout": self.dropout,
-                "max_sequence_length": self.max_sequence_length,
-            }
-        )
-        return config
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+        return {
+            "vocabulary_size": self.vocabulary_size,
+            "num_layers": self.num_layers,
+            "num_heads": self.num_heads,
+            "hidden_dim": self.hidden_dim,
+            "intermediate_dim": self.intermediate_dim,
+            "dropout": self.dropout,
+            "max_sequence_length": self.max_sequence_length,
+        }
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_causal_lm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,155 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2024 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
-from keras_nlp.src.models.generative_task import GenerativeTask
-from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
-from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import (
-    GPT2CausalLMPreprocessor,
+from keras_nlp.src.models.bloom.bloom_backbone import BloomBackbone
+from keras_nlp.src.models.bloom.bloom_causal_lm_preprocessor import (
+    BloomCausalLMPreprocessor,
 )
-from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.causal_lm import CausalLM
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
-@keras_nlp_export("keras_nlp.models.GPT2CausalLM")
-class GPT2CausalLM(GenerativeTask):
-    """An end-to-end GPT2 model for causal language modeling.
+@keras_nlp_export("keras_nlp.models.BloomCausalLM")
+class BloomCausalLM(CausalLM):
+    """An end-to-end BLOOM model for causal language modeling.
 
     A causal language model (LM) predicts the next token based on previous
     tokens. This task setup can be used to train the model unsupervised on
     plain text input, or to autoregressively generate plain text similar to
     the data used for training. This task can be used for pre-training or
-    fine-tuning a GPT-2 model, simply by calling `fit()`.
+    fine-tuning a BLOOM model, simply by calling `fit()`.
 
     This model has a `generate()` method, which generates text based on a
     prompt. The generation strategy used is controlled by an additional
     `sampler` argument on `compile()`. You can recompile the model with
     different `keras_nlp.samplers` objects to control the generation. By
-    default, `"top_k"` sampling will be used.
+    default, `"greedy"` sampling will be used.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to string inputs during
     `fit()`, `predict()`, `evaluate()` and `generate()`. This is done by default
     when creating the model with `from_preset()`.
 
-    Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available
-    [here](https://github.com/openai/gpt-2).
-
     Args:
-        backbone: A `keras_nlp.models.GPT2Backbone` instance.
-        preprocessor: A `keras_nlp.models.GPT2CausalLMPreprocessor` or `None`.
+        backbone: A `keras_nlp.models.BloomBackbone` instance.
+        preprocessor: A `keras_nlp.models.BloomCausalLMPreprocessor` or `None`.
             If `None`, this model will not apply preprocessing, and inputs
             should be preprocessed before calling the model.
 
     Examples:
 
     Use `generate()` to do text generation.
     ```python
-    gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
-    gpt2_lm.generate("I want to say", max_length=30)
+    bloom_lm = keras_nlp.models.BloomCausalLM.from_preset("bloom_560m_multi")
+    bloom_lm.generate("I want to say", max_length=30)
 
     # Generate with batched prompts.
-    gpt2_lm.generate(["This is a", "Where are you"], max_length=30)
+    bloom_lm.generate(["This is a", "Where are you"], max_length=30)
     ```
 
     Compile the `generate()` function with a custom sampler.
     ```python
-    gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
-    gpt2_lm.compile(sampler="greedy")
-    gpt2_lm.generate("I want to say", max_length=30)
+    bloom_lm = keras_nlp.models.BloomCausalLM.from_preset("bloom_560m_multi")
+    bloom_lm.compile(sampler="top_k")
+    bloom_lm.generate("I want to say", max_length=30)
 
-    gpt2_lm.compile(sampler=keras_nlp.samplers.BeamSampler(num_beams=2))
-    gpt2_lm.generate("I want to say", max_length=30)
+    bloom_lm.compile(sampler=keras_nlp.samplers.BeamSampler(num_beams=2))
+    bloom_lm.generate("I want to say", max_length=30)
     ```
 
     Use `generate()` without preprocessing.
     ```python
-    # Prompt the model with `5338, 318` (the token ids for `"Who is"`).
-    # Use `"padding_mask"` to indicate values that should not be overridden.
     prompt = {
-        "token_ids": np.array([[5338, 318, 0, 0, 0]] * 2),
-        "padding_mask": np.array([[1, 1, 0, 0, 0]] * 2),
+        # Token ids for "<s> Keras is".
+        "token_ids": np.array([[1, 46, 15762, 632, 3, 3, 3, 3, 3]] * 2),
+        # Use `"padding_mask"` to indicate values that should not be overridden.
+        "padding_mask": np.array([[1, 1, 1, 1, 0, 0, 0, 0, 0]] * 2),
     }
 
-    gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset(
-        "gpt2_base_en",
+    bloom_lm = keras_nlp.models.BloomCausalLM.from_preset(
+        "bloom_560m_multi",
         preprocessor=None,
     )
-    gpt2_lm.generate(prompt)
+    bloom_lm.generate(prompt)
     ```
 
     Call `fit()` on a single batch.
     ```python
     features = ["The quick brown fox jumped.", "I forgot my homework."]
-    gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
-    gpt2_lm.fit(x=features, batch_size=2)
+    bloom_lm = keras_nlp.models.BloomCausalLM.from_preset("bloom_560m_multi")
+    bloom_lm.fit(x=features, batch_size=2)
     ```
 
     Call `fit()` without preprocessing.
     ```python
     x = {
-        "token_ids": np.array([[50256, 1, 2, 3, 4]] * 2),
-        "padding_mask": np.array([[1, 1, 1, 1, 1]] * 2),
+        # Token ids for "<bos> Keras is deep learning library<eos>"
+        "token_ids": np.array([[2, 214064, 603, 5271, 6044, 9581, 1, 0]] * 2),
+        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 0]] * 2),
     }
-    y = np.array([[1, 2, 3, 4, 50256]] * 2)
-    sw = np.array([[1, 1, 1, 1, 1]] * 2)
+    y = np.array([[214064, 603, 5271, 6044, 9581, 3, 0, 0]] * 2)
+    sw = np.array([[1, 1, 1, 1, 1, 1, 0, 0]] * 2)
 
-    gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset(
-        "gpt2_base_en",
+    bloom_lm = keras_nlp.models.BloomCausalLM.from_preset(
+        "bloom_560m_multi",
         preprocessor=None,
     )
-    gpt2_lm.fit(x=x, y=y, sample_weight=sw, batch_size=2)
+    bloom_lm.fit(x=x, y=y, sample_weight=sw, batch_size=2)
     ```
 
     Custom backbone and vocabulary.
     ```python
-    features = ["a quick fox.", "a fox quick."]
-    vocab = {"<|endoftext|>": 0, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    merges += ["Ġ f", "o x", "Ġf ox"]
-
-    tokenizer = keras_nlp.models.GPT2Tokenizer(
-        vocabulary=vocab,
-        merges=merges,
-    )
-    preprocessor = keras_nlp.models.GPT2CausalLMPreprocessor(
+    features = [
+        " airplane at airport",
+        " airplane airport",
+    ]
+    vocab = ["<unk>", "<s>", "</s>", "<pad>"]
+    vocab += ["!", "air", "Ġair", "plane", "Ġat", "port"]
+    vocab = dict([(token, i) for i, token in enumerate(vocab)])
+    merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+    merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
+    merges += ["Ġai r", "Ġa i", "pla ne"]
+    tokenizer = keras_nlp.models.BloomTokenizer(vocabulary=vocab, merges=merges)
+    preprocessor = keras_nlp.models.BloomCausalLMPreprocessor(
         tokenizer=tokenizer,
         sequence_length=128,
     )
-    backbone = keras_nlp.models.GPT2Backbone(
-        vocabulary_size=30552,
+    backbone = keras_nlp.models.BloomBackbone(
+        vocabulary_size=tokenizer.vocabulary_size(),
         num_layers=4,
         num_heads=4,
-        hidden_dim=256,
-        intermediate_dim=512,
-        max_sequence_length=128,
+        hidden_dim=32,
+        intermediate_dim=128,
     )
-    gpt2_lm = keras_nlp.models.GPT2CausalLM(
+    bloom_lm = keras_nlp.models.BloomCausalLM(
         backbone=backbone,
         preprocessor=preprocessor,
     )
-    gpt2_lm.fit(x=features, batch_size=2)
+    bloom_lm.fit(x=features, batch_size=2)
     ```
     """
 
+    backbone_cls = BloomBackbone
+    preprocessor_cls = BloomCausalLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -165,109 +162,85 @@
         outputs = backbone.token_embedding(hidden_states, reverse=True)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def backbone_cls(cls):
-        return GPT2Backbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return GPT2CausalLMPreprocessor
-
     def call_with_cache(
         self,
         token_ids,
         cache,
         cache_update_index,
     ):
-        """Forward pass of `GPT2CausalLM` with cache.
+        """Forward pass of `BloomCausalLM` with cache.
 
         `call_with_cache` adds an additional forward pass for the model for
         autoregressive inference. Unlike calling the model directly, this method
         allows caching previous key/value Tensors in multi-head attention layer,
         and avoids recomputing the outputs of seen tokens.
 
         Args:
             token_ids: a dense int Tensor with shape `(batch_size, max_length)`.
             cache: a dense float Tensor, the cache of key and value.
-            cache_update_index: int, or int Tensor. The index of current inputs in the
-                whole sequence.
+            cache_update_index: int, or int Tensor. The index of current inputs
+                in the whole sequence.
 
         Returns:
             A (logits, hidden_states, cache) tuple. Where `logits` is the
             language model logits for the input token_ids, `hidden_states` is
             the final hidden representation of the input tokens, and `cache` is
             the decoding cache.
         """
-        tokens = self.backbone.token_embedding(token_ids)
-        positions = self.backbone.position_embedding(
-            tokens, start_index=cache_update_index
-        )
-        x = self.backbone.embeddings_add((tokens, positions))
-        x = self.backbone.embeddings_dropout(x)
+        x = self.backbone.token_embedding(token_ids)
+        x = self.backbone.embeddings_layer_norm(x)
         # Each decoder layer has a cache; we update them separately.
         caches = []
         for i, transformer_layer in enumerate(self.backbone.transformer_layers):
             current_cache = cache[:, i, ...]
             x, next_cache = transformer_layer(
                 x,
-                self_attention_cache=current_cache,
-                self_attention_cache_update_index=cache_update_index,
+                cache=current_cache,
+                cache_update_index=cache_update_index,
             )
             caches.append(next_cache)
         cache = ops.stack(caches, axis=1)
         hidden_states = x = self.backbone.layer_norm(x)
         logits = self.backbone.token_embedding(x, reverse=True)
         return logits, hidden_states, cache
 
     def _build_cache(self, token_ids):
         """Build an empty cache for use with `call_with_cache()`."""
         batch_size = ops.shape(token_ids)[0]
         max_length = ops.shape(token_ids)[1]
         num_layers = self.backbone.num_layers
         num_heads = self.backbone.num_heads
-        head_dim = self.backbone.hidden_dim // self.backbone.num_heads
+        head_dim = self.backbone.hidden_dim // num_heads
         shape = [batch_size, num_layers, 2, max_length, num_heads, head_dim]
         cache = ops.zeros(shape, dtype=self.compute_dtype)
         # Seed the cache.
         _, hidden_states, cache = self.call_with_cache(token_ids, cache, 0)
         return hidden_states, cache
 
     def generate_step(
         self,
         inputs,
-        end_token_id=None,
+        stop_token_ids=None,
     ):
         """A compilable generation function for a single batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
         for a single batch of inputs. Inputs should have the same structure as
         model inputs, a dictionary with keys `"token_ids"` and `"padding_mask"`.
 
         Args:
             inputs: A dictionary with two keys `"token_ids"` and
                 `"padding_mask"` and batched tensor values.
-            end_token_id: The id of the end token to stop on. If all
-                sequences have produced a new `end_token_id`, generation
+            stop_token_ids: Tuple of id's of end token's to stop on. If all
+                sequences have produced a new stop token, generation
                 will stop.
         """
         token_ids, padding_mask = inputs["token_ids"], inputs["padding_mask"]
         # Create and seed cache with a single forward pass.
         hidden_states, cache = self._build_cache(token_ids)
         # Compute the lengths of all user inputted tokens ids.
         row_lengths = ops.sum(ops.cast(padding_mask, "int32"), axis=-1)
@@ -286,33 +259,33 @@
             )
             return (
                 ops.squeeze(logits, axis=1),
                 ops.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        token_ids = self._sampler(
+        token_ids = self.sampler(
             next=next,
             prompt=token_ids,
             cache=cache,
             index=index,
             mask=padding_mask,
-            end_token_id=end_token_id,
+            stop_token_ids=stop_token_ids,
             hidden_states=hidden_states,
             model=self,
         )
 
         # Compute an output padding mask with the token ids we updated.
-        if end_token_id is not None:
-            # Build a mask of `end_token_id` locations not in the original
+        if stop_token_ids is not None:
+            # Build a mask of stop token locations not in the original
             # prompt (not in locations where `padding_mask` is True).
-            end_locations = ops.logical_and(
-                ops.equal(token_ids, end_token_id),
-                ops.logical_not(padding_mask),
+            end_locations = any_equal(
+                token_ids, stop_token_ids, ops.logical_not(padding_mask)
             )
+
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
         else:
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     def generate_preprocess(
         self,
         x,
         sequence_length=None,
     ):
-        """Covert strings to integer token input for generation.
+        """Convert strings to integer token input for generation.
 
         Similar to calling the layer for training, this method takes in strings
         or tensor strings, tokenizes and packs the input, and computes a padding
         mask masking all inputs not filled in with a padded value.
 
         Unlike calling the layer for training, this method does not compute
         labels and will never append a `tokenizer.end_token_id` to the end of
@@ -155,15 +155,15 @@
             "padding_mask": padding_mask,
         }
 
     def generate_postprocess(
         self,
         x,
     ):
-        """Covert integer token output to strings for generation.
+        """Convert integer token output to strings for generation.
 
         This method reverses `generate_preprocess()`, by first removing all
         padding and start/end tokens, and then converting the integer sequence
         back to a string.
         """
         if not self.built:
             self.build(None)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
-from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
 from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GPT2Preprocessor")
 class GPT2Preprocessor(Preprocessor):
     """GPT2 preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
@@ -105,14 +102,16 @@
 
     # Map unlabeled single sentences.
     ds = tf.data.Dataset.from_tensor_slices(text)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
+    tokenizer_cls = GPT2Tokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=1024,
         add_start_token=True,
         add_end_token=True,
         **kwargs,
@@ -182,15 +181,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def tokenizer_cls(cls):
-        return GPT2Tokenizer
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt2/gpt2_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GPT2Tokenizer")
 class GPT2Tokenizer(BytePairTokenizer):
     """A GPT-2 tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -100,18 +97,14 @@
             self.start_token_id = self.end_token_id
             self.pad_token_id = 0
         else:
             self.end_token_id = None
             self.start_token_id = None
             self.pad_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         sequence_output = self.layer_norm(x)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=sequence_output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
-from keras_nlp.src.models.generative_task import GenerativeTask
+from keras_nlp.src.models.causal_lm import CausalLM
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_backbone import GPTNeoXBackbone
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_causal_lm_preprocessor import (
     GPTNeoXCausalLMPreprocessor,
 )
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
-class GPTNeoXCausalLM(GenerativeTask):
+class GPTNeoXCausalLM(CausalLM):
     """An end-to-end GPTNeoX model for causal language modeling.
 
     A causal language model (LM) predicts the next token based on previous
     tokens. This task setup can be used to train the model unsupervised on
     plain text input, or to autoregressively generate plain text similar to
     the data used for training. This task can be used for pre-training or
     fine-tuning a GPT-NeoX model, simply by calling `fit()`.
@@ -41,14 +41,17 @@
     Args:
         backbone: A `keras_nlp.models.GPTNeoXBackbone` instance.
         preprocessor: A `keras_nlp.models.GPTNeoXCausalLMPreprocessor` or `None`.
             If `None`, this model will not apply preprocessing, and inputs
             should be preprocessed before calling the model.
     """
 
+    backbone_cls = GPTNeoXBackbone
+    preprocessor_cls = GPTNeoXCausalLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -61,30 +64,14 @@
         outputs = backbone.token_embedding(hidden_states, reverse=True)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return GPTNeoXBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return GPTNeoXCausalLMPreprocessor
-
     def call_with_cache(
         self,
         token_ids,
         cache,
         cache_update_index,
     ):
         """Forward pass of `GPTNeoXCausalLM` with cache.
@@ -136,27 +123,27 @@
         # Seed the cache.
         _, hidden_states, cache = self.call_with_cache(token_ids, cache, 0)
         return hidden_states, cache
 
     def generate_step(
         self,
         inputs,
-        end_token_id=None,
+        stop_token_ids=None,
     ):
         """A compilable generation function for a single batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
         for a single batch of inputs. Inputs should have the same structure as
         model inputs, a dictionary with keys `"token_ids"` and `"padding_mask"`.
 
         Args:
             inputs: A dictionary with two keys `"token_ids"` and
                 `"padding_mask"` and batched tensor values.
-            end_token_id: The id of the end token to stop on. If all
-                sequences have produced a new `end_token_id`, generation
+             stop_token_ids: Tuple of id's of end token's to stop on. If all
+                sequences have produced a new stop token, generation
                 will stop.
         """
         token_ids, padding_mask = inputs["token_ids"], inputs["padding_mask"]
         # Create and seed cache with a single forward pass.
         hidden_states, cache = self._build_cache(token_ids)
         # Compute the lengths of all user inputted tokens ids.
         row_lengths = ops.sum(ops.cast(padding_mask, "int32"), axis=-1)
@@ -175,33 +162,33 @@
             )
             return (
                 ops.squeeze(logits, axis=1),
                 ops.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        token_ids = self._sampler(
+        token_ids = self.sampler(
             next=next,
             prompt=token_ids,
             cache=cache,
             index=index,
             mask=padding_mask,
-            end_token_id=end_token_id,
+            stop_token_ids=stop_token_ids,
             hidden_states=hidden_states,
             model=self,
         )
 
         # Compute an output padding mask with the token ids we updated.
-        if end_token_id is not None:
-            # Build a mask of `end_token_id` locations not in the original
+        if stop_token_ids is not None:
+            # Build a mask of stop_tokens locations not in the original
             # prompt (not in locations where `padding_mask` is True).
-            end_locations = ops.logical_and(
-                ops.equal(token_ids, end_token_id),
-                ops.logical_not(padding_mask),
+            end_locations = any_equal(
+                token_ids, stop_token_ids, ops.logical_not(padding_mask)
             )
+
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
         else:
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     def generate_preprocess(
         self,
         x,
         sequence_length=None,
     ):
-        """Covert strings to integer token input for generation.
+        """Convert strings to integer token input for generation.
 
         Similar to calling the layer for training, this method takes in strings
         or tensor strings, tokenizes and packs the input, and computes a padding
         mask masking all inputs not filled in with a padded value.
 
         Unlike calling the layer for training, this method does not compute
         labels and will never append a `tokenizer.end_token_id` to the end of
@@ -123,15 +123,15 @@
             "padding_mask": padding_mask,
         }
 
     def generate_postprocess(
         self,
         x,
     ):
-        """Covert integer token output to strings for generation.
+        """Convert integer token output to strings for generation.
 
         This method reverses `generate_preprocess()`, by first removing all
         padding and start/end tokens, and then converting the integer sequence
         back to a string.
         """
         if not self.built:
             self.build(None)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
 from keras_nlp.src.models.gpt_neo_x.gpt_neo_x_tokenizer import GPTNeoXTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
 class GPTNeoXPreprocessor(Preprocessor):
     """GPTNeoX preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
@@ -61,14 +60,16 @@
         x: A string, `tf.Tensor` or list of python strings.
         y: Any label data. Will be passed through unaltered.
         sample_weight: Any label weight data. Will be passed through unaltered.
         sequence_length: Pass to override the configured `sequence_length` of
             the layer.
     """
 
+    tokenizer_cls = GPTNeoXTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=1024,
         add_start_token=True,
         add_end_token=True,
         **kwargs,
@@ -138,11 +139,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return GPTNeoXTokenizer
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_attention.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,199 +13,226 @@
 # limitations under the License.
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.rotary_embedding import RotaryEmbedding
 from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
-class LlamaAttention(keras.layers.Layer):
-    """Grouped query attention for Llama models"""
+# This is just a self-attention layer in Mistral. But it can be generalized
+# to use the `keras_nlp.layers.CachedMultiHeadAttention` API. Since this layer
+# implements grouped-query attention and sliding window attention, it might be
+# useful outside of Mistral itself.
+# TODO(tirthasheshpatel): Generalize the attention layer
+# TODO(tirthasheshpatel): Merge `LlamaAttention` with this layer
+# TODO(tirthasheshpatel): Use flash attention
+class CachedMistralAttention(keras.layers.Layer):
+    """A cached grounded query attention layer with sliding window."""
 
     def __init__(
         self,
         num_query_heads,
         num_key_value_heads,
+        rope_max_wavelength=10000,
         rope_scaling_factor=1.0,
         kernel_initializer="glorot_uniform",
-        rope_max_wavelength=10000,
-        max_sequence_length=512,
+        sliding_window=512,
+        dropout=0,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.num_query_heads = num_query_heads
-        self.num_key_value_heads = num_key_value_heads
+        self._num_query_heads = num_query_heads
+        self._num_key_value_heads = num_key_value_heads
+        self._sliding_window = sliding_window
+        self._dropout = dropout
 
-        self.num_key_value_groups = num_query_heads // num_key_value_heads
+        self._num_key_value_groups = num_query_heads // num_key_value_heads
+        self._rope_max_wavelength = rope_max_wavelength
 
-        self.kernel_initializer = keras.initializers.get(kernel_initializer)
-        self.max_sequence_length = max_sequence_length
+        self._kernel_initializer = keras.initializers.get(
+            clone_initializer(kernel_initializer)
+        )
 
-        self.rope_scaling_factor = rope_scaling_factor
-        self.rope_max_wavelength = rope_max_wavelength
+        self._rope_scaling_factor = rope_scaling_factor
 
     def build(self, inputs_shape):
-        self.hidden_dim = inputs_shape[-1]
-        self.attn_head_size = self.hidden_dim // self.num_query_heads
-
         # Einsum variables:
         # b = batch size
         # q = query length
         # k = key/value length
         # m = model dim
         # u = num query heads
         # v = num key/value heads
         # h = head dim
+        self._hidden_dim = inputs_shape[-1]
+        self._head_dim = self._hidden_dim // self._num_query_heads
+
         self._query_dense = keras.layers.EinsumDense(
             equation="bqm,muh->bquh",
-            output_shape=(None, self.num_query_heads, self.attn_head_size),
-            kernel_initializer=clone_initializer(self.kernel_initializer),
+            output_shape=(None, self._num_query_heads, self._head_dim),
+            kernel_initializer=self._kernel_initializer,
             dtype=self.dtype_policy,
             name="query",
         )
         self._query_dense.build(inputs_shape)
+
         self._key_dense = keras.layers.EinsumDense(
             equation="bkm,mvh->bkvh",
-            output_shape=(None, self.num_key_value_heads, self.attn_head_size),
-            kernel_initializer=clone_initializer(self.kernel_initializer),
+            output_shape=(
+                None,
+                self._num_key_value_heads,
+                self._head_dim,
+            ),
+            kernel_initializer=self._kernel_initializer,
             dtype=self.dtype_policy,
             name="key",
         )
         self._key_dense.build(inputs_shape)
 
         self._value_dense = keras.layers.EinsumDense(
             equation="bkm,mvh->bkvh",
-            output_shape=(None, self.num_key_value_heads, self.attn_head_size),
-            kernel_initializer=clone_initializer(self.kernel_initializer),
+            output_shape=(
+                None,
+                self._num_key_value_heads,
+                self._head_dim,
+            ),
+            kernel_initializer=self._kernel_initializer,
             dtype=self.dtype_policy,
             name="value",
         )
         self._value_dense.build(inputs_shape)
 
         self._softmax = keras.layers.Softmax(
             axis=-1,
             dtype="float32",
             name="attention_softmax",
         )
 
+        self._dropout_layer = keras.layers.Dropout(
+            rate=self._dropout,
+            dtype=self.dtype_policy,
+        )
+
         self._output_dense = keras.layers.EinsumDense(
-            equation="bqm,mh->bqh",
-            output_shape=(None, self.hidden_dim),
-            kernel_initializer=clone_initializer(self.kernel_initializer),
+            equation="bquh,uhm->bqm",
+            output_shape=(None, self._hidden_dim),
+            kernel_initializer=self._kernel_initializer,
             dtype=self.dtype_policy,
             name="attention_output",
         )
-        self._output_dense.build(inputs_shape)
+        self._output_dense.build(
+            (None, None, self._num_query_heads, self._head_dim)
+        )
 
-        self._rotary_embedding_layer = RotaryEmbedding(
-            max_wavelength=self.rope_max_wavelength,
-            scaling_factor=self.rope_scaling_factor,
+        self.rotary_embedding_layer = RotaryEmbedding(
+            max_wavelength=self._rope_max_wavelength,
+            scaling_factor=self._rope_scaling_factor,
             dtype=self.dtype_policy,
         )
-        self._rotary_embedding_layer.build(inputs_shape)
+
+        self._dot_product_equation = "bquh,bkuh->buqk"
+        self._combine_equation = "buqk,bkuh->bquh"
 
         self.built = True
 
     def call(
         self,
         hidden_states,
         attention_mask=None,
         cache=None,
         cache_update_index=None,
+        training=None,
     ):
+        start_index = (
+            cache_update_index if cache_update_index is not None else 0
+        )
+
         query = self._query_dense(hidden_states)
 
+        # Compute RoPE for queries
+        query = self.rotary_embedding_layer(query, start_index=start_index)
+
+        def _compute_key_value(x):
+            key, value = self._key_dense(x), self._value_dense(x)
+            # Compute RoPE for keys
+            key = self.rotary_embedding_layer(key, start_index=start_index)
+            return key, value
+
         if cache is not None:
             key_cache = cache[:, 0, ...]
             value_cache = cache[:, 1, ...]
             if cache_update_index is None:
                 key = key_cache
                 value = value_cache
             else:
-                key_update = self._key_dense(hidden_states)
-                value_update = self._value_dense(hidden_states)
+                key_update, value_update = _compute_key_value(hidden_states)
                 start = [0, cache_update_index, 0, 0]
                 key = ops.slice_update(key_cache, start, key_update)
                 value = ops.slice_update(value_cache, start, value_update)
                 cache = ops.stack((key, value), axis=1)
         else:
             if cache_update_index is not None:
                 raise ValueError(
                     "`cache_update_index` should not be set if `cache` is "
                     f"`None`. Received: cache={cache}, "
                     f"cache_update_index={cache_update_index}"
                 )
-            key = self._key_dense(hidden_states)
-            value = self._value_dense(hidden_states)
+            key, value = _compute_key_value(hidden_states)
 
-        query = self._rotary_embedding_layer(query)
-        key = self._rotary_embedding_layer(key)
+        # [batch_shape, seq_len, num_key_value_heads, head_dim]
+        # -> [batch_shape, seq_len, num_heads, head_dim]
+        key = ops.repeat(key, repeats=self._num_key_value_groups, axis=2)
+        value = ops.repeat(value, repeats=self._num_key_value_groups, axis=2)
 
-        key = ops.tile(key, [1, 1, self.num_key_value_groups, 1])
-        value = ops.tile(value, [1, 1, self.num_key_value_groups, 1])
-
-        attention_output, attention_scores = self._compute_attention(
+        attention_output = self._compute_attention(
             query, key, value, attention_mask
         )
 
-        attention_output_shape = ops.shape(attention_output)
-
-        attention_output = ops.reshape(
-            attention_output,
-            [
-                attention_output_shape[0],
-                attention_output_shape[1],
-                self.hidden_dim,
-            ],
+        attention_output = self._dropout_layer(
+            attention_output, training=training
         )
 
         attention_output = self._output_dense(attention_output)
 
         if cache is not None:
-            return (attention_output, cache)
+            return attention_output, cache
         return attention_output
 
     def _masked_softmax(self, attention_scores, attention_mask=None):
         if attention_mask is not None:
-            mask_expansion_axis = -3
-            for _ in range(
-                len(attention_scores.shape) - len(attention_mask.shape)
-            ):
-                attention_mask = ops.expand_dims(
-                    attention_mask, axis=mask_expansion_axis
-                )
-        return self._softmax(attention_scores, attention_mask)
+            return self._softmax(
+                attention_scores, attention_mask[:, None, :, :]
+            )
+        return self._softmax(attention_scores)
 
     def _compute_attention(self, query, key, value, attention_mask=None):
-        attention_scores = ops.einsum("aecd,abcd->acbe", key, query)
+        attention_scores = ops.einsum(self._dot_product_equation, query, key)
 
-        norm_factor = ops.sqrt(
-            ops.convert_to_tensor(self.attn_head_size, self.compute_dtype)
-        )
+        norm_factor = ops.sqrt(ops.cast(self._head_dim, self.compute_dtype))
 
-        attention_scores /= norm_factor
+        attention_scores = attention_scores / norm_factor
         attention_scores = self._masked_softmax(
             attention_scores, attention_mask
         )
         attention_scores = ops.cast(attention_scores, self.compute_dtype)
         attention_output = ops.einsum(
-            "acbe,aecd->abcd", attention_scores, value
+            self._combine_equation, attention_scores, value
         )
 
-        return attention_output, attention_scores
+        return attention_output
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "num_query_heads": self.num_query_heads,
-                "hidden_dim": self.hidden_dim,
+                "num_query_heads": self._num_query_heads,
+                "num_key_value_heads": self._num_key_value_heads,
+                "rope_max_wavelength": self._rope_max_wavelength,
+                "rope_scaling_factor": self._rope_scaling_factor,
                 "kernel_initializer": keras.initializers.serialize(
-                    self.kernel_initializer
+                    self._kernel_initializer
                 ),
-                "rope_max_wavelength": self.rope_max_wavelength,
-                "rope_scaling_factor": self.rope_scaling_factor,
-                "num_key_value_heads": self.num_key_value_heads,
-                "max_sequence_length": self.max_sequence_length,
+                "sliding_window": self._sliding_window,
+                "dropout": self._dropout,
             }
         )
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_backbone.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,110 +7,135 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.llama.llama_decoder import LlamaDecoder
+from keras_nlp.src.models.llama.llama_decoder import LlamaTransformerDecoder
 from keras_nlp.src.models.llama.llama_layernorm import LlamaLayerNorm
 
 
 def _llama_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.LlamaBackbone")
 class LlamaBackbone(Backbone):
     """
-    LLaMA core network with hyperparameters.
+    The Llama Transformer core architecture with hyperparameters.
 
     This network implements a Transformer-based decoder network,
-    LLaMA, as described in ["LLaMA: Open Foundation and Fine-Tuned Language Models"](https://arxiv.org/abs/2302.13971).
+    Llama, as described in
+    ["Llama 7B"](https://arxiv.org/pdf/2310.06825.pdf).
+    It includes the embedding lookups and transformer layers.
 
     The default constructor gives a fully customizable, randomly initialized
-    LLaMA model with any number of layers, heads, and embedding
-    dimensions. This backbone also supports LLaMA2 checkpoints.
+    Llama model with any number of layers, heads, and embedding
+    dimensions. To load preset architectures and weights, use the `from_preset`
+    constructor.
 
     Args:
-        vocabulary_size: int. The size of the token vocabulary.
-        num_layers: int. The number of transformer layers.
-        num_query_heads: int. The number of attention heads for each transformer.
-            The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The size of the transformer encoding and pooler layers.
-        intermediate_dim: int. The output dimension of the first Dense layer in
-            a two-layer feedforward network for each transformer.
-        num_key_value_heads: int. This is the number of key_value heads that
-            should be used to implement Grouped Query Attention. If num_key_value_heads=num_attention_heads,
-            the model will use Multi Head Attention (MHA), if num_key_value_heads=1
-            the model will use Multi Query Attention (MQA)
-        rope_scaling_factor: float. The scaling factor for calculation of rotary
-            embedding
-        rope_max_wavelength: int. The maximum angular wavelength of the
-            sine/cosine curves, for rotary embeddings.
-        layer_norm_epsilon: float. a value added to the denominator for
-            numerical stability.
-        max_sequence_length: int. The maximum sequence length that this encoder
-            can consume. If `None`, `max_sequence_length` uses the value from
-            sequence length. This determines the variable shape for positional
-            embeddings.
+        vocabulary_size (int): The size of the token vocabulary.
+        num_layers (int): The number of transformer layers.
+        num_query_heads (int): The number of query attention heads for
+            each transformer.
+        hidden_dim (int): The size of the transformer encoding and pooling layers.
+        intermediate_dim (int): The output dimension of the first Dense layer in a
+            three-layer feedforward network for each transformer.
+        num_key_value_heads (int): The number of key and value attention heads for
+            each transformer.
+        rope_max_wavelength (int, optional): The maximum angular wavelength of the
+            sine/cosine curves, for rotary embeddings. Defaults to `10000`.
+        rope_scaling_factor (float, optional): The scaling factor for calculation
+            of roatary embedding. Defaults to `1.0`.
+        layer_norm_epsilon (float, optional): Epsilon for the layer normalization
+            layers in the transformer decoder. Defaults to `1e-6`.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
             for model computations and weights. Note that some computations,
             such as softmax and layer normalization, will always be done at
             float32 precision regardless of dtype.
+
+    Examples:
+
+    ```python
+    input_data = {
+        "token_ids": np.ones(shape=(1, 12), dtype="int32"),
+        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
+    }
+
+    # Pretrained Llama decoder.
+    model = keras_nlp.models.LlamaBackbone.from_preset("llama7b_base_en")
+    model(input_data)
+
+    # Randomly initialized Llama decoder with custom config.
+    model = keras_nlp.models.LlamaBackbone(
+        vocabulary_size=10,
+        hidden_dim=512,
+        num_layers=2,
+        num_query_heads=32,
+        num_key_value_heads=8,
+        intermediate_dim=1024,
+        layer_norm_epsilon=1e-6,
+        dtype="float32"
+    )
+    model(input_data)
+    ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
         num_query_heads,
         hidden_dim,
         intermediate_dim,
         num_key_value_heads,
-        rope_scaling_factor=1.0,
         rope_max_wavelength=10000,
-        layer_norm_epsilon=1e-5,
-        max_sequence_length=4096,
+        rope_scaling_factor=1.0,
+        layer_norm_epsilon=1e-6,
+        dropout=0,
         dtype=None,
         **kwargs,
     ):
         # === Layers ===
         self.token_embedding = ReversibleEmbedding(
             input_dim=vocabulary_size,
             output_dim=hidden_dim,
-            embeddings_initializer=_llama_kernel_initializer(stddev=0.01),
             tie_weights=False,
+            embeddings_initializer=_llama_kernel_initializer(stddev=0.01),
             dtype=dtype,
+            reverse_dtype=dtype,
             name="token_embedding",
         )
         self.transformer_layers = []
         for i in range(num_layers):
-            layer = LlamaDecoder(
+            layer = LlamaTransformerDecoder(
                 intermediate_dim=intermediate_dim,
                 num_query_heads=num_query_heads,
                 num_key_value_heads=num_key_value_heads,
-                rope_scaling_factor=rope_scaling_factor,
-                max_sequence_length=max_sequence_length,
                 rope_max_wavelength=rope_max_wavelength,
+                rope_scaling_factor=rope_scaling_factor,
                 layer_norm_epsilon=layer_norm_epsilon,
                 activation=ops.silu,
                 kernel_initializer=_llama_kernel_initializer(stddev=0.02),
+                dropout=dropout,
                 dtype=dtype,
                 name=f"transformer_layer_{i}",
             )
             self.transformer_layers.append(layer)
         self.layer_norm = LlamaLayerNorm(
-            dtype=dtype,
             epsilon=layer_norm_epsilon,
-            name="layer_norm",
+            dtype=dtype,
+            name="sequence_output_layernorm",
         )
 
         # === Functional Model ===
         token_id_input = keras.Input(
             shape=(None,), dtype="int32", name="token_ids"
         )
         padding_mask_input = keras.Input(
@@ -122,40 +147,41 @@
         sequence_output = self.layer_norm(x)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=sequence_output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_query_heads = num_query_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.rope_max_wavelength = rope_max_wavelength
         self.num_key_value_heads = num_key_value_heads
         self.rope_scaling_factor = rope_scaling_factor
-        self.max_sequence_length = max_sequence_length
         self.layer_norm_epsilon = layer_norm_epsilon
+        self.dropout = dropout
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "vocabulary_size": self.vocabulary_size,
                 "num_layers": self.num_layers,
                 "num_query_heads": self.num_query_heads,
                 "hidden_dim": self.hidden_dim,
                 "intermediate_dim": self.intermediate_dim,
                 "rope_max_wavelength": self.rope_max_wavelength,
                 "rope_scaling_factor": self.rope_scaling_factor,
                 "num_key_value_heads": self.num_key_value_heads,
-                "max_sequence_length": self.max_sequence_length,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
+                "dropout": self.dropout,
             }
         )
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_decoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_decoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,209 +7,200 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# from keras_nlp.src.backend import keras
+# from keras_nlp.src.backend import ops
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.transformer_layer_utils import (
     compute_causal_mask,
 )
 from keras_nlp.src.layers.modeling.transformer_layer_utils import (
     merge_padding_and_attention_mask,
 )
-from keras_nlp.src.models.llama.llama_attention import LlamaAttention
-from keras_nlp.src.models.llama.llama_layernorm import LlamaLayerNorm
+from keras_nlp.src.models.bloom.bloom_attention import BloomAttention
 from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
-class LlamaDecoder(keras.layers.Layer):
-    """Llama decoder block."""
-
+class BloomDecoder(keras.layers.Layer):
     def __init__(
         self,
+        num_heads,
         intermediate_dim,
-        num_query_heads,
-        num_key_value_heads,
-        rope_scaling_factor=1.0,
-        activation="relu",
+        dropout=0.0,
         layer_norm_epsilon=1e-5,
         kernel_initializer="glorot_uniform",
-        rope_max_wavelength=10000,
-        max_sequence_length=512,
+        bias_initializer="zeros",
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.intermediate_dim = intermediate_dim
-        self.num_query_heads = num_query_heads
-        self.num_key_value_heads = num_key_value_heads
-
-        self.rope_max_wavelength = rope_max_wavelength
-        self.rope_scaling_factor = rope_scaling_factor
 
-        self.max_sequence_length = max_sequence_length
-        self.activation = keras.activations.get(activation)
+        self.num_heads = num_heads
+        self.intermediate_dim = intermediate_dim
+        self.dropout = dropout
         self.layer_norm_epsilon = layer_norm_epsilon
         self.kernel_initializer = keras.initializers.get(kernel_initializer)
+        self.bias_initializer = keras.initializers.get(bias_initializer)
 
     def build(self, decoder_sequence_shape):
-        self.hidden_dim = decoder_sequence_shape[-1]
+        hidden_dim = decoder_sequence_shape[-1]
+        head_dim = int(hidden_dim // self.num_heads)
 
-        # Self attention layers.
-        self._self_attention_layer = LlamaAttention(
-            num_query_heads=self.num_query_heads,
-            num_key_value_heads=self.num_key_value_heads,
-            rope_max_wavelength=self.rope_max_wavelength,
-            max_sequence_length=self.max_sequence_length,
-            rope_scaling_factor=self.rope_scaling_factor,
-            kernel_initializer=clone_initializer(self.kernel_initializer),
-            dtype=self.dtype_policy,
-        )
-        self._self_attention_layer.build(decoder_sequence_shape)
+        if head_dim * self.num_heads != hidden_dim:
+            raise ValueError(
+                f"`hidden_dim` must be divisible by num_heads (got `hidden_dim`"
+                f": {hidden_dim} and `num_heads`: {self.num_heads})."
+            )
 
-        self._self_attention_layernorm = LlamaLayerNorm(
+        self._pre_attention_layernorm = keras.layers.LayerNormalization(
             epsilon=self.layer_norm_epsilon,
             dtype=self.dtype_policy,
+            name="pre_attention_layernorm",
         )
-        self._self_attention_layernorm.build(decoder_sequence_shape)
+        self._pre_attention_layernorm.build(decoder_sequence_shape)
 
-        # Feedforward layers.
-        self._feedforward_intermediate_dense = keras.layers.Dense(
-            self.intermediate_dim,
+        self._self_attention_layer = BloomAttention(
+            num_heads=self.num_heads,
+            dropout=self.dropout,
             kernel_initializer=clone_initializer(self.kernel_initializer),
+            bias_initializer=clone_initializer(self.bias_initializer),
             dtype=self.dtype_policy,
+            name="self_attention",
         )
-        self._feedforward_intermediate_dense.build(decoder_sequence_shape)
+        self._self_attention_layer.build(decoder_sequence_shape)
+
+        self._post_attention_layernorm = keras.layers.LayerNormalization(
+            epsilon=self.layer_norm_epsilon,
+            dtype=self.dtype_policy,
+            name="post_attention_layernorm",
+        )
+        self._post_attention_layernorm.build(decoder_sequence_shape)
 
-        self._feedforward_gate_dense = keras.layers.Dense(
+        self._mlp_intermediate_dense = keras.layers.Dense(
             self.intermediate_dim,
-            activation=self.activation,
             kernel_initializer=clone_initializer(self.kernel_initializer),
+            bias_initializer=clone_initializer(self.bias_initializer),
             dtype=self.dtype_policy,
+            name="mlp_intermediate_dense",
         )
-        self._feedforward_gate_dense.build(decoder_sequence_shape)
+        self._mlp_intermediate_dense.build(decoder_sequence_shape)
 
-        self._feedforward_output_dense = keras.layers.Dense(
-            self.hidden_dim,
+        self._mlp_output_dense = keras.layers.Dense(
+            hidden_dim,
             kernel_initializer=clone_initializer(self.kernel_initializer),
+            bias_initializer=clone_initializer(self.bias_initializer),
             dtype=self.dtype_policy,
+            name="mlp_output_dense",
         )
-
         intermediate_shape = list(decoder_sequence_shape)
         intermediate_shape[-1] = self.intermediate_dim
-        self._feedforward_output_dense.build(tuple(intermediate_shape))
+        self._mlp_output_dense.build(tuple(intermediate_shape))
 
-        self._feedforward_layernorm = LlamaLayerNorm(
-            epsilon=self.layer_norm_epsilon,
-            dtype=self.dtype_policy,
+        self._dropout_layer = keras.layers.Dropout(
+            rate=self.dropout, dtype=self.dtype_policy, name="dropout"
         )
-        self._feedforward_layernorm.build(decoder_sequence_shape)
 
         self.built = True
 
     def call(
         self,
         decoder_sequence,
         decoder_padding_mask=None,
         decoder_attention_mask=None,
-        self_attention_cache=None,
-        self_attention_cache_update_index=None,
+        cache=None,
+        cache_update_index=None,
+        use_causal_mask=True,
     ):
-        self_attention_mask = self._compute_self_attention_mask(
+        self_attention_mask = self._compute_attention_mask(
             decoder_sequence=decoder_sequence,
             decoder_padding_mask=decoder_padding_mask,
             decoder_attention_mask=decoder_attention_mask,
-            self_attention_cache=self_attention_cache,
-            self_attention_cache_update_index=self_attention_cache_update_index,
+            use_causal_mask=use_causal_mask,
+            cache=cache,
+            cache_update_index=cache_update_index,
         )
-        residual = decoder_sequence
 
-        x = self._self_attention_layernorm(
-            decoder_sequence,
-        )
+        residual = decoder_sequence
+        x = self._pre_attention_layernorm(decoder_sequence)
 
-        x = self._self_attention_layer(
+        attention_output = self._self_attention_layer(
             hidden_states=x,
             attention_mask=self_attention_mask,
-            cache=self_attention_cache,
-            cache_update_index=self_attention_cache_update_index,
+            cache=cache,
+            cache_update_index=cache_update_index,
         )
 
-        if self_attention_cache is not None:
-            x, self_attention_cache = x
+        if cache is None:
+            x = attention_output
+        else:
+            x, cache = attention_output
 
         x = x + residual
         residual = x
+        x = self._post_attention_layernorm(x)
+        x = self._mlp_intermediate_dense(x)
+        x = keras.activations.gelu(x, approximate=True)
+        x = self._mlp_output_dense(x)
+        x = self._dropout_layer(x)
+        x = x + residual
 
-        x = self._feedforward_layernorm(x)
-        gate_output = self._feedforward_gate_dense(x)
-
-        x = self._feedforward_intermediate_dense(x)
-
-        x = self._feedforward_output_dense(ops.multiply(x, gate_output))
-
-        decoder_output = x + residual
-
-        if self_attention_cache is not None:
-            return (decoder_output, self_attention_cache)
-        return decoder_output
+        if cache is not None:
+            return x, cache
+        else:
+            return x
 
-    def _compute_self_attention_mask(
+    def _compute_attention_mask(
         self,
         decoder_sequence,
         decoder_padding_mask,
         decoder_attention_mask,
-        self_attention_cache=None,
-        self_attention_cache_update_index=None,
+        use_causal_mask,
+        cache,
+        cache_update_index,
     ):
         decoder_mask = merge_padding_and_attention_mask(
             decoder_sequence, decoder_padding_mask, decoder_attention_mask
         )
-        batch_size = ops.shape(decoder_sequence)[0]
-        input_length = output_length = ops.shape(decoder_sequence)[1]
-        # We need to handle a rectangular causal mask when doing cached
-        # decoding. For generative inference, `decoder_sequence` will
-        # generally be length 1, and `cache` will be the full generation length.
-        if self_attention_cache is not None:
-            input_length = ops.shape(self_attention_cache)[2]
-
-        causal_mask = compute_causal_mask(
-            batch_size,
-            input_length,
-            output_length,
-            (
-                0
-                if self_attention_cache_update_index is None
-                else self_attention_cache_update_index
-            ),
-        )
-        return (
-            ops.minimum(decoder_mask, causal_mask)
-            if decoder_mask is not None
-            else causal_mask
-        )
-
-    def compute_output_shape(self, decoder_sequence_shape):
-        return decoder_sequence_shape
+        if use_causal_mask:
+            batch_size = ops.shape(decoder_sequence)[0]
+            input_length = output_length = ops.shape(decoder_sequence)[1]
+            if cache is not None:
+                input_length = ops.shape(cache)[2]
+
+            causal_mask = compute_causal_mask(
+                batch_size,
+                input_length,
+                output_length,
+                (0 if cache_update_index is None else cache_update_index),
+            )
+            return (
+                ops.minimum(decoder_mask, causal_mask)
+                if decoder_mask is not None
+                else causal_mask
+            )
+        return decoder_mask
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
+                "num_heads": self.num_heads,
                 "intermediate_dim": self.intermediate_dim,
-                "hidden_dim": self.hidden_dim,
-                "num_query_heads": self.num_query_heads,
-                "rope_max_wavelength": self.rope_max_wavelength,
-                "rope_scaling_factor": self.rope_scaling_factor,
-                "num_key_value_heads": self.num_key_value_heads,
-                "max_sequence_length": self.max_sequence_length,
-                "activation": keras.activations.serialize(self.activation),
+                "dropout": self.dropout,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
                 "kernel_initializer": keras.initializers.serialize(
                     self.kernel_initializer
                 ),
+                "bias_initializer": keras.initializers.serialize(
+                    self.bias_initializer
+                ),
             }
         )
         return config
 
+    def compute_output_shape(self, decoder_sequence_shape):
+        return decoder_sequence_shape
+
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_layernorm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_layer_norm.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,32 +7,30 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 
-# TODO: Should be replaced with LayerNormalization with `rms_scaling` param
-# https://github.com/keras-team/keras-core/pull/726
-
 
-class LlamaLayerNorm(keras.layers.Layer):
+class T5LayerNorm(keras.layers.Layer):
     def __init__(self, epsilon=1e-6, **kwargs):
         super().__init__(**kwargs)
         self.epsilon = epsilon
 
     def build(self, input_shape):
         self.weight = self.add_weight(
             name="weight",
             shape=(input_shape[-1],),
             initializer="ones",
         )
         self.built = True
 
     def call(self, hidden_states):
         variance = ops.mean(ops.square(hidden_states), axis=-1, keepdims=True)
-        hidden_states = hidden_states * 1 / ops.sqrt(variance + self.epsilon)
+        hidden_states = hidden_states * ops.rsqrt(variance + self.epsilon)
         return self.weight * hidden_states
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/llama/llama_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import copy
+
 from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.llama.llama_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.LlamaTokenizer")
 class LlamaTokenizer(SentencePieceTokenizer):
     """Llama tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -76,7 +80,11 @@
             self.end_token_id = self.token_to_id(self.end_token)
             self.pad_token_id = 0
         else:
             self.start_token_id = None
             self.end_token_id = None
             self.pad_token_id = None
 
+    @classproperty
+    def presets(cls):
+        return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_attention.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,122 +13,112 @@
 # limitations under the License.
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.rotary_embedding import RotaryEmbedding
 from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
-# This is just a self-attention layer in Mistral. But it can be generalized
-# to use the `keras_nlp.layers.CachedMultiHeadAttention` API. Since this layer
-# implements grouped-query attention and sliding window attention, it might be
-# useful outside of Mistral itself.
-# TODO(tirthasheshpatel): Generalize the attention layer
-# TODO(tirthasheshpatel): Merge `LlamaAttention` with this layer
-# TODO(tirthasheshpatel): Use flash attention
-class CachedMistralAttention(keras.layers.Layer):
+class LlamaAttention(keras.layers.Layer):
     """A cached grounded query attention layer with sliding window."""
 
     def __init__(
         self,
         num_query_heads,
         num_key_value_heads,
         rope_max_wavelength=10000,
         rope_scaling_factor=1.0,
         kernel_initializer="glorot_uniform",
-        sliding_window=512,
         dropout=0,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self._num_query_heads = num_query_heads
-        self._num_key_value_heads = num_key_value_heads
-        self._sliding_window = sliding_window
-        self._dropout = dropout
+        self.num_query_heads = num_query_heads
+        self.num_key_value_heads = num_key_value_heads
+        self.dropout = dropout
 
-        self._num_key_value_groups = num_query_heads // num_key_value_heads
-        self._rope_max_wavelength = rope_max_wavelength
+        self.num_key_value_groups = num_query_heads // num_key_value_heads
+        self.rope_max_wavelength = rope_max_wavelength
 
-        self._kernel_initializer = keras.initializers.get(
+        self.kernel_initializer = keras.initializers.get(
             clone_initializer(kernel_initializer)
         )
 
-        self._rope_scaling_factor = rope_scaling_factor
+        self.rope_scaling_factor = rope_scaling_factor
 
     def build(self, inputs_shape):
         # Einsum variables:
         # b = batch size
         # q = query length
         # k = key/value length
         # m = model dim
         # u = num query heads
         # v = num key/value heads
         # h = head dim
-        self._hidden_dim = inputs_shape[-1]
-        self._head_dim = self._hidden_dim // self._num_query_heads
+        hidden_dim = inputs_shape[-1]
+        head_dim = hidden_dim // self.num_query_heads
+        self._norm_factor = ops.sqrt(ops.cast(head_dim, self.compute_dtype))
 
         self._query_dense = keras.layers.EinsumDense(
             equation="bqm,muh->bquh",
-            output_shape=(None, self._num_query_heads, self._head_dim),
-            kernel_initializer=self._kernel_initializer,
+            output_shape=(None, self.num_query_heads, head_dim),
+            kernel_initializer=self.kernel_initializer,
             dtype=self.dtype_policy,
             name="query",
         )
         self._query_dense.build(inputs_shape)
 
         self._key_dense = keras.layers.EinsumDense(
             equation="bkm,mvh->bkvh",
             output_shape=(
                 None,
-                self._num_key_value_heads,
-                self._head_dim,
+                self.num_key_value_heads,
+                head_dim,
             ),
-            kernel_initializer=self._kernel_initializer,
+            kernel_initializer=self.kernel_initializer,
             dtype=self.dtype_policy,
             name="key",
         )
         self._key_dense.build(inputs_shape)
 
         self._value_dense = keras.layers.EinsumDense(
             equation="bkm,mvh->bkvh",
             output_shape=(
                 None,
-                self._num_key_value_heads,
-                self._head_dim,
+                self.num_key_value_heads,
+                head_dim,
             ),
-            kernel_initializer=self._kernel_initializer,
+            kernel_initializer=self.kernel_initializer,
             dtype=self.dtype_policy,
             name="value",
         )
         self._value_dense.build(inputs_shape)
 
         self._softmax = keras.layers.Softmax(
             axis=-1,
             dtype="float32",
             name="attention_softmax",
         )
 
         self._dropout_layer = keras.layers.Dropout(
-            rate=self._dropout,
+            rate=self.dropout,
             dtype=self.dtype_policy,
         )
 
         self._output_dense = keras.layers.EinsumDense(
             equation="bquh,uhm->bqm",
-            output_shape=(None, self._hidden_dim),
-            kernel_initializer=self._kernel_initializer,
+            output_shape=(None, hidden_dim),
+            kernel_initializer=self.kernel_initializer,
             dtype=self.dtype_policy,
             name="attention_output",
         )
-        self._output_dense.build(
-            (None, None, self._num_query_heads, self._head_dim)
-        )
+        self._output_dense.build((None, None, self.num_query_heads, head_dim))
 
         self.rotary_embedding_layer = RotaryEmbedding(
-            max_wavelength=self._rope_max_wavelength,
-            scaling_factor=self._rope_scaling_factor,
+            max_wavelength=self.rope_max_wavelength,
+            scaling_factor=self.rope_scaling_factor,
             dtype=self.dtype_policy,
         )
 
         self._dot_product_equation = "bquh,bkuh->buqk"
         self._combine_equation = "buqk,bkuh->bquh"
 
         self.built = True
@@ -140,19 +130,14 @@
         cache=None,
         cache_update_index=None,
         training=None,
     ):
         start_index = (
             cache_update_index if cache_update_index is not None else 0
         )
-        # If `cache_update_index` is a tensor, RotaryEmbedding expects it
-        # to have dtype `self.compute_dtype`.
-        start_index = ops.cast(
-            start_index, self.rotary_embedding_layer.compute_dtype
-        )
 
         query = self._query_dense(hidden_states)
 
         # Compute RoPE for queries
         query = self.rotary_embedding_layer(query, start_index=start_index)
 
         def _compute_key_value(x):
@@ -180,16 +165,16 @@
                     f"`None`. Received: cache={cache}, "
                     f"cache_update_index={cache_update_index}"
                 )
             key, value = _compute_key_value(hidden_states)
 
         # [batch_shape, seq_len, num_key_value_heads, head_dim]
         # -> [batch_shape, seq_len, num_heads, head_dim]
-        key = ops.repeat(key, repeats=self._num_key_value_groups, axis=2)
-        value = ops.repeat(value, repeats=self._num_key_value_groups, axis=2)
+        key = ops.repeat(key, repeats=self.num_key_value_groups, axis=2)
+        value = ops.repeat(value, repeats=self.num_key_value_groups, axis=2)
 
         attention_output = self._compute_attention(
             query, key, value, attention_mask
         )
 
         attention_output = self._dropout_layer(
             attention_output, training=training
@@ -207,37 +192,34 @@
                 attention_scores, attention_mask[:, None, :, :]
             )
         return self._softmax(attention_scores)
 
     def _compute_attention(self, query, key, value, attention_mask=None):
         attention_scores = ops.einsum(self._dot_product_equation, query, key)
 
-        norm_factor = ops.sqrt(ops.cast(self._head_dim, self.compute_dtype))
-
-        attention_scores = attention_scores / norm_factor
+        attention_scores = attention_scores / self._norm_factor
         attention_scores = self._masked_softmax(
             attention_scores, attention_mask
         )
         attention_scores = ops.cast(attention_scores, self.compute_dtype)
         attention_output = ops.einsum(
             self._combine_equation, attention_scores, value
         )
 
         return attention_output
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "num_query_heads": self._num_query_heads,
-                "num_key_value_heads": self._num_key_value_heads,
-                "rope_max_wavelength": self._rope_max_wavelength,
-                "rope_scaling_factor": self._rope_scaling_factor,
+                "num_query_heads": self.num_query_heads,
+                "num_key_value_heads": self.num_key_value_heads,
+                "rope_max_wavelength": self.rope_max_wavelength,
+                "rope_scaling_factor": self.rope_scaling_factor,
                 "kernel_initializer": keras.initializers.serialize(
-                    self._kernel_initializer
+                    self.kernel_initializer
                 ),
-                "sliding_window": self._sliding_window,
-                "dropout": self._dropout,
+                "dropout": self.dropout,
             }
         )
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.mistral.mistral_layer_norm import (
     MistralLayerNormalization,
 )
-from keras_nlp.src.models.mistral.mistral_presets import backbone_presets
 from keras_nlp.src.models.mistral.mistral_transformer_decoder import (
     MistralTransformerDecoder,
 )
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def _mistral_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.MistralBackbone")
@@ -120,14 +117,15 @@
         # === Layers ===
         self.token_embedding = ReversibleEmbedding(
             input_dim=vocabulary_size,
             output_dim=hidden_dim,
             tie_weights=False,
             embeddings_initializer=_mistral_kernel_initializer(stddev=0.01),
             dtype=dtype,
+            reverse_dtype=dtype,
             name="token_embedding",
         )
         self.transformer_layers = []
         for i in range(num_layers):
             layer = MistralTransformerDecoder(
                 intermediate_dim=intermediate_dim,
                 num_query_heads=num_query_heads,
@@ -162,14 +160,15 @@
         sequence_output = self.layer_norm(x)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=sequence_output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_query_heads = num_query_heads
@@ -197,11 +196,7 @@
                 "sliding_window": self.sliding_window,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
                 "dropout": self.dropout,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_causal_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_causal_lm.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,159 +7,243 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
+
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
-from keras_nlp.src.models.generative_task import GenerativeTask
-from keras_nlp.src.models.mistral.mistral_backbone import MistralBackbone
-from keras_nlp.src.models.mistral.mistral_causal_lm_preprocessor import (
-    MistralCausalLMPreprocessor,
+from keras_nlp.src.models.causal_lm import CausalLM
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
+    OPTCausalLMPreprocessor,
 )
-from keras_nlp.src.models.mistral.mistral_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
-@keras_nlp_export("keras_nlp.models.MistralCausalLM")
-class MistralCausalLM(GenerativeTask):
-    """An end-to-end Mistral model for causal language modeling.
+@keras_nlp_export("keras_nlp.models.OPTCausalLM")
+class OPTCausalLM(CausalLM):
+    """An end-to-end OPT model for causal language modeling.
 
     A causal language model (LM) predicts the next token based on previous
     tokens. This task setup can be used to train the model unsupervised on
     plain text input, or to autoregressively generate plain text similar to
     the data used for training. This task can be used for pre-training or
-    fine-tuning a GPT-NeoX model, simply by calling `fit()`.
+    fine-tuning a GPT-2 model, simply by calling `fit()`.
 
     This model has a `generate()` method, which generates text based on a
     prompt. The generation strategy used is controlled by an additional
     `sampler` argument on `compile()`. You can recompile the model with
     different `keras_nlp.samplers` objects to control the generation. By
     default, `"top_k"` sampling will be used.
 
+    This model can optionally be configured with a `preprocessor` layer, in
+    which case it will automatically apply preprocessing to string inputs during
+    `fit()`, `predict()`, `evaluate()` and `generate()`. This is done by default
+    when creating the model with `from_preset()`.
+
+    Disclaimer: Pre-trained models are provided on an "as is" basis, without
+    warranties or conditions of any kind. The underlying model is provided by a
+    third party and subject to a separate license, available
+    [here](https://github.com/facebookresearch/fairseq/).
+
     Args:
-        backbone: A `keras_nlp.models.MistralBackbone` instance.
-        preprocessor: A `keras_nlp.models.MistralCausalLMPreprocessor` or `None`.
+        backbone: A `keras_nlp.models.OPTBackbone` instance.
+        preprocessor: A `keras_nlp.models.OPTCausalLMPreprocessor` or `None`.
             If `None`, this model will not apply preprocessing, and inputs
             should be preprocessed before calling the model.
+
+    Examples:
+
+    Use `generate()` to do text generation.
+    ```python
+    opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
+    opt_lm.generate("I want to say", max_length=30)
+
+    # Generate with batched prompts.
+    opt_lm.generate(["This is a", "Where are you"], max_length=30)
+    ```
+
+    Compile the `generate()` function with a custom sampler.
+    ```python
+    opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
+    opt_lm.compile(sampler="greedy")
+    opt_lm.generate("I want to say", max_length=30)
+
+    opt_lm.compile(sampler=keras_nlp.samplers.BeamSampler(num_beams=2))
+    opt_lm.generate("I want to say", max_length=30)
+    ```
+
+    Use `generate()` without preprocessing.
+    ```python
+    # Prompt the model with `5338, 318` (the token ids for `"Who is"`).
+    # Use `"padding_mask"` to indicate values that should not be overridden.
+    prompt = {
+        "token_ids": np.array([[5338, 318, 0, 0, 0]] * 2),
+        "padding_mask": np.array([[1, 1, 0, 0, 0]] * 2),
+    }
+
+    opt_lm = keras_nlp.models.OPTCausalLM.from_preset(
+        "opt_125m_en",
+        preprocessor=None,
+    )
+    opt_lm.generate(prompt)
+    ```
+
+    Call `fit()` on a single batch.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
+    opt_lm.fit(x=features, batch_size=2)
+    ```
+
+    Call `fit()` without preprocessing.
+    ```python
+    x = {
+        "token_ids": np.array([[1, 2, 3, 4, 5]] * 2),
+        "padding_mask": np.array([[1, 1, 1, 1, 1]] * 2),
+    }
+    y = np.array([[2, 3, 4, 5, 0]] * 2)
+    sw = np.array([[1, 1, 1, 1, 1]] * 2)
+
+    opt_lm = keras_nlp.models.OPTCausalLM.from_preset(
+        "opt_base_en",
+        preprocessor=None,
+    )
+    opt_lm.fit(x=x, y=y, sample_weight=sw, batch_size=2)
+    ```
+
+    Custom backbone and vocabulary.
+    ```python
+    features = ["a quick fox.", "a fox quick."]
+    vocab = {"<|endoftext|>": 0, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+
+    tokenizer = keras_nlp.models.OPTTokenizer(
+        vocabulary=vocab,
+        merges=merges,
+    )
+    preprocessor = keras_nlp.models.OPTCausalLMPreprocessor(
+        tokenizer=tokenizer,
+        sequence_length=128,
+    )
+    model = keras_nlp.models.OPTBackbone(
+        vocabulary_size=50265,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
+    )
+    opt_lm = keras_nlp.models.OPTCausalLM(
+        backbone=backbone,
+        preprocessor=preprocessor,
+    )
+    opt_lm.fit(x=features, batch_size=2)
+    ```
     """
 
-    def __init__(self, backbone, preprocessor=None, **kwargs):
+    backbone_cls = OPTBackbone
+    preprocessor_cls = OPTCausalLMPreprocessor
+
+    def __init__(
+        self,
+        backbone,
+        preprocessor=None,
+        **kwargs,
+    ):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
 
         # === Functional Model ===
-        inputs = backbone.inputs
+        inputs = backbone.input
         hidden_states = backbone(inputs)
         outputs = backbone.token_embedding(hidden_states, reverse=True)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return MistralBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return MistralCausalLMPreprocessor
-
     def call_with_cache(
         self,
         token_ids,
         cache,
         cache_update_index,
     ):
-        """Forward pass of `MistralCausalLM` with cache.
+        """Forward pass of `OPTCausalLM` with cache.
 
         `call_with_cache` adds an additional forward pass for the model for
         autoregressive inference. Unlike calling the model directly, this method
         allows caching previous key/value Tensors in multi-head attention layer,
         and avoids recomputing the outputs of seen tokens.
 
         Args:
             token_ids: a dense int Tensor with shape `(batch_size, max_length)`.
             cache: a dense float Tensor, the cache of key and value.
-            cache_update_index: int, or int Tensor. The index of current inputs
-            in the whole sequence.
+            cache_update_index: int, or int Tensor. The index of current inputs in the
+                whole sequence.
 
         Returns:
             A (logits, hidden_states, cache) tuple. Where `logits` is the
             language model logits for the input token_ids, `hidden_states` is
             the final hidden representation of the input tokens, and `cache` is
             the decoding cache.
         """
-        x = self.backbone.token_embedding(token_ids)
+        x = self.backbone.embeddings(token_ids, start_index=cache_update_index)
         # Each decoder layer has a cache; we update them separately.
-        updated_cache = []
-        for i in range(self.backbone.num_layers):
+        caches = []
+        for i, transformer_layer in enumerate(self.backbone.transformer_layers):
             current_cache = cache[:, i, ...]
-            x, next_cache = self.backbone.transformer_layers[i](
+            x, next_cache = transformer_layer(
                 x,
                 self_attention_cache=current_cache,
                 self_attention_cache_update_index=cache_update_index,
             )
-            updated_cache.append(next_cache)
-        cache = ops.stack(updated_cache, axis=1)
-        hidden_states = x = self.backbone.layer_norm(x)
-        logits = self.backbone.token_embedding(x, reverse=True)
+            caches.append(next_cache)
+        cache = ops.stack(caches, axis=1)
+        x = self.backbone.layer_norm(x)
+        hidden_states = x
+        logits = self.backbone.token_embedding(hidden_states, reverse=True)
         return logits, hidden_states, cache
 
     def _build_cache(self, token_ids):
         """Build an empty cache for use with `call_with_cache()`."""
         batch_size = ops.shape(token_ids)[0]
         max_length = ops.shape(token_ids)[1]
         num_layers = self.backbone.num_layers
-        num_key_value_heads = self.backbone.num_key_value_heads
-        head_dim = self.backbone.hidden_dim // self.backbone.num_query_heads
-        shape = [
-            batch_size,
-            num_layers,
-            2,
-            max_length,
-            num_key_value_heads,
-            head_dim,
-        ]
+        num_heads = self.backbone.num_heads
+        head_dim = self.backbone.hidden_dim // self.backbone.num_heads
+        shape = [batch_size, num_layers, 2, max_length, num_heads, head_dim]
         cache = ops.zeros(shape, dtype=self.compute_dtype)
         # Seed the cache.
         _, hidden_states, cache = self.call_with_cache(token_ids, cache, 0)
         return hidden_states, cache
 
     def generate_step(
         self,
         inputs,
-        end_token_id=None,
+        stop_token_ids=None,
     ):
         """A compilable generation function for a single batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
         for a single batch of inputs. Inputs should have the same structure as
         model inputs, a dictionary with keys `"token_ids"` and `"padding_mask"`.
 
         Args:
             inputs: A dictionary with two keys `"token_ids"` and
                 `"padding_mask"` and batched tensor values.
-            end_token_id: The id of the end token to stop on. If all
-                sequences have produced a new `end_token_id`, generation
+            stop_token_ids: Tuple of id's of end token's to stop on. If all
+                sequences have produced a new stop token, generation
                 will stop.
         """
         token_ids, padding_mask = inputs["token_ids"], inputs["padding_mask"]
         # Create and seed cache with a single forward pass.
         hidden_states, cache = self._build_cache(token_ids)
         # Compute the lengths of all user inputted tokens ids.
         row_lengths = ops.sum(ops.cast(padding_mask, "int32"), axis=-1)
@@ -178,44 +262,40 @@
             )
             return (
                 ops.squeeze(logits, axis=1),
                 ops.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        token_ids = self._sampler(
+        token_ids = self.sampler(
             next=next,
             prompt=token_ids,
             cache=cache,
             index=index,
             mask=padding_mask,
-            end_token_id=end_token_id,
+            stop_token_ids=stop_token_ids,
             hidden_states=hidden_states,
             model=self,
         )
 
         # Compute an output padding mask with the token ids we updated.
-        if end_token_id is not None:
-            # Build a mask of `end_token_id` locations not in the original
+        if stop_token_ids is not None:
+            # Build a mask of stop token locations not in the original
             # prompt (not in locations where `padding_mask` is True).
-            end_locations = ops.logical_and(
-                ops.equal(token_ids, end_token_id),
-                ops.logical_not(padding_mask),
+            end_locations = any_equal(
+                token_ids, stop_token_ids, ops.logical_not(padding_mask)
             )
+
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
             padding_mask = ops.logical_not(ops.cast(overflow, "bool"))
         else:
             # Without early stopping, all locations will have been updated.
             padding_mask = ops.ones_like(token_ids, dtype="bool")
         return {
             "token_ids": token_ids,
             "padding_mask": padding_mask,
         }
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_causal_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_causal_lm_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     def generate_preprocess(
         self,
         x,
         sequence_length=None,
     ):
-        """Covert strings to integer token input for generation.
+        """Convert strings to integer token input for generation.
 
         Similar to calling the layer for training, this method takes in strings
         or tensor strings, tokenizes and packs the input, and computes a padding
         mask masking all inputs not filled in with a padded value.
 
         Unlike calling the layer for training, this method does not compute
         labels and will never append a `tokenizer.end_token_id` to the end of
@@ -155,15 +155,15 @@
             "padding_mask": padding_mask,
         }
 
     def generate_postprocess(
         self,
         x,
     ):
-        """Covert integer token output to strings for generation.
+        """Convert integer token output to strings for generation.
 
         This method reverses `generate_preprocess()`, by first removing all
         padding and start/end tokens, and then converting the integer sequence
         back to a string.
         """
         token_ids, padding_mask = x["token_ids"], x["padding_mask"]
         # Convert the inputs to numpy arrays if they aren't a tensor already.
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_layer_norm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_layer_norm.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 # `keras.layers.LayerNormalization(rms_scaling=True)` once Keras 2 support is
 # removed.
 class MistralLayerNormalization(keras.layers.Layer):
     """A normalization layer for Mistral that implements RMS normalization."""
 
     def __init__(self, epsilon=1e-6, **kwargs):
         super().__init__(**kwargs)
-        self._epsilon = epsilon
+        self.epsilon = epsilon
 
     def build(self, input_shape):
-        self._dim = input_shape[-1]
-        self._weight = self.add_weight(
-            name="weight",
+        dim = input_shape[-1]
+        self.scale = self.add_weight(
+            name="scale",
             trainable=True,
-            shape=(self._dim,),
+            shape=(dim,),
             initializer="ones",
+            dtype=self.variable_dtype,
         )
         self.built = True
 
     def call(self, x):
-        x = x * ops.rsqrt(
-            ops.mean(ops.power(x, 2), axis=-1, keepdims=True) + self._epsilon
-        )
-        return x * self._weight
+        x = ops.cast(x, "float32")
+        var = ops.mean(ops.power(x, 2), axis=-1, keepdims=True)
+        x = x * ops.rsqrt(var + self.epsilon)
+        return ops.cast(x, self.compute_dtype) * self.scale
 
     def get_config(self):
         config = super().get_config()
-        config.update({"epsilon": self._epsilon})
+        config.update({"epsilon": self.epsilon})
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_preprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,46 +7,42 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
-from keras_nlp.src.models.mistral.mistral_presets import backbone_presets
-from keras_nlp.src.models.mistral.mistral_tokenizer import MistralTokenizer
+from keras_nlp.src.models.llama.llama_tokenizer import LlamaTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras_nlp_export("keras_nlp.models.MistralPreprocessor")
-class MistralPreprocessor(Preprocessor):
-    """A Mistral preprocessing layer which tokenizes and packs inputs.
+@keras_nlp_export("keras_nlp.models.LlamaPreprocessor")
+class LlamaPreprocessor(Preprocessor):
+    """A Llama preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
 
      1. Tokenize any number of input segments using the `tokenizer`.
      2. Pack the inputs together using a `keras_nlp.layers.StartEndPacker`.
        with the appropriate tokens.
      3. Construct a dictionary with keys `"token_ids"`, and `"padding_mask"`
-       that can be passed directly to `keras_nlp.models.MistralBackbone`.
+       that can be passed directly to `keras_nlp.models.LlamaBackbone`.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
     Args:
-        tokenizer: A `keras_nlp.models.MistralTokenizer` instance.
+        tokenizer: A `keras_nlp.models.LlamaTokenizer` instance.
         sequence_length: The length of the packed inputs.
         add_start_token: If `True`, the preprocessor will prepend the tokenizer
             start token to each input sequence. Default is `True`.
         add_end_token: If `True`, the preprocessor will append the tokenizer
             end token to each input sequence. Default is `False`.
 
     Call arguments:
@@ -59,16 +55,16 @@
         sequence_length: Pass to override the configured `sequence_length` of
             the layer.
 
     Examples:
 
     Directly calling the from_preset().
     ```python
-    preprocessor = keras_nlp.models.MistralPreprocessor.from_preset(
-        "mistral_base_en"
+    preprocessor = keras_nlp.models.LlamaPreprocessor.from_preset(
+        "llama_base_en"
     )
 
     # Tokenize and pack a single sentence.
     preprocessor("The quick brown fox jumped.")
 
     # Tokenize and a batch of single sentences.
     preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
@@ -78,16 +74,16 @@
     first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
     second = tf.constant(["The fox tripped.", "Oh look, a whale."])
     preprocessor((first, second))
     ```
 
     Mapping with `tf.data.Dataset`.
     ```python
-    preprocessor = keras_nlp.models.MistralPreprocessor.from_preset(
-        "mistral_base_en"
+    preprocessor = keras_nlp.models.LlamaPreprocessor.from_preset(
+        "llama_base_en"
     )
     first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
     second = tf.constant(["The fox tripped.", "Oh look, a whale."])
     label = tf.constant([1, 1])
 
     # Map labeled single sentences.
     ds = tf.data.Dataset.from_tensor_slices((first, label))
@@ -109,14 +105,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = LlamaTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=1024,
         add_start_token=True,
         add_end_token=False,
         **kwargs,
@@ -156,16 +154,16 @@
         y=None,
         sample_weight=None,
         sequence_length=None,
     ):
         x = convert_inputs_to_list_of_tensor_segments(x)
         if len(x) != 1:
             raise ValueError(
-                "Mistral requires each input feature to contain only "
-                f"one segment, but received {len(x)}. If you are using Mistral"
+                "Llama requires each input feature to contain only "
+                f"one segment, but received {len(x)}. If you are using Llama"
                 " for a multi-segment classification task, please refer to "
                 "classification models like BERT or RoBERTa."
             )
         sequence_length = sequence_length or self.sequence_length
         token_ids, padding_mask = self.packer(
             self.tokenizer(x[0]),
             sequence_length=sequence_length,
@@ -185,15 +183,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return MistralTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_presets.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,9 +31,19 @@
             "params": 7241732096,
             "official_name": "Mistral",
             "path": "mistral",
             "model_card": "https://github.com/mistralai/mistral-src/blob/main/README.md",
         },
         "kaggle_handle": "kaggle://keras/mistral/keras/mistral_instruct_7b_en/6",
     },
+    "mistral_0.2_instruct_7b_en": {
+        "metadata": {
+            "description": "Mistral 7B instruct Version 0.2 model",
+            "params": 7241732096,
+            "official_name": "Mistral",
+            "path": "mistral",
+            "model_card": "https://github.com/mistralai/mistral-src/blob/main/README.md",
+        },
+        "kaggle_handle": "kaggle://keras/mistral/keras/mistral_0.2_instruct_7b_en/1",
+    },
 }
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.mistral.mistral_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.MistralTokenizer")
 class MistralTokenizer(SentencePieceTokenizer):
     """Mistral tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -45,15 +42,15 @@
             [SentencePiece repository](https://github.com/google/sentencepiece)
             for more details on the format.
 
     Examples:
     ```python
     # Unbatched input.
     tokenizer = keras_nlp.models.MistralTokenizer.from_preset(
-        "mistral_base_en",
+        "mistral_7b_en",
     )
     tokenizer("The quick brown fox jumped.")
 
     # Batched input.
     tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
@@ -78,11 +75,7 @@
                     )
             self.start_token_id = self.token_to_id(self.start_token)
             self.end_token_id = self.token_to_id(self.end_token)
         else:
             self.start_token_id = None
             self.end_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/mistral/mistral_transformer_decoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/mistral/mistral_transformer_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             dtype=self.dtype_policy,
             name="feedforward_intermediate_dense",
         )
         self._feedforward_intermediate_dense.build(decoder_sequence_shape)
 
         self._feedforward_gate_dense = keras.layers.Dense(
             self.intermediate_dim,
-            activation=self.activation,
             kernel_initializer=clone_initializer(self.kernel_initializer),
             use_bias=False,
             dtype=self.dtype_policy,
             name="feedforward_gate_dense",
         )
         self._feedforward_gate_dense.build(decoder_sequence_shape)
 
@@ -168,14 +167,25 @@
 
         x = x + residual
         residual = x
 
         x = self._feedforward_layernorm(x)
         gate_output = self._feedforward_gate_dense(x)
 
+        # Note that we run the activation function in full 32-bit
+        # precision since this is what `torch.nn.functional.silu`
+        # does. Internally, `torch.nn.functional.silu` converts the
+        # inputs to float32, computes SiLU, and converts the outputs
+        # back to compute dtype.
+        # CPU Kernel: https://github.com/pytorch/pytorch/blob/35c493f2cf9b623bfdc7e6b34dc1cb39690a7919/aten/src/ATen/native/cpu/Activation.cpp#L1221-L1235  # noqa: E501
+        # CUDA Kernel: https://github.com/pytorch/pytorch/blob/35c493f2cf9b623bfdc7e6b34dc1cb39690a7919/aten/src/ATen/native/cuda/ActivationSiluKernel.cu  # noqa: E501
+        gate_output = ops.cast(gate_output, "float32")
+        gate_output = self.activation(gate_output)
+        gate_output = ops.cast(gate_output, self.compute_dtype)
+
         x = self._feedforward_intermediate_dense(x)
 
         x = self._feedforward_output_dense(ops.multiply(x, gate_output))
 
         decoder_output = x + residual
 
         if self_attention_cache is not None:
@@ -203,25 +213,28 @@
 
         cache_update_index = (
             0
             if self_attention_cache_update_index is None
             else self_attention_cache_update_index
         )
 
-        # Mistral uses a banded attention mask
-        causal_mask_lower = compute_causal_mask(
+        # The lower traingular attention mask
+        causal_mask = compute_causal_mask(
             batch_size, input_length, output_length, cache_update_index
         )
-        # Below is a workaround for `ops.triu` for Keras 2.
-        # TODO(tirthasheshpatel): Use `ops.triu` once Keras 2 support is removed.
-        # causal_mask = ops.triu(causal_mask_lower, k=-self.sliding_window)
-        i = ops.arange(output_length)[:, None] + cache_update_index
-        j = ops.arange(input_length)[None, :]
-        causal_mask_upper = ops.cast(i < j + self.sliding_window, "int32")
-        causal_mask = ops.minimum(causal_mask_lower, causal_mask_upper)
+
+        # Mistral uses a banded attention mask if sliding window is not None
+        if self.sliding_window is not None:
+            # Below is a workaround for `ops.triu` for Keras 2.
+            # TODO(tirthasheshpatel): Use `ops.triu` once Keras 2 support is removed.
+            # causal_mask = ops.triu(causal_mask, k=-self.sliding_window)
+            i = ops.arange(output_length)[:, None] + cache_update_index
+            j = ops.arange(input_length)[None, :]
+            causal_mask_upper = ops.cast(i < j + self.sliding_window, "int32")
+            causal_mask = ops.minimum(causal_mask, causal_mask_upper)
 
         return (
             ops.minimum(decoder_mask, causal_mask)
             if decoder_mask is not None
             else causal_mask
         )
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_backbone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,86 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
-from keras_nlp.src.layers.modeling.transformer_decoder import TransformerDecoder
+from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.opt.opt_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-def opt_kernel_initializer(stddev=0.02):
+def roberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras_nlp_export("keras_nlp.models.OPTBackbone")
-class OPTBackbone(Backbone):
-    """An OPT decoder network.
-
-    This class implements a Transformer-based decoder model as described in
-    ["OPT: Open Pre-trained Transformer Language Models"](https://arxiv.org/abs/2205.01068).
-    The default constructor gives a fully customizable, randomly initialized OPT
-    model with any number of layers, heads, and embedding dimensions. To load
-    preset architectures and weights, use the `from_preset()` constructor.
+@keras_nlp_export("keras_nlp.models.RobertaBackbone")
+class RobertaBackbone(Backbone):
+    """A RoBERTa encoder network.
+
+    This network implements a bi-directional Transformer-based encoder as
+    described in ["RoBERTa: A Robustly Optimized BERT Pretraining Approach"](https://arxiv.org/abs/1907.11692).
+    It includes the embedding lookups and transformer layers, but does not
+    include the masked language model head used during pretraining.
+
+    The default constructor gives a fully customizable, randomly initialized
+    RoBERTa encoder with any number of layers, heads, and embedding
+    dimensions. To load preset architectures and weights, use the `from_preset()`
+    constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
-    [here](https://github.com/facebookresearch/fairseq/).
+    [here](https://github.com/facebookresearch/fairseq).
 
     Args:
         vocabulary_size: int. The size of the token vocabulary.
-        num_layers: int. The number of transformer decoder layers.
+        num_layers: int. The number of transformer layers.
         num_heads: int. The number of attention heads for each transformer.
             The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The hidden size of the transformer decoder layers.
+        hidden_dim: int. The size of the transformer encoding layer.
         intermediate_dim: int. The output dimension of the first Dense layer in
-            a two-layer feedforward network for each transformer decoder layer.
-        dropout: float. Dropout probability for the Transformer decoder.
-        max_sequence_length: int. The maximum sequence length that this decoder
-            can consume. If `None`, `max_sequence_length` uses the value from
-            sequence length. This determines the variable shape for positional
-            embeddings.
+            a two-layer feedforward network for each transformer.
+        dropout: float. Dropout probability for the Transformer encoder.
+        max_sequence_length: int. The maximum sequence length this encoder can
+            consume. The sequence length of the input must be less than
+            `max_sequence_length` default value. This determines the variable
+            shape for positional embeddings.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
             for model computations and weights. Note that some computations,
             such as softmax and layer normalization, will always be done at
             float32 precision regardless of dtype.
 
     Examples:
     ```python
     input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
-        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
+        "padding_mask": np.array(
+            [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
     }
 
-    # Pretrained OPT decoder
-    model = keras_nlp.models.OPTBackbone.from_preset("opt_125m_en")
+    # Pretrained RoBERTa encoder
+    model = keras_nlp.models.RobertaBackbone.from_preset("roberta_base_en")
     model(input_data)
 
-    # Randomly initialized OPT decoder model with a custom config
-    model = keras_nlp.models.OPTBackbone(
+    # Randomly initialized RoBERTa model with custom config
+    model = keras_nlp.models.RobertaBackbone(
         vocabulary_size=50265,
         num_layers=4,
         num_heads=4,
         hidden_dim=256,
         intermediate_dim=512,
         max_sequence_length=128,
     )
@@ -90,86 +92,93 @@
         self,
         vocabulary_size,
         num_layers,
         num_heads,
         hidden_dim,
         intermediate_dim,
         dropout=0.1,
-        max_sequence_length=2048,
+        max_sequence_length=512,
         dtype=None,
         **kwargs,
     ):
         # === Layers ===
         self.embeddings = TokenAndPositionEmbedding(
             vocabulary_size=vocabulary_size,
             sequence_length=max_sequence_length,
             embedding_dim=hidden_dim,
-            embeddings_initializer=opt_kernel_initializer(),
+            embeddings_initializer=roberta_kernel_initializer(),
             dtype=dtype,
             name="embeddings",
         )
         self.token_embedding = self.embeddings.token_embedding
+        self.embeddings_layer_norm = keras.layers.LayerNormalization(
+            axis=-1,
+            epsilon=1e-5,  # Original paper uses this epsilon value
+            dtype=dtype,
+            name="embeddings_layer_norm",
+        )
+        self.embeddings_dropout = keras.layers.Dropout(
+            dropout,
+            dtype=dtype,
+            name="embeddings_dropout",
+        )
         self.transformer_layers = []
         for i in range(num_layers):
-            layer = TransformerDecoder(
-                intermediate_dim=intermediate_dim,
+            layer = TransformerEncoder(
                 num_heads=num_heads,
+                intermediate_dim=intermediate_dim,
+                activation="gelu",
                 dropout=dropout,
-                activation="relu",
                 layer_norm_epsilon=1e-5,
-                normalize_first=True,
-                kernel_initializer=opt_kernel_initializer(),
+                kernel_initializer=roberta_kernel_initializer(),
                 dtype=dtype,
                 name=f"transformer_layer_{i}",
             )
             self.transformer_layers.append(layer)
-        self.layer_norm = keras.layers.LayerNormalization(
-            axis=-1,
-            epsilon=1e-5,
-            dtype=dtype,
-            name="layer_norm",
-        )
 
         # === Functional Model ===
         token_id_input = keras.Input(
             shape=(None,), dtype="int32", name="token_ids"
         )
         padding_mask_input = keras.Input(
             shape=(None,), dtype="int32", name="padding_mask"
         )
         x = self.embeddings(token_id_input)
+        x = self.embeddings_layer_norm(x)
+        x = self.embeddings_dropout(x)
         for transformer_layer in self.transformer_layers:
-            x = transformer_layer(x, decoder_padding_mask=padding_mask_input)
-        x = self.layer_norm(x)
+            x = transformer_layer(x, padding_mask=padding_mask_input)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
             outputs=x,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
         self.max_sequence_length = max_sequence_length
+        self.start_token_index = 0
 
     def get_config(self):
-        return {
-            "vocabulary_size": self.vocabulary_size,
-            "num_layers": self.num_layers,
-            "num_heads": self.num_heads,
-            "hidden_dim": self.hidden_dim,
-            "intermediate_dim": self.intermediate_dim,
-            "dropout": self.dropout,
-            "max_sequence_length": self.max_sequence_length,
-        }
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+        config = super().get_config()
+        config.update(
+            {
+                "vocabulary_size": self.vocabulary_size,
+                "num_layers": self.num_layers,
+                "num_heads": self.num_heads,
+                "hidden_dim": self.hidden_dim,
+                "intermediate_dim": self.intermediate_dim,
+                "dropout": self.dropout,
+                "max_sequence_length": self.max_sequence_length,
+            }
+        )
+        return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_causal_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/llama/llama_causal_lm.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,263 +7,149 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
-from keras_nlp.src.models.generative_task import GenerativeTask
-from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
-from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
-    OPTCausalLMPreprocessor,
+from keras_nlp.src.models.causal_lm import CausalLM
+from keras_nlp.src.models.llama.llama_backbone import LlamaBackbone
+from keras_nlp.src.models.llama.llama_causal_lm_preprocessor import (
+    LlamaCausalLMPreprocessor,
 )
-from keras_nlp.src.models.opt.opt_presets import backbone_presets
 from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
-@keras_nlp_export("keras_nlp.models.OPTCausalLM")
-class OPTCausalLM(GenerativeTask):
-    """An end-to-end OPT model for causal language modeling.
+@keras_nlp_export("keras_nlp.models.LlamaCausalLM")
+class LlamaCausalLM(CausalLM):
+    """An end-to-end Llama model for causal language modeling.
 
     A causal language model (LM) predicts the next token based on previous
     tokens. This task setup can be used to train the model unsupervised on
     plain text input, or to autoregressively generate plain text similar to
     the data used for training. This task can be used for pre-training or
-    fine-tuning a GPT-2 model, simply by calling `fit()`.
+    fine-tuning a LLaMA model, simply by calling `fit()`.
 
     This model has a `generate()` method, which generates text based on a
     prompt. The generation strategy used is controlled by an additional
     `sampler` argument on `compile()`. You can recompile the model with
     different `keras_nlp.samplers` objects to control the generation. By
     default, `"top_k"` sampling will be used.
 
-    This model can optionally be configured with a `preprocessor` layer, in
-    which case it will automatically apply preprocessing to string inputs during
-    `fit()`, `predict()`, `evaluate()` and `generate()`. This is done by default
-    when creating the model with `from_preset()`.
-
-    Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available
-    [here](https://github.com/facebookresearch/fairseq/).
-
     Args:
-        backbone: A `keras_nlp.models.OPTBackbone` instance.
-        preprocessor: A `keras_nlp.models.OPTCausalLMPreprocessor` or `None`.
+        backbone: A `keras_nlp.models.LlamaBackbone` instance.
+        preprocessor: A `keras_nlp.models.LlamaCausalLMPreprocessor` or `None`.
             If `None`, this model will not apply preprocessing, and inputs
             should be preprocessed before calling the model.
-
-    Examples:
-
-    Use `generate()` to do text generation.
-    ```python
-    opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
-    opt_lm.generate("I want to say", max_length=30)
-
-    # Generate with batched prompts.
-    opt_lm.generate(["This is a", "Where are you"], max_length=30)
-    ```
-
-    Compile the `generate()` function with a custom sampler.
-    ```python
-    opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
-    opt_lm.compile(sampler="greedy")
-    opt_lm.generate("I want to say", max_length=30)
-
-    opt_lm.compile(sampler=keras_nlp.samplers.BeamSampler(num_beams=2))
-    opt_lm.generate("I want to say", max_length=30)
-    ```
-
-    Use `generate()` without preprocessing.
-    ```python
-    # Prompt the model with `5338, 318` (the token ids for `"Who is"`).
-    # Use `"padding_mask"` to indicate values that should not be overridden.
-    prompt = {
-        "token_ids": np.array([[5338, 318, 0, 0, 0]] * 2),
-        "padding_mask": np.array([[1, 1, 0, 0, 0]] * 2),
-    }
-
-    opt_lm = keras_nlp.models.OPTCausalLM.from_preset(
-        "opt_125m_en",
-        preprocessor=None,
-    )
-    opt_lm.generate(prompt)
-    ```
-
-    Call `fit()` on a single batch.
-    ```python
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
-    opt_lm.fit(x=features, batch_size=2)
-    ```
-
-    Call `fit()` without preprocessing.
-    ```python
-    x = {
-        "token_ids": np.array([[1, 2, 3, 4, 5]] * 2),
-        "padding_mask": np.array([[1, 1, 1, 1, 1]] * 2),
-    }
-    y = np.array([[2, 3, 4, 5, 0]] * 2)
-    sw = np.array([[1, 1, 1, 1, 1]] * 2)
-
-    opt_lm = keras_nlp.models.OPTCausalLM.from_preset(
-        "opt_base_en",
-        preprocessor=None,
-    )
-    opt_lm.fit(x=x, y=y, sample_weight=sw, batch_size=2)
-    ```
-
-    Custom backbone and vocabulary.
-    ```python
-    features = ["a quick fox.", "a fox quick."]
-    vocab = {"<|endoftext|>": 0, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    merges += ["Ġ f", "o x", "Ġf ox"]
-
-    tokenizer = keras_nlp.models.OPTTokenizer(
-        vocabulary=vocab,
-        merges=merges,
-    )
-    preprocessor = keras_nlp.models.OPTCausalLMPreprocessor(
-        tokenizer=tokenizer,
-        sequence_length=128,
-    )
-    model = keras_nlp.models.OPTBackbone(
-        vocabulary_size=50265,
-        num_layers=4,
-        num_heads=4,
-        hidden_dim=256,
-        intermediate_dim=512,
-        max_sequence_length=128,
-    )
-    opt_lm = keras_nlp.models.OPTCausalLM(
-        backbone=backbone,
-        preprocessor=preprocessor,
-    )
-    opt_lm.fit(x=features, batch_size=2)
-    ```
     """
 
-    def __init__(
-        self,
-        backbone,
-        preprocessor=None,
-        **kwargs,
-    ):
+    def __init__(self, backbone, preprocessor=None, **kwargs):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
 
         # === Functional Model ===
-        inputs = backbone.input
+        inputs = backbone.inputs
         hidden_states = backbone(inputs)
         outputs = backbone.token_embedding(hidden_states, reverse=True)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
     @classproperty
     def backbone_cls(cls):
-        return OPTBackbone
+        return LlamaBackbone
 
     @classproperty
     def preprocessor_cls(cls):
-        return OPTCausalLMPreprocessor
+        return LlamaCausalLMPreprocessor
 
     def call_with_cache(
         self,
         token_ids,
         cache,
         cache_update_index,
     ):
-        """Forward pass of `OPTCausalLM` with cache.
+        """Forward pass of `LlamaCausalLM` with cache.
 
         `call_with_cache` adds an additional forward pass for the model for
         autoregressive inference. Unlike calling the model directly, this method
         allows caching previous key/value Tensors in multi-head attention layer,
         and avoids recomputing the outputs of seen tokens.
 
         Args:
             token_ids: a dense int Tensor with shape `(batch_size, max_length)`.
             cache: a dense float Tensor, the cache of key and value.
-            cache_update_index: int, or int Tensor. The index of current inputs in the
-                whole sequence.
+            cache_update_index: int, or int Tensor. The index of current inputs
+            in the whole sequence.
 
         Returns:
             A (logits, hidden_states, cache) tuple. Where `logits` is the
             language model logits for the input token_ids, `hidden_states` is
             the final hidden representation of the input tokens, and `cache` is
             the decoding cache.
         """
-        x = self.backbone.embeddings(token_ids, start_index=cache_update_index)
+        x = self.backbone.token_embedding(token_ids)
         # Each decoder layer has a cache; we update them separately.
-        caches = []
-        for i, transformer_layer in enumerate(self.backbone.transformer_layers):
+        updated_cache = []
+        for i in range(self.backbone.num_layers):
             current_cache = cache[:, i, ...]
-            x, next_cache = transformer_layer(
+            x, next_cache = self.backbone.transformer_layers[i](
                 x,
                 self_attention_cache=current_cache,
                 self_attention_cache_update_index=cache_update_index,
             )
-            caches.append(next_cache)
-        cache = ops.stack(caches, axis=1)
-        x = self.backbone.layer_norm(x)
-        hidden_states = x
-        logits = self.backbone.token_embedding(hidden_states, reverse=True)
+            updated_cache.append(next_cache)
+        cache = ops.stack(updated_cache, axis=1)
+        hidden_states = x = self.backbone.layer_norm(x)
+        logits = self.backbone.token_embedding(x, reverse=True)
         return logits, hidden_states, cache
 
     def _build_cache(self, token_ids):
         """Build an empty cache for use with `call_with_cache()`."""
         batch_size = ops.shape(token_ids)[0]
         max_length = ops.shape(token_ids)[1]
         num_layers = self.backbone.num_layers
-        num_heads = self.backbone.num_heads
-        head_dim = self.backbone.hidden_dim // self.backbone.num_heads
-        shape = [batch_size, num_layers, 2, max_length, num_heads, head_dim]
+        num_key_value_heads = self.backbone.num_key_value_heads
+        head_dim = self.backbone.hidden_dim // self.backbone.num_query_heads
+        shape = [
+            batch_size,
+            num_layers,
+            2,
+            max_length,
+            num_key_value_heads,
+            head_dim,
+        ]
         cache = ops.zeros(shape, dtype=self.compute_dtype)
         # Seed the cache.
         _, hidden_states, cache = self.call_with_cache(token_ids, cache, 0)
         return hidden_states, cache
 
     def generate_step(
         self,
         inputs,
-        end_token_id=None,
+        stop_token_ids=None,
     ):
         """A compilable generation function for a single batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
         for a single batch of inputs. Inputs should have the same structure as
         model inputs, a dictionary with keys `"token_ids"` and `"padding_mask"`.
 
         Args:
             inputs: A dictionary with two keys `"token_ids"` and
                 `"padding_mask"` and batched tensor values.
-            end_token_id: The id of the end token to stop on. If all
-                sequences have produced a new `end_token_id`, generation
+            stop_token_ids: Tuple of id's of the end token to stop on. If all
+                sequences have produced a new stop token, generation
                 will stop.
         """
         token_ids, padding_mask = inputs["token_ids"], inputs["padding_mask"]
         # Create and seed cache with a single forward pass.
         hidden_states, cache = self._build_cache(token_ids)
         # Compute the lengths of all user inputted tokens ids.
         row_lengths = ops.sum(ops.cast(padding_mask, "int32"), axis=-1)
@@ -282,31 +168,31 @@
             )
             return (
                 ops.squeeze(logits, axis=1),
                 ops.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        token_ids = self._sampler(
+        token_ids = self.sampler(
             next=next,
             prompt=token_ids,
             cache=cache,
             index=index,
             mask=padding_mask,
-            end_token_id=end_token_id,
+            stop_token_ids=stop_token_ids,
             hidden_states=hidden_states,
             model=self,
         )
 
         # Compute an output padding mask with the token ids we updated.
-        if end_token_id is not None:
-            # Build a mask of `end_token_id` locations not in the original
+        if stop_token_ids is not None:
+            # Build a mask of stop token locations not in the original
             # prompt (not in locations where `padding_mask` is True).
             end_locations = ops.logical_and(
-                ops.equal(token_ids, end_token_id),
+                any_equal(token_ids, stop_token_ids),
                 ops.logical_not(padding_mask),
             )
             end_locations = ops.cast(end_locations, "int32")
             # Use cumsum to get ones in all locations after end_locations.
             cumsum = ops.cast(ops.cumsum(end_locations, axis=-1), "int32")
             overflow = cumsum - end_locations
             # Our padding mask is the inverse of these overflow locations.
@@ -315,7 +201,134 @@
             # Without early stopping, all locations will have been updated.
             padding_mask = ops.ones_like(token_ids, dtype="bool")
         return {
             "token_ids": token_ids,
             "padding_mask": padding_mask,
         }
 
+    def score(
+        self,
+        token_ids,
+        padding_mask=None,
+        scoring_mode="logits",
+        layer_intercept_fn=None,
+        target_ids=None,
+    ):
+        """Score a generation represented by the provided token ids.
+
+        Args:
+            token_ids: A <int>[batch_size, num_tokens] tensor containing tokens
+                to score. Typically, this tensor captures the output from a call
+                to `LlamaCausalLM.generate()`, i.e., tokens for both the input
+                text and the model-generated text.
+            padding_mask: A <bool>[batch_size, num_tokens] tensor indicating the
+                tokens that should be preserved during generation. This is an
+                artifact required by the `LlamaBackbone` and isn't influential
+                on the computation of this function. If omitted, this function
+                uses `keras.ops.ones()` to create a tensor of the appropriate
+                shape.
+            scoring_mode: The type of scores to return, either "logits" or
+                "loss", both will be per input token.
+            layer_intercept_fn: An optional function for augmenting activations
+                with additional computation, for example, as part of
+                interpretability research. This function will be passed the
+                activations as its first parameter and a numeric index
+                associated with that backbone layer. _This index _is not_ an
+                index into `self.backbone.layers`_. The index -1 accompanies the
+                embeddings returned by calling `self.backbone.token_embedding()`
+                on `token_ids` in the forward direction. All subsequent indexes
+                will be 0-based indices for the activations returned by each of
+                the Transformers layers in the backbone. This function must
+                return a <float>[batch_size, num_tokens, hidden_dims] tensor
+                that can be passed as an input to the next layer in the model.
+            target_ids: An <bool>[batch_size, num_tokens] tensor containing the
+                predicted tokens against which the loss should be computed. If a
+                span of tokens is provided (sequential truthy values along
+                axis=1 in the tensor), the loss will be computed as the
+                aggregate across those tokens.
+
+        Raises:
+            ValueError: If an unsupported scoring_mode is provided, or if the
+                target_ids are not provided when using ScoringMode.LOSS.
+
+        Returns:
+            The per-token scores as a tensor of size
+            <float>[batch_size, num_tokens, vocab_size] in "logits" mode, or
+            <float>[batch_size, num_tokens] in "loss" mode.
+
+        Example:
+
+        Compute gradients between embeddings and loss scores with TensorFlow:
+        ```python
+        llama_lm = keras_nlp.models.LlamaCausalLM.from_preset("llama2_7b_en")
+        generations = llama_lm.generate(
+            ["This is a", "Where are you"],
+            max_length=30
+        )
+        preprocessed = llama_lm.preprocessor.generate_preprocess(generations)
+        generation_ids = preprocessed["token_ids"]
+        padding_mask = preprocessed["padding_mask"]
+        target_ids = keras.ops.roll(generation_ids, shift=-1, axis=1)
+
+        embeddings = None
+        with tf.GradientTape(watch_accessed_variables=True) as tape:
+            def layer_intercept_fn(x, i):
+                if i == -1:
+                    nonlocal embeddings, tape
+                    embeddings = x
+                    tape.watch(embeddings)
+                return x
+
+            losses = llama_lm.score(
+                token_ids=generation_ids,
+                padding_mask=padding_mask,
+                scoring_mode="loss",
+                layer_intercept_fn=layer_intercept_fn,
+                target_ids=target_ids,
+            )
+
+        grads = tape.gradient(losses, embeddings)
+        ```
+        """
+        if scoring_mode not in ("logits", "loss"):
+            raise ValueError(
+                "Unsupported scoring_mode. Must be one of 'logits' or 'loss'."
+            )
+
+        if scoring_mode == "loss" and target_ids is None:
+            raise ValueError(
+                "Cannot compute loss without targets. Please provide target "
+                "token ids via the target_ids parameter."
+            )
+
+        batch_shape = ops.shape(token_ids)[:2]
+        assert len(batch_shape) == 2
+
+        if padding_mask is None:
+            padding_mask = ops.ones(shape=batch_shape)
+
+        if layer_intercept_fn is None:
+
+            def default_layer_intercept_fn(x, unused_i):
+                return x
+
+            layer_intercept_fn = default_layer_intercept_fn
+
+        token_embeddings = self.backbone.token_embedding(token_ids)
+        x = layer_intercept_fn(token_embeddings, -1)
+
+        for i, transformer_layer in enumerate(self.backbone.transformer_layers):
+            x = transformer_layer(x, decoder_padding_mask=padding_mask)
+            x = layer_intercept_fn(x, i)
+
+        x = self.backbone.layer_norm(x)
+        logits = self.backbone.token_embedding(x, reverse=True)
+
+        if scoring_mode == "logits":
+            return logits
+
+        per_token_loss_fn = keras.losses.SparseCategoricalCrossentropy(
+            from_logits=True, reduction="none"
+        )
+        per_token_loss = per_token_loss_fn(target_ids, logits)
+        return per_token_loss
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     def generate_preprocess(
         self,
         x,
         sequence_length=None,
     ):
-        """Covert strings to integer token input for generation.
+        """Convert strings to integer token input for generation.
 
         Similar to calling the layer for training, this method takes in strings
         or tensor strings, tokenizes and packs the input, and computes a padding
         mask masking all inputs not filled in with a padded value.
 
         Unlike calling the layer for training, this method does not compute
         labels and will never append a `tokenizer.end_token_id` to the end of
@@ -156,15 +156,15 @@
             "padding_mask": padding_mask,
         }
 
     def generate_postprocess(
         self,
         x,
     ):
-        """Covert integer token output to strings for generation.
+        """Convert integer token output to strings for generation.
 
         This method reverses `generate_preprocess()`, by first removing all
         padding and start/end tokens, and then converting the integer sequence
         back to a string.
         """
         if not self.built:
             self.build(None)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
-from keras_nlp.src.models.opt.opt_presets import backbone_presets
 from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.OPTPreprocessor")
 class OPTPreprocessor(Preprocessor):
     """OPT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
@@ -105,14 +102,16 @@
 
     # Map unlabeled single sentences.
     ds = tf.data.Dataset.from_tensor_slices(text)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
+    tokenizer_cls = OPTTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=2048,
         add_start_token=True,
         add_end_token=True,
         **kwargs,
@@ -183,15 +182,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classproperty
-    def tokenizer_cls(cls):
-        return OPTTokenizer
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/opt/opt_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/opt/opt_tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.opt.opt_presets import backbone_presets
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.OPTTokenizer")
 class OPTTokenizer(BytePairTokenizer):
     """An OPT tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -106,18 +103,14 @@
             self.pad_token_id = self.token_to_id(self.pad_token)
             self.end_token_id = self.token_to_id(self.end_token)
         else:
             self.start_token_id = None
             self.pad_token_id = None
             self.end_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_backbone.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,183 +8,164 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.layers.modeling.token_and_position_embedding import (
-    TokenAndPositionEmbedding,
-)
-from keras_nlp.src.layers.modeling.transformer_encoder import TransformerEncoder
+from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
-from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.bloom.bloom_decoder import BloomDecoder
 
 
-def roberta_kernel_initializer(stddev=0.02):
-    return keras.initializers.TruncatedNormal(stddev=stddev)
+def _bloom_kernel_initializer(stddev=0.02):
+    return keras.initializers.RandomNormal(stddev=stddev)
 
 
-@keras_nlp_export("keras_nlp.models.RobertaBackbone")
-class RobertaBackbone(Backbone):
-    """A RoBERTa encoder network.
+@keras_nlp_export("keras_nlp.models.BloomBackbone")
+class BloomBackbone(Backbone):
+    """A BLOOM decoder network.
 
-    This network implements a bi-directional Transformer-based encoder as
-    described in ["RoBERTa: A Robustly Optimized BERT Pretraining Approach"](https://arxiv.org/abs/1907.11692).
-    It includes the embedding lookups and transformer layers, but does not
-    include the masked language model head used during pretraining.
+    This network implements a Transformer-based decoder network, BigScience
+    Language Open-science Open-access Multilingual (BLOOM), as descriped in
+    ["BLOOM: A 176B-Parameter Open-Access Multilingual Language Model"](https://arxiv.org/pdf/2211.05100.pdf).
 
     The default constructor gives a fully customizable, randomly initialized
-    RoBERTa encoder with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset()`
-    constructor.
+    Bloom model with any number of layers, heads, and embedding dimensions. To
+    load preset architectures and weights, use the `from_preset()` constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available
-    [here](https://github.com/facebookresearch/fairseq).
+    third party and subject to a separate license, available [here](https://huggingface.co/spaces/bigscience/license).
 
     Args:
         vocabulary_size: int. The size of the token vocabulary.
         num_layers: int. The number of transformer layers.
         num_heads: int. The number of attention heads for each transformer.
             The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The size of the transformer encoding layer.
+        hidden_dim: int. The dimensionality of the embeddings and hidden states.
         intermediate_dim: int. The output dimension of the first Dense layer in
-            a two-layer feedforward network for each transformer.
-        dropout: float. Dropout probability for the Transformer encoder.
-        max_sequence_length: int. The maximum sequence length this encoder can
-            consume. The sequence length of the input must be less than
-            `max_sequence_length` default value. This determines the variable
-            shape for positional embeddings.
+            the MLP network of each transformer.
+        dropout: float. Dropout probability for the Transformer decoder.
+        layer_norm_epsilon: float. Epsilon for the layer normalization layers in
+            the transformer decoder.
         dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
             for model computations and weights. Note that some computations,
             such as softmax and layer normalization, will always be done at
             float32 precision regardless of dtype.
 
-    Examples:
+    Example:
     ```python
     input_data = {
         "token_ids": np.ones(shape=(1, 12), dtype="int32"),
-        "padding_mask": np.array(
-            [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
+        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]]),
     }
 
-    # Pretrained RoBERTa encoder
-    model = keras_nlp.models.RobertaBackbone.from_preset("roberta_base_en")
+    # Pretrained BLOOM decoder.
+    model = keras_nlp.models.BloomBackbone.from_preset("bloom_560m_multi")
     model(input_data)
 
-    # Randomly initialized RoBERTa model with custom config
-    model = keras_nlp.models.RobertaBackbone(
-        vocabulary_size=50265,
-        num_layers=4,
-        num_heads=4,
-        hidden_dim=256,
-        intermediate_dim=512,
-        max_sequence_length=128,
+    # Randomly initialized BLOOM decoder with a custom config.
+    model = keras_nlp.models.BloomBackbone(
+        vocabulary_size=10,
+        num_layers=2,
+        num_heads=2,
+        hidden_dim=32,
+        intermediate_dim=32*4,
+        dropout=0.0,
+        layer_norm_epsilon=1e-5,
     )
     model(input_data)
     ```
+
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
         num_heads,
         hidden_dim,
         intermediate_dim,
-        dropout=0.1,
-        max_sequence_length=512,
+        dropout=0.0,
+        layer_norm_epsilon=1e-5,
         dtype=None,
         **kwargs,
     ):
         # === Layers ===
-        self.embeddings = TokenAndPositionEmbedding(
-            vocabulary_size=vocabulary_size,
-            sequence_length=max_sequence_length,
-            embedding_dim=hidden_dim,
-            embeddings_initializer=roberta_kernel_initializer(),
+        self.token_embedding = ReversibleEmbedding(
+            input_dim=vocabulary_size,
+            output_dim=hidden_dim,
+            embeddings_initializer=_bloom_kernel_initializer(stddev=0.02),
             dtype=dtype,
-            name="embeddings",
+            name="token_embedding",
         )
-        self.token_embedding = self.embeddings.token_embedding
         self.embeddings_layer_norm = keras.layers.LayerNormalization(
-            axis=-1,
-            epsilon=1e-5,  # Original paper uses this epsilon value
-            dtype=dtype,
-            name="embeddings_layer_norm",
-        )
-        self.embeddings_dropout = keras.layers.Dropout(
-            dropout,
+            epsilon=layer_norm_epsilon,
             dtype=dtype,
-            name="embeddings_dropout",
+            name="token_embedding_layernorm",
         )
         self.transformer_layers = []
         for i in range(num_layers):
-            layer = TransformerEncoder(
+            layer = BloomDecoder(
                 num_heads=num_heads,
                 intermediate_dim=intermediate_dim,
-                activation="gelu",
                 dropout=dropout,
-                layer_norm_epsilon=1e-5,
-                kernel_initializer=roberta_kernel_initializer(),
+                layer_norm_epsilon=layer_norm_epsilon,
                 dtype=dtype,
                 name=f"transformer_layer_{i}",
             )
             self.transformer_layers.append(layer)
+        self.layer_norm = keras.layers.LayerNormalization(
+            epsilon=layer_norm_epsilon,
+            dtype=dtype,
+            name="final_layernorm",
+        )
 
         # === Functional Model ===
         token_id_input = keras.Input(
             shape=(None,), dtype="int32", name="token_ids"
         )
         padding_mask_input = keras.Input(
             shape=(None,), dtype="int32", name="padding_mask"
         )
-        x = self.embeddings(token_id_input)
+        x = self.token_embedding(token_id_input)
         x = self.embeddings_layer_norm(x)
-        x = self.embeddings_dropout(x)
         for transformer_layer in self.transformer_layers:
-            x = transformer_layer(x, padding_mask=padding_mask_input)
+            x = transformer_layer(x, decoder_padding_mask=padding_mask_input)
+        sequence_output = self.layer_norm(x)
         super().__init__(
             inputs={
                 "token_ids": token_id_input,
                 "padding_mask": padding_mask_input,
             },
-            outputs=x,
+            outputs=sequence_output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
-        self.max_sequence_length = max_sequence_length
-        self.start_token_index = 0
+        self.layer_norm_epsilon = layer_norm_epsilon
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "vocabulary_size": self.vocabulary_size,
                 "num_layers": self.num_layers,
                 "num_heads": self.num_heads,
                 "hidden_dim": self.hidden_dim,
                 "intermediate_dim": self.intermediate_dim,
                 "dropout": self.dropout,
-                "max_sequence_length": self.max_sequence_length,
+                "layer_norm_epsilon": self.layer_norm_epsilon,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
+from keras_nlp.src.models.classifier import Classifier
 from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
 from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.RobertaClassifier")
-class RobertaClassifier(Task):
+class RobertaClassifier(Classifier):
     """An end-to-end RoBERTa model for classification tasks.
 
     This model attaches a classification head to a
     `keras_nlp.model.RobertaBackbone` instance, mapping from the backbone
     outputs to logits suitable for a classification task. For usage of this
     model with pre-trained weights, see the `from_preset()` constructor.
 
@@ -130,14 +127,17 @@
         preprocessor=preprocessor,
         num_classes=4,
     )
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = RobertaBackbone
+    preprocessor_cls = RobertaPreprocessor
+
     def __init__(
         self,
         backbone,
         num_classes,
         preprocessor=None,
         activation=None,
         hidden_dim=None,
@@ -187,42 +187,19 @@
 
         # === Config ===
         self.num_classes = num_classes
         self.activation = keras.activations.get(activation)
         self.hidden_dim = hidden_dim
         self.dropout = dropout
 
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(2e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "activation": keras.activations.serialize(self.activation),
                 "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return RobertaBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return RobertaPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
-from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.masked_lm import MaskedLM
 from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
-    RobertaMaskedLMPreprocessor,
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+    XLMRobertaMaskedLMPreprocessor,
 )
-from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras_nlp_export("keras_nlp.models.RobertaMaskedLM")
-class RobertaMaskedLM(Task):
-    """An end-to-end RoBERTa model for the masked language modeling task.
+@keras_nlp_export("keras_nlp.models.XLMRobertaMaskedLM")
+class XLMRobertaMaskedLM(MaskedLM):
+    """An end-to-end XLM-RoBERTa model for the masked language modeling task.
 
-    This model will train RoBERTa on a masked language modeling task.
+    This model will train XLM-RoBERTa on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` method.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case inputs can be raw string features during `fit()`, `predict()`,
     and `evaluate()`. Inputs will be tokenized and dynamically masked during
@@ -44,30 +41,33 @@
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq).
 
     Args:
-        backbone: A `keras_nlp.models.RobertaBackbone` instance.
-        preprocessor: A `keras_nlp.models.RobertaMaskedLMPreprocessor` or
+        backbone: A `keras_nlp.models.XLMRobertaBackbone` instance.
+        preprocessor: A `keras_nlp.models.XLMRobertaMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
     Examples:
 
-    Raw string data.
+    Raw string inputs and pretrained backbone.
     ```python
+    # Create a dataset with raw string features. Labels are inferred.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
-    # Pretrained language model.
-    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
-        "roberta_base_en",
+    # Pretrained language model
+    # on an MLM task.
+    masked_lm = keras_nlp.models.XLMRobertaMaskedLM.from_preset(
+        "xlm_roberta_base_multi",
     )
     masked_lm.fit(x=features, batch_size=2)
+    ```
 
     # Re-compile (e.g., with a new learning rate).
     masked_lm.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
         optimizer=keras.optimizers.Adam(5e-5),
         jit_compile=True,
     )
@@ -84,23 +84,26 @@
         "token_ids": np.array([[1, 2, 0, 4, 0, 6, 7, 8]] * 2),
         "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1]] * 2),
         "mask_positions": np.array([[2, 4]] * 2)
     }
     # Labels are the original masked values.
     labels = [[3, 5]] * 2
 
-    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
-        "roberta_base_en",
+    masked_lm = keras_nlp.models.XLMRobertaMaskedLM.from_preset(
+        "xlm_roberta_base_multi",
         preprocessor=None,
     )
 
     masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = XLMRobertaBackbone
+    preprocessor_cls = XLMRobertaMaskedLMPreprocessor
+
     def __init__(
         self,
         backbone,
         preprocessor=None,
         **kwargs,
     ):
         # === Layers ===
@@ -128,27 +131,7 @@
         )
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
-
-    @classproperty
-    def backbone_cls(cls):
-        return RobertaBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return RobertaMaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
 from keras_nlp.src.models.preprocessor import Preprocessor
-from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
 from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.RobertaPreprocessor")
 class RobertaPreprocessor(Preprocessor):
     """A RoBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -129,14 +126,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = RobertaTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -187,15 +186,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return RobertaTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/roberta/roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/roberta/roberta_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,133 +8,138 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
+import io
+
+import tensorflow as tf
+
+try:
+    import sentencepiece as spm
+except ImportError:
+    spm = None
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
-
-
-@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
-class RobertaTokenizer(BytePairTokenizer):
-    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
-
-    This tokenizer class will tokenize raw strings into integer sequences and
-    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by RoBERTa
-    models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a RoBERTa preset.
-
-    This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.RobertaPreprocessor` layer for input
-    packing.
 
-    If input is a batch of strings (rank > 0), the layer will output a
-    `tf.RaggedTensor` where the last dimension of the output is ragged.
 
-    If input is a scalar string (rank == 0), the layer will output a dense
-    `tf.Tensor` with static shape `[None]`.
+@keras_nlp_export("keras_nlp.tokenizers.compute_sentence_piece_proto")
+def compute_sentence_piece_proto(
+    data,
+    vocabulary_size,
+    model_type="unigram",
+    proto_output_file=None,
+    lowercase=False,
+):
+    r"""A utility to train a SentencePiece vocabulary.
 
-    Args:
-        vocabulary: A dictionary mapping tokens to integer ids, or file path
-            to a json file containing the token to id mapping.
-        merges: A list of merge rules or a string file path, If passing a file
-            path. the file should have one merge rule per line. Every merge
-            rule contains merge entities separated by a space.
+    Trains a SentencePiece vocabulary from an input dataset or a list of
+    filenames.
 
-    Examples:
-    ```python
-    # Unbatched input.
-    tokenizer = keras_nlp.models.RobertaTokenizer.from_preset(
-        "roberta_base_en",
-    )
-    tokenizer("The quick brown fox jumped.")
+    If `data` is a list of filenames, the file format is required to be plain
+    text files, and the text will be read in line by line during training.
 
-    # Batched input.
-    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+    Args:
+        data: A `tf.data.Dataset`, or a list of filenames.
+        vocabulary_size: int. The maximum size of a vocabulary to be trained.
+        model_type: str. The model algorithm must be one of
+            `"unigram"`, `"bpe"`, `"word"` or `"char"`. Defaults to `"unigram"`.
+        proto_output_file: str. If provided it will be used
+            as model_file which is passed to model_writer.
+            If `None`, the model_file will be `io.BytesIO` object.
+            Defaults to `None`.
+        lowercase: bool. If True, the input text will be
+            lowercased before tokenization. Defaults to `False`.
+
+    Returns:
+        A `bytes` object with a serialized SentencePiece proto or
+        `None` if proto_output_file if provided.
 
-    # Detokenization.
-    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+    Examples:
 
-    # Custom vocabulary.
-    # Note: 'Ġ' is space
-    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    merges += ["Ġ f", "o x", "Ġf ox"]
-    tokenizer = keras_nlp.models.RobertaTokenizer(
-        vocabulary=vocab,
-        merges=merges
-    )
-    tokenizer(["a quick fox", "a fox quick"])
+    Basic Usage (from Dataset).
+    >>> inputs = tf.data.Dataset.from_tensor_slices(["Drifting Along"])
+    >>> proto = keras_nlp.tokenizers.compute_sentence_piece_proto(inputs, vocabulary_size=15)
+    >>> tokenizer = keras_nlp.tokenizers.SentencePieceTokenizer(proto=proto)
+    >>> outputs = inputs.map(tokenizer)
+    >>> for output in outputs:
+    ...     print(output)
+    tf.Tensor([ 4  8 12  5  9 14  5  6 13  4  7 10 11  6 13],
+    shape=(15,), dtype=int32)
+
+    Basic Usage (with files).
+    ``` python
+    with open("test.txt", "w+") as f: f.write("Drifting Along\n")
+    inputs = ["test.txt"]
+    proto = keras_nlp.tokenizers.compute_sentence_piece_proto(
+         inputs, vocabulary_size=15, proto_output_file="model.spm")
+    tokenizer = keras_nlp.tokenizers.SentencePieceTokenizer(proto="model.spm")
+    ds = tf.data.Dataset.from_tensor_slices(["the quick brown fox."])
+    ds = ds.map(tokenizer)
     ```
+
+    Usage with lowercase
+    >>> inputs = tf.data.Dataset.from_tensor_slices(["Drifting Along"])
+    >>> proto = keras_nlp.tokenizers.compute_sentence_piece_proto(
+    ...     inputs, vocabulary_size=15, lowercase=True)
+    >>> tokenizer = keras_nlp.tokenizers.SentencePieceTokenizer(proto=proto)
+    >>> outputs = inputs.map(tokenizer)
+    >>> for output in outputs:
+    ...     print(output)
+    tf.Tensor([ 4  8 12  5  9 14  5  6 13  4  7 10 11  6 13],
+    shape=(15,), dtype=int32)
     """
 
-    def __init__(
-        self,
-        vocabulary=None,
-        merges=None,
-        **kwargs,
-    ):
-        self.start_token = "<s>"
-        self.pad_token = "<pad>"
-        self.end_token = "</s>"
-        self.mask_token = "<mask>"
-
-        super().__init__(
-            vocabulary=vocabulary,
-            merges=merges,
-            unsplittable_tokens=[
-                self.start_token,
-                self.pad_token,
-                self.end_token,
-                self.mask_token,
-            ],
-            **kwargs,
+    if spm is None:
+        raise ImportError(
+            f"{compute_sentence_piece_proto.__name__} requires the "
+            "`sentencepiece` package. Please install it with "
+            "`pip install sentencepiece`."
+        )
+
+    if not isinstance(data, (list, tuple, tf.data.Dataset)):
+        raise ValueError(
+            "The `data` argument must be either `tf.data.Dataset` or `tuple` or `list`. "
+            f"Received: type(data)={type(data)}."
         )
 
-    def set_vocabulary_and_merges(self, vocabulary, merges):
-        super().set_vocabulary_and_merges(vocabulary, merges)
+    if model_type not in ["unigram", "bpe", "word", "char"]:
+        raise ValueError(
+            "The `model_type` argument must be one of `unigram`, `bpe`, `word`"
+            f"or `char`. Received: model_type={model_type}."
+        )
 
-        if vocabulary is not None:
-            # Check for necessary special tokens.
-            for token in [
-                self.start_token,
-                self.pad_token,
-                self.end_token,
-                self.mask_token,
-            ]:
-                if token not in self.vocabulary:
-                    raise ValueError(
-                        f"Cannot find token `'{token}'` in the provided "
-                        f"`vocabulary`. Please provide `'{token}'` in your "
-                        "`vocabulary` or use a pretrained `vocabulary` name."
-                    )
-
-            self.start_token_id = self.token_to_id(self.start_token)
-            self.pad_token_id = self.token_to_id(self.pad_token)
-            self.end_token_id = self.token_to_id(self.end_token)
-            self.mask_token_id = self.token_to_id(self.mask_token)
-        else:
-            self.start_token_id = None
-            self.pad_token_id = None
-            self.end_token_id = None
-            self.mask_token_id = None
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    def get_config(self):
-        config = super().get_config()
-        # In the constructor, we pass the list of special tokens to the
-        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
-        # delete it from the config here.
-        del config["unsplittable_tokens"]
-        return config
+    model_writer = (
+        open(proto_output_file, "wb") if proto_output_file else io.BytesIO()
+    )
+    is_dataset = isinstance(data, tf.data.Dataset)
+    if is_dataset:
+        spm.SentencePieceTrainer.train(
+            sentence_iterator=data.as_numpy_iterator(),
+            model_writer=model_writer,
+            vocab_size=vocabulary_size,
+            model_type=model_type,
+            normalization_rule_name="nmt_nfkc_cf" if lowercase else "nmt_nfkc",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+        )
+    else:
+        spm.SentencePieceTrainer.train(
+            input=data,
+            model_writer=model_writer,
+            vocab_size=vocabulary_size,
+            model_type=model_type,
+            normalization_rule_name="nmt_nfkc_cf" if lowercase else "nmt_nfkc",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+        )
+    if proto_output_file:
+        model_writer.close()
+    else:
+        return model_writer.getvalue()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_backbone.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,20 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.modeling.reversible_embedding import ReversibleEmbedding
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.t5.t5_layer_norm import T5LayerNorm
-from keras_nlp.src.models.t5.t5_presets import backbone_presets
 from keras_nlp.src.models.t5.t5_transformer_layer import T5TransformerLayer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
 class T5Backbone(Backbone):
     """T5 encoder-decoder backbone model.
 
     T5 is a LLM pretrained on a mix of unsupervised and supervised tasks,
@@ -219,14 +216,15 @@
                 "decoder_token_ids": decoder_token_id_input,
                 "decoder_padding_mask": decoder_padding_mask_input,
             },
             outputs={
                 "encoder_sequence_output": encoder_output,
                 "decoder_sequence_output": decoder_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
@@ -254,11 +252,7 @@
                 "use_gated_activation": self.use_gated_activation,
                 "layer_norm_epsilon": self.layer_norm_epsilon,
                 "tie_embedding_weights": self.tie_embedding_weights,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_tokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.t5.t5_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
 class T5Tokenizer(SentencePieceTokenizer):
     """T5 tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -96,11 +93,7 @@
             # T5 uses the same start token as end token, i.e., "<\s>".
             self.start_token_id = self.end_token_id
         else:
             self.end_token_id = None
             self.pad_token_id = None
             self.start_token_id = None
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/t5/t5_transformer_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/task.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,34 +12,62 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rich import console as rich_console
 from rich import markup
 from rich import table as rich_table
 
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import config
 from keras_nlp.src.backend import keras
+from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.utils.keras_utils import print_msg
 from keras_nlp.src.utils.pipeline_model import PipelineModel
-from keras_nlp.src.utils.preset_utils import check_preset_class
+from keras_nlp.src.utils.preset_utils import check_config_class
+from keras_nlp.src.utils.preset_utils import list_presets
+from keras_nlp.src.utils.preset_utils import list_subclasses
 from keras_nlp.src.utils.preset_utils import load_from_preset
 from keras_nlp.src.utils.python_utils import classproperty
-from keras_nlp.src.utils.python_utils import format_docstring
 
 
-@keras.saving.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.Task")
 class Task(PipelineModel):
-    """Base class for Task models."""
+    """Base class for all Task models.
+
+    A `Task` wraps a `keras_nlp.models.Backbone` and
+    a `keras_nlp.models.Preprocessor` to create a model that can be directly
+    used for training, fine-tuning, and prediction for a given text problem.
+
+    All `Task` models have `backbone` and `preprocessor` properties. By
+    default `fit()`, `predict()` and `evaluate()` will preprocess all inputs
+    automatically. To preprocess inputs separately or with a custom function,
+    you can set `task.preprocessor = None`, which disable any automatic
+    preprocessing on inputs.
+
+    All `Task` classes include a `from_preset()` constructor which can be used
+    to load a pre-trained config and weights. Calling `from_preset()` on a task
+    will automatically instantiate a `keras_nlp.models.Backbone` and
+    `keras_nlp.models.Preprocessor`.
+    """
+
+    backbone_cls = None
+    preprocessor_cls = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._functional_layer_ids = set(
             id(layer) for layer in self._flatten_layers()
         )
         self._initialized = True
+        if self.backbone is not None:
+            # Keras 2 and Keras 3 handle setting policy differently.
+            if config.keras_3():
+                self.dtype_policy = self._backbone.dtype_policy
+            else:
+                self._set_dtype_policy(self._backbone.dtype_policy)
 
     def __dir__(self):
         if config.keras_3():
             return super().__dir__()
 
         # Temporary fixes for Keras 2 saving. This mimics the following PR for
         # older version of Keras: https://github.com/keras-team/keras/pull/18982
@@ -51,64 +79,14 @@
                 "decoder_transformer_layers",
             ]:
                 return False
             return id(getattr(self, attr)) not in self._functional_layer_ids
 
         return filter(filter_fn, super().__dir__())
 
-    def _check_for_loss_mismatch(self, loss):
-        """Check for a softmax/from_logits mismatch after compile.
-
-        We cannot handle this in the general case, but we can handle this for
-        the extremely common case of a single `SparseCategoricalCrossentropy`
-        loss, and a `None` or `"softmax"` activation.
-        """
-        # Only handle a single loss.
-        if isinstance(loss, (dict, list, tuple)):
-            return
-        # Only handle tasks with activation.
-        if not hasattr(self, "activation"):
-            return
-
-        loss = keras.losses.get(loss)
-        activation = keras.activations.get(self.activation)
-        if isinstance(loss, keras.losses.SparseCategoricalCrossentropy):
-            from_logits = loss.get_config()["from_logits"]
-        elif loss == keras.losses.sparse_categorical_crossentropy:
-            from_logits = False
-        else:
-            # Only handle sparse categorical crossentropy.
-            return
-
-        softmax_output = activation == keras.activations.softmax
-        logit_output = activation == keras.activations.linear
-        if softmax_output and from_logits:
-            raise ValueError(
-                "The `loss` passed to `compile()` expects logit output, but "
-                "the model is configured to output softmax probabilities "
-                "(`activation='softmax'`). This will not converge! Pass "
-                "`from_logits=False` to your loss, e.g. "
-                "`loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False)`. "
-            )
-        if logit_output and not from_logits:
-            raise ValueError(
-                "The `loss` passed to `compile()` expects softmax probability "
-                "output, but the model is configured to output logits "
-                "(`activation=None`). This will not converge! Pass "
-                "`from_logits=True` to your loss, e.g. "
-                "`loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True)`. "
-            )
-
-    def compile(self, optimizer="rmsprop", loss=None, **kwargs):
-        # Temporarily disable jit compilation on torch.
-        if config.backend() == "torch":
-            kwargs["jit_compile"] = False
-        self._check_for_loss_mismatch(loss)
-        super().compile(optimizer=optimizer, loss=loss, **kwargs)
-
     def preprocess_samples(self, x, y=None, sample_weight=None):
         if self.preprocessor is not None:
             return self.preprocessor(x, y=y, sample_weight=sample_weight)
         else:
             return super().preprocess_samples(x, y, sample_weight)
 
     def __setattr__(self, name, value):
@@ -124,24 +102,24 @@
         if is_keras_2 and is_unitialized:
             return object.__setattr__(self, name, value)
         return super().__setattr__(name, value)
 
     @property
     def backbone(self):
         """A `keras.Model` instance providing the backbone sub-model."""
-        return self._backbone
+        return getattr(self, "_backbone", None)
 
     @backbone.setter
     def backbone(self, value):
         self._backbone = value
 
     @property
     def preprocessor(self):
         """A `keras.layers.Layer` instance used to preprocess inputs."""
-        return self._preprocessor
+        return getattr(self, "_preprocessor", None)
 
     @preprocessor.setter
     def preprocessor(self, value):
         self._preprocessor = value
 
     def get_config(self):
         # Don't chain to super here. The default `get_config()` for functional
@@ -163,67 +141,108 @@
         ):
             config["preprocessor"] = keras.layers.deserialize(
                 config["preprocessor"]
             )
         return cls(**config)
 
     @classproperty
-    def backbone_cls(cls):
-        return None
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return None
-
-    @classproperty
     def presets(cls):
-        return {}
+        """List built-in presets for a `Task` subclass."""
+        presets = list_presets(cls)
+        # We can also load backbone presets.
+        if cls.backbone_cls is not None:
+            presets.update(cls.backbone_cls.presets)
+        for subclass in list_subclasses(cls):
+            presets.update(subclass.presets)
+        return presets
 
     @classmethod
     def from_preset(
         cls,
         preset,
         load_weights=True,
         **kwargs,
     ):
-        """Instantiate {{model_task_name}} model from preset architecture and weights.
+        """Instantiate a `keras_nlp.models.Task` from a model preset.
+
+        A preset is a directory of configs, weights and other file assets used
+        to save and load a pre-trained model. The `preset` can be passed as a
+        one of:
+
+        1. a built in preset identifier like `'bert_base_en'`
+        2. a Kaggle Models handle like `'kaggle://user/bert/keras/bert_base_en'`
+        3. a Hugging Face handle like `'hf://user/bert_base_en'`
+        4. a path to a local preset directory like `'./bert_base_en'`
+
+        For any `Task` subclass, you can run `cls.presets.keys()` to list all
+        built-in presets available on the class.
+
+        This constructor can be called in one of two ways. Either from a task
+        specific base class like `keras_nlp.models.CausalLM.from_preset()`, or
+        from a model class like `keras_nlp.models.BertClassifier.from_preset()`.
+        If calling from the a base class, the subclass of the returning object
+        will be inferred from the config in the preset directory.
 
         Args:
-            preset: string. Must be one of "{{preset_names}}".
-            load_weights: Whether to load pre-trained weights into model.
-                Defaults to `True`.
+            preset: string. A built in preset identifier, a Kaggle Models
+                handle, a Hugging Face handle, or a path to a local directory.
+            load_weights: bool. If `True`, the weights will be loaded into the
+                model architecture. If `False`, the weights will be randomly
+                initialized.
 
         Examples:
         ```python
-        # Load architecture and weights from preset
-        model = {{model_task_name}}.from_preset("{{example_preset_name}}")
+        # Load a Gemma generative task.
+        causal_lm = keras_nlp.models.CausalLM.from_preset(
+            "gemma_2b_en",
+        )
 
-        # Load randomly initialized model from preset architecture
-        model = {{model_task_name}}.from_preset(
-            "{{example_preset_name}}",
-            load_weights=False
+        # Load a Bert classification task.
+        model = keras_nlp.models.Classifier.from_preset(
+            "bert_base_en",
+            num_classes=2,
         )
         ```
         """
+        if cls == Task:
+            raise ValueError(
+                "Do not call `Task.from_preset()` directly. Instead call a "
+                "particular task class, e.g. "
+                "`keras_nlp.models.Classifier.from_preset()` or "
+                "`keras_nlp.models.BertClassifier.from_preset()`."
+            )
         if "backbone" in kwargs:
             raise ValueError(
                 "You cannot pass a `backbone` argument to the `from_preset` "
                 f"method. Instead, call the {cls.__name__} default "
                 "constructor with a `backbone` argument. "
                 f"Received: backbone={kwargs['backbone']}."
             )
-        # We support short IDs for official presets, e.g. `"bert_base_en"`.
-        # Map these to a Kaggle Models handle.
-        if preset in cls.presets:
-            preset = cls.presets[preset]["kaggle_handle"]
-
-        preset_cls = check_preset_class(preset, (cls, cls.backbone_cls))
+        preset_cls = check_config_class(preset)
 
         # Backbone case.
-        if preset_cls == cls.backbone_cls:
+        if issubclass(preset_cls, Backbone):
+            if preset_cls is not cls.backbone_cls:
+                subclasses = list_subclasses(cls)
+                subclasses = tuple(
+                    filter(lambda x: x.backbone_cls == preset_cls, subclasses)
+                )
+                if len(subclasses) == 0:
+                    raise ValueError(
+                        f"No registered subclass of `{cls.__name__}` can load "
+                        f"a `{preset_cls.__name__}`."
+                    )
+                if len(subclasses) > 1:
+                    names = ", ".join(f"`{x.__name__}`" for x in subclasses)
+                    raise ValueError(
+                        f"Ambiguous call to `{cls.__name__}.from_preset()`. "
+                        f"Found multiple possible subclasses {names}. "
+                        "Please call `from_preset` on a subclass directly."
+                    )
+                cls = subclasses[0]
             # Forward dtype to the backbone.
             config_overrides = {}
             if "dtype" in kwargs:
                 config_overrides["dtype"] = kwargs.pop("dtype")
             backbone = load_from_preset(
                 preset,
                 load_weights=load_weights,
@@ -236,42 +255,26 @@
                     preset,
                     config_file="tokenizer.json",
                 )
                 preprocessor = cls.preprocessor_cls(tokenizer=tokenizer)
             return cls(backbone=backbone, preprocessor=preprocessor, **kwargs)
 
         # Task case.
+        if not issubclass(preset_cls, cls):
+            raise ValueError(
+                f"Preset has type `{preset_cls.__name__}` which is not a "
+                f"a subclass of calling class `{cls.__name__}`. Call "
+                f"`from_preset` directly on `{preset_cls.__name__}` instead."
+            )
         return load_from_preset(
             preset,
             load_weights=load_weights,
             config_overrides=kwargs,
         )
 
-    def __init_subclass__(cls, **kwargs):
-        # Use __init_subclass__ to setup a correct docstring for from_preset.
-        super().__init_subclass__(**kwargs)
-
-        # If the subclass does not define `from_preset`, assign a wrapper so that
-        # each class can have a distinct docstring.
-        if "from_preset" not in cls.__dict__:
-
-            def from_preset(calling_cls, *args, **kwargs):
-                return super(cls, calling_cls).from_preset(*args, **kwargs)
-
-            cls.from_preset = classmethod(from_preset)
-
-        # Format and assign the docstring unless the subclass has overridden it.
-        if cls.from_preset.__doc__ is None:
-            cls.from_preset.__func__.__doc__ = Task.from_preset.__doc__
-            format_docstring(
-                model_task_name=cls.__name__,
-                example_preset_name=next(iter(cls.presets), ""),
-                preset_names='", "'.join(cls.presets),
-            )(cls.from_preset.__func__)
-
     @property
     def layers(self):
         # Remove preprocessor from layers so it does not show up in the summary.
         layers = super().layers
         if self.preprocessor and self.preprocessor in layers:
             layers.remove(self.preprocessor)
         return layers
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_audio_feature_extractor.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 import numpy as np
 import tensorflow as tf
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.preprocessing.preprocessing_layer import (
     PreprocessingLayer,
 )
-from keras_nlp.src.models.whisper.whisper_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
-from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
 class WhisperAudioFeatureExtractor(PreprocessingLayer):
     """
     Whisper audio feature extractor layer.
 
@@ -262,56 +258,7 @@
                 "stride": self.stride,
                 "sampling_rate": self.sampling_rate,
                 "max_audio_length": self.max_audio_length,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    @classmethod
-    def from_preset(
-        cls,
-        preset,
-        **kwargs,
-    ):
-        """Instantiate Whisper audio feature extractor from a given preset.
-
-        Args:
-            preset: string. Must be one of "{{preset_names}}".
-
-        Examples:
-        ```python
-        # Load a preset tokenizer.
-        audio_feature_extractor = WhisperAudioFeatureExtractor.from_preset(
-            "{{example_preset_name}}"
-        )
-
-        # Compute the log-mel spectrogram.
-        audio_tensor = tf.ones((8000,), dtype=tf.float32)
-        audio_feature_extractor(audio_tensor)
-        ```
-        """
-
-        if not cls.presets:
-            raise NotImplementedError(
-                "No presets have been created for this class"
-            )
-
-        if preset not in cls.presets:
-            raise ValueError(
-                "`preset` must be one of "
-                f"""{", ".join(cls.presets)}. Received: {preset}."""
-            )
-
-        config = cls.presets[preset]["audio_feature_extractor_config"]
-
-        return cls.from_config({**config, **kwargs})
-
-
-format_docstring(
-    example_preset_name=next(iter(backbone_presets), ""),
-    preset_names='", "'.join(backbone_presets),
-)(WhisperAudioFeatureExtractor.from_preset.__func__)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.layers.modeling.position_embedding import PositionEmbedding
 from keras_nlp.src.layers.modeling.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
 from keras_nlp.src.models.backbone import Backbone
 from keras_nlp.src.models.whisper.whisper_decoder import WhisperDecoder
 from keras_nlp.src.models.whisper.whisper_encoder import WhisperEncoder
-from keras_nlp.src.models.whisper.whisper_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
 from keras_nlp.src.utils.tensor_utils import assert_tf_backend
 
 
 def whisper_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
@@ -269,14 +266,15 @@
                 "decoder_token_ids": decoder_token_id_input,
                 "decoder_padding_mask": decoder_padding_mask_input,
             },
             outputs={
                 "encoder_sequence_output": encoder_output,
                 "decoder_sequence_output": decoder_output,
             },
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
@@ -300,11 +298,7 @@
                 "dropout": self.dropout,
                 "max_encoder_sequence_length": self.max_encoder_sequence_length,
                 "max_decoder_sequence_length": self.max_decoder_sequence_length,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_cached_multi_head_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_cached_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_decoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_encoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from absl import logging
 
 from keras_nlp.src.backend import keras
 from keras_nlp.src.layers.preprocessing.start_end_packer import StartEndPacker
 from keras_nlp.src.models.preprocessor import Preprocessor
 from keras_nlp.src.models.whisper.whisper_audio_feature_extractor import (
     WhisperAudioFeatureExtractor,
 )
-from keras_nlp.src.models.whisper.whisper_presets import backbone_presets
 from keras_nlp.src.models.whisper.whisper_tokenizer import WhisperTokenizer
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.saving.register_keras_serializable(package="keras_nlp")
 class WhisperPreprocessor(Preprocessor):
     """A Whisper preprocessing layer which handles audio and text input.
 
     This preprocessing layer will do three things:
@@ -149,14 +146,16 @@
         "decoder_text": ["The quick brown fox jumped.", "Call me Ishmael."],
     }
     ds = tf.data.Dataset.from_tensor_slices(features)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
+    tokenizer_cls = WhisperTokenizer
+
     def __init__(
         self,
         tokenizer,
         audio_feature_extractor=None,
         decoder_sequence_length=448,
         language=None,
         task=None,
@@ -322,19 +321,7 @@
         """Alias for `decoder_sequence_length`."""
         return self.decoder_sequence_length
 
     @sequence_length.setter
     def sequence_length(self, value):
         self.decoder_sequence_length = value
 
-    @classproperty
-    def audio_feature_extractor_cls(cls):
-        return WhisperAudioFeatureExtractor
-
-    @classproperty
-    def tokenizer_cls(cls):
-        return WhisperTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/whisper/whisper_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 import json
 
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.whisper.whisper_presets import backbone_presets
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 def _load_dict(dict_or_path):
     if isinstance(dict_or_path, str):
         with open(dict_or_path, "r", encoding="utf-8") as f:
             dict_or_path = json.load(f)
     return dict_or_path
@@ -161,11 +158,7 @@
             {
                 "special_tokens": self.special_tokens,
                 "language_tokens": self.language_tokens,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.models.roberta import roberta_backbone
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaBackbone")
 class XLMRobertaBackbone(roberta_backbone.RobertaBackbone):
     """An XLM-RoBERTa encoder network.
 
     This class implements a bi-directional Transformer-based encoder as
@@ -79,11 +76,7 @@
         intermediate_dim=512,
         max_sequence_length=128
     )
     model(input_data)
     ```
     """
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/xlnet_backbone.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,237 +8,214 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
-from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
-    XLMRobertaPreprocessor,
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.xlnet.xlnet_content_and_query_embedding import (
+    ContentAndQueryEmbedding,
 )
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.models.xlnet.xlnet_encoder import XLNetAttentionMaskLayer
+from keras_nlp.src.models.xlnet.xlnet_encoder import XLNetEncoder
+from keras_nlp.src.models.xlnet.xlnet_encoder import XLNetSegmentMatrixLayer
 
 
-@keras_nlp_export("keras_nlp.models.XLMRobertaClassifier")
-class XLMRobertaClassifier(Task):
-    """An end-to-end XLM-RoBERTa model for classification tasks.
-
-    This model attaches a classification head to a
-    `keras_nlp.model.XLMRobertaBackbone` instance, mapping from the backbone
-    outputs to logits suitable for a classification task. For usage of
-    this model with pre-trained weights, see the `from_preset()` constructor.
-
-    This model can optionally be configured with a `preprocessor` layer, in
-    which case it will automatically apply preprocessing to raw inputs during
-    `fit()`, `predict()`, and `evaluate()`. This is done by default when
-    creating the model with `from_preset()`.
+@keras.saving.register_keras_serializable(package="keras_nlp")
+class XLNetBackbone(Backbone):
+    """XLNet encoder network.
 
-    Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available
-    [here](https://github.com/facebookresearch/fairseq).
-
-    Args:
-        backbone: A `keras_nlp.models.XLMRobertaBackbone` instance.
-        num_classes: int. Number of classes to predict.
-        preprocessor: A `keras_nlp.models.XLMRobertaPreprocessor` or `None`. If
-            `None`, this model will not apply preprocessing, and inputs should
-            be preprocessed before calling the model.
-        activation: Optional `str` or callable. The activation function to use
-            on the model outputs. Set `activation="softmax"` to return output
-            probabilities. Defaults to `None`.
-        hidden_dim: int. The size of the pooler layer.
-        dropout: float. The dropout probability value, applied to the pooled
-            output, and after the first dense layer.
+    This class implements a XLNet Transformer.
 
-    Examples:
+    The default constructor gives a fully customizable, randomly initialized
+    XLNet encoder with any number of layers, heads, and embedding dimensions.
+    To load preset architectures and weights, use the `from_preset` constructor.
 
-    Raw string data.
-    ```python
-    features = ["The quick brown fox jumped.", "نسيت الواجب"]
-    labels = [0, 3]
+    Disclaimer: Pre-trained models are provided on an "as is" basis, without
+    warranties or conditions of any kind.
 
-    # Pretrained classifier.
-    classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
-        "xlm_roberta_base_multi",
-        num_classes=4,
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
-    classifier.predict(x=features, batch_size=2)
+    Attributes:
+        vocabulary_size: int. The size of the token vocabulary.
+        num_layers: int. The number of transformer encoder layers.
+        num_heads: int, the number of heads in the
+            `keras.layers.TwoStreamRelativeAttention` layer.
+        hidden_dim: int, the size hidden states.
+        intermediate_dim: int, the hidden size of feedforward network.
+        dropout: float, defaults to 0.0 the dropout value, shared by
+            `keras.layers.TwoStreamRelativeAttention` and feedforward network.
+        activation: string or `keras.activations`, defaults to "gelu". the
+            activation function of feedforward network.
+        kernel_initializer_range: int, defaults to 0.02. The kernel initializer
+            range for the dense and relative attention layers.
+        bias_initializer: string or `keras.initializers` initializer,
+            defaults to "zeros". The bias initializer for
+            the dense and multiheaded relative attention layers.
+        dtype: string or `keras.mixed_precision.DTypePolicy`. The dtype to use
+            for model computations and weights. Note that some computations,
+            such as softmax and layer normalization, will always be done at
+            float32 precision regardless of dtype.
+
+    Call arguments:
+        token_ids: Indices of input sequence tokens in the vocabulary of shape
+            `[batch_size, sequence_length]`.
+        segment_ids: Segment token indices to indicate first and second portions
+            of the inputs of shape `[batch_size, sequence_length]`.
+        padding_mask: Mask to avoid performing attention on padding token indices
+            of shape `[batch_size, sequence_length]`.
 
-    # Re-compile (e.g., with a new learning rate).
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-        optimizer=keras.optimizers.Adam(5e-5),
-        jit_compile=True,
-    )
-    # Access backbone programmatically (e.g., to change `trainable`).
-    classifier.backbone.trainable = False
-    # Fit again.
-    classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-
-    Preprocessed integer data.
+    Example:
     ```python
-    features = {
-        "token_ids": np.ones(shape=(2, 12), dtype="int32"),
-        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2),
-    }
-    labels = [0, 3]
-
-    # Pretrained classifier without preprocessing.
-    classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
-        "xlm_roberta_base_multi",
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
-    ```
+    import numpy as np
+    from keras_nlp.models import XLNetBackbone
 
-    Custom backbone and vocabulary.
-    ```python
-    features = ["The quick brown fox jumped.", "نسيت الواجب"]
-    labels = [0, 3]
+    input_data = {
+        "token_ids": np.array(
+            [460, 5272, 1758, 4905, 9, 4, 3], shape=(1, 7),
+        ),
+        "segment_ids": np.array(
+            [0, 0, 0, 0, 0, 0, 2], shape=(1, 7),
+        ),
+        "padding_mask": np.array(
+            [1, 1, 1, 1, 1, 1, 1], shape=(1, 7)
+        ),
+    }
 
-    def train_sentencepiece(ds, vocab_size):
-        bytes_io = io.BytesIO()
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=ds.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=vocab_size,
-            model_type="WORD",
-            unk_id=0,
-            bos_id=1,
-            eos_id=2,
-        )
-        return bytes_io.getvalue()
-    ds = tf.data.Dataset.from_tensor_slices(
-        ["the quick brown fox", "the earth is round"]
-    )
-    proto = train_sentencepiece(ds, vocab_size=10)
-    tokenizer = keras_nlp.models.XLMRobertaTokenizer(
-        proto=proto
-    )
-    preprocessor = keras_nlp.models.XLMRobertaPreprocessor(
-        tokenizer,
-        sequence_length=128,
+    # Randomly initialized XLNet encoder with a custom config
+    model = keras_nlp.models.XLNetBackbone(
+        vocabulary_size=32000,
+        num_layers=12,
+        num_heads=12,
+        hidden_dim=768,
+        intermediate_dim=3072,
     )
-    backbone = keras_nlp.models.XLMRobertaBackbone(
-        vocabulary_size=250002,
-        num_layers=4,
-        num_heads=4,
-        hidden_dim=256,
-        intermediate_dim=512,
-        max_sequence_length=128,
-    )
-    classifier = keras_nlp.models.XLMRobertaClassifier(
-        backbone=backbone,
-        preprocessor=preprocessor,
-        num_classes=4,
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
+    output = model(input_data)
     ```
     """
 
     def __init__(
         self,
-        backbone,
-        num_classes,
-        preprocessor=None,
-        activation=None,
-        hidden_dim=None,
+        vocabulary_size,
+        num_layers,
+        num_heads,
+        hidden_dim,
+        intermediate_dim,
         dropout=0.0,
+        activation="gelu",
+        kernel_initializer_range=0.02,
+        bias_initializer="zeros",
+        dtype=None,
         **kwargs,
     ):
         # === Layers ===
-        self.backbone = backbone
-        self.preprocessor = preprocessor
-        self.pooled_dropout = keras.layers.Dropout(
+        self.content_query_embedding = ContentAndQueryEmbedding(
+            vocabulary_size=vocabulary_size,
+            hidden_dim=hidden_dim,
+            dropout=dropout,
+            dtype=dtype,
+            name="content_query_embedding",
+        )
+        self.attn_mask_layer = XLNetAttentionMaskLayer(
+            hidden_dim=hidden_dim,
+            kernel_initializer_range=kernel_initializer_range,
+            dtype=dtype,
+            name="encoder_block_attn_mask_layer",
+        )
+        self.seg_mat_layer = XLNetSegmentMatrixLayer(
+            dtype=dtype,
+            name="encoder_block_seg_mat_layer",
+        )
+        head_dim = hidden_dim // num_heads
+        self.transformer_layers = []
+        for i in range(num_layers):
+            layer = XLNetEncoder(
+                num_heads=num_heads,
+                hidden_dim=hidden_dim,
+                head_dim=head_dim,
+                intermediate_dim=intermediate_dim,
+                dropout=dropout,
+                activation=activation,
+                layer_norm_epsilon=1e-12,
+                kernel_initializer_range=kernel_initializer_range,
+                bias_initializer=bias_initializer,
+                dtype=dtype,
+                name=f"xlnet_encoder_{i}",
+            )
+            self.transformer_layers.append(layer)
+        self.dropout = keras.layers.Dropout(
             dropout,
-            dtype=backbone.dtype_policy,
-            name="pooled_dropout",
+            dtype=dtype,
+            name="dropout",
         )
-        hidden_dim = hidden_dim or backbone.hidden_dim
-        self.pooled_dense = keras.layers.Dense(
-            hidden_dim,
-            activation="tanh",
-            dtype=backbone.dtype_policy,
-            name="pooled_dense",
+
+        # === Functional Model ===
+        token_id_input = keras.Input(
+            shape=(None,), dtype="int32", name="token_ids"
         )
-        self.output_dropout = keras.layers.Dropout(
-            dropout,
-            dtype=backbone.dtype_policy,
-            name="output_dropout",
+        padding_mask_input = keras.Input(
+            shape=(None,), dtype="int32", name="padding_mask"
         )
-        self.output_dense = keras.layers.Dense(
-            num_classes,
-            kernel_initializer=roberta_kernel_initializer(),
-            activation=activation,
-            dtype=backbone.dtype_policy,
-            name="logits",
+        segment_id_input = keras.Input(
+            shape=(None,), dtype="int32", name="segment_ids"
         )
-
-        # === Functional Model ===
-        inputs = backbone.input
-        x = backbone(inputs)[:, backbone.start_token_index, :]
-        x = self.pooled_dropout(x)
-        x = self.pooled_dense(x)
-        x = self.output_dropout(x)
-        outputs = self.output_dense(x)
-        # Instantiate using Functional API Model constructor
+        # Content and Query Embedding
+        word_emb, pos_emb = self.content_query_embedding(token_id_input)
+        # Apply XLNetAttentionMaskLayer and XLNetSegmentMatrixLayer Layers
+        # to get the processed attention masks and segment matrix.
+        attn_mask_content, attn_mask_query = self.attn_mask_layer(
+            padding_mask_input
+        )
+        seg_mat = self.seg_mat_layer(segment_id_input)
+        output_content = word_emb
+        for transformer_layer in self.transformer_layers:
+            output_content, output_query = transformer_layer(
+                output_content=output_content,
+                attn_mask_content=attn_mask_content,
+                attn_mask_query=attn_mask_query,
+                pos_emb=pos_emb,
+                seg_mat=seg_mat,
+            )
+        output = self.dropout(output_content)
         super().__init__(
-            inputs=inputs,
-            outputs=outputs,
+            inputs={
+                "token_ids": token_id_input,
+                "padding_mask": padding_mask_input,
+                "segment_ids": segment_id_input,
+            },
+            outputs=output,
+            dtype=dtype,
             **kwargs,
         )
 
         # === Config ===
-        self.backbone = backbone
-        self.preprocessor = preprocessor
-        self.num_classes = num_classes
-        self.activation = keras.activations.get(activation)
+        self.vocabulary_size = vocabulary_size
+        self.num_layers = num_layers
+        self.num_heads = num_heads
         self.hidden_dim = hidden_dim
+        self.intermediate_dim = intermediate_dim
         self.dropout = dropout
-
-        # === Default compilation ===
-        logit_output = self.activation == keras.activations.linear
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=logit_output
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
-        )
+        self.activation = activation
+        self.kernel_initializer_range = kernel_initializer_range
+        self.bias_initializer = bias_initializer
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "num_classes": self.num_classes,
-                "activation": keras.activations.serialize(self.activation),
+                "vocabulary_size": self.vocabulary_size,
+                "num_layers": self.num_layers,
+                "num_heads": self.num_heads,
                 "hidden_dim": self.hidden_dim,
+                "intermediate_dim": self.intermediate_dim,
                 "dropout": self.dropout,
+                "activation": self.activation,
+                "kernel_initializer_range": self.kernel_initializer_range,
+                "bias_initializer": self.bias_initializer,
             }
         )
         return config
 
-    @classproperty
-    def backbone_cls(cls):
-        return XLMRobertaBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return XLMRobertaPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+    @property
+    def token_embedding(self):
+        return self.get_layer("content_query_embedding").word_embed
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/albert/albert_classifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,200 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import keras
-from keras_nlp.src.layers.modeling.masked_lm_head import MaskedLMHead
-from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.src.models.task import Task
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
-    XLMRobertaMaskedLMPreprocessor,
-)
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.src.utils.python_utils import classproperty
-
-
-@keras_nlp_export("keras_nlp.models.XLMRobertaMaskedLM")
-class XLMRobertaMaskedLM(Task):
-    """An end-to-end XLM-RoBERTa model for the masked language modeling task.
-
-    This model will train XLM-RoBERTa on a masked language modeling task.
-    The model will predict labels for a number of masked tokens in the
-    input data. For usage of this model with pre-trained weights, see the
-    `from_preset()` method.
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_backbone import albert_kernel_initializer
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.models.classifier import Classifier
+
+
+@keras_nlp_export("keras_nlp.models.AlbertClassifier")
+class AlbertClassifier(Classifier):
+    """An end-to-end ALBERT model for classification tasks
+
+    This model attaches a classification head to a `keras_nlp.model.AlbertBackbone`
+    backbone, mapping from the backbone outputs to logit output suitable for
+    a classification task. For usage of this model with pre-trained weights, see
+    the `from_preset()` method.
 
     This model can optionally be configured with a `preprocessor` layer, in
-    which case inputs can be raw string features during `fit()`, `predict()`,
-    and `evaluate()`. Inputs will be tokenized and dynamically masked during
-    training and evaluation. This is done by default when creating the model
-    with `from_preset()`.
+    which case it will automatically apply preprocessing to raw inputs during
+    `fit()`, `predict()`, and `evaluate()`. This is done by default when
+    creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available
-    [here](https://github.com/facebookresearch/fairseq).
+    warranties or conditions of any kind.
 
     Args:
-        backbone: A `keras_nlp.models.XLMRobertaBackbone` instance.
-        preprocessor: A `keras_nlp.models.XLMRobertaMaskedLMPreprocessor` or
-            `None`. If `None`, this model will not apply preprocessing, and
-            inputs should be preprocessed before calling the model.
+        backbone: A `keras_nlp.models.AlertBackbone` instance.
+        num_classes: int. Number of classes to predict.
+        preprocessor: A `keras_nlp.models.AlbertPreprocessor` or `None`. If
+            `None`, this model will not apply preprocessing, and inputs should
+            be preprocessed before calling the model.
+        activation: Optional `str` or callable. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+            Defaults to `None`.
+        dropout: float. The dropout probability value, applied after the dense
+            layer.
 
-    Example usage:
+    Examples:
 
-    Raw string inputs and pretrained backbone.
+     Raw string data.
     ```python
-    # Create a dataset with raw string features. Labels are inferred.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
 
-    # Pretrained language model
-    # on an MLM task.
-    masked_lm = keras_nlp.models.XLMRobertaMaskedLM.from_preset(
-        "xlm_roberta_base_multi",
+    # Pretrained classifier.
+    classifier = keras_nlp.models.AlbertClassifier.from_preset(
+        "albert_base_en_uncased",
+        num_classes=4,
     )
-    masked_lm.fit(x=features, batch_size=2)
-    ```
+    classifier.fit(x=features, y=labels, batch_size=2)
+    classifier.predict(x=features, batch_size=2)
 
     # Re-compile (e.g., with a new learning rate).
-    masked_lm.compile(
+    classifier.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
         optimizer=keras.optimizers.Adam(5e-5),
         jit_compile=True,
     )
     # Access backbone programmatically (e.g., to change `trainable`).
-    masked_lm.backbone.trainable = False
+    classifier.backbone.trainable = False
     # Fit again.
-    masked_lm.fit(x=features, batch_size=2)
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
     Preprocessed integer data.
     ```python
-    # Create a preprocessed dataset where 0 is the mask token.
     features = {
-        "token_ids": np.array([[1, 2, 0, 4, 0, 6, 7, 8]] * 2),
-        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1]] * 2),
-        "mask_positions": np.array([[2, 4]] * 2)
+        "token_ids": np.ones(shape=(2, 12), dtype="int32"),
+        "segment_ids": np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2),
+        "padding_mask": np.array([[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2),
     }
-    # Labels are the original masked values.
-    labels = [[3, 5]] * 2
+    labels = [0, 3]
 
-    masked_lm = keras_nlp.models.XLMRobertaMaskedLM.from_preset(
-        "xlm_roberta_base_multi",
+    # Pretrained classifier without preprocessing.
+    classifier = keras_nlp.models.AlbertClassifier.from_preset(
+        "albert_base_en_uncased",
+        num_classes=4,
         preprocessor=None,
     )
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
 
-    masked_lm.fit(x=features, y=labels, batch_size=2)
+    Custom backbone and vocabulary.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
+
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(features)
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=10,
+        model_type="WORD",
+        pad_id=0,
+        unk_id=1,
+        bos_id=2,
+        eos_id=3,
+        pad_piece="<pad>",
+        unk_piece="<unk>",
+        bos_piece="[CLS]",
+        eos_piece="[SEP]",
+        user_defined_symbols="[MASK]",
+    )
+    tokenizer = keras_nlp.models.AlbertTokenizer(
+        proto=bytes_io.getvalue(),
+    )
+    preprocessor = keras_nlp.models.AlbertPreprocessor(
+        tokenizer=tokenizer,
+        sequence_length=128,
+    )
+    backbone = keras_nlp.models.AlbertBackbone(
+        vocabulary_size=tokenizer.vocabulary_size(),
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        embedding_dim=128,
+        intermediate_dim=512,
+        max_sequence_length=128,
+    )
+    classifier = keras_nlp.models.AlbertClassifier(
+        backbone=backbone,
+        preprocessor=preprocessor,
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
+    backbone_cls = AlbertBackbone
+    preprocessor_cls = AlbertPreprocessor
+
     def __init__(
         self,
         backbone,
+        num_classes,
         preprocessor=None,
+        activation=None,
+        dropout=0.1,
         **kwargs,
     ):
         # === Layers ===
         self.backbone = backbone
         self.preprocessor = preprocessor
-        self.masked_lm_head = MaskedLMHead(
-            vocabulary_size=backbone.vocabulary_size,
-            token_embedding=backbone.token_embedding,
-            intermediate_activation="gelu",
-            kernel_initializer=roberta_kernel_initializer(),
+        self.output_dense = keras.layers.Dense(
+            num_classes,
+            kernel_initializer=albert_kernel_initializer(),
+            activation=activation,
+            dtype=backbone.dtype_policy,
+            name="logits",
+        )
+        self.output_dropout = keras.layers.Dropout(
+            dropout,
             dtype=backbone.dtype_policy,
-            name="mlm_head",
+            name="output_dropout",
         )
 
         # === Functional Model ===
-        inputs = {
-            **backbone.input,
-            "mask_positions": keras.Input(
-                shape=(None,), dtype="int32", name="mask_positions"
-            ),
-        }
-        backbone_outputs = backbone(backbone.input)
-        outputs = self.masked_lm_head(
-            backbone_outputs, inputs["mask_positions"]
-        )
+        inputs = backbone.input
+        pooled = backbone(inputs)["pooled_output"]
+        pooled = self.output_dropout(pooled)
+        outputs = self.output_dense(pooled)
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             **kwargs,
         )
 
-        # === Default compilation ===
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            optimizer=keras.optimizers.Adam(5e-5),
-            weighted_metrics=[keras.metrics.SparseCategoricalAccuracy()],
-            jit_compile=True,
+        # === Config ===
+        self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
+        self.dropout = dropout
+
+    def get_config(self):
+        config = super().get_config()
+        config.update(
+            {
+                "num_classes": self.num_classes,
+                "activation": keras.activations.serialize(self.activation),
+                "dropout": self.dropout,
+            }
         )
 
-    @classproperty
-    def backbone_cls(cls):
-        return XLMRobertaBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return XLMRobertaMaskedLMPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+        return config
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.layers.preprocessing.multi_segment_packer import (
     MultiSegmentPacker,
 )
 from keras_nlp.src.models.preprocessor import Preprocessor
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
 from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaPreprocessor")
 class XLMRobertaPreprocessor(Preprocessor):
     """An XLM-RoBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -142,14 +139,16 @@
     ds = ds.map(
         lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
+    tokenizer_cls = XLMRobertaTokenizer
+
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
         **kwargs,
     ):
@@ -200,15 +199,7 @@
 
     @sequence_length.setter
     def sequence_length(self, value):
         self._sequence_length = value
         if self.packer is not None:
             self.packer.sequence_length = value
 
-    @classproperty
-    def tokenizer_cls(cls):
-        return XLMRobertaTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
 
 import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
 from keras_nlp.src.utils.tensor_utils import tensor_to_list
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaTokenizer")
 class XLMRobertaTokenizer(SentencePieceTokenizer):
     """An XLM-RoBERTa tokenizer using SentencePiece subword segmentation.
 
@@ -184,11 +181,7 @@
         tokens = tf.where(tf.equal(tokens, self.start_token_id - 1), 1, tokens)
 
         # Note: Even though we map `"<s>" and `"</s>"` to the correct IDs,
         # the `detokenize` method will return empty strings for these tokens.
         # This is a vagary of the `sentencepiece` library.
         return super().detokenize(tokens)
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/relative_attention.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/relative_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/xlnet_content_and_query_embedding.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/xlnet_content_and_query_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/models/xlnet/xlnet_encoder.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/xlnet/xlnet_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/beam_sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/beam_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import tensorflow as tf
 import tree
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import ops
 from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
 @keras_nlp_export("keras_nlp.samplers.BeamSampler")
 class BeamSampler(Sampler):
     """Beam Sampler class.
 
     This sampler implements beam search algorithm. At each time-step, beam
@@ -66,15 +67,15 @@
     def __call__(
         self,
         next,
         prompt,
         cache=None,
         index=0,
         mask=None,
-        end_token_id=None,
+        stop_token_ids=None,
         hidden_states=None,
         model=None,
     ):
         batch_size, max_length = ops.shape(prompt)[0], ops.shape(prompt)[1]
         index = ops.cast(index, "int32")
 
         def create_beams(x):
@@ -105,18 +106,18 @@
         # On the first loop, make sure only the original beam is considered.
         log_probs = ops.array(
             [[0.0] + [-1e9] * (self.num_beams - 1)], dtype="float32"
         )
         log_probs = flatten_beams(ops.repeat(log_probs, batch_size, axis=0))
 
         def cond(prompt, cache, index, log_probs):
-            if end_token_id is None:
+            if stop_token_ids is None:
                 return True
-            # Stop if all sequences have produced a *new* end_token_id.
-            end_tokens = (prompt == end_token_id) & (~mask)
+            # Stop if all sequences have produced a *new* stop token.
+            end_tokens = any_equal(prompt, stop_token_ids, ~mask)
             prompt_done = ops.any(end_tokens, axis=-1)
             return ops.logical_not(ops.all(prompt_done))
 
         def body(prompt, cache, index, log_probs):
             # Compute the softmax distribution for the next token.
             logits, _, cache = next(prompt, cache, index)
             vocab_size = ops.shape(logits)[-1]
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/contrastive_sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/contrastive_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 import tree
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import ops
 from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
 @keras_nlp_export("keras_nlp.samplers.ContrastiveSampler")
 class ContrastiveSampler(Sampler):
     """Contrastive Sampler class.
 
     This sampler implements contrastive search algorithm. In short, the sampler
@@ -30,15 +31,14 @@
     behavior of duplicating seen tokens.
 
     Args:
         k: int, the `k` value of top-k. Next token will be chosen from k tokens.
         alpha: float, the weight of minus max similarity in joint score
             computation. The larger the value of `alpha`, the score relies more
             on the similarity than the token probability.
-        seed: int. The random seed. Defaults to `None`.
 
     Call arguments:
         {{call_args}}
 
     Examples:
     ```python
     causal_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
@@ -67,15 +67,15 @@
     def __call__(
         self,
         next,
         prompt,
         cache=None,
         index=0,
         mask=None,
-        end_token_id=None,
+        stop_token_ids=None,
         hidden_states=None,
         model=None,
     ):
         if hidden_states is None:
             raise ValueError(
                 "`ContrastiveSampler` requires passing a `hidden_states`, but"
                 "received `None`."
@@ -103,18 +103,18 @@
         # Compute initial logits.
         logits, _, cache = next(prompt, cache, index)
         # `ops.while_loop` will not accept `None` as a value for `loop_vars`.
         has_cache = cache is not None
         cache = cache if has_cache else ()
 
         def cond(prompt, cache, index, logits, hidden_states):
-            if end_token_id is None:
+            if stop_token_ids is None:
                 return True
-            # Stop if all sequences have produced a *new* end_token_id.
-            end_tokens = (prompt == end_token_id) & (~mask)
+            # Stop if all sequences have produced a *new* stop token.
+            end_tokens = any_equal(prompt, stop_token_ids, ~mask)
             prompt_done = ops.any(end_tokens, axis=-1)
             return ops.logical_not(ops.all(prompt_done))
 
         def body(prompt, cache, index, logits, hidden_states):
             # Compute the softmax distribution for the next token.
             probabilities = self.compute_probabilities(logits)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/greedy_sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/greedy_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/random_sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.backend import config
 from keras_nlp.src.backend import keras
 from keras_nlp.src.backend import ops
 from keras_nlp.src.backend import random
+from keras_nlp.src.utils.tensor_utils import any_equal
 
 
 @keras_nlp_export("keras_nlp.samplers.Sampler")
 class Sampler:
     """Base sampler class.
 
     Args:
@@ -32,15 +33,15 @@
         {{call_args}}
 
     This base class can be extended to implement different auto-regressive
     sampling methods. To do so, override the `get_next_token()` method, which
     computes the next token based on a probability distribution over all
     possible vocab entries.
 
-    Examples:
+    Example:
 
     ```python
     causal_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
 
     # Greedy search with some tokens forbidden.
     class CustomSampler(keras_nlp.samplers.Sampler):
         def __init__(self, forbidden_tokens, **kwargs):
@@ -86,15 +87,15 @@
     def __call__(
         self,
         next,
         prompt,
         cache=None,
         index=0,
         mask=None,
-        end_token_id=None,
+        stop_token_ids=None,
         hidden_states=None,
         model=None,
     ):
         max_length = ops.shape(prompt)[-1]
         # Make sure `max_length` and `index` are the same dtype.
         index = ops.cast(index, "int32")
         max_length = ops.cast(max_length, "int32")
@@ -102,18 +103,18 @@
             mask = ops.zeros_like(prompt, dtype="bool")
         else:
             mask = ops.cast(mask, dtype="bool")
         # `ops.while_loop` will not accept `None` as a value for `loop_vars`.
         cache = () if cache is None else cache
 
         def cond(prompt, cache, index):
-            if end_token_id is None:
+            if stop_token_ids is None:
                 return True
-            # Stop if all sequences have produced a *new* end_token_id.
-            end_tokens = (prompt == end_token_id) & (~mask)
+            # Stop if all sequences have produced a *new* id from stop_token_ids.
+            end_tokens = any_equal(prompt, stop_token_ids, ~mask)
             prompt_done = ops.any(end_tokens, axis=-1)
             return ops.logical_not(ops.all(prompt_done))
 
         def body(prompt, cache, index):
             # Compute the softmax distribution for the next token.
             logits, _, cache = next(prompt, cache, index)
             probabilities = self.compute_probabilities(logits)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/serialization.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/top_k_sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/top_k_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/samplers/top_p_sampler.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/samplers/top_p_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tests/test_case.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tests/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,18 +325,18 @@
                 output_data = layer(input_data)
             for tensor in tree.flatten(output_data):
                 if is_float_dtype(tensor.dtype):
                     self.assertDTypeEqual(tensor, policy.compute_dtype)
             for weight in layer.weights:
                 if is_float_dtype(weight.dtype):
                     self.assertDTypeEqual(weight, policy.variable_dtype)
-            for sublayer in layer._flatten_layers(include_self=False):
-                if isinstance(
-                    sublayer, (keras.layers.Softmax, keras.layers.InputLayer)
-                ):
+            for sublayer in layer._flatten_layers():
+                if isinstance(sublayer, keras.layers.Softmax):
+                    continue
+                if isinstance(sublayer, keras.layers.InputLayer):
                     continue
                 self.assertEqual(policy.compute_dtype, sublayer.compute_dtype)
                 self.assertEqual(policy.variable_dtype, sublayer.variable_dtype)
 
     def run_model_saving_test(
         self,
         cls,
@@ -454,16 +454,14 @@
         input_data,
         init_kwargs={},
         expected_output=None,
         expected_output_shape=None,
         expected_partial_output=None,
     ):
         """Run instantiation and a forward pass for a preset."""
-        self.assertRegex(cls.from_preset.__doc__, preset)
-
         with self.assertRaises(Exception):
             cls.from_preset("clowntown", **init_kwargs)
 
         instance = cls.from_preset(preset, **init_kwargs)
 
         if isinstance(input_data, tuple):
             # Mimic tf.data unpacking behavior for preprocessing layers.
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/byte_pair_tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,25 +18,21 @@
 https://github.com/openai/gpt-2/blob/master/src/encoder.py,
 but is TF graph compatible.
 """
 
 import json
 import os
 from typing import Iterable
-from typing import List
 
+import keras
 import regex as re
 import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.tokenizers import tokenizer
-from keras_nlp.src.utils.preset_utils import check_preset_class
-from keras_nlp.src.utils.preset_utils import load_from_preset
-from keras_nlp.src.utils.python_utils import classproperty
-from keras_nlp.src.utils.python_utils import format_docstring
 from keras_nlp.src.utils.tensor_utils import assert_tf_text_installed
 from keras_nlp.src.utils.tensor_utils import convert_to_ragged_batch
 from keras_nlp.src.utils.tensor_utils import is_int_dtype
 from keras_nlp.src.utils.tensor_utils import is_string_dtype
 
 try:
     import tensorflow_text as tf_text
@@ -145,15 +141,15 @@
 
 class BytePairTokenizerCache(tf.Module):
     """Cache that stores the encoded result of seen tokens.
 
     The cache key is string tensor or python strings, and the value is split
     tokens joined by whitespace. For example, "dragonfly" => "dragon fly"
 
-    Examples:
+    Example:
     ```
     cache = BytePairTokenizerCache()
     cache.insert(["butterfly", "dragonfly"], ["but ter fly", "dragon fly"])
     cache.lookup(["butterfly"])
     ```
     """
 
@@ -387,38 +383,38 @@
         self.merge_ranks_lookup_default = len(self.merges) + 1
         self.merge_ranks = create_static_hashtable(
             self.merges,
             list(range(len(self.merges))),
             default=self.merge_ranks_lookup_default,
         )
 
-    def get_vocabulary(self) -> List[str]:
+    def get_vocabulary(self):
         """Get the tokenizer vocabulary as a list of strings tokens."""
         self._check_vocabulary()
         return self.vocabulary.keys()
 
-    def vocabulary_size(self) -> int:
-        """Get the size of the tokenizer vocabulary."""
+    def vocabulary_size(self):
+        """Get the integer size of the tokenizer vocabulary."""
         self._check_vocabulary()
         return len(self.vocabulary)
 
-    def id_to_token(self, id: int) -> str:
+    def id_to_token(self, id):
         """Convert an integer id to a string token."""
         # This will be slow, but keep memory usage down compared to building a
         # dict. Assuming the main use case is looking up a few special tokens
         # early in the vocab, this should be fine.
         self._check_vocabulary()
 
         keys = self.get_vocabulary()
         for token in keys:
             if self.vocabulary[token] == id:
                 return token
         raise ValueError(f"`id` is out of the vocabulary. Received: {id}")
 
-    def token_to_id(self, token: str) -> int:
+    def token_to_id(self, token):
         """Convert a string token to an integer id."""
         self._check_vocabulary()
         return self.vocabulary[token]
 
     @tf.function
     def _bpe_merge_one_step(self, words, mask):
         """Perform one step of byte-pair merge."""
@@ -605,14 +601,19 @@
             self.unicode2byte.lookup(split_unicode_text), axis=-1
         )
 
         if unbatched:
             outputs = tf.squeeze(outputs, 0)
         return outputs
 
+    def compute_output_spec(self, input_spec):
+        return keras.KerasTensor(
+            input_spec.shape + (self.sequence_length,), dtype=self.compute_dtype
+        )
+
     def _transform_bytes(self, tokens):
         """Map token bytes to unicode using `byte2unicode`."""
         split_bytes = tf.strings.bytes_split(tokens)
         split_unicode = self.byte2unicode.lookup(split_bytes)
         return split_unicode
 
     def _bpe_merge_and_update_cache(self, tokens):
@@ -634,71 +635,7 @@
                 "sequence_length": self.sequence_length,
                 "add_prefix_space": self.add_prefix_space,
                 "unsplittable_tokens": self.unsplittable_tokens,
             }
         )
         return config
 
-    @classproperty
-    def presets(cls):
-        return {}
-
-    @classmethod
-    def from_preset(
-        cls,
-        preset,
-        **kwargs,
-    ):
-        """Instantiate {{model_name}} tokenizer from preset vocabulary.
-
-        Args:
-            preset: string. Must be one of "{{preset_names}}".
-
-        Examples:
-        ```python
-        # Load a preset tokenizer.
-        tokenizer = {{model_name}}.from_preset("{{example_preset_name}}")
-
-        # Tokenize some input.
-        tokenizer("The quick brown fox tripped.")
-
-        # Detokenize some input.
-        tokenizer.detokenize([5, 6, 7, 8, 9])
-        ```
-        """
-        # We support short IDs for official presets, e.g. `"bert_base_en"`.
-        # Map these to a Kaggle Models handle.
-        if preset in cls.presets:
-            preset = cls.presets[preset]["kaggle_handle"]
-
-        config_file = "tokenizer.json"
-        check_preset_class(preset, cls, config_file=config_file)
-        return load_from_preset(
-            preset,
-            config_file=config_file,
-            config_overrides=kwargs,
-        )
-
-    def __init_subclass__(cls, **kwargs):
-        # Use __init_subclass__ to setup a correct docstring for from_preset.
-        super().__init_subclass__(**kwargs)
-
-        # If the subclass does not define from_preset, assign a wrapper so that
-        # each class can have a distinct docstring.
-        if "from_preset" not in cls.__dict__:
-
-            def from_preset(calling_cls, *args, **kwargs):
-                return super(cls, calling_cls).from_preset(*args, **kwargs)
-
-            cls.from_preset = classmethod(from_preset)
-
-        # Format and assign the docstring unless the subclass has overridden it.
-        if cls.from_preset.__doc__ is None:
-            cls.from_preset.__func__.__doc__ = (
-                BytePairTokenizer.from_preset.__doc__
-            )
-            format_docstring(
-                model_name=cls.__name__,
-                example_preset_name=next(iter(cls.presets), ""),
-                preset_names='", "'.join(cls.presets),
-            )(cls.from_preset.__func__)
-
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/byte_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,19 +151,19 @@
     >>> outputs = tokenizer.detokenize(inputs)
     >>> np.array(outputs).astype("U")
     array('heXllo', dtype='<U6')
     """
 
     def __init__(
         self,
-        lowercase: bool = True,
-        sequence_length: int = None,
-        normalization_form: str = None,
-        errors: str = "replace",
-        replacement_char: int = 65533,
+        lowercase=True,
+        sequence_length=None,
+        normalization_form=None,
+        errors="replace",
+        replacement_char=65533,
         dtype="int32",
         **kwargs,
     ):
         assert_tf_text_installed(self.__class__.__name__)
 
         if not is_int_dtype(dtype):
             raise ValueError(
@@ -194,16 +194,16 @@
         self.errors = errors
         self.replacement_char = replacement_char
 
         self._char_lst = tf.constant(
             [i.tobytes() for i in np.arange(256, dtype=np.uint8)]
         )
 
-    def vocabulary_size(self) -> int:
-        """Get the size of the tokenizer vocabulary."""
+    def vocabulary_size(self):
+        """Get the integer size of the tokenizer vocabulary."""
         return 256
 
     def tokenize(self, inputs):
         if not isinstance(inputs, (tf.Tensor, tf.RaggedTensor)):
             inputs = tf.convert_to_tensor(inputs)
 
         scalar_input = inputs.shape.rank == 0
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/models/bloom/bloom_tokenizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,119 +8,110 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.layers.preprocessing.preprocessing_layer import (
-    PreprocessingLayer,
-)
-
-
-@keras_nlp_export("keras_nlp.tokenizers.Tokenizer")
-class Tokenizer(PreprocessingLayer):
-    """A base class for tokenizer layers.
-
-    Tokenizers in the KerasNLP library should all subclass this layer.
-    The class provides two core methods `tokenize()` and `detokenize()` for
-    going from plain text to sequences and back. A tokenizer is a subclass of
-    `keras.layers.Layer` and can be combined into a `keras.Model`.
-
-    Subclassers should always implement the `tokenize()` method, which will also
-    be the default when calling the layer directly on inputs.
-
-    Subclassers can optionally implement the `detokenize()` method if the
-    tokenization is reversible. Otherwise, this can be skipped.
-
-    Subclassers should implement `get_vocabulary()`, `vocabulary_size()`,
-    `token_to_id()` and `id_to_token()` if applicable. For some simple
-    "vocab free" tokenizers, such as a whitespace splitter show below, these
-    methods do not apply and can be skipped.
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 
-    Examples:
-
-    ```python
-    class WhitespaceSplitterTokenizer(keras_nlp.tokenizers.Tokenizer):
-        def tokenize(self, inputs):
-            return tf.strings.split(inputs)
 
-        def detokenize(self, inputs):
-            return tf.strings.reduce_join(inputs, separator=" ", axis=-1)
+@keras_nlp_export("keras_nlp.models.BloomTokenizer")
+class BloomTokenizer(BytePairTokenizer):
+    """A BLOOM tokenizer using Byte-Pair Encoding subword segmentation.
+
+    This tokenizer class will tokenize raw strings into integer sequences and
+    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by BLOOM
+    models and provides a `from_preset()` method to automatically download
+    a matching vocabulary for a BLOOM preset.
+
+    This tokenizer does not provide truncation or padding of inputs.
+
+    If input is a batch of strings (rank > 0), the layer will output a
+    `tf.RaggedTensor` where the last dimension of the output is ragged.
+
+    If input is a scalar string (rank == 0), the layer will output a dense
+    `tf.Tensor` with static shape `[None]`.
+
+    Args:
+        vocabulary: string or dict, maps token to integer ids. If it is a
+            string, it should be the file path to a json file.
+        merges: string or list, contains the merge rule. If it is a string,
+            it should be the file path to merge rules. The merge rule file
+            should have one merge rule per line. Every merge rule contains
+            merge entities separated by a space.
 
-    tokenizer = WhitespaceSplitterTokenizer()
-
-    # Tokenize some inputs.
-    tokenizer.tokenize("This is a test")
-
-    # Shorthard for `tokenize()`.
-    tokenizer("This is a test")
+    Examples:
 
-    # Detokenize some outputs.
-    tokenizer.detokenize(["This", "is", "a", "test"])
+    ```python
+    # Unbatched input.
+    tokenizer = keras_nlp.models.BloomTokenizer.from_preset("bloom_560m_multi")
+    tokenizer("The quick brown fox jumped.")
+
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    vocab = {"<s>": 0, "</s>": 1, "<pad>": 2, "a": 3, "Ġquick": 4, "Ġfox": 5}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.BloomTokenizer(vocabulary=vocab, merges=merges)
+    tokenizer("a quick fox.")
     ```
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def tokenize(self, inputs, *args, **kwargs):
-        """Transform input tensors of strings into output tokens.
-
-        Args:
-            inputs: Input tensor, or dict/list/tuple of input tensors.
-            *args: Additional positional arguments.
-            **kwargs: Additional keyword arguments.
-        """
-        raise NotImplementedError(
-            "No implementation of `tokenize()` was found for "
-            f"{self.__class__.__name__}. All tokenizers should implement "
-            "`tokenize()`."
-        )
-
-    def detokenize(self, inputs, *args, **kwargs):
-        """Transform tokens back into strings.
-
-        Args:
-            inputs: Input tensor, or dict/list/tuple of input tensors.
-            *args: Additional positional arguments.
-            **kwargs: Additional keyword arguments.
-        """
-        raise NotImplementedError(
-            "No implementation of `detokenize()` was found for "
-            f"{self.__class__.__name__}."
-        )
-
-    def get_vocabulary(self) -> List[str]:
-        """Get the tokenizer vocabulary as a list of strings terms."""
-        raise NotImplementedError(
-            "No implementation of `get_vocabulary()` was found for "
-            f"{self.__class__.__name__}."
-        )
-
-    def vocabulary_size(self) -> int:
-        """Returns the total size of the token id space."""
-        raise NotImplementedError(
-            "No implementation of `vocabulary_size()` was found for "
-            f"{self.__class__.__name__}."
-        )
-
-    def id_to_token(self, id: int) -> str:
-        """Convert an integer id to a string token."""
-        raise NotImplementedError(
-            "No implementation of `id_to_token()` was found for "
-            f"{self.__class__.__name__}."
-        )
-
-    def token_to_id(self, token: str) -> int:
-        """Convert a string token to an integer id."""
-        raise NotImplementedError(
-            "No implementation of `token_to_id()` was found for "
-            f"{self.__class__.__name__}."
-        )
-
-    def call(self, inputs, *args, training=None, **kwargs):
-        return self.tokenize(inputs, *args, **kwargs)
+    def __init__(
+        self,
+        vocabulary=None,
+        merges=None,
+        **kwargs,
+    ):
+        self.start_token = "<s>"
+        self.end_token = "</s>"
+        self.pad_token = "<pad>"
+
+        super().__init__(
+            vocabulary=vocabulary,
+            merges=merges,
+            unsplittable_tokens=[
+                self.start_token,
+                self.end_token,
+                self.pad_token,
+            ],
+            **kwargs,
+        )
+
+    def set_vocabulary_and_merges(self, vocabulary, merges):
+        super().set_vocabulary_and_merges(vocabulary, merges)
+
+        if vocabulary is not None:
+            # Check for necessary special tokens.
+            for token in [self.start_token, self.end_token, self.pad_token]:
+                if token not in self.get_vocabulary():
+                    raise ValueError(
+                        f"Cannot find token `'{token}'` in the provided "
+                        f"`vocabulary`. Please provide `'{token}'` in "
+                        "your `vocabulary` or use a pretrained `vocabulary` name."
+                    )
+
+            self.start_token_id = self.token_to_id(self.start_token)
+            self.end_token_id = self.token_to_id(self.end_token)
+            self.pad_token_id = self.token_to_id(self.pad_token)
+        else:
+            self.start_token_id = None
+            self.end_token_id = None
+            self.pad_token_id = None
+
+    def get_config(self):
+        config = super().get_config()
+        # In the constructor, we pass the list of special tokens to the
+        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
+        # delete it from the config here.
+        del config["unsplittable_tokens"]
+        return config
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,22 +202,22 @@
     >>> outputs = tokenizer.detokenize(inputs)
     >>> np.array(outputs).astype("U")
     array('niXnja', dtype='<U6')
     """
 
     def __init__(
         self,
-        sequence_length: int = None,
-        lowercase: bool = True,
-        normalization_form: str = None,
-        errors: str = "replace",
-        replacement_char: int = 65533,
-        input_encoding: str = "UTF-8",
-        output_encoding: str = "UTF-8",
-        vocabulary_size: int = None,
+        sequence_length=None,
+        lowercase=True,
+        normalization_form=None,
+        errors="replace",
+        replacement_char=65533,
+        input_encoding="UTF-8",
+        output_encoding="UTF-8",
+        vocabulary_size=None,
         dtype="int32",
         **kwargs,
     ) -> None:
         assert_tf_text_installed(self.__class__.__name__)
 
         if not is_int_dtype(dtype):
             raise ValueError(
@@ -271,15 +271,15 @@
                 "input_encoding": self.input_encoding,
                 "output_encoding": self.output_encoding,
                 "vocabulary_size": self._vocabulary_size,
             }
         )
         return config
 
-    def vocabulary_size(self) -> int:
+    def vocabulary_size(self):
         """Get the size of the tokenizer vocabulary. None implies no vocabulary
         size was provided"""
         return self._vocabulary_size
 
     def tokenize(self, inputs):
         if not isinstance(inputs, (tf.Tensor, tf.RaggedTensor)):
             inputs = tf.convert_to_tensor(inputs)
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import re
 from typing import Iterable
-from typing import List
 
+import keras
 import tensorflow as tf
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.tokenizers import tokenizer
-from keras_nlp.src.utils.preset_utils import check_preset_class
-from keras_nlp.src.utils.preset_utils import load_from_preset
-from keras_nlp.src.utils.python_utils import classproperty
-from keras_nlp.src.utils.python_utils import format_docstring
 from keras_nlp.src.utils.tensor_utils import assert_tf_text_installed
 from keras_nlp.src.utils.tensor_utils import convert_to_ragged_batch
 from keras_nlp.src.utils.tensor_utils import is_int_dtype
 from keras_nlp.src.utils.tensor_utils import is_string_dtype
 
 try:
     import tensorflow_text as tf_text
@@ -97,20 +94,27 @@
     [
         WHITESPACE_AND_PUNCTUATION_REGEX,
         CJK_REGEX,
     ]
 )
 
 
+def get_special_tokens_pattern(special_tokens):
+    if special_tokens is None or len(special_tokens) == 0:
+        return None
+    return r"|".join([re.escape(token) for token in special_tokens])
+
+
 def pretokenize(
     text,
     lowercase=False,
     strip_accents=True,
     split=True,
     split_on_cjk=True,
+    special_tokens_pattern=None,
 ):
     """Helper function that takes in a dataset element and pretokenizes it.
 
     Args:
         text: `tf.Tensor` or `tf.RaggedTensor`. Input to be pretokenized.
         lowercase: bool. If True, the input text will be
             lowercased before tokenization. Defaults to `True`.
@@ -120,15 +124,22 @@
             whitespace and punctuation marks, and all punctuation marks will be
             kept as tokens. If `False`, input should be split ("pre-tokenized")
             before calling the tokenizer, and passed as a dense or ragged tensor
             of whole words. Defaults to `True`.
         split_on_cjk: bool. If `True`, input will be split
             on CJK characters, i.e., Chinese, Japanese, Korean and Vietnamese
             characters (https://en.wikipedia.org/wiki/CJK_Unified_Ideographs_(Unicode_block)).
-            Note that this is applicable only when `split` is `True`. Defaults to `True`.
+            Note that this is applicable only when `split` is `True`. Defaults
+            to `True`.
+        special_tokens_pattern: str. A regex pattern that contain the
+            special tokens that will never be split during the word-level
+            splitting applied before the word-peice encoding. This can be used
+            to ensure special tokens map to unique indices in the vocabulary,
+            even if these special tokens contain splittable characters such as
+            punctuation.
 
     Returns:
         A tensor containing the pre-processed and pre-tokenized `text`.
     """
     # Check for correct types.
     if not is_string_dtype(text.dtype):
         raise ValueError(
@@ -136,33 +147,60 @@
             f"Received: {text.dtype}."
         )
     # Preprocess, lowercase, strip and split input data.
     if text.shape.rank == 0:
         text = tf.expand_dims(text, 0)
     if split_on_cjk and split:
         text = tf.strings.regex_replace(text, CJK_REGEX, r" \0 ")
-    if lowercase:
-        text = tf_text.case_fold_utf8(text)
     if strip_accents:
         # Normalize unicode to NFD, which splits out accent mark characters.
         text = tf_text.normalize_utf8(text, "NFD")
         # Remove the accent marks.
         text = tf.strings.regex_replace(text, r"\p{Mn}", "")
     if split:
         if split_on_cjk:
             split_pattern = WHITESPACE_PUNCTUATION_AND_CJK_REGEX
             keep_split_pattern = PUNCTUATION_AND_CJK_REGEX
         else:
             split_pattern = WHITESPACE_AND_PUNCTUATION_REGEX
             keep_split_pattern = PUNCTUATION_REGEX
+        if special_tokens_pattern is not None:
+            # the idea here is to pass the special tokens regex to the split
+            # function as delimiter regex pattern, so the input will be splitted
+            # by them, but also the function will treat each on of them as one
+            # entity that shouldn't be splitted even if they have other
+            # delimiter regex pattern inside them. then pass the special tokens
+            # regex also as keep delimiter regex pattern, so they will
+            # not be removed.
+            split_pattern = r"|".join(
+                [
+                    special_tokens_pattern,
+                    split_pattern,
+                ]
+            )
+            keep_split_pattern = r"|".join(
+                [special_tokens_pattern, keep_split_pattern]
+            )
         text = tf_text.regex_split(
             text,
             delim_regex_pattern=split_pattern,
             keep_delim_regex_pattern=keep_split_pattern,
         )
+    if lowercase:
+        if special_tokens_pattern is not None:
+            # Do not lowercase special tokens in string space. They often
+            # contain capital letters, e.g. `"[CLS]"`.
+            mask = (
+                tf.strings.regex_replace(text, special_tokens_pattern, "६")
+                == "६"
+            )
+            text = tf.where(mask, text, tf_text.case_fold_utf8(text))
+        else:
+            text = tf_text.case_fold_utf8(text)
+
     return text
 
 
 @keras_nlp_export("keras_nlp.tokenizers.WordPieceTokenizer")
 class WordPieceTokenizer(tokenizer.Tokenizer):
     """A WordPiece tokenizer layer.
 
@@ -221,14 +259,23 @@
             Defaults to `True`.
         suffix_indicator: str. The characters prepended to a
             WordPiece to indicate that it is a suffix to another subword.
             E.g. "##ing". Defaults to `"##"`.
         oov_token: str. The string value to substitute for
             an unknown token. It must be included in the vocab.
             Defaults to `"[UNK]"`.
+        special_tokens: list. A list of special tokens. when
+            `special_tokens_in_strings` is set to `True`, the tokenizer will map
+            every special token in the input strings to its id, even if these
+            special tokens contain characters that should be splitted before
+            tokenization such as punctuation. `special_tokens` must be included
+            in `vocabulary`.
+        special_tokens_in_strings: bool. A bool to indicate if the tokenizer
+            should expect special tokens in input strings that should be
+            tokenized and mapped correctly to their ids. Defaults to False.
 
     References:
      - [Schuster and Nakajima, 2012](https://research.google/pubs/pub37842/)
      - [Song et al., 2020](https://arxiv.org/abs/2012.15524)
 
     Examples:
 
@@ -292,21 +339,23 @@
     >>> np.array(outputs).astype("U")
     array(['the', 'qu', '##ick', 'br', '##own', 'fox'], dtype='<U5')
     """
 
     def __init__(
         self,
         vocabulary=None,
-        sequence_length: int = None,
-        lowercase: bool = False,
-        strip_accents: bool = False,
-        split: bool = True,
-        split_on_cjk: bool = True,
-        suffix_indicator: str = "##",
-        oov_token: str = "[UNK]",
+        sequence_length=None,
+        lowercase=False,
+        strip_accents=False,
+        split=True,
+        split_on_cjk=True,
+        suffix_indicator="##",
+        oov_token="[UNK]",
+        special_tokens=None,
+        special_tokens_in_strings=False,
         dtype="int32",
         **kwargs,
     ) -> None:
         assert_tf_text_installed(self.__class__.__name__)
 
         if not is_int_dtype(dtype) and not is_string_dtype(dtype):
             raise ValueError(
@@ -321,14 +370,27 @@
         self.sequence_length = sequence_length
         self.lowercase = lowercase
         self.strip_accents = strip_accents
         self.split = split
         self.split_on_cjk = split_on_cjk
         self.suffix_indicator = suffix_indicator
         self.oov_token = oov_token
+        self.special_tokens = special_tokens
+        self._special_tokens_pattern = None
+        if self.split and special_tokens_in_strings:
+            # the idea here is to pass the special tokens regex to the
+            # split function as delimiter regex pattern, so the input will
+            # be splitted by them, but also the function will treat each on
+            # of them as one entity that shouldn't be splitted even if they
+            # have other delimiter regex pattern inside them. then pass the
+            # special tokens regex also as keep delimiter regex
+            # pattern, so they will not be removed.
+            self._special_tokens_pattern = get_special_tokens_pattern(
+                self.special_tokens
+            )
         self.set_vocabulary(vocabulary)
 
     def save_assets(self, dir_path):
         path = os.path.join(dir_path, VOCAB_FILENAME)
         with open(path, "w", encoding="utf-8") as file:
             for token in self.vocabulary:
                 file.write(f"{token}\n")
@@ -361,44 +423,54 @@
                 f'Cannot find `oov_token="{self.oov_token}"` in the '
                 "vocabulary.\n"
                 "You can either update the vocabulary to include "
                 f'`"{self.oov_token}"`, or pass a different value for '
                 "the `oov_token` argument when creating the tokenizer."
             )
 
+        # Check for special tokens in the vocabulary
+        if self.special_tokens is not None:
+            for token in self.special_tokens:
+                if token not in self.vocabulary:
+                    raise ValueError(
+                        f"Cannot find token `'{token}'` in the provided "
+                        f"`vocabulary`. Please provide `'{token}'` in your "
+                        "`vocabulary` or use a pretrained `vocabulary` name."
+                    )
+
         self._fast_word_piece = tf_text.FastWordpieceTokenizer(
             vocab=self.vocabulary,
             token_out_type=self.compute_dtype,
             suffix_indicator=self.suffix_indicator,
             unknown_token=self.oov_token,
             no_pretokenization=True,
             support_detokenization=True,
         )
 
-    def get_vocabulary(self) -> List[str]:
+    def get_vocabulary(self):
         """Get the tokenizer vocabulary as a list of strings tokens."""
         self._check_vocabulary()
         return self.vocabulary
 
-    def vocabulary_size(self) -> int:
-        """Get the size of the tokenizer vocabulary."""
+    def vocabulary_size(self):
+        """Get the integer size of the tokenizer vocabulary."""
         self._check_vocabulary()
         return len(self.vocabulary)
 
-    def id_to_token(self, id: int) -> str:
+    def id_to_token(self, id):
         """Convert an integer id to a string token."""
         self._check_vocabulary()
         if id >= self.vocabulary_size() or id < 0:
             raise ValueError(
                 f"`id` must be in range [0, {self.vocabulary_size() - 1}]. "
                 f"Received: {id}"
             )
         return self.vocabulary[id]
 
-    def token_to_id(self, token: str) -> int:
+    def token_to_id(self, token):
         """Convert a string token to an integer id."""
         # This will be slow, but keep memory usage down compared to building a
         # . Assuming the main use case is looking up a few special tokens
         # early in the vocab, this should be fine.
         self._check_vocabulary()
         return self.vocabulary.index(token)
 
@@ -409,14 +481,15 @@
                 "vocabulary": None,  # Save vocabulary via an asset!
                 "sequence_length": self.sequence_length,
                 "lowercase": self.lowercase,
                 "strip_accents": self.strip_accents,
                 "split": self.split,
                 "suffix_indicator": self.suffix_indicator,
                 "oov_token": self.oov_token,
+                "special_tokens": self.special_tokens,
             }
         )
         return config
 
     def _check_vocabulary(self):
         if self.vocabulary is None:
             raise ValueError(
@@ -432,14 +505,15 @@
         scalar_input = inputs.shape.rank == 0
         inputs = pretokenize(
             inputs,
             self.lowercase,
             self.strip_accents,
             self.split,
             self.split_on_cjk,
+            self._special_tokens_pattern,
         )
 
         # Apply WordPiece and coerce shape for outputs.
         tokens = self._fast_word_piece.tokenize(inputs)
         # By default tf.text tokenizes text with two ragged dimensions (one for
         # split words and one for split subwords). We will collapse to a single
         # ragged dimension which is a better out of box default.
@@ -461,71 +535,12 @@
         self._check_vocabulary()
         inputs, unbatched, _ = convert_to_ragged_batch(inputs)
         outputs = self._fast_word_piece.detokenize(inputs)
         if unbatched:
             outputs = tf.squeeze(outputs, 0)
         return outputs
 
-    @classproperty
-    def presets(cls):
-        return {}
-
-    @classmethod
-    def from_preset(
-        cls,
-        preset,
-        **kwargs,
-    ):
-        """Instantiate {{model_name}} tokenizer from preset vocabulary.
-
-        Args:
-            preset: string. Must be one of "{{preset_names}}".
-
-        Examples:
-        ```python
-        # Load a preset tokenizer.
-        tokenizer = {{model_name}}.from_preset("{{example_preset_name}}")
-
-        # Tokenize some input.
-        tokenizer("The quick brown fox tripped.")
-
-        # Detokenize some input.
-        tokenizer.detokenize([5, 6, 7, 8, 9])
-        ```
-        """
-        # We support short IDs for official presets, e.g. `"bert_base_en"`.
-        # Map these to a Kaggle Models handle.
-        if preset in cls.presets:
-            preset = cls.presets[preset]["kaggle_handle"]
-
-        config_file = "tokenizer.json"
-        check_preset_class(preset, cls, config_file=config_file)
-        return load_from_preset(
-            preset,
-            config_file=config_file,
-            config_overrides=kwargs,
+    def compute_output_spec(self, input_spec):
+        return keras.KerasTensor(
+            input_spec.shape + (self.sequence_length,), dtype=self.compute_dtype
         )
 
-    def __init_subclass__(cls, **kwargs):
-        # Use __init_subclass__ to setup a correct docstring for from_preset.
-        super().__init_subclass__(**kwargs)
-
-        # If the subclass does not define from_preset, assign a wrapper so that
-        # each class can have a distinct docstring.
-        if "from_preset" not in cls.__dict__:
-
-            def from_preset(calling_cls, *args, **kwargs):
-                return super(cls, calling_cls).from_preset(*args, **kwargs)
-
-            cls.from_preset = classmethod(from_preset)
-
-        # Format and assign the docstring unless the subclass has overridden it.
-        if cls.from_preset.__doc__ is None:
-            cls.from_preset.__func__.__doc__ = (
-                WordPieceTokenizer.from_preset.__doc__
-            )
-            format_docstring(
-                model_name=cls.__name__,
-                example_preset_name=next(iter(cls.presets), ""),
-                preset_names='", "'.join(cls.presets),
-            )(cls.from_preset.__func__)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/utils/keras_utils.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/utils/keras_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/utils/tensor_utils.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/utils/tensor_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     jax both lack native types for ragged and string data.
 
     If we encounter one of these types in torch or jax, we will instead covert
     the tensor to simple pythonic types (lists of strings).
     """
     if isinstance(x, tf.RaggedTensor) or getattr(x, "dtype", None) == tf.string:
         return tensor_to_list(x)
-    return ops.convert_to_tensor(x)
+    dtype = getattr(x, "dtype", "float32")
+    dtype = standardize_dtype(dtype)
+    return ops.convert_to_tensor(x, dtype=dtype)
 
 
 def convert_to_ragged_batch(inputs):
     """Convert pythonic or numpy-like input to a 2-D `tf.RaggedTensor`.
 
     This is useful for text preprocessing layers which deal with already
     tokenized or split text.
@@ -167,7 +169,31 @@
 def is_int_dtype(dtype):
     return "int" in standardize_dtype(dtype)
 
 
 def is_string_dtype(dtype):
     return "string" in standardize_dtype(dtype)
 
+
+def any_equal(inputs, values, padding_mask):
+    """Return a mask that is True anywhere `inputs` has a value in `values`.
+
+    Final mask has `padding_mask` applied.
+
+    Args:
+        inputs: Input tensor.
+        values: List or iterable of tensors shaped like `inputs` or broadcastable
+            by bit operators.
+        padding_mask: Tensor with shape compatible with inputs that will condition
+            output.
+
+    Returns:
+        A tensor with `inputs` shape where each position is True if it contains
+            a value from any `values`. Padding mask will be applied before
+            returning."""
+    output = ops.equal(inputs, values[0])
+    for value in values[1:]:
+        value_equality = ops.equal(inputs, value)
+        output = ops.logical_or(output, value_equality)
+
+    return ops.logical_and(output, padding_mask)
+
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/src/version_utils.py` & `keras-nlp-0.9.0.dev0/keras_nlp/src/version_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_nlp.src.api_export import keras_nlp_export
 
 # Unique source of truth for the version number.
-__version__ = "0.8.2.dev0"
+__version__ = "0.9.0.dev0"
 
 
 @keras_nlp_export("keras_nlp.version")
 def version():
     return __version__
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp/tokenizers/__init__.py` & `keras-nlp-0.9.0.dev0/keras_nlp/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp.egg-info/PKG-INFO` & `keras-nlp-0.9.0.dev0/keras_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.8.2.dev0
+Version: 0.9.0.dev0
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nlp-0.8.2.dev0/keras_nlp.egg-info/SOURCES.txt` & `keras-nlp-0.9.0.dev0/keras_nlp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,19 @@
 keras_nlp/src/metrics/edit_distance.py
 keras_nlp/src/metrics/perplexity.py
 keras_nlp/src/metrics/rouge_base.py
 keras_nlp/src/metrics/rouge_l.py
 keras_nlp/src/metrics/rouge_n.py
 keras_nlp/src/models/__init__.py
 keras_nlp/src/models/backbone.py
-keras_nlp/src/models/generative_task.py
+keras_nlp/src/models/causal_lm.py
+keras_nlp/src/models/classifier.py
+keras_nlp/src/models/masked_lm.py
 keras_nlp/src/models/preprocessor.py
+keras_nlp/src/models/seq_2_seq_lm.py
 keras_nlp/src/models/task.py
 keras_nlp/src/models/albert/__init__.py
 keras_nlp/src/models/albert/albert_backbone.py
 keras_nlp/src/models/albert/albert_classifier.py
 keras_nlp/src/models/albert/albert_masked_lm.py
 keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
 keras_nlp/src/models/albert/albert_preprocessor.py
@@ -75,14 +78,15 @@
 keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
 keras_nlp/src/models/bert/bert_preprocessor.py
 keras_nlp/src/models/bert/bert_presets.py
 keras_nlp/src/models/bert/bert_tokenizer.py
 keras_nlp/src/models/bloom/__init__.py
 keras_nlp/src/models/bloom/bloom_attention.py
 keras_nlp/src/models/bloom/bloom_backbone.py
+keras_nlp/src/models/bloom/bloom_causal_lm.py
 keras_nlp/src/models/bloom/bloom_causal_lm_preprocessor.py
 keras_nlp/src/models/bloom/bloom_decoder.py
 keras_nlp/src/models/bloom/bloom_preprocessor.py
 keras_nlp/src/models/bloom/bloom_presets.py
 keras_nlp/src/models/bloom/bloom_tokenizer.py
 keras_nlp/src/models/deberta_v3/__init__.py
 keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
@@ -101,23 +105,33 @@
 keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
 keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
 keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
 keras_nlp/src/models/distil_bert/distil_bert_presets.py
 keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
 keras_nlp/src/models/electra/__init__.py
 keras_nlp/src/models/electra/electra_backbone.py
+keras_nlp/src/models/electra/electra_preprocessor.py
+keras_nlp/src/models/electra/electra_presets.py
 keras_nlp/src/models/electra/electra_tokenizer.py
 keras_nlp/src/models/f_net/__init__.py
 keras_nlp/src/models/f_net/f_net_backbone.py
 keras_nlp/src/models/f_net/f_net_classifier.py
 keras_nlp/src/models/f_net/f_net_masked_lm.py
 keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
 keras_nlp/src/models/f_net/f_net_preprocessor.py
 keras_nlp/src/models/f_net/f_net_presets.py
 keras_nlp/src/models/f_net/f_net_tokenizer.py
+keras_nlp/src/models/falcon/__init__.py
+keras_nlp/src/models/falcon/falcon_attention.py
+keras_nlp/src/models/falcon/falcon_backbone.py
+keras_nlp/src/models/falcon/falcon_causal_lm_preprocessor.py
+keras_nlp/src/models/falcon/falcon_preprocessor.py
+keras_nlp/src/models/falcon/falcon_presets.py
+keras_nlp/src/models/falcon/falcon_tokenizer.py
+keras_nlp/src/models/falcon/falcon_transformer_decoder.py
 keras_nlp/src/models/gemma/__init__.py
 keras_nlp/src/models/gemma/gemma_attention.py
 keras_nlp/src/models/gemma/gemma_backbone.py
 keras_nlp/src/models/gemma/gemma_causal_lm.py
 keras_nlp/src/models/gemma/gemma_causal_lm_preprocessor.py
 keras_nlp/src/models/gemma/gemma_decoder_block.py
 keras_nlp/src/models/gemma/gemma_preprocessor.py
@@ -138,16 +152,20 @@
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_causal_lm_preprocessor.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_decoder.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_preprocessor.py
 keras_nlp/src/models/gpt_neo_x/gpt_neo_x_tokenizer.py
 keras_nlp/src/models/llama/__init__.py
 keras_nlp/src/models/llama/llama_attention.py
 keras_nlp/src/models/llama/llama_backbone.py
+keras_nlp/src/models/llama/llama_causal_lm.py
+keras_nlp/src/models/llama/llama_causal_lm_preprocessor.py
 keras_nlp/src/models/llama/llama_decoder.py
 keras_nlp/src/models/llama/llama_layernorm.py
+keras_nlp/src/models/llama/llama_preprocessor.py
+keras_nlp/src/models/llama/llama_presets.py
 keras_nlp/src/models/llama/llama_tokenizer.py
 keras_nlp/src/models/mistral/__init__.py
 keras_nlp/src/models/mistral/mistral_attention.py
 keras_nlp/src/models/mistral/mistral_backbone.py
 keras_nlp/src/models/mistral/mistral_causal_lm.py
 keras_nlp/src/models/mistral/mistral_causal_lm_preprocessor.py
 keras_nlp/src/models/mistral/mistral_layer_norm.py
```

### Comparing `keras-nlp-0.8.2.dev0/setup.cfg` & `keras-nlp-0.9.0.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.8.2.dev0/setup.py` & `keras-nlp-0.9.0.dev0/setup.py`

 * *Files identical despite different names*

