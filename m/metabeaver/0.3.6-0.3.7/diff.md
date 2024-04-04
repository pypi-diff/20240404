# Comparing `tmp/metabeaver-0.3.6.tar.gz` & `tmp/metabeaver-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.3.6.tar", last modified: Wed Apr  3 08:46:40 2024, max compression
+gzip compressed data, was "metabeaver-0.3.7.tar", last modified: Thu Apr  4 10:57:59 2024, max compression
```

## Comparing `metabeaver-0.3.6.tar` & `metabeaver-0.3.7.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.641451 metabeaver-0.3.6/
--rw-rw-rw-   0        0        0      682 2024-04-03 08:46:40.639451 metabeaver-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.430852 metabeaver-0.3.6/metabeaver/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.469942 metabeaver-0.3.6/metabeaver/BeaverTown/
--rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.6/metabeaver/BeaverTown/__init__.py
--rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.6/metabeaver/BeaverTown/abstractBeaver.py
--rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.6/metabeaver/BeaverTown/beaverOn.py
--rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.6/metabeaver/BeaverTown/pumpkinPie.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.473987 metabeaver-0.3.6/metabeaver/Binary/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Binary/__init__.py
--rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.6/metabeaver/Binary/binaryOperations.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.477003 metabeaver-0.3.6/metabeaver/Caching/
--rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.6/metabeaver/Caching/LeastRecentlyUsed.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Caching/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.484566 metabeaver-0.3.6/metabeaver/DataManipulation/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.6/metabeaver/DataManipulation/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.3.6/metabeaver/DataManipulation/filterPandas.py
--rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.6/metabeaver/DataManipulation/localPickle.py
--rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.6/metabeaver/DataManipulation/universalResourceLinkHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.499105 metabeaver-0.3.6/metabeaver/DataStructures/
--rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.6/metabeaver/DataStructures/BinarySearchTree.py
--rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.6/metabeaver/DataStructures/Node.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.6/metabeaver/DataStructures/firstInFirstOutQueue.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.6/metabeaver/DataStructures/firstInLastOut.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.6/metabeaver/DataStructures/linkedList.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.500142 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.505461 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQL/
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQL/__init__.py
--rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.514999 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/
--rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
--rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.6/metabeaver/DatabaseFunctionality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.517993 metabeaver-0.3.6/metabeaver/DatesAndTime/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.6/metabeaver/DatesAndTime/__init__.py
--rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.6/metabeaver/DatesAndTime/getToday.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.519997 metabeaver-0.3.6/metabeaver/Dynamic Programming/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Dynamic Programming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.522534 metabeaver-0.3.6/metabeaver/FileIO/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/FileIO/__init__.py
--rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.6/metabeaver/FileIO/yamlIO.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.527543 metabeaver-0.3.6/metabeaver/Formatting/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.6/metabeaver/Formatting/__init__.py
--rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.6/metabeaver/Formatting/printControl.py
--rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.6/metabeaver/Formatting/printControlTest.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.530547 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.539092 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     5076 2024-01-05 18:52:24.000000 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0      718 2024-01-05 19:16:53.000000 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
--rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
--rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.551623 metabeaver-0.3.6/metabeaver/Graph Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Graph Algorithms/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.6/metabeaver/Graph Algorithms/bellmanFord.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.6/metabeaver/Graph Algorithms/breadthFirstSearch.py
--rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.6/metabeaver/Graph Algorithms/depthFirstSearch.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.6/metabeaver/Graph Algorithms/dijkstra.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.6/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.554137 metabeaver-0.3.6/metabeaver/Graphing/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.6/metabeaver/Graphing/__init__.py
--rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.6/metabeaver/Graphing/markdownGenerator.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.558146 metabeaver-0.3.6/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.6/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.559141 metabeaver-0.3.6/metabeaver/InterviewQuestions/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.567815 metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
--rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
--rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/twoSum.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.570829 metabeaver-0.3.6/metabeaver/InterviewQuestions/Stacks/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/Stacks/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/InterviewQuestions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.572339 metabeaver-0.3.6/metabeaver/LearnPython/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.576903 metabeaver-0.3.6/metabeaver/LearnPython/ControlFlow/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/LearnPython/ControlFlow/__init__.py
--rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.6/metabeaver/LearnPython/ControlFlow/ifelifelse.py
--rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.6/metabeaver/LearnPython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.582471 metabeaver-0.3.6/metabeaver/Machine Learning/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.587473 metabeaver-0.3.6/metabeaver/Machine Learning/LLM/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Machine Learning/LLM/__init__.py
--rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.6/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
--rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.6/metabeaver/Machine Learning/LLM/loadWithTransformers.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Machine Learning/__init__.py
--rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.6/metabeaver/Machine Learning/lassoRegression.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.592975 metabeaver-0.3.6/metabeaver/Mathematical Operations/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Mathematical Operations/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.6/metabeaver/Mathematical Operations/greatestCommonDenominator.py
--rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.6/metabeaver/Mathematical Operations/vectorDotProduct.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.595982 metabeaver-0.3.6/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.598324 metabeaver-0.3.6/metabeaver/OperationBeaver/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/OperationBeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.601734 metabeaver-0.3.6/metabeaver/Search Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Search Algorithms/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.6/metabeaver/Search Algorithms/binarySearch.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.606193 metabeaver-0.3.6/metabeaver/Set Theory/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Set Theory/__init__.py
--rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.6/metabeaver/Set Theory/findAllSubsets.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.618207 metabeaver-0.3.6/metabeaver/Sorting Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/Sorting Algorithms/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.6/metabeaver/Sorting Algorithms/heapSort.py
--rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.6/metabeaver/Sorting Algorithms/insertionSort.py
--rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.6/metabeaver/Sorting Algorithms/mergeSort.py
--rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.6/metabeaver/Sorting Algorithms/quickSort.py
--rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.6/metabeaver/Sorting Algorithms/timsort.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.622449 metabeaver-0.3.6/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.6/metabeaver/Testing/scratchPad.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.631420 metabeaver-0.3.6/metabeaver/TextValidation/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.6/metabeaver/TextValidation/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.6/metabeaver/TextValidation/closureChecker.py
--rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.6/metabeaver/TextValidation/establishLargestPalindrome.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.635452 metabeaver-0.3.6/metabeaver/WebScraping/
--rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.6/metabeaver/WebScraping/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.6/metabeaver/WebScraping/simpleRequests.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.6/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:46:40.637452 metabeaver-0.3.6/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      682 2024-04-03 08:46:40.000000 metabeaver-0.3.6/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4044 2024-04-03 08:46:40.000000 metabeaver-0.3.6/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:46:40.000000 metabeaver-0.3.6/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-03 08:46:40.000000 metabeaver-0.3.6/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 08:46:40.000000 metabeaver-0.3.6/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:46:40.641451 metabeaver-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1299 2024-04-03 08:45:05.000000 metabeaver-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.100226 metabeaver-0.3.7/
+-rw-rw-rw-   0        0        0      682 2024-04-04 10:57:59.097224 metabeaver-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.121827 metabeaver-0.3.7/metabeaver/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.218047 metabeaver-0.3.7/metabeaver/BeaverTown/
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.7/metabeaver/BeaverTown/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.7/metabeaver/BeaverTown/abstractBeaver.py
+-rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.7/metabeaver/BeaverTown/beaverOn.py
+-rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.7/metabeaver/BeaverTown/pumpkinPie.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.232597 metabeaver-0.3.7/metabeaver/Binary/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Binary/__init__.py
+-rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.7/metabeaver/Binary/binaryOperations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.257907 metabeaver-0.3.7/metabeaver/Caching/
+-rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.7/metabeaver/Caching/LeastRecentlyUsed.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Caching/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.298876 metabeaver-0.3.7/metabeaver/DataManipulation/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/DataManipulation/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.3.7/metabeaver/DataManipulation/filterPandas.py
+-rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.7/metabeaver/DataManipulation/localPickle.py
+-rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.7/metabeaver/DataManipulation/universalResourceLinkHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.343834 metabeaver-0.3.7/metabeaver/DataStructures/
+-rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.7/metabeaver/DataStructures/BinarySearchTree.py
+-rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.7/metabeaver/DataStructures/Node.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.7/metabeaver/DataStructures/firstInFirstOutQueue.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.7/metabeaver/DataStructures/firstInLastOut.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.7/metabeaver/DataStructures/linkedList.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.346361 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.369324 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.437598 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/
+-rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
+-rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.7/metabeaver/DatabaseFunctionality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.455783 metabeaver-0.3.7/metabeaver/DatesAndTime/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/DatesAndTime/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.7/metabeaver/DatesAndTime/getToday.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.458330 metabeaver-0.3.7/metabeaver/Dynamic Programming/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Dynamic Programming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.496393 metabeaver-0.3.7/metabeaver/FileIO/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/FileIO/__init__.py
+-rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.3.7/metabeaver/FileIO/pickleObject.py
+-rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.7/metabeaver/FileIO/yamlIO.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.541106 metabeaver-0.3.7/metabeaver/Formatting/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/Formatting/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.7/metabeaver/Formatting/printControl.py
+-rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.7/metabeaver/Formatting/printControlTest.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.543111 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.592120 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     6125 2024-04-04 10:48:03.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0     1898 2024-04-04 10:30:27.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
+-rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
+-rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.619725 metabeaver-0.3.7/metabeaver/Graph Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/bellmanFord.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/breadthFirstSearch.py
+-rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/depthFirstSearch.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/dijkstra.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.7/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.638317 metabeaver-0.3.7/metabeaver/Graphing/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.7/metabeaver/Graphing/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.7/metabeaver/Graphing/markdownGenerator.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.666284 metabeaver-0.3.7/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.7/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.668613 metabeaver-0.3.7/metabeaver/InterviewQuestions/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.731537 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
+-rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
+-rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/twoSum.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.757217 metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/InterviewQuestions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.760745 metabeaver-0.3.7/metabeaver/LearnPython/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.781885 metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/__init__.py
+-rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/ifelifelse.py
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.7/metabeaver/LearnPython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.810387 metabeaver-0.3.7/metabeaver/Machine Learning/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.846053 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/__init__.py
+-rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
+-rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.7/metabeaver/Machine Learning/LLM/loadWithTransformers.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Machine Learning/__init__.py
+-rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.7/metabeaver/Machine Learning/lassoRegression.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.869110 metabeaver-0.3.7/metabeaver/Mathematical Operations/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Mathematical Operations/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.7/metabeaver/Mathematical Operations/greatestCommonDenominator.py
+-rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.7/metabeaver/Mathematical Operations/vectorDotProduct.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.872123 metabeaver-0.3.7/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.873115 metabeaver-0.3.7/metabeaver/OperationBeaver/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/OperationBeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.884265 metabeaver-0.3.7/metabeaver/Search Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Search Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.7/metabeaver/Search Algorithms/binarySearch.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:58.910902 metabeaver-0.3.7/metabeaver/Set Theory/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Set Theory/__init__.py
+-rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.7/metabeaver/Set Theory/findAllSubsets.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.008602 metabeaver-0.3.7/metabeaver/Sorting Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/heapSort.py
+-rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/insertionSort.py
+-rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/mergeSort.py
+-rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/quickSort.py
+-rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.7/metabeaver/Sorting Algorithms/timsort.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.028691 metabeaver-0.3.7/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.7/metabeaver/Testing/scratchPad.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.059875 metabeaver-0.3.7/metabeaver/TextValidation/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.7/metabeaver/TextValidation/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.7/metabeaver/TextValidation/closureChecker.py
+-rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.7/metabeaver/TextValidation/establishLargestPalindrome.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.091715 metabeaver-0.3.7/metabeaver/WebScraping/
+-rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.7/metabeaver/WebScraping/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.7/metabeaver/WebScraping/simpleRequests.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.7/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:57:59.094706 metabeaver-0.3.7/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      682 2024-04-04 10:57:57.000000 metabeaver-0.3.7/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4078 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 10:57:58.000000 metabeaver-0.3.7/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:57:59.101541 metabeaver-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-04-04 10:48:03.000000 metabeaver-0.3.7/setup.py
```

### Comparing `metabeaver-0.3.6/PKG-INFO` & `metabeaver-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.3.6
+Version: 0.3.7
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: numpy
```

### Comparing `metabeaver-0.3.6/metabeaver/BeaverTown/abstractBeaver.py` & `metabeaver-0.3.7/metabeaver/BeaverTown/abstractBeaver.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/BeaverTown/beaverOn.py` & `metabeaver-0.3.7/metabeaver/BeaverTown/beaverOn.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Binary/binaryOperations.py` & `metabeaver-0.3.7/metabeaver/Binary/binaryOperations.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Caching/LeastRecentlyUsed.py` & `metabeaver-0.3.7/metabeaver/Caching/LeastRecentlyUsed.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DataManipulation/filterPandas.py` & `metabeaver-0.3.7/metabeaver/DataManipulation/filterPandas.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DataManipulation/localPickle.py` & `metabeaver-0.3.7/metabeaver/DataManipulation/localPickle.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DataManipulation/universalResourceLinkHandler.py` & `metabeaver-0.3.7/metabeaver/DataManipulation/universalResourceLinkHandler.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DataStructures/BinarySearchTree.py` & `metabeaver-0.3.7/metabeaver/DataStructures/BinarySearchTree.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQL/rawSQL.py` & `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQL/rawSQL.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py` & `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py` & `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py` & `metabeaver-0.3.7/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/DatesAndTime/getToday.py` & `metabeaver-0.3.7/metabeaver/DatesAndTime/getToday.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/FileIO/yamlIO.py` & `metabeaver-0.3.7/metabeaver/FileIO/yamlIO.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Formatting/printControlTest.py` & `metabeaver-0.3.7/metabeaver/Formatting/printControlTest.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py` & `metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Rename the get crawled pages as it can be much more generic
 
 import datetime as dt
 import pandas as pd
 import numpy as np
