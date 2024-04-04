# Comparing `tmp/metabeaver-0.3.7.tar.gz` & `tmp/metabeaver-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.3.7.tar", last modified: Thu Apr  4 10:57:59 2024, max compression
+gzip compressed data, was "metabeaver-0.3.8.tar", last modified: Thu Apr  4 19:15:09 2024, max compression
```

## Comparing `metabeaver-0.3.7.tar` & `metabeaver-0.3.8.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.100226 metabeaver-0.3.7/
--rw-rw-rw-   0        0        0      682 2024-04-04 10:57:59.097224 metabeaver-0.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.121827 metabeaver-0.3.7/metabeaver/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.218047 metabeaver-0.3.7/metabeaver/BeaverTown/
--rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.7/metabeaver/BeaverTown/__init__.py
--rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.7/metabeaver/BeaverTown/abstractBeaver.py
--rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.7/metabeaver/BeaverTown/beaverOn.py
--rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.7/metabeaver/BeaverTown/pumpkinPie.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.232597 metabeaver-0.3.7/metabeaver/Binary/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Binary/__init__.py
--rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.7/metabeaver/Binary/binaryOperations.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.257907 metabeaver-0.3.7/metabeaver/Caching/
--rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.7/metabeaver/Caching/LeastRecentlyUsed.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Caching/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.298876 metabeaver-0.3.7/metabeaver/DataManipulation/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/DataManipulation/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.3.7/metabeaver/DataManipulation/filterPandas.py
--rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.7/metabeaver/DataManipulation/localPickle.py
--rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.7/metabeaver/DataManipulation/universalResourceLinkHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.343834 metabeaver-0.3.7/metabeaver/DataStructures/
--rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.7/metabeaver/DataStructures/BinarySearchTree.py
--rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.7/metabeaver/DataStructures/Node.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.7/metabeaver/DataStructures/firstInFirstOutQueue.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.7/metabeaver/DataStructures/firstInLastOut.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.7/metabeaver/DataStructures/linkedList.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.346361 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.369324 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/__init__.py
--rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.437598 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/
--rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
--rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.455783 metabeaver-0.3.7/metabeaver/DatesAndTime/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/DatesAndTime/__init__.py
--rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.7/metabeaver/DatesAndTime/getToday.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.458330 metabeaver-0.3.7/metabeaver/Dynamic Programming/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Dynamic Programming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.496393 metabeaver-0.3.7/metabeaver/FileIO/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/FileIO/__init__.py
--rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.3.7/metabeaver/FileIO/pickleObject.py
--rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.7/metabeaver/FileIO/yamlIO.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.541106 metabeaver-0.3.7/metabeaver/Formatting/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/Formatting/__init__.py
--rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.7/metabeaver/Formatting/printControl.py
--rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.7/metabeaver/Formatting/printControlTest.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.543111 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.592120 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     6125 2024-04-04 10:48:03.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0     1898 2024-04-04 10:30:27.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
--rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
--rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.619725 metabeaver-0.3.7/metabeaver/Graph Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/bellmanFord.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/breadthFirstSearch.py
--rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/depthFirstSearch.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/dijkstra.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.638317 metabeaver-0.3.7/metabeaver/Graphing/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/Graphing/__init__.py
--rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.7/metabeaver/Graphing/markdownGenerator.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.666284 metabeaver-0.3.7/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.7/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.668613 metabeaver-0.3.7/metabeaver/InterviewQuestions/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.731537 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
--rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
--rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/twoSum.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.757217 metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.760745 metabeaver-0.3.7/metabeaver/LearnPython/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.781885 metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/__init__.py
--rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/ifelifelse.py
--rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.7/metabeaver/LearnPython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.810387 metabeaver-0.3.7/metabeaver/Machine Learning/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.846053 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/__init__.py
--rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
--rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/loadWithTransformers.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Machine Learning/__init__.py
--rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.7/metabeaver/Machine Learning/lassoRegression.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.869110 metabeaver-0.3.7/metabeaver/Mathematical Operations/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Mathematical Operations/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.7/metabeaver/Mathematical Operations/greatestCommonDenominator.py
--rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.7/metabeaver/Mathematical Operations/vectorDotProduct.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.872123 metabeaver-0.3.7/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.873115 metabeaver-0.3.7/metabeaver/OperationBeaver/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/OperationBeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.884265 metabeaver-0.3.7/metabeaver/Search Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Search Algorithms/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.7/metabeaver/Search Algorithms/binarySearch.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.910902 metabeaver-0.3.7/metabeaver/Set Theory/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Set Theory/__init__.py
--rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.7/metabeaver/Set Theory/findAllSubsets.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.008602 metabeaver-0.3.7/metabeaver/Sorting Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/heapSort.py
--rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/insertionSort.py
--rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/mergeSort.py
--rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/quickSort.py
--rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/timsort.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.028691 metabeaver-0.3.7/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.7/metabeaver/Testing/scratchPad.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.059875 metabeaver-0.3.7/metabeaver/TextValidation/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/TextValidation/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.7/metabeaver/TextValidation/closureChecker.py
--rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.7/metabeaver/TextValidation/establishLargestPalindrome.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.091715 metabeaver-0.3.7/metabeaver/WebScraping/
--rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.7/metabeaver/WebScraping/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.7/metabeaver/WebScraping/simpleRequests.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.094706 metabeaver-0.3.7/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      682 2024-04-04 10:57:57.000000 metabeaver-0.3.7/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4078 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 10:57:59.101541 metabeaver-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1299 2024-04-04 10:48:03.000000 metabeaver-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.860001 metabeaver-0.3.8/
+-rw-rw-rw-   0        0        0      682 2024-04-04 19:15:09.860001 metabeaver-0.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:08.986854 metabeaver-0.3.8/metabeaver/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.087717 metabeaver-0.3.8/metabeaver/BeaverTown/
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.8/metabeaver/BeaverTown/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.8/metabeaver/BeaverTown/abstractBeaver.py
+-rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.8/metabeaver/BeaverTown/beaverOn.py
+-rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.8/metabeaver/BeaverTown/pumpkinPie.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.103437 metabeaver-0.3.8/metabeaver/Binary/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Binary/__init__.py
+-rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.8/metabeaver/Binary/binaryOperations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.119077 metabeaver-0.3.8/metabeaver/Caching/
+-rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.8/metabeaver/Caching/LeastRecentlyUsed.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Caching/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.166438 metabeaver-0.3.8/metabeaver/DataManipulation/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.8/metabeaver/DataManipulation/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.3.8/metabeaver/DataManipulation/filterPandas.py
+-rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.8/metabeaver/DataManipulation/localPickle.py
+-rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.8/metabeaver/DataManipulation/universalResourceLinkHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.229367 metabeaver-0.3.8/metabeaver/DataStructures/
+-rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.8/metabeaver/DataStructures/BinarySearchTree.py
+-rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.8/metabeaver/DataStructures/Node.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.8/metabeaver/DataStructures/firstInFirstOutQueue.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.8/metabeaver/DataStructures/firstInLastOut.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.8/metabeaver/DataStructures/linkedList.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.229367 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.244972 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQL/
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQL/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.308249 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/
+-rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
+-rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.8/metabeaver/DatabaseFunctionality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.323903 metabeaver-0.3.8/metabeaver/DatesAndTime/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.8/metabeaver/DatesAndTime/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.8/metabeaver/DatesAndTime/getToday.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.323903 metabeaver-0.3.8/metabeaver/Dynamic Programming/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Dynamic Programming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.371265 metabeaver-0.3.8/metabeaver/FileIO/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/FileIO/__init__.py
+-rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.3.8/metabeaver/FileIO/pickleObject.py
+-rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.8/metabeaver/FileIO/yamlIO.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.396116 metabeaver-0.3.8/metabeaver/Formatting/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.8/metabeaver/Formatting/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.8/metabeaver/Formatting/printControl.py
+-rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.8/metabeaver/Formatting/printControlTest.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.402632 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.433911 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     7534 2024-04-04 19:02:59.000000 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0     3354 2024-04-04 19:05:00.000000 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
+-rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
+-rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.465574 metabeaver-0.3.8/metabeaver/Graph Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Graph Algorithms/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.8/metabeaver/Graph Algorithms/bellmanFord.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.8/metabeaver/Graph Algorithms/breadthFirstSearch.py
+-rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.8/metabeaver/Graph Algorithms/depthFirstSearch.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.8/metabeaver/Graph Algorithms/dijkstra.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.8/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.481200 metabeaver-0.3.8/metabeaver/Graphing/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.8/metabeaver/Graphing/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.8/metabeaver/Graphing/markdownGenerator.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.497252 metabeaver-0.3.8/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.8/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.497252 metabeaver-0.3.8/metabeaver/InterviewQuestions/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.528549 metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
+-rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
+-rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/twoSum.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.544362 metabeaver-0.3.8/metabeaver/InterviewQuestions/Stacks/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/Stacks/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/InterviewQuestions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.544362 metabeaver-0.3.8/metabeaver/LearnPython/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.560000 metabeaver-0.3.8/metabeaver/LearnPython/ControlFlow/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/LearnPython/ControlFlow/__init__.py
+-rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.8/metabeaver/LearnPython/ControlFlow/ifelifelse.py
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.8/metabeaver/LearnPython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.596471 metabeaver-0.3.8/metabeaver/Machine Learning/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.607491 metabeaver-0.3.8/metabeaver/Machine Learning/LLM/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Machine Learning/LLM/__init__.py
+-rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.8/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
+-rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.8/metabeaver/Machine Learning/LLM/loadWithTransformers.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Machine Learning/__init__.py
+-rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.8/metabeaver/Machine Learning/lassoRegression.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.623596 metabeaver-0.3.8/metabeaver/Mathematical Operations/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Mathematical Operations/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.8/metabeaver/Mathematical Operations/greatestCommonDenominator.py
+-rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.8/metabeaver/Mathematical Operations/vectorDotProduct.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.623596 metabeaver-0.3.8/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.639235 metabeaver-0.3.8/metabeaver/OperationBeaver/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/OperationBeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.639235 metabeaver-0.3.8/metabeaver/Search Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Search Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.8/metabeaver/Search Algorithms/binarySearch.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.670874 metabeaver-0.3.8/metabeaver/Set Theory/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Set Theory/__init__.py
+-rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.8/metabeaver/Set Theory/findAllSubsets.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.751431 metabeaver-0.3.8/metabeaver/Sorting Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/Sorting Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.8/metabeaver/Sorting Algorithms/heapSort.py
+-rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.8/metabeaver/Sorting Algorithms/insertionSort.py
+-rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.8/metabeaver/Sorting Algorithms/mergeSort.py
+-rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.8/metabeaver/Sorting Algorithms/quickSort.py
+-rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.8/metabeaver/Sorting Algorithms/timsort.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.765943 metabeaver-0.3.8/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.8/metabeaver/Testing/scratchPad.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.828405 metabeaver-0.3.8/metabeaver/TextValidation/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.8/metabeaver/TextValidation/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.8/metabeaver/TextValidation/closureChecker.py
+-rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.8/metabeaver/TextValidation/establishLargestPalindrome.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.844331 metabeaver-0.3.8/metabeaver/WebScraping/
+-rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.8/metabeaver/WebScraping/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.8/metabeaver/WebScraping/simpleRequests.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.8/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:15:09.860001 metabeaver-0.3.8/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      682 2024-04-04 19:15:08.000000 metabeaver-0.3.8/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4078 2024-04-04 19:15:08.000000 metabeaver-0.3.8/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:15:08.000000 metabeaver-0.3.8/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-04 19:15:08.000000 metabeaver-0.3.8/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 19:15:08.000000 metabeaver-0.3.8/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:15:09.860001 metabeaver-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-04-04 19:14:49.000000 metabeaver-0.3.8/setup.py
```

### Comparing `metabeaver-0.3.7/PKG-INFO` & `metabeaver-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.3.7
+Version: 0.3.8
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: numpy
```

### Comparing `metabeaver-0.3.7/metabeaver/BeaverTown/abstractBeaver.py` & `metabeaver-0.3.8/metabeaver/BeaverTown/abstractBeaver.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/BeaverTown/beaverOn.py` & `metabeaver-0.3.8/metabeaver/BeaverTown/beaverOn.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Binary/binaryOperations.py` & `metabeaver-0.3.8/metabeaver/Binary/binaryOperations.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Caching/LeastRecentlyUsed.py` & `metabeaver-0.3.8/metabeaver/Caching/LeastRecentlyUsed.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DataManipulation/filterPandas.py` & `metabeaver-0.3.8/metabeaver/DataManipulation/filterPandas.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DataManipulation/localPickle.py` & `metabeaver-0.3.8/metabeaver/DataManipulation/localPickle.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DataManipulation/universalResourceLinkHandler.py` & `metabeaver-0.3.8/metabeaver/DataManipulation/universalResourceLinkHandler.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DataStructures/BinarySearchTree.py` & `metabeaver-0.3.8/metabeaver/DataStructures/BinarySearchTree.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/rawSQL.py` & `metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQL/rawSQL.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py` & `metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py` & `metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py` & `metabeaver-0.3.8/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/DatesAndTime/getToday.py` & `metabeaver-0.3.8/metabeaver/DatesAndTime/getToday.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/FileIO/yamlIO.py` & `metabeaver-0.3.8/metabeaver/FileIO/yamlIO.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Formatting/printControlTest.py` & `metabeaver-0.3.8/metabeaver/Formatting/printControlTest.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py` & `metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # Rename the get crawled pages as it can be much more generic
 
 import datetime as dt
 import pandas as pd
 import numpy as np
