# Comparing `tmp/eis1600-1.6.1.tar.gz` & `tmp/eis1600-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-1.6.1.tar", last modified: Fri Mar 22 22:56:47 2024, max compression
+gzip compressed data, was "eis1600-1.6.2.tar", last modified: Thu Apr  4 14:25:54 2024, max compression
```

## Comparing `eis1600-1.6.1.tar` & `eis1600-1.6.2.tar`

### file list

```diff
@@ -1,153 +1,155 @@
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1046 2023-08-12 14:27:20.000000 eis1600-1.6.1/LICENSE
--rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-03-22 22:56:47.391313 eis1600-1.6.1/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    13595 2024-03-16 19:46:15.000000 eis1600-1.6.1/README.md
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.379313 eis1600-1.6.1/eis1600/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.379313 eis1600-1.6.1/eis1600/bio/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/bio/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7450 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/bio/md_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3998 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/bio/q_tags_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3108 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/bio/topo_tags_to_bio.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.379313 eis1600-1.6.1/eis1600/corpus_analysis/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-06 14:14:46.000000 eis1600-1.6.1/eis1600/corpus_analysis/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5592 2024-03-22 22:07:21.000000 eis1600-1.6.1/eis1600/corpus_analysis/analyse_all_on_cluster.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1732 2024-03-22 08:47:34.000000 eis1600-1.6.1/eis1600/corpus_analysis/analyse_text.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4728 2024-03-22 09:23:55.000000 eis1600-1.6.1/eis1600/corpus_analysis/miu_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3308 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/corpus_analysis/text_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.379313 eis1600-1.6.1/eis1600/dates/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      911 2023-11-02 15:25:23.000000 eis1600-1.6.1/eis1600/dates/Date.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      755 2024-02-12 17:00:08.000000 eis1600-1.6.1/eis1600/dates/Month.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/dates/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6571 2024-03-21 18:00:42.000000 eis1600-1.6.1/eis1600/dates/date_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7397 2024-03-21 17:57:44.000000 eis1600-1.6.1/eis1600/dates/date_patterns.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2237 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/dates/month_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.379313 eis1600-1.6.1/eis1600/gazetteers/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4411 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1267 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/gazetteers/Spellings.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3553 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/gazetteers/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.6.1/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.6.1/eis1600/gazetteers/data/days_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.6.1/eis1600/gazetteers/data/months_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.6.1/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1448 2023-10-25 09:16:34.000000 eis1600-1.6.1/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)   339886 2023-11-06 12:34:27.000000 eis1600-1.6.1/eis1600/gazetteers/data/toponyms_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.6.1/eis1600/gazetteers/data/years_gazetteer.csv
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/helper/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3429 2024-03-22 08:56:31.000000 eis1600-1.6.1/eis1600/helper/CheckFileEndingActions.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      186 2023-11-10 14:22:15.000000 eis1600-1.6.1/eis1600/helper/Singleton.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/helper/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1212 2024-02-19 13:06:34.000000 eis1600-1.6.1/eis1600/helper/ar_normalization.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3934 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/helper/chunking.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/helper/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.1/eis1600/helper/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1356 2024-03-18 17:41:21.000000 eis1600-1.6.1/eis1600/helper/files_sizes.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      994 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/helper/logging.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6461 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      370 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/helper/parse_range.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      306 2024-03-21 11:13:13.000000 eis1600-1.6.1/eis1600/helper/part_file_names.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/json_to_text/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:40:12.000000 eis1600-1.6.1/eis1600/json_to_text/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2504 2024-03-22 13:26:51.000000 eis1600-1.6.1/eis1600/json_to_text/reconstruct.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/json_to_tsv/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:34:00.000000 eis1600-1.6.1/eis1600/json_to_tsv/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4731 2024-03-22 13:11:46.000000 eis1600-1.6.1/eis1600/json_to_tsv/corpus_dump.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/markdown/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      988 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/markdown/EntityTags.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/markdown/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/markdown/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.1/eis1600/markdown/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-02-07 09:59:48.000000 eis1600-1.6.1/eis1600/markdown/data/entity_tags.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      851 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/markdown/markdown_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6551 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/markdown/markdown_patterns.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/miu/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3513 2024-02-13 09:24:54.000000 eis1600-1.6.1/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/miu/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.383313 eis1600-1.6.1/eis1600/model_evaluations/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      393 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/model_evaluations/EvalResultsEncoder.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/model_evaluations/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7701 2024-02-12 17:00:08.000000 eis1600-1.6.1/eis1600/model_evaluations/eval_date_model.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4800 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/model_evaluations/eval_topo_cat_model.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.387313 eis1600-1.6.1/eis1600/models/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      671 2024-02-05 08:54:18.000000 eis1600-1.6.1/eis1600/models/BiosPunctuationModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      566 2024-02-13 10:55:51.000000 eis1600-1.6.1/eis1600/models/Disambiguator.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      660 2024-02-12 17:00:08.000000 eis1600-1.6.1/eis1600/models/EventsPunctuationModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      259 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/models/FamilyContactOpinionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      592 2024-02-13 10:55:51.000000 eis1600-1.6.1/eis1600/models/Lemmatizer.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1762 2024-02-05 08:54:18.000000 eis1600-1.6.1/eis1600/models/Model.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      237 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/models/NERModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      250 2024-02-01 10:44:02.000000 eis1600-1.6.1/eis1600/models/NasabDetectionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      257 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/models/OnomsticElementsModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      582 2024-02-13 10:55:51.000000 eis1600-1.6.1/eis1600/models/POSTagger.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1154 2024-02-16 15:42:32.000000 eis1600-1.6.1/eis1600/models/PoetryDetectionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      258 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/models/StudentTeacherModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      261 2023-11-20 09:22:09.000000 eis1600-1.6.1/eis1600/models/ToponymDescriptionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      246 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/models/ToponymModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-20 09:22:09.000000 eis1600-1.6.1/eis1600/models/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.387313 eis1600-1.6.1/eis1600/nlp/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/nlp/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4464 2024-02-16 15:40:22.000000 eis1600-1.6.1/eis1600/nlp/annotation_utils.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1604 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/nlp/utils.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.387313 eis1600-1.6.1/eis1600/onomastics/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/onomastics/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1364 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/onomastics/initial_annotation.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    10575 2024-02-12 17:00:08.000000 eis1600-1.6.1/eis1600/onomastics/methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1968 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.387313 eis1600-1.6.1/eis1600/paragraphs/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/paragraphs/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     9974 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/paragraphs/paragraph_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2163 2024-02-16 15:42:32.000000 eis1600-1.6.1/eis1600/paragraphs/split_mius_into_paragraphs.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.387313 eis1600-1.6.1/eis1600/processing/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/processing/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5513 2024-03-22 10:18:48.000000 eis1600-1.6.1/eis1600/processing/postprocessing.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6230 2024-02-19 09:55:38.000000 eis1600-1.6.1/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.387313 eis1600-1.6.1/eis1600/repositories/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/repositories/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    16476 2024-03-22 09:46:46.000000 eis1600-1.6.1/eis1600/repositories/repo.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/eis1600/texts_to_mius/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      431 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/texts_to_mius/SubIDs.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1820 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/texts_to_mius/UIDs.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/texts_to_mius/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1939 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/texts_to_mius/check_formatting.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7303 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/texts_to_mius/check_formatting_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3696 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/texts_to_mius/check_mius.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3742 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/texts_to_mius/convert_mARkdown_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4179 2024-02-05 08:54:18.000000 eis1600-1.6.1/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1562 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/texts_to_mius/download_text_selection_sheet.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3312 2024-03-16 19:46:15.000000 eis1600-1.6.1/eis1600/texts_to_mius/ids_insert_or_update.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1463 2024-03-01 13:50:55.000000 eis1600-1.6.1/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    13825 2024-02-20 09:13:15.000000 eis1600-1.6.1/eis1600/texts_to_mius/subid_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/eis1600/toponym_descriptions/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/toponym_descriptions/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/toponym_descriptions/annotate_topd.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2783 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/toponym_descriptions/btopd_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4944 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/toponym_descriptions/topod_extract_incomplete.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4151 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/toponym_descriptions/topod_extract_places_regex.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3709 2024-02-16 15:42:32.000000 eis1600-1.6.1/eis1600/toponym_descriptions/topod_insert_into_miu.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1710 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/toponym_descriptions/topod_sheets_stats.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/eis1600/toponyms/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.1/eis1600/toponyms/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1975 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/toponyms/initial_category_annotation.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3199 2023-11-02 14:43:12.000000 eis1600-1.6.1/eis1600/toponyms/methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1659 2023-11-02 14:43:12.000000 eis1600-1.6.1/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/eis1600/training_data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/training_data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1535 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/training_data/annotate_onomastics.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1098 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/training_data/online_editor_files.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4121 2024-01-30 08:39:34.000000 eis1600-1.6.1/eis1600/training_data/reannotation.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/eis1600/yml/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     9274 2024-03-01 13:31:17.000000 eis1600-1.6.1/eis1600/yml/YAMLHandler.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/yml/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    12654 2024-03-22 09:40:57.000000 eis1600-1.6.1/eis1600/yml/yml_handling.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-01-18 10:18:32.000000 eis1600-1.6.1/eis1600/yml/yml_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-03-22 22:56:47.391313 eis1600-1.6.1/eis1600.egg-info/
--rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-03-22 22:56:47.000000 eis1600-1.6.1/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4395 2024-03-22 22:56:47.000000 eis1600-1.6.1/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2024-03-22 22:56:47.000000 eis1600-1.6.1/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1770 2024-03-22 22:56:47.000000 eis1600-1.6.1/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      201 2024-03-22 22:56:47.000000 eis1600-1.6.1/eis1600.egg-info/requires.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        8 2024-03-22 22:56:47.000000 eis1600-1.6.1/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2024-03-22 22:56:47.391313 eis1600-1.6.1/setup.cfg
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3930 2024-03-22 22:56:01.000000 eis1600-1.6.1/setup.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1046 2023-08-12 14:27:20.000000 eis1600-1.6.2/LICENSE
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-04-04 14:25:54.176272 eis1600-1.6.2/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    13595 2024-03-16 19:46:15.000000 eis1600-1.6.2/README.md
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.160272 eis1600-1.6.2/eis1600/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/bio/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7450 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/md_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3998 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/q_tags_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3108 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/topo_tags_to_bio.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/corpus_analysis/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-06 14:14:46.000000 eis1600-1.6.2/eis1600/corpus_analysis/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5545 2024-03-27 16:37:17.000000 eis1600-1.6.2/eis1600/corpus_analysis/analyse_all_on_cluster.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1732 2024-03-22 08:47:34.000000 eis1600-1.6.2/eis1600/corpus_analysis/analyse_text.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5156 2024-04-04 09:50:23.000000 eis1600-1.6.2/eis1600/corpus_analysis/miu_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3335 2024-03-27 16:36:35.000000 eis1600-1.6.2/eis1600/corpus_analysis/text_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/dates/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      911 2023-11-02 15:25:23.000000 eis1600-1.6.2/eis1600/dates/Date.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      755 2024-02-12 17:00:08.000000 eis1600-1.6.2/eis1600/dates/Month.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/dates/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6571 2024-03-21 18:00:42.000000 eis1600-1.6.2/eis1600/dates/date_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7397 2024-03-21 17:57:44.000000 eis1600-1.6.2/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2237 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/dates/month_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/gazetteers/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4411 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1267 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/gazetteers/Spellings.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3553 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/gazetteers/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.6.2/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.6.2/eis1600/gazetteers/data/days_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.6.2/eis1600/gazetteers/data/months_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.6.2/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1448 2023-10-25 09:16:34.000000 eis1600-1.6.2/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)   339886 2023-11-06 12:34:27.000000 eis1600-1.6.2/eis1600/gazetteers/data/toponyms_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.6.2/eis1600/gazetteers/data/years_gazetteer.csv
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/helper/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3429 2024-03-22 08:56:31.000000 eis1600-1.6.2/eis1600/helper/CheckFileEndingActions.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      186 2023-11-10 14:22:15.000000 eis1600-1.6.2/eis1600/helper/Singleton.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/helper/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1212 2024-02-19 13:06:34.000000 eis1600-1.6.2/eis1600/helper/ar_normalization.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3934 2024-03-27 11:22:04.000000 eis1600-1.6.2/eis1600/helper/chunking.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/helper/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.2/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1356 2024-03-18 17:41:21.000000 eis1600-1.6.2/eis1600/helper/files_sizes.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2027 2024-04-04 11:02:16.000000 eis1600-1.6.2/eis1600/helper/fix_dataframe.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      994 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/helper/logging.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6461 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      370 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/helper/parse_range.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      306 2024-03-21 11:13:13.000000 eis1600-1.6.2/eis1600/helper/part_file_names.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/json_to_text/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:40:12.000000 eis1600-1.6.2/eis1600/json_to_text/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4106 2024-04-04 10:56:08.000000 eis1600-1.6.2/eis1600/json_to_text/reconstruct.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/json_to_tsv/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:34:00.000000 eis1600-1.6.2/eis1600/json_to_tsv/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4912 2024-04-04 08:53:33.000000 eis1600-1.6.2/eis1600/json_to_tsv/corpus_dump.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/markdown/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      988 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/markdown/EntityTags.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/markdown/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1606 2024-04-03 11:51:57.000000 eis1600-1.6.2/eis1600/markdown/category.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/markdown/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.2/eis1600/markdown/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-02-07 09:59:48.000000 eis1600-1.6.2/eis1600/markdown/data/entity_tags.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      851 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/markdown/markdown_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6628 2024-04-03 09:08:42.000000 eis1600-1.6.2/eis1600/markdown/markdown_patterns.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/miu/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3513 2024-02-13 09:24:54.000000 eis1600-1.6.2/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/miu/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/model_evaluations/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      393 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/model_evaluations/EvalResultsEncoder.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/model_evaluations/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7701 2024-02-12 17:00:08.000000 eis1600-1.6.2/eis1600/model_evaluations/eval_date_model.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4800 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/model_evaluations/eval_topo_cat_model.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/models/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      671 2024-02-05 08:54:18.000000 eis1600-1.6.2/eis1600/models/BiosPunctuationModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      566 2024-02-13 10:55:51.000000 eis1600-1.6.2/eis1600/models/Disambiguator.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      660 2024-02-12 17:00:08.000000 eis1600-1.6.2/eis1600/models/EventsPunctuationModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      259 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/FamilyContactOpinionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      592 2024-02-13 10:55:51.000000 eis1600-1.6.2/eis1600/models/Lemmatizer.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1762 2024-02-05 08:54:18.000000 eis1600-1.6.2/eis1600/models/Model.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      237 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/NERModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      250 2024-02-01 10:44:02.000000 eis1600-1.6.2/eis1600/models/NasabDetectionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      257 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/OnomsticElementsModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      582 2024-02-13 10:55:51.000000 eis1600-1.6.2/eis1600/models/POSTagger.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1154 2024-02-16 15:42:32.000000 eis1600-1.6.2/eis1600/models/PoetryDetectionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      258 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/StudentTeacherModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      261 2023-11-20 09:22:09.000000 eis1600-1.6.2/eis1600/models/ToponymDescriptionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      246 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/ToponymModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-20 09:22:09.000000 eis1600-1.6.2/eis1600/models/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/nlp/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/nlp/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4464 2024-04-03 13:59:59.000000 eis1600-1.6.2/eis1600/nlp/annotation_utils.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1604 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/nlp/utils.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/onomastics/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1364 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/onomastics/initial_annotation.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    10640 2024-04-03 11:14:52.000000 eis1600-1.6.2/eis1600/onomastics/methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1968 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/paragraphs/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/paragraphs/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     9974 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/paragraphs/paragraph_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2163 2024-02-16 15:42:32.000000 eis1600-1.6.2/eis1600/paragraphs/split_mius_into_paragraphs.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/processing/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/processing/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5802 2024-04-04 10:38:59.000000 eis1600-1.6.2/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6230 2024-04-03 13:24:21.000000 eis1600-1.6.2/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/repositories/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/repositories/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    16545 2024-04-04 08:50:01.000000 eis1600-1.6.2/eis1600/repositories/repo.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/texts_to_mius/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      431 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/texts_to_mius/SubIDs.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1820 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/texts_to_mius/UIDs.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/texts_to_mius/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1939 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/texts_to_mius/check_formatting.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7572 2024-04-03 09:09:16.000000 eis1600-1.6.2/eis1600/texts_to_mius/check_formatting_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3696 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/texts_to_mius/check_mius.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3742 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4179 2024-02-05 08:54:18.000000 eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1562 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/texts_to_mius/download_text_selection_sheet.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3312 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/texts_to_mius/ids_insert_or_update.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1463 2024-03-01 13:50:55.000000 eis1600-1.6.2/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    14062 2024-04-03 11:49:39.000000 eis1600-1.6.2/eis1600/texts_to_mius/subid_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/toponym_descriptions/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/toponym_descriptions/annotate_topd.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2783 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/btopd_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4944 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_incomplete.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4151 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_places_regex.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3709 2024-02-16 15:42:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_insert_into_miu.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1710 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_sheets_stats.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/toponyms/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1975 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/toponyms/initial_category_annotation.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3199 2023-11-02 14:43:12.000000 eis1600-1.6.2/eis1600/toponyms/methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1659 2023-11-02 14:43:12.000000 eis1600-1.6.2/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/training_data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1535 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/annotate_onomastics.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1098 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/online_editor_files.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4121 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/reannotation.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/yml/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     9610 2024-04-03 15:04:40.000000 eis1600-1.6.2/eis1600/yml/YAMLHandler.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/yml/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    12671 2024-04-04 08:44:59.000000 eis1600-1.6.2/eis1600/yml/yml_handling.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/yml/yml_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600.egg-info/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1770 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      201 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        8 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2024-04-04 14:25:54.176272 eis1600-1.6.2/setup.cfg
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3930 2024-04-04 14:25:31.000000 eis1600-1.6.2/setup.py
```

### Comparing `eis1600-1.6.1/LICENSE` & `eis1600-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/PKG-INFO` & `eis1600-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 1.6.1
+Version: 1.6.2
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-1.6.1/README.md` & `eis1600-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/bio/md_to_bio.py` & `eis1600-1.6.2/eis1600/bio/md_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/bio/q_tags_to_bio.py` & `eis1600-1.6.2/eis1600/bio/q_tags_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/bio/topo_tags_to_bio.py` & `eis1600-1.6.2/eis1600/bio/topo_tags_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/corpus_analysis/analyse_all_on_cluster.py` & `eis1600-1.6.2/eis1600/corpus_analysis/analyse_all_on_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,27 +56,26 @@
     if parallel:
         res += p_uimap(partial(analyse_miu, debug=debug), mius_list)
     else:
         for idx, tup in tqdm(list(enumerate(mius_list))):
             try:
                 res.append(analyse_miu(tup, debug))
             except ValueError as e:
-                uid, miu_as_text, analyse_flag = tup
+                uid, *_ = tup
                 error += f'{uid}\n{e}\n\n\n'
             except Exception:
                 raise
 
     dir_path, _ = os.path.split(out_path)
     Path(dir_path).mkdir(parents=True, exist_ok=True)
 
-    #FIXME remove original too !!!!!
     # if file is original or part 1, remove previous json files to avoid problem with previous chunkings
     if clean_out_dir and (PART_NAME_INFIX not in out_path or int(PART_NUM_REGEX.search(out_path).group(1)) == 1):
         if os.path.exists(dir_path):
-            for json_file in glob.iglob(f"{dir_path}*.json"):
+            for json_file in glob.iglob(os.path.join(dir_path, "*.json")):
                 os.remove(json_file)
 
     with open(out_path, 'w', encoding='utf-8') as fh:
         jsonpickle.set_encoder_options('json', indent=4, ensure_ascii=False)
         json_str = jsonpickle.encode(res, unpicklable=False)
         fh.write(json_str)
```

### Comparing `eis1600-1.6.1/eis1600/corpus_analysis/analyse_text.py` & `eis1600-1.6.2/eis1600/corpus_analysis/analyse_text.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/corpus_analysis/miu_methods.py` & `eis1600-1.6.2/eis1600/corpus_analysis/miu_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 from eis1600.bio.md_to_bio import bio_to_md
 from eis1600.dates.date_methods import date_annotate_miu_text
 from eis1600.nlp.annotation_utils import annotate_miu_text, insert_onom_tag, insert_onomastic_tags
 from eis1600.nlp.utils import aggregate_STFCON_classes, merge_ner_with_person_classes, merge_ner_with_toponym_classes
 from eis1600.processing.postprocessing import merge_tagslists, reconstruct_miu_text_with_tags
 from eis1600.processing.preprocessing import get_yml_and_miu_df
 from eis1600.yml.yml_handling import add_annotated_entities_to_yml, add_statistics_to_yml