-
-
 from typing import List
 from google.cloud import bigquery
 
 
+# Given valid credentials, details for the table location, and a schema, this function will create a table in BigQuery.
 def create_bigquery_table(credentials, project_id, tableset, table_name, schema):
     """Creates a BigQuery table in the specified tableset with the given table name and schema.
 
     Args:
         credentials (google.auth.credentials.Credentials): The credentials to use to authenticate with BigQuery.
         project_id (str): The project ID for the BigQuery table.
         tableset (str): The tableset to create the table in.
@@ -88,14 +87,34 @@
         field_name = field_names[idx] if idx < len(field_names) else f'field_{idx}'
         # Create a new schema field with the determined type and name
         schema.append(bigquery.SchemaField(name=field_name, field_type=bq_type))
 
     return schema
 
 
+# Takes a pandas dataframe and creates a BigQuery table in target location, with an automatically determined schema.
+def create_bigquery_table_from_dataframe(client: bigquery.Client,
+                                         dataset_id: str,
+                                         table_name: str,
+                                         dataframe: pd.DataFrame):
+    """
+    Create a BigQuery table from a Pandas DataFrame.
+
+    :param client: BigQuery client object.
+    :param dataset_id: ID of the dataset where the table will be created.
+    :param table_name: Name of the table to be created.
+    :param dataframe: Pandas DataFrame containing the data.
+    """
+    # Generate BigQuery schema from DataFrame columns
+    schema = create_schema(dataframe.values[0], dataframe.columns.tolist())
+
+    # Create BigQuery table
+    create_bigquery_table(client, client.project, dataset_id, table_name, schema)
+
+
 # Gets the most up to date data for a table where the target column has an entries within the last n_days
 def get_valid_pages(client, dataset_name, table_name, target_column, date_column, n_days=30, end_date=None):
 
         # Get current time in UTC
         now_utc = dt.datetime.utcnow()
 
         # Calculate start time based on specified number of days
```

### Comparing `metabeaver-0.3.6/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py` & `metabeaver-0.3.7/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Graph Algorithms/depthFirstSearch.py` & `metabeaver-0.3.7/metabeaver/Graph Algorithms/depthFirstSearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Graphing/markdownGenerator.py` & `metabeaver-0.3.7/metabeaver/Graphing/markdownGenerator.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.3.7/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py` & `metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py` & `metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/InterviewQuestions/Arrays/twoSum.py` & `metabeaver-0.3.7/metabeaver/InterviewQuestions/Arrays/twoSum.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py` & `metabeaver-0.3.7/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/LearnPython/ControlFlow/ifelifelse.py` & `metabeaver-0.3.7/metabeaver/LearnPython/ControlFlow/ifelifelse.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Machine Learning/LLM/loadWithTransformers.py` & `metabeaver-0.3.7/metabeaver/Machine Learning/LLM/loadWithTransformers.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Machine Learning/lassoRegression.py` & `metabeaver-0.3.7/metabeaver/Machine Learning/lassoRegression.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Mathematical Operations/vectorDotProduct.py` & `metabeaver-0.3.7/metabeaver/Mathematical Operations/vectorDotProduct.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Search Algorithms/binarySearch.py` & `metabeaver-0.3.7/metabeaver/Search Algorithms/binarySearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Set Theory/findAllSubsets.py` & `metabeaver-0.3.7/metabeaver/Set Theory/findAllSubsets.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Sorting Algorithms/heapSort.py` & `metabeaver-0.3.7/metabeaver/Sorting Algorithms/heapSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Sorting Algorithms/insertionSort.py` & `metabeaver-0.3.7/metabeaver/Sorting Algorithms/insertionSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Sorting Algorithms/mergeSort.py` & `metabeaver-0.3.7/metabeaver/Sorting Algorithms/mergeSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Sorting Algorithms/quickSort.py` & `metabeaver-0.3.7/metabeaver/Sorting Algorithms/quickSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Sorting Algorithms/timsort.py` & `metabeaver-0.3.7/metabeaver/Sorting Algorithms/timsort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/Testing/scratchPad.py` & `metabeaver-0.3.7/metabeaver/Testing/scratchPad.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/TextValidation/closureChecker.py` & `metabeaver-0.3.7/metabeaver/TextValidation/closureChecker.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/TextValidation/establishLargestPalindrome.py` & `metabeaver-0.3.7/metabeaver/TextValidation/establishLargestPalindrome.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver/WebScraping/simpleRequests.py` & `metabeaver-0.3.7/metabeaver/WebScraping/simpleRequests.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.6/metabeaver.egg-info/PKG-INFO` & `metabeaver-0.3.7/metabeaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.3.6
+Version: 0.3.7
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: numpy
```

### Comparing `metabeaver-0.3.6/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.3.7/metabeaver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 metabeaver/DatabaseFunctionality/SQLite/__init__.py
 metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
 metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
 metabeaver/DatesAndTime/__init__.py
 metabeaver/DatesAndTime/getToday.py
 metabeaver/Dynamic Programming/__init__.py
 metabeaver/FileIO/__init__.py
+metabeaver/FileIO/pickleObject.py
 metabeaver/FileIO/yamlIO.py
 metabeaver/Formatting/__init__.py
 metabeaver/Formatting/printControl.py
 metabeaver/Formatting/printControlTest.py
 metabeaver/GoogleCloudPlatform/__init__.py
 metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
 metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
```

### Comparing `metabeaver-0.3.6/setup.py` & `metabeaver-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.3.6', # Major, minor, patch
+    version='0.3.7', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-core',
         'numpy',
         'pandas',
         #transformers,
```

