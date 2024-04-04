# Comparing `tmp/batchalign-0.7.0b0.tar.gz` & `tmp/batchalign-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchalign-0.7.0b0.tar", last modified: Mon Apr  1 06:52:09 2024, max compression
+gzip compressed data, was "batchalign-0.7.0b1.tar", last modified: Thu Apr  4 00:34:08 2024, max compression
```

## Comparing `batchalign-0.7.0b0.tar` & `batchalign-0.7.0b1.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.163445 batchalign-0.7.0b0/
--rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.0b0/LICENSE
--rw-r--r--   0 houjun     (501) staff       (20)      107 2023-12-17 07:44:23.000000 batchalign-0.7.0b0/MANIFEST.in
--rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-01 06:52:09.163226 batchalign-0.7.0b0/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     9384 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/README.md
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.151131 batchalign-0.7.0b0/batchalign/
--rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.0b0/batchalign/__main__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.152221 batchalign-0.7.0b0/batchalign/cli/
--rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.0b0/batchalign/cli/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     9127 2024-04-01 06:42:31.000000 batchalign-0.7.0b0/batchalign/cli/cli.py
--rw-r--r--   0 houjun     (501) staff       (20)     7542 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/cli/dispatch.py
--rw-r--r--   0 houjun     (501) staff       (20)      777 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/constants.py
--rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-03-25 21:38:05.000000 batchalign-0.7.0b0/batchalign/document.py
--rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.0b0/batchalign/errors.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.152430 batchalign-0.7.0b0/batchalign/formats/
--rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/batchalign/formats/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.0b0/batchalign/formats/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.153097 batchalign-0.7.0b0/batchalign/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/batchalign/formats/chat/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     4550 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/batchalign/formats/chat/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3671 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/batchalign/formats/chat/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.0b0/batchalign/formats/chat/lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    12408 2024-03-05 20:11:39.000000 batchalign-0.7.0b0/batchalign/formats/chat/parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-02-09 21:34:57.000000 batchalign-0.7.0b0/batchalign/formats/chat/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.153518 batchalign-0.7.0b0/batchalign/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.0b0/batchalign/formats/textgrid/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/batchalign/formats/textgrid/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.0b0/batchalign/formats/textgrid/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.0b0/batchalign/formats/textgrid/parser.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.153835 batchalign-0.7.0b0/batchalign/models/
--rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      454 2024-03-16 03:57:38.000000 batchalign-0.7.0b0/batchalign/models/resolve.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.154171 batchalign-0.7.0b0/batchalign/models/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:49:26.000000 batchalign-0.7.0b0/batchalign/models/speaker/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/speaker/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.154526 batchalign-0.7.0b0/batchalign/models/training/
--rw-r--r--   0 houjun     (501) staff       (20)       22 2024-03-08 20:19:04.000000 batchalign-0.7.0b0/batchalign/models/training/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/training/run.py
--rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-03-08 20:43:01.000000 batchalign-0.7.0b0/batchalign/models/training/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-03-08 20:19:04.000000 batchalign-0.7.0b0/batchalign/models/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.155213 batchalign-0.7.0b0/batchalign/models/utterance/
--rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/utterance/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/utterance/dataset.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/utterance/execute.py
--rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/utterance/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/utterance/prep.py
--rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/utterance/train.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.155582 batchalign-0.7.0b0/batchalign/models/whisper/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/whisper/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/whisper/infer_asr.py
--rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/models/whisper/infer_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.156015 batchalign-0.7.0b0/batchalign/pipelines/
--rw-r--r--   0 houjun     (501) staff       (20)      404 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/pipelines/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.156246 batchalign-0.7.0b0/batchalign/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/analysis/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/analysis/eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.156867 batchalign-0.7.0b0/batchalign/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)       99 2024-02-16 23:42:52.000000 batchalign-0.7.0b0/batchalign/pipelines/asr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3500 2024-03-16 00:40:13.000000 batchalign-0.7.0b0/batchalign/pipelines/asr/rev.py
--rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-03-16 03:51:34.000000 batchalign-0.7.0b0/batchalign/pipelines/asr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     1866 2024-03-16 03:58:06.000000 batchalign-0.7.0b0/batchalign/pipelines/asr/whisper.py
--rw-r--r--   0 houjun     (501) staff       (20)     4205 2024-03-16 00:40:13.000000 batchalign-0.7.0b0/batchalign/pipelines/asr/whisperx.py
--rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.157420 batchalign-0.7.0b0/batchalign/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/cleanup.py
--rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/disfluencies.py
--rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/parse_support.py
--rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/retrace.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.157744 batchalign-0.7.0b0/batchalign/pipelines/cleanup/support/
--rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/support/filled_pauses.eng
--rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/support/replacements.eng
--rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/pipelines/cleanup/support/test.test
--rw-r--r--   0 houjun     (501) staff       (20)     3786 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/pipelines/dispatch.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.157979 batchalign-0.7.0b0/batchalign/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.0b0/batchalign/pipelines/fa/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     6432 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/fa/whisper_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.158210 batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/
--rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.158343 batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/fr/
--rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/fr/case.py
--rw-r--r--   0 houjun     (501) staff       (20)    28591 2024-03-23 17:56:36.000000 batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/ud.py
--rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/pipelines/pipeline.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.158590 batchalign-0.7.0b0/batchalign/pipelines/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/pipelines/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 05:59:25.000000 batchalign-0.7.0b0/batchalign/pipelines/speaker/nemo_speaker.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.159070 batchalign-0.7.0b0/batchalign/pipelines/utr/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.0b0/batchalign/pipelines/utr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-02-29 21:43:03.000000 batchalign-0.7.0b0/batchalign/pipelines/utr/rev_utr.py
--rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-01-13 18:25:54.000000 batchalign-0.7.0b0/batchalign/pipelines/utr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/pipelines/utr/whisper_utr.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.159375 batchalign-0.7.0b0/batchalign/tests/
--rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.0b0/batchalign/tests/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/conftest.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.149445 batchalign-0.7.0b0/batchalign/tests/formats/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.159922 batchalign-0.7.0b0/batchalign/tests/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-03-18 04:57:15.000000 batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_generator.py
--rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.160037 batchalign-0.7.0b0/batchalign/tests/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/formats/textgrid/test_textgrid.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.160392 batchalign-0.7.0b0/batchalign/tests/pipelines/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.160527 batchalign-0.7.0b0/batchalign/tests/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/analysis/test_eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.160786 batchalign-0.7.0b0/batchalign/tests/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/asr/test_asr_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/asr/test_asr_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.161006 batchalign-0.7.0b0/batchalign/tests/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-03-25 21:40:17.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/cleanup/test_disfluency.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/cleanup/test_parse_support.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.161127 batchalign-0.7.0b0/batchalign/tests/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)      261 2023-12-20 18:33:49.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/fa/test_fa_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/fixures.py
--rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/test_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/pipelines/test_pipeline_models.py
--rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.0b0/batchalign/tests/test_document.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.161569 batchalign-0.7.0b0/batchalign/utils/
--rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.0b0/batchalign/utils/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.0b0/batchalign/utils/config.py
--rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.0b0/batchalign/utils/dp.py
--rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-02-17 06:35:14.000000 batchalign-0.7.0b0/batchalign/utils/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)       43 2024-04-01 06:47:44.000000 batchalign-0.7.0b0/batchalign/version
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-01 06:52:09.161731 batchalign-0.7.0b0/batchalign.egg-info/
--rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-01 06:52:09.000000 batchalign-0.7.0b0/batchalign.egg-info/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     3648 2024-04-01 06:52:09.000000 batchalign-0.7.0b0/batchalign.egg-info/SOURCES.txt
--rw-r--r--   0 houjun     (501) staff       (20)        1 2024-04-01 06:52:09.000000 batchalign-0.7.0b0/batchalign.egg-info/dependency_links.txt
--rw-r--r--   0 houjun     (501) staff       (20)       61 2024-04-01 06:52:09.000000 batchalign-0.7.0b0/batchalign.egg-info/entry_points.txt
--rw-r--r--   0 houjun     (501) staff       (20)      902 2024-04-01 06:52:09.000000 batchalign-0.7.0b0/batchalign.egg-info/requires.txt
--rw-r--r--   0 houjun     (501) staff       (20)       11 2024-04-01 06:52:09.000000 batchalign-0.7.0b0/batchalign.egg-info/top_level.txt
--rw-r--r--   0 houjun     (501) staff       (20)       38 2024-04-01 06:52:09.163476 batchalign-0.7.0b0/setup.cfg
--rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:36:33.000000 batchalign-0.7.0b0/setup.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.505056 batchalign-0.7.0b1/
+-rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.0b1/LICENSE
+-rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.0b1/MANIFEST.in
+-rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-04 00:34:08.504776 batchalign-0.7.0b1/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     9384 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/README.md
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.488713 batchalign-0.7.0b1/batchalign/
+-rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.0b1/batchalign/__main__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.489700 batchalign-0.7.0b1/batchalign/cli/
+-rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.0b1/batchalign/cli/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     9127 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/cli/cli.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7542 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/cli/dispatch.py
+-rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/constants.py
+-rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/document.py
+-rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.0b1/batchalign/errors.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.489920 batchalign-0.7.0b1/batchalign/formats/
+-rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.0b1/batchalign/formats/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.0b1/batchalign/formats/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.490589 batchalign-0.7.0b1/batchalign/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.0b1/batchalign/formats/chat/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4550 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/formats/chat/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3671 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/formats/chat/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.0b1/batchalign/formats/chat/lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    12408 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/formats/chat/parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/formats/chat/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.491053 batchalign-0.7.0b1/batchalign/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.0b1/batchalign/formats/textgrid/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.0b1/batchalign/formats/textgrid/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.0b1/batchalign/formats/textgrid/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.0b1/batchalign/formats/textgrid/parser.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.491395 batchalign-0.7.0b1/batchalign/models/
+-rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/models/resolve.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.491880 batchalign-0.7.0b1/batchalign/models/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/speaker/config.yaml
+-rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/speaker/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/speaker/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.492249 batchalign-0.7.0b1/batchalign/models/training/
+-rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/models/training/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/training/run.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/models/training/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/models/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.492977 batchalign-0.7.0b1/batchalign/models/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/utterance/dataset.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/utterance/execute.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/utterance/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/utterance/prep.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/utterance/train.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.493347 batchalign-0.7.0b1/batchalign/models/whisper/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/whisper/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/whisper/infer_asr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/models/whisper/infer_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.493832 batchalign-0.7.0b1/batchalign/pipelines/
+-rw-r--r--   0 houjun     (501) staff       (20)      404 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/pipelines/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.494059 batchalign-0.7.0b1/batchalign/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/analysis/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/analysis/eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.494604 batchalign-0.7.0b1/batchalign/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/asr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3500 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/asr/rev.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/asr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1866 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/asr/whisper.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4205 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/asr/whisperx.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.495218 batchalign-0.7.0b1/batchalign/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/cleanup.py
+-rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/disfluencies.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/parse_support.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/retrace.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.495552 batchalign-0.7.0b1/batchalign/pipelines/cleanup/support/
+-rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/support/filled_pauses.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/support/replacements.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/pipelines/cleanup/support/test.test
+-rw-r--r--   0 houjun     (501) staff       (20)     3786 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/pipelines/dispatch.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.495770 batchalign-0.7.0b1/batchalign/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.0b1/batchalign/pipelines/fa/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     6432 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/fa/whisper_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.498959 batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/
+-rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.499209 batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/fr/
+-rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/fr/case.py
+-rw-r--r--   0 houjun     (501) staff       (20)    28591 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/ud.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/pipelines/pipeline.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.499486 batchalign-0.7.0b1/batchalign/pipelines/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/pipelines/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/batchalign/pipelines/speaker/nemo_speaker.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.499989 batchalign-0.7.0b1/batchalign/pipelines/utr/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.0b1/batchalign/pipelines/utr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/pipelines/utr/rev_utr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-01-13 18:25:54.000000 batchalign-0.7.0b1/batchalign/pipelines/utr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/pipelines/utr/whisper_utr.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.500378 batchalign-0.7.0b1/batchalign/tests/
+-rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.0b1/batchalign/tests/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/conftest.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.486989 batchalign-0.7.0b1/batchalign/tests/formats/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.501012 batchalign-0.7.0b1/batchalign/tests/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.501135 batchalign-0.7.0b1/batchalign/tests/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/formats/textgrid/test_textgrid.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.501472 batchalign-0.7.0b1/batchalign/tests/pipelines/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.501590 batchalign-0.7.0b1/batchalign/tests/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/analysis/test_eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.501849 batchalign-0.7.0b1/batchalign/tests/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/asr/test_asr_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/asr/test_asr_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.502091 batchalign-0.7.0b1/batchalign/tests/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/cleanup/test_disfluency.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/cleanup/test_parse_support.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.502211 batchalign-0.7.0b1/batchalign/tests/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)      261 2023-12-20 18:33:49.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/fa/test_fa_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/fixures.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/test_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/pipelines/test_pipeline_models.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.0b1/batchalign/tests/test_document.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.502775 batchalign-0.7.0b1/batchalign/utils/
+-rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.0b1/batchalign/utils/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.0b1/batchalign/utils/config.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.0b1/batchalign/utils/dp.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.0b1/batchalign/utils/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)       43 2024-04-04 00:32:54.000000 batchalign-0.7.0b1/batchalign/version
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-04 00:34:08.489380 batchalign-0.7.0b1/batchalign.egg-info/
+-rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-04 00:34:08.000000 batchalign-0.7.0b1/batchalign.egg-info/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     3686 2024-04-04 00:34:08.000000 batchalign-0.7.0b1/batchalign.egg-info/SOURCES.txt
+-rw-r--r--   0 houjun     (501) staff       (20)        1 2024-04-04 00:34:08.000000 batchalign-0.7.0b1/batchalign.egg-info/dependency_links.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       61 2024-04-04 00:34:08.000000 batchalign-0.7.0b1/batchalign.egg-info/entry_points.txt
+-rw-r--r--   0 houjun     (501) staff       (20)      902 2024-04-04 00:34:08.000000 batchalign-0.7.0b1/batchalign.egg-info/requires.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       11 2024-04-04 00:34:08.000000 batchalign-0.7.0b1/batchalign.egg-info/top_level.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       38 2024-04-04 00:34:08.505097 batchalign-0.7.0b1/setup.cfg
+-rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.0b1/setup.py
```

### Comparing `batchalign-0.7.0b0/LICENSE` & `batchalign-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/PKG-INFO` & `batchalign-0.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.0b0
+Version: 0.7.0b1
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.0b0/README.md` & `batchalign-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/cli/cli.py` & `batchalign-0.7.0b1/batchalign/cli/cli.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/cli/dispatch.py` & `batchalign-0.7.0b1/batchalign/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/constants.py` & `batchalign-0.7.0b1/batchalign/constants.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/document.py` & `batchalign-0.7.0b1/batchalign/document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/chat/file.py` & `batchalign-0.7.0b1/batchalign/formats/chat/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/chat/generator.py` & `batchalign-0.7.0b1/batchalign/formats/chat/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/chat/lexer.py` & `batchalign-0.7.0b1/batchalign/formats/chat/lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/chat/parser.py` & `batchalign-0.7.0b1/batchalign/formats/chat/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/chat/utils.py` & `batchalign-0.7.0b1/batchalign/formats/chat/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/textgrid/file.py` & `batchalign-0.7.0b1/batchalign/formats/textgrid/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/textgrid/generator.py` & `batchalign-0.7.0b1/batchalign/formats/textgrid/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/formats/textgrid/parser.py` & `batchalign-0.7.0b1/batchalign/formats/textgrid/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/speaker/infer.py` & `batchalign-0.7.0b1/batchalign/models/speaker/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/speaker/utils.py` & `batchalign-0.7.0b1/batchalign/models/speaker/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/training/run.py` & `batchalign-0.7.0b1/batchalign/models/training/run.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/training/utils.py` & `batchalign-0.7.0b1/batchalign/models/training/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/utils.py` & `batchalign-0.7.0b1/batchalign/models/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/utterance/dataset.py` & `batchalign-0.7.0b1/batchalign/models/utterance/dataset.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/utterance/execute.py` & `batchalign-0.7.0b1/batchalign/models/utterance/execute.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/utterance/infer.py` & `batchalign-0.7.0b1/batchalign/models/utterance/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/utterance/prep.py` & `batchalign-0.7.0b1/batchalign/models/utterance/prep.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/utterance/train.py` & `batchalign-0.7.0b1/batchalign/models/utterance/train.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/whisper/infer_asr.py` & `batchalign-0.7.0b1/batchalign/models/whisper/infer_asr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/models/whisper/infer_fa.py` & `batchalign-0.7.0b1/batchalign/models/whisper/infer_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/analysis/eval.py` & `batchalign-0.7.0b1/batchalign/pipelines/analysis/eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/asr/rev.py` & `batchalign-0.7.0b1/batchalign/pipelines/asr/rev.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/asr/utils.py` & `batchalign-0.7.0b1/batchalign/pipelines/asr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/asr/whisper.py` & `batchalign-0.7.0b1/batchalign/pipelines/asr/whisper.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/asr/whisperx.py` & `batchalign-0.7.0b1/batchalign/pipelines/asr/whisperx.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/base.py` & `batchalign-0.7.0b1/batchalign/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/cleanup/disfluencies.py` & `batchalign-0.7.0b1/batchalign/pipelines/cleanup/disfluencies.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/cleanup/parse_support.py` & `batchalign-0.7.0b1/batchalign/pipelines/cleanup/parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/cleanup/retrace.py` & `batchalign-0.7.0b1/batchalign/pipelines/cleanup/retrace.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/dispatch.py` & `batchalign-0.7.0b1/batchalign/pipelines/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/fa/whisper_fa.py` & `batchalign-0.7.0b1/batchalign/pipelines/fa/whisper_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/fr/case.py` & `batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/fr/case.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/morphosyntax/ud.py` & `batchalign-0.7.0b1/batchalign/pipelines/morphosyntax/ud.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/pipeline.py` & `batchalign-0.7.0b1/batchalign/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/speaker/nemo_speaker.py` & `batchalign-0.7.0b1/batchalign/pipelines/speaker/nemo_speaker.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/utr/rev_utr.py` & `batchalign-0.7.0b1/batchalign/pipelines/utr/rev_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/utr/utils.py` & `batchalign-0.7.0b1/batchalign/pipelines/utr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/pipelines/utr/whisper_utr.py` & `batchalign-0.7.0b1/batchalign/pipelines/utr/whisper_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/conftest.py` & `batchalign-0.7.0b1/batchalign/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_file.py` & `batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_generator.py` & `batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_lexer.py` & `batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_parser.py` & `batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/formats/chat/test_chat_utils.py` & `batchalign-0.7.0b1/batchalign/tests/formats/chat/test_chat_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/formats/textgrid/test_textgrid.py` & `batchalign-0.7.0b1/batchalign/tests/formats/textgrid/test_textgrid.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/analysis/test_eval.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/analysis/test_eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/asr/test_asr_pipeline.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/asr/test_asr_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/asr/test_asr_utils.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/asr/test_asr_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/cleanup/test_disfluency.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/cleanup/test_disfluency.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/cleanup/test_parse_support.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/cleanup/test_parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/fixures.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/fixures.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/test_pipeline.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/pipelines/test_pipeline_models.py` & `batchalign-0.7.0b1/batchalign/tests/pipelines/test_pipeline_models.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/tests/test_document.py` & `batchalign-0.7.0b1/batchalign/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/utils/config.py` & `batchalign-0.7.0b1/batchalign/utils/config.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/utils/dp.py` & `batchalign-0.7.0b1/batchalign/utils/dp.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign/utils/utils.py` & `batchalign-0.7.0b1/batchalign/utils/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/batchalign.egg-info/PKG-INFO` & `batchalign-0.7.0b1/batchalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.0b0
+Version: 0.7.0b1
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.0b0/batchalign.egg-info/SOURCES.txt` & `batchalign-0.7.0b1/batchalign.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 batchalign/formats/textgrid/file.py
 batchalign/formats/textgrid/generator.py
 batchalign/formats/textgrid/parser.py
 batchalign/models/__init__.py
 batchalign/models/resolve.py
 batchalign/models/utils.py
 batchalign/models/speaker/__init__.py
+batchalign/models/speaker/config.yaml
 batchalign/models/speaker/infer.py
 batchalign/models/speaker/utils.py
 batchalign/models/training/__init__.py
 batchalign/models/training/run.py
 batchalign/models/training/utils.py
 batchalign/models/utterance/__init__.py
 batchalign/models/utterance/dataset.py
```

### Comparing `batchalign-0.7.0b0/batchalign.egg-info/requires.txt` & `batchalign-0.7.0b1/batchalign.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b0/setup.py` & `batchalign-0.7.0b1/setup.py`

 * *Files identical despite different names*