+from eis1600.markdown.category import Category, CategoryType
+from eis1600.helper.fix_dataframe import fix_bonom_position
 
 
-def analyse_miu(tup: Tuple[str, str, bool], debug: Optional[bool] = False) -> Dict:
+def analyse_miu(tup: Tuple[str, str, Category], debug: Optional[bool] = False) -> Dict:
     """Analysis the miu with our models.
 
     This methods applies our models to the text of the MIU and thereby runs different analysis (NER, POS, LEMMAS,
     ROOTS, TOPONYMS, PERSONS, ONOMASTICS, DATES). Results are added to the df representation of the MIU. Returns a
     JSON object which contains yml information, as well as the df with all analysis results.
-    :param Tuple tup: Params are given as a Tuple: (uid: str, miu_as_text: str, analyse_flag: bool).
+    :param Tuple tup: Params are given as a Tuple: (uid: str, miu_as_text: str, category: Category).
     :param bool debug: Optional flag to print debug statements
     :return Dict: JSON representation of the miu, including yml header and analysis results.
     """
-    uid, miu_as_text, analyse_flag = tup
+    uid, miu_as_text, miu_category = tup
 
     # 1. open miu file and disassemble the file to its parts
     if debug:
         print('1. open miu file and disassemble the file to its parts')
     yml_handler, df = get_yml_and_miu_df(miu_as_text)
 
-    if analyse_flag:
+    if miu_category.type != CategoryType.EXTERNAl:
         # 2. annotate NEs, POS and lemmatize. NE are: person + relation(s), toponym + relation, onomastic information
         if debug:
             print('2. annotate NEs, POS and lemmatize. NE are: person + relation(s), toponym + relation, onomastic information')
         df['NER_LABELS'], df['LEMMAS'], df['POS_TAGS'], df['ROOTS'], ST_labels, FCO_labels, \
             df['TOPONYM_LABELS'] = annotate_miu_text(df, debug)
 
         # 3. convert cameltools labels format to markdown format
@@ -46,22 +48,27 @@
 
         # 4. annotate dates
         if debug:
             print('4. annotate dates')
         df['DATE_TAGS'] = date_annotate_miu_text(df[['TOKENS']], uid, yml_handler)
         df['MONTH_TAGS'] = month_annotate_miu_text(df[['TOKENS']], uid)
 
