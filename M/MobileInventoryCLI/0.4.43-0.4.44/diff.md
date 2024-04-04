# Comparing `tmp/MobileInventoryCLI-0.4.43.tar.gz` & `tmp/MobileInventoryCLI-0.4.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.43.tar", last modified: Wed Apr  3 04:04:48 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.44.tar", last modified: Thu Apr  4 15:07:15 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.43.tar` & `MobileInventoryCLI-0.4.44.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.627046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.630379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.633712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.637046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.637046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.637046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.637046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.637046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.637046 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.640379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34801 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.640379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.640379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.640379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.640379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-03 04:04:44.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.640379 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-03 04:03:34.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-03 04:04:48.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-03 04:04:48.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-03 04:04:48.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-03 04:04:48.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-03 04:04:48.000000 MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-03 04:04:48.643712 MobileInventoryCLI-0.4.43/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      810 2024-04-03 04:04:48.000000 MobileInventoryCLI-0.4.43/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.274943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.278276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-04 14:53:24.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-04 15:03:39.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-04 15:07:09.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      810 2024-04-04 15:07:14.000000 MobileInventoryCLI-0.4.44/setup.py
```

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         explanation_color=Fore.light_green
 
         self.helpText=f'''
 {cmd_color}CMD{Style.reset}- {explanation_color}Explanation{Style.reset}
 {Fore.cyan}Billing Info -----------{Style.reset}
 {cmd_color}new_b|newb|nb{Style.reset}- {explanation_color}create new business information{Style.reset}
 {cmd_color}view_db|viewb|vdb{Style.reset}- {explanation_color}view DEFAULT business information{Style.reset}
-{cmd_color}view_all_business|view_ab|vab{Style.reset}- {explanation_color}view ALL business information{Style.reset}
+{cmd_color}view_all_billing|view_ab|vab{Style.reset}- {explanation_color}view ALL business information{Style.reset}
 {cmd_color}remove_bid{Style.reset}- {explanation_color}remove business information by id, or comma separated list of id's{Style.reset}
 {cmd_color}setdefaultid|sdi{Style.reset}- {explanation_color}set default business, and all others are set to non-default{Style.reset}
 {cmd_color}edit_business|eb{Style.reset}- {explanation_color}edit business details {Fore.light_red}{Style.bold}You will be asked for a 'yes' or 'no' before being asked for the value!{Style.reset}
 {cmd_color}search_billing_text|sbt{Style.reset}- {explanation_color}search billing text fields{Style.reset}
 {Fore.spring_green_3a}ReceiptEntry CMD's ----{Style.reset}
 {cmd_color}mkrcpt|make_receipt|pos{Style.reset}- {explanation_color}add entry items to {Style.reset}
 {cmd_color}dltr|del_receipt|rr{Style.reset}- {explanation_color}remove Reciept.RecieptId and ReceiptEntry.RecieptId{Style.reset}
@@ -68,15 +68,15 @@
                 cmd=Prompt.__init2__(None,func=mkT,ptext="Do What",helpText=self.helpText,data=self)
                 if cmd in [None,]:
                     return
                 if cmd.lower() in ['new_b','newb','nb']:
                     self.mkBusiness()
                 elif cmd.lower() in ['view_db','viewdb','vdb']:
                     self.viewDefault()
-                elif cmd.lower() in ['view_all_business','view_ab','vab']:
+                elif cmd.lower() in ['view_all_billing','view_ab','vab']:
                     self.viewAll()
                 elif cmd.lower() in ['remove_bid',]:
                     self.removeId()
                 elif cmd.lower() in ['edit_business','eb']:
                     self.edit_business()
                 elif cmd.lower() in ['setdefaultid','sdi']:
                     self.setdefaultid()
```

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -204,14 +204,26 @@
 this option uses the PairCollection's Table which is independent of the Entry's table.
 {Style.reset}
 {Fore.light_magenta}Switch to Shelf Tag Locator Mode [9]{Style.reset}
 {Fore.light_green}Scan a Product Barcode, then scan shelf tags until a match is found or use quits(q)/backs up a menu(b)
 this option uses the Entry's Table which is independent of the PairCollection's table.
 {Style.reset}
 
+{Fore.light_magenta}Switch to POS Mode[16 or {Style.bold}pos{Style.reset}{Fore.light_magenta}]{Style.reset}
+{Fore.cyan}Task Order{Style.reset}{Fore.light_yellow} ->{Style.reset} Task Mode Cmd [{Fore.light_green}Explanation{Style.reset}]
+{Fore.cyan}newb|new_b|nb{Style.reset} ->{Fore.light_yellow} Create New Billing Information Entry{Style.reset}
+{Fore.cyan}view_db|viewdb|vdb{Style.reset} ->{Fore.light_yellow}View Default Billing Information Entry{Style.reset}
+{Fore.cyan}view_all_billing|view_ab|vab{Style.reset} ->{Fore.light_yellow}View All Billing information{Style.reset}
+{Fore.cyan}listr|ls_rcpt|lr{Style.reset} ->{Fore.light_yellow} List Reciepts{Style.reset}
+{Fore.cyan}deltr|del_reciept|rr{Style.reset} ->{Fore.light_yellow} Delete a reciept by RecieptId{Style.reset}
+{Fore.cyan}newb|new_b|nb{Style.reset} ->{Fore.light_yellow} Create New Business Information Entry{Style.reset}
+{Fore.cyan}mkrcpt|make_receipt|{Style.bold}pos{Style.reset} ->{Fore.light_yellow} Create New Reciept/Invoice{Style.reset}
+{Fore.cyan}are|add_rcpt_ent|add_reciept_entry{Style.reset} ->{Fore.light_yellow} Update Reciept Entry with new items{Style.reset}
+{Fore.cyan}search_billing_text|{Style.bold}sbt{Style.reset} ->{Fore.light_yellow}Search Billing text{Style.reset}
+
 {Fore.light_magenta}Switch to Task Mode [t]{Style.reset}
 {Fore.cyan}Task Order{Style.reset}{Fore.light_yellow} ->{Style.reset} Task Mode Cmd [{Fore.light_green}Explanation{Style.reset}]
 {Fore.cyan}1{Style.reset} ->{Fore.light_yellow} ca{Style.reset} [{Fore.light_green}Clear All List Maker Qty's{Style.reset}]
 
 {Fore.light_magenta}Switch to Task Mode [t]{Style.reset}
 {Fore.cyan}Task Order{Style.reset}{Fore.light_yellow} ->{Style.reset} Task Mode Cmd [{Fore.light_green}Explanation{Style.reset}]
 {Fore.cyan}1{Style.reset} ->{Fore.light_yellow} #40{Style.reset} [{Fore.light_green}Starbux water Display Barge and Display at end of Self-Checkout{Style.reset}]
```

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.43
+Version: 0.4.44
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.43/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.43/PKG-INFO` & `MobileInventoryCLI-0.4.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.43
+Version: 0.4.44
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.43/setup.py` & `MobileInventoryCLI-0.4.44/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.43'
+version='0.4.44'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