+import yaml
 from typing import List
 from google.cloud import bigquery
+from google.oauth2 import service_account
 
 
-# Given valid credentials, details for the table location, and a schema, this function will create a table in BigQuery.
-def create_bigquery_table(credentials, project_id, tableset, table_name, schema):
+# Given valid client, details for the table location, and a schema, this function will create a table in BigQuery.
+def create_bigquery_table(client, tableset, table_name, schema):
     """Creates a BigQuery table in the specified tableset with the given table name and schema.
 
     Args:
-        credentials (google.auth.credentials.Credentials): The credentials to use to authenticate with BigQuery.
-        project_id (str): The project ID for the BigQuery table.
-        tableset (str): The tableset to create the table in.
+        client (google.cloud.bigquery.client.Client): The BigQuery client to use for creating the table.
+        tableset (str): The dataset ID where the table will be created.
         table_name (str): The name for the new BigQuery table.
         schema (list[google.cloud.bigquery.SchemaField]): The schema for the new BigQuery table.
 
     Returns:
         google.cloud.bigquery.table.Table: The newly created BigQuery table.
     """
-    # Create the BigQuery client
-    client = bigquery.Client(project=project_id, credentials=credentials)
-
-    # Get a reference to the table
-    table_ref = client.dataset(tableset).table(table_name)
-
-    # Create the table object
-    table = bigquery.Table(table_ref, schema=schema)
-
-    # Create the table in BigQuery
-    table = client.create_table(table)
-
-    # Return the new table object
-    return table
+    try:
+        # Get a reference to the table
+        table_ref = client.dataset(tableset).table(table_name)
+
+        # Create the table object
+        table = bigquery.Table(table_ref, schema=schema)
+
+        # Create the table in BigQuery
+        table = client.create_table(table)
+
+        # Return the new table object
+        return table
+    except Exception as e:
+        print(f"Error creating table '{table_name}' in dataset '{tableset}': {e}")
 
 
 # Maps Python primitive types and numpy/panda types to BigQuery equivalents
 def create_schema(items: List, field_names: List[str]) -> List[bigquery.SchemaField]:
     """
     Creates a BigQuery schema based on a list of items.
 
@@ -57,14 +58,16 @@
         bytearray: 'BYTES',
         memoryview: 'BYTES',
         'Int64': 'INTEGER',
         'Float64': 'FLOAT',
         pd.Timestamp: 'TIMESTAMP',
         pd.DateOffset: 'DATE',
         pd.Timedelta: 'TIME',
+        pd.Interval: 'STRING',  # Can't directly map to BigQuery type, so using STRING as a placeholder
+        pd.CategoricalDtype: 'STRING',  # Can't directly map to BigQuery type, so using STRING as a placeholder
         np.float16: 'FLOAT',
         np.float32: 'FLOAT',
         np.float64: 'FLOAT',
         np.int8: 'INTEGER',
         np.int16: 'INTEGER',
         np.int32: 'INTEGER',
         np.int64: 'INTEGER',
@@ -107,14 +110,42 @@
     # Generate BigQuery schema from DataFrame columns
     schema = create_schema(dataframe.values[0], dataframe.columns.tolist())
 
     # Create BigQuery table
     create_bigquery_table(client, client.project, dataset_id, table_name, schema)
 
 
+def create_bq_table_from_df_with_credentials(credentials: google.auth.credentials.Credentials,
+                                         dataset_id: str,
+                                         table_name: str,
+                                         dataframe: pd.DataFrame):
+    """
+    Create a BigQuery table from a Pandas DataFrame.
+
+    :param credentials: Google Cloud credentials object.
+    :param dataset_id: ID of the dataset where the table will be created.
+    :param table_name: Name of the table to be created.
+    :param dataframe: Pandas DataFrame containing the data.
+    """
+    #
+    try:
+        # Create BigQuery client with provided credentials
+        client = bigquery.Client(credentials=credentials)
+
+        # Generate BigQuery schema from DataFrame columns
+        schema = create_schema(dataframe.iloc[0], dataframe.columns.tolist())
+
+        # Create BigQuery table
+        create_bigquery_table(client, client.project, dataset_id, table_name, schema)
+        print(f"Table '{table_name}' created successfully in dataset '{dataset_id}'.")
+    #
+    except Exception as e:
+        print(f"Error creating table: {e}")
+
+
 # Gets the most up to date data for a table where the target column has an entries within the last n_days
 def get_valid_pages(client, dataset_name, table_name, target_column, date_column, n_days=30, end_date=None):
 
         # Get current time in UTC
         now_utc = dt.datetime.utcnow()
 
         # Calculate start time based on specified number of days
```

### Comparing `metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py` & `metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,34 @@
 
 import yaml
 
 from typing import List
 import pandas as pd
 
 
+# Return a credentials via supplying a service_account.Credentials with valid credential.json loc GCP API calls
+def get_credentials_from_yaml(yaml_file_path):
+
+    # Attempt to load a service_account.Credentials from a YAML file reference to stored location."""
+    try:
+        # Try to load the YAML file
+        with open(yaml_file_path, 'r') as yaml_file:
+            config = yaml.safe_load(yaml_file)
+
+        # Extract path to service account JSON file from YAML config
+        credentials_path = config['credentials']['service_account_json_path']
+
+        # Load service account credentials from JSON file and return the credentials to be used in API calls.
+        credentials = service_account.Credentials.from_service_account_file(credentials_path)
+        return credentials
+    # Print any Exception associated with retrieval.
+    except Exception as e:
+        print(f"Error: {e}")
+
+
 # Create a bigquery client from a credentials.json
 def get_bigquery_client_from_json(credentials_path='path/to/your/credentials.json'):
     # Example usage with explicit credentials file path
     # bigquery_client = get_bigquery_client(r'C:\Users\lukep\OneDrive\workandplay\credentials.json')
 
     # Explicitly provide the path to your service account key file
     credentials = service_account.Credentials.from_service_account_file(credentials_path)