-        # 5. insert BONOM and EONOM tags with the pretrained transformer model
-        df['ONOM_TAGS'] = insert_onom_tag(df, debug)
+        if miu_category.type == CategoryType.BIOGRAPHY:
+            # 5. insert BONOM and EONOM tags with the pretrained transformer model
+            df['ONOM_TAGS'] = insert_onom_tag(df, debug)
+
+            # 6. annotate onomastic information
+            df['ONOMASTIC_TAGS'] = insert_onomastic_tags(df, debug)
+
+            # if there is a BONOM value in ONOM_TAGS and a sections in the previous and following token,
+            # move the BONOM to the next token
+            df = fix_bonom_position(df)
 
-        # 6. annotate onomastic information
-        df['ONOMASTIC_TAGS'] = insert_onomastic_tags(df, debug)
-
-        # TODO 6. disambiguation of toponyms (same toponym, different places) --> replace ambiguous toponyms flag
-        # TODO 9. get frequencies of unidentified entities (toponyms, nisbas)
+            # TODO 6. disambiguation of toponyms (same toponym, different places) --> replace ambiguous toponyms flag
+            # TODO 9. get frequencies of unidentified entities (toponyms, nisbas)
 
         # 11. reconstruct the text, populate yml with annotated entities and save it to the output file
         if debug:
             print('Reconstruct the text, populate yml with annotated entities and save it to the output file')
         columns_of_automated_tags = ['DATE_TAGS', 'MONTH_TAGS', 'ONOM_TAGS', 'ONOMASTIC_TAGS', 'NER_TAGS']
         for col in columns_of_automated_tags:
             if col in df.columns:
```

### Comparing `eis1600-1.6.1/eis1600/corpus_analysis/text_methods.py` & `eis1600-1.6.2/eis1600/corpus_analysis/text_methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import List, Tuple
 
 from eis1600.markdown.markdown_patterns import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
     MIU_UID_TAG_PATTERN, PAGE_TAG_PATTERN
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.texts_to_mius.check_formatting_methods import check_file_for_mal_formatting
 from eis1600.yml.yml_handling import create_yml_header
+from eis1600.markdown.category import Category
 
 
-def get_text_as_list_of_mius(infile: str) -> Tuple[str, List[Tuple[str, str, bool]]]:
+def get_text_as_list_of_mius(infile: str) -> Tuple[str, List[Tuple[str, str, Category]]]:
     """Disassemble text into list of MIUs.
 
     Splits the texts into individual MIUs and returns a list of all contained MIUs.
     :param str infile: File which will be disassembled.
     :return List[Tuple[str, str, bool]]: returns the individual MIUs as tuples of (uid, miu_text, analysis_flag).
     """
     heading_tracker = HeadingTracker()
@@ -44,34 +45,34 @@
                     m = HEADING_PATTERN.match(text_line)
                     heading_text = m.group('heading')
                     if PAGE_TAG_PATTERN.search(heading_text):
                         heading_text = PAGE_TAG_PATTERN.sub('', heading_text)
                     heading_tracker.track_headings(len(m.group('level')), heading_text)
                 if miu_text:
                     # Do not create a preface MIU file if there is no preface
-                    mius.append((uid, miu_text + '\n', analyse_flag))
+                    mius.append((uid, miu_text + '\n', miu_category))
                 m = MIU_TAG_PATTERN.match(text_line)
                 uid = uri + '.' + m.group('UID')
                 category = ''
                 try:
                     category = CATEGORY_PATTERN.search(m.group('category')).group(0)
                 except AttributeError:
                     mal_formatted.append(f"Category not recognised: {m.group(0)}\n")
                 yml_header = create_yml_header(category, heading_tracker.get_curr_state())
-                analyse_flag = category not in ['|PARATEXT|', '|EDITOR|']
+                miu_category = Category(category)
                 miu_text = yml_header
                 miu_text += text_line
             else:
                 miu_text += text_line
 
             if PAGE_TAG_PATTERN.search(text_line):
                 heading_tracker.track_pages(PAGE_TAG_PATTERN.search(text_line).group(0))
 
         # last MIU needs to be appended after the for-loop is finished
-        mius.append((uid, miu_text + '\n', analyse_flag))
+        mius.append((uid, miu_text + '\n', miu_category))
 
     if mal_formatted:
         print('Something seems to be mal-formatted, check:')
         print(infile)
         for elem in mal_formatted:
             print(elem)
```

### Comparing `eis1600-1.6.1/eis1600/dates/Date.py` & `eis1600-1.6.2/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/dates/Month.py` & `eis1600-1.6.2/eis1600/dates/Month.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/dates/date_methods.py` & `eis1600-1.6.2/eis1600/dates/date_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/dates/date_patterns.py` & `eis1600-1.6.2/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/dates/month_methods.py` & `eis1600-1.6.2/eis1600/dates/month_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/Onomastics.py` & `eis1600-1.6.2/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/Spellings.py` & `eis1600-1.6.2/eis1600/gazetteers/Spellings.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/Toponyms.py` & `eis1600-1.6.2/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/data/days_gazetteer.csv` & `eis1600-1.6.2/eis1600/gazetteers/data/days_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/data/months_gazetteer.csv` & `eis1600-1.6.2/eis1600/gazetteers/data/months_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-1.6.2/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-1.6.2/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-1.6.2/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/gazetteers/data/years_gazetteer.csv` & `eis1600-1.6.2/eis1600/gazetteers/data/years_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/helper/CheckFileEndingActions.py` & `eis1600-1.6.2/eis1600/helper/CheckFileEndingActions.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/helper/ar_normalization.py` & `eis1600-1.6.2/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/helper/chunking.py` & `eis1600-1.6.2/eis1600/helper/chunking.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/helper/files_sizes.py` & `eis1600-1.6.2/eis1600/helper/files_sizes.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/helper/logging.py` & `eis1600-1.6.2/eis1600/helper/logging.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/helper/miu_random_revisions.py` & `eis1600-1.6.2/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/json_to_tsv/corpus_dump.py` & `eis1600-1.6.2/eis1600/json_to_tsv/corpus_dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os.path
-
 import jsonpickle
-from sys import argv
 import ujson as json
 import pandas as pd
+from pathlib import Path
+from sys import argv
 from tqdm import tqdm
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 
-from eis1600.repositories.repo import get_ready_and_double_checked_files, TEXT_REPO, JSON_REPO, COLUMNS, SEP, SEP2
+from eis1600.repositories.repo import get_ready_and_double_checked_files, TEXT_REPO, JSON_REPO, TSV_REPO, COLUMNS, \
+    SEP, SEP2
 from eis1600.helper.CheckFileEndingActions import CheckFileEndingEIS1600JsonAction
 
 
 ALL_LABELS = ("SECTIONS", "TOKENS", "TAGS_LISTS", "NER_LABELS", "LEMMAS", "POS_TAGS", "ROOTS", "TOPONYM_LABELS",
               "NER_TAGS", "DATE_TAGS", "MONTH_TAGS", "ONOM_TAGS", "ONOMASTIC_TAGS")
 
 
@@ -69,14 +70,18 @@
                 if type(value) == list:
                     value = SEP2.join(value)
                 if value:
                     content_data.append((uid, entity, f"{j}{SEP}{value}"))
 
     fbase, _ = os.path.splitext(fpath)
 
+    fbase = fbase.replace(JSON_REPO, TSV_REPO)
+    dir_path, _ = os.path.split(fbase)
+    Path(dir_path).mkdir(parents=True, exist_ok=True)
+
     content_df = pd.DataFrame(content_data, columns=COLUMNS)
     content_df.to_csv(f"{fbase}_df.tsv", sep="\t", index=False)
 
     struct_df = pd.DataFrame(structural_data, columns=COLUMNS)
     struct_df.to_csv(f"{fbase}_yml.tsv", sep="\t", index=False)
