# Comparing `tmp/metabeaver-0.3.9.tar.gz` & `tmp/metabeaver-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.3.9.tar", last modified: Thu Apr  4 19:21:15 2024, max compression
+gzip compressed data, was "metabeaver-0.4.0.tar", last modified: Thu Apr  4 19:54:00 2024, max compression
```

## Comparing `metabeaver-0.3.9.tar` & `metabeaver-0.4.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.397422 metabeaver-0.3.9/
--rw-rw-rw-   0        0        0      682 2024-04-04 19:21:15.382406 metabeaver-0.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.190961 metabeaver-0.3.9/metabeaver/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.222620 metabeaver-0.3.9/metabeaver/BeaverTown/
--rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.9/metabeaver/BeaverTown/__init__.py
--rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.9/metabeaver/BeaverTown/abstractBeaver.py
--rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.9/metabeaver/BeaverTown/beaverOn.py
--rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.9/metabeaver/BeaverTown/pumpkinPie.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.238351 metabeaver-0.3.9/metabeaver/Binary/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Binary/__init__.py
--rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.9/metabeaver/Binary/binaryOperations.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.238351 metabeaver-0.3.9/metabeaver/Caching/
--rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.9/metabeaver/Caching/LeastRecentlyUsed.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Caching/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.238351 metabeaver-0.3.9/metabeaver/DataManipulation/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.9/metabeaver/DataManipulation/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.3.9/metabeaver/DataManipulation/filterPandas.py
--rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.9/metabeaver/DataManipulation/localPickle.py
--rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.9/metabeaver/DataManipulation/universalResourceLinkHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.254457 metabeaver-0.3.9/metabeaver/DataStructures/
--rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.9/metabeaver/DataStructures/BinarySearchTree.py
--rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.9/metabeaver/DataStructures/Node.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.9/metabeaver/DataStructures/firstInFirstOutQueue.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.9/metabeaver/DataStructures/firstInLastOut.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.9/metabeaver/DataStructures/linkedList.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.254457 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.254457 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQL/
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQL/__init__.py
--rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.270099 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/
--rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
--rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.9/metabeaver/DatabaseFunctionality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.270099 metabeaver-0.3.9/metabeaver/DatesAndTime/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.9/metabeaver/DatesAndTime/__init__.py
--rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.9/metabeaver/DatesAndTime/getToday.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.282127 metabeaver-0.3.9/metabeaver/Dynamic Programming/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Dynamic Programming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.286757 metabeaver-0.3.9/metabeaver/FileIO/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/FileIO/__init__.py
--rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.3.9/metabeaver/FileIO/pickleObject.py
--rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.9/metabeaver/FileIO/yamlIO.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.286757 metabeaver-0.3.9/metabeaver/Formatting/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.9/metabeaver/Formatting/__init__.py
--rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.9/metabeaver/Formatting/printControl.py
--rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.9/metabeaver/Formatting/printControlTest.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.286757 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.302953 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     7559 2024-04-04 19:20:08.000000 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0     3354 2024-04-04 19:05:00.000000 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
--rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
--rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.302953 metabeaver-0.3.9/metabeaver/Graph Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Graph Algorithms/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.9/metabeaver/Graph Algorithms/bellmanFord.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.9/metabeaver/Graph Algorithms/breadthFirstSearch.py
--rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.9/metabeaver/Graph Algorithms/depthFirstSearch.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.9/metabeaver/Graph Algorithms/dijkstra.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.9/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.318723 metabeaver-0.3.9/metabeaver/Graphing/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.9/metabeaver/Graphing/__init__.py
--rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.9/metabeaver/Graphing/markdownGenerator.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.318723 metabeaver-0.3.9/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.9/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.318723 metabeaver-0.3.9/metabeaver/InterviewQuestions/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.333742 metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
--rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
--rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/twoSum.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.336215 metabeaver-0.3.9/metabeaver/InterviewQuestions/Stacks/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/Stacks/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/InterviewQuestions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.336215 metabeaver-0.3.9/metabeaver/LearnPython/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.336215 metabeaver-0.3.9/metabeaver/LearnPython/ControlFlow/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/LearnPython/ControlFlow/__init__.py
--rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.9/metabeaver/LearnPython/ControlFlow/ifelifelse.py
--rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.9/metabeaver/LearnPython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.336215 metabeaver-0.3.9/metabeaver/Machine Learning/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.349734 metabeaver-0.3.9/metabeaver/Machine Learning/LLM/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Machine Learning/LLM/__init__.py
--rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.9/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
--rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.9/metabeaver/Machine Learning/LLM/loadWithTransformers.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Machine Learning/__init__.py
--rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.9/metabeaver/Machine Learning/lassoRegression.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.349734 metabeaver-0.3.9/metabeaver/Mathematical Operations/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Mathematical Operations/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.9/metabeaver/Mathematical Operations/greatestCommonDenominator.py
--rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.9/metabeaver/Mathematical Operations/vectorDotProduct.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.349734 metabeaver-0.3.9/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.349734 metabeaver-0.3.9/metabeaver/OperationBeaver/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/OperationBeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.365397 metabeaver-0.3.9/metabeaver/Search Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Search Algorithms/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.9/metabeaver/Search Algorithms/binarySearch.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.365397 metabeaver-0.3.9/metabeaver/Set Theory/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Set Theory/__init__.py
--rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.9/metabeaver/Set Theory/findAllSubsets.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.365397 metabeaver-0.3.9/metabeaver/Sorting Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/Sorting Algorithms/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.9/metabeaver/Sorting Algorithms/heapSort.py
--rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.9/metabeaver/Sorting Algorithms/insertionSort.py
--rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.9/metabeaver/Sorting Algorithms/mergeSort.py
--rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.9/metabeaver/Sorting Algorithms/quickSort.py
--rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.9/metabeaver/Sorting Algorithms/timsort.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.382406 metabeaver-0.3.9/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.9/metabeaver/Testing/scratchPad.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.382406 metabeaver-0.3.9/metabeaver/TextValidation/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.9/metabeaver/TextValidation/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.9/metabeaver/TextValidation/closureChecker.py
--rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.9/metabeaver/TextValidation/establishLargestPalindrome.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.382406 metabeaver-0.3.9/metabeaver/WebScraping/
--rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.9/metabeaver/WebScraping/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.9/metabeaver/WebScraping/simpleRequests.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.9/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:21:15.382406 metabeaver-0.3.9/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      682 2024-04-04 19:21:15.000000 metabeaver-0.3.9/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4078 2024-04-04 19:21:15.000000 metabeaver-0.3.9/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 19:21:15.000000 metabeaver-0.3.9/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-04 19:21:15.000000 metabeaver-0.3.9/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 19:21:15.000000 metabeaver-0.3.9/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 19:21:15.397422 metabeaver-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1299 2024-04-04 19:20:59.000000 metabeaver-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.703094 metabeaver-0.4.0/
+-rw-rw-rw-   0        0        0      682 2024-04-04 19:54:00.703094 metabeaver-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.286297 metabeaver-0.4.0/metabeaver/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.381375 metabeaver-0.4.0/metabeaver/BeaverTown/
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.4.0/metabeaver/BeaverTown/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.4.0/metabeaver/BeaverTown/abstractBeaver.py
+-rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.4.0/metabeaver/BeaverTown/beaverOn.py
+-rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.4.0/metabeaver/BeaverTown/pumpkinPie.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.387888 metabeaver-0.4.0/metabeaver/Binary/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Binary/__init__.py
+-rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.4.0/metabeaver/Binary/binaryOperations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.392745 metabeaver-0.4.0/metabeaver/Caching/
+-rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.4.0/metabeaver/Caching/LeastRecentlyUsed.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Caching/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.406019 metabeaver-0.4.0/metabeaver/DataManipulation/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.0/metabeaver/DataManipulation/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.4.0/metabeaver/DataManipulation/filterPandas.py
+-rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.4.0/metabeaver/DataManipulation/localPickle.py
+-rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.4.0/metabeaver/DataManipulation/universalResourceLinkHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.438159 metabeaver-0.4.0/metabeaver/DataStructures/
+-rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.4.0/metabeaver/DataStructures/BinarySearchTree.py
+-rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.4.0/metabeaver/DataStructures/Node.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.4.0/metabeaver/DataStructures/firstInFirstOutQueue.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.4.0/metabeaver/DataStructures/firstInLastOut.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.4.0/metabeaver/DataStructures/linkedList.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.438697 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.444417 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQL/
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQL/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.453246 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/
+-rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
+-rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.4.0/metabeaver/DatabaseFunctionality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.460902 metabeaver-0.4.0/metabeaver/DatesAndTime/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.0/metabeaver/DatesAndTime/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.4.0/metabeaver/DatesAndTime/getToday.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.465604 metabeaver-0.4.0/metabeaver/Dynamic Programming/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Dynamic Programming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.469077 metabeaver-0.4.0/metabeaver/FileIO/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/FileIO/__init__.py
+-rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.4.0/metabeaver/FileIO/pickleObject.py
+-rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.4.0/metabeaver/FileIO/yamlIO.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.477281 metabeaver-0.4.0/metabeaver/Formatting/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.0/metabeaver/Formatting/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.4.0/metabeaver/Formatting/printControl.py
+-rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.4.0/metabeaver/Formatting/printControlTest.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.478300 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.510343 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     7559 2024-04-04 19:20:08.000000 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0     3388 2024-04-04 19:42:42.000000 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
+-rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
+-rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.526739 metabeaver-0.4.0/metabeaver/Graph Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Graph Algorithms/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.4.0/metabeaver/Graph Algorithms/bellmanFord.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.4.0/metabeaver/Graph Algorithms/breadthFirstSearch.py
+-rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.4.0/metabeaver/Graph Algorithms/depthFirstSearch.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.4.0/metabeaver/Graph Algorithms/dijkstra.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.4.0/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.530779 metabeaver-0.4.0/metabeaver/Graphing/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.0/metabeaver/Graphing/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.4.0/metabeaver/Graphing/markdownGenerator.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.534683 metabeaver-0.4.0/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.4.0/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.538285 metabeaver-0.4.0/metabeaver/InterviewQuestions/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.548296 metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
+-rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
+-rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/twoSum.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.556403 metabeaver-0.4.0/metabeaver/InterviewQuestions/Stacks/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/Stacks/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/InterviewQuestions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.559609 metabeaver-0.4.0/metabeaver/LearnPython/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.577142 metabeaver-0.4.0/metabeaver/LearnPython/ControlFlow/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/LearnPython/ControlFlow/__init__.py
+-rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.4.0/metabeaver/LearnPython/ControlFlow/ifelifelse.py
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.4.0/metabeaver/LearnPython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.582000 metabeaver-0.4.0/metabeaver/Machine Learning/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.588023 metabeaver-0.4.0/metabeaver/Machine Learning/LLM/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Machine Learning/LLM/__init__.py
+-rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.4.0/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
+-rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.4.0/metabeaver/Machine Learning/LLM/loadWithTransformers.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Machine Learning/__init__.py
+-rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.4.0/metabeaver/Machine Learning/lassoRegression.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.598146 metabeaver-0.4.0/metabeaver/Mathematical Operations/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Mathematical Operations/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.4.0/metabeaver/Mathematical Operations/greatestCommonDenominator.py
+-rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.4.0/metabeaver/Mathematical Operations/vectorDotProduct.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.608296 metabeaver-0.4.0/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.608296 metabeaver-0.4.0/metabeaver/OperationBeaver/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/OperationBeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.623278 metabeaver-0.4.0/metabeaver/Search Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Search Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.4.0/metabeaver/Search Algorithms/binarySearch.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.635367 metabeaver-0.4.0/metabeaver/Set Theory/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Set Theory/__init__.py
+-rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.4.0/metabeaver/Set Theory/findAllSubsets.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.661698 metabeaver-0.4.0/metabeaver/Sorting Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/Sorting Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.4.0/metabeaver/Sorting Algorithms/heapSort.py
+-rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.4.0/metabeaver/Sorting Algorithms/insertionSort.py
+-rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.4.0/metabeaver/Sorting Algorithms/mergeSort.py
+-rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.4.0/metabeaver/Sorting Algorithms/quickSort.py
+-rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.4.0/metabeaver/Sorting Algorithms/timsort.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.669574 metabeaver-0.4.0/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.4.0/metabeaver/Testing/scratchPad.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.688547 metabeaver-0.4.0/metabeaver/TextValidation/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.0/metabeaver/TextValidation/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.4.0/metabeaver/TextValidation/closureChecker.py
+-rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.4.0/metabeaver/TextValidation/establishLargestPalindrome.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.698083 metabeaver-0.4.0/metabeaver/WebScraping/
+-rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.4.0/metabeaver/WebScraping/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.4.0/metabeaver/WebScraping/simpleRequests.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.0/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:54:00.698083 metabeaver-0.4.0/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      682 2024-04-04 19:54:00.000000 metabeaver-0.4.0/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4078 2024-04-04 19:54:00.000000 metabeaver-0.4.0/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:54:00.000000 metabeaver-0.4.0/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-04 19:54:00.000000 metabeaver-0.4.0/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 19:54:00.000000 metabeaver-0.4.0/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:54:00.703094 metabeaver-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-04-04 19:53:45.000000 metabeaver-0.4.0/setup.py
```

### Comparing `metabeaver-0.3.9/PKG-INFO` & `metabeaver-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.3.9
+Version: 0.4.0
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: numpy
```

### Comparing `metabeaver-0.3.9/metabeaver/BeaverTown/abstractBeaver.py` & `metabeaver-0.4.0/metabeaver/BeaverTown/abstractBeaver.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/BeaverTown/beaverOn.py` & `metabeaver-0.4.0/metabeaver/BeaverTown/beaverOn.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Binary/binaryOperations.py` & `metabeaver-0.4.0/metabeaver/Binary/binaryOperations.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Caching/LeastRecentlyUsed.py` & `metabeaver-0.4.0/metabeaver/Caching/LeastRecentlyUsed.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DataManipulation/filterPandas.py` & `metabeaver-0.4.0/metabeaver/DataManipulation/filterPandas.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DataManipulation/localPickle.py` & `metabeaver-0.4.0/metabeaver/DataManipulation/localPickle.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DataManipulation/universalResourceLinkHandler.py` & `metabeaver-0.4.0/metabeaver/DataManipulation/universalResourceLinkHandler.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DataStructures/BinarySearchTree.py` & `metabeaver-0.4.0/metabeaver/DataStructures/BinarySearchTree.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQL/rawSQL.py` & `metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQL/rawSQL.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py` & `metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py` & `metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py` & `metabeaver-0.4.0/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/DatesAndTime/getToday.py` & `metabeaver-0.4.0/metabeaver/DatesAndTime/getToday.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/FileIO/yamlIO.py` & `metabeaver-0.4.0/metabeaver/FileIO/yamlIO.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Formatting/printControlTest.py` & `metabeaver-0.4.0/metabeaver/Formatting/printControlTest.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py` & `metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py` & `metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import yaml
 
 from typing import List
 import pandas as pd
 
 
 # Return a credentials via supplying a service_account.Credentials with valid credential.json loc GCP API calls
