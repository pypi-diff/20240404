# Comparing `tmp/mteb-1.5.1.tar.gz` & `tmp/mteb-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.5.1.tar", last modified: Wed Apr  3 12:30:54 2024, max compression
+gzip compressed data, was "mteb-1.5.2.tar", last modified: Thu Apr  4 12:49:30 2024, max compression
```

## Comparing `mteb-1.5.1.tar` & `mteb-1.5.2.tar`

### file list

```diff
@@ -1,371 +1,371 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.661619 mteb-1.5.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-03 12:30:50.000000 mteb-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-03 12:30:54.661619 mteb-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9190 2024-04-03 12:30:50.000000 mteb-1.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.605618 mteb-1.5.1/mteb/
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.605618 mteb-1.5.1/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     6430 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13124 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/tasks/BitextMining/da/
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2194 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/BitextMining/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/Classification/da/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2505 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2937 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/Classification/en/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1485 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     1823 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6075 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/nb/
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/nb/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/nb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/pl/
--rw-r--r--   0 root         (0) root         (0)     4892 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/pl/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/sv/
--rw-r--r--   0 root         (0) root         (0)     1037 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/sv/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/sv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/zh/
--rw-r--r--   0 root         (0) root         (0)     6535 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/zh/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1249 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.621618 mteb-1.5.1/mteb/tasks/Clustering/de/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.621618 mteb-1.5.1/mteb/tasks/Clustering/en/
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1055 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1096 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/es/
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/es/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/fr/
--rw-r--r--   0 root         (0) root         (0)     1905 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1619 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2499 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/nb/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3590 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/nb/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/pl/
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/pl/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/sv/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/zh/
--rw-r--r--   0 root         (0) root         (0)     3615 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/zh/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/en/
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2687 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/pl/
--rw-r--r--   0 root         (0) root         (0)     3553 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/pl/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/zh/
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/Reranking/en/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3010 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/Reranking/fr/
--rw-r--r--   0 root         (0) root         (0)     1189 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/fr/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/fr/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1206 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Reranking/zh/
--rw-r--r--   0 root         (0) root         (0)     3504 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/zh/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     2462 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Retrieval/da/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2577 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Retrieval/de/
--rw-r--r--   0 root         (0) root         (0)     1997 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2896 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/en/
--rw-r--r--   0 root         (0) root         (0)     1005 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      977 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3699 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1108 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/es/
--rw-r--r--   0 root         (0) root         (0)     2117 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/fr/
--rw-r--r--   0 root         (0) root         (0)     2182 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2469 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2164 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/ko/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMrtydi.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3248 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3250 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2921 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/nb/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2702 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/nb/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/pl/
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1157 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1079 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/sv/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2613 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/zh/
--rw-r--r--   0 root         (0) root         (0)    10336 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/de/
--rw-r--r--   0 root         (0) root         (0)     1364 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/en/
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/es/
--rw-r--r--   0 root         (0) root         (0)     1480 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/es/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/fr/
--rw-r--r--   0 root         (0) root         (0)     1466 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/fr/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/pl/
--rw-r--r--   0 root         (0) root         (0)     2256 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/pl/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/STS/zh/
--rw-r--r--   0 root         (0) root         (0)     7080 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/zh/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/Summarization/en/
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/en/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/Summarization/fr/
--rw-r--r--   0 root         (0) root         (0)     1298 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12579 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2120 2024-04-03 12:30:51.000000 mteb-1.5.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5217 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/mteb_meta.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 12:30:54.661619 mteb-1.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_all_abstasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.124882 mteb-1.5.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-04 12:49:25.000000 mteb-1.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-04 12:49:30.120882 mteb-1.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9190 2024-04-04 12:49:25.000000 mteb-1.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.068882 mteb-1.5.2/mteb/
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     6430 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13124 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/tasks/BitextMining/da/
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/BitextMining/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/Classification/da/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/en/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/nb/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/nb/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/nb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/pl/
+-rw-r--r--   0 root         (0) root         (0)     4892 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/pl/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/sv/
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/sv/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/sv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/zh/
+-rw-r--r--   0 root         (0) root         (0)     6535 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/zh/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.084882 mteb-1.5.2/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.084882 mteb-1.5.2/mteb/tasks/Clustering/de/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.084882 mteb-1.5.2/mteb/tasks/Clustering/en/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/es/
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/es/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/fr/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/nb/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/nb/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/pl/
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/pl/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/sv/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/zh/
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/zh/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/en/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/pl/
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/pl/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/zh/
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/Reranking/en/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/Reranking/fr/
+-rw-r--r--   0 root         (0) root         (0)     1189 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/fr/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/fr/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Reranking/zh/
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/zh/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Retrieval/da/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Retrieval/de/
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.100882 mteb-1.5.2/mteb/tasks/Retrieval/en/
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/es/
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/fr/
+-rw-r--r--   0 root         (0) root         (0)     2182 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/ko/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMrtydi.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/nb/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/nb/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/Retrieval/pl/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/Retrieval/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/sv/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/Retrieval/zh/
+-rw-r--r--   0 root         (0) root         (0)    10336 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/STS/de/
+-rw-r--r--   0 root         (0) root         (0)     1364 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/en/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/es/
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/es/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/fr/
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/fr/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/pl/
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/pl/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/zh/
+-rw-r--r--   0 root         (0) root         (0)     7080 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/zh/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/mteb/tasks/Summarization/en/
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/en/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/mteb/tasks/Summarization/fr/
+-rw-r--r--   0 root         (0) root         (0)     1298 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12579 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-04 12:49:26.000000 mteb-1.5.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/mteb_meta.py
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 12:49:30.124882 mteb-1.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_all_abstasks.py
```

### Comparing `mteb-1.5.1/LICENSE` & `mteb-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/PKG-INFO` & `mteb-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.1
+Version: 1.5.2
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.1/README.md` & `mteb-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/__init__.py` & `mteb-1.5.2/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTask.py` & `mteb-1.5.2/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.5.2/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/CrosslingualTask.py` & `mteb-1.5.2/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/LangMapping.py` & `mteb-1.5.2/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/MultilingualTask.py` & `mteb-1.5.2/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/abstasks/TaskMetadata.py` & `mteb-1.5.2/mteb/abstasks/TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/cmd.py` & `mteb-1.5.2/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/MTEB.py` & `mteb-1.5.2/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.5.2/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/evaluation/evaluators/utils.py` & `mteb-1.5.2/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/logging.py` & `mteb-1.5.2/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/da/BornholmskBitextMining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/da/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py` & `mteb-1.5.2/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nb", "nn"],
         main_score="accuracy",
         date=("2000-01-01", "2020-12-31"),  # approximate guess
         form=["spoken"],