```

### Comparing `eis1600-1.6.1/eis1600/markdown/EntityTags.py` & `eis1600-1.6.2/eis1600/markdown/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/markdown/markdown_methods.py` & `eis1600-1.6.2/eis1600/markdown/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/markdown/markdown_patterns.py` & `eis1600-1.6.2/eis1600/markdown/markdown_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 UID_WITHOUT_CAPTURING_GROUP = r'\d{12}(?:-\d{8})?'
 UID_TAG = r'_ء_(#)?=' + UID + '= '
 UID_TAG_PATTERN = compile(UID_TAG)
 MIU_UID_TAG = r'_ء_#=(?P<UID>\d{12})= '
 MIU_UID_TAG_WITHOUT_CAPTURING_GROUP = r'_ء_#=\d{12}= '
 MIU_UID_TAG_PATTERN = compile(MIU_UID_TAG)
 MIU_SPLITTER_PATTERN = compile(r'(?:^|\n\n)(?=' + MIU_UID_TAG + ')')
-PARAGRAPH_CAT = '::(?P<cat>[A-Z_]+)::'
+PARAGRAPH_CAT = '::(?P<cat>[A-Z_]+(?::: ::[A-Z_]+)*)::'
 PARAGRAPH_CAT_PATTERN = compile(PARAGRAPH_CAT)
 PARAGRAPH_CAT_WITHOUT_CAPTURING_GROUPS = '::[A-Z_]+::'
 PARAGRAPH_SIMPLE_SPLITTER_PATTERN = compile('\n\n(' + PARAGRAPH_CAT_WITHOUT_CAPTURING_GROUPS + ')\n')
 PARAGRAPH_UID_TAG = r'_ء_=' + UID_WITHOUT_CAPTURING_GROUP + '= ' + PARAGRAPH_CAT + ' ~'
 PARAGRAPH_UID_TAG_WITHOUT_CAPTURING_GROUPS = r'_ء_=' + UID_WITHOUT_CAPTURING_GROUP + '= ' + PARAGRAPH_CAT_WITHOUT_CAPTURING_GROUPS + ' ~'
 PARAGRAPH_UID_TAG_PATTERN = compile(PARAGRAPH_UID_TAG)
 HEADER_END_PATTERN = compile(r'(#META#Header#End#)\n')
@@ -112,9 +112,11 @@
 PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN = compile(
         '(' + AR_STR + ' ?)' + r'\n\n' + PAGE_TAG + r'\n\n' + '(' + AR_STR +
         ')'
 )
 NORMALIZE_BIO_CHR_MD_PATTERN = compile('# ([$@]((BIO|CHR)_[A-Z]+[$@])| RAW)')
 BIO_CHR_TO_NEWLINE_PATTERN = compile(TAG_AND_TEXT_SAME_LINE)
 
+SECTION_KEYWORDS_WITHOUT_SPACE = compile("[A-Z]::::[A-Z]")
+
 # Fixed poetry old file path pattern
 FIXED_POETRY_OLD_PATH_PATTERN = compile(r'/Users/romanov/_OpenITI/_main_corpus/\w+/data/')
```

### Comparing `eis1600-1.6.1/eis1600/miu/HeadingTracker.py` & `eis1600-1.6.2/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/model_evaluations/eval_date_model.py` & `eis1600-1.6.2/eis1600/model_evaluations/eval_date_model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/model_evaluations/eval_topo_cat_model.py` & `eis1600-1.6.2/eis1600/model_evaluations/eval_topo_cat_model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/BiosPunctuationModel.py` & `eis1600-1.6.2/eis1600/models/BiosPunctuationModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/Disambiguator.py` & `eis1600-1.6.2/eis1600/models/Disambiguator.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/EventsPunctuationModel.py` & `eis1600-1.6.2/eis1600/models/EventsPunctuationModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/Lemmatizer.py` & `eis1600-1.6.2/eis1600/models/Lemmatizer.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/Model.py` & `eis1600-1.6.2/eis1600/models/Model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/POSTagger.py` & `eis1600-1.6.2/eis1600/models/POSTagger.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/models/PoetryDetectionModel.py` & `eis1600-1.6.2/eis1600/models/PoetryDetectionModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/nlp/annotation_utils.py` & `eis1600-1.6.2/eis1600/nlp/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/nlp/utils.py` & `eis1600-1.6.2/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/onomastics/initial_annotation.py` & `eis1600-1.6.2/eis1600/onomastics/initial_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/onomastics/methods.py` & `eis1600-1.6.2/eis1600/onomastics/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from eis1600.gazetteers.Toponyms import Toponyms
 from eis1600.helper.logging import setup_logger
 from eis1600.onomastics.re_pattern import ABI, ABU, BN_BNT, CRF_PATTERN, IBN_IBNA, SHR_PATTERN, SPELLING, UMM
 from eis1600.processing.postprocessing import write_updated_miu_to_file
 from eis1600.processing.preprocessing import get_tokens_and_tags, get_yml_and_miu_df
 from eis1600.repositories.repo import GAZETTEERS_REPO
 from eis1600.yml.YAMLHandler import YAMLHandler
+from eis1600.markdown.category import BIO_MAN, BIO_REP
 
 __log_filename = GAZETTEERS_REPO + 'logs/nasab_unknown.log'
 makedirs(dirname(__log_filename), exist_ok=True)
 LOGGER_NASAB_UNKNOWN = setup_logger('nasab_unknown', __log_filename)
 
 
 def get_nas(text: str) -> str:
@@ -234,18 +235,18 @@
     :param str file: Path of the miu file to annotate.
     :param bool test: Indicating if the script is run with test data, defaults to false.
     """
     with open(file, 'r', encoding='utf-8') as miu_file_object:
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
     if test:
         # Only used if run on training_data batch because this information is missing there
-        if '$' not in df.iat[0]['SECTIONS'] or '$$$' in df.iat[0]['SECTIONS'] or not yml_handler.is_reviewed():
+        if BIO_MAN not in df.iat[0]['SECTIONS'] or BIO_REP in df.iat[0]['SECTIONS'] or not yml_handler.is_reviewed():
             df['ONOM_TAGS'] = Series([nan] * len(df))
         else:
-            yml_handler.set_category('$')
+            yml_handler.set_category(BIO_MAN)
             df['ONOM_TAGS'] = nasab_annotate_miu(df, yml_handler, file, test)
     else:
         # Run on new data batch
         df['ONOM_TAGS'] = nasab_annotate_miu(df, yml_handler, file, test)
     yml_handler.unset_reviewed()
 
     if test:
```

### Comparing `eis1600-1.6.1/eis1600/onomastics/re_pattern.py` & `eis1600-1.6.2/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/paragraphs/paragraph_methods.py` & `eis1600-1.6.2/eis1600/paragraphs/paragraph_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/paragraphs/split_mius_into_paragraphs.py` & `eis1600-1.6.2/eis1600/paragraphs/split_mius_into_paragraphs.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/processing/postprocessing.py` & `eis1600-1.6.2/eis1600/processing/postprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,19 @@
         text_and_tags_iter = text_and_tags.itertuples(index=False)
     else:
         text_and_tags_iter = text_and_tags.__iter__()
     heading, _, _ = next(text_and_tags_iter)
     reconstructed_text = heading
     for section, token, tags in text_and_tags_iter:
         if notna(section):
-            reconstructed_text += '\n\n' + section + '\n_ء_'
+            if token and notna(token):
+                reconstructed_text += '\n\n' + section + '\n_ء_'
+            else:
+                reconstructed_text += '\n\n' + section
+
         if isinstance(tags, list):
             reconstructed_text += ' ' + ' '.join(tags)
         elif tags is not None:
             print("df['TAGS_LISTS'] must be list but is " + type(tags))
             print(tags)
             raise TypeError
         if notna(token):
@@ -93,33 +97,37 @@
         return None
 
 
 def write_updated_miu_to_file(
         miu_file_object: TextIO,
         yml_handler: YAMLHandler,
         df: DataFrame,
-        forced_re_annotation: Optional[bool] = False
+        target_columns: tuple[str],
+        forced_re_annotation: Optional[bool] = False,
+        add_annotations_to_yml: Optional[bool] = True
 ) -> None:
     """Write MIU file with annotations and populated YAML header.
 
     :param TextIO miu_file_object: Path to the MIU file to write
     :param YAMLHandler yml_handler: The YAMLHandler of the MIU.
     :param DataFrame df: df containing the columns ['SECTIONS', 'TOKENS', 'TAGS_LISTS'].
