# Comparing `tmp/MobileInventoryCLI-0.4.44.tar.gz` & `tmp/MobileInventoryCLI-0.4.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.44.tar", last modified: Thu Apr  4 15:07:15 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.45.tar", last modified: Thu Apr  4 17:57:23 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.44.tar` & `MobileInventoryCLI-0.4.45.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.274943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.278276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.281610 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-04 14:53:24.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-04 15:03:39.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.284943 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-04 15:07:09.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.288276 MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-03 04:04:57.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-04 15:07:15.000000 MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-04 15:07:15.291610 MobileInventoryCLI-0.4.44/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      810 2024-04-04 15:07:14.000000 MobileInventoryCLI-0.4.44/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.585045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.588378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28740 2024-04-04 17:55:15.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.591712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.595045 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-04 17:57:19.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.598378 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-04 15:07:27.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 17:57:23.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-04 17:57:23.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-04 17:57:23.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-04 17:57:23.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-04 17:57:23.000000 MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-04 17:57:23.601712 MobileInventoryCLI-0.4.45/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      810 2024-04-04 17:57:23.000000 MobileInventoryCLI-0.4.45/setup.py
```

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,19 +35,29 @@
             'desc':'collect code pairs',
         },
         'collect_barcode_w_nu_code':{
             'cmds':['collect_barcode_w_nu_code','1bnuc'],
             'exec':self.collect_barcode_w_nu_code,
             'desc':'collect code pairs with item code, but do not check item code uniqueness [all item code duplicates!]',
         },
+         'collect_barcode_w_nu_code_plus':{
+            'cmds':['collect_barcode_w_nu_code+','1bnuc+'],
+            'exec':self.collect_barcode_w_nu_code_plus,
+            'desc':'collect code pairs with item code, but do not check item code uniqueness [all item code duplicates!], check entry db for barcodes dont add if found',
+        },
         'collect_barcode_wo_nu_code':{
             'cmds':['collect_barcode_w_nu_code','1bnoc'],
             'exec':self.collect_barcode_wo_nu_code,
             'desc':'collect code pairs without item code!]',
         },
+        'collect_barcode_wo_nu_code_plus':{
+            'cmds':['collect_barcode_w_nu_code+','1bnoc+'],
+            'exec':self.collect_barcode_wo_nu_code_plus,
+            'desc':'collect code pairs without item code, but do not add if found in Entry table!]',
+        },
         'export':{
             'cmds':['export','2'],
             'exec':self.export,
             'desc':'export code pairs',
         },
         'edit':{
             'cmds':['edit','3'],
@@ -146,14 +156,33 @@
                         self.cmds[c]['exec']()
                     break
                 elif self.cmds[c]['exec']==None and cmd.lower() in self.cmds[c]['cmds']:
                     return
                 elif self.parent != None and self.parent.Unified(cmd):
                     print("ran an external command!")
                     break
+    def checkEntryForBarcode(self,barcode):
+        try:
+            with Session(self.engine) as session:
+                results=session.query(Entry).filter(Entry.Barcode==barcode).all()
+                ct=len(results)
+                if ct != 0:
+                    print(f"{Fore.light_magenta}{'-*-'*2} Entry Found {'-*-'*2}{Style.reset}")
+                for num,i in enumerate(results):
+                    msg=f"""{Fore.yellow}{num}/{Style.reset}{Fore.light_red}{ct}{Style.reset} {Fore.magenta}{Style.bold}FOUND{Style.reset} -> {i}"""
+                    print(msg)
+                if ct != 0:
+                    print(f"{Fore.light_magenta}{'-*-'*2} Entry Found {'-*-'*2}{Style.reset}")
+                if ct == 0:
+                    return False
+                elif ct != 0:
+                    return True
+        except Exception as e:
+            print(e)
+
 
     def edit(self,ID,field=None,value=None):
         try:
             if field and value:
                 with Session(self.engine) as session:
                     result=session.query(PairCollection).filter(PairCollection.PairCollectionId==ID).first()
                     if result:
@@ -430,14 +459,41 @@
                         print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
 
                     else:
                         print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
                 print(Style.reset)
             except Exception as e:
                 print(e)
+    def collect_barcode_wo_nu_code_plus(self):
+        while True:
+            try:                
+                def mkT(text,self):
+                    return text
+                barcode=Prompt.__init2__(None,func=mkT,ptext="Barcode",helpText="Barcode to Store in PairCollections",data=self)
+                if barcode == None:
+                    return
+                t=self.checkEntryForBarcode(barcode=barcode)
+                if t:
+                    continue
+                with Session(self.engine) as session:
+                    query=session.query(PairCollection).filter(PairCollection.Barcode==barcode)
+                    result=query.first()
+                    if not result:
+                        pcd=PairCollection(Barcode=barcode,Code="No_CODE",Name=f"New Item Created From Scan @ {datetime.now().ctime()}")
+                        session.add(pcd)
+                        session.commit()
+                        session.flush()
+                        session.refresh(pcd)
+                        print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
+
+                    else:
+                        print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
+                print(Style.reset)
+            except Exception as e:
+                print(e)
 
     def collect_barcode_w_nu_code(self):
         while True:
             try:
                 print(Style.reset)
                 def mkT(text,self):
                     return text
@@ -454,14 +510,51 @@
                
                 with Session(self.engine) as session:
                     query=session.query(PairCollection).filter(PairCollection.Barcode==barcode)
                     result=query.first()
                     if not result:
                         pcd=PairCollection(Barcode=barcode,Code=code,Name=f"New Item Created From Scan @ {datetime.now().ctime()}")
                         session.add(pcd)
+                        session.commit()
+                        session.flush()
+                        session.refresh(pcd)
+                        print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
+
+                    else:
+                        print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
+                print(Style.reset)
+            except Exception as e:
+                print(e)
+
+    def collect_barcode_w_nu_code_plus(self):
+        while True:
+            try:
+                print(Style.reset)
+                def mkT(text,self):
+                    return text
+                barcode=Prompt.__init2__(None,func=mkT,ptext="Barcode",helpText="Barcode to Store in PairCollections",data=self)
+                if barcode == None:
+                    return
+
+                def mkT(text,self):
+                    return text
+                code=Prompt.__init2__(None,func=mkT,ptext=f"{Style.bold}{Fore.dark_goldenrod}Shelf Tag Code/ItemCode/Code/CIC:",helpText="Code to Store in PairCollections",data=self)
+                if code == None:
+                    return
+
+                t=self.checkEntryForBarcode(barcode=barcode)
+                if t:
+                    continue
+               
+                with Session(self.engine) as session:
+                    query=session.query(PairCollection).filter(PairCollection.Barcode==barcode)
+                    result=query.first()
+                    if not result:
+                        pcd=PairCollection(Barcode=barcode,Code=code,Name=f"New Item Created From Scan @ {datetime.now().ctime()}")
+                        session.add(pcd)
                         session.commit()
                         session.flush()
                         session.refresh(pcd)
                         print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
 
                     else:
                         print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
```

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.44
+Version: 0.4.45
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.44/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.45/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.44/PKG-INFO` & `MobileInventoryCLI-0.4.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.44
+Version: 0.4.45
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.44/setup.py` & `MobileInventoryCLI-0.4.45/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.44'
+version='0.4.45'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