-def get_credentials_from_yaml(yaml_file_path):
+def get_credentials_from_yaml(yaml_file_path, cloud_platform, service_json_filepath):
 
     # Attempt to load a service_account.Credentials from a YAML file reference to stored location."""
     try:
         # Try to load the YAML file
         with open(yaml_file_path, 'r') as yaml_file:
             config = yaml.safe_load(yaml_file)
 
         # Extract path to service account JSON file from YAML config
-        credentials_path = config['credentials']['service_account_json_path']
+        credentials_path = config[cloud_platform][service_json_filepath]
 
         # Load service account credentials from JSON file and return the credentials to be used in API calls.
         credentials = service_account.Credentials.from_service_account_file(credentials_path)
         return credentials
     # Print any Exception associated with retrieval.
     except Exception as e:
         print(f"Error: {e}")
```

### Comparing `metabeaver-0.3.9/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py` & `metabeaver-0.4.0/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Graph Algorithms/depthFirstSearch.py` & `metabeaver-0.4.0/metabeaver/Graph Algorithms/depthFirstSearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Graphing/markdownGenerator.py` & `metabeaver-0.4.0/metabeaver/Graphing/markdownGenerator.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.4.0/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py` & `metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py` & `metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/InterviewQuestions/Arrays/twoSum.py` & `metabeaver-0.4.0/metabeaver/InterviewQuestions/Arrays/twoSum.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py` & `metabeaver-0.4.0/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/LearnPython/ControlFlow/ifelifelse.py` & `metabeaver-0.4.0/metabeaver/LearnPython/ControlFlow/ifelifelse.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Machine Learning/LLM/loadWithTransformers.py` & `metabeaver-0.4.0/metabeaver/Machine Learning/LLM/loadWithTransformers.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Machine Learning/lassoRegression.py` & `metabeaver-0.4.0/metabeaver/Machine Learning/lassoRegression.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Mathematical Operations/vectorDotProduct.py` & `metabeaver-0.4.0/metabeaver/Mathematical Operations/vectorDotProduct.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Search Algorithms/binarySearch.py` & `metabeaver-0.4.0/metabeaver/Search Algorithms/binarySearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Set Theory/findAllSubsets.py` & `metabeaver-0.4.0/metabeaver/Set Theory/findAllSubsets.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Sorting Algorithms/heapSort.py` & `metabeaver-0.4.0/metabeaver/Sorting Algorithms/heapSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Sorting Algorithms/insertionSort.py` & `metabeaver-0.4.0/metabeaver/Sorting Algorithms/insertionSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Sorting Algorithms/mergeSort.py` & `metabeaver-0.4.0/metabeaver/Sorting Algorithms/mergeSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Sorting Algorithms/quickSort.py` & `metabeaver-0.4.0/metabeaver/Sorting Algorithms/quickSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Sorting Algorithms/timsort.py` & `metabeaver-0.4.0/metabeaver/Sorting Algorithms/timsort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/Testing/scratchPad.py` & `metabeaver-0.4.0/metabeaver/Testing/scratchPad.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/TextValidation/closureChecker.py` & `metabeaver-0.4.0/metabeaver/TextValidation/closureChecker.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/TextValidation/establishLargestPalindrome.py` & `metabeaver-0.4.0/metabeaver/TextValidation/establishLargestPalindrome.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver/WebScraping/simpleRequests.py` & `metabeaver-0.4.0/metabeaver/WebScraping/simpleRequests.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/metabeaver.egg-info/PKG-INFO` & `metabeaver-0.4.0/metabeaver.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.3.9
+Version: 0.4.0
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: numpy
```

### Comparing `metabeaver-0.3.9/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.4.0/metabeaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.9/setup.py` & `metabeaver-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.3.9', # Major, minor, patch
+    version='0.4.0', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-core',
         'numpy',
         'pandas',
         #transformers,
```