@@ -47,8 +67,23 @@
     # Create a BigQuery client using the loaded credentials
     client = bigquery.Client.from_service_account_info(
         credentials_info,
         project=gcp_project
     )
 
     # Returns a client we can use to interact with BigQuery.
-    return client
+    return client
+
+
+def create_bigquery_client(credentials_path):
+    """Create a BigQuery client using service account credentials."""
+    try:
+        # Load service account credentials from JSON file
+        credentials = service_account.Credentials.from_service_account_file(credentials_path)
+
+        # Create BigQuery client with the loaded credentials
+        client = bigquery.Client(credentials=credentials)
+
+        return client
+    except Exception as e:
+        print(f"Error creating BigQuery client: {e}")
+        return None
```

### Comparing `metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py` & `metabeaver-0.3.8/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Graph Algorithms/depthFirstSearch.py` & `metabeaver-0.3.8/metabeaver/Graph Algorithms/depthFirstSearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Graphing/markdownGenerator.py` & `metabeaver-0.3.8/metabeaver/Graphing/markdownGenerator.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.3.8/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py` & `metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py` & `metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/twoSum.py` & `metabeaver-0.3.8/metabeaver/InterviewQuestions/Arrays/twoSum.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py` & `metabeaver-0.3.8/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/ifelifelse.py` & `metabeaver-0.3.8/metabeaver/LearnPython/ControlFlow/ifelifelse.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Machine Learning/LLM/loadWithTransformers.py` & `metabeaver-0.3.8/metabeaver/Machine Learning/LLM/loadWithTransformers.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Machine Learning/lassoRegression.py` & `metabeaver-0.3.8/metabeaver/Machine Learning/lassoRegression.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Mathematical Operations/vectorDotProduct.py` & `metabeaver-0.3.8/metabeaver/Mathematical Operations/vectorDotProduct.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Search Algorithms/binarySearch.py` & `metabeaver-0.3.8/metabeaver/Search Algorithms/binarySearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Set Theory/findAllSubsets.py` & `metabeaver-0.3.8/metabeaver/Set Theory/findAllSubsets.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Sorting Algorithms/heapSort.py` & `metabeaver-0.3.8/metabeaver/Sorting Algorithms/heapSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Sorting Algorithms/insertionSort.py` & `metabeaver-0.3.8/metabeaver/Sorting Algorithms/insertionSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Sorting Algorithms/mergeSort.py` & `metabeaver-0.3.8/metabeaver/Sorting Algorithms/mergeSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Sorting Algorithms/quickSort.py` & `metabeaver-0.3.8/metabeaver/Sorting Algorithms/quickSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Sorting Algorithms/timsort.py` & `metabeaver-0.3.8/metabeaver/Sorting Algorithms/timsort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/Testing/scratchPad.py` & `metabeaver-0.3.8/metabeaver/Testing/scratchPad.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/TextValidation/closureChecker.py` & `metabeaver-0.3.8/metabeaver/TextValidation/closureChecker.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/TextValidation/establishLargestPalindrome.py` & `metabeaver-0.3.8/metabeaver/TextValidation/establishLargestPalindrome.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver/WebScraping/simpleRequests.py` & `metabeaver-0.3.8/metabeaver/WebScraping/simpleRequests.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/metabeaver.egg-info/PKG-INFO` & `metabeaver-0.3.8/metabeaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.3.7
+Version: 0.3.8
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: numpy
```

### Comparing `metabeaver-0.3.7/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.3.8/metabeaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.7/setup.py` & `metabeaver-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.3.7', # Major, minor, patch
+    version='0.3.8', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-core',
         'numpy',
         'pandas',
         #transformers,
```