+    :param tuple target_columns: columns to include in reconstructed text.
     :param bool forced_re_annotation: some annotation was added to already existing annotation, therefore merge new
     annotation into TAGS_LISTS.
+    :param bool add_annotations_to_yml: add all annotations to yml header.
     :return None:
     """
     if not yml_handler.is_reviewed() or forced_re_annotation:
-        columns_of_automated_tags = ['DATE_TAGS', 'ONOM_TAGS', 'ONOMASTIC_TAGS', 'NER_TAGS']
-        for col in columns_of_automated_tags:
+        for col in target_columns:
             if col in df.columns:
                 df['TAGS_LISTS'] = df.apply(merge_tagslists, key=col, axis=1)
         df_subset = df[['SECTIONS', 'TOKENS', 'TAGS_LISTS']]
     else:
         df_subset = df[['SECTIONS', 'TOKENS', 'TAGS_LISTS']]
 
-    add_annotated_entities_to_yml(df_subset, yml_handler, path.realpath(miu_file_object.name), df_subset)
+    if add_annotations_to_yml:
+        add_annotated_entities_to_yml(df_subset, yml_handler, path.realpath(miu_file_object.name), df_subset)
     updated_text = reconstruct_miu_text_with_tags(df_subset)
 
     miu_file_object.seek(0)
     miu_file_object.write(str(yml_handler) + updated_text)
     miu_file_object.truncate()
```

### Comparing `eis1600-1.6.1/eis1600/processing/preprocessing.py` & `eis1600-1.6.2/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/repositories/repo.py` & `eis1600-1.6.2/eis1600/repositories/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 # Path variables
 
 MIU_REPO = 'EIS1600_MIUs/'
 TEXT_REPO = 'OpenITI_EIS1600_Texts/'
 NEW_PARAGRAPHS_REPO_ERROR_LOG = 'OpenITI_EIS1600_Texts_New_Paragraphs/error_log/'
 NEW_PARAGRAPHS_REPO = 'OpenITI_EIS1600_Texts_New_Paragraphs/'
 JSON_REPO = 'EIS1600_JSONs/'
+TSV_REPO = 'EIS1600_TSVs/'
+RECONSTRUCTED_REPO = 'EIS1600_Reconstructed/'
 PRETRAINED_MODELS_REPO = 'EIS1600_Pretrained_Models/'
 TOPO_REPO = 'Topo_Data/'
 TRAINING_DATA_REPO = 'Training_Data/'
 RESEARCH_DATA_REPO = 'Research_Data/'
 TRAINING_RESULTS_REPO = 'Training_Results/'
 GAZETTEERS_REPO = 'gazetteers/'
 MC_REPO = 'MasterChronicle/'
 BACKEND_REPO = 'backend/'
 TOPO_TRAINING_REPO = 'topo_training/data/'
 POETRY_TEST_RES_REPO = 'POETRY_TEST_RESULTS/'
 
 PART_NAME_INFIX = '_part'
-RECONSTRUCTED_INFIX = '_reconstructed'
+RECONSTRUCTED_INFIX = '_assembled'
 
 PART_NUM_REGEX = re.compile(fr"{PART_NAME_INFIX}0+([0-9]+)")
 
 # columns for tsv output
 COLUMNS = ["MIUID", "ENTITY", "VALUE"]
 
 # separators for tsv containing annotated tokens
```

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/UIDs.py` & `eis1600-1.6.2/eis1600/texts_to_mius/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/check_formatting.py` & `eis1600-1.6.2/eis1600/texts_to_mius/check_formatting.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/check_formatting_methods.py` & `eis1600-1.6.2/eis1600/texts_to_mius/check_formatting_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import remove
 from os.path import splitext, exists
 from itertools import zip_longest
 from eis1600.markdown.markdown_patterns import MIU_UID_TAG_AND_TEXT_SAME_LINE_PATTERN, \
     NEW_LINE_BUT_NO_EMPTY_LINE_PATTERN, NEW_LINE_INSIDE_PARAGRAPH_NOT_POETRY_PATTERN, PARAGRAPH_TAG_MISSING, \
     EMPTY_PARAGRAPH_CHECK_PATTERN, SIMPLE_MARKDOWN, MISSING_DIRECTIONALITY_TAG_PATTERN, SPAN_ELEMENTS, \
     TEXT_START_PATTERN, TILDA_HICKUPS_PATTERN, HEADER_END_PATTERN, CATEGORY_PATTERN, MIU_TAG_PATTERN
-from eis1600.markdown.markdown_patterns import SIMPLE_MARKDOWN_TEXT_START_PATTERN
+from eis1600.markdown.markdown_patterns import SIMPLE_MARKDOWN_TEXT_START_PATTERN, SECTION_KEYWORDS_WITHOUT_SPACE
 from eis1600.repositories.repo import get_part_filepath
 
 
 def check_file_for_mal_formatting(infile: str, content: str):
     errors = []
 
     for line in content.splitlines():
@@ -17,15 +17,17 @@
             try:
                 CATEGORY_PATTERN.search(m.group('category')).group(0)
             except AttributeError:
                 errors.append(f"** Category not recognised in \"{m.group(0)}\"")
 
     # Poetry is still to messed up, do not bother with it for now
     # or POETRY_ATTACHED_AFTER_PAGE_TAG.search(content):
-
+    if SECTION_KEYWORDS_WITHOUT_SPACE.search(content):
+        errors.append("the text seems to contain keywords that are not separated."
+                      "Check for :::: and add a space in between \":: ::\"")
     if not TEXT_START_PATTERN.match(content):
         errors.append('* Text does not start with an MIU tag, check if the preface is tagged as PARATEXT.')
     if m := PARAGRAPH_TAG_MISSING.search(content):
         errors.append(f'* There are missing paragraph tags. Failed at "{m.group(0)}"')
     if m := SIMPLE_MARKDOWN.search(content):
         errors.append(f'* There is simple mARkdown left. Failed at "{m.group(0)}"')
     if m := NEW_LINE_BUT_NO_EMPTY_LINE_PATTERN.search(content):
@@ -36,23 +38,25 @@
                       f'`ids_insert_or_update` on {infile}. Failed at "{m.group(0)}"')
     if m := TILDA_HICKUPS_PATTERN.search(content):
         errors.append(f'* There is this pattern with tildes: `~\\n~`. Failed at "{m.group(0)}"')
     if m := NEW_LINE_INSIDE_PARAGRAPH_NOT_POETRY_PATTERN.search(content):
         errors.append('* There is a single newline inside a paragraph (somewhere the emtpy line is missing). '
                       f'Failed at "{m.group(0)}"')
     if m := EMPTY_PARAGRAPH_CHECK_PATTERN.search(content):
-        errors.append(f'* There are empty paragraphs in the text. Failed at "{m.group(0)}"')
+        context = content[m.span()[0] - 50:m.span()[1] + 50]
+        err = f'\n * There are empty paragraphs in the text. Failed at "{m.group(0)}".\n' \
+              f'Failed position with more context = "{context}"'
+        errors.append(err)
     if m := SPAN_ELEMENTS.search(content):
         errors.append(f'* There are span elements in the text. Failed at "{m.group(0)}"')
     if m := MISSING_DIRECTIONALITY_TAG_PATTERN.search(content):
         errors.append('* There are missing direction tags at the beginning of paragraphs, fix it by running '
                       f'`ids_insert_or_update` on {infile}. Failed at "{m.group(0)}"')
     # if POETRY_ATTACHED_AFTER_PAGE_TAG.search(content):
     #     errors.append('* There is poetry attached to a PageTag (there should be a linebreak instead).')
-
     if errors:
         errors_str = "\n".join(errors)
         raise ValueError(
             f'Correct the following errors\n'
             f'open -a kate {infile}\n'
             f'kate {infile}\n'
             f'{errors_str}\n\n'
@@ -69,37 +73,36 @@
         try:
             check_file_for_mal_formatting(infile, header_text[1])
         except ValueError:
             raise
 
 
 def check_formatting_before_update_ids(infile: str, content: str):
-    if not TEXT_START_PATTERN.match(content) and not SIMPLE_MARKDOWN_TEXT_START_PATTERN.match(content) \
-            or NEW_LINE_BUT_NO_EMPTY_LINE_PATTERN.search(content) \
-            or TILDA_HICKUPS_PATTERN.search(content) \
-            or NEW_LINE_INSIDE_PARAGRAPH_NOT_POETRY_PATTERN.search(content) \
-            or EMPTY_PARAGRAPH_CHECK_PATTERN.search(content) \
-            or SPAN_ELEMENTS.search(content):
-
-        error = ''
-        if not TEXT_START_PATTERN.match(content) and not SIMPLE_MARKDOWN_TEXT_START_PATTERN.match(content):
-            error += f'\n * Text does not start with Header or PARATEXT, check if the preface is tagged.'
-        if m := NEW_LINE_BUT_NO_EMPTY_LINE_PATTERN.search(content):
-            error += f'\n * There are elements missing the double newline (somewhere the emtpy line is missing). ' \
-                     f'Failed at "{m.group(0)}"'
-        if m := TILDA_HICKUPS_PATTERN.search(content):
-            error += f'\n * There is this pattern with tildes: `~\\n~`. Failed at "{m.group(0)}"'
-        if m := NEW_LINE_INSIDE_PARAGRAPH_NOT_POETRY_PATTERN.search(content):
-            error += f'\n * There is a single newline inside a paragraph (somewhere the emtpy line is missing). ' \
-                     f'Failed at "{m.group(0)}"'
-        if m := EMPTY_PARAGRAPH_CHECK_PATTERN.search(content):
-            error += f'\n * There are empty paragraphs in the text. Failed at "{m.group(0)}"'
-        if m := SPAN_ELEMENTS.search(content):
-            error += f'\n * There are span elements in the text. Failed at "{m.group(0)}"'
+    error = ''
+    if SECTION_KEYWORDS_WITHOUT_SPACE.search(content):
+        error += "the text seems to contain keywords that are not separated."\
+                 "Check for :::: and add a space in between \":: ::\""
+    if not TEXT_START_PATTERN.match(content) and not SIMPLE_MARKDOWN_TEXT_START_PATTERN.match(content):
+        error += f'\n * Text does not start with Header or PARATEXT, check if the preface is tagged.'
+    if m := NEW_LINE_BUT_NO_EMPTY_LINE_PATTERN.search(content):
+        error += f'\n * There are elements missing the double newline (somewhere the emtpy line is missing). ' \
+                 f'Failed at "{m.group(0)}"'
+    if m := TILDA_HICKUPS_PATTERN.search(content):
+        error += f'\n * There is this pattern with tildes: `~\\n~`. Failed at "{m.group(0)}"'
+    if m := NEW_LINE_INSIDE_PARAGRAPH_NOT_POETRY_PATTERN.search(content):
+        error += f'\n * There is a single newline inside a paragraph (somewhere the emtpy line is missing). ' \
+                 f'Failed at "{m.group(0)}"'
+    if m := EMPTY_PARAGRAPH_CHECK_PATTERN.search(content):
+        context = content[m.span()[0]-50:m.span()[1]+50]
+        error += f'\n * There are empty paragraphs in the text. Failed at "{m.group(0)}".\n'\
+                 f'Failed position with more context = "{context}"'
+    if m := SPAN_ELEMENTS.search(content):
+        error += f'\n * There are span elements in the text. Failed at "{m.group(0)}"'
 
+    if error:
         raise ValueError(
             f'Correct the following errors\n'
             f'open -a kate {infile}\n'
             f'kate {infile}\n'
             f'{error}\n\n'
             f'And now run\n'
             f'ids_insert_or_update {infile}\n'
```

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/check_mius.py` & `eis1600-1.6.2/eis1600/texts_to_mius/check_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/convert_mARkdown_methods.py` & `eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/download_text_selection_sheet.py` & `eis1600-1.6.2/eis1600/texts_to_mius/download_text_selection_sheet.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/ids_insert_or_update.py` & `eis1600-1.6.2/eis1600/texts_to_mius/ids_insert_or_update.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py` & `eis1600-1.6.2/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/texts_to_mius/subid_methods.py` & `eis1600-1.6.2/eis1600/texts_to_mius/subid_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     HEADER_END_PATTERN, \
     MIU_SPLITTER_PATTERN, MIU_UID_TAG_PATTERN, SIMPLE_HEADING_OR_BIO_PATTERN, MISSING_DIRECTIONALITY_TAG_PATTERN, \
     MIU_TAG_AND_TEXT_PATTERN, \
     NEWLINES_CROWD_PATTERN, \
     NEW_LINE_BUT_NO_EMPTY_LINE_PATTERN, ONLY_PAGE_TAG_PATTERN, PAGE_TAG_IN_BETWEEN_PATTERN, \
     PAGE_TAG_ON_NEWLINE_TMP_PATTERN, PAGE_TAG_PATTERN, \
     PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN, UID_TAG_PATTERN, MIU_UID_TAG_AND_TEXT_SAME_LINE_PATTERN, \
-    PARAGRAPH_UID_TAG_PATTERN
+    PARAGRAPH_UID_TAG_PATTERN, MIU_TAG_PATTERN
+from eis1600.markdown.category import convert_to_longer_bio_tag
 from eis1600.texts_to_mius.SubIDs import SubIDs
 from eis1600.texts_to_mius.UIDs import UIDs
 from eis1600.texts_to_mius.check_formatting_methods import check_formatting_before_update_ids
 
 
 def pre_clean_text(text: str) -> str:
     text = NEWLINES_CROWD_PATTERN.sub('\n\n', text)
@@ -255,14 +256,17 @@
                     raise ValueError(
                             'There is an empty paragraph, check with\n'
                             '::\\n[^هسءگؤقأذپيمجثاڤوضآرتنكزفبعٱشىصلدطغإـئظحةچخ_]'
                     )
                 paragraph = f'_ء_={sub_ids.get_id()}= {section_header} ~\n' + paragraph
             elif not MIU_UID_TAG_PATTERN.match(paragraph):
                 paragraph = f'_ء_={sub_ids.get_id()}= ::UNDEFINED:: ~\n' + paragraph
+            else:
+                if "$" in MIU_TAG_PATTERN.match(paragraph).group(3):
+                    paragraph = convert_to_longer_bio_tag(paragraph)
 
             text_updated.append(paragraph)
 
     # 5. Reassemble text
     text = '\n\n'.join(text_updated)
     return text
```

### Comparing `eis1600-1.6.1/eis1600/toponym_descriptions/annotate_topd.py` & `eis1600-1.6.2/eis1600/toponym_descriptions/annotate_topd.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponym_descriptions/btopd_to_bio.py` & `eis1600-1.6.2/eis1600/toponym_descriptions/btopd_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponym_descriptions/topod_extract_incomplete.py` & `eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_incomplete.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponym_descriptions/topod_extract_places_regex.py` & `eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_places_regex.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponym_descriptions/topod_insert_into_miu.py` & `eis1600-1.6.2/eis1600/toponym_descriptions/topod_insert_into_miu.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponym_descriptions/topod_sheets_stats.py` & `eis1600-1.6.2/eis1600/toponym_descriptions/topod_sheets_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponyms/initial_category_annotation.py` & `eis1600-1.6.2/eis1600/toponyms/initial_category_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponyms/methods.py` & `eis1600-1.6.2/eis1600/toponyms/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/toponyms/toponym_categories.py` & `eis1600-1.6.2/eis1600/toponyms/toponym_categories.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/training_data/annotate_onomastics.py` & `eis1600-1.6.2/eis1600/training_data/annotate_onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/training_data/online_editor_files.py` & `eis1600-1.6.2/eis1600/training_data/online_editor_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/training_data/reannotation.py` & `eis1600-1.6.2/eis1600/training_data/reannotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/eis1600/yml/YAMLHandler.py` & `eis1600-1.6.2/eis1600/yml/YAMLHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from decimal import Decimal
 from typing import Any, Dict, Optional
 
 from ast import literal_eval
 
 from eis1600.markdown.markdown_patterns import MIU_HEADER
+from eis1600.markdown.category import Category
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.yml.yml_methods import dict_to_yaml
 
 
 class YAMLHandler:
     """A class to take care of the MIU YAML Headers
 