-        domains=["Spoken"],
-        task_subtypes=["Political classification"],
+        domains=["Spoken", "Legal"],
+        task_subtypes=["Dialect pairing"],
         license="openUnder-PSI",
         socioeconomic_status="high",
         annotations_creators="derived",  # best guess
         dialect=[],
         text_creation="found",
         bibtex_citation=None,
         n_samples={"test": 456},
```

### Comparing `mteb-1.5.1/mteb/tasks/Classification/__init__.py` & `mteb-1.5.2/mteb/tasks/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/da/AngryTweetsClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/da/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/da/DKHateClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/da/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/da/DalajClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/da/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/da/DdiscoCohesionClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/da/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/da/LccSentimentClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/da/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/en/AmazonPolarityClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/en/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/en/Banking77Classification.py` & `mteb-1.5.2/mteb/tasks/Classification/en/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/en/EmotionClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/en/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/en/ImdbClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/en/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/en/ToxicConversationsClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/en/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/nb/NoRecClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/nb/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/pl/PolishClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/pl/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/sv/SweRecClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/sv/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Classification/zh/CMTEBClassification.py` & `mteb-1.5.2/mteb/tasks/Classification/zh/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/__init__.py` & `mteb-1.5.2/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/BigPatentClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/RedditClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/RedditClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/en/WikiCitiesClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/en/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/es/FloresClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/es/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/fr/HALClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/fr/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/nb/snl_clustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/nb/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/nb/vg_clustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/nb/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/pl/PolishClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/pl/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/sv/swedn_clustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/sv/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Clustering/zh/CMTEBClustering.py` & `mteb-1.5.2/mteb/tasks/Clustering/zh/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py` & `mteb-1.5.2/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py` & `mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py` & `mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.5.2/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.5.2/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/pl/PolishPC.py` & `mteb-1.5.2/mteb/tasks/PairClassification/pl/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py` & `mteb-1.5.2/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py` & `mteb-1.5.2/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/en/MindSmallReranking.py` & `mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMrtydi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskReranking import AbsTaskReranking
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MindSmallReranking(AbsTaskReranking):
+class KoMrtydi(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MindSmallReranking",
-        description="Microsoft News Dataset: A Large-Scale English Dataset for News Recommendation Research",
-        reference="https://msnews.github.io/assets/doc/ACL2020_MIND.pdf",
+        name="Ko-mrtydi",
+        description="Ko-mrtydi",
+        reference=None,
         dataset={
-            "path": "mteb/mind_small",
-            "revision": "3bdac13927fdc888b903db93b2ffdbd90b295a69",
+            "path": "taeminlee/Ko-mrtydi",
+            "revision": "71a2e011a42823051a2b4eb303a3366bdbe048d3",
         },
-        type="Reranking",
-        category="s2s",
-        eval_splits=["test"],
-        eval_langs=["en"],
-        main_score="map",
+        type="Retrieval",
+        category="s2p",
+        eval_splits=["dev"],
+        eval_langs=["ko"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 107968},
-        avg_character_length={"test": 70.9},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/en/SciDocsReranking.py` & `mteb-1.5.2/mteb/tasks/Reranking/en/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py` & `mteb-1.5.2/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/fr/AlloprofReranking.py` & `mteb-1.5.2/mteb/tasks/Reranking/fr/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/fr/SyntecReranking.py` & `mteb-1.5.2/mteb/tasks/Reranking/fr/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.5.2/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Reranking/zh/CMTEBReranking.py` & `mteb-1.5.2/mteb/tasks/Reranking/zh/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/__init__.py` & `mteb-1.5.2/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/da/dan_fever.py` & `mteb-1.5.2/mteb/tasks/Retrieval/da/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/da/t2nord_retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/da/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/da/twitterhjerne.py` & `mteb-1.5.2/mteb/tasks/Retrieval/da/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/DBPediaRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/FEVERRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/HagridRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/HotpotQARetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCORetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/NQRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/QuoraRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/SciFactRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/en/Touche2020Retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/en/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py` & `mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py` & `mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/fr/BSARDRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/fr/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/fr/SyntecRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/fr/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMiracl.py` & `mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMrtydi.py` & `mteb-1.5.2/mteb/tasks/Retrieval/ko/KoStrategyQA.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class KoMrtydi(AbsTaskRetrieval):
+class KoStrategyQA(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Ko-mrtydi",
-        description="Ko-mrtydi",
+        name="Ko-StrategyQA",
+        description="Ko-StrategyQA",
         reference=None,
         dataset={
-            "path": "taeminlee/Ko-mrtydi",
-            "revision": "71a2e011a42823051a2b4eb303a3366bdbe048d3",
+            "path": "taeminlee/Ko-StrategyQA",
+            "revision": "d243889a3eb6654029dbd7e7f9319ae31d58f97c",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["ko"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/ko/KoStrategyQA.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class KoStrategyQA(AbsTaskRetrieval):
+class MSMARCOPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Ko-StrategyQA",
-        description="Ko-StrategyQA",
-        reference=None,
+        name="MSMARCO-PL",
+        description="MS MARCO is a collection of datasets focused on deep learning in search",
+        reference="https://microsoft.github.io/msmarco/",
         dataset={
-            "path": "taeminlee/Ko-StrategyQA",
-            "revision": "d243889a3eb6654029dbd7e7f9319ae31d58f97c",
+            "path": "clarin-knext/msmarco-pl",
+            "revision": "8634c07806d5cce3a6138e260e59b81760a0a640",
         },
         type="Retrieval",
         category="s2p",
-        eval_splits=["dev"],
-        eval_langs=["ko"],
+        eval_splits=["test"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/nb/norquad.py` & `mteb-1.5.2/mteb/tasks/Retrieval/nb/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/nb/snl_retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/nb/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/NQPLRetrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MSMARCOPL(AbsTaskRetrieval):
+class NQPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MSMARCO-PL",
-        description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/",
+        name="NQ-PL",
+        description="Natural Questions: A Benchmark for Question Answering Research",
+        reference="https://ai.google.com/research/NaturalQuestions/",
         dataset={
-            "path": "clarin-knext/msmarco-pl",
-            "revision": "8634c07806d5cce3a6138e260e59b81760a0a640",
+            "path": "clarin-knext/nq-pl",
+            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/NQPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NQPL(AbsTaskRetrieval):
+class SciFactPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NQ-PL",
-        description="Natural Questions: A Benchmark for Question Answering Research",
-        reference="https://ai.google.com/research/NaturalQuestions/",
+        name="SciFact-PL",
+        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
+        reference="https://github.com/allenai/scifact",
         dataset={
-            "path": "clarin-knext/nq-pl",
-            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
+            "path": "clarin-knext/scifact-pl",
+            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,55 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks import AbsTaskSTS, CrosslingualTask
 
+_LANGUAGES = [
+    "ko-ko",
+    "ar-ar",
+    "en-ar",
+    "en-de",
+    "en-en",
+    "en-tr",
+    "es-en",
+    "es-es",
+    "fr-en",
+    "it-en",
+    "nl-en",
+]
 
-class SciFactPL(AbsTaskRetrieval):
+
+class STS17Crosslingual(AbsTaskSTS, CrosslingualTask):
     metadata = TaskMetadata(
-        name="SciFact-PL",
-        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
-        reference="https://github.com/allenai/scifact",
+        name="STS17",
         dataset={
-            "path": "clarin-knext/scifact-pl",
-            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
+            "path": "mteb/sts17-crosslingual-sts",
+            "revision": "af5e6fb845001ecf41f4c1e033ce921939a2a68d",
         },
-        type="Retrieval",
-        category="s2p",
+        description="STS 2017 dataset",
+        reference="http://alt.qcri.org/semeval2016/task1/",
+        type="STS",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
+        eval_langs=_LANGUAGES,
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 500},
+        avg_character_length={"test": 43.3},
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/sv/swedn_retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/sv/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/sv/swefaq_retrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/sv/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py` & `mteb-1.5.2/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/__init__.py` & `mteb-1.5.2/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py` & `mteb-1.5.2/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/BiossesSTS.py` & `mteb-1.5.2/mteb/tasks/STS/en/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/STS12STS.py` & `mteb-1.5.2/mteb/tasks/STS/en/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/STS13STS.py` & `mteb-1.5.2/mteb/tasks/STS/en/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/STS14STS.py` & `mteb-1.5.2/mteb/tasks/STS/en/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/STS15STS.py` & `mteb-1.5.2/mteb/tasks/STS/en/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/STS16STS.py` & `mteb-1.5.2/mteb/tasks/STS/en/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/STSBenchmarkSTS.py` & `mteb-1.5.2/mteb/tasks/STS/en/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/en/SickrSTS.py` & `mteb-1.5.2/mteb/tasks/STS/en/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/es/STSES.py` & `mteb-1.5.2/mteb/tasks/STS/es/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/fr/SickFrSTS.py` & `mteb-1.5.2/mteb/tasks/STS/fr/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.5.2/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.5.2/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/pl/PolishSTS.py` & `mteb-1.5.2/mteb/tasks/STS/pl/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/STS/zh/CMTEBSTS.py` & `mteb-1.5.2/mteb/tasks/STS/zh/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Summarization/en/SummEvalSummarization.py` & `mteb-1.5.2/mteb/tasks/Summarization/en/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py` & `mteb-1.5.2/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/mteb.egg-info/PKG-INFO` & `mteb-1.5.2/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.1
+Version: 1.5.2
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.1/mteb.egg-info/SOURCES.txt` & `mteb-1.5.2/mteb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/pyproject.toml` & `mteb-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.5.1"
+version = "1.5.2"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.5.1/scripts/data/amazon_polarity/create_data.py` & `mteb-1.5.2/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.5.2/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/arxiv/script_clustering.py` & `mteb-1.5.2/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/arxiv/script_raw.py` & `mteb-1.5.2/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/biorxiv/script_clustering.py` & `mteb-1.5.2/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/biorxiv/script_raw.py` & `mteb-1.5.2/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/bucc/create_data.py` & `mteb-1.5.2/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/create_task_table.py` & `mteb-1.5.2/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/germanquad/process_data.py` & `mteb-1.5.2/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/hal/create_data.py` & `mteb-1.5.2/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/imdb/create_data.py` & `mteb-1.5.2/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/medrxiv/script_clustering.py` & `mteb-1.5.2/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/medrxiv/script_raw.py` & `mteb-1.5.2/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/mind/prepare_data.py` & `mteb-1.5.2/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/redditp2p/script_clustering.py` & `mteb-1.5.2/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.5.2/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.5.2/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/summeval_fr/create_data.py` & `mteb-1.5.2/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.5.2/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/merge_cqadupstack.py` & `mteb-1.5.2/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/mteb_meta.py` & `mteb-1.5.2/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/run_mteb_chinese.py` & `mteb-1.5.2/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/run_mteb_english.py` & `mteb-1.5.2/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/run_mteb_french.py` & `mteb-1.5.2/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/run_mteb_german.py` & `mteb-1.5.2/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/run_mteb_korean.py` & `mteb-1.5.2/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/scripts/run_mteb_polish.py` & `mteb-1.5.2/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/tests/test_ClusteringEvaluator.py` & `mteb-1.5.2/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/tests/test_PairClassificationEvaluator.py` & `mteb-1.5.2/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/tests/test_RerankingEvaluator.py` & `mteb-1.5.2/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/tests/test_RetrievalEvaluator.py` & `mteb-1.5.2/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/tests/test_TaskMetadata.py` & `mteb-1.5.2/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.1/tests/test_all_abstasks.py` & `mteb-1.5.2/tests/test_all_abstasks.py`

 * *Files identical despite different names*