@@ -21,17 +22,31 @@
     :ivar List[str] dates_headings: List of dates tags contained in headings.
     :ivar List[int] dates: List of dates contained in the text.
     :ivar Dict onomstics: contains onomastic elements by category.
     :ivar str category: String categorising the type of the entry, bio, chr, dict, etc.
     """
     # Only attributes named in the following list are allowed to be added to the YAMLHeader - add any new attribute
     # to that list
-    __attr_from_annotation = ['dates', 'min_date', 'max_date', 'ages', 'onomastics', 'ambiguous_toponyms', 'persons',
-                              'toponyms', 'settlements', 'provinces', 'edges_settlements', 'edges_provinces',
-                              'books', 'miscs']
+    __attr_from_annotation = [
+        'dates',
+        'min_date',
+        'max_date',
+        'lunar_months',
+        'ages',
+        'onomastics',
+        'ambiguous_toponyms',
+        'persons',
+        'toponyms',
+        'settlements',
+        'provinces',
+        'edges_settlements',
+        'edges_provinces',
+        'books',
+        'miscs'
+    ]
 
     @staticmethod
     def __parse_yml_val(val: str) -> Any:
         if val.isdigit():
             return int(val)
         if len(val.split('.')) == 2 and val.split('.')[0].isdigit() and val.split('.')[1].isdigit():
             return float(val)
@@ -109,15 +124,15 @@
 
         # This is fix for old files, nas should be part of onomastics
         if hasattr(yml, 'nas'):
             delattr(yml, 'nas')
 
         return yml
 
-    def __init__(self, yml: Optional[Dict] = None) -> None:
+    def __init__(self, yml: Optional[Dict] = None, ignore_annotations: bool = False) -> None:
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = 'RESEARCHER'
         self.category = None
         self.headings = None
         self.dates_headings = None
         self.number_of_tokens = None
 
@@ -130,15 +145,19 @@
         if yml:
             for key, val in yml.items():
                 if key == 'headings':
                     val = HeadingTracker(val)
                 if key == 'ambigious':
                     # Fix typo
                     key = 'ambiguous'
-                self.__setattr__(key, val)
+                if ignore_annotations:
+                    if key not in YAMLHandler.__attr_from_annotation:
+                        self.__setattr__(key, val)
+                else:
+                    self.__setattr__(key, val)
 
     @classmethod
     def from_yml_str(cls, yml_str: str) -> YAMLHandler:
         """Return instance with attr set from the yml_str."""
         return cls(YAMLHandler.__parse_yml(yml_str))
 
     def set_category(self, category: str) -> None:
@@ -196,15 +215,15 @@
                         raise TypeError(
                             f'{val} is of type {type(val)} which is not pickable - make sure to use int '
                             f'or float'
                             )
         return json_dict
 
     def is_bio(self) -> bool:
-        return self.category == '$' or self.category == '$$'
+        return Category(self.category).is_bio()
 
     def is_reviewed(self) -> bool:
         return self.reviewed.startswith('REVIEWED')
 
     def add_date_headings(self, date: int) -> None:
         if self.dates_headings:
             if date not in self.dates_headings:
```

### Comparing `eis1600-1.6.1/eis1600/yml/yml_handling.py` & `eis1600-1.6.2/eis1600/yml/yml_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 from typing import Dict, List, Optional, Set, Tuple, Union, Iterator
 
 from itertools import combinations
 from operator import itemgetter
 from os import makedirs
 from os.path import dirname, split, splitext
 
@@ -140,22 +141,21 @@
         index = index_tuple[0]
         tag = row['entity']
         length = int(row['length'])
         sub_cat = row['sub_cat']
         try:
             entity = ' '.join(df['TOKENS'].iloc[index:index + length].to_list())
         except TypeError:
-            print(f'Something is at odd here: {row["full_tag"]}\nCheck: {file_path}')
-            yml_handler.set_error_while_collecting_annotated_entities(row["full_tag"])
-            return
+            print(f'Entity {" ".join(df["TOKENS"].iloc[index:index + length].replace(np.nan, ""))}'
+                  f' with tag {row["full_tag"]} seem to be splitted between two sections.'
+                  f' It has been added to the first section.\nCheck: {file_path}')
+            entity = ' '.join(df['TOKENS'].iloc[index:index + length].replace(np.nan, '').to_list())
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
 
         if cat == 'DATE' or cat == 'LUNAR_MONTH' or cat == 'AGE':
-            # TODO what about the month? ATM, they are not collected into the yml. If you want to change that,
-            #  add 'month' (or maybe lunar_month) to YAMLHandler line 27!
             try:
                 val, e_cat = get_yrs_tag_value(row['full_tag'])
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
                 print(
                         f'Tag is neither year nor age: {row["full_tag"]}\nCheck: {file_path}\n'
                         f'{reconstructed_miu_text_with_tags}'
```

### Comparing `eis1600-1.6.1/eis1600.egg-info/PKG-INFO` & `eis1600-1.6.2/eis1600.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 1.6.1
+Version: 1.6.2
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-1.6.1/eis1600.egg-info/SOURCES.txt` & `eis1600-1.6.2/eis1600.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,25 +36,27 @@
 eis1600/gazetteers/data/years_gazetteer.csv
 eis1600/helper/CheckFileEndingActions.py
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
 eis1600/helper/chunking.py
 eis1600/helper/files_sizes.py
+eis1600/helper/fix_dataframe.py
 eis1600/helper/logging.py
 eis1600/helper/miu_random_revisions.py
 eis1600/helper/parse_range.py
 eis1600/helper/part_file_names.py
 eis1600/helper/data/__init__.py
 eis1600/json_to_text/__init__.py
 eis1600/json_to_text/reconstruct.py
 eis1600/json_to_tsv/__init__.py
 eis1600/json_to_tsv/corpus_dump.py
 eis1600/markdown/EntityTags.py
 eis1600/markdown/__init__.py
+eis1600/markdown/category.py
 eis1600/markdown/markdown_methods.py
 eis1600/markdown/markdown_patterns.py
 eis1600/markdown/data/__init__.py
 eis1600/markdown/data/entity_tags.csv
 eis1600/miu/HeadingTracker.py
 eis1600/miu/__init__.py
 eis1600/model_evaluations/EvalResultsEncoder.py
```

### Comparing `eis1600-1.6.1/eis1600.egg-info/entry_points.txt` & `eis1600-1.6.2/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.1/setup.py` & `eis1600-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='1.6.1',
+      version='1.6.2',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

