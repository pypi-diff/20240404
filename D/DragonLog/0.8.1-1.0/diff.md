# Comparing `tmp/DragonLog-0.8.1.tar.gz` & `tmp/DragonLog-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DragonLog-0.8.1.tar", last modified: Wed Mar 27 06:18:53 2024, max compression
+gzip compressed data, was "DragonLog-1.0.tar", last modified: Thu Apr  4 05:34:36 2024, max compression
```

## Comparing `DragonLog-0.8.1.tar` & `DragonLog-1.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 06:18:53.798893 DragonLog-0.8.1/
-drwxrwxrwx   0        0        0        0 2024-03-27 06:18:53.793404 DragonLog-0.8.1/DragonLog.egg-info/
--rw-rw-rw-   0        0        0     7347 2024-03-27 06:18:53.000000 DragonLog-0.8.1/DragonLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1555 2024-03-27 06:18:53.000000 DragonLog-0.8.1/DragonLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 06:18:53.000000 DragonLog-0.8.1/DragonLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-27 06:18:53.000000 DragonLog-0.8.1/DragonLog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-03-27 06:18:53.000000 DragonLog-0.8.1/DragonLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 06:18:53.000000 DragonLog-0.8.1/DragonLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 DragonLog-0.8.1/LICENCE.txt
--rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 DragonLog-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7347 2024-03-27 06:18:53.795899 DragonLog-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     6345 2024-03-25 18:19:47.000000 DragonLog-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 06:18:53.700589 DragonLog-0.8.1/dragonlog/
--rw-rw-rw-   0        0        0    58995 2024-03-26 06:57:11.000000 DragonLog-0.8.1/dragonlog/DragonLog.py
--rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 DragonLog-0.8.1/dragonlog/DragonLog_AppSelect.py
--rw-rw-rw-   0        0        0     3041 2024-03-27 06:17:55.000000 DragonLog-0.8.1/dragonlog/DragonLog_AppSelect_ui.py
--rw-rw-rw-   0        0        0     5971 2024-03-27 06:07:28.000000 DragonLog-0.8.1/dragonlog/DragonLog_CallBook.py
--rw-rw-rw-   0        0        0     5904 2024-03-25 18:19:47.000000 DragonLog-0.8.1/dragonlog/DragonLog_LoTW.py
--rw-rw-rw-   0        0        0    16563 2024-03-27 06:17:54.000000 DragonLog-0.8.1/dragonlog/DragonLog_MainWindow_ui.py
--rw-rw-rw-   0        0        0    40792 2024-03-27 05:50:27.000000 DragonLog-0.8.1/dragonlog/DragonLog_QSOForm.py
--rw-rw-rw-   0        0        0    37529 2024-03-27 06:17:54.000000 DragonLog-0.8.1/dragonlog/DragonLog_QSOForm_ui.py
--rw-rw-rw-   0        0        0      914 2024-03-05 19:23:18.000000 DragonLog-0.8.1/dragonlog/DragonLog_RegEx.py
--rw-rw-rw-   0        0        0    18535 2024-03-25 18:19:47.000000 DragonLog-0.8.1/dragonlog/DragonLog_Settings.py
--rw-rw-rw-   0        0        0    38585 2024-03-27 06:17:55.000000 DragonLog-0.8.1/dragonlog/DragonLog_Settings_ui.py
--rw-rw-rw-   0        0        0     5324 2024-03-23 19:55:25.000000 DragonLog-0.8.1/dragonlog/DragonLog_eQSL.py
--rw-rw-rw-   0        0        0     2422 2024-03-23 19:55:25.000000 DragonLog-0.8.1/dragonlog/Logger.py
--rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 DragonLog-0.8.1/dragonlog/__init__.py
--rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 DragonLog-0.8.1/dragonlog/__main__.py
--rw-rw-rw-   0        0        0       65 2024-03-27 06:17:54.000000 DragonLog-0.8.1/dragonlog/__version__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:18:53.713064 DragonLog-0.8.1/dragonlog/data/
--rw-rw-rw-   0        0        0     6345 2024-03-25 18:19:47.000000 DragonLog-0.8.1/dragonlog/data/README.md
--rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 DragonLog-0.8.1/dragonlog/data/bands.json
--rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 DragonLog-0.8.1/dragonlog/data/cb_channels.json
--rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 DragonLog-0.8.1/dragonlog/data/color_map.json
-drwxrwxrwx   0        0        0        0 2024-03-27 06:18:53.717555 DragonLog-0.8.1/dragonlog/data/i18n/
--rw-rw-rw-   0        0        0    22273 2024-03-27 06:17:56.000000 DragonLog-0.8.1/dragonlog/data/i18n/DragonLog_de.qm
--rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 DragonLog-0.8.1/dragonlog/data/modes.json
-drwxrwxrwx   0        0        0        0 2024-03-27 06:18:53.788913 DragonLog-0.8.1/dragonlog/icons/
--rw-rw-rw-   0        0        0    63030 2024-03-10 12:41:11.000000 DragonLog-0.8.1/dragonlog/icons/Screenshot.png
--rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 DragonLog-0.8.1/dragonlog/icons/db.png
--rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 DragonLog-0.8.1/dragonlog/icons/edit.png
--rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 DragonLog-0.8.1/dragonlog/icons/edit_add.png
--rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 DragonLog-0.8.1/dragonlog/icons/edit_addmulti.png
--rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 DragonLog-0.8.1/dragonlog/icons/edit_addmulti.xcf
--rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 DragonLog-0.8.1/dragonlog/icons/edit_remove.png
--rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 DragonLog-0.8.1/dragonlog/icons/exit.png
--rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 DragonLog-0.8.1/dragonlog/icons/file_doc.png
--rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 DragonLog-0.8.1/dragonlog/icons/fileexport.png
--rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 DragonLog-0.8.1/dragonlog/icons/fileimport.png
--rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 DragonLog-0.8.1/dragonlog/icons/gear.png
--rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 DragonLog-0.8.1/dragonlog/icons/help.png
--rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 DragonLog-0.8.1/dragonlog/icons/icons8-dragon-96.png
--rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 DragonLog-0.8.1/dragonlog/icons/icons8-dragon-96.xcf
--rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 DragonLog-0.8.1/dragonlog/icons/info.png
--rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 DragonLog-0.8.1/dragonlog/icons/logo.ico
--rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 DragonLog-0.8.1/dragonlog/icons/player_play.png
--rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 DragonLog-0.8.1/dragonlog/icons/player_stop.png
--rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 DragonLog-0.8.1/dragonlog/icons/upload_lotw.png
--rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 DragonLog-0.8.1/dragonlog/icons/upload_lotw.xcf
--rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 DragonLog-0.8.1/dragonlog/icons/watch.png
--rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 DragonLog-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 06:18:53.799393 DragonLog-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 DragonLog-0.8.1/setup_msi.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.292085 DragonLog-1.0/
+drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.285091 DragonLog-1.0/DragonLog.egg-info/
+-rw-rw-rw-   0        0        0     7399 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1597 2024-04-04 05:34:36.000000 DragonLog-1.0/DragonLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 DragonLog-1.0/LICENCE.txt
+-rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 DragonLog-1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7399 2024-04-04 05:34:36.289088 DragonLog-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 DragonLog-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.191157 DragonLog-1.0/dragonlog/
+-rw-rw-rw-   0        0        0    61318 2024-04-02 11:52:42.000000 DragonLog-1.0/dragonlog/DragonLog.py
+-rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 DragonLog-1.0/dragonlog/DragonLog_AppSelect.py
+-rw-rw-rw-   0        0        0     3041 2024-04-04 05:33:29.000000 DragonLog-1.0/dragonlog/DragonLog_AppSelect_ui.py
+-rw-rw-rw-   0        0        0     5971 2024-03-27 06:07:28.000000 DragonLog-1.0/dragonlog/DragonLog_CallBook.py
+-rw-rw-rw-   0        0        0     7403 2024-04-01 18:20:40.000000 DragonLog-1.0/dragonlog/DragonLog_LoTW.py
+-rw-rw-rw-   0        0        0    17410 2024-04-04 05:33:28.000000 DragonLog-1.0/dragonlog/DragonLog_MainWindow_ui.py
+-rw-rw-rw-   0        0        0    44824 2024-04-02 19:00:21.000000 DragonLog-1.0/dragonlog/DragonLog_QSOForm.py
+-rw-rw-rw-   0        0        0    40015 2024-04-04 05:33:29.000000 DragonLog-1.0/dragonlog/DragonLog_QSOForm_ui.py
+-rw-rw-rw-   0        0        0     1054 2024-04-02 05:05:28.000000 DragonLog-1.0/dragonlog/DragonLog_RegEx.py
+-rw-rw-rw-   0        0        0    19600 2024-03-29 19:18:43.000000 DragonLog-1.0/dragonlog/DragonLog_Settings.py
+-rw-rw-rw-   0        0        0    38585 2024-04-04 05:33:29.000000 DragonLog-1.0/dragonlog/DragonLog_Settings_ui.py
+-rw-rw-rw-   0        0        0     5324 2024-03-23 19:55:25.000000 DragonLog-1.0/dragonlog/DragonLog_eQSL.py
+-rw-rw-rw-   0        0        0     2484 2024-04-04 05:17:54.000000 DragonLog-1.0/dragonlog/Logger.py
+-rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 DragonLog-1.0/dragonlog/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 DragonLog-1.0/dragonlog/__main__.py
+-rw-rw-rw-   0        0        0       63 2024-04-04 05:33:28.000000 DragonLog-1.0/dragonlog/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.208145 DragonLog-1.0/dragonlog/data/
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 DragonLog-1.0/dragonlog/data/README.md
+-rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 DragonLog-1.0/dragonlog/data/bands.json
+-rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 DragonLog-1.0/dragonlog/data/cb_channels.json
+-rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 DragonLog-1.0/dragonlog/data/color_map.json
+drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.213142 DragonLog-1.0/dragonlog/data/i18n/
+-rw-rw-rw-   0        0        0    23695 2024-04-04 05:33:32.000000 DragonLog-1.0/dragonlog/data/i18n/DragonLog_de.qm
+-rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 DragonLog-1.0/dragonlog/data/i18n/ascii_replace_de.json
+-rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 DragonLog-1.0/dragonlog/data/modes.json
+drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.280093 DragonLog-1.0/dragonlog/icons/
+-rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 DragonLog-1.0/dragonlog/icons/Screenshot.png
+-rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 DragonLog-1.0/dragonlog/icons/db.png
+-rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 DragonLog-1.0/dragonlog/icons/edit.png
+-rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 DragonLog-1.0/dragonlog/icons/edit_add.png
+-rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 DragonLog-1.0/dragonlog/icons/edit_addmulti.png
+-rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 DragonLog-1.0/dragonlog/icons/edit_addmulti.xcf
+-rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 DragonLog-1.0/dragonlog/icons/edit_remove.png
+-rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 DragonLog-1.0/dragonlog/icons/exit.png
+-rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 DragonLog-1.0/dragonlog/icons/file_doc.png
+-rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 DragonLog-1.0/dragonlog/icons/fileexport.png
+-rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 DragonLog-1.0/dragonlog/icons/fileimport.png
+-rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 DragonLog-1.0/dragonlog/icons/gear.png
+-rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 DragonLog-1.0/dragonlog/icons/help.png
+-rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 DragonLog-1.0/dragonlog/icons/icons8-dragon-96.png
+-rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 DragonLog-1.0/dragonlog/icons/icons8-dragon-96.xcf
+-rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 DragonLog-1.0/dragonlog/icons/info.png
+-rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 DragonLog-1.0/dragonlog/icons/logo.ico
+-rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 DragonLog-1.0/dragonlog/icons/player_play.png
+-rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 DragonLog-1.0/dragonlog/icons/player_stop.png
+-rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 DragonLog-1.0/dragonlog/icons/upload_lotw.png
+-rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 DragonLog-1.0/dragonlog/icons/upload_lotw.xcf
+-rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 DragonLog-1.0/dragonlog/icons/watch.png
+-rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 DragonLog-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 05:34:36.293085 DragonLog-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 DragonLog-1.0/setup_msi.py
```

### Comparing `DragonLog-0.8.1/DragonLog.egg-info/PKG-INFO` & `DragonLog-1.0/DragonLog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 0.8.1
+Version: 1.0
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
@@ -49,21 +49,22 @@
 * input validation for callsign, RST, locator
 * show worked before if a callsign is already logged
 * distance calculation
 * automatic time
 * callbook search and log upload (HamQTH.com)
 * eQSL upload, check and download
 * LoTW signing, upload and check status
-* CAT (band, frequency, mode, power via hamlib integration)
+* CAT (band, frequency, mode/submode, power via hamlib integration)
 * watch log files for automatic log import of WSJT-X, JS8Call, fldigi and others
 * ADIF adi/adx export/import
 * Excel/CSV export/import
 * log 11m band QSOs
-* filter recent QSOs (last week, mont, half year, year)
-* UTF-8 (i.e. use german umlauts) and convert german umlauts for ADIF export
+* filter recent QSOs (last week, month, half year, year)
+* UTF-8 (i.e. use german umlauts)
+* convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
 The installation requires a python installation (>= 3.9).
     
     # python3 -m pip install DragonLog
 
@@ -168,15 +169,15 @@
 
 Hamlib integration
 ------------------
 You can use hamlib to interact with your radio. 
 
 The QSO logging form automatically updates radio information:
 * frequency (and band)
-* mode
+* mode (and submode)
 * power
 
 Hamlib can be downloaded at https://github.com/Hamlib/Hamlib/releases.
 DragonLog is tested against version 4.5.5.
 
 After selecting your radio and interface settings you can press the start button to start the communication.
```

### Comparing `DragonLog-0.8.1/DragonLog.egg-info/SOURCES.txt` & `DragonLog-1.0/DragonLog.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 dragonlog/__version__.py
 dragonlog/data/README.md
 dragonlog/data/bands.json
 dragonlog/data/cb_channels.json
 dragonlog/data/color_map.json
 dragonlog/data/modes.json
 dragonlog/data/i18n/DragonLog_de.qm
+dragonlog/data/i18n/ascii_replace_de.json
 dragonlog/icons/Screenshot.png
 dragonlog/icons/db.png
 dragonlog/icons/edit.png
 dragonlog/icons/edit_add.png
 dragonlog/icons/edit_addmulti.png
 dragonlog/icons/edit_addmulti.xcf
 dragonlog/icons/edit_remove.png
```

### Comparing `DragonLog-0.8.1/PKG-INFO` & `DragonLog-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 0.8.1
+Version: 1.0
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
@@ -49,21 +49,22 @@
 * input validation for callsign, RST, locator
 * show worked before if a callsign is already logged
 * distance calculation
 * automatic time
 * callbook search and log upload (HamQTH.com)
 * eQSL upload, check and download
 * LoTW signing, upload and check status
-* CAT (band, frequency, mode, power via hamlib integration)
+* CAT (band, frequency, mode/submode, power via hamlib integration)
 * watch log files for automatic log import of WSJT-X, JS8Call, fldigi and others
 * ADIF adi/adx export/import
 * Excel/CSV export/import
 * log 11m band QSOs
-* filter recent QSOs (last week, mont, half year, year)
-* UTF-8 (i.e. use german umlauts) and convert german umlauts for ADIF export
+* filter recent QSOs (last week, month, half year, year)
+* UTF-8 (i.e. use german umlauts)
+* convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
 The installation requires a python installation (>= 3.9).
     
     # python3 -m pip install DragonLog
 
@@ -168,15 +169,15 @@
 
 Hamlib integration
 ------------------
 You can use hamlib to interact with your radio. 
 
 The QSO logging form automatically updates radio information:
 * frequency (and band)
-* mode
+* mode (and submode)
 * power
 
 Hamlib can be downloaded at https://github.com/Hamlib/Hamlib/releases.
 DragonLog is tested against version 4.5.5.
 
 After selecting your radio and interface settings you can press the start button to start the communication.
```

### Comparing `DragonLog-0.8.1/README.md` & `DragonLog-1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 * input validation for callsign, RST, locator
 * show worked before if a callsign is already logged
 * distance calculation
 * automatic time
 * callbook search and log upload (HamQTH.com)
 * eQSL upload, check and download
 * LoTW signing, upload and check status
-* CAT (band, frequency, mode, power via hamlib integration)
+* CAT (band, frequency, mode/submode, power via hamlib integration)
 * watch log files for automatic log import of WSJT-X, JS8Call, fldigi and others
 * ADIF adi/adx export/import
 * Excel/CSV export/import
 * log 11m band QSOs
-* filter recent QSOs (last week, mont, half year, year)
-* UTF-8 (i.e. use german umlauts) and convert german umlauts for ADIF export
+* filter recent QSOs (last week, month, half year, year)
+* UTF-8 (i.e. use german umlauts)
+* convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
 The installation requires a python installation (>= 3.9).
     
     # python3 -m pip install DragonLog
 
@@ -141,15 +142,15 @@
 
 Hamlib integration
 ------------------
 You can use hamlib to interact with your radio. 
 
 The QSO logging form automatically updates radio information:
 * frequency (and band)
-* mode
+* mode (and submode)
 * power
 
 Hamlib can be downloaded at https://github.com/Hamlib/Hamlib/releases.
 DragonLog is tested against version 4.5.5.
 
 After selecting your radio and interface settings you can press the start button to start the communication.
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog.py` & `DragonLog-1.0/dragonlog/DragonLog.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     OPTION_OPENPYXL = True
 except ImportError:
     pass
 
 from . import DragonLog_MainWindow_ui
 from .Logger import Logger
+from .DragonLog_RegEx import find_non_ascii
 from .DragonLog_QSOForm import QSOForm
 from .DragonLog_Settings import Settings
 from .DragonLog_AppSelect import AppSelect
 from .DragonLog_LoTW import LoTW, LoTWADIFFieldException, LoTWRequestException, LoTWCommunicationException
 
 __prog_name__ = 'DragonLog'
 __prog_desc__ = 'Log QSO for Ham radio'
@@ -72,23 +73,23 @@
 
         option.backgroundBrush = QtGui.QBrush(
             QtGui.QColor(*self.getColor(index.model().data(index.siblingAtColumn(self.column)))))
 
 
 class DragonLog(QtWidgets.QMainWindow, DragonLog_MainWindow_ui.Ui_MainWindow):
     __sql_cols__ = ('id', 'date_time', 'date_time_off', 'own_callsign', 'call_sign', 'name', 'qth', 'locator',
-                    'rst_sent', 'rst_rcvd', 'band', 'mode', 'freq', 'channel', 'power',
+                    'rst_sent', 'rst_rcvd', 'band', 'mode', 'submode', 'freq', 'channel', 'power', 'propagation',
                     'own_name', 'own_qth', 'own_locator', 'radio', 'antenna',
                     'remarks', 'comments', 'dist',
                     'qsl_via', 'qsl_path', 'qsl_msg', 'qsl_sent', 'qsl_rcvd',
                     'eqsl_sent', 'eqsl_rcvd', 'lotw_sent', 'lotw_rcvd', 'hamqth')
 
     __adx_cols__ = (
         'QSO_DATE/TIME_ON', 'QSO_DATE/TIME_OFF', 'STATION_CALLSIGN', 'CALL', 'NAME_INTL', 'QTH_INTL', 'GRIDSQUARE',
-        'RST_SENT', 'RST_RCVD', 'BAND', 'MODE', 'FREQ', 'APP_DRAGONLOG_CBCHANNEL', 'TX_PWR',
+        'RST_SENT', 'RST_RCVD', 'BAND', 'MODE', 'SUBMODE', 'FREQ', 'APP_DRAGONLOG_CBCHANNEL', 'TX_PWR', 'PROP_MODE',
         'MY_NAME_INTL', 'MY_CITY_INTL', 'MY_GRIDSQUARE', 'MY_RIG_INTL', 'MY_ANTENNA_INTL',
         'NOTES_INTL', 'COMMENT_INTL', 'DISTANCE',
         'QSL_VIA', 'QSL_SENT_VIA', 'QSLMSG_INTL', 'QSL_SENT', 'QSL_RCVD',
         'EQSL_QSL_SENT', 'EQSL_QSL_RCVD', 'LOTW_QSL_SENT', 'LOTW_QSL_RCVD', 'HAMQTH_QSO_UPLOAD_STATUS')
 
     __db_create_stmnt__ = '''CREATE TABLE IF NOT EXISTS "qsos" (
                             "id"    INTEGER PRIMARY KEY NOT NULL,
@@ -99,17 +100,19 @@
                             "name"  TEXT,
                             "qth"    TEXT,
                             "locator" TEXT,
                             "rst_sent" TEXT,
                             "rst_rcvd" TEXT,
                             "band"    TEXT,
                             "mode"   TEXT,
+                            "submode"  TEXT,
                             "freq"  REAL,
                             "channel"  INTEGER,
                             "power"  REAL,
+                            "propagation"  TEXT,
                             "own_name"  TEXT,
                             "own_qth"   TEXT,
                             "own_locator" TEXT,
                             "radio"   TEXT,
                             "antenna"   TEXT,
                             "remarks"   TEXT,
                             "comments"   TEXT,
@@ -153,18 +156,21 @@
         self.help_dialog = None
 
         self.settings = QtCore.QSettings(self.tr(__prog_name__))
 
         self.log = Logger(self.logTextEdit, self.settings)
         self.log.info(f'Starting {__prog_name__} {__version__}...')
 
-        dock_area = self.int2dock_area(int(self.settings.value('ui/log_dock_area',
-                                                               QtCore.Qt.DockWidgetArea.BottomDockWidgetArea.value)))
-        self.addDockWidget(dock_area,
-                           self.logDockWidget)
+        if self.settings.value('ui/log_dock_float', 0):
+            self.logDockWidget.setFloating(True)
+        else:
+            log_dock_area = self.int2dock_area(int(self.settings.value('ui/log_dock_area',
+                                                                       QtCore.Qt.DockWidgetArea.BottomDockWidgetArea.value)))
+            self.addDockWidget(log_dock_area,
+                               self.logDockWidget)
         self.logDockWidget.setVisible(bool(self.settings.value('ui/show_log', 0)))
 
         self.dummy_status = QtWidgets.QLabel()
         self.statusBar().addPermanentWidget(self.dummy_status)
         self.watch_status = QtWidgets.QLabel(self.tr('Watching file') + ': ' + self.tr('inactiv'))
         self.statusBar().addPermanentWidget(self.watch_status)
         self.hamlib_status = QtWidgets.QLabel(self.tr('Hamlib') + ': ' + self.tr('inactiv'))
@@ -174,35 +180,69 @@
 
         with open(self.searchFile('data:bands.json')) as bj:
             self.bands: dict = json.load(bj)
         with open(self.searchFile('data:modes.json')) as mj:
             self.modes: dict = json.load(mj)
         with open(self.searchFile('data:cb_channels.json')) as cj:
             self.cb_channels: dict = json.load(cj)
-
         with open(self.searchFile('data:color_map.json')) as cmj:
             color_map: dict = json.load(cmj)
         self.QSOTableView.setItemDelegate(BackgroundBrushDelegate(color_map, self.__sql_cols__.index('band')))
 
+        self.prop: dict = {
+            '': '',
+            'AS': self.tr('Aircraft Scatter'),
+            'AUE': self.tr('Aurora-E'),
+            'AUR': self.tr('Aurora'),
+            'BS': self.tr('Back scatter'),
+            'ECH': self.tr('EchoLink'),
+            'EME': self.tr('Earth-Moon-Earth'),
+            'ES': self.tr('Sporadic E'),
+            'F2': self.tr('F2 Reflection'),
+            'FAI': self.tr('Field Aligned Irregularities'),
+            'GWAVE': self.tr('Ground Wave'),
+            'INTERNET': self.tr('Internet-assisted'),
+            'ION': self.tr('Ionoscatter'),
+            'IRL': self.tr('IRLP'),
+            'LOS': self.tr('Line of Sight'),
+            'MS': self.tr('Meteor scatter'),
+            'RPT': self.tr('Repeater or Transponder'),
+            'RS': self.tr('Rain scatter'),
+            'SAT': self.tr('Satellite'),
+            'TEP': self.tr('Trans-equatorial'),
+            'TR': self.tr('Tropospheric ducting'),
+        }
+
+        self.ascii_replace: dict = {}
+        try:
+            with open(self.searchFile(f'data:i18n/ascii_replace_{QtCore.QLocale.system().name()[:2]}.json'),
+                      encoding='utf-8') as arf:
+                self.ascii_replace = json.load(arf)
+                self.log.debug(f'Loaded ascii_replace from "{arf.name}"')
+        except Exception:
+            self.log.debug(f'Found no ascii_replace_xx.json for "{print(QtCore.QLocale.system().name()[:2])}"')
+
         self.__headers__ = (
             self.tr('QSO'),
             self.tr('Date/Time start'),
             self.tr('Date/Time end'),
             self.tr('Own call sign'),
             self.tr('Call sign'),
             self.tr('Name'),
             self.tr('QTH'),
             self.tr('Locator'),
             self.tr('RST sent'),
             self.tr('RST rcvd'),
             self.tr('Band'),
             self.tr('Mode'),
+            self.tr('Submode'),
             self.tr('Frequency'),
             self.tr('Channel'),
             self.tr('Power'),
+            self.tr('Propagation'),
             self.tr('Own Name'),
             self.tr('Own QTH'),
             self.tr('Own Locator'),
             self.tr('Radio'),
             self.tr('Antenna'),
             self.tr('Notes'),
             self.tr('Comments'),
@@ -219,18 +259,32 @@
             self.tr('HamQTH'),
         )
 
         self.__header_map__ = dict(zip(self.__sql_cols__, self.__headers__))
 
         self.settings_form = Settings(self, self.settings, self.hamlib_status, self.__headers__, self.log)
 
-        self.qso_form = QSOForm(self, self.bands, self.modes, self.settings, self.settings_form,
+        # QSOForm
+        self.qso_form = QSOForm(self, self, self.bands, self.modes, self.prop, self.settings, self.settings_form,
                                 self.cb_channels, self.hamlib_error, self.log)
+        self.qsoDockWidget.setWidget(self.qso_form)
+        self.qsoDockWidget.visibilityChanged.connect(self.qso_form.startTimers)
+
+        if self.settings.value('ui/qso_dock_float', 0):
+            self.qsoDockWidget.setFloating(True)
+        else:
+            qso_dock_area = self.int2dock_area(int(self.settings.value('ui/qso_dock_area',
+                                                                       QtCore.Qt.DockWidgetArea.RightDockWidgetArea.value)))
+            self.addDockWidget(qso_dock_area,
+                               self.qsoDockWidget)
+        self.qsoDockWidget.setVisible(bool(self.settings.value('ui/show_qso', 0)))
+
         self.keep_logging = False
 
+        # Database
         self.__db_con__ = QtSql.QSqlDatabase.addDatabase('QSQLITE', 'main')
 
         if file:
             self.log.info(f'Opening database from commandline {file}...')
             self.connectDB(file)
         elif self.settings.value('lastDatabase', None):
             if os.path.isfile(self.settings.value('lastDatabase', None)):
@@ -256,14 +310,15 @@
                 dock_area = QtCore.Qt.DockWidgetArea.LeftDockWidgetArea
             case 2:
                 dock_area = QtCore.Qt.DockWidgetArea.RightDockWidgetArea
             case 4:
                 dock_area = QtCore.Qt.DockWidgetArea.TopDockWidgetArea
             case 8:
                 dock_area = QtCore.Qt.DockWidgetArea.BottomDockWidgetArea
+
         return dock_area
 
     def showSettings(self):
         if self.settings_form.exec():
             self.refreshTableView()
 
     def selectDB(self):
@@ -453,51 +508,32 @@
         self.QSOTableView.model().setFilter(self.getFilter())
 
     def ctrlHamlib(self, start):
         self.settings_form.ctrlRigctld(start)
 
     def logQSO(self):
         self.qso_form.clear()
-        if not self.keep_logging:
-            self.qso_form.reset()
-
-        dt = QtCore.QDateTime.currentDateTimeUtc()
-        self.qso_form.dateEdit.setDate(dt.date())
-        self.qso_form.dateOnEdit.setDate(dt.date())
-        self.qso_form.timeEdit.setTime(dt.time())
-        self.qso_form.timeOnEdit.setTime(dt.time())
+        self.qso_form.setChangeMode(False)
+        self.qso_form.reset()
+        self.qsoDockWidget.setVisible(True)
 
-        if self.qso_form.exec():
-            self.log.info('Logging QSO...')
-            query = QtSql.QSqlQuery(self.__db_con__)
-            query.prepare(self.__db_insert_stmnt__)
-            for i, val in enumerate(self.qso_form.values):
-                query.bindValue(i, val)
-            query.exec()
-            if query.lastError().text():
-                raise Exception(query.lastError().text())
+    def fetchQSO(self):
+        self.log.info('Logging QSO...')
+        query = QtSql.QSqlQuery(self.__db_con__)
+        query.prepare(self.__db_insert_stmnt__)
+        for i, val in enumerate(self.qso_form.values):
+            query.bindValue(i, val)
+        query.exec()
+        if query.lastError().text():
+            raise Exception(query.lastError().text())
 
-            self.__db_con__.commit()
-        else:
-            self.log.info('Logging aborted')
-            self.keep_logging = False
-            
+        self.__db_con__.commit()
         self.refreshTableView(sort=False)
 
-        self.hamlib_error.setText('')
-
-    def logMultiQSOs(self):
-        self.keep_logging = True
-
-        self.qso_form.setWindowTitle(self.tr('Log multi QSOs'))
-
-        while self.keep_logging:
-            self.logQSO()
-
-        self.qso_form.reset()  # To reset window title
+        self.hamlib_error.setText('')  # TODO: Why???
 
     def deleteQSO(self):
         res = QtWidgets.QMessageBox.question(self, self.tr('Delete QSO'),
                                              self.tr('Do you really want to delete the selected QSO(s)?'),
                                              defaultButton=QtWidgets.QMessageBox.StandardButton.No)
 
         if res == QtWidgets.QMessageBox.StandardButton.Yes:
@@ -519,55 +555,49 @@
                 if query.lastError().text():
                     raise Exception(query.lastError().text())
 
             self.__db_con__.commit()
             self.refreshTableView(sort=False)
 
     def changeQSO(self):
-        done_ids = []
+        self.qso_form.clear()
+        self.qsoDockWidget.setVisible(True)
         self.qso_form.setChangeMode()
 
-        for i in self.QSOTableView.selectedIndexes():
-            qso_id = self.QSOTableView.model().data(i.siblingAtColumn(0))
-
-            if qso_id in done_ids or qso_id is None:
-                continue
-            done_ids.append(qso_id)
-
-            values = []
-            for col in range(len(self.__sql_cols__)):
-                values.append(self.QSOTableView.model().data(i.siblingAtColumn(col)))
-
-            self.qso_form.clear()
-            self.qso_form.setChangeMode()
-            self.qso_form.values = dict(zip(self.__sql_cols__, values))
-
-            self.qso_form.setWindowTitle(self.tr('Change QSO') + f' #{qso_id}')
-
-            if self.qso_form.exec():
-                self.log.info(f'Changing QSO {qso_id}...')
-                values = self.qso_form.values
-                values += (qso_id,)
+        i = self.QSOTableView.selectedIndexes().pop(0)
+        qso_id = self.QSOTableView.model().data(i.siblingAtColumn(0))
 
-                query = QtSql.QSqlQuery(self.__db_con__)
-                query.prepare(self.__db_update_stmnt__)
-
-                for col, val in enumerate(values):
-                    query.bindValue(col, val)
-                query.exec()
-                if query.lastError().text():
-                    raise Exception(query.lastError().text())
-            else:
-                self.log.info('Changing QSO(s) aborted')
-                break
+        values = []
+        for col in range(len(self.__sql_cols__)):
+            values.append(self.QSOTableView.model().data(i.siblingAtColumn(col)))
+
+        self.qso_form.values = dict(zip(self.__sql_cols__, values))
+
+    def updateQSO(self, qso_id: int):
+        self.log.info(f'Changing QSO {qso_id}...')
+        values = self.qso_form.values
+        values += (qso_id,)
+
+        query = QtSql.QSqlQuery(self.__db_con__)
+        query.prepare(self.__db_update_stmnt__)
+
+        for col, val in enumerate(values):
+            query.bindValue(col, val)
+        query.exec()
+        if query.lastError().text():
+            raise Exception(query.lastError().text())
 
         self.__db_con__.commit()
         self.refreshTableView(sort=False)
         self.qso_form.setChangeMode(False)
 
+    def clearQSOForm(self):
+        self.qso_form.clear()
+        self.qso_form.setChangeMode(False)
+
     def export(self):
         exp_formats = {
             self.tr('ADIF 3 (*.adx *.adi *.adif)'): self.exportADIF,
             self.tr('CSV-File (*.csv)'): self.exportCSV,
         }
 
         if OPTION_OPENPYXL:
@@ -659,23 +689,24 @@
         except OSError as e:
             self.log.critical(e)
             QtWidgets.QMessageBox.critical(
                 self,
                 f'{__prog_name__} - {self.tr("Error")}',
                 str(e))
 
-    @staticmethod
-    def replaceUmlautsLigatures(text: str):
-        text = text.replace('Ä', 'Ae')
-        text = text.replace('Ö', 'Oe')
-        text = text.replace('Ü', 'Ue')
-        text = text.replace('ä', 'ae')
-        text = text.replace('ö', 'oe')
-        text = text.replace('ü', 'ue')
-        text = text.replace('ß', 'ss')
+    def replaceNonASCII(self, text: str) -> str:
+        non_ascii = find_non_ascii(text)
+
+        for na in non_ascii:
+            if na:
+                if na in self.ascii_replace:
+                    text = text.replace(na, self.ascii_replace[na])
+                else:
+                    text = text.replace(na, '_')
+
         return text
 
     def exportADIF(self, file):
         self.log.info('Exporting to ADIF...')
 
         query_str = self.getQueryStr() if self.settings.value('imp_exp/only_recent', 0) else self.__db_select_stmnt__
         is_adx: bool = os.path.splitext(file)[-1] == '.adx'
@@ -731,20 +762,20 @@
             if query.value(self.__sql_cols__.index('call_sign')):
                 if band == '11m' and is_adx:
                     record['APP'].append({'@PROGRAMID': 'DRAGONLOG',
                                           '@FIELDNAME': 'CBCALL',
                                           '@TYPE': 'I',
                                           '$': query.value(self.__sql_cols__.index('call_sign'))})
                 else:
-                    record['CALL'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('call_sign')))
+                    record['CALL'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('call_sign')))
             if query.value(self.__sql_cols__.index('name')):
-                record['NAME'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('name')))
+                record['NAME'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('name')))
                 record['NAME_INTL'] = query.value(self.__sql_cols__.index('name'))
             if query.value(self.__sql_cols__.index('qth')):
-                record['QTH'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('qth')))
+                record['QTH'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('qth')))
                 record['QTH_INTL'] = query.value(self.__sql_cols__.index('qth'))
             if query.value(self.__sql_cols__.index('locator')):
                 record['GRIDSQUARE'] = query.value(self.__sql_cols__.index('locator'))
             if query.value(self.__sql_cols__.index('rst_sent')):
                 record['RST_SENT'] = query.value(self.__sql_cols__.index('rst_sent'))
             if query.value(self.__sql_cols__.index('rst_rcvd')):
                 record['RST_RCVD'] = query.value(self.__sql_cols__.index('rst_rcvd'))
@@ -776,49 +807,55 @@
             if query.value(self.__sql_cols__.index('own_callsign')):
                 if band == '11m' and is_adx:
                     record['APP'].append({'@PROGRAMID': 'DRAGONLOG',
                                           '@FIELDNAME': 'CBOWNCALL',
                                           '@TYPE': 'I',
                                           '$': query.value(self.__sql_cols__.index('own_callsign'))})
                 else:
-                    record['STATION_CALLSIGN'] = self.replaceUmlautsLigatures(
+                    record['STATION_CALLSIGN'] = self.replaceNonASCII(
                         query.value(self.__sql_cols__.index('own_callsign')))
             if query.value(self.__sql_cols__.index('own_name')):
-                record['MY_NAME'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('own_name')))
+                record['MY_NAME'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('own_name')))
                 record['MY_NAME_INTL'] = query.value(self.__sql_cols__.index('own_name'))
             if query.value(self.__sql_cols__.index('own_qth')):
-                record['MY_CITY'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('own_qth')))
+                record['MY_CITY'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('own_qth')))
                 record['MY_CITY_INTL'] = query.value(self.__sql_cols__.index('own_qth'))
             if query.value(self.__sql_cols__.index('own_locator')):
                 record['MY_GRIDSQUARE'] = query.value(self.__sql_cols__.index('own_locator'))
             if query.value(self.__sql_cols__.index('radio')):
-                record['MY_RIG'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('radio')))
+                record['MY_RIG'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('radio')))
                 record['MY_RIG_INTL'] = query.value(self.__sql_cols__.index('radio'))
             if query.value(self.__sql_cols__.index('antenna')):
-                record['MY_ANTENNA'] = self.replaceUmlautsLigatures(query.value(self.__sql_cols__.index('antenna')))
+                record['MY_ANTENNA'] = self.replaceNonASCII(query.value(self.__sql_cols__.index('antenna')))
                 record['MY_ANTENNA_INTL'] = query.value(self.__sql_cols__.index('antenna'))
             if query.value(self.__sql_cols__.index('dist')):
                 record['DISTANCE'] = query.value(self.__sql_cols__.index('dist'))
             if query.value(self.__sql_cols__.index('remarks')) and bool(
                     self.settings.value('imp_exp/own_notes_adif', 0)):
-                record['NOTES'] = self.replaceUmlautsLigatures(
-                    query.value(self.__sql_cols__.index('remarks')).replace('\n', '\r\n'))
-                record['NOTES_INTL'] = query.value(self.__sql_cols__.index('remarks')).replace('\n', '\r\n')
+                remarks = query.value(self.__sql_cols__.index('remarks'))
+                if platform.system() == 'Linux':
+                    remarks = remarks.replace('\n', '\r\n')
+                record['NOTES'] = self.replaceNonASCII(remarks)
+                record['NOTES_INTL'] = remarks
             if query.value(self.__sql_cols__.index('comments')):
-                record['COMMENT'] = self.replaceUmlautsLigatures(
-                    query.value(self.__sql_cols__.index('comments')).replace('\n', '\r\n'))
-                record['COMMENT_INTL'] = query.value(self.__sql_cols__.index('comments')).replace('\n', '\r\n')
+                comment = query.value(self.__sql_cols__.index('comments'))
+                if platform.system() == 'Linux':
+                    comment = comment.replace('\n', '\r\n')
+                record['COMMENT'] = self.replaceNonASCII(comment)
+                record['COMMENT_INTL'] = comment
             if query.value(self.__sql_cols__.index('qsl_via')):
                 record['QSL_VIA'] = query.value(self.__sql_cols__.index('qsl_via'))
             if query.value(self.__sql_cols__.index('qsl_path')):
                 record['QSL_SENT_VIA'] = query.value(self.__sql_cols__.index('qsl_path'))
             if query.value(self.__sql_cols__.index('qsl_msg')):
-                record['QSLMSG'] = self.replaceUmlautsLigatures(
-                    query.value(self.__sql_cols__.index('qsl_msg')).replace('\n', '\r\n'))
-                record['QSLMSG_INTL'] = query.value(self.__sql_cols__.index('qsl_msg')).replace('\n', '\r\n')
+                qsl_msg = query.value(self.__sql_cols__.index('qsl_msg'))
+                if platform.system() == 'Linux':
+                    qsl_msg = qsl_msg.replace('\n', '\r\n')
+                record['QSLMSG'] = self.replaceNonASCII(qsl_msg)
+                record['QSLMSG_INTL'] = qsl_msg
             if query.value(self.__sql_cols__.index('qsl_sent')):
                 record['QSL_SENT'] = query.value(self.__sql_cols__.index('qsl_sent'))
             if query.value(self.__sql_cols__.index('qsl_rcvd')):
                 record['QSL_RCVD'] = query.value(self.__sql_cols__.index('qsl_rcvd'))
             if query.value(self.__sql_cols__.index('eqsl_sent')):
                 record['EQSL_QSL_SENT'] = query.value(self.__sql_cols__.index('eqsl_sent'))
             if query.value(self.__sql_cols__.index('eqsl_rcvd')):
@@ -1030,15 +1067,15 @@
                     f'QSO date/time missing in record {i}.\nSkipped record.'
                 )
                 continue
 
             query = QtSql.QSqlQuery(self.__db_con__)
             query.prepare(self.__db_insert_stmnt__)
 
-            for j, val in enumerate(self._build_values_adiimport_(r)):
+            for j, val in enumerate(self._build_adif_import_(r)):
                 query.bindValue(j, val)
             query.exec()
             if query.lastError().text():
                 QtWidgets.QMessageBox.warning(
                     self,
                     self.tr('Log import ADIF'),
                     f'Record {i} import error ("{query.lastError().text()}").\nSkipped record.'
@@ -1047,15 +1084,15 @@
                 imported += 1
 
         self.__db_con__.commit()
         self.refreshTableView()
 
         self.log.info(f'Imported {imported} QSOs from "{file}"')
 
-    def _build_values_adiimport_(self, r, use_cfg_id=False, use_cfg_station=False):
+    def _build_adif_import_(self, r, use_cfg_id=False, use_cfg_station=False):
         values = [''] * (len(self.__sql_cols__) - 1)
         date = r['QSO_DATE']
         timex = r['TIME_ON']
         time = f'{timex[:2]}:{timex[2:4]}' if len(timex) == 4 else f'{timex[:2]}:{timex[2:4]}:{timex[4:6]}'
         values[0] = f'{date[:4]}-{date[4:6]}-{date[6:8]} {time}'
         if 'TIME_OFF' in r:
             date_off = r['QSO_DATE_OFF'] if 'QSO_DATE_OFF' in r else date  # Fallback
@@ -1074,32 +1111,38 @@
             values[self.__sql_cols__.index('radio') - 1] = self.settings.value('station/radio', '')
             values[self.__sql_cols__.index('antenna') - 1] = self.settings.value('station/antenna', '')
             values[self.__sql_cols__.index('own_qth') - 1] = self.settings.value('station/QTH', '')
             values[self.__sql_cols__.index('own_locator') - 1] = self.settings.value('station/own_locator', '')
 
         values[self.__sql_cols__.index('channel') - 1] = '-'
 
+        submode_eval = False
+
         for p in r:
             match p:
                 case 'QSO_DATE' | 'TIME_ON' | 'QSO_DATE_OFF' | 'TIME_OFF' | 'APP_DRAGONLOG_CBQSO':
                     continue
                 case 'BAND':
                     values[self.__adx_cols__.index(p)] = r[p].lower()
                 case 'FREQ':
                     freq = r[p].replace(',', '.')  # Workaround for wrong export from fldigi
                     values[self.__adx_cols__.index(p)] = str(float(freq) * 1000)
                 case 'MODE':
-                    if r[p] in self.modes['AFU'] or r[p] in self.modes['CB']:
+                    if r[p] in self.modes['AFU'] or r[p] in self.modes['CB']:  # If it is a main mode
                         values[self.__adx_cols__.index(p)] = r[p]
                     else:  # Workaround for wrong mode export from fldigi
-                        # TODO: store in submode if Dragonlog supports submodes
                         for m in self.modes['AFU']:
                             if r[p] in self.modes['AFU'][m]:
                                 values[self.__adx_cols__.index(p)] = m
+                                values[self.__adx_cols__.index('SUBMODE')] = r[p]
+                                submode_eval = True
                                 break
+                case 'SUBMODE':
+                    if not submode_eval:  # Set only if not already evaluated from mode
+                        values[self.__adx_cols__.index(p)] = r[p]
                 case 'APP':  # Only for ADX as ADI App fields are recognised the standard way
                     for af in r[p]:
                         af_param = f'APP_{af["@PROGRAMID"].upper()}_{af["@FIELDNAME"].upper()}'
                         if af_param in self.__adx_cols__:
                             values[self.__adx_cols__.index(af_param)] = af['$']
                         elif af_param == 'APP_DRAGONLOG_CBCALL':
                             values[self.__adx_cols__.index('CALL')] = af['$']
@@ -1147,19 +1190,19 @@
 
             if not self.findQSO(timestamp, rec['CALL']):
                 self.log.info(f'Adding QSO #{i} from "{self.watchFileName}" to logbook...')
 
                 query = QtSql.QSqlQuery(self.__db_con__)
                 query.prepare(self.__db_insert_stmnt__)
 
-                for j, val in enumerate(self._build_values_adiimport_(rec,
-                                                                      bool(self.settings.value('imp_exp/use_id_watch',
-                                                                                               0)),
-                                                                      bool(self.settings.value(
-                                                                          'imp_exp/use_station_watch', 0)))):
+                for j, val in enumerate(self._build_adif_import_(rec,
+                                                                 bool(self.settings.value('imp_exp/use_id_watch',
+                                                                                          0)),
+                                                                 bool(self.settings.value(
+                                                                     'imp_exp/use_station_watch', 0)))):
                     query.bindValue(j, val)
                 query.exec()
                 if query.lastError().text():
                     self.log.error(
                         f'Record #{self.watchPos + 1} import error from watched file ("{query.lastError().text()}").'
                         'Skipped.')
 
@@ -1287,16 +1330,23 @@
 
     def showAboutQt(self):
         QtWidgets.QMessageBox.aboutQt(self, __prog_name__ + ' - ' + self.tr('About Qt'))
 
     def closeEvent(self, e):
         self.log.info(f'Quiting {__prog_name__}...')
         self.__db_con__.close()
+
         self.settings.setValue('ui/show_log', int(self.logDockWidget.isVisible()))
         self.settings.setValue('ui/log_dock_area', self.dockWidgetArea(self.logDockWidget).value)
+        self.settings.setValue('ui/log_dock_float', int(self.logDockWidget.isFloating()))
+
+        self.settings.setValue('ui/show_qso', int(self.qsoDockWidget.isVisible()))
+        self.settings.setValue('ui/qso_dock_area', self.dockWidgetArea(self.qsoDockWidget).value)
+        self.settings.setValue('ui/qso_dock_float', int(self.qsoDockWidget.isFloating()))
+
         self.settings_form.ctrlRigctld(False)
         e.accept()
 
 
 def main():
     app = QtWidgets.QApplication(sys.argv)
     app_path = os.path.dirname(__file__)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_AppSelect.py` & `DragonLog-1.0/dragonlog/DragonLog_AppSelect.py`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_AppSelect_ui.py` & `DragonLog-1.0/dragonlog/DragonLog_AppSelect_ui.py`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_CallBook.py` & `DragonLog-1.0/dragonlog/DragonLog_CallBook.py`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_LoTW.py` & `DragonLog-1.0/dragonlog/DragonLog_eQSL.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,148 @@
 import re
-import os.path
 import logging
-import platform
-import tempfile
-import subprocess
 
 import requests
 from adif_file import adi
-from PyQt6 import QtCore
 
 from .Logger import Logger
 
 
-class LoTWCommunicationException(Exception):
+class EQSLCommunicationException(Exception):
     pass
 
 
-class LoTWRequestException(Exception):
+class EQSLRequestException(Exception):
     pass
 
 
-class LoTWLoginException(Exception):
+class EQSLLoginException(Exception):
     pass
 
 
-class LoTWNoRecordException(Exception):
+class EQSLUserCallMatchException(Exception):
     pass
 
 
-class LoTWADIFFieldException(Exception):
+class EQSLQSODuplicateException(Exception):
     pass
 
 
-class LoTW:
+class EQSLADIFFieldException(Exception):
+    pass
+
+
+class EQSL:
     required_fields = ('QSO_DATE', 'TIME_ON', 'CALL', 'MODE', 'BAND')
-    fields = required_fields + ('FREQ', 'QSLMSG', 'RST_SENT', 'MY_GRIDSQUARE', 'STATION_CALLSIGN')
-    REGEX_RECORDS = re.compile(r'(?:.*?<[eE][oO][hH]>)?\n*(.*?<[eE][oO][rR]>).*?', re.DOTALL)
+    fields = required_fields + ('FREQ', 'QSLMSG', 'RST_SENT', 'MY_GRIDSQUARE')
+    image_pattern = re.compile(r'.*<img src="(.*)" alt="" />.*')
+    upl_res_pattern = re.compile(r' *([EWCIR][a-z]*:.*)<BR>')
 
-    def __init__(self, logger: Logger):
-        self.log = logging.getLogger('LoTW')
+    def __init__(self, program: str, logger: Logger):
+        self.__program_str__ = program
+
+        self.log = logging.getLogger('EQSL')
         self.log.addHandler(logger)
         self.log.setLevel(logger.loglevel)
         self.logger = logger
         self.log.debug('Initialising...')
 
-    def upload_log(self, station: str, doc: dict, password: str = '') -> bool:
-        self._check_fields_(doc)
+    def upload_log(self, username: str, password: str, record: dict) -> bool:
+        self._check_fields_(record)
 
-        # Export to tempfile
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            tmp_file = os.path.join(tmp_dir, 'DragonLog_Export.adi')
-            adi.dump(tmp_file, doc, 'ADIF Export by DragonLog')
+        record = record.copy()
 
-            if platform.system() == 'Windows':
-                tqsl_path = 'C:/Program Files (x86)/TrustedQSL/tqsl.exe'
-            else:
-                tqsl_path = 'tqsl'
+        for field in list(record.keys()):
+            if not field in self.fields:
+                record.pop(field)
 
-            cmd = [tqsl_path,
-                   '-d',  # Supress date range dialog
-                   '-u',  # Directly upload
-                   '-a', 'all',  # Sign all including already sent
-                   '-f', 'ignore',  # Ignore QTH information
-                   '-x',  # Batch mode
-                   '-l', station,
-                   tmp_file]
-            if password:
-                cmd.append('-p')
-                cmd.append(password)
-
-            res = subprocess.run(cmd, capture_output=True)
-            match res.returncode:
-                case 0:
-                    self.log.debug('TQSL exited with success')
-                    return True
-                case 1:  # Will it be possible?
-                    self.log.debug('TQSL canceled by user')
-                case 2:
-                    self.log.warning('Log rejected by LoTW')
-                    raise LoTWRequestException
-                case 3 | 4 | 5:
-                    self.log.error(f'Local or server error: {res.returncode}')
-                case 6 | 7:  # Should not occur on tempfile
-                    self.log.error(f'Error for read/write on input/output file: {res.returncode}')
-                case 8:  # Should never occur
-                    self.log.warning('TQSL no QSOs were processed')
-                case 9:
-                    self.log.warning('TQSL some QSOs were already uploaded')
-                    return True
-                case 10:  # Should not occur due to tested syntax
-                    self.log.error('TQSL command syntax error')
-                case 11:
-                    self.log.warning('LoTW Connection error or network unreachable')
-                    raise LoTWCommunicationException()
-
-        return False
-
-    def _check_fields_(self, doc: dict):
-        for i, record in enumerate(doc['RECORDS']):
-            for field in self.required_fields:
-                if field not in record:
-                    raise LoTWADIFFieldException(f'{field} in record #{i + 1}')
-
-    def check_inbox(self, username: str, password: str, record: dict) -> bool:
-        self._check_fields_({'RECORDS': [record]})
-        self.log.debug(f"Checking inbox for {record['CALL']} on {record['QSO_DATE']}")
-
-        if not username or not password:
-            raise LoTWLoginException('Missing username or password')
-
-        qso_dt = QtCore.QDateTime.fromString(
-            f"{record['QSO_DATE'][:4]}-{record['QSO_DATE'][4:6]}-{record['QSO_DATE'][6:8]} "
-            f"{record['TIME_ON'][:2]}:{record['TIME_ON'][2:4]}",
-            'yyyy-MM-dd hh:mm')
-        start_dt = qso_dt.addSecs(-600)
-        end_dt = qso_dt.addSecs(600)
+        record['ADIF_VER'] = '3.1.4'
+        record['PROGRAMID'] = self.__program_str__
 
-        self.log.debug(f"Filter QSOs between {start_dt.toString('yyyy-MM-dd hh:mm')} and "
-                       f"{end_dt.toString('yyyy-MM-dd hh:mm')}")
+        # Skip header and remove linebreaks
+        data = adi.dumps({'RECORDS': [record]}).replace('\n', ' ')
 
         params = {
-            'login': username,
-            'password': password,
-            'qso_query': '1',
-            'qso_callsing': record['CALL'],
-            'qso_startdate': start_dt.date().toString('yyyy-MM-dd'),
-            'qso_starttime': start_dt.time().toString('hh:mm'),
-            'qso_enddate': end_dt.date().toString('yyyy-MM-dd'),
-            'qso_endtime': end_dt.time().toString('hh:mm'),
-            'qso_band': record['BAND'],
-            'qso_mode': record['MODE'],
+            'ADIFData': 'QSL-Upload ' + data,
+            'EQSL_USER': username,
+            'EQSL_PSWD': password,
         }
 
-        r = requests.get('https://lotw.arrl.org/lotwuser/lotwreport.adi', params=params)
+        r = requests.get('https://www.eQSL.cc/qslcard/importADIF.cfm', params=params)
+
         if r.status_code == 200:
-            if r.text.strip().endswith('<APP_LoTW_EOF>'):
-                records = re.findall(self.REGEX_RECORDS, r.text)
-                if len(records) > 1:
-                    raise LoTWRequestException('Too much search results')
-                elif len(records) == 0:
-                    raise LoTWNoRecordException('No search results')
+            for res in re.findall(self.upl_res_pattern, r.text):
+                if 'Error' in res:
+                    if ('No match on eQSL_User/eQSL_Pswd' in res or
+                            'Multiple accounts match eQSL_User/eQSL_Pswd' in res):
+                        raise EQSLUserCallMatchException(res)
+                    elif 'Missing eQSL_User' in res or 'Missing eQSL_Pswd' in res:
+                        raise EQSLLoginException(res)
+                    elif 'Missing ADIFData parameter' in res:
+                        raise EQSLADIFFieldException(res)
+                    else:
+                        raise EQSLRequestException(res)
+                elif 'Warning' in res:
+                    if 'Bad record: Duplicate' in res:
+                        raise EQSLQSODuplicateException(res)
+                    else:
+                        raise EQSLADIFFieldException(res)
+                elif 'Caution' in res:
+                    self.log.warning(f'eQSL result: {res}')
+                elif 'Information' in res:
+                    self.log.info(f'eQSL result: {res}')
+                elif 'Result' in res:
+                    self.log.debug(f'eQSL result: {res}')
 
-                try:
-                    doc = adi.loads(records[0].strip())
+            return True
+        else:
+            raise EQSLCommunicationException(f'eQSL error: HTTP-Error {r.status_code}')
 
-                    if doc['RECORDS'][0]['QSL_RCVD'] == 'Y':
-                        return True
-                    else:
-                        return False
-                except adi.TagDefinitionException as exc:
-                    raise LoTWRequestException(exc)
+    def _check_fields_(self, record: dict):
+        for field in self.required_fields:
+            if field not in record:
+                raise EQSLADIFFieldException(field)
+
+    def check_inbox(self, username: str, password: str, record: dict) -> str:
+        self._check_fields_(record)
+
+        params = {
+            'Username': username,
+            'Password': password,
+            'CallsignFrom': record['CALL'],
+            'QSOYear': record['QSO_DATE'][:4],
+            'QSOMonth': record['QSO_DATE'][4:6],
+            'QSODay': record['QSO_DATE'][6:],
+            'QSOHour': record['TIME_ON'][:2],
+            'QSOMinute': record['TIME_ON'][2:4],
+            'QSOBand': record['BAND'],
+            'QSOMode': record['MODE'],
+        }
+
+        r = requests.get('https://www.eQSL.cc/qslcard/GeteQSL.cfm', params=params)
+
+        if r.status_code == 200:
+            if r.text.strip().startswith('Error'):
+                if ('No match on Username/Password for that QSO Date/Time' in r.text or
+                        'overlapping accounts for that QSO Date/Time' in r.text):
+                    raise EQSLUserCallMatchException(r.text.strip())
+                elif ('User is Regular member but must be at least Silver to download mass eQSLs.' in r.text or
+                      'User is Bronze member but must be at least Silver to download mass eQSLs.' in r.text or
+                      'Not Authorized to download mass eQSLs.' in r.text):
+                    raise EQSLLoginException(r.text.strip())
+                else:
+                    raise EQSLRequestException(r.text.strip())
             else:
-                raise LoTWLoginException()
+                url_part = re.findall(self.image_pattern, r.text)
+                if url_part:
+                    return 'https://www.eQSL.cc' + url_part[0]
+        else:
+            raise EQSLCommunicationException(f'eQSL error: HTTP-Error {r.status_code}')
+
+    @staticmethod
+    def receive_qsl_card(url: str) -> bytes:
+        r = requests.get(url)
+
+        if r.status_code == 200:
+            return r.content
         else:
-            raise LoTWCommunicationException(f'LoTW error: HTTP-Error {r.status_code}')
+            raise EQSLCommunicationException(f'eQSL error: HTTP-Error {r.status_code}')
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_MainWindow_ui.py` & `DragonLog-1.0/dragonlog/DragonLog_MainWindow_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
-        MainWindow.resize(1200, 600)
+        MainWindow.resize(1300, 900)
         icon = QtGui.QIcon()
         icon.addPixmap(QtGui.QPixmap("icons:icons8-dragon-96.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         MainWindow.setWindowIcon(icon)
         self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout.setObjectName("verticalLayout")
@@ -26,15 +26,15 @@
         self.QSOTableView.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectionBehavior.SelectRows)
         self.QSOTableView.setSortingEnabled(True)
         self.QSOTableView.setObjectName("QSOTableView")
         self.QSOTableView.verticalHeader().setVisible(False)
         self.verticalLayout.addWidget(self.QSOTableView)
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QtWidgets.QMenuBar(parent=MainWindow)
-        self.menubar.setGeometry(QtCore.QRect(0, 0, 1200, 22))
+        self.menubar.setGeometry(QtCore.QRect(0, 0, 1300, 22))
         self.menubar.setObjectName("menubar")
         self.menuFile = QtWidgets.QMenu(parent=self.menubar)
         self.menuFile.setObjectName("menuFile")
         self.menuEdit = QtWidgets.QMenu(parent=self.menubar)
         self.menuEdit.setObjectName("menuEdit")
         self.menuHelp = QtWidgets.QMenu(parent=self.menubar)
         self.menuHelp.setObjectName("menuHelp")
@@ -43,28 +43,41 @@
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
         self.toolBar = QtWidgets.QToolBar(parent=MainWindow)
         self.toolBar.setObjectName("toolBar")
         MainWindow.addToolBar(QtCore.Qt.ToolBarArea.TopToolBarArea, self.toolBar)
         self.logDockWidget = QtWidgets.QDockWidget(parent=MainWindow)
         self.logDockWidget.setFeatures(QtWidgets.QDockWidget.DockWidgetFeature.DockWidgetClosable|QtWidgets.QDockWidget.DockWidgetFeature.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetFeature.DockWidgetMovable)
+        self.logDockWidget.setAllowedAreas(QtCore.Qt.DockWidgetArea.BottomDockWidgetArea|QtCore.Qt.DockWidgetArea.TopDockWidgetArea)
         self.logDockWidget.setObjectName("logDockWidget")
-        self.dockWidgetContents = QtWidgets.QWidget()
-        self.dockWidgetContents.setObjectName("dockWidgetContents")
-        self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.dockWidgetContents)
+        self.logDockWidgetContents = QtWidgets.QWidget()
+        self.logDockWidgetContents.setObjectName("logDockWidgetContents")
+        self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.logDockWidgetContents)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.logTextEdit = QtWidgets.QTextEdit(parent=self.dockWidgetContents)
+        self.logTextEdit = QtWidgets.QTextEdit(parent=self.logDockWidgetContents)
         font = QtGui.QFont()
         font.setFamily("Courier New")
         self.logTextEdit.setFont(font)
         self.logTextEdit.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.TextSelectableByKeyboard|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.logTextEdit.setObjectName("logTextEdit")
         self.verticalLayout_2.addWidget(self.logTextEdit)
-        self.logDockWidget.setWidget(self.dockWidgetContents)
-        MainWindow.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.logDockWidget)
+        self.logDockWidget.setWidget(self.logDockWidgetContents)
+        MainWindow.addDockWidget(QtCore.Qt.DockWidgetArea(8), self.logDockWidget)
+        self.qsoDockWidget = QtWidgets.QDockWidget(parent=MainWindow)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.MinimumExpanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.qsoDockWidget.sizePolicy().hasHeightForWidth())
+        self.qsoDockWidget.setSizePolicy(sizePolicy)
+        self.qsoDockWidget.setAllowedAreas(QtCore.Qt.DockWidgetArea.LeftDockWidgetArea|QtCore.Qt.DockWidgetArea.RightDockWidgetArea)
+        self.qsoDockWidget.setObjectName("qsoDockWidget")
+        self.qsoDockWidgetContents = QtWidgets.QWidget()
+        self.qsoDockWidgetContents.setObjectName("qsoDockWidgetContents")
+        self.qsoDockWidget.setWidget(self.qsoDockWidgetContents)
+        MainWindow.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.qsoDockWidget)
         self.actionLog_QSO = QtGui.QAction(parent=MainWindow)
         icon1 = QtGui.QIcon()
         icon1.addPixmap(QtGui.QPixmap("icons:edit_add.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionLog_QSO.setIcon(icon1)
         self.actionLog_QSO.setObjectName("actionLog_QSO")
         self.actionLog_QSO_TB = QtGui.QAction(parent=MainWindow)
         self.actionLog_QSO_TB.setIcon(icon1)
@@ -88,14 +101,20 @@
         self.actionExport.setIcon(icon4)
         self.actionExport.setObjectName("actionExport")
         self.actionImport = QtGui.QAction(parent=MainWindow)
         icon5 = QtGui.QIcon()
         icon5.addPixmap(QtGui.QPixmap("icons:fileimport.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionImport.setIcon(icon5)
         self.actionImport.setObjectName("actionImport")
+        self.actionExport_TB = QtGui.QAction(parent=MainWindow)
+        self.actionExport_TB.setIcon(icon4)
+        self.actionExport_TB.setObjectName("actionExport_TB")
+        self.actionImport_TB = QtGui.QAction(parent=MainWindow)
+        self.actionImport_TB.setIcon(icon5)
+        self.actionImport_TB.setObjectName("actionImport_TB")
         self.actionAbout = QtGui.QAction(parent=MainWindow)
         icon6 = QtGui.QIcon()
         icon6.addPixmap(QtGui.QPixmap("icons:info.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionAbout.setIcon(icon6)
         self.actionAbout.setObjectName("actionAbout")
         self.actionAbout_Qt = QtGui.QAction(parent=MainWindow)
         self.actionAbout_Qt.setIcon(icon6)
@@ -114,64 +133,55 @@
         icon9 = QtGui.QIcon()
         icon9.addPixmap(QtGui.QPixmap("icons:gear.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionSettings.setIcon(icon9)
         self.actionSettings.setObjectName("actionSettings")
         self.actionSettings_TB = QtGui.QAction(parent=MainWindow)
         self.actionSettings_TB.setIcon(icon9)
         self.actionSettings_TB.setObjectName("actionSettings_TB")
-        self.actionLog_multi_QSOs = QtGui.QAction(parent=MainWindow)
-        icon10 = QtGui.QIcon()
-        icon10.addPixmap(QtGui.QPixmap("icons:edit_addmulti.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionLog_multi_QSOs.setIcon(icon10)
-        self.actionLog_multi_QSOs.setObjectName("actionLog_multi_QSOs")
-        self.actionLog_multi_QSOs_TB = QtGui.QAction(parent=MainWindow)
-        self.actionLog_multi_QSOs_TB.setIcon(icon10)
-        self.actionLog_multi_QSOs_TB.setObjectName("actionLog_multi_QSOs_TB")
         self.actionHelp = QtGui.QAction(parent=MainWindow)
-        icon11 = QtGui.QIcon()
-        icon11.addPixmap(QtGui.QPixmap("icons:help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionHelp.setIcon(icon11)
+        icon10 = QtGui.QIcon()
+        icon10.addPixmap(QtGui.QPixmap("icons:help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionHelp.setIcon(icon10)
         self.actionHelp.setObjectName("actionHelp")
         self.actionStart_hamlib_TB = QtGui.QAction(parent=MainWindow)
         self.actionStart_hamlib_TB.setCheckable(True)
-        icon12 = QtGui.QIcon()
-        icon12.addPixmap(QtGui.QPixmap("icons:player_play.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        icon12.addPixmap(QtGui.QPixmap("icons:player_stop.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.On)
-        self.actionStart_hamlib_TB.setIcon(icon12)
+        icon11 = QtGui.QIcon()
+        icon11.addPixmap(QtGui.QPixmap("icons:player_play.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        icon11.addPixmap(QtGui.QPixmap("icons:player_stop.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.On)
+        self.actionStart_hamlib_TB.setIcon(icon11)
         self.actionStart_hamlib_TB.setObjectName("actionStart_hamlib_TB")
         self.actionWatch_file_for_QSOs = QtGui.QAction(parent=MainWindow)
         self.actionWatch_file_for_QSOs.setCheckable(True)
-        icon13 = QtGui.QIcon()
-        icon13.addPixmap(QtGui.QPixmap("icons:watch.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionWatch_file_for_QSOs.setIcon(icon13)
+        icon12 = QtGui.QIcon()
+        icon12.addPixmap(QtGui.QPixmap("icons:watch.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionWatch_file_for_QSOs.setIcon(icon12)
         self.actionWatch_file_for_QSOs.setObjectName("actionWatch_file_for_QSOs")
         self.actionWatch_file_for_QSOs_TB = QtGui.QAction(parent=MainWindow)
         self.actionWatch_file_for_QSOs_TB.setCheckable(True)
-        self.actionWatch_file_for_QSOs_TB.setIcon(icon13)
+        self.actionWatch_file_for_QSOs_TB.setIcon(icon12)
         self.actionWatch_file_for_QSOs_TB.setObjectName("actionWatch_file_for_QSOs_TB")
         self.actionShow_log = QtGui.QAction(parent=MainWindow)
-        icon14 = QtGui.QIcon()
-        icon14.addPixmap(QtGui.QPixmap("icons:file_doc.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionShow_log.setIcon(icon14)
+        icon13 = QtGui.QIcon()
+        icon13.addPixmap(QtGui.QPixmap("icons:file_doc.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionShow_log.setIcon(icon13)
         self.actionShow_log.setObjectName("actionShow_log")
         self.actionUpload_logs_to_LoTW = QtGui.QAction(parent=MainWindow)
-        icon15 = QtGui.QIcon()
-        icon15.addPixmap(QtGui.QPixmap("icons:upload_lotw.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionUpload_logs_to_LoTW.setIcon(icon15)
+        icon14 = QtGui.QIcon()
+        icon14.addPixmap(QtGui.QPixmap("icons:upload_lotw.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionUpload_logs_to_LoTW.setIcon(icon14)
         self.actionUpload_logs_to_LoTW.setObjectName("actionUpload_logs_to_LoTW")
         self.menuFile.addAction(self.actionSelect_DB)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionExport)
         self.menuFile.addAction(self.actionImport)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionSettings)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionExit)
         self.menuEdit.addAction(self.actionLog_QSO)
-        self.menuEdit.addAction(self.actionLog_multi_QSOs)
         self.menuEdit.addSeparator()
         self.menuEdit.addAction(self.actionDelete_log_entry)
         self.menuEdit.addAction(self.actionChange_log_entry)
         self.menuEdit.addSeparator()
         self.menuEdit.addAction(self.actionWatch_file_for_QSOs)
         self.menuEdit.addSeparator()
         self.menuEdit.addAction(self.actionUpload_logs_to_LoTW)
@@ -181,75 +191,76 @@
         self.menuHelp.addSeparator()
         self.menuHelp.addAction(self.actionAbout)
         self.menuHelp.addAction(self.actionAbout_Qt)
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuEdit.menuAction())
         self.menubar.addAction(self.menuHelp.menuAction())
         self.toolBar.addAction(self.actionSelect_DB_TB)
+        self.toolBar.addAction(self.actionImport_TB)
+        self.toolBar.addAction(self.actionExport_TB)
         self.toolBar.addAction(self.actionSettings_TB)
-        self.toolBar.addAction(self.actionStart_hamlib_TB)
         self.toolBar.addSeparator()
+        self.toolBar.addAction(self.actionStart_hamlib_TB)
         self.toolBar.addAction(self.actionLog_QSO_TB)
-        self.toolBar.addAction(self.actionLog_multi_QSOs_TB)
-        self.toolBar.addSeparator()
         self.toolBar.addAction(self.actionWatch_file_for_QSOs_TB)
 
         self.retranslateUi(MainWindow)
         self.actionAbout.triggered.connect(MainWindow.showAbout) # type: ignore
         self.actionAbout_Qt.triggered.connect(MainWindow.showAboutQt) # type: ignore
         self.actionLog_QSO.triggered.connect(MainWindow.logQSO) # type: ignore
         self.actionLog_QSO_TB.triggered.connect(MainWindow.logQSO) # type: ignore
         self.actionExit.triggered.connect(MainWindow.close) # type: ignore
         self.actionSelect_DB.triggered.connect(MainWindow.selectDB) # type: ignore
         self.actionDelete_log_entry.triggered.connect(MainWindow.deleteQSO) # type: ignore
         self.actionChange_log_entry.triggered.connect(MainWindow.changeQSO) # type: ignore
         self.actionSettings.triggered.connect(MainWindow.showSettings) # type: ignore
         self.actionSettings_TB.triggered.connect(MainWindow.showSettings) # type: ignore
         self.actionExport.triggered.connect(MainWindow.export) # type: ignore
-        self.actionLog_multi_QSOs.triggered.connect(MainWindow.logMultiQSOs) # type: ignore
-        self.actionLog_multi_QSOs_TB.triggered.connect(MainWindow.logMultiQSOs) # type: ignore
+        self.actionExport_TB.triggered.connect(MainWindow.export) # type: ignore
         self.QSOTableView.doubleClicked['QModelIndex'].connect(MainWindow.changeQSO) # type: ignore
         self.actionHelp.triggered.connect(MainWindow.showHelp) # type: ignore
         self.actionImport.triggered.connect(MainWindow.logImport) # type: ignore
+        self.actionImport_TB.triggered.connect(MainWindow.logImport) # type: ignore
         self.actionStart_hamlib_TB.triggered['bool'].connect(MainWindow.ctrlHamlib) # type: ignore
         self.actionSelect_DB_TB.triggered.connect(MainWindow.selectDB) # type: ignore
         self.actionWatch_file_for_QSOs.triggered['bool'].connect(MainWindow.ctrlWatching) # type: ignore
         self.actionWatch_file_for_QSOs_TB.triggered['bool'].connect(MainWindow.ctrlWatching) # type: ignore
         self.actionShow_log.triggered.connect(self.logDockWidget.show) # type: ignore
         self.actionUpload_logs_to_LoTW.triggered.connect(MainWindow.lotwUpload) # type: ignore
+        self.QSOTableView.clicked['QModelIndex'].connect(MainWindow.clearQSOForm) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "DragonLog"))
         self.menuFile.setTitle(_translate("MainWindow", "File"))
         self.menuEdit.setTitle(_translate("MainWindow", "Edit"))
         self.menuHelp.setTitle(_translate("MainWindow", "Help"))
         self.toolBar.setWindowTitle(_translate("MainWindow", "Toolbar"))
         self.logDockWidget.setWindowTitle(_translate("MainWindow", "Application Log"))
+        self.qsoDockWidget.setWindowTitle(_translate("MainWindow", "QSO Form"))
         self.actionLog_QSO.setText(_translate("MainWindow", "Log QSO..."))
         self.actionLog_QSO.setShortcut(_translate("MainWindow", "Ctrl+L"))
         self.actionLog_QSO_TB.setText(_translate("MainWindow", "Log QSO..."))
         self.actionSelect_DB.setText(_translate("MainWindow", "Select database..."))
         self.actionSelect_DB_TB.setText(_translate("MainWindow", "Select database..."))
         self.actionExit.setText(_translate("MainWindow", "Exit"))
         self.actionExit.setShortcut(_translate("MainWindow", "Ctrl+Q"))
         self.actionExport.setText(_translate("MainWindow", "Export..."))
         self.actionImport.setText(_translate("MainWindow", "Import..."))
+        self.actionExport_TB.setText(_translate("MainWindow", "Export"))
+        self.actionImport_TB.setText(_translate("MainWindow", "Import"))
         self.actionAbout.setText(_translate("MainWindow", "About"))
         self.actionAbout_Qt.setText(_translate("MainWindow", "About Qt"))
         self.actionDelete_log_entry.setText(_translate("MainWindow", "Delete log entry"))
         self.actionDelete_log_entry.setShortcut(_translate("MainWindow", "Ctrl+X"))
         self.actionChange_log_entry.setText(_translate("MainWindow", "Change log entry..."))
         self.actionChange_log_entry.setShortcut(_translate("MainWindow", "Ctrl+E"))
         self.actionSettings.setText(_translate("MainWindow", "Settings"))
         self.actionSettings_TB.setText(_translate("MainWindow", "Settings"))
-        self.actionLog_multi_QSOs.setText(_translate("MainWindow", "Log multi QSOs..."))
-        self.actionLog_multi_QSOs.setShortcut(_translate("MainWindow", "Ctrl+Shift+L"))
-        self.actionLog_multi_QSOs_TB.setText(_translate("MainWindow", "Log multi QSOs..."))
         self.actionHelp.setText(_translate("MainWindow", "Help"))
         self.actionStart_hamlib_TB.setText(_translate("MainWindow", "Start hamlib"))
         self.actionWatch_file_for_QSOs.setText(_translate("MainWindow", "Watch file for QSOs..."))
         self.actionWatch_file_for_QSOs.setShortcut(_translate("MainWindow", "Ctrl+W"))
         self.actionWatch_file_for_QSOs_TB.setText(_translate("MainWindow", "Watch file for QSOs..."))
         self.actionShow_log.setText(_translate("MainWindow", "Show log"))
         self.actionUpload_logs_to_LoTW.setText(_translate("MainWindow", "Upload logs to LoTW..."))
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_QSOForm.py` & `DragonLog-1.0/dragonlog/DragonLog_QSOForm.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,53 +14,63 @@
                                  MissingADIFFieldException, LoginException, CallsignNotFoundException)
 from .DragonLog_eQSL import (EQSL, EQSLADIFFieldException, EQSLLoginException,
                              EQSLRequestException, EQSLUserCallMatchException, EQSLQSODuplicateException)
 from .DragonLog_LoTW import (LoTW, LoTWRequestException, LoTWCommunicationException,
                              LoTWLoginException, LoTWNoRecordException)
 
 
-class QSOForm(QtWidgets.QDialog, DragonLog_QSOForm_ui.Ui_QSOFormDialog):
-    def __init__(self, parent, bands: dict, modes: dict, settings: QtCore.QSettings, settings_form: Settings,
-                 cb_channels: dict, hamlib_error: QtWidgets.QLabel, logger: Logger):
+class QSOForm(QtWidgets.QDialog, DragonLog_QSOForm_ui.Ui_QSOForm):
+    def __init__(self, parent, dragonlog, bands: dict, modes: dict, prop: dict, settings: QtCore.QSettings,
+                 settings_form: Settings, cb_channels: dict, hamlib_error: QtWidgets.QLabel, logger: Logger):
         super().__init__(parent)
+        self.dragonlog = dragonlog
         self.setupUi(self)
 
         self.log = logging.getLogger('QSOForm')
         self.log.addHandler(logger)
         self.log.setLevel(logger.loglevel)
         self.logger = logger
         self.log.debug('Initialising...')
 
-        self.default_title = self.windowTitle()
         self.lastpos = None
         self.bands = bands
         self.modes = modes
+        self.prop = prop
+        self.prop_trans = dict(zip(prop.values(), prop.keys()))
         self.settings = settings
         self.settings_form = settings_form
+        self.qso_id = None
 
         self.cb_channels = cb_channels
         self.channelComboBox.insertItems(0, ['-'] + list(cb_channels.keys()))
 
         self.bandComboBox.insertItems(0, bands.keys())
 
+        self.propComboBox.insertItems(0, self.prop.values())
+
         self.stationChanged(True)
         self.identityChanged(True)
 
         self.hamlib_error = hamlib_error
-        self.rig_modes = {'USB': 'SSB',
-                          'LSB': 'SSB',
-                          'CW': 'CW',
-                          'CWR': 'CW',
-                          'RTTY': 'RTTY',
-                          'RTTYR': 'RTTY',
-                          'AM': 'AM',
-                          'FM': 'FM',
-                          'WFM': 'FM',
+        self.rig_modes = {'USB': ('SSB', 'USB'),
+                          'LSB': ('SSB', 'LSB'),
+                          'CW': ('CW', ''),
+                          'CWR': ('CW', ''),
+                          'RTTY': ('RTTY', ''),
+                          'RTTYR': ('RTTY', ''),
+                          'AM': ('AM', ''),
+                          'FM': ('FM', ''),
+                          'WFM': ('FM', ''),
+                          'PKTUSB': ('SSB', 'USB'),
+                          'PKTLSB': ('SSB', 'LSB'),
                           }
         self.__last_mode__ = ''
+        self.__last_band__ = ''
+        self.__last_freq__ = 0.0
+        self.__last_pwr__ = ''
 
         self.__change_mode__ = False
 
         self.refreshTimer = QtCore.QTimer(self)
         self.refreshTimer.timeout.connect(self.refreshRigData)
 
         self.timeTimer = QtCore.QTimer(self)
@@ -82,49 +92,62 @@
         self.palette_worked.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
                                      QtGui.QColor(204, 204, 255))
 
         self.worked_dialog: QtWidgets.QListWidget = None
         self._create_worked_dlg_()
 
         self.callbook = CallBook(CallBookType.HamQTH,
-                                 f'{self.parent().programName}-{self.parent().programVersion}',
+                                 f'{self.dragonlog.programName}-{self.dragonlog.programVersion}',
                                  self.logger)
-        self.eqsl = EQSL(self.parent().programName, self.logger)
+        self.eqsl = EQSL(self.dragonlog.programName, self.logger)
         self.eqsl_url = ''
 
         self.lotw = LoTW(self.logger)
 
         view_only_widgets = (
             self.qslAccBureauCheckBox,
             self.qslAccDirectCheckBox,
             self.qslAcceQSLCheckBox,
             self.qslAccLoTWCheckBox,
             self.eqslSentCheckBox,
             self.eqslRcvdCheckBox,
+            self.lotwSentCheckBox,
+            self.lotwRcvdCheckBox,
             self.hamQTHuplRadioButton,
             self.hamQTHmodRadioButton,
         )
 
         for w in view_only_widgets:
             w.setAttribute(QtCore.Qt.WidgetAttribute.WA_TransparentForMouseEvents)
             w.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
 
+        self.clear()
+
+    def startTimers(self, start: bool):
+        if start:
+            self.refreshTimer.start(500)
+            self.timeTimer.start(1000)
+        else:
+            self.refreshTimer.stop()
+            self.timeTimer.stop()
+
     def _create_worked_dlg_(self):
         self.worked_dialog = QtWidgets.QListWidget(self)
         self.worked_dialog.setMinimumHeight(100)
         self.worked_dialog.setSelectionMode(QtWidgets.QAbstractItemView.SelectionMode.NoSelection)
         self.worked_dialog.setSortingEnabled(True)
+        self.worked_dialog.hide()
 
     def setWorkedBefore(self, worked: list = None):
         self.worked_dialog.clear()
         if worked:
             self.worked_dialog.addItems(worked)
             call_edit_pos = self.callSignLineEdit.pos()
-            call_edit_pos.setX(call_edit_pos.x())
-            call_edit_pos.setY(call_edit_pos.y() + self.callSignLineEdit.height())
+            call_edit_pos.setX(call_edit_pos.x() + 15)
+            call_edit_pos.setY(call_edit_pos.y() + self.callSignLineEdit.height() + 40)
             self.worked_dialog.move(call_edit_pos)
             self.worked_dialog.show()
         else:
             self.worked_dialog.hide()
 
     def refreshTime(self):
         if self.autoDateCheckBox.isChecked():
@@ -135,104 +158,132 @@
     def setStartTimeNow(self):
         dt = QtCore.QDateTime.currentDateTimeUtc()
         self.dateOnEdit.setDate(dt.date())
         self.timeOnEdit.setTime(dt.time())
 
     # noinspection PyBroadException
     def refreshRigData(self):
-        if self.settings_form.isRigctldActive():
-            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-                s.connect(('127.0.0.1', 4532))
-                s.settimeout(1)
-                try:
-                    # Get frequency
-                    s.sendall(b'\\get_freq\n')
-                    freq_s = s.recv(1024).decode('utf-8').strip()
-                    if freq_s.startswith('RPRT'):
-                        self.hamlib_error.setText(self.tr('Error') + ':' + freq_s.split()[1])
-                        self.log.error(f'rigctld error get_freq: {freq_s.split()[1]}')
-                        return
-
+        if self.settings_form.isRigctldActive() and not self.__change_mode__:
+            try:
+                with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+                    s.connect(('127.0.0.1', 4532))
+                    s.settimeout(1)
                     try:
-                        freq = float(freq_s) / 1000
-                        for b in self.bands:
-                            if freq < self.bands[b][1]:
-                                if freq > self.bands[b][0]:
-                                    self.bandComboBox.setCurrentText(b)
-                                    self.freqDoubleSpinBox.setValue(freq)
-                                break
-                    except Exception:
-                        pass
-
-                    # Get mode
-                    s.sendall(b'\\get_mode\n')
-                    mode_s = s.recv(1024).decode('utf-8').strip()
-                    if mode_s.startswith('RPRT'):
-                        self.hamlib_error.setText(self.tr('Error') + ':' + mode_s.split()[1])
-                        self.log.error(f'rigctld error get_mode: {mode_s.split()[1]}')
-                        return
-
-                    try:
-                        mode, passband = [v.strip() for v in mode_s.split('\n')]
-                        if mode in self.rig_modes and mode != self.__last_mode__:
-                            self.modeComboBox.setCurrentText(self.rig_modes[mode])
-                            self.__last_mode__ = mode
-                    except Exception:
-                        pass
-
-                    # Get power
-                    if 'get level' in self.settings_form.rig_caps and 'get power2mw' in self.settings_form.rig_caps:
-                        # Get power level
-                        s.sendall(b'\\get_level RFPOWER\n')
-                        pwrlvl_s = s.recv(1024).decode('utf-8').strip()
-                        if pwrlvl_s.startswith('RPRT'):
-                            self.hamlib_error.setText(self.tr('Error') + ':' + pwrlvl_s.split()[1])
-                            self.log.error(f'rigctld error get_level: {pwrlvl_s.split()[1]}')
+                        # Get frequency
+                        s.sendall(b'\\get_freq\n')
+                        freq_s = s.recv(1024).decode('utf-8').strip()
+                        if freq_s.startswith('RPRT'):
+                            self.hamlib_error.setText(self.tr('Error') + ':' + freq_s.split()[1])
+                            self.log.error(f'rigctld error get_freq: {freq_s.split()[1]}')
                             return
 
-                        # Convert level to W
-                        s.sendall(f'\\power2mW {pwrlvl_s} {freq_s} {mode}\n'.encode())
-                        pwr_s = s.recv(1024).decode('utf-8').strip()
-                        if pwr_s.startswith('RPRT'):
-                            self.hamlib_error.setText(self.tr('Error') + ':' + pwr_s.split()[1])
-                            self.log.error(f'rigctld error power2mW: {pwr_s.split()[1]}')
+                        try:
+                            freq = float(freq_s) / 1000
+                            if freq != self.__last_freq__:
+                                for b in self.bands:
+                                    if freq < self.bands[b][1]:
+                                        if freq > self.bands[b][0]:
+                                            if b != self.__last_band__:
+                                                self.bandComboBox.setCurrentText(b)
+                                                self.log.info(f'CAT changed band to {b}')
+                                                self.__last_band__ = b
+                                                self.__last_mode__ = ''
+                                        break
+                                self.freqDoubleSpinBox.setValue(freq)
+                                self.__last_freq__ = freq
+                        except Exception:
+                            pass
+
+                        # Get mode
+                        s.sendall(b'\\get_mode\n')
+                        mode_s = s.recv(1024).decode('utf-8').strip()
+                        if mode_s.startswith('RPRT'):
+                            self.hamlib_error.setText(self.tr('Error') + ':' + mode_s.split()[1])
+                            self.log.error(f'rigctld error get_mode: {mode_s.split()[1]}')
                             return
 
                         try:
-                            pwr = int(int(pwr_s) / 1000 + .9)
-                            self.powerSpinBox.setValue(pwr)
+                            mode, passband = [v.strip() for v in mode_s.split('\n')]
+                            if mode in self.rig_modes and mode != self.__last_mode__:
+                                self.modeComboBox.setCurrentText(self.rig_modes[mode][0])
+                                self.log.info(f'CAT changed mode to {self.rig_modes[mode][0]}')
+                                if self.rig_modes[mode][1]:
+                                    self.submodeComboBox.setCurrentText(self.rig_modes[mode][1])
+                                self.__last_mode__ = mode
                         except Exception:
                             pass
-                    else:
-                        self.powerSpinBox.setValue(0)
-                except socket.timeout:
-                    self.hamlib_error.setText(self.tr('rigctld timeout'))
-                    self.log.error('rigctld error: timeout')
-                    self.refreshTimer.stop()
-        else:
-            self.refreshTimer.stop()
+
+                        # Get power
+                        if 'get level' in self.settings_form.rig_caps and 'get power2mw' in self.settings_form.rig_caps:
+                            # Get power level
+                            s.sendall(b'\\get_level RFPOWER\n')
+                            pwrlvl_s = s.recv(1024).decode('utf-8').strip()
+                            if pwrlvl_s.startswith('RPRT'):
+                                self.hamlib_error.setText(self.tr('Error') + ':' + pwrlvl_s.split()[1])
+                                self.log.error(f'rigctld error get_level: {pwrlvl_s.split()[1]}')
+                                return
+
+                            if pwrlvl_s != self.__last_pwr__:
+                                self.__last_pwr__ = pwrlvl_s
+                                # Convert level to W
+                                s.sendall(f'\\power2mW {pwrlvl_s} {freq_s} {mode}\n'.encode())
+                                pwr_s = s.recv(1024).decode('utf-8').strip()
+                                if pwr_s.startswith('RPRT'):
+                                    self.hamlib_error.setText(self.tr('Error') + ':' + pwr_s.split()[1])
+                                    self.log.error(f'rigctld error power2mW: {pwr_s.split()[1]}')
+                                    return
+
+                                try:
+                                    pwr = int(int(pwr_s) / 1000 + .9)
+                                    self.powerSpinBox.setValue(pwr)
+                                    self.log.info(f'CAT changed power to {pwr} W')
+                                except Exception:
+                                    pass
+                    except socket.timeout:
+                        self.hamlib_error.setText(self.tr('rigctld timeout'))
+                        self.log.error('rigctld error: timeout')
+            except ConnectionRefusedError:
+                self.log.error('Could not connect to rigctld')
+                self.refreshTimer.stop()
 
     def clear(self):
+        self.qso_id = None
         self.callSignLineEdit.clear()
         self.nameLineEdit.clear()
         self.QTHLineEdit.clear()
         self.locatorLineEdit.clear()
         self.RSTSentLineEdit.setText('59')
         self.RSTRcvdLineEdit.setText('59')
         self.remarksTextEdit.clear()
         self.powerSpinBox.setValue(0)
 
+        self.callSignChanged('')
+        self.locatorChanged('')
+        self.ownCallSignChanged(self.ownCallSignLineEdit.text())
+        self.ownLocatorChanged(self.ownLocatorLineEdit.text())
+        self.rstSentChanged(self.RSTSentLineEdit.text())
+        self.rstRcvdChanged(self.RSTRcvdLineEdit.text())
+
+        dt = QtCore.QDateTime.currentDateTimeUtc()
+        self.dateEdit.setDate(dt.date())
+        self.dateOnEdit.setDate(dt.date())
+        self.timeEdit.setTime(dt.time())
+        self.timeOnEdit.setTime(dt.time())
+
         if bool(self.settings.value('station_cb/cb_by_default', 0)):
             self.bandComboBox.setCurrentText('11m')
 
         if self.bandComboBox.currentIndex() < 0:
             self.bandComboBox.setCurrentIndex(0)
         if self.modeComboBox.currentIndex() < 0:
             self.modeComboBox.setCurrentIndex(0)
 
+        self.submodeComboBox.setCurrentIndex(-1)
+        self.propComboBox.setCurrentIndex(-1)
+
         self.qslBurDirGroupBox.setChecked(False)
         self.qslViaLineEdit.clear()
         self.qslBureauRadioButton.setChecked(False)
         self.qslDirectRadioButton.setChecked(False)
         self.qslAccBureauCheckBox.setChecked(False)
         self.qslAccDirectCheckBox.setChecked(False)
         self.qslAcceQSLCheckBox.setChecked(False)
@@ -243,29 +294,33 @@
 
         self.eqslSentCheckBox.setChecked(False)
         self.eqslRcvdCheckBox.setChecked(False)
         self.eqslLinkLabel.setEnabled(False)
         self.eqslLinkLabel.setText(self.tr('Link to eQSL Card'))
         self.eqslDownloadPushButton.setEnabled(False)
 
+        self.lotwGroupBox.setChecked(False)
+        self.lotwSentCheckBox.setChecked(False)
+        self.lotwRcvdCheckBox.setChecked(False)
+        self.lotwInboxPushButton.setEnabled(False)
+
         self.hamQTHGroupBox.setChecked(False)
         self.hamQTHmodRadioButton.setChecked(True)  # Just not check upload
 
         self.toolBox.setCurrentIndex(0)
 
     def reset(self):
         self.autoDateCheckBox.setEnabled(True)
         self.autoDateCheckBox.setChecked(True)
         self.stationGroupBox.setChecked(True)
         self.identityGroupBox.setChecked(True)
 
-        self.setWindowTitle(self.default_title)
-
     def setChangeMode(self, activate=True):
         self.__change_mode__ = activate
+        self.startTimers(not activate)
 
         if activate:
             self.stationGroupBox.setChecked(False)
             self.stationGroupBox.setCheckable(False)
             self.stationGroupBox.setTitle(self.tr('Station'))
             self.identityGroupBox.setChecked(False)
             self.identityGroupBox.setCheckable(False)
@@ -288,14 +343,15 @@
         self.freqDoubleSpinBox.setMinimum(self.bands[band][0] - self.bands[band][2])
         self.freqDoubleSpinBox.setValue(self.bands[band][0] - self.bands[band][2])
         self.freqDoubleSpinBox.setMaximum(self.bands[band][1])
         self.freqDoubleSpinBox.setSingleStep(self.bands[band][2])
 
         self.modeComboBox.clear()
         if band == '11m':
+            self.modeComboBox.insertItems(0, self.modes['CB'].keys())
             self.powerSpinBox.setMaximum(12)
             self.channelComboBox.setVisible(True)
             self.channelLabel.setVisible(True)
             self.freqDoubleSpinBox.setEnabled(False)
             self.searchCallbookPushButton.setEnabled(False)
             self.uploadPushButton.setEnabled(False)
             self.qslPage.setEnabled(False)
@@ -322,14 +378,28 @@
             if self.stationGroupBox.isChecked():
                 self.radioLineEdit.setText(self.settings.value('station/radio', ''))
                 self.antennaLineEdit.setText(self.settings.value('station/antenna', ''))
 
             if self.identityGroupBox.isChecked():
                 self.ownCallSignLineEdit.setText(self.settings.value('station/callSign', ''))
 
+    def modeChanged(self, mode: str):
+        self.submodeComboBox.clear()
+        self.submodeComboBox.setEnabled(True)
+        if self.bandComboBox.currentText() == '11m':
+            if mode in self.modes['CB'] and self.modes['CB'][mode]:
+                self.submodeComboBox.insertItems(0, [''] + self.modes['CB'][mode])
+            else:
+                self.submodeComboBox.setEnabled(False)
+        else:
+            if mode in self.modes['AFU'] and  self.modes['AFU'][mode]:
+                self.submodeComboBox.insertItems(0, [''] + self.modes['AFU'][mode])
+            else:
+                self.submodeComboBox.setEnabled(False)
+
     def stationChanged(self, checked):
         if checked:
             self.ownQTHLineEdit.setText(self.settings.value('station/QTH', ''))
             self.ownLocatorLineEdit.setText(self.settings.value('station/locator', ''))
 
             if self.bandComboBox.currentText() == '11m':
                 self.radioLineEdit.setText(self.settings.value('station_cb/radio', ''))
@@ -373,15 +443,15 @@
             self.RSTSentLineEdit.setPalette(self.palette_faulty)
 
     def callSignChanged(self, txt):
         self.setWorkedBefore()
         if not txt:
             self.callSignLineEdit.setPalette(self.palette_empty)
         elif check_format(REGEX_CALL, txt):
-            worked = self.parent().workedBefore(check_call(txt)[1])
+            worked = self.dragonlog.workedBefore(check_call(txt)[1])
             if not self.__change_mode__ and worked:
                 self.setWorkedBefore(worked)
                 self.callSignLineEdit.setPalette(self.palette_worked)
             else:
                 self.callSignLineEdit.setPalette(self.palette_ok)
         elif self.bandComboBox.currentText() == '11m':
             self.callSignLineEdit.setPalette(self.palette_ok)
@@ -441,14 +511,18 @@
             else:
                 date_time_off = self.dateEdit.text() + ' ' + self.timeEdit.text()
         else:
             date_time_off = self.dateEdit.text() + ' ' + self.timeEdit.text()
 
         band = self.bandComboBox.currentText()
 
+        prop = ''
+        if self.propComboBox.currentText():
+            prop = self.prop_trans[self.propComboBox.currentText()]
+
         qsl_via = ''
         qsl_path = ''
         qsl_msg = ''
         qsl_sent = 'N'
         qsl_rcvd = 'N'
         eqsl_sent = 'N'
         eqsl_rcvd = 'N'
@@ -486,18 +560,20 @@
             self.nameLineEdit.text(),
             self.QTHLineEdit.text(),
             self.locatorLineEdit.text(),
             self.RSTSentLineEdit.text(),
             self.RSTRcvdLineEdit.text(),
             band,
             self.modeComboBox.currentText(),
+            self.submodeComboBox.currentText(),
             self.freqDoubleSpinBox.value() if self.freqDoubleSpinBox.value() >= self.bands[band][
                 0] else '',
             self.channelComboBox.currentText() if band == '11m' else '-',
             self.powerSpinBox.value() if self.powerSpinBox.value() > 0 else '',
+            prop,
             self.ownNameLineEdit.text(),
             self.ownQTHLineEdit.text(),
             self.ownLocatorLineEdit.text(),
             self.radioLineEdit.text(),
             self.antennaLineEdit.text(),
             self.remarksTextEdit.toPlainText().strip(),
             self.commentsTextEdit.toPlainText().strip(),
@@ -514,14 +590,15 @@
             hamqth_state,
         )
 
     @values.setter
     def values(self, values: dict):
         """Set all form values"""
 
+        self.qso_id = values['id']
         date, time = values['date_time'].split()
         self.dateOnEdit.setDate(QtCore.QDate.fromString(date, 'yyyy-MM-dd'))
         self.timeOnEdit.setTime(QtCore.QTime.fromString(time))
 
         if values['date_time_off']:
             date_off, time_off = values['date_time_off'].split()
         else:
@@ -533,18 +610,27 @@
         self.callSignLineEdit.setText(values['call_sign'])
         self.nameLineEdit.setText(values['name'])
         self.QTHLineEdit.setText(values['qth'])
         self.locatorLineEdit.setText(values['locator'])
         self.RSTSentLineEdit.setText(values['rst_sent'])
         self.RSTRcvdLineEdit.setText(values['rst_rcvd'])
 
+        self.callSignChanged(self.callSignLineEdit.text())
+        self.locatorChanged(self.locatorLineEdit.text())
+        self.ownCallSignChanged(self.ownCallSignLineEdit.text())
+        self.ownLocatorChanged(self.ownLocatorLineEdit.text())
+        self.rstSentChanged(self.RSTSentLineEdit.text())
+        self.rstRcvdChanged(self.RSTRcvdLineEdit.text())
+
         band = values['band']
         self.bandComboBox.setCurrentText(band)
 
         self.modeComboBox.setCurrentText(values['mode'])
+        if values['submode']:
+            self.submodeComboBox.setCurrentText(values['submode'])
 
         try:
             freq = float(values['freq'])
         except ValueError:
             freq = self.bands[band][0] - self.bands[band][2]
         self.freqDoubleSpinBox.setValue(freq)
 
@@ -554,14 +640,18 @@
             self.channelComboBox.setCurrentText(str(channel) if channel else '-')
 
         try:
             power = int(values['power'])
         except ValueError:
             power = 0
         self.powerSpinBox.setValue(power)
+
+        if values['propagation']:
+            self.propComboBox.setCurrentText(self.prop[values['propagation']])
+
         self.ownNameLineEdit.setText(values['own_name'])
         self.ownQTHLineEdit.setText(values['own_qth'])
         self.ownLocatorLineEdit.setText(values['own_locator'])
         self.radioLineEdit.setText(values['radio'])
         self.antennaLineEdit.setText(values['antenna'])
         self.remarksTextEdit.setText(values['remarks'])
         self.commentsTextEdit.setText(values['comments'])
@@ -587,14 +677,15 @@
                     self.eqslLinkLabel.setEnabled(True)
                     self.eqslDownloadPushButton.setEnabled(True)
 
         if values['lotw_sent'] in ('R', 'Y') or values['lotw_rcvd'] in ('R', 'Y'):
             self.lotwGroupBox.setChecked(True)
             self.lotwSentCheckBox.setChecked(values['lotw_sent'] == 'Y')
             self.lotwRcvdCheckBox.setChecked(values['lotw_rcvd'] == 'Y')
+            self.lotwInboxPushButton.setEnabled(True)
 
         match values['hamqth']:
             case 'Y':
                 self.hamQTHGroupBox.setChecked(True)
                 self.hamQTHuplRadioButton.setChecked(True)
             case 'M':
                 self.hamQTHGroupBox.setChecked(True)
@@ -647,26 +738,31 @@
         except Exception as exc:
             QtWidgets.QMessageBox.warning(self, self.tr('Callbook search error'),
                                           self.tr('During callbook search an error occured') + f':\n{exc}')
 
     def saveLog(self):
         self.hamQTHmodRadioButton.setChecked(True)
 
-        # finally accept dialog anyway
-        self.accept()
+        if self.__change_mode__:
+            self.dragonlog.updateQSO(self.qso_id)
+        else:
+            self.dragonlog.fetchQSO()
+
+        self.toolBox.setCurrentIndex(0)
+        self.clear()
 
     def uploadLog(self):
         if self.hamQTHGroupBox.isChecked() or self.eqslGroupBox.isChecked():
             record = self._build_record_()
 
             adif_doc = {'HEADER':
                 {
                     'ADIF_VER': '3.1.4',
-                    'PROGRAMID': self.parent().programName,
-                    'PROGRAMVERSION': self.parent().programVersion,
+                    'PROGRAMID': self.dragonlog.programName,
+                    'PROGRAMVERSION': self.dragonlog.programVersion,
                     'CREATED_TIMESTAMP': QtCore.QDateTime.currentDateTimeUtc().toString(
                         'yyyyMMdd HHmmss')
                 },
                 'RECORDS': [record]}
 
             if self.hamQTHGroupBox.isChecked() and not self.hamQTHuplRadioButton.isChecked():
                 try:
@@ -706,52 +802,57 @@
                     QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
                                                   self.tr('User call does not match') + ': ' + self.settings.value(
                                                       'eqsl/username', ''))
                 except EQSLRequestException as exc:
                     QtWidgets.QMessageBox.information(self, self.tr('Upload eQSL error'),
                                                       self.tr('Error on upload') + f':\n"{exc.args[0]}"')
 
-        # finally accept dialog anyway
-        self.accept()
+        if self.__change_mode__:
+            self.dragonlog.updateQSO(self.qso_id)
+        else:
+            self.dragonlog.fetchQSO()
+
+        self.toolBox.setCurrentIndex(0)
+        self.clear()
 
     def _build_record_(self):
         record = {
             'QSO_DATE': self.dateOnEdit.text().replace('-', ''),
             'TIME_ON': self.timeOnEdit.text().replace(':', ''),
             'TIME_OFF': self.timeEdit.text().replace(':', ''),
             'BAND': self.bandComboBox.currentText(),
             'MODE': self.modeComboBox.currentText(),
         }
         if self.ownCallSignLineEdit.text():
             record['STATION_CALLSIGN'] = self.ownCallSignLineEdit.text().upper()
         if self.callSignLineEdit.text():
             record['CALL'] = self.callSignLineEdit.text().upper()
         if self.nameLineEdit.text():
-            record['NAME'] = self.parent().replaceUmlautsLigatures(self.nameLineEdit.text())
+            record['NAME'] = self.dragonlog.replaceNonASCII(self.nameLineEdit.text())
         if self.QTHLineEdit.text():
-            record['QTH'] = self.parent().replaceUmlautsLigatures(self.QTHLineEdit.text())
+            record['QTH'] = self.dragonlog.replaceNonASCII(self.QTHLineEdit.text())
         if self.locatorLineEdit.text():
             record['GRIDSQUARE'] = self.locatorLineEdit.text()
         if self.RSTSentLineEdit.text():
             record['RST_SENT'] = self.RSTSentLineEdit.text()
         if self.RSTRcvdLineEdit.text():
             record['RST_RCVD'] = self.RSTRcvdLineEdit.text()
         if self.freqDoubleSpinBox.value() >= self.bands[self.bandComboBox.currentText()][0]:
             record['FREQ'] = f'{self.freqDoubleSpinBox.value() / 1000:0.3f}'
         if self.powerSpinBox.value() > 0:
             record['TX_PWR'] = self.powerSpinBox.value()
         if self.ownLocatorLineEdit.text():
             record['MY_GRIDSQUARE'] = self.ownLocatorLineEdit.text()
         if self.remarksTextEdit.toPlainText().strip() and not bool(
                 self.settings.value('imp_exp/own_notes_adif', 0)):
-            record['NOTES'] = self.parent().replaceUmlautsLigatures(self.remarksTextEdit.toPlainText().strip())
+            record['NOTES'] = self.dragonlog.replaceNonASCII(self.remarksTextEdit.toPlainText().strip())
         if self.commentsTextEdit.toPlainText().strip():
-            record['COMMENTS'] = self.parent().replaceUmlautsLigatures(self.commentsTextEdit.toPlainText().strip())
+            record['COMMENTS'] = self.dragonlog.replaceNonASCII(self.commentsTextEdit.toPlainText().strip())
         if self.qslMessageTextEdit.toPlainText().strip():
-            record['QSLMSG'] = self.parent().replaceUmlautsLigatures(self.qslMessageTextEdit.toPlainText().strip())
+            record['QSLMSG'] = self.dragonlog.replaceNonASCII(self.qslMessageTextEdit.toPlainText().strip())
 
         return record
 
     def eqslCheckInbox(self, only_url: bool = False):
         try:
             res = self.eqsl.check_inbox(self.settings.value('eqsl/username', ''),
                                         self.settings_form.eqslPassword(),
@@ -822,45 +923,20 @@
             rcvd = self.lotw.check_inbox(self.settings.value('lotw/username', ''),
                                          self.settings_form.lotwPassword(),
                                          self._build_record_())
 
             self.lotwRcvdCheckBox.setChecked(rcvd)
             self.lotwSentCheckBox.setChecked(True)
         except LoTWNoRecordException:
-            self.lotwSentCheckBox.setChecked(False)
             self.lotwRcvdCheckBox.setChecked(False)
+            QtWidgets.QMessageBox.information(self, self.tr('Check LoTW QSL'),
+                                              self.tr('No QSL available'))
         except LoTWCommunicationException:
             QtWidgets.QMessageBox.warning(self, self.tr('Check LoTW Inbox error'),
                                           self.tr('Server communication error'))
         except LoTWRequestException as exc:
             QtWidgets.QMessageBox.warning(self, self.tr('Check LoTW Inbox error'),
                                           self.tr('Bad request result') + f'\n{exc}')
         except LoTWLoginException as exc:
             QtWidgets.QMessageBox.warning(self, self.tr('Check LoTW Inbox error'),
                                           self.tr('Login failed for user') + ': ' + self.settings.value(
                                               'lotw/username', '') + f'\n{exc}')
-
-    def exec(self) -> int:
-        if self.lastpos:
-            self.move(self.lastpos)
-
-        self.callSignLineEdit.setFocus()
-
-        if self.settings_form.isRigctldActive():
-            self.refreshTimer.start(500)
-
-        self.callSignChanged(self.callSignLineEdit.text())
-        self.locatorChanged(self.locatorLineEdit.text())
-        self.rstSentChanged(self.RSTSentLineEdit.text())
-        self.rstRcvdChanged(self.RSTRcvdLineEdit.text())
-        self.ownCallSignChanged(self.ownCallSignLineEdit.text())
-        self.ownLocatorChanged(self.ownLocatorLineEdit.text())
-
-        self.timeTimer.start(1000)
-
-        return super().exec()
-
-    def hideEvent(self, e):
-        self.lastpos = self.pos()
-        self.refreshTimer.stop()
-        self.timeTimer.stop()
-        e.accept()
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_QSOForm_ui.py` & `DragonLog-1.0/dragonlog/DragonLog_QSOForm_ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,30 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_QSOFormDialog(object):
-    def setupUi(self, QSOFormDialog):
-        QSOFormDialog.setObjectName("QSOFormDialog")
-        QSOFormDialog.resize(575, 592)
-        self.verticalLayout = QtWidgets.QVBoxLayout(QSOFormDialog)
+class Ui_QSOForm(object):
+    def setupUi(self, QSOForm):
+        QSOForm.setObjectName("QSOForm")
+        QSOForm.resize(500, 600)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.MinimumExpanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(QSOForm.sizePolicy().hasHeightForWidth())
+        QSOForm.setSizePolicy(sizePolicy)
+        QSOForm.setMinimumSize(QtCore.QSize(500, 600))
+        self.verticalLayout = QtWidgets.QVBoxLayout(QSOForm)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.toolBox = QtWidgets.QToolBox(parent=QSOFormDialog)
+        self.toolBox = QtWidgets.QToolBox(parent=QSOForm)
         self.toolBox.setObjectName("toolBox")
         self.mainPage = QtWidgets.QWidget()
-        self.mainPage.setGeometry(QtCore.QRect(0, 0, 557, 482))
+        self.mainPage.setGeometry(QtCore.QRect(0, 0, 482, 490))
         self.mainPage.setObjectName("mainPage")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.mainPage)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.gridLayout_3 = QtWidgets.QGridLayout()
         self.gridLayout_3.setObjectName("gridLayout_3")
@@ -106,21 +112,30 @@
         self.freqDoubleSpinBox = QtWidgets.QDoubleSpinBox(parent=self.mainPage)
         self.freqDoubleSpinBox.setAccelerated(True)
         self.freqDoubleSpinBox.setDecimals(3)
         self.freqDoubleSpinBox.setMinimum(100.0)
         self.freqDoubleSpinBox.setMaximum(7500000000.0)
         self.freqDoubleSpinBox.setObjectName("freqDoubleSpinBox")
         self.horizontalLayout_8.addWidget(self.freqDoubleSpinBox)
-        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_8.addItem(spacerItem2)
+        self.verticalLayout_2.addLayout(self.horizontalLayout_8)
+        self.horizontalLayout_14 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_14.setObjectName("horizontalLayout_14")
         self.modeComboBox = QtWidgets.QComboBox(parent=self.mainPage)
         self.modeComboBox.setMinimumContentsLength(2)
         self.modeComboBox.setObjectName("modeComboBox")
-        self.horizontalLayout_8.addWidget(self.modeComboBox)
-        self.verticalLayout_2.addLayout(self.horizontalLayout_8)
+        self.horizontalLayout_14.addWidget(self.modeComboBox)
+        self.submodeComboBox = QtWidgets.QComboBox(parent=self.mainPage)
+        self.submodeComboBox.setObjectName("submodeComboBox")
+        self.horizontalLayout_14.addWidget(self.submodeComboBox)
+        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_14.addItem(spacerItem2)
+        self.propComboBox = QtWidgets.QComboBox(parent=self.mainPage)
+        self.propComboBox.setObjectName("propComboBox")
+        self.horizontalLayout_14.addWidget(self.propComboBox)
+        self.verticalLayout_2.addLayout(self.horizontalLayout_14)
         self.identityGroupBox = QtWidgets.QGroupBox(parent=self.mainPage)
         self.identityGroupBox.setCheckable(True)
         self.identityGroupBox.setObjectName("identityGroupBox")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.identityGroupBox)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.horizontalLayout_5 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_5.setObjectName("horizontalLayout_5")
@@ -208,26 +223,28 @@
         self.gridLayout.setColumnStretch(1, 1)
         self.gridLayout.setColumnStretch(2, 1)
         self.gridLayout.setColumnStretch(3, 2)
         self.verticalLayout_2.addLayout(self.gridLayout)
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
         self.commentsTextEdit = QtWidgets.QTextEdit(parent=self.mainPage)
+        self.commentsTextEdit.setAcceptRichText(False)
         self.commentsTextEdit.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByKeyboard|QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextBrowserInteraction|QtCore.Qt.TextInteractionFlag.TextEditable|QtCore.Qt.TextInteractionFlag.TextEditorInteraction|QtCore.Qt.TextInteractionFlag.TextSelectableByKeyboard|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.commentsTextEdit.setObjectName("commentsTextEdit")
         self.horizontalLayout_4.addWidget(self.commentsTextEdit)
         self.remarksTextEdit = QtWidgets.QTextEdit(parent=self.mainPage)
+        self.remarksTextEdit.setAcceptRichText(False)
         self.remarksTextEdit.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByKeyboard|QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextBrowserInteraction|QtCore.Qt.TextInteractionFlag.TextEditable|QtCore.Qt.TextInteractionFlag.TextEditorInteraction|QtCore.Qt.TextInteractionFlag.TextSelectableByKeyboard|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.remarksTextEdit.setObjectName("remarksTextEdit")
         self.horizontalLayout_4.addWidget(self.remarksTextEdit)
         self.verticalLayout_2.addLayout(self.horizontalLayout_4)
         self.verticalLayout_5.addLayout(self.verticalLayout_2)
         self.toolBox.addItem(self.mainPage, "")
         self.qslPage = QtWidgets.QWidget()
-        self.qslPage.setGeometry(QtCore.QRect(0, 0, 540, 484))
+        self.qslPage.setGeometry(QtCore.QRect(0, 0, 482, 490))
         self.qslPage.setObjectName("qslPage")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.qslPage)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.qslGroupBox = QtWidgets.QGroupBox(parent=self.qslPage)
         self.qslGroupBox.setObjectName("qslGroupBox")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.qslGroupBox)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
@@ -362,154 +379,182 @@
         self.verticalLayout_6.addItem(spacerItem11)
         self.toolBox.addItem(self.qslPage, "")
         self.verticalLayout.addWidget(self.toolBox)
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
         spacerItem12 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_2.addItem(spacerItem12)
-        self.uploadPushButton = QtWidgets.QPushButton(parent=QSOFormDialog)
+        self.uploadPushButton = QtWidgets.QPushButton(parent=QSOForm)
         self.uploadPushButton.setObjectName("uploadPushButton")
         self.horizontalLayout_2.addWidget(self.uploadPushButton)
-        self.savePushButton = QtWidgets.QPushButton(parent=QSOFormDialog)
+        self.savePushButton = QtWidgets.QPushButton(parent=QSOForm)
         self.savePushButton.setObjectName("savePushButton")
         self.horizontalLayout_2.addWidget(self.savePushButton)
-        self.cancelPushButton = QtWidgets.QPushButton(parent=QSOFormDialog)
+        self.cancelPushButton = QtWidgets.QPushButton(parent=QSOForm)
         self.cancelPushButton.setObjectName("cancelPushButton")
         self.horizontalLayout_2.addWidget(self.cancelPushButton)
         self.verticalLayout.addLayout(self.horizontalLayout_2)
 
-        self.retranslateUi(QSOFormDialog)
+        self.retranslateUi(QSOForm)
         self.toolBox.setCurrentIndex(0)
-        self.savePushButton.clicked.connect(QSOFormDialog.saveLog) # type: ignore
-        self.cancelPushButton.clicked.connect(QSOFormDialog.reject) # type: ignore
+        self.savePushButton.clicked.connect(QSOForm.saveLog) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(self.timeEdit.setDisabled) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(self.dateEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.ownLocatorLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.ownQTHLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.radioLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.antennaLineEdit.setDisabled) # type: ignore
-        self.bandComboBox.currentTextChanged['QString'].connect(QSOFormDialog.bandChanged) # type: ignore
-        self.stationGroupBox.toggled['bool'].connect(QSOFormDialog.stationChanged) # type: ignore
-        self.identityGroupBox.toggled['bool'].connect(QSOFormDialog.identityChanged) # type: ignore
+        self.bandComboBox.currentTextChanged['QString'].connect(QSOForm.bandChanged) # type: ignore
+        self.stationGroupBox.toggled['bool'].connect(QSOForm.stationChanged) # type: ignore
+        self.identityGroupBox.toggled['bool'].connect(QSOForm.identityChanged) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(self.ownCallSignLineEdit.setDisabled) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(self.ownNameLineEdit.setDisabled) # type: ignore
-        self.channelComboBox.currentTextChanged['QString'].connect(QSOFormDialog.channelChanged) # type: ignore
-        self.RSTRcvdLineEdit.textEdited['QString'].connect(QSOFormDialog.rstRcvdChanged) # type: ignore
-        self.RSTSentLineEdit.textEdited['QString'].connect(QSOFormDialog.rstSentChanged) # type: ignore
-        self.locatorLineEdit.textEdited['QString'].connect(QSOFormDialog.locatorChanged) # type: ignore
-        self.callSignLineEdit.textEdited['QString'].connect(QSOFormDialog.callSignChanged) # type: ignore
-        self.ownLocatorLineEdit.textEdited['QString'].connect(QSOFormDialog.ownLocatorChanged) # type: ignore
-        self.ownCallSignLineEdit.textEdited['QString'].connect(QSOFormDialog.ownCallSignChanged) # type: ignore
-        self.callSignLineEdit.editingFinished.connect(QSOFormDialog.setWorkedBefore) # type: ignore
-        self.timeNowPushButton.clicked.connect(QSOFormDialog.setStartTimeNow) # type: ignore
-        self.searchCallbookPushButton.clicked.connect(QSOFormDialog.searchCallbook) # type: ignore
-        self.uploadPushButton.clicked.connect(QSOFormDialog.uploadLog) # type: ignore
-        self.eqslInboxPushButton.clicked.connect(QSOFormDialog.eqslCheckInbox) # type: ignore
-        self.eqslDownloadPushButton.clicked.connect(QSOFormDialog.eqslDownload) # type: ignore
-        self.lotwInboxPushButton.clicked.connect(QSOFormDialog.lotwCheckInbox) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(QSOFormDialog)
-        QSOFormDialog.setTabOrder(self.callSignLineEdit, self.nameLineEdit)
-        QSOFormDialog.setTabOrder(self.nameLineEdit, self.QTHLineEdit)
-        QSOFormDialog.setTabOrder(self.QTHLineEdit, self.locatorLineEdit)
-        QSOFormDialog.setTabOrder(self.locatorLineEdit, self.searchCallbookPushButton)
-        QSOFormDialog.setTabOrder(self.searchCallbookPushButton, self.RSTSentLineEdit)
-        QSOFormDialog.setTabOrder(self.RSTSentLineEdit, self.RSTRcvdLineEdit)
-        QSOFormDialog.setTabOrder(self.RSTRcvdLineEdit, self.powerSpinBox)
-        QSOFormDialog.setTabOrder(self.powerSpinBox, self.bandComboBox)
-        QSOFormDialog.setTabOrder(self.bandComboBox, self.channelComboBox)
-        QSOFormDialog.setTabOrder(self.channelComboBox, self.freqDoubleSpinBox)
-        QSOFormDialog.setTabOrder(self.freqDoubleSpinBox, self.modeComboBox)
-        QSOFormDialog.setTabOrder(self.modeComboBox, self.identityGroupBox)
-        QSOFormDialog.setTabOrder(self.identityGroupBox, self.ownCallSignLineEdit)
-        QSOFormDialog.setTabOrder(self.ownCallSignLineEdit, self.ownNameLineEdit)
-        QSOFormDialog.setTabOrder(self.ownNameLineEdit, self.stationGroupBox)
-        QSOFormDialog.setTabOrder(self.stationGroupBox, self.ownQTHLineEdit)
-        QSOFormDialog.setTabOrder(self.ownQTHLineEdit, self.ownLocatorLineEdit)
-        QSOFormDialog.setTabOrder(self.ownLocatorLineEdit, self.radioLineEdit)
-        QSOFormDialog.setTabOrder(self.radioLineEdit, self.antennaLineEdit)
-        QSOFormDialog.setTabOrder(self.antennaLineEdit, self.dateOnEdit)
-        QSOFormDialog.setTabOrder(self.dateOnEdit, self.timeOnEdit)
-        QSOFormDialog.setTabOrder(self.timeOnEdit, self.timeNowPushButton)
-        QSOFormDialog.setTabOrder(self.timeNowPushButton, self.dateEdit)
-        QSOFormDialog.setTabOrder(self.dateEdit, self.timeEdit)
-        QSOFormDialog.setTabOrder(self.timeEdit, self.autoDateCheckBox)
-        QSOFormDialog.setTabOrder(self.autoDateCheckBox, self.commentsTextEdit)
-        QSOFormDialog.setTabOrder(self.commentsTextEdit, self.remarksTextEdit)
-        QSOFormDialog.setTabOrder(self.remarksTextEdit, self.savePushButton)
-        QSOFormDialog.setTabOrder(self.savePushButton, self.uploadPushButton)
-        QSOFormDialog.setTabOrder(self.uploadPushButton, self.cancelPushButton)
+        self.channelComboBox.currentTextChanged['QString'].connect(QSOForm.channelChanged) # type: ignore
+        self.RSTRcvdLineEdit.textEdited['QString'].connect(QSOForm.rstRcvdChanged) # type: ignore
+        self.RSTSentLineEdit.textEdited['QString'].connect(QSOForm.rstSentChanged) # type: ignore
+        self.locatorLineEdit.textEdited['QString'].connect(QSOForm.locatorChanged) # type: ignore
+        self.callSignLineEdit.textEdited['QString'].connect(QSOForm.callSignChanged) # type: ignore
+        self.ownLocatorLineEdit.textEdited['QString'].connect(QSOForm.ownLocatorChanged) # type: ignore
+        self.ownCallSignLineEdit.textEdited['QString'].connect(QSOForm.ownCallSignChanged) # type: ignore
+        self.callSignLineEdit.editingFinished.connect(QSOForm.setWorkedBefore) # type: ignore
+        self.timeNowPushButton.clicked.connect(QSOForm.setStartTimeNow) # type: ignore
+        self.searchCallbookPushButton.clicked.connect(QSOForm.searchCallbook) # type: ignore
+        self.uploadPushButton.clicked.connect(QSOForm.uploadLog) # type: ignore
+        self.eqslInboxPushButton.clicked.connect(QSOForm.eqslCheckInbox) # type: ignore
+        self.eqslDownloadPushButton.clicked.connect(QSOForm.eqslDownload) # type: ignore
+        self.lotwInboxPushButton.clicked.connect(QSOForm.lotwCheckInbox) # type: ignore
+        self.cancelPushButton.clicked.connect(QSOForm.clear) # type: ignore
+        self.modeComboBox.currentTextChanged['QString'].connect(QSOForm.modeChanged) # type: ignore
+        QtCore.QMetaObject.connectSlotsByName(QSOForm)
+        QSOForm.setTabOrder(self.callSignLineEdit, self.searchCallbookPushButton)
+        QSOForm.setTabOrder(self.searchCallbookPushButton, self.RSTSentLineEdit)
+        QSOForm.setTabOrder(self.RSTSentLineEdit, self.RSTRcvdLineEdit)
+        QSOForm.setTabOrder(self.RSTRcvdLineEdit, self.bandComboBox)
+        QSOForm.setTabOrder(self.bandComboBox, self.channelComboBox)
+        QSOForm.setTabOrder(self.channelComboBox, self.freqDoubleSpinBox)
+        QSOForm.setTabOrder(self.freqDoubleSpinBox, self.modeComboBox)
+        QSOForm.setTabOrder(self.modeComboBox, self.submodeComboBox)
+        QSOForm.setTabOrder(self.submodeComboBox, self.nameLineEdit)
+        QSOForm.setTabOrder(self.nameLineEdit, self.QTHLineEdit)
+        QSOForm.setTabOrder(self.QTHLineEdit, self.locatorLineEdit)
+        QSOForm.setTabOrder(self.locatorLineEdit, self.powerSpinBox)
+        QSOForm.setTabOrder(self.powerSpinBox, self.propComboBox)
+        QSOForm.setTabOrder(self.propComboBox, self.identityGroupBox)
+        QSOForm.setTabOrder(self.identityGroupBox, self.ownCallSignLineEdit)
+        QSOForm.setTabOrder(self.ownCallSignLineEdit, self.ownNameLineEdit)
+        QSOForm.setTabOrder(self.ownNameLineEdit, self.stationGroupBox)
+        QSOForm.setTabOrder(self.stationGroupBox, self.ownQTHLineEdit)
+        QSOForm.setTabOrder(self.ownQTHLineEdit, self.ownLocatorLineEdit)
+        QSOForm.setTabOrder(self.ownLocatorLineEdit, self.radioLineEdit)
+        QSOForm.setTabOrder(self.radioLineEdit, self.antennaLineEdit)
+        QSOForm.setTabOrder(self.antennaLineEdit, self.timeNowPushButton)
+        QSOForm.setTabOrder(self.timeNowPushButton, self.autoDateCheckBox)
+        QSOForm.setTabOrder(self.autoDateCheckBox, self.dateOnEdit)
+        QSOForm.setTabOrder(self.dateOnEdit, self.timeOnEdit)
+        QSOForm.setTabOrder(self.timeOnEdit, self.dateEdit)
+        QSOForm.setTabOrder(self.dateEdit, self.timeEdit)
+        QSOForm.setTabOrder(self.timeEdit, self.commentsTextEdit)
+        QSOForm.setTabOrder(self.commentsTextEdit, self.remarksTextEdit)
+        QSOForm.setTabOrder(self.remarksTextEdit, self.eqslSentCheckBox)
+        QSOForm.setTabOrder(self.eqslSentCheckBox, self.lotwSentCheckBox)
+        QSOForm.setTabOrder(self.lotwSentCheckBox, self.qslAccBureauCheckBox)
+        QSOForm.setTabOrder(self.qslAccBureauCheckBox, self.qslViaLineEdit)
+        QSOForm.setTabOrder(self.qslViaLineEdit, self.qslMessageTextEdit)
+        QSOForm.setTabOrder(self.qslMessageTextEdit, self.qslBurDirGroupBox)
+        QSOForm.setTabOrder(self.qslBurDirGroupBox, self.qslBureauRadioButton)
+        QSOForm.setTabOrder(self.qslBureauRadioButton, self.qslDirectRadioButton)
+        QSOForm.setTabOrder(self.qslDirectRadioButton, self.qslSentCheckBox)
+        QSOForm.setTabOrder(self.qslSentCheckBox, self.qslRcvdCheckBox)
+        QSOForm.setTabOrder(self.qslRcvdCheckBox, self.eqslGroupBox)
+        QSOForm.setTabOrder(self.eqslGroupBox, self.eqslInboxPushButton)
+        QSOForm.setTabOrder(self.eqslInboxPushButton, self.eqslDownloadPushButton)
+        QSOForm.setTabOrder(self.eqslDownloadPushButton, self.lotwGroupBox)
+        QSOForm.setTabOrder(self.lotwGroupBox, self.lotwInboxPushButton)
+        QSOForm.setTabOrder(self.lotwInboxPushButton, self.hamQTHGroupBox)
+        QSOForm.setTabOrder(self.hamQTHGroupBox, self.uploadPushButton)
+        QSOForm.setTabOrder(self.uploadPushButton, self.savePushButton)
+        QSOForm.setTabOrder(self.savePushButton, self.cancelPushButton)
+        QSOForm.setTabOrder(self.cancelPushButton, self.qslAccDirectCheckBox)
+        QSOForm.setTabOrder(self.qslAccDirectCheckBox, self.qslAcceQSLCheckBox)
+        QSOForm.setTabOrder(self.qslAcceQSLCheckBox, self.qslAccLoTWCheckBox)
+        QSOForm.setTabOrder(self.qslAccLoTWCheckBox, self.hamQTHmodRadioButton)
+        QSOForm.setTabOrder(self.hamQTHmodRadioButton, self.hamQTHuplRadioButton)
+        QSOForm.setTabOrder(self.hamQTHuplRadioButton, self.lotwRcvdCheckBox)
+        QSOForm.setTabOrder(self.lotwRcvdCheckBox, self.eqslRcvdCheckBox)
 
-    def retranslateUi(self, QSOFormDialog):
+    def retranslateUi(self, QSOForm):
         _translate = QtCore.QCoreApplication.translate
-        QSOFormDialog.setWindowTitle(_translate("QSOFormDialog", "Enter QSO"))
-        self.nameLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Name"))
-        self.callSignLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Call sign"))
-        self.QTHLineEdit.setPlaceholderText(_translate("QSOFormDialog", "QTH"))
-        self.locatorLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Locator"))
-        self.searchCallbookPushButton.setText(_translate("QSOFormDialog", "Callbook"))
-        self.label.setText(_translate("QSOFormDialog", "RST Tx"))
-        self.RSTSentLineEdit.setText(_translate("QSOFormDialog", "59"))
-        self.RSTSentLineEdit.setPlaceholderText(_translate("QSOFormDialog", "RST sent"))
-        self.label_2.setText(_translate("QSOFormDialog", "RST Rx"))
-        self.RSTRcvdLineEdit.setText(_translate("QSOFormDialog", "59"))
-        self.RSTRcvdLineEdit.setPlaceholderText(_translate("QSOFormDialog", "RST received"))
-        self.powerLabel.setText(_translate("QSOFormDialog", "Power"))
-        self.powerSpinBox.setSpecialValueText(_translate("QSOFormDialog", "n.a."))
-        self.powerSpinBox.setSuffix(_translate("QSOFormDialog", " W"))
-        self.bandComboBox.setPlaceholderText(_translate("QSOFormDialog", "Band"))
-        self.channelLabel.setText(_translate("QSOFormDialog", "Channel"))
-        self.freqLabel.setText(_translate("QSOFormDialog", "Frequency"))
-        self.freqDoubleSpinBox.setSpecialValueText(_translate("QSOFormDialog", "n.a."))
-        self.freqDoubleSpinBox.setSuffix(_translate("QSOFormDialog", " kHz"))
-        self.modeComboBox.setPlaceholderText(_translate("QSOFormDialog", "Mode"))
-        self.identityGroupBox.setTitle(_translate("QSOFormDialog", "Configured identity"))
-        self.ownCallSignLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Own call sign"))
-        self.ownNameLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Own name"))
-        self.stationGroupBox.setTitle(_translate("QSOFormDialog", "Configured station"))
-        self.ownQTHLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Own QTH"))
-        self.ownLocatorLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Own locator"))
-        self.radioLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Radio"))
-        self.antennaLineEdit.setPlaceholderText(_translate("QSOFormDialog", "Antenna"))
-        self.dateEdit.setDisplayFormat(_translate("QSOFormDialog", "yyyy-MM-dd"))
-        self.dateOnEdit.setDisplayFormat(_translate("QSOFormDialog", "yyyy-MM-dd"))
-        self.timeNowPushButton.setText(_translate("QSOFormDialog", "Now"))
-        self.label_4.setText(_translate("QSOFormDialog", "End"))
-        self.timeEdit.setDisplayFormat(_translate("QSOFormDialog", "HH:mm:ss"))
-        self.timeOnEdit.setDisplayFormat(_translate("QSOFormDialog", "HH:mm:ss"))
-        self.label_3.setText(_translate("QSOFormDialog", "Start"))
-        self.autoDateCheckBox.setText(_translate("QSOFormDialog", "Automatically"))
-        self.commentsTextEdit.setPlaceholderText(_translate("QSOFormDialog", "QSO comments"))
-        self.remarksTextEdit.setPlaceholderText(_translate("QSOFormDialog", "Own notes"))
-        self.toolBox.setItemText(self.toolBox.indexOf(self.mainPage), _translate("QSOFormDialog", "Main data"))
-        self.qslGroupBox.setTitle(_translate("QSOFormDialog", "QSL"))
-        self.qslViaLineEdit.setToolTip(_translate("QSOFormDialog", "The contacted station QSL route.\n"
+        QSOForm.setWindowTitle(_translate("QSOForm", "QSO Form"))
+        self.nameLineEdit.setPlaceholderText(_translate("QSOForm", "Name"))
+        self.callSignLineEdit.setPlaceholderText(_translate("QSOForm", "Call sign"))
+        self.QTHLineEdit.setPlaceholderText(_translate("QSOForm", "QTH"))
+        self.locatorLineEdit.setPlaceholderText(_translate("QSOForm", "Locator"))
+        self.searchCallbookPushButton.setText(_translate("QSOForm", "Callbook"))
+        self.label.setText(_translate("QSOForm", "RST Tx"))
+        self.RSTSentLineEdit.setText(_translate("QSOForm", "59"))
+        self.RSTSentLineEdit.setPlaceholderText(_translate("QSOForm", "RST sent"))
+        self.label_2.setText(_translate("QSOForm", "RST Rx"))
+        self.RSTRcvdLineEdit.setText(_translate("QSOForm", "59"))
+        self.RSTRcvdLineEdit.setPlaceholderText(_translate("QSOForm", "RST received"))
+        self.powerLabel.setText(_translate("QSOForm", "Power"))
+        self.powerSpinBox.setSpecialValueText(_translate("QSOForm", "n.a."))
+        self.powerSpinBox.setSuffix(_translate("QSOForm", " W"))
+        self.bandComboBox.setPlaceholderText(_translate("QSOForm", "Band"))
+        self.channelLabel.setText(_translate("QSOForm", "Channel"))
+        self.freqLabel.setText(_translate("QSOForm", "Frequency"))
+        self.freqDoubleSpinBox.setSpecialValueText(_translate("QSOForm", "n.a."))
+        self.freqDoubleSpinBox.setSuffix(_translate("QSOForm", " kHz"))
+        self.modeComboBox.setPlaceholderText(_translate("QSOForm", "Mode"))
+        self.submodeComboBox.setPlaceholderText(_translate("QSOForm", "Submode"))
+        self.propComboBox.setPlaceholderText(_translate("QSOForm", "Propagation"))
+        self.identityGroupBox.setTitle(_translate("QSOForm", "Configured identity"))
+        self.ownCallSignLineEdit.setPlaceholderText(_translate("QSOForm", "Own call sign"))
+        self.ownNameLineEdit.setPlaceholderText(_translate("QSOForm", "Own name"))
+        self.stationGroupBox.setTitle(_translate("QSOForm", "Configured station"))
+        self.ownQTHLineEdit.setPlaceholderText(_translate("QSOForm", "Own QTH"))
+        self.ownLocatorLineEdit.setPlaceholderText(_translate("QSOForm", "Own locator"))
+        self.radioLineEdit.setPlaceholderText(_translate("QSOForm", "Radio"))
+        self.antennaLineEdit.setPlaceholderText(_translate("QSOForm", "Antenna"))
+        self.dateEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
+        self.dateOnEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
+        self.timeNowPushButton.setText(_translate("QSOForm", "Now"))
+        self.label_4.setText(_translate("QSOForm", "End"))
+        self.timeEdit.setDisplayFormat(_translate("QSOForm", "HH:mm:ss"))
+        self.timeOnEdit.setDisplayFormat(_translate("QSOForm", "HH:mm:ss"))
+        self.label_3.setText(_translate("QSOForm", "Start"))
+        self.autoDateCheckBox.setText(_translate("QSOForm", "Automatically"))
+        self.commentsTextEdit.setPlaceholderText(_translate("QSOForm", "QSO comments"))
+        self.remarksTextEdit.setPlaceholderText(_translate("QSOForm", "Own notes"))
+        self.toolBox.setItemText(self.toolBox.indexOf(self.mainPage), _translate("QSOForm", "Main data"))
+        self.qslGroupBox.setTitle(_translate("QSOForm", "QSL"))
+        self.qslViaLineEdit.setToolTip(_translate("QSOForm", "The contacted station QSL route.\n"
 "This is not the QSL manager/bureau address."))
-        self.qslViaLineEdit.setPlaceholderText(_translate("QSOFormDialog", "QSL via"))
-        self.qslMessageTextEdit.setPlaceholderText(_translate("QSOFormDialog", "QSL card message"))
-        self.label_5.setText(_translate("QSOFormDialog", "Accepts:"))
-        self.qslAccBureauCheckBox.setText(_translate("QSOFormDialog", "Bureau"))
-        self.qslAccDirectCheckBox.setText(_translate("QSOFormDialog", "Direct"))
-        self.qslAcceQSLCheckBox.setText(_translate("QSOFormDialog", "eQSL"))
-        self.qslAccLoTWCheckBox.setText(_translate("QSOFormDialog", "LoTW"))
-        self.qslBurDirGroupBox.setTitle(_translate("QSOFormDialog", "Bureau/Direct"))
-        self.qslBureauRadioButton.setText(_translate("QSOFormDialog", "Bureau"))
-        self.qslDirectRadioButton.setText(_translate("QSOFormDialog", "Direct"))
-        self.qslSentCheckBox.setText(_translate("QSOFormDialog", "QSL sent"))
-        self.qslRcvdCheckBox.setText(_translate("QSOFormDialog", "QSL received"))
-        self.eqslGroupBox.setTitle(_translate("QSOFormDialog", "eQSL"))
-        self.eqslSentCheckBox.setText(_translate("QSOFormDialog", "eQSL sent"))
-        self.eqslRcvdCheckBox.setText(_translate("QSOFormDialog", "eQSL received"))
-        self.eqslInboxPushButton.setText(_translate("QSOFormDialog", "Check Inbox"))
-        self.eqslLinkLabel.setText(_translate("QSOFormDialog", "Link to eQSL Card"))
-        self.eqslDownloadPushButton.setText(_translate("QSOFormDialog", "Download eQSL"))
-        self.lotwGroupBox.setTitle(_translate("QSOFormDialog", "LoTW"))
-        self.lotwSentCheckBox.setText(_translate("QSOFormDialog", "LoTW sent"))
-        self.lotwRcvdCheckBox.setText(_translate("QSOFormDialog", "LoTW received"))
-        self.lotwInboxPushButton.setText(_translate("QSOFormDialog", "Check Inbox"))
-        self.hamQTHGroupBox.setTitle(_translate("QSOFormDialog", "HamQTH"))
-        self.hamQTHuplRadioButton.setText(_translate("QSOFormDialog", "Uploaded"))
-        self.hamQTHmodRadioButton.setText(_translate("QSOFormDialog", "Modified"))
-        self.toolBox.setItemText(self.toolBox.indexOf(self.qslPage), _translate("QSOFormDialog", "QSL && Log upload"))
-        self.uploadPushButton.setToolTip(_translate("QSOFormDialog", "Uploads only if selected on QSL page"))
-        self.uploadPushButton.setText(_translate("QSOFormDialog", "Save && Upload"))
-        self.savePushButton.setText(_translate("QSOFormDialog", "Save"))
-        self.cancelPushButton.setText(_translate("QSOFormDialog", "Cancel"))
+        self.qslViaLineEdit.setPlaceholderText(_translate("QSOForm", "QSL via"))
+        self.qslMessageTextEdit.setPlaceholderText(_translate("QSOForm", "QSL card message"))
+        self.label_5.setText(_translate("QSOForm", "Accepts:"))
+        self.qslAccBureauCheckBox.setText(_translate("QSOForm", "Bureau"))
+        self.qslAccDirectCheckBox.setText(_translate("QSOForm", "Direct"))
+        self.qslAcceQSLCheckBox.setText(_translate("QSOForm", "eQSL"))
+        self.qslAccLoTWCheckBox.setText(_translate("QSOForm", "LoTW"))
+        self.qslBurDirGroupBox.setTitle(_translate("QSOForm", "Bureau/Direct"))
+        self.qslBureauRadioButton.setText(_translate("QSOForm", "Bureau"))
+        self.qslDirectRadioButton.setText(_translate("QSOForm", "Direct"))
+        self.qslSentCheckBox.setText(_translate("QSOForm", "QSL sent"))
+        self.qslRcvdCheckBox.setText(_translate("QSOForm", "QSL received"))
+        self.eqslGroupBox.setTitle(_translate("QSOForm", "eQSL"))
+        self.eqslSentCheckBox.setText(_translate("QSOForm", "eQSL sent"))
+        self.eqslRcvdCheckBox.setText(_translate("QSOForm", "eQSL received"))
+        self.eqslInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
+        self.eqslLinkLabel.setText(_translate("QSOForm", "Link to eQSL Card"))
+        self.eqslDownloadPushButton.setText(_translate("QSOForm", "Download eQSL"))
+        self.lotwGroupBox.setTitle(_translate("QSOForm", "LoTW"))
+        self.lotwSentCheckBox.setText(_translate("QSOForm", "LoTW sent"))
+        self.lotwRcvdCheckBox.setText(_translate("QSOForm", "LoTW received"))
+        self.lotwInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
+        self.hamQTHGroupBox.setTitle(_translate("QSOForm", "HamQTH"))
+        self.hamQTHuplRadioButton.setText(_translate("QSOForm", "Uploaded"))
+        self.hamQTHmodRadioButton.setText(_translate("QSOForm", "Modified"))
+        self.toolBox.setItemText(self.toolBox.indexOf(self.qslPage), _translate("QSOForm", "QSL && Log upload"))
+        self.uploadPushButton.setToolTip(_translate("QSOForm", "Uploads only if selected on QSL page"))
+        self.uploadPushButton.setText(_translate("QSOForm", "Save && Upload"))
+        self.savePushButton.setText(_translate("QSOForm", "Save"))
+        self.cancelPushButton.setText(_translate("QSOForm", "Clear"))
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_RegEx.py` & `DragonLog-1.0/dragonlog/DragonLog_RegEx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module contains the regular expression for field validation"""
 import re
 
 REGEX_CALL = re.compile(r'([a-zA-Z0-9]{1,3}?/)?([a-zA-Z0-9]{1,3}?[0-9][a-zA-Z0-9]{0,3}?[a-zA-Z])(/[aAmMpPrRtT]{1,2}?)?')
-REGEX_RSTFIELD = re.compile(r'([1-5][1-9][1-9aAcCkKmMsSxX]?)|([rR]?-?[0-9]{1,2})')
+REGEX_RSTFIELD = re.compile(r'([1-5][1-9][1-9aAcCkKmMsSxX]?)|([rR]?[-+]?[0-9]{1,2})')
 REGEX_LOCATOR = re.compile(r'[a-rA-R]{2}[0-9]{2}([a-xA-X]{2}([0-9]{2})?)?')
-
+REGEX_NONASCII = re.compile(r'[ -~\n\r]*(.)?')
 
 def check_format(exp: re.Pattern, txt: str) -> bool:
     """Test the given text against a regular expression
     :param exp: a compiled pattern
     :param txt: a text
     :return: true if pattern matches"""
     return bool(re.fullmatch(exp, txt))
@@ -17,7 +17,10 @@
     """Test a call sign against a regular expression
     :param call: a call sign
     :return: tuple of parts ('Country prefix/', 'Call sign', '/Operation suffix')"""
 
     m = re.fullmatch(REGEX_CALL, call)
     if m:
         return m.groups()
+
+def find_non_ascii(text: str) -> set:
+    return set(re.findall(REGEX_NONASCII, text))
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_Settings.py` & `DragonLog-1.0/dragonlog/DragonLog_Settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,18 @@
         self.rig_ids = None
         self.rigs = None
         self.rigctld_path = None
         self.rigctld = None
         self.rig_caps = []
         self.rig_status = rig_status
 
+        self.rigctl_startupinfo = None
         if platform.system() == 'Windows':
+            self.rigctl_startupinfo = subprocess.STARTUPINFO()
+            self.rigctl_startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
             if self.settings.value('cat/rigctldPath', None):
                 if self.__is_exe__(self.settings.value('cat/rigctldPath')):
                     self.init_hamlib(self.settings.value('cat/rigctldPath'))
                 else:
                     self.settings.setValue('cat/rigctldPath', '')
                     self.hamlibPathLineEdit.setText('')
         else:
@@ -85,15 +88,15 @@
             self.ctrlRigctldPushButton.setText(self.tr('Start'))
             self.ctrlRigctldPushButton.setChecked(False)
             self.rig_caps = []
             self.checkHamlibTimer.stop()
             self.rig_status.setText(self.tr('Hamlib') + ': ' + self.tr('inactiv'))
 
     def isRigctldActive(self):
-        return self.ctrlRigctldPushButton.isChecked()
+        return self.rigctld and not self.rigctld.poll()
 
     @staticmethod
     def __is_exe__(path):
         return os.path.isfile(path) and os.access(path, os.X_OK)
 
     def chooseHamlibPath(self):
         rigctld_path = QtWidgets.QFileDialog.getOpenFileName(
@@ -155,42 +158,60 @@
             self.settings.setValue('cat/rigctldPath', rigctld_path)
             self.hamlibPathLineEdit.setText(rigctld_path)
             self.checkHamlibLabel.setText('')
             self.rigctld_path = rigctld_path
 
     def mfrChanged(self, mfr):
         self.modelComboBox.clear()
-        self.modelComboBox.insertItems(0, sorted(self.rigs[mfr]))
+
+        if mfr in self.rigs:
+            self.modelComboBox.insertItems(0, sorted(self.rigs[mfr]))
 
         if self.settings.value('cat/rigModel', None):
             self.modelComboBox.setCurrentText(self.settings.value('cat/rigModel'))
 
     def collectRigCaps(self, rig_id):
-        res = subprocess.run([self.rigctld_path, f'--model={rig_id}', '-u'], capture_output=True)
+        res = subprocess.run([self.rigctld_path, f'--model={rig_id}', '-u'],
+                             capture_output=True,
+                             startupinfo=self.rigctl_startupinfo)
         stdout = str(res.stdout, sys.getdefaultencoding()).replace('\r', '')
         self.rig_caps = []
         for ln in stdout.split('\n'):
             if ln.startswith('Can '):
                 cap, able = ln.split(':')
                 if able.strip() == 'Y':
                     self.rig_caps.append(cap[4:].lower())
 
     def ctrlRigctld(self, start):
         if start:
             if not self.rigctld:
-                # FIXME: read from settings not from UI (problem if UI was never initialised)
-                rig_id = self.rig_ids[self.manufacturerComboBox.currentText() + '/' + self.modelComboBox.currentText()]
+                rig_mfr = self.settings.value('cat/rigMfr')
+                rig_model = self.settings.value('cat/rigModel')
+                rig_if = self.settings.value("cat/interface")
+                rig_speed = self.settings.value("cat/baud")
+                if not rig_mfr or not rig_model or not rig_if or not rig_speed:
+                    QtWidgets.QMessageBox.critical(self, self.tr('CAT settings error'),
+                                                   self.tr('CAT configuration was never saved '
+                                                           'or a parameter is missing'))
+                    self.ctrlRigctldPushButton.setChecked(False)
+                    self.parent().actionStart_hamlib_TB.setChecked(False)
+                    self.parent().actionStart_hamlib_TB.setText(self.tr('Start hamlib'))
+                    return
+
+                rig_id = self.rig_ids[f'{rig_mfr}/{rig_model}']
 
                 self.collectRigCaps(rig_id)
 
                 self.rigctld = subprocess.Popen([self.rigctld_path,
                                                  f'--model={rig_id}',
-                                                 f'--rig-file={self.catInterfaceLineEdit.text().strip()}',
-                                                 f'--serial-speed={self.catBaudComboBox.currentText()}',
-                                                 '--listen-addr=127.0.0.1'])
+                                                 f'--rig-file={rig_if}',
+                                                 f'--serial-speed={rig_speed}',
+                                                 '--listen-addr=127.0.0.1'],
+                                                startupinfo=self.rigctl_startupinfo)
+
                 if self.rigctld.poll():
                     self.checkHamlibRunLabel.setText(self.tr('rigctld did not start properly'))
                     self.ctrlRigctldPushButton.setChecked(False)
                     self.parent().actionStart_hamlib_TB.setChecked(False)
                     self.parent().actionStart_hamlib_TB.setText(self.tr('Start hamlib'))
                     self.rig_status.setText(self.tr('Hamlib') + ': ' + self.tr('inactiv'))
                 else:
```

### Comparing `DragonLog-0.8.1/dragonlog/DragonLog_Settings_ui.py` & `DragonLog-1.0/dragonlog/DragonLog_Settings_ui.py`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/Logger.py` & `DragonLog-1.0/dragonlog/Logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os.path
 import sys
+import time
 import logging
 
 from PyQt6 import QtCore, QtWidgets, QtGui
 
 
 class Logger(logging.Handler):
     def __init__(self, log_widget: QtWidgets.QTextEdit, settings: QtCore.QSettings):
         super().__init__()
         self.log_widget = log_widget
         self.settings = settings
 
         self.__loglevel__ = self.settings.value('ui/log_level', 'INFO')
-
+        logging.Formatter.converter = time.gmtime
         self.setFormatter(logging.Formatter('%(asctime)s %(levelname)-8s: %(name)s - %(message)s'))
         self.__log__ = logging.getLogger('DragonLog')
         self.__log__.setLevel(self.__loglevel__)
         self.__log__.addHandler(self)
 
         self.__log_file__ = None
         if int(self.settings.value('ui/log_file', 0)):
```

### Comparing `DragonLog-0.8.1/dragonlog/data/README.md` & `DragonLog-1.0/dragonlog/data/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 * input validation for callsign, RST, locator
 * show worked before if a callsign is already logged
 * distance calculation
 * automatic time
 * callbook search and log upload (HamQTH.com)
 * eQSL upload, check and download
 * LoTW signing, upload and check status
-* CAT (band, frequency, mode, power via hamlib integration)
+* CAT (band, frequency, mode/submode, power via hamlib integration)
 * watch log files for automatic log import of WSJT-X, JS8Call, fldigi and others
 * ADIF adi/adx export/import
 * Excel/CSV export/import
 * log 11m band QSOs
-* filter recent QSOs (last week, mont, half year, year)
-* UTF-8 (i.e. use german umlauts) and convert german umlauts for ADIF export
+* filter recent QSOs (last week, month, half year, year)
+* UTF-8 (i.e. use german umlauts)
+* convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
 The installation requires a python installation (>= 3.9).
     
     # python3 -m pip install DragonLog
 
@@ -141,15 +142,15 @@
 
 Hamlib integration
 ------------------
 You can use hamlib to interact with your radio. 
 
 The QSO logging form automatically updates radio information:
 * frequency (and band)
-* mode
+* mode (and submode)
 * power
 
 Hamlib can be downloaded at https://github.com/Hamlib/Hamlib/releases.
 DragonLog is tested against version 4.5.5.
 
 After selecting your radio and interface settings you can press the start button to start the communication.
```

### Comparing `DragonLog-0.8.1/dragonlog/data/bands.json` & `DragonLog-1.0/dragonlog/data/bands.json`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/data/cb_channels.json` & `DragonLog-1.0/dragonlog/data/cb_channels.json`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/data/color_map.json` & `DragonLog-1.0/dragonlog/data/color_map.json`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/data/i18n/DragonLog_de.qm` & `DragonLog-1.0/dragonlog/data/i18n/DragonLog_de.qm`

 * *Files 10% similar despite different names*

```diff
@@ -1,1393 +1,1481 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0564 655f 4445 4200 0008 e800  .....de_DEB.....
+00000010: a700 0000 0564 655f 4445 4200 0009 a800  .....de_DEB.....
 00000020: 0000 3c00 0001 5c00 0000 3e00 0001 7800  ..<...\...>...x.
-00000030: 0002 5700 0039 8600 0003 8900 0039 d000  ..W..9.......9..
-00000040: 0005 5b00 0020 9500 000c d000 0011 4100  ..[.. ........A.
+00000030: 0002 5700 0035 4700 0003 8900 0035 8500  ..W..5G......5..
+00000040: 0005 5b00 0023 6c00 000c d000 0011 4100  ..[..#l.......A.
 00000050: 0031 0e00 0000 0000 0047 6400 0001 fe00  .1.......Gd.....
-00000060: 004c 4400 003d 9600 0052 8400 0007 8400  .LD..=...R......
-00000070: 0053 5e00 0008 b200 0055 6700 0040 9400  .S^......Ug..@..
-00000080: 0056 7c00 0042 6000 0056 7f00 0023 1300  .V|..B`..V...#..
-00000090: 0056 8800 000a 9000 0056 8800 0023 bb00  .V.......V...#..
-000000a0: 0056 8800 0044 2500 0058 f700 000b 0c00  .V...D%..X......
-000000b0: 026f fa00 0039 aa00 0345 3000 0000 3f00  .o...9...E0...?.
+00000060: 004c 4400 003d 5700 0052 8400 0007 8400  .LD..=W..R......
+00000070: 0053 5e00 0008 b200 0055 6700 0041 7e00  .S^......Ug..A~.
+00000080: 0056 7c00 0043 6500 0056 7f00 0026 2900  .V|..Ce..V...&).
+00000090: 0056 8800 000a 9000 0056 8800 0026 d100  .V.......V...&..
+000000a0: 0056 8800 0045 4a00 0058 f700 000b 0c00  .V...EJ..X......
+000000b0: 026f fa00 0035 6500 0345 3000 0000 3f00  .o...5e..E0...?.
 000000c0: 0357 3000 0000 bf00 037b 3000 0000 fe00  .W0......{0.....
-000000d0: 03c9 3000 0001 3d00 0488 4400 0014 0f00  ..0...=...D.....
-000000e0: 0488 4400 003a b000 04bb 0400 002c 1700  ..D..:.......,..
-000000f0: 04cf 0400 002c 4e00 04d0 2500 002c c300  .....,N...%..,..
-00000100: 04ec 3000 001b de00 04ec 3000 002c f000  ..0.......0..,..
-00000110: 0534 9700 0007 d800 0534 9700 003e ec00  .4.......4...>..
-00000120: 0545 a500 001f b700 0545 a500 0040 0c00  .E.......E...@..
-00000130: 0548 3500 0008 da00 0548 3500 001f d900  .H5......H5.....
-00000140: 0548 3500 0040 6e00 0596 7c00 000e 2800  .H5..@n...|...(.
-00000150: 0598 c500 0045 4b00 05ab 6000 004b 9c00  .....EK...`..K..
-00000160: 06a6 7c00 0011 2200 06a6 7c00 0048 1400  ..|..."...|..H..
-00000170: 06fb 2100 003f cd00 0714 3e00 0048 ca00  ..!..?....>..H..
-00000180: 144b 9e00 000d 9500 144e e600 001d ff00  .K.......N......
-00000190: 3477 3000 0000 7f00 34c5 3000 0000 9f00  4w0.....4.0.....
-000001a0: 36b7 3000 0000 de00 38a9 3000 0001 1d00  6.0.....8.0.....
-000001b0: 4796 c400 0013 4f00 4796 c400 0029 c100  G.....O.G....)..
-000001c0: 47ab 7600 0029 8e00 47ab 7600 004c 2b00  G.v..)..G.v..L+.
-000001d0: 4c99 6200 001a 8500 4c99 6200 0035 0e00  L.b.....L.b..5..
-000001e0: 52cc bc00 0007 ae00 556a c300 0020 6400  R.......Uj... d.
-000001f0: 56ae c200 004d 0d00 576d c200 0021 c400  V....M..Wm...!..
-00000200: 576d c200 0042 2900 587a ff00 000a ae00  Wm...B).Xz......
-00000210: 587a ff00 0024 4a00 587a ff00 0045 2400  Xz...$J.Xz...E$.
-00000220: 5aa8 9400 000d e600 5aa8 9400 0045 d900  Z.......Z....E..
-00000230: 5aa8 9400 004b 3700 67ab 0600 004b ff00  Z....K7.g....K..
-00000240: 6d92 9400 0049 d700 753c 2300 0041 e200  m....I..u<#..A..
-00000250: 8cd2 1500 0010 1200 aa80 2500 0019 9800  ..........%.....
-00000260: ab72 4500 0009 cd00 bf5b b400 0005 f500  .rE......[......
-00000270: c656 de00 0034 0700 c656 de00 003c b900  .V...4...V...<..
-00000280: ff2c 7700 001b 0d01 48c4 ff00 0019 d201  .,w.....H.......
-00000290: 4d8a bc00 001e 7401 5478 6c00 001f 1a01  M.....t.Txl.....
-000002a0: 6bb3 1300 0043 db01 945e f800 0025 1001  k....C...^...%..
-000002b0: 9ce8 5e00 0046 0001 e578 e300 000d 2601  ..^..F...x....&.
-000002c0: e907 4500 0036 7801 fdeb 5400 0048 3a02  ..E..6x...T..H:.
-000002d0: 3222 f900 003a 6b02 33a9 3400 0008 f902  2"...:k.3.4.....
-000002e0: 96b3 2e00 002d a202 e7d6 5e00 0002 4102  .....-....^...A.
-000002f0: e7d6 5e00 0014 8102 e7d6 5e00 003b 4b02  ..^.......^..;K.
-00000300: e81d 2400 0034 5f03 004d 1200 000c 2d03  ..$..4_..M....-.
-00000310: 0149 e600 001e 2c03 0cac 0500 000f 9c03  .I....,.........
-00000320: 0f6b 1200 0041 5503 0f6b 3200 0020 b503  .k...AU..k2.. ..
-00000330: 4485 3000 0000 1e03 45b3 3000 0000 5e03  D.0.....E.0...^.
-00000340: 4ecb 9200 002e e103 4ecb 9200 004b 5903  N.......N....KY.
-00000350: 533f be00 004d 3603 598b 3200 0007 f703  S?...M6.Y.2.....
-00000360: 598b 3200 001d da03 598b 3200 003f a403  Y.2.....Y.2..?..
-00000370: 6cc3 0400 000b c503 881f d400 0006 1e03  l...............
-00000380: 9ce9 a500 0021 f703 f5e0 0700 0028 6e04  .....!.......(n.
-00000390: 07f6 ee00 0021 7504 07f6 ee00 0041 0204  .....!u......A..
-000003a0: 6c90 3200 0036 0504 8caf 6200 0013 e104  l.2..6....b.....
-000003b0: 9849 bc00 003b b404 9c8b 8500 003a d604  .I...;.......:..
-000003c0: a472 8400 0026 c304 ab8e f500 002a be04  .r...&.......*..
-000003d0: ab8e fc00 002a e304 ab8f 0100 002b 0804  .....*.......+..
-000003e0: ab8f 0700 002b 5804 ab8f 0800 002b 7d04  .....+X......+}.
-000003f0: b08b a400 003d 1704 b2b6 6400 0008 6b04  .....=....d...k.
-00000400: c4a9 a900 0013 1604 cf76 9400 0004 7104  .........v....q.
-00000410: d3c8 ff00 0014 bc04 e826 8800 0005 d404  .........&......
-00000420: e826 8800 001b 9604 e826 8800 003e 6b04  .&.......&...>k.
-00000430: e842 f200 001b ba04 e842 f200 004a 4d04  .B.......B...JM.
-00000440: edd3 6400 0030 cc04 f5b6 e700 0026 1405  ..d..0.......&..
-00000450: 1f06 1500 004a 7005 3268 c400 0003 f505  .....Jp.2h......
-00000460: 3ddf a300 000a ce05 4466 8200 0036 cb05  =.......Df...6..
-00000470: 5776 4500 0042 da05 6336 9e00 002d 6105  WvE..B..c6...-a.
-00000480: 647d 0e00 002a 6a05 7865 9800 0044 4a05  d}...*j.xe...DJ.
-00000490: 7865 b800 0044 7205 afca f400 0040 3205  xe...Dr......@2.
-000004a0: c7f7 2800 004d 9a05 c984 e900 002b a206  ..(..M.......+..
-000004b0: 011e c400 0002 7906 43c1 1300 0015 ed06  ......y.C.......
-000004c0: 778d 0800 0006 cd06 778d 0800 001c 5606  w.......w.....V.
-000004d0: 7e7c a100 0022 e006 7e7c a100 0043 b206  ~|..."..~|...C..
-000004e0: 830d be00 0025 ce06 bdf0 a400 0018 c406  .....%..........
-000004f0: be94 d200 004b bd06 d2af d900 004d c406  .....K.......M..
-00000500: e056 d800 0021 3a06 e056 d800 0040 c306  .V...!:..V...@..
-00000510: f895 8e00 0015 2707 2f4a 1500 0037 b207  ......'./J...7..
-00000520: 357f 7400 0047 2607 366b 9300 0004 f707  5.t..G&.6k......
-00000530: 50be 3900 004c 5d07 68f8 4400 0039 2707  P.9..L].h.D..9'.
-00000540: 693d fe00 002c 7f07 6941 4e00 002d 1d07  i=...,..iAN..-..
-00000550: 6cbb 6300 000e 4707 e67a d700 002b ef07  l.c...G..z...+..
-00000560: e76d c800 0022 3a07 e78f a400 0022 7007  .m...":......"p.
-00000570: e79f 3400 0022 a807 e79f 3400 0043 7007  ..4.."....4..Cp.
-00000580: e7e0 a400 0029 1807 e7f2 3400 0029 5307  .....)....4..)S.
-00000590: e7f2 3400 0048 8508 3292 cb00 003b 8a08  ..4..H..2....;..
-000005a0: 3587 6a00 0027 2208 36b6 5400 0012 5a08  5.j..'".6.T...Z.
-000005b0: 5ac5 0100 0001 9408 5ac5 0100 0013 ae08  Z.......Z.......
-000005c0: 5ac5 0100 003a 3408 678f b400 0023 dc08  Z....:4.g....#..
-000005d0: 679f 2400 0024 1408 679f 2400 0044 e208  g.$..$..g.$..D..
-000005e0: 8879 1400 0018 5608 aae3 e400 0009 9a08  .y....V.........
-000005f0: b63d de00 002f cf08 bd74 5e00 001f fb08  .=.../...t^.....
-00000600: d39b 6400 003f 1208 f89a cb00 0030 4609  ..d..?.......0F.
-00000610: 14be 9200 0037 2309 1c52 9500 0028 cd09  .....7#..R...(..
-00000620: 238c 7500 0016 2709 3f8c ad00 000c aa09  #.u...'.?.......
-00000630: 564e 4200 0038 1409 6c61 f400 0013 7a09  VNB..8..la....z.
-00000640: 6c61 f400 0029 ed09 6fe6 7e00 0011 5e09  la...)..o.~...^.
-00000650: 8fa3 8700 002a 2209 97c9 1400 001d 9f09  .....*".........
-00000660: 97c9 1400 003f 5d09 97d9 8400 001d 6409  .....?].......d.
-00000670: 9c7f 1a00 0039 f409 a118 8500 0010 dd09  .....9..........
-00000680: c004 d700 0003 bc09 c4e8 d700 0001 c409  ................
-00000690: c943 f500 000f d709 e854 fc00 0014 f809  .C.......T......
-000006a0: e854 fc00 003b ee0a 2190 e200 0006 840a  .T...;..!.......
-000006b0: 2190 e200 001c 0a0a 3f0e 9500 0024 c70a  !.......?....$..
-000006c0: 5e68 d900 0023 340a 6789 3b00 0007 0c0a  ^h...#4.g.;.....
-000006d0: 6789 3b00 001c 980a 67a9 0200 0007 480a  g.;.....g.....H.
-000006e0: 67a9 0200 001c d70a 6dc8 3e00 002f 680a  g.......m.>../h.
-000006f0: 7833 e400 003b 060a 7d6b 2400 0017 8a0a  x3...;..}k$.....
-00000700: 92a2 e500 0025 7a0a 9612 e500 0024 6d0a  .....%z......$m.
-00000710: a8b0 0e00 000e 060a a8b0 0e00 0037 8f0a  .............7..
-00000720: acdb 7e00 0002 1c0a c41a 2f00 003d c30a  ..~......./..=..
-00000730: c5b4 4900 0035 8a0a c897 c500 0006 460a  ..I..5........F.
-00000740: d2f0 b500 0002 e60a d382 7700 0003 340a  ..........w...4.
-00000750: e2b5 9600 0004 920a f31c 2200 0032 da0b  .........."..2..
-00000760: 1805 3900 0014 310b 4597 5500 0008 190b  ..9...1.E.U.....
-00000770: 6628 d200 002f 260b 7fe2 de00 002d fc0c  f(.../&......-..
-00000780: 08f5 6c00 003d 4b0c 107d 9300 0003 7e0c  ..l..=K..}....~.
-00000790: 1415 6300 003e 410c 1f2f 0200 0038 650c  ..c..>A../...8e.
-000007a0: 29f2 a400 0048 f80c 6a19 e900 0033 b80c  )....H..j....3..
-000007b0: 6a19 e900 003c 640c 8c09 2900 001b 5f0c  j....<d...)..._.
-000007c0: 8c09 2900 003e 060c a3fa 5f00 0019 5a0c  ..)..>...._...Z.
-000007d0: a6e8 d400 0032 1e0c bb01 7300 000c 6d0c  .....2....s...m.
-000007e0: bb01 7300 002e 530c c9a0 0e00 0028 490d  ..s...S......(I.
-000007f0: 0218 6400 0045 830d 07a4 f800 003c 210d  ..d..E.......<!.
-00000800: 3504 b400 0032 7a0d 4459 fc00 002b 2d0d  5....2z.DY...+-.
-00000810: 76f7 5900 001a b40d 825f 7300 000e ea0d  v.Y......_s.....
-00000820: f2ea c200 0033 4e0d fe4e 2400 0019 0d0d  .....3N..N$.....
-00000830: fe4e 2400 0049 8b0e 0543 5500 0020 fc0e  .N$..I...CU.. ..
-00000840: 05d1 b500 0049 240e 0743 5500 0041 a00e  .....I$..CU..A..
-00000850: 233d d500 0047 660e 87ac 6400 001d 160e  #=...Gf...d.....
-00000860: 93fa 5200 0016 cc0e a32f e400 0035 3b0e  ..R....../...5;.
-00000870: c497 a200 000b 3c0e c72a a600 0005 5f0e  ......<..*...._.
-00000880: de3d a200 0031 b10e e46b 3400 0044 9a0e  .=...1...k4..D..
-00000890: fdeb 3400 0043 280f 165e c400 0042 850f  ..4..C(..^...B..
-000008a0: 2229 6300 001e c20f 3562 ce00 0017 2d0f  ")c.....5b....-.
-000008b0: 6963 bc00 000c ef0f 6963 bc00 0026 890f  ic......ic...&..
-000008c0: 6963 bc00 004a fe0f 6978 c700 002e 940f  ic...J..ix......
-000008d0: 6c98 6c00 004c e20f 7ddd 2800 0038 ab0f  l.l..L..}.(..8..
-000008e0: 8007 d400 0031 4b0f 8313 8900 0012 e30f  .....1K.........
-000008f0: cb15 5200 0018 0c0f e6f6 3400 0035 b20f  ..R.......4..5..
-00000900: e6f6 3400 003e 9369 0000 4dee 03ff ffff  ..4..>.i..M.....
-00000910: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
-00000920: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000930: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
-00000940: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000950: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
-00000960: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000970: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
-00000980: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000990: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
-000009a0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-000009b0: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
-000009c0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-000009d0: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
+000000d0: 03c9 3000 0001 3d00 0488 4400 0014 e900  ..0...=...D.....
+000000e0: 0488 4400 0037 b800 04bb 0400 0030 e900  ..D..7.......0..
+000000f0: 04cf 0400 0031 2000 04d0 2500 0031 ba00  .....1 ...%..1..
+00000100: 04e7 1000 001d f000 04ec 3000 001d c400  ..........0.....
+00000110: 04ec 3000 0031 e700 0534 9700 0007 d800  ..0..1...4......
+00000120: 0534 9700 003e f000 0545 a500 0022 8e00  .4...>...E..."..
+00000130: 0545 a500 0040 6500 0548 3500 0008 da00  .E...@e..H5.....
+00000140: 0548 3500 0022 b000 0548 3500 0040 bb00  .H5.."...H5..@..
+00000150: 0596 7c00 000e 2800 0598 c500 0046 4c00  ..|...(......FL.
+00000160: 05ab 6000 0050 6a00 06a6 7c00 0011 2200  ..`..Pj...|...".
+00000170: 06a6 7c00 004b 7000 06fb 2100 0040 2c00  ..|..Kp...!..@,.
+00000180: 0714 3e00 004c 1400 144b 9e00 000d 9500  ..>..L...K......
+00000190: 144e e600 0020 e600 3477 3000 0000 7f00  .N... ..4w0.....
+000001a0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
+000001b0: 38a9 3000 0001 1d00 4796 c400 0013 4f00  8.0.....G.....O.
+000001c0: 4796 c400 002e be00 47ab 7600 002e 8b00  G.......G.v.....
+000001d0: 47ab 7600 0050 f900 4a2b 8200 003b 5500  G.v..P..J+...;U.
+000001e0: 4c99 6200 001b 7700 4c99 6200 003d 7e00  L.b...w.L.b..=~.
+000001f0: 52cc bc00 0007 ae00 556a c300 0023 3b00  R.......Uj...#;.
+00000200: 56ae c200 0051 db00 576d c200 0024 9b00  V....Q..Wm...$..
+00000210: 576d c200 0042 ef00 587a ff00 000a ae00  Wm...B..Xz......
+00000220: 587a ff00 0027 6000 587a ff00 0046 2b00  Xz...'`.Xz...F+.
+00000230: 5aa8 9400 000d e600 5aa8 9400 0047 9200  Z.......Z....G..
+00000240: 5aa8 9400 0050 0500 67ab 0600 0050 cd00  Z....P..g....P..
+00000250: 6d92 9400 004e a500 753c 2300 0042 ae00  m....N..u<#..B..
+00000260: 8cd2 1500 0010 1200 aa80 2500 001a 3600  ..........%...6.
+00000270: ab72 4500 0009 cd00 bf5b b400 0005 f500  .rE......[......
+00000280: c656 de00 003b dd00 ff2c 7700 001b ff01  .V...;...,w.....
+00000290: 30ed a300 001c 9601 48c4 ff00 001a 7001  0.......H.....p.
+000002a0: 4d8a bc00 0021 5b01 5478 6c00 0021 f101  M....![.Txl..!..
+000002b0: 6bb3 1300 0045 0601 945e f800 0029 0601  k....E...^...)..
+000002c0: 9942 b500 0040 db01 9ce8 5e00 0048 5b01  .B...@....^..H[.
+000002d0: e578 e300 000d 2601 e907 4500 0041 2b01  .x....&...E..A+.
+000002e0: fdeb 5400 004b 9002 3222 f900 0037 1302  ..T..K..2"...7..
+000002f0: 33a9 3400 0008 f902 e7d6 5e00 0002 4102  3.4.......^...A.
+00000300: e7d6 5e00 0015 5b02 e7d6 5e00 0038 4102  ..^...[...^..8A.
+00000310: e81d 2400 003c a803 004d 1200 000c 2d03  ..$..<...M....-.
+00000320: 0149 e600 0021 1303 0cac 0500 000f 9c03  .I...!..........
+00000330: 0f6b 1200 0042 2d03 0f6b 3200 0023 8c03  .k...B-..k2..#..
+00000340: 1bec 1200 0013 ae03 4485 3000 0000 1e03  ........D.0.....
+00000350: 45b3 3000 0000 5e03 4ecb 9200 0033 e203  E.0...^.N....3..
+00000360: 4ecb 9200 0050 2703 533f be00 0052 0403  N....P'.S?...R..
+00000370: 598b 3200 0007 f703 598b 3200 0020 c103  Y.2.....Y.2.. ..
+00000380: 598b 3200 003f 9603 6cc3 0400 000b c503  Y.2..?..l.......
+00000390: 881f d400 0006 1e03 9ce3 f400 001e 1203  ................
+000003a0: 9ce9 a500 0025 0d03 f5e0 0700 002d 6b04  .....%.......-k.
+000003b0: 07f6 ee00 0024 4c04 07f6 ee00 0041 e004  .....$L......A..
+000003c0: 2b4e 0500 001d 3f04 6c90 3200 003f b904  +N....?.l.2..?..
+000003d0: 8c96 8100 0014 2f04 8caf 6200 0014 7904  ....../...b...y.
+000003e0: 9c8b 8500 0037 d804 a472 8400 002b 1a04  .....7...r...+..
+000003f0: ab8e f500 002f bb04 ab8e fc00 002f e004  ...../......./..
+00000400: ab8f 0100 0030 0504 ab8f 0700 0030 2a04  .....0.......0*.
+00000410: ab8f 0800 0030 4f04 b08b a400 003c 3504  .....0O......<5.
+00000420: b2b6 6400 0008 6b04 c4a9 a900 0013 1604  ..d...k.........
+00000430: cf76 9400 0004 7104 cf76 9400 0031 5104  .v....q..v...1Q.
+00000440: e826 8800 0005 d404 e826 8800 001d 7c04  .&.......&....|.
+00000450: e826 8800 003e 5304 e842 f200 001d a004  .&...>S..B......
+00000460: e842 f200 004f 1b04 edd3 6400 0036 2904  .B...O....d..6).
+00000470: f5b6 e700 002a 0a05 0476 9400 0032 1405  .....*...v...2..
+00000480: 1f06 1500 004f 3e05 3268 c400 0003 f505  .....O>.2h......
+00000490: 34db 8200 0021 a905 3ddf a300 000a ce05  4....!..=.......
+000004a0: 4466 8200 0046 ce05 5776 4500 0043 d305  Df...F..WvE..C..
+000004b0: 6336 9e00 0032 7d05 647d 0e00 002f 6705  c6...2}.d}.../g.
+000004c0: 7865 9800 0045 6905 7865 b800 0045 8b05  xe...Ei.xe...E..
+000004d0: afca f400 0040 8505 c7f7 2800 0052 6805  .....@....(..Rh.
+000004e0: c984 e900 0030 7406 011e c400 0002 7906  .....0t.......y.
+000004f0: 43c1 1300 0016 8b06 778d 0800 0006 cd06  C.......w.......
+00000500: 778d 0800 001e f406 7e7c a100 0025 f606  w.......~|...%..
+00000510: 7e7c a100 0044 9906 830d be00 0029 c406  ~|...D.......)..
+00000520: bdf0 a400 0019 6206 be94 d200 0050 8b06  ......b......P..
+00000530: d2af d900 0052 9206 db4d 4200 0027 c506  .....R...MB..'..
+00000540: e056 d800 0024 1106 e056 d800 0041 a706  .V...$...V...A..
+00000550: f895 8e00 0015 c507 2f4a 1500 0047 f907  ......../J...G..
+00000560: 357f 7400 004a 1207 366b 9300 0004 f707  5.t..J..6k......
+00000570: 50be 3900 0051 2b07 68f8 4400 004c 3c07  P.9..Q+.h.D..L<.
+00000580: 693d fe00 0031 7607 6941 4e00 0032 3907  i=...1v.iAN..29.
+00000590: 6cbb 6300 000e 4707 8f3a 3e00 0024 ce07  l.c...G..:>..$..
+000005a0: 8f3a 3e00 0043 2007 e67a d700 0030 c107  .:>..C ..z...0..
+000005b0: e76d c800 0025 5007 e78f a400 0025 8607  .m...%P......%..
+000005c0: e79f 3400 0025 be07 e79f 3400 0044 5d07  ..4..%....4..D].
+000005d0: e7e0 a400 002e 1507 e7f2 3400 002e 5007  ..........4...P.
+000005e0: e7f2 3400 004b d508 14d3 ed00 0032 be08  ..4..K.......2..
+000005f0: 14d3 ed00 0044 ca08 3292 cb00 0038 7a08  .....D..2....8z.
+00000600: 3587 6a00 002b 7908 36b6 5400 0012 5a08  5.j..+y.6.T...Z.
+00000610: 5ac5 0100 0001 9408 5ac5 0100 0013 fc08  Z.......Z.......
+00000620: 5ac5 0100 0036 e208 678f b400 0026 f208  Z....6..g....&..
+00000630: 679f 2400 0027 2a08 679f 2400 0045 ef08  g.$..'*.g.$..E..
+00000640: 7f52 2500 002a b908 8879 1400 0018 f408  .R%..*...y......
+00000650: aae3 e400 0009 9a08 b63d de00 0034 d008  .........=...4..
+00000660: bd74 5e00 0022 d208 d39b 6400 003f 1008  .t^.."....d..?..
+00000670: f89a cb00 0035 a309 14be 9200 0047 2609  .....5.......G&.
+00000680: 1c52 9500 002d ca09 238c 7500 0016 c509  .R...-..#.u.....
+00000690: 3f8c ad00 000c aa09 564e 4200 0049 7b09  ?.......VNB..I{.
+000006a0: 6c61 f400 0013 7a09 6c61 f400 002e ea09  la....z.la......
+000006b0: 6fe6 7e00 0011 5e09 8fa3 8700 002f 1f09  o.~...^....../..
+000006c0: 97c9 1400 0020 8609 97c9 1400 003f 5509  ..... .......?U.
+000006d0: 97d9 8400 0020 4b09 9c7f 1a00 0036 a809  ..... K......6..
+000006e0: a118 8500 0010 dd09 c004 d700 0003 bc09  ................
+000006f0: c4e8 d700 0001 c409 c8df a200 001e 6709  ..............g.
+00000700: c943 f500 000f d709 e854 fc00 0015 9609  .C.......T......
+00000710: e854 fc00 0039 c709 f42c fb00 001b 510a  .T...9...,....Q.
+00000720: 2087 bc00 003a a50a 2190 e200 0006 840a   ....:..!.......
+00000730: 2190 e200 001e a80a 3f0e 9500 0028 bd0a  !.......?....(..
+00000740: 5e68 d900 0026 4a0a 6789 3b00 0007 0c0a  ^h...&J.g.;.....
+00000750: 6789 3b00 001f 360a 67a9 0200 0007 480a  g.;...6.g.....H.
+00000760: 67a9 0200 001f 750a 6dc8 3e00 0034 690a  g.....u.m.>..4i.
+00000770: 7833 e400 0038 020a 7d6b 2400 0018 280a  x3...8..}k$...(.
+00000780: 92a2 e500 0029 700a 9612 e500 0028 630a  .....)p......(c.
+00000790: a8b0 0e00 000e 060a a8b0 0e00 0047 b30a  .............G..
+000007a0: acdb 7e00 0002 1c0a b945 f500 002a f50a  ..~......E...*..
+000007b0: b945 f500 0047 d60a c389 2500 0028 2c0a  .E...G....%..(,.
+000007c0: c5b4 4900 003e 750a c897 c500 0006 460a  ..I..>u.......F.
+000007d0: d2f0 b500 0002 e60a d382 7700 0003 340a  ..........w...4.
+000007e0: e2b5 9600 0004 920a f31c 2200 003a 310b  .........."..:1.
+000007f0: 1562 0700 004c c10b 1805 3900 0015 0b0b  .b...L....9.....
+00000800: 4597 5500 0008 190b 5d8a f400 001f b40b  E.U.....].......
+00000810: 6628 d200 0034 270b 7fe2 de00 0032 fd0b  f(...4'......2..
+00000820: ad17 7800 001b 230b ff25 ce00 001c 510c  ..x...#..%....Q.
+00000830: 08f5 6c00 003c 630c 107d 9300 0003 7e0c  ..l..<c..}....~.
+00000840: 10ba b200 0027 830c 1415 6300 003e 2f0c  .....'....c..>/.
+00000850: 1536 f700 002c ec0c 1f2f 0200 0049 cc0c  .6...,.../...I..
+00000860: 29f2 a400 004c 9b0c 6a19 e900 003b 8e0c  )....L..j....;..
+00000870: 8c09 2900 001d 080c 8c09 2900 003d fa0c  ..).......)..=..
+00000880: 9688 9500 0014 530c a3fa 5f00 0019 f80c  ......S..._.....
+00000890: a6e8 d400 0039 0b0c bb01 7300 000c 6d0c  .....9....s...m.
+000008a0: bb01 7300 0033 540c c9a0 0e00 002d 460d  ..s..3T......-F.
+000008b0: 0218 6400 0046 7e0d 07a4 f800 0039 f40d  ..d..F~......9..
+000008c0: 1f27 b200 0014 a70d 3504 b400 0039 670d  .'......5....9g.
+000008d0: 76f7 5900 001b a60d 825f 7300 000e ea0d  v.Y......_s.....
+000008e0: a03c 1200 004d 930d d0ff 4c00 002c a00d  .<...M....L..,..
+000008f0: f2ea c200 003a eb0d fe4e 2400 0019 ab0d  .....:...N$.....
+00000900: fe4e 2400 004e 590e 0543 5500 0023 d30e  .N$..NY..CU..#..
+00000910: 05d1 b500 004d f20e 0743 5500 0042 720e  .....M...CU..Br.
+00000920: 233d d500 004a 4c0e 87ac 6400 001f fd0e  #=...JL...d.....
+00000930: 93fa 5200 0017 6a0e a32f e400 003d ab0e  ..R...j../...=..
+00000940: c497 a200 000b 3c0e c72a a600 0005 5f0e  ......<..*...._.
+00000950: de3d a200 0038 9e0e e46b 3400 0045 ad0e  .=...8...k4..E..
+00000960: fdeb 3400 0044 1b0f 165e c400 0043 840f  ..4..D...^...C..
+00000970: 3562 ce00 0017 cb0f 6963 bc00 000c ef0f  5b......ic......
+00000980: 6963 bc00 002a 7f0f 6963 bc00 004f cc0f  ic...*..ic...O..
+00000990: 6978 c700 0033 950f 6c98 6c00 0051 b00f  ix...3..l.l..Q..
+000009a0: 7ddd 2800 004a f40f 8007 d400 0037 520f  }.(..J.......7R.
+000009b0: 8313 8900 0012 e30f cb15 5200 0018 aa0f  ..........R.....
+000009c0: e6f6 3400 003e 9d69 0000 52bc 03ff ffff  ..4..>.i..R.....
+000009d0: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
 000009e0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-000009f0: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
-00000a00: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000a10: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
-00000a20: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000a30: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
-00000a40: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000a50: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
-00000a60: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000a70: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
-00000a80: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00000a90: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
-00000aa0: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
-00000ab0: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
-00000ac0: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
-00000ad0: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
-00000ae0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
-00000af0: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
-00000b00: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000b10: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
+000009f0: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
+00000a00: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000a10: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
+00000a20: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000a30: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
+00000a40: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000a50: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
+00000a60: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000a70: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
+00000a80: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000a90: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
+00000aa0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000ab0: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
+00000ac0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000ad0: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
+00000ae0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000af0: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
+00000b00: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000b10: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
 00000b20: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000b30: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
-00000b40: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
-00000b50: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
-00000b60: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
-00000b70: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
-00000b80: 616c 6f67 0103 0000 0038 005a 0065 0072  alog.....8.Z.e.r
-00000b90: 0074 0069 0066 0069 006b 0061 0074 0020  .t.i.f.i.k.a.t. 
-00000ba0: 0062 0065 006e 00f6 0074 0069 0067 0074  .b.e.n...t.i.g.t
-00000bb0: 0020 0050 0061 0073 0073 0077 006f 0072  . .P.a.s.s.w.o.r
-00000bc0: 0074 0800 0000 0006 0000 001a 4365 7274  .t..........Cert
-00000bd0: 6966 6963 6174 6520 6e65 6564 7320 7061  ificate needs pa
-00000be0: 7373 776f 7264 0700 0000 0644 6961 6c6f  ssword.....Dialo
-00000bf0: 6701 0300 0000 2400 5300 7000 6100 6c00  g.....$.S.p.a.l.
-00000c00: 7400 6500 6e00 2000 7600 6500 7200 7300  t.e.n. .v.e.r.s.
-00000c10: 7400 6500 6300 6b00 6500 6e08 0000 0000  t.e.c.k.e.n.....
-00000c20: 0600 0000 0f43 6f6c 756d 6e73 2074 6f20  .....Columns to 
-00000c30: 6869 6465 0700 0000 0644 6961 6c6f 6701  hide.....Dialog.
-00000c40: 0300 0000 2000 5300 7000 6100 6c00 7400  .... .S.p.a.l.t.
-00000c50: 6500 6e00 2000 6100 6e00 7a00 6500 6900  e.n. .a.n.z.e.i.
-00000c60: 6700 6500 6e08 0000 0000 0600 0000 0f43  g.e.n..........C
-00000c70: 6f6c 756d 6e73 2074 6f20 7368 6f77 0700  olumns to show..
-00000c80: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
-00000c90: 4100 6e00 6d00 6500 6c00 6400 6500 6400  A.n.m.e.l.d.e.d.
-00000ca0: 6100 7400 6500 6e08 0000 0000 0600 0000  a.t.e.n.........
-00000cb0: 0b43 7265 6465 6e74 6961 6c73 0700 0000  .Credentials....
-00000cc0: 0644 6961 6c6f 6701 0300 0000 1400 4100  .Dialog.......A.
-00000cd0: 6200 7300 7400 6500 6900 6700 6500 6e00  b.s.t.e.i.g.e.n.
-00000ce0: 6408 0000 0000 0600 0000 0a44 6573 6365  d..........Desce
-00000cf0: 6e64 696e 6707 0000 0006 4469 616c 6f67  nding.....Dialog
-00000d00: 0103 0000 003e 0057 0069 0072 006b 0073  .....>.W.i.r.k.s
-00000d10: 0061 006d 0020 006e 0061 0063 0068 0020  .a.m. .n.a.c.h. 
-00000d20: 0041 006e 0077 0065 006e 0064 0075 006e  .A.n.w.e.n.d.u.n
-00000d30: 0067 0073 006e 0065 0075 0073 0074 0061  .g.s.n.e.u.s.t.a
-00000d40: 0072 0074 0800 0000 0006 0000 0023 4566  .r.t.........#Ef
-00000d50: 6665 6374 6976 6520 6166 7465 7220 6170  fective after ap
-00000d60: 706c 6963 6174 696f 6e20 7265 7374 6172  plication restar
-00000d70: 7407 0000 0006 4469 616c 6f67 0103 ffff  t.....Dialog....
-00000d80: ffff 0800 0000 0006 0000 0006 4578 706f  ............Expo
-00000d90: 7274 0700 0000 0644 6961 6c6f 6701 0300  rt.....Dialog...
-00000da0: 0000 3400 4500 7800 7000 6f00 7200 7400  ..4.E.x.p.o.r.t.
-00000db0: 6900 6500 7200 6500 2000 4300 4200 2d00  i.e.r.e. .C.B.-.
-00000dc0: 5100 5300 4f00 7300 2000 6900 6e00 2000  Q.S.O.s. .i.n. .
-00000dd0: 4100 4400 4900 4608 0000 0000 0600 0000  A.D.I.F.........
-00000de0: 1645 7870 6f72 7420 4342 2051 534f 7320  .Export CB QSOs 
-00000df0: 746f 2041 4449 4607 0000 0006 4469 616c  to ADIF.....Dial
-00000e00: 6f67 0103 0000 0036 0045 0078 0070 006f  og.....6.E.x.p.o
-00000e10: 0072 0074 0069 0065 0072 0065 0020 006e  .r.t.i.e.r.e. .n
-00000e20: 0075 0072 0020 006e 0065 0075 0065 0073  .u.r. .n.e.u.e.s
-00000e30: 0074 0065 0020 0051 0053 004f 0073 0800  .t.e. .Q.S.O.s..
-00000e40: 0000 0006 0000 0017 4578 706f 7274 206f  ........Export o
-00000e50: 6e6c 7920 7265 6365 6e74 2051 534f 7307  nly recent QSOs.
-00000e60: 0000 0006 4469 616c 6f67 0103 0000 0042  ....Dialog.....B
-00000e70: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
-00000e80: 0072 0065 0020 0065 0069 0067 0065 006e  .r.e. .e.i.g.e.n
-00000e90: 0065 0020 004e 006f 0074 0069 007a 0065  .e. .N.o.t.i.z.e
-00000ea0: 006e 0020 0069 006e 0020 0041 0044 0049  .n. .i.n. .A.D.I
-00000eb0: 0046 0800 0000 0006 0000 0018 4578 706f  .F..........Expo
-00000ec0: 7274 206f 776e 206e 6f74 6573 2074 6f20  rt own notes to 
-00000ed0: 4144 4946 0700 0000 0644 6961 6c6f 6701  ADIF.....Dialog.
-00000ee0: 03ff ffff ff08 0000 0000 0600 0000 0648  ...............H
-00000ef0: 616d 5154 4807 0000 0006 4469 616c 6f67  amQTH.....Dialog
-00000f00: 0103 ffff ffff 0800 0000 0006 0000 000e  ................
-00000f10: 4861 6d6c 6962 2072 6967 6374 6c64 0700  Hamlib rigctld..
-00000f20: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000f30: 0000 0000 0600 0000 0d49 6d70 6f72 742f  .........Import/
-00000f40: 4578 706f 7274 0700 0000 0644 6961 6c6f  Export.....Dialo
-00000f50: 6701 0300 0000 1a00 5300 6300 6800 6e00  g.......S.c.h.n.
-00000f60: 6900 7400 7400 7300 7400 6500 6c00 6c00  i.t.t.s.t.e.l.l.
-00000f70: 6508 0000 0000 0600 0000 0949 6e74 6572  e..........Inter
-00000f80: 6661 6365 0700 0000 0644 6961 6c6f 6701  face.....Dialog.
-00000f90: 0300 0000 2000 6c00 6500 7400 7a00 7400  .... .l.e.t.z.t.
-00000fa0: 6500 7300 2000 4800 6100 6c00 6200 6a00  e.s. .H.a.l.b.j.
-00000fb0: 6100 6800 7208 0000 0000 0600 0000 0e4c  a.h.r..........L
-00000fc0: 6173 7420 6861 6c66 2079 6561 7207 0000  ast half year...
-00000fd0: 0006 4469 616c 6f67 0103 0000 001a 006c  ..Dialog.......l
-00000fe0: 0065 0074 007a 0074 0065 006e 0020 004d  .e.t.z.t.e.n. .M
-00000ff0: 006f 006e 0061 0074 0800 0000 0006 0000  .o.n.a.t........
-00001000: 000a 4c61 7374 206d 6f6e 7468 0700 0000  ..Last month....
-00001010: 0644 6961 6c6f 6701 0300 0000 1800 6c00  .Dialog.......l.
-00001020: 6500 7400 7a00 7400 6500 2000 5700 6f00  e.t.z.t.e. .W.o.
-00001030: 6300 6800 6508 0000 0000 0600 0000 094c  c.h.e..........L
-00001040: 6173 7420 7765 656b 0700 0000 0644 6961  ast week.....Dia
-00001050: 6c6f 6701 0300 0000 1800 6c00 6500 7400  log.......l.e.t.
-00001060: 7a00 7400 6500 7300 2000 4a00 6100 6800  z.t.e.s. .J.a.h.
-00001070: 7208 0000 0000 0600 0000 094c 6173 7420  r..........Last 
-00001080: 7965 6172 0700 0000 0644 6961 6c6f 6701  year.....Dialog.
-00001090: 0300 0000 0c00 4200 7200 6500 6900 7400  ......B.r.e.i.t.
-000010a0: 6508 0000 0000 0600 0000 034c 6174 0700  e..........Lat..
-000010b0: 0000 0644 6961 6c6f 6701 0300 0000 0a00  ...Dialog.......
-000010c0: 5300 7400 7500 6600 6508 0000 0000 0600  S.t.u.f.e.......
-000010d0: 0000 054c 6576 656c 0700 0000 0644 6961  ...Level.....Dia
-000010e0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-000010f0: 0000 044c 6f54 5707 0000 0006 4469 616c  ...LoTW.....Dial
-00001100: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00001110: 0007 4c6f 6361 746f 7207 0000 0006 4469  ..Locator.....Di
-00001120: 616c 6f67 0103 0000 002c 004c 006f 0067  alog.....,.L.o.g
-00001130: 0020 0069 006e 0020 0044 0061 0074 0065  . .i.n. .D.a.t.e
-00001140: 0069 0020 0073 0063 0068 0072 0065 0069  .i. .s.c.h.r.e.i
-00001150: 0062 0065 006e 0800 0000 0006 0000 000b  .b.e.n..........
-00001160: 4c6f 6720 746f 2066 696c 6507 0000 0006  Log to file.....
-00001170: 4469 616c 6f67 0103 0000 001e 004c 006f  Dialog.......L.o
-00001180: 0067 0067 0069 006e 0067 002d 0041 0075  .g.g.i.n.g.-.A.u
-00001190: 0073 0067 0061 0062 0065 0800 0000 0006  .s.g.a.b.e......
-000011a0: 0000 000e 4c6f 6767 696e 6720 6f75 7470  ....Logging outp
-000011b0: 7574 0700 0000 0644 6961 6c6f 6701 0300  ut.....Dialog...
-000011c0: 0000 0a00 4c00 e400 6e00 6700 6508 0000  ....L...n.g.e...
-000011d0: 0000 0600 0000 034c 6f6e 0700 0000 0644  .......Lon.....D
-000011e0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-000011f0: 0600 0000 044e 616d 6507 0000 0006 4469  .....Name.....Di
-00001200: 616c 6f67 0103 0000 005e 0043 0042 0020  alog.....^.C.B. 
-00001210: 0051 0053 004f 0073 0020 0077 0065 0072  .Q.S.O.s. .w.e.r
-00001220: 0064 0065 006e 0020 0062 0065 0069 006d  .d.e.n. .b.e.i.m
-00001230: 0020 0049 006d 0070 006f 0072 0074 0020  . .I.m.p.o.r.t. 
-00001240: 0069 006d 006d 0065 0072 0020 0062 0065  .i.m.m.e.r. .b.e
-00001250: 0072 00fc 0063 006b 0073 0069 0063 0068  .r...c.k.s.i.c.h
-00001260: 0074 0069 0067 0074 0800 0000 0006 0000  .t.i.g.t........
-00001270: 0028 4f6e 2069 6d70 6f72 7420 4342 2051  .(On import CB Q
-00001280: 534f 7320 7769 6c6c 2061 6c77 6179 7320  SOs will always 
-00001290: 6265 2068 616e 646c 6564 0700 0000 0644  be handled.....D
-000012a0: 6961 6c6f 6701 0300 0000 1000 5000 6100  ialog.......P.a.
-000012b0: 7300 7300 7700 6f00 7200 7408 0000 0000  s.s.w.o.r.t.....
-000012c0: 0600 0000 0850 6173 7377 6f72 6407 0000  .....Password...
-000012d0: 0006 4469 616c 6f67 0103 0000 0070 0050  ..Dialog.....p.P
-000012e0: 0061 0073 0073 0077 006f 0072 0074 0020  .a.s.s.w.o.r.t. 
-000012f0: 0064 0065 0073 0020 004c 006f 0054 0057  .d.e.s. .L.o.T.W
-00001300: 002d 004f 006e 006c 0069 006e 0065 002d  .-.O.n.l.i.n.e.-
-00001310: 0041 0063 0063 006f 0075 006e 0074 0073  .A.c.c.o.u.n.t.s
-00001320: 002c 0020 006e 0069 0063 0068 0074 0020  .,. .n.i.c.h.t. 
-00001330: 0064 0065 0073 0020 005a 0065 0072 0074  .d.e.s. .Z.e.r.t
-00001340: 0069 0066 0069 006b 0061 0074 0073 0800  .i.f.i.k.a.t.s..
-00001350: 0000 0006 0000 0038 5061 7373 776f 7264  .......8Password
-00001360: 2066 6f72 204c 6f54 5720 6f6e 6c69 6e65   for LoTW online
-00001370: 2061 6363 6f75 6e74 206e 6f74 2066 6f72   account not for
-00001380: 2074 6865 2063 6572 7469 6669 6361 7465   the certificate
-00001390: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
-000013a0: ff08 0000 0000 0600 0000 0351 5448 0700  ...........QTH..
-000013b0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-000013c0: 0000 0000 0600 0000 0552 6164 696f 0700  .........Radio..
-000013d0: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
-000013e0: 4e00 6500 7500 6500 7300 7400 6500 2000  N.e.u.e.s.t.e. .
-000013f0: 5100 5300 4f00 7308 0000 0000 0600 0000  Q.S.O.s.........
-00001400: 0b52 6563 656e 7420 5153 4f73 0700 0000  .Recent QSOs....
-00001410: 0644 6961 6c6f 6701 0300 0000 1200 4600  .Dialog.......F.
-00001420: 7500 6e00 6b00 6700 6500 7200 e400 7408  u.n.k.g.e.r...t.
-00001430: 0000 0000 0600 0000 0352 6967 0700 0000  .........Rig....
-00001440: 0644 6961 6c6f 6701 0300 0000 4c00 5300  .Dialog.....L.S.
-00001450: 6900 6500 6800 6500 2000 4500 6900 6e00  i.e.h.e. .E.i.n.
-00001460: 7300 7400 6500 6c00 6c00 7500 6e00 6700  s.t.e.l.l.u.n.g.
-00001470: 6500 6e00 2000 5200 6500 6900 7400 6500  e.n. .R.e.i.t.e.
-00001480: 7200 2000 2200 4100 6e00 7700 6500 6e00  r. .".A.n.w.e.n.
-00001490: 6400 7500 6e00 6700 2208 0000 0000 0600  d.u.n.g.".......
-000014a0: 0000 2253 6565 2073 6574 7469 6e67 7320  .."See settings 
-000014b0: 7061 6765 2022 5573 6572 2069 6e74 6572  page "User inter
-000014c0: 6661 6365 2207 0000 0006 4469 616c 6f67  face".....Dialog
-000014d0: 0103 0000 0034 0043 0042 002d 0042 0061  .....4.C.B.-.B.a
-000014e0: 006e 0064 0020 0061 0075 0074 006f 006d  .n.d. .a.u.t.o.m
-000014f0: 0061 0074 0069 0073 0063 0068 0020 0077  .a.t.i.s.c.h. .w
-00001500: 00e4 0068 006c 0065 006e 0800 0000 0006  ...h.l.e.n......
-00001510: 0000 0019 5365 6c65 6374 2043 4220 6261  ....Select CB ba
-00001520: 6e64 2062 7920 6465 6661 756c 7407 0000  nd by default...
-00001530: 0006 4469 616c 6f67 0103 0000 001a 0053  ..Dialog.......S
-00001540: 0065 0074 007a 0065 0020 004c 006f 0063  .e.t.z.e. .L.o.c
-00001550: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
-00001560: 000b 5365 7420 6c6f 6361 746f 7207 0000  ..Set locator...
-00001570: 0006 4469 616c 6f67 0103 0000 001a 0045  ..Dialog.......E
-00001580: 0069 006e 0073 0074 0065 006c 006c 0075  .i.n.s.t.e.l.l.u
-00001590: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
-000015a0: 0008 5365 7474 696e 6773 0700 0000 0644  ..Settings.....D
-000015b0: 6961 6c6f 6701 0300 0000 1c00 5a00 6500  ialog.......Z.e.
-000015c0: 6900 6700 6500 2000 5100 5300 4f00 7300  i.g.e. .Q.S.O.s.
-000015d0: 2000 6600 fc00 7208 0000 0000 0600 0000   .f...r.........
-000015e0: 0e53 686f 7720 5153 4f73 2066 726f 6d07  .Show QSOs from.
-000015f0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
-00001600: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
-00001610: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
-00001620: 6f77 2061 6c6c 0700 0000 0644 6961 6c6f  ow all.....Dialo
-00001630: 6701 0300 0000 4000 5300 7000 6100 6c00  g.....@.S.p.a.l.
-00001640: 7400 6500 6e00 2000 6100 6e00 7a00 6500  t.e.n. .a.n.z.e.
-00001650: 6900 6700 6500 6e00 2000 6f00 6400 6500  i.g.e.n. .o.d.e.
-00001660: 7200 2000 7600 6500 7200 7300 7400 6500  r. .v.e.r.s.t.e.
-00001670: 6300 6b00 6500 6e08 0000 0000 0600 0000  c.k.e.n.........
-00001680: 1453 686f 7720 6f72 2068 6964 6520 636f  .Show or hide co
-00001690: 6c75 6d6e 7307 0000 0006 4469 616c 6f67  lumns.....Dialog
-000016a0: 0103 0000 0028 0053 006f 0072 0074 0069  .....(.S.o.r.t.i
-000016b0: 0065 0072 0065 0020 006e 0061 0063 0068  .e.r.e. .n.a.c.h
-000016c0: 0020 0053 0070 0061 006c 0074 0065 0800  . .S.p.a.l.t.e..
-000016d0: 0000 0006 0000 000e 536f 7274 206f 6e20  ........Sort on 
-000016e0: 636f 6c75 6d6e 0700 0000 0644 6961 6c6f  column.....Dialo
-000016f0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001700: 0553 7461 7274 0700 0000 0644 6961 6c6f  .Start.....Dialo
-00001710: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001720: 0753 7461 7469 6f6e 0700 0000 0644 6961  .Station.....Dia
-00001730: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00001740: 0000 0454 5153 4c07 0000 0006 4469 616c  ...TQSL.....Dial
-00001750: 6f67 0103 0000 0064 0056 0065 0072 0077  og.....d.V.e.r.w
-00001760: 0065 006e 0064 0065 0020 0064 0069 0065  .e.n.d.e. .d.i.e
-00001770: 0020 006b 006f 006e 0066 0069 0067 0075  . .k.o.n.f.i.g.u
-00001780: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
-00001790: 0044 0020 0062 0065 0069 0020 0066 0065  .D. .b.e.i. .f.e
-000017a0: 0068 006c 0065 006e 0064 0065 006e 0020  .h.l.e.n.d.e.n. 
-000017b0: 0057 0065 0072 0074 0065 006e 0800 0000  .W.e.r.t.e.n....
-000017c0: 0006 0000 0024 5573 6520 636f 6e66 6967  .....$Use config
-000017d0: 7572 6564 2049 4420 666f 7220 6d69 7373  ured ID for miss
-000017e0: 696e 6720 7661 6c75 6573 0700 0000 0644  ing values.....D
-000017f0: 6961 6c6f 6701 0300 0000 6e00 5600 6500  ialog.....n.V.e.
-00001800: 7200 7700 6500 6e00 6400 6500 2000 6400  r.w.e.n.d.e. .d.
-00001810: 6900 6500 2000 6b00 6f00 6e00 6600 6900  i.e. .k.o.n.f.i.
-00001820: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
-00001830: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
-00001840: 2000 6200 6500 6900 2000 6600 6500 6800   .b.e.i. .f.e.h.
-00001850: 6c00 6500 6e00 6400 6500 6e00 2000 5700  l.e.n.d.e.n. .W.
-00001860: 6500 7200 7400 6500 6e08 0000 0000 0600  e.r.t.e.n.......
-00001870: 0000 2955 7365 2063 6f6e 6669 6775 7265  ..)Use configure
-00001880: 6420 5374 6174 696f 6e20 666f 7220 6d69  d Station for mi
-00001890: 7373 696e 6720 7661 6c75 6573 0700 0000  ssing values....
-000018a0: 0644 6961 6c6f 6701 0300 0000 1200 4100  .Dialog.......A.
-000018b0: 6e00 7700 6500 6e00 6400 7500 6e00 6708  n.w.e.n.d.u.n.g.
-000018c0: 0000 0000 0600 0000 0e55 7365 7220 696e  .........User in
-000018d0: 7465 7266 6163 6507 0000 0006 4469 616c  terface.....Dial
-000018e0: 6f67 0103 0000 0018 0042 0065 006e 0075  og.......B.e.n.u
-000018f0: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
-00001900: 0800 0000 0006 0000 0008 5573 6572 6e61  ..........Userna
-00001910: 6d65 0700 0000 0644 6961 6c6f 6701 0300  me.....Dialog...
-00001920: 0000 7800 4200 6500 6e00 7500 7400 7a00  ..x.B.e.n.u.t.z.
-00001930: 6500 7200 6e00 6100 6d00 6500 2000 6400  e.r.n.a.m.e. .d.
-00001940: 6500 7300 2000 4c00 6f00 5400 5700 2d00  e.s. .L.o.T.W.-.
-00001950: 4f00 6e00 6c00 6900 6e00 6500 2d00 4100  O.n.l.i.n.e.-.A.
-00001960: 6300 6300 6f00 7500 6e00 7400 7300 2c00  c.c.o.u.n.t.s.,.
-00001970: 2000 6e00 6900 6300 6800 7400 2000 6400   .n.i.c.h.t. .d.
-00001980: 6500 7300 2000 5a00 6500 7200 7400 6900  e.s. .Z.e.r.t.i.
-00001990: 6600 6900 6b00 6100 7400 7308 0000 0000  f.i.k.a.t.s.....
-000019a0: 0600 0000 3855 7365 726e 616d 6520 666f  ....8Username fo
-000019b0: 7220 4c6f 5457 206f 6e6c 696e 6520 6163  r LoTW online ac
-000019c0: 636f 756e 7420 6e6f 7420 666f 7220 7468  count not for th
-000019d0: 6520 6365 7274 6966 6963 6174 6507 0000  e certificate...
-000019e0: 0006 4469 616c 6f67 0103 0000 0020 0044  ..Dialog..... .D
-000019f0: 0061 0074 0065 0069 00fc 0062 0065 0072  .a.t.e.i...b.e.r
-00001a00: 0077 0061 0063 0068 0075 006e 0067 0800  .w.a.c.h.u.n.g..
-00001a10: 0000 0006 0000 000a 5761 7463 6820 4669  ........Watch Fi
-00001a20: 6c65 0700 0000 0644 6961 6c6f 6701 03ff  le.....Dialog...
-00001a30: ffff ff08 0000 0000 0600 0000 0465 5153  .............eQS
-00001a40: 4c07 0000 0006 4469 616c 6f67 0103 ffff  L.....Dialog....
-00001a50: ffff 0800 0000 0006 0000 0002 c2b0 0700  ................
-00001a60: 0000 0644 6961 6c6f 6701 0300 0000 9e00  ...Dialog.......
-00001a70: 4500 6900 6e00 2000 4400 6100 7400 6500  E.i.n. .D.a.t.e.
-00001a80: 6e00 6200 6100 6e00 6b00 2d00 4200 6100  n.b.a.n.k.-.B.a.
-00001a90: 6300 6b00 7500 7000 2000 6b00 6f00 6e00  c.k.u.p. .k.o.n.
-00001aa0: 6e00 7400 6500 2000 6e00 6900 6300 6800  n.t.e. .n.i.c.h.
-00001ab0: 7400 2000 6500 7200 7300 7400 6500 6c00  t. .e.r.s.t.e.l.
-00001ac0: 6c00 7400 2000 7700 6500 7200 6400 6500  l.t. .w.e.r.d.e.
-00001ad0: 6e00 2e00 0a00 4400 6900 6500 2000 4400  n.....D.i.e. .D.
-00001ae0: 6100 7400 6500 6900 2000 6500 7800 6900  a.t.e.i. .e.x.i.
-00001af0: 7300 7400 6900 6500 7200 7400 2000 6200  s.t.i.e.r.t. .b.
-00001b00: 6500 7200 6500 6900 7400 7300 2e08 0000  e.r.e.i.t.s.....
-00001b10: 0000 0600 0000 4041 2064 6174 6162 6173  ......@A databas
-00001b20: 6520 6261 636b 7570 2063 6f75 6c64 206e  e backup could n
-00001b30: 6f74 2062 6520 6372 6561 7465 642e 0a54  ot be created..T
-00001b40: 6865 2066 696c 6520 616c 7265 6164 7920  he file already 
-00001b50: 6578 6973 7473 2e07 0000 0009 4472 6167  exists......Drag
-00001b60: 6f6e 4c6f 6701 0300 0000 4e00 4500 6900  onLog.....N.E.i.
-00001b70: 6e00 2000 4100 4400 4900 4600 2d00 4600  n. .A.D.I.F.-.F.
-00001b80: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
-00001b90: 7400 2000 6600 fc00 7200 2000 6400 6500  t. .f...r. .d.e.
-00001ba0: 6e00 2000 4c00 6f00 5400 5700 2d00 5500  n. .L.o.T.W.-.U.
-00001bb0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
-00001bc0: 0000 1d41 2066 6965 6c64 2069 7320 6d69  ...A field is mi
-00001bd0: 7373 696e 6720 666f 7220 7570 6c6f 6164  ssing for upload
-00001be0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001bf0: ffff ffff 0800 0000 0006 0000 0015 4144  ..............AD
-00001c00: 4946 2033 2028 2a2e 6164 6920 2a2e 6164  IF 3 (*.adi *.ad
-00001c10: 6966 2907 0000 0009 4472 6167 6f6e 4c6f  if).....DragonLo
-00001c20: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001c30: 1b41 4449 4620 3320 282a 2e61 6478 202a  .ADIF 3 (*.adx *
-00001c40: 2e61 6469 202a 2e61 6469 6629 0700 0000  .adi *.adif)....
-00001c50: 0944 7261 676f 6e4c 6f67 0103 0000 0008  .DragonLog......
-00001c60: 00dc 0062 0065 0072 0800 0000 0006 0000  ...b.e.r........
-00001c70: 0005 4162 6f75 7407 0000 0009 4472 6167  ..About.....Drag
-00001c80: 6f6e 4c6f 6701 0300 0000 0e00 dc00 6200  onLog.........b.
-00001c90: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
-00001ca0: 0000 0841 626f 7574 2051 7407 0000 0009  ...About Qt.....
-00001cb0: 4472 6167 6f6e 4c6f 6701 0300 0000 0e00  DragonLog.......
-00001cc0: 4100 6e00 7400 6500 6e00 6e00 6508 0000  A.n.t.e.n.n.e...
-00001cd0: 0000 0600 0000 0741 6e74 656e 6e61 0700  .......Antenna..
-00001ce0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00001cf0: 000a 0041 0075 0074 006f 0072 0800 0000  ...A.u.t.o.r....
-00001d00: 0006 0000 0006 4175 7468 6f72 0700 0000  ......Author....
-00001d10: 0944 7261 676f 6e4c 6f67 0103 ffff ffff  .DragonLog......
-00001d20: 0800 0000 0006 0000 0004 4261 6e64 0700  ..........Band..
-00001d30: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00001d40: 0022 0043 0053 0056 002d 0044 0061 0074  .".C.S.V.-.D.a.t
-00001d50: 0065 0069 0020 0028 002a 002e 0063 0073  .e.i. .(.*...c.s
-00001d60: 0076 0029 0800 0000 0006 0000 0010 4353  .v.)..........CS
-00001d70: 562d 4669 6c65 2028 2a2e 6373 7629 0700  V-File (*.csv)..
-00001d80: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00001d90: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
-00001da0: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
-00001db0: 4361 6c6c 2073 6967 6e07 0000 0009 4472  Call sign.....Dr
-00001dc0: 6167 6f6e 4c6f 6701 0300 0000 1400 5100  agonLog.......Q.
-00001dd0: 5300 4f00 2000 e400 6e00 6400 6500 7200  S.O. ...n.d.e.r.
-00001de0: 6e08 0000 0000 0600 0000 0a43 6861 6e67  n..........Chang
-00001df0: 6520 5153 4f07 0000 0009 4472 6167 6f6e  e QSO.....Dragon
-00001e00: 4c6f 6701 0300 0000 0a00 4b00 6100 6e00  Log.......K.a.n.
-00001e10: 6100 6c08 0000 0000 0600 0000 0743 6861  a.l..........Cha
-00001e20: 6e6e 656c 0700 0000 0944 7261 676f 6e4c  nnel.....DragonL
-00001e30: 6f67 0103 0000 0074 0050 0072 00fc 0066  og.....t.P.r...f
-00001e40: 0075 006e 0067 0020 0064 0065 0072 0020  .u.n.g. .d.e.r. 
-00001e50: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
-00001e60: 006b 0020 0066 0065 0068 006c 0067 0065  .k. .f.e.h.l.g.e
-00001e70: 0073 0063 0068 006c 0061 0067 0065 006e  .s.c.h.l.a.g.e.n
-00001e80: 002e 0020 0049 006e 0068 0061 006c 0074  ... .I.n.h.a.l.t
-00001e90: 0020 006e 0069 0063 0068 0074 0020 006c  . .n.i.c.h.t. .l
-00001ea0: 0065 0073 0062 0061 0072 002e 0800 0000  .e.s.b.a.r......
-00001eb0: 0006 0000 0034 4368 6563 6b69 6e67 2064  .....4Checking d
-00001ec0: 6174 6162 6173 6520 6661 696c 6564 2e20  atabase failed. 
-00001ed0: 436f 6e74 656e 7420 6973 206e 6f74 2061  Content is not a
-00001ee0: 6363 6573 7361 626c 652e 0700 0000 0944  ccessable......D
-00001ef0: 7261 676f 6e4c 6f67 0103 0000 0014 004b  ragonLog.......K
-00001f00: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-00001f10: 0065 0800 0000 0006 0000 0008 436f 6d6d  .e..........Comm
-00001f20: 656e 7473 0700 0000 0944 7261 676f 6e4c  ents.....DragonL
-00001f30: 6f67 0103 0000 0060 0056 0065 0072 0062  og.....`.V.e.r.b
-00001f40: 0069 006e 0064 0075 006e 0067 0073 0066  .i.n.d.u.n.g.s.f
-00001f50: 0065 0068 006c 0065 0072 0020 006f 0064  .e.h.l.e.r. .o.d
-00001f60: 0065 0072 0020 004e 0065 0074 007a 0077  .e.r. .N.e.t.z.w
-00001f70: 0065 0072 006b 0020 006e 0069 0063 0068  .e.r.k. .n.i.c.h
-00001f80: 0074 0020 0065 0072 0072 0065 0069 0063  .t. .e.r.r.e.i.c
-00001f90: 0068 0062 0061 0072 0800 0000 0006 0000  .h.b.a.r........
-00001fa0: 0027 436f 6e6e 6563 7469 6f6e 2065 7272  .'Connection err
-00001fb0: 6f72 206f 7220 6e65 7477 6f72 6b20 756e  or or network un
-00001fc0: 7265 6163 6861 626c 6507 0000 0009 4472  reachable.....Dr
-00001fd0: 6167 6f6e 4c6f 6701 0300 0000 2e00 4400  agonLog.......D.
-00001fe0: 6100 7400 6500 6e00 6200 6100 6e00 6b00  a.t.e.n.b.a.n.k.
-00001ff0: 2d00 4200 6100 6300 6b00 7500 7000 2000  -.B.a.c.k.u.p. .
-00002000: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-00002010: 0600 0000 1544 6174 6162 6173 6520 6261  .....Database ba
-00002020: 636b 7570 2065 7272 6f72 0700 0000 0944  ckup error.....D
-00002030: 7261 676f 6e4c 6f67 0103 0000 002c 0044  ragonLog.....,.D
-00002040: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
-00002050: 006b 006f 006e 0076 0065 0072 0074 0069  .k.o.n.v.e.r.t.i
-00002060: 0065 0072 0075 006e 0067 0800 0000 0006  .e.r.u.n.g......
-00002070: 0000 0013 4461 7461 6261 7365 2063 6f6e  ....Database con
-00002080: 7665 7273 696f 6e07 0000 0009 4472 6167  version.....Drag
-00002090: 6f6e 4c6f 6701 0300 0000 4800 4400 6100  onLog.....H.D.a.
-000020a0: 7400 6500 6e00 6200 6100 6e00 6b00 6b00  t.e.n.b.a.n.k.k.
-000020b0: 6f00 6e00 7600 6500 7200 7400 6900 6500  o.n.v.e.r.t.i.e.
-000020c0: 7200 7500 6e00 6700 2000 6100 6200 6700  r.u.n.g. .a.b.g.
-000020d0: 6500 7300 6300 6800 6c00 6f00 7300 7300  e.s.c.h.l.o.s.s.
-000020e0: 6500 6e08 0000 0000 0600 0000 1c44 6174  e.n..........Dat
-000020f0: 6162 6173 6520 636f 6e76 6572 7369 6f6e  abase conversion
-00002100: 2066 696e 6973 6865 6407 0000 0009 4472   finished.....Dr
-00002110: 6167 6f6e 4c6f 6701 0300 0000 1e00 4400  agonLog.......D.
-00002120: 6100 7400 6500 6e00 6200 6100 6e00 6b00  a.t.e.n.b.a.n.k.
-00002130: 6600 6500 6800 6c00 6500 7208 0000 0000  f.e.h.l.e.r.....
-00002140: 0600 0000 0e44 6174 6162 6173 6520 6572  .....Database er
-00002150: 726f 7207 0000 0009 4472 6167 6f6e 4c6f  ror.....DragonLo
-00002160: 6701 0300 0000 3400 4400 6100 7400 6500  g.....4.D.a.t.e.
-00002170: 6e00 6200 6100 6e00 6b00 7300 7400 7200  n.b.a.n.k.s.t.r.
-00002180: 7500 6b00 7400 7500 7200 2000 7600 6500  u.k.t.u.r. .v.e.
-00002190: 7200 6100 6c00 7400 6500 7408 0000 0000  r.a.l.t.e.t.....
-000021a0: 0600 0000 1c44 6174 6162 6173 6520 7374  .....Database st
-000021b0: 7275 6374 7572 6520 6f75 742d 6461 7465  ructure out-date
-000021c0: 6407 0000 0009 4472 6167 6f6e 4c6f 6701  d.....DragonLog.
-000021d0: 0300 0000 1e00 4400 6100 7400 7500 6d00  ......D.a.t.u.m.
-000021e0: 2f00 5a00 6500 6900 7400 2000 4500 6e00  /.Z.e.i.t. .E.n.
-000021f0: 6400 6508 0000 0000 0600 0000 0d44 6174  d.e..........Dat
-00002200: 652f 5469 6d65 2065 6e64 0700 0000 0944  e/Time end.....D
-00002210: 7261 676f 6e4c 6f67 0103 0000 0020 0044  ragonLog..... .D
-00002220: 0061 0074 0075 006d 002f 005a 0065 0069  .a.t.u.m./.Z.e.i
-00002230: 0074 0020 0053 0074 0061 0072 0074 0800  .t. .S.t.a.r.t..
-00002240: 0000 0006 0000 000f 4461 7465 2f54 696d  ........Date/Tim
-00002250: 6520 7374 6172 7407 0000 0009 4472 6167  e start.....Drag
-00002260: 6f6e 4c6f 6701 0300 0000 1600 5100 5300  onLog.......Q.S.
-00002270: 4f00 2000 6c00 f600 7300 6300 6800 6500  O. .l...s.c.h.e.
-00002280: 6e08 0000 0000 0600 0000 0a44 656c 6574  n..........Delet
-00002290: 6520 5153 4f07 0000 0009 4472 6167 6f6e  e QSO.....Dragon
-000022a0: 4c6f 6701 0300 0000 1400 4500 6e00 7400  Log.......E.n.t.
-000022b0: 6600 6500 7200 6e00 7500 6e00 6708 0000  f.e.r.n.u.n.g...
-000022c0: 0000 0600 0000 0844 6973 7461 6e63 6507  .......Distance.
-000022d0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-000022e0: 0000 6400 5700 6f00 6c00 6c00 6500 6e00  ..d.W.o.l.l.e.n.
-000022f0: 2000 7300 6900 6500 2000 6400 6900 6500   .s.i.e. .d.i.e.
-00002300: 2000 7300 6500 6c00 6500 6b00 7400 6900   .s.e.l.e.k.t.i.
-00002310: 6500 7200 7400 6500 6e00 2000 5100 5300  e.r.t.e.n. .Q.S.
-00002320: 4f00 7300 2000 7700 6900 7200 6b00 6c00  O.s. .w.i.r.k.l.
-00002330: 6900 6300 6800 2000 6c00 f600 7300 6300  i.c.h. .l...s.c.
-00002340: 6800 6500 6e00 3f08 0000 0000 0600 0000  h.e.n.?.........
-00002350: 3144 6f20 796f 7520 7265 616c 6c79 2077  1Do you really w
-00002360: 616e 7420 746f 2064 656c 6574 6520 7468  ant to delete th
-00002370: 6520 7365 6c65 6374 6564 2051 534f 2873  e selected QSO(s
-00002380: 293f 0700 0000 0944 7261 676f 6e4c 6f67  )?.....DragonLog
-00002390: 0103 0000 000c 0046 0065 0068 006c 0065  .......F.e.h.l.e
-000023a0: 0072 0800 0000 0006 0000 0005 4572 726f  .r..........Erro
-000023b0: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
-000023c0: 0300 0000 2800 4500 7800 6300 6500 6c00  ....(.E.x.c.e.l.
-000023d0: 2d00 4400 6100 7400 6500 6900 2000 2800  -.D.a.t.e.i. .(.
-000023e0: 2a00 2e00 7800 6c00 7300 7800 2908 0000  *...x.l.s.x.)...
-000023f0: 0000 0600 0000 1345 7863 656c 2d46 696c  .......Excel-Fil
-00002400: 6520 282a 2e78 6c73 7829 0700 0000 0944  e (*.xlsx).....D
-00002410: 7261 676f 6e4c 6f67 0103 0000 0024 0045  ragonLog.....$.E
-00002420: 0078 0070 006f 0072 0074 0069 0065 0072  .x.p.o.r.t.i.e.r
-00002430: 0065 0020 0051 0053 004f 0020 006c 006f  .e. .Q.S.O. .l.o
-00002440: 0067 0800 0000 0006 0000 0010 4578 706f  .g..........Expo
-00002450: 7274 6564 2051 534f 206c 6f67 0700 0000  rted QSO log....
-00002460: 0944 7261 676f 6e4c 6f67 0103 0000 0010  .DragonLog......
-00002470: 0046 0072 0065 0071 0075 0065 006e 007a  .F.r.e.q.u.e.n.z
-00002480: 0800 0000 0006 0000 0009 4672 6571 7565  ..........Freque
-00002490: 6e63 7907 0000 0009 4472 6167 6f6e 4c6f  ncy.....DragonLo
-000024a0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-000024b0: 0648 616d 5154 4807 0000 0009 4472 6167  .HamQTH.....Drag
-000024c0: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
-000024d0: 0600 0000 0648 616d 6c69 6207 0000 0009  .....Hamlib.....
-000024e0: 4472 6167 6f6e 4c6f 6701 0300 0000 0a00  DragonLog.......
-000024f0: 4800 6900 6c00 6600 6508 0000 0000 0600  H.i.l.f.e.......
-00002500: 0000 0448 656c 7007 0000 0009 4472 6167  ...Help.....Drag
-00002510: 6f6e 4c6f 6701 0300 0000 2000 6c00 6500  onLog..... .l.e.
-00002520: 7400 7a00 7400 6500 7300 2000 4800 6100  t.z.t.e.s. .H.a.
-00002530: 6c00 6200 6a00 6100 6800 7208 0000 0000  l.b.j.a.h.r.....
-00002540: 0600 0000 0e4c 6173 7420 6861 6c66 2079  .....Last half y
-00002550: 6561 7207 0000 0009 4472 6167 6f6e 4c6f  ear.....DragonLo
-00002560: 6701 0300 0000 1a00 6c00 6500 7400 7a00  g.......l.e.t.z.
-00002570: 7400 6500 6e00 2000 4d00 6f00 6e00 6100  t.e.n. .M.o.n.a.
-00002580: 7408 0000 0000 0600 0000 0a4c 6173 7420  t..........Last 
-00002590: 6d6f 6e74 6807 0000 0009 4472 6167 6f6e  month.....Dragon
-000025a0: 4c6f 6701 0300 0000 1800 6c00 6500 7400  Log.......l.e.t.
-000025b0: 7a00 7400 6500 2000 5700 6f00 6300 6800  z.t.e. .W.o.c.h.
-000025c0: 6508 0000 0000 0600 0000 094c 6173 7420  e..........Last 
-000025d0: 7765 656b 0700 0000 0944 7261 676f 6e4c  week.....DragonL
-000025e0: 6f67 0103 0000 0018 006c 0065 0074 007a  og.......l.e.t.z
-000025f0: 0074 0065 0073 0020 004a 0061 0068 0072  .t.e.s. .J.a.h.r
-00002600: 0800 0000 0006 0000 0009 4c61 7374 2079  ..........Last y
-00002610: 6561 7207 0000 0009 4472 6167 6f6e 4c6f  ear.....DragonLo
-00002620: 6701 0300 0000 2000 4c00 6f00 5400 5700  g..... .L.o.T.W.
-00002630: 2d00 4100 4400 4900 4600 2d00 5500 7000  -.A.D.I.F.-.U.p.
-00002640: 6c00 6f00 6100 6408 0000 0000 0600 0000  l.o.a.d.........
-00002650: 104c 6f54 5720 4144 4946 2075 706c 6f61  .LoTW ADIF uploa
-00002660: 6407 0000 0009 4472 6167 6f6e 4c6f 6701  d.....DragonLog.
-00002670: 0300 0000 1400 4c00 6f00 5400 5700 2000  ......L.o.T.W. .
-00002680: 6500 6d00 7000 6600 2e08 0000 0000 0600  e.m.p.f.........
-00002690: 0000 094c 6f54 5720 7263 7664 0700 0000  ...LoTW rcvd....
-000026a0: 0944 7261 676f 6e4c 6f67 0103 0000 0014  .DragonLog......
-000026b0: 004c 006f 0054 0057 0020 0076 0065 0072  .L.o.T.W. .v.e.r
-000026c0: 0073 002e 0800 0000 0006 0000 0009 4c6f  .s............Lo
-000026d0: 5457 2073 656e 7407 0000 0009 4472 6167  TW sent.....Drag
-000026e0: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
-000026f0: 0600 0000 074c 6f63 6174 6f72 0700 0000  .....Locator....
-00002700: 0944 7261 676f 6e4c 6f67 0103 ffff ffff  .DragonLog......
-00002710: 0800 0000 0006 0000 000f 4c6f 6720 696d  ..........Log im
-00002720: 706f 7274 2041 4449 4607 0000 0009 4472  port ADIF.....Dr
-00002730: 6167 6f6e 4c6f 6701 0300 0000 1c00 4c00  agonLog.......L.
-00002740: 6f00 6700 2000 4900 6d00 7000 6f00 7200  o.g. .I.m.p.o.r.
-00002750: 7400 2000 4300 5300 5608 0000 0000 0600  t. .C.S.V.......
-00002760: 0000 0e4c 6f67 2069 6d70 6f72 7420 4353  ...Log import CS
-00002770: 5607 0000 0009 4472 6167 6f6e 4c6f 6701  V.....DragonLog.
-00002780: 0300 0000 2000 4c00 6f00 6700 2000 4900  .... .L.o.g. .I.
-00002790: 6d00 7000 6f00 7200 7400 2000 4500 7800  m.p.o.r.t. .E.x.
-000027a0: 6300 6500 6c08 0000 0000 0600 0000 104c  c.e.l..........L
-000027b0: 6f67 2069 6d70 6f72 7420 4578 6365 6c07  og import Excel.
-000027c0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-000027d0: 0000 2c00 4d00 6500 6800 7200 6600 6100  ..,.M.e.h.r.f.a.
-000027e0: 6300 6800 2000 5100 5300 4f00 7300 2000  c.h. .Q.S.O.s. .
-000027f0: 6500 6900 6e00 6700 6500 6200 6500 6e08  e.i.n.g.e.b.e.n.
-00002800: 0000 0000 0600 0000 0e4c 6f67 206d 756c  .........Log mul
-00002810: 7469 2051 534f 7307 0000 0009 4472 6167  ti QSOs.....Drag
-00002820: 6f6e 4c6f 6701 0300 0000 5a00 4b00 6500  onLog.....Z.K.e.
-00002830: 6900 6e00 6500 2000 5300 7400 6100 7400  i.n.e. .S.t.a.t.
-00002840: 6900 6f00 6e00 7300 6b00 6f00 6e00 6600  i.o.n.s.k.o.n.f.
-00002850: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00002860: 6e00 2000 6900 6e00 2000 5400 5100 5300  n. .i.n. .T.Q.S.
-00002870: 4c00 2000 7600 6500 7200 6600 fc00 6700  L. .v.e.r.f...g.
-00002880: 6200 6100 7208 0000 0000 0600 0000 254d  b.a.r.........%M
-00002890: 6973 7369 6e67 2073 7461 7469 6f6e 2063  issing station c
-000028a0: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
-000028b0: 5451 534c 0700 0000 0944 7261 676f 6e4c  TQSL.....DragonL
-000028c0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-000028d0: 0004 4d6f 6465 0700 0000 0944 7261 676f  ..Mode.....Drago
-000028e0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-000028f0: 0000 0004 4e61 6d65 0700 0000 0944 7261  ....Name.....Dra
-00002900: 676f 6e4c 6f67 0103 0000 0034 004b 0065  gonLog.....4.K.e
-00002910: 0069 006e 0065 0020 0051 0053 004f 0073  .i.n.e. .Q.S.O.s
-00002920: 0020 0066 00fc 0072 0020 0064 0065 006e  . .f...r. .d.e.n
-00002930: 0020 004c 006f 0063 0061 0074 006f 0072  . .L.o.c.a.t.o.r
-00002940: 0800 0000 0006 0000 0017 4e6f 2072 6563  ..........No rec
-00002950: 6f72 6473 2066 6f72 206c 6f63 6174 696f  ords for locatio
-00002960: 6e07 0000 0009 4472 6167 6f6e 4c6f 6701  n.....DragonLog.
-00002970: 0300 0000 0e00 4e00 6f00 7400 6900 7a00  ......N.o.t.i.z.
-00002980: 6500 6e08 0000 0000 0600 0000 054e 6f74  e.n..........Not
-00002990: 6573 0700 0000 0944 7261 676f 6e4c 6f67  es.....DragonLog
-000029a0: 0103 ffff ffff 0800 0000 0006 0000 0002  ................
-000029b0: 4f6b 0700 0000 0944 7261 676f 6e4c 6f67  Ok.....DragonLog
-000029c0: 0103 0000 001e 0045 0069 0067 0065 006e  .......E.i.g.e.n
-000029d0: 0065 0072 0020 004c 006f 0063 0061 0074  .e.r. .L.o.c.a.t
-000029e0: 006f 0072 0800 0000 0006 0000 000b 4f77  .o.r..........Ow
-000029f0: 6e20 4c6f 6361 746f 7207 0000 0009 4472  n Locator.....Dr
-00002a00: 6167 6f6e 4c6f 6701 0300 0000 1800 4500  agonLog.......E.
-00002a10: 6900 6700 6500 6e00 6500 7200 2000 4e00  i.g.e.n.e.r. .N.
-00002a20: 6100 6d00 6508 0000 0000 0600 0000 084f  a.m.e..........O
-00002a30: 776e 204e 616d 6507 0000 0009 4472 6167  wn Name.....Drag
-00002a40: 6f6e 4c6f 6701 0300 0000 1600 4500 6900  onLog.......E.i.
-00002a50: 6700 6500 6e00 6500 7200 2000 5100 5400  g.e.n.e.r. .Q.T.
-00002a60: 4808 0000 0000 0600 0000 074f 776e 2051  H..........Own Q
-00002a70: 5448 0700 0000 0944 7261 676f 6e4c 6f67  TH.....DragonLog
-00002a80: 0103 0000 0024 0045 0069 0067 0065 006e  .....$.E.i.g.e.n
-00002a90: 0065 0073 0020 0052 0075 0066 007a 0065  .e.s. .R.u.f.z.e
-00002aa0: 0069 0063 0068 0065 006e 0800 0000 0006  .i.c.h.e.n......
-00002ab0: 0000 000d 4f77 6e20 6361 6c6c 2073 6967  ....Own call sig
-00002ac0: 6e07 0000 0009 4472 6167 6f6e 4c6f 6701  n.....DragonLog.
-00002ad0: 0300 0000 1000 4c00 6500 6900 7300 7400  ......L.e.i.s.t.
-00002ae0: 7500 6e00 6708 0000 0000 0600 0000 0550  u.n.g..........P
-00002af0: 6f77 6572 0700 0000 0944 7261 676f 6e4c  ower.....DragonL
-00002b00: 6f67 0103 0000 001a 0051 0053 004c 002d  og.......Q.S.L.-
-00002b10: 004e 0061 0063 0068 0072 0069 0063 0068  .N.a.c.h.r.i.c.h
-00002b20: 0074 0800 0000 0006 0000 000b 5153 4c20  .t..........QSL 
-00002b30: 6d65 7373 6167 6507 0000 0009 4472 6167  message.....Drag
-00002b40: 6f6e 4c6f 6701 0300 0000 1000 5100 5300  onLog.......Q.S.
-00002b50: 4c00 2d00 5000 6600 6100 6408 0000 0000  L.-.P.f.a.d.....
-00002b60: 0600 0000 0851 534c 2070 6174 6807 0000  .....QSL path...
-00002b70: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002b80: 1200 5100 5300 4c00 2000 6500 6d00 7000  ..Q.S.L. .e.m.p.
-00002b90: 6600 2e08 0000 0000 0600 0000 0851 534c  f............QSL
-00002ba0: 2072 6376 6407 0000 0009 4472 6167 6f6e   rcvd.....Dragon
-00002bb0: 4c6f 6701 0300 0000 1200 5100 5300 4c00  Log.......Q.S.L.
-00002bc0: 2000 7600 6500 7200 7300 2e08 0000 0000   .v.e.r.s.......
-00002bd0: 0600 0000 0851 534c 2073 656e 7407 0000  .....QSL sent...
-00002be0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002bf0: 0e00 5100 5300 4c00 2d00 5600 6900 6108  ..Q.S.L.-.V.i.a.
-00002c00: 0000 0000 0600 0000 0751 534c 2076 6961  .........QSL via
-00002c10: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002c20: ffff ffff 0800 0000 0006 0000 0003 5153  ..............QS
-00002c30: 4f07 0000 0009 4472 6167 6f6e 4c6f 6701  O.....DragonLog.
-00002c40: 0300 0000 4800 5100 5300 4f00 2d00 4c00  ....H.Q.S.O.-.L.
-00002c50: 6f00 6700 2000 2800 2a00 2e00 7100 6c00  o.g. .(.*...q.l.
-00002c60: 6f00 6700 2900 3b00 3b00 4100 6c00 6c00  o.g.).;.;.A.l.l.
-00002c70: 6500 2000 4400 6100 7400 6500 6900 6500  e. .D.a.t.e.i.e.
-00002c80: 6e00 2000 2800 2a00 2e00 2a00 2908 0000  n. .(.*...*.)...
-00002c90: 0000 0600 0000 2151 534f 2d4c 6f67 2028  ......!QSO-Log (
-00002ca0: 2a2e 716c 6f67 293b 3b41 6c6c 2046 696c  *.qlog);;All Fil
-00002cb0: 6573 2028 2a2e 2a29 0700 0000 0944 7261  es (*.*).....Dra
-00002cc0: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00002cd0: 0006 0000 0003 5154 4807 0000 0009 4472  ......QTH.....Dr
-00002ce0: 6167 6f6e 4c6f 6701 0300 0000 1200 5200  agonLog.......R.
-00002cf0: 5300 5400 2000 6500 6d00 7000 6600 2e08  S.T. .e.m.p.f...
-00002d00: 0000 0000 0600 0000 0852 5354 2072 6376  .........RST rcv
-00002d10: 6407 0000 0009 4472 6167 6f6e 4c6f 6701  d.....DragonLog.
-00002d20: 0300 0000 1000 5200 5300 5400 2000 6700  ......R.S.T. .g.
-00002d30: 6500 7300 2e08 0000 0000 0600 0000 0852  e.s............R
-00002d40: 5354 2073 656e 7407 0000 0009 4472 6167  ST sent.....Drag
-00002d50: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
-00002d60: 0600 0000 0552 6164 696f 0700 0000 0944  .....Radio.....D
-00002d70: 7261 676f 6e4c 6f67 0103 0000 002a 0045  ragonLog.....*.E
-00002d80: 0078 0070 006f 0072 0074 0064 0061 0074  .x.p.o.r.t.d.a.t
-00002d90: 0065 0069 0020 0073 0070 0065 0069 0063  .e.i. .s.p.e.i.c
-00002da0: 0068 0065 0072 006e 0800 0000 0006 0000  .h.e.r.n........
-00002db0: 0012 5365 6c65 6374 2065 7870 6f72 7420  ..Select export 
-00002dc0: 6669 6c65 0700 0000 0944 7261 676f 6e4c  file.....DragonL
-00002dd0: 6f67 0103 0000 0020 0044 0061 0074 0065  og..... .D.a.t.e
-00002de0: 006e 0062 0061 006e 006b 0020 00f6 0066  .n.b.a.n.k. ...f
-00002df0: 0066 006e 0065 006e 0800 0000 0006 0000  .f.n.e.n........
-00002e00: 000b 5365 6c65 6374 2066 696c 6507 0000  ..Select file...
-00002e10: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002e20: 3800 5a00 7500 2000 fc00 6200 6500 7200  8.Z.u. ...b.e.r.
-00002e30: 7700 6100 6300 6800 6500 6e00 6400 6500  w.a.c.h.e.n.d.e.
-00002e40: 2000 4400 6100 7400 6500 6900 2000 7700   .D.a.t.e.i. .w.
-00002e50: e400 6800 6c00 6500 6e08 0000 0000 0600  ..h.l.e.n.......
-00002e60: 0000 1453 656c 6563 7420 6669 6c65 2074  ...Select file t
-00002e70: 6f20 7761 7463 6807 0000 0009 4472 6167  o watch.....Drag
-00002e80: 6f6e 4c6f 6701 0300 0000 2400 4900 6d00  onLog.....$.I.m.
-00002e90: 7000 6f00 7200 7400 6400 6100 7400 6500  p.o.r.t.d.a.t.e.
-00002ea0: 6900 2000 f600 6600 6600 6e00 6500 6e08  i. ...f.f.n.e.n.
-00002eb0: 0000 0000 0600 0000 1253 656c 6563 7420  .........Select 
-00002ec0: 696d 706f 7274 2066 696c 6507 0000 0009  import file.....
-00002ed0: 4472 6167 6f6e 4c6f 6701 0300 0000 1a00  DragonLog.......
-00002ee0: 5700 e400 6800 6c00 6500 2000 5300 7400  W...h.l.e. .S.t.
-00002ef0: 6100 7400 6900 6f00 6e08 0000 0000 0600  a.t.i.o.n.......
-00002f00: 0000 0e53 656c 6563 7420 7374 6174 696f  ...Select statio
-00002f10: 6e07 0000 0009 4472 6167 6f6e 4c6f 6701  n.....DragonLog.
-00002f20: 0300 0000 4400 4c00 6f00 5400 5700 2d00  ....D.L.o.T.W.-.
-00002f30: 5300 6500 7200 7600 6500 7200 2000 6800  S.e.r.v.e.r. .h.
-00002f40: 6100 7400 2000 6400 6100 7300 2000 4c00  a.t. .d.a.s. .L.
-00002f50: 6f00 6700 2000 6100 6200 6700 6500 7700  o.g. .a.b.g.e.w.
-00002f60: 6900 6500 7300 6500 6e08 0000 0000 0600  i.e.s.e.n.......
-00002f70: 0000 1353 6572 7665 7220 7265 6a65 6374  ...Server reject
-00002f80: 6564 206c 6f67 0700 0000 0944 7261 676f  ed log.....Drago
-00002f90: 6e4c 6f67 0103 0000 0014 007a 0065 0069  nLog.......z.e.i
-00002fa0: 0067 0065 0020 0061 006c 006c 0065 0800  .g.e. .a.l.l.e..
-00002fb0: 0000 0006 0000 0008 5368 6f77 2061 6c6c  ........Show all
-00002fc0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002fd0: 0000 002a 0054 0051 0053 004c 002d 0053  ...*.T.Q.S.L.-.S
-00002fe0: 0069 0067 006e 0061 0074 0075 0072 0070  .i.g.n.a.t.u.r.p
-00002ff0: 0061 0073 0073 0077 006f 0072 0074 0800  .a.s.s.w.o.r.t..
-00003000: 0000 0006 0000 0017 5451 534c 2073 6967  ........TQSL sig
-00003010: 6e61 7475 7265 2070 6173 7377 6f72 6407  nature password.
-00003020: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00003030: 0000 b200 4400 6900 6500 2000 4400 6100  ....D.i.e. .D.a.
-00003040: 7400 6500 6e00 6200 6100 6e00 6b00 7300  t.e.n.b.a.n.k.s.
-00003050: 7400 7200 7500 6b00 7400 7500 7200 2000  t.r.u.k.t.u.r. .
-00003060: 6900 7300 7400 2000 7600 6500 7200 6100  i.s.t. .v.e.r.a.
-00003070: 6c00 7400 6500 7400 2000 7500 6e00 6400  l.t.e.t. .u.n.d.
-00003080: 2000 6d00 7500 7300 7300 2000 6b00 6f00   .m.u.s.s. .k.o.
-00003090: 6e00 7600 6500 7200 7400 6900 6500 7200  n.v.e.r.t.i.e.r.
-000030a0: 7400 2000 7700 6500 7200 6400 6500 6e00  t. .w.e.r.d.e.n.
-000030b0: 0a00 0a00 4500 6900 6e00 2000 4200 6100  ....E.i.n. .B.a.
-000030c0: 6300 6b00 7500 7000 2000 7700 6900 7200  c.k.u.p. .w.i.r.
-000030d0: 6400 2000 6500 7200 7300 7400 6500 6c00  d. .e.r.s.t.e.l.
-000030e0: 6c00 7400 3a08 0000 0000 0600 0000 5754  l.t.:.........WT
-000030f0: 6865 2064 6174 6162 6173 6520 7374 7275  he database stru
-00003100: 6374 7572 6520 6973 206f 7574 2d64 6174  cture is out-dat
-00003110: 6564 2061 6e64 206e 6565 6473 2061 2063  ed and needs a c
-00003120: 6f6e 7665 7273 696f 6e0a 0a41 2062 6163  onversion..A bac
-00003130: 6b75 7020 7769 6c6c 2062 6520 6765 6e65  kup will be gene
-00003140: 7261 7465 643a 0700 0000 0944 7261 676f  rated:.....Drago
-00003150: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-00003160: 0000 0007 5665 7273 696f 6e07 0000 0009  ....Version.....
-00003170: 4472 6167 6f6e 4c6f 6701 0300 0000 2c00  DragonLog.....,.
-00003180: 5000 7200 6f00 6700 7200 6100 6d00 6d00  P.r.o.g.r.a.m.m.
-00003190: 6c00 6f00 6700 2000 fc00 6200 6500 7200  l.o.g. ...b.e.r.
-000031a0: 7700 6100 6300 6800 6500 6e08 0000 0000  w.a.c.h.e.n.....
-000031b0: 0600 0000 1557 6174 6368 2061 7070 6c69  .....Watch appli
-000031c0: 6361 7469 6f6e 206c 6f67 0700 0000 0944  cation log.....D
-000031d0: 7261 676f 6e4c 6f67 0103 0000 0020 0044  ragonLog..... .D
-000031e0: 0061 0074 0065 0069 00fc 0062 0065 0072  .a.t.e.i...b.e.r
-000031f0: 0077 0061 0063 0068 0075 006e 0067 0800  .w.a.c.h.u.n.g..
-00003200: 0000 0006 0000 000d 5761 7463 6869 6e67  ........Watching
-00003210: 2066 696c 6507 0000 0009 4472 6167 6f6e   file.....Dragon
-00003220: 4c6f 6701 0300 0000 1400 6500 5100 5300  Log.......e.Q.S.
-00003230: 4c00 2000 6500 6d00 7000 6600 2e08 0000  L. .e.m.p.f.....
-00003240: 0000 0600 0000 0965 5153 4c20 7263 7664  .......eQSL rcvd
-00003250: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003260: 0000 0014 0065 0051 0053 004c 0020 0076  .....e.Q.S.L. .v
-00003270: 0065 0072 0073 002e 0800 0000 0006 0000  .e.r.s..........
-00003280: 0009 6551 534c 2073 656e 7407 0000 0009  ..eQSL sent.....
-00003290: 4472 6167 6f6e 4c6f 6701 0300 0000 0e00  DragonLog.......
-000032a0: 6900 6e00 6100 6b00 7400 6900 7608 0000  i.n.a.k.t.i.v...
-000032b0: 0000 0600 0000 0769 6e61 6374 6976 0700  .......inactiv..
-000032c0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-000032d0: 0008 00dc 0062 0065 0072 0800 0000 0006  .....b.e.r......
-000032e0: 0000 0005 4162 6f75 7407 0000 000a 4d61  ....About.....Ma
-000032f0: 696e 5769 6e64 6f77 0103 0000 000e 00dc  inWindow........
-00003300: 0062 0065 0072 0020 0051 0074 0800 0000  .b.e.r. .Q.t....
-00003310: 0006 0000 0008 4162 6f75 7420 5174 0700  ......About Qt..
-00003320: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00003330: 0000 1a00 4100 6e00 7700 6500 6e00 6400  ....A.n.w.e.n.d.
-00003340: 7500 6e00 6700 7300 6c00 6f00 6708 0000  u.n.g.s.l.o.g...
-00003350: 0000 0600 0000 0f41 7070 6c69 6361 7469  .......Applicati
-00003360: 6f6e 204c 6f67 0700 0000 0a4d 6169 6e57  on Log.....MainW
-00003370: 696e 646f 7701 0300 0000 2200 4500 6900  indow.....".E.i.
-00003380: 6e00 7400 7200 6100 6700 2000 e400 6e00  n.t.r.a.g. ...n.
-00003390: 6400 6500 7200 6e00 2e00 2e00 2e08 0000  d.e.r.n.........
-000033a0: 0000 0600 0000 1343 6861 6e67 6520 6c6f  .......Change lo
-000033b0: 6720 656e 7472 792e 2e2e 0700 0000 0a4d  g entry........M
-000033c0: 6169 6e57 696e 646f 7701 03ff ffff ff08  ainWindow.......
-000033d0: 0000 0000 0600 0000 0643 7472 6c2b 4507  .........Ctrl+E.
-000033e0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-000033f0: ffff ffff 0800 0000 0006 0000 0006 4374  ..............Ct
-00003400: 726c 2b4c 0700 0000 0a4d 6169 6e57 696e  rl+L.....MainWin
-00003410: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
-00003420: 0000 0643 7472 6c2b 5107 0000 000a 4d61  ...Ctrl+Q.....Ma
-00003430: 696e 5769 6e64 6f77 0103 ffff ffff 0800  inWindow........
-00003440: 0000 0006 0000 000c 4374 726c 2b53 6869  ........Ctrl+Shi
-00003450: 6674 2b4c 0700 0000 0a4d 6169 6e57 696e  ft+L.....MainWin
-00003460: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
-00003470: 0000 0643 7472 6c2b 5707 0000 000a 4d61  ...Ctrl+W.....Ma
-00003480: 696e 5769 6e64 6f77 0103 ffff ffff 0800  inWindow........
-00003490: 0000 0006 0000 0006 4374 726c 2b58 0700  ........Ctrl+X..
-000034a0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-000034b0: 0000 1e00 4500 6900 6e00 7400 7200 6100  ....E.i.n.t.r.a.
-000034c0: 6700 2000 6c00 f600 7300 6300 6800 6500  g. .l...s.c.h.e.
-000034d0: 6e08 0000 0000 0600 0000 1044 656c 6574  n..........Delet
-000034e0: 6520 6c6f 6720 656e 7472 7907 0000 000a  e log entry.....
-000034f0: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
-00003500: 0800 0000 0006 0000 0009 4472 6167 6f6e  ..........Dragon
-00003510: 4c6f 6707 0000 000a 4d61 696e 5769 6e64  Log.....MainWind
-00003520: 6f77 0103 0000 0014 0042 0065 0061 0072  ow.......B.e.a.r
-00003530: 0062 0065 0069 0074 0065 006e 0800 0000  .b.e.i.t.e.n....
-00003540: 0006 0000 0004 4564 6974 0700 0000 0a4d  ......Edit.....M
-00003550: 6169 6e57 696e 646f 7701 0300 0000 0e00  ainWindow.......
-00003560: 4200 6500 6500 6e00 6400 6500 6e08 0000  B.e.e.n.d.e.n...
-00003570: 0000 0600 0000 0445 7869 7407 0000 000a  .......Exit.....
-00003580: 4d61 696e 5769 6e64 6f77 0103 0000 001c  MainWindow......
-00003590: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
-000035a0: 0072 0065 006e 002e 002e 002e 0800 0000  .r.e.n..........
-000035b0: 0006 0000 0009 4578 706f 7274 2e2e 2e07  ......Export....
-000035c0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-000035d0: 0000 000a 0044 0061 0074 0065 0069 0800  .....D.a.t.e.i..
-000035e0: 0000 0006 0000 0004 4669 6c65 0700 0000  ........File....
-000035f0: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-00003600: 0a00 4800 6900 6c00 6600 6508 0000 0000  ..H.i.l.f.e.....
-00003610: 0600 0000 0448 656c 7007 0000 000a 4d61  .....Help.....Ma
-00003620: 696e 5769 6e64 6f77 0103 0000 001c 0049  inWindow.......I
-00003630: 006d 0070 006f 0072 0074 0069 0065 0072  .m.p.o.r.t.i.e.r
-00003640: 0065 006e 002e 002e 002e 0800 0000 0006  .e.n............
-00003650: 0000 0009 496d 706f 7274 2e2e 2e07 0000  ....Import......
-00003660: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
-00003670: 0018 004c 006f 0067 0067 0065 0020 0051  ...L.o.g.g.e. .Q
-00003680: 0053 004f 002e 002e 002e 0800 0000 0006  .S.O............
-00003690: 0000 000a 4c6f 6720 5153 4f2e 2e2e 0700  ....Log QSO.....
-000036a0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-000036b0: 0000 2a00 4c00 6f00 6700 6700 6500 2000  ..*.L.o.g.g.e. .
-000036c0: 6d00 6500 6800 7200 6500 7200 6500 2000  m.e.h.r.e.r.e. .
-000036d0: 5100 5300 4f00 7300 2e00 2e00 2e08 0000  Q.S.O.s.........
-000036e0: 0000 0600 0000 114c 6f67 206d 756c 7469  .......Log multi
-000036f0: 2051 534f 732e 2e2e 0700 0000 0a4d 6169   QSOs........Mai
-00003700: 6e57 696e 646f 7701 0300 0000 2600 4400  nWindow.....&.D.
-00003710: 6100 7400 6500 6e00 6200 6100 6e00 6b00  a.t.e.n.b.a.n.k.
-00003720: 2000 7700 e400 6800 6c00 6500 6e00 2e00   .w...h.l.e.n...
-00003730: 2e00 2e08 0000 0000 0600 0000 1253 656c  .............Sel
-00003740: 6563 7420 6461 7461 6261 7365 2e2e 2e07  ect database....
-00003750: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-00003760: 0000 001a 0045 0069 006e 0073 0074 0065  .....E.i.n.s.t.e
-00003770: 006c 006c 0075 006e 0067 0065 006e 0800  .l.l.u.n.g.e.n..
-00003780: 0000 0006 0000 0008 5365 7474 696e 6773  ........Settings
-00003790: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-000037a0: 0300 0000 2600 5a00 6500 6900 6700 6500  ....&.Z.e.i.g.e.
-000037b0: 2000 4100 6e00 7700 6500 6e00 6400 7500   .A.n.w.e.n.d.u.
-000037c0: 6e00 6700 7300 6c00 6f00 6708 0000 0000  n.g.s.l.o.g.....
-000037d0: 0600 0000 0853 686f 7720 6c6f 6707 0000  .....Show log...
-000037e0: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
-000037f0: 001a 0053 0074 0061 0072 0074 0065 0020  ...S.t.a.r.t.e. 
-00003800: 0048 0061 006d 006c 0069 0062 0800 0000  .H.a.m.l.i.b....
-00003810: 0006 0000 000c 5374 6172 7420 6861 6d6c  ......Start haml
-00003820: 6962 0700 0000 0a4d 6169 6e57 696e 646f  ib.....MainWindo
-00003830: 7701 0300 0000 1c00 5700 6500 7200 6b00  w.......W.e.r.k.
-00003840: 7a00 6500 7500 6700 6c00 6500 6900 7300  z.e.u.g.l.e.i.s.
-00003850: 7400 6508 0000 0000 0600 0000 0754 6f6f  t.e..........Too
-00003860: 6c62 6172 0700 0000 0a4d 6169 6e57 696e  lbar.....MainWin
-00003870: 646f 7701 0300 0000 3200 4c00 6f00 6700  dow.....2.L.o.g.
-00003880: 7300 2000 7a00 7500 2000 4c00 6f00 5400  s. .z.u. .L.o.T.
-00003890: 5700 2000 6800 6f00 6300 6800 6c00 6100  W. .h.o.c.h.l.a.
-000038a0: 6400 6500 6e00 2e00 2e00 2e08 0000 0000  d.e.n...........
-000038b0: 0600 0000 1655 706c 6f61 6420 6c6f 6773  .....Upload logs
-000038c0: 2074 6f20 4c6f 5457 2e2e 2e07 0000 000a   to LoTW........
-000038d0: 4d61 696e 5769 6e64 6f77 0103 0000 0042  MainWindow.....B
-000038e0: 0044 0061 0074 0065 0069 0020 0061 0075  .D.a.t.e.i. .a.u
-000038f0: 0066 0020 006e 0065 0075 0065 0020 0051  .f. .n.e.u.e. .Q
-00003900: 0053 004f 0073 0020 00fc 0062 0065 0072  .S.O.s. ...b.e.r
-00003910: 0077 0061 0063 0068 0065 006e 002e 002e  .w.a.c.h.e.n....
-00003920: 002e 0800 0000 0006 0000 0016 5761 7463  ............Watc
-00003930: 6820 6669 6c65 2066 6f72 2051 534f 732e  h file for QSOs.
-00003940: 2e2e 0700 0000 0a4d 6169 6e57 696e 646f  .......MainWindo
-00003950: 7701 0300 0000 4800 4500 6900 6e00 2000  w.....H.E.i.n. .
-00003960: 4600 6500 6c00 6400 2000 6600 6500 6800  F.e.l.d. .f.e.h.
-00003970: 6c00 7400 2000 6600 fc00 7200 2000 6400  l.t. .f...r. .d.
-00003980: 6900 6500 2000 4900 6e00 6200 6f00 7800  i.e. .I.n.b.o.x.
-00003990: 2d00 5000 7200 fc00 6600 7500 6e00 6708  -.P.r...f.u.n.g.
-000039a0: 0000 0000 0600 0000 2241 2066 6965 6c64  ........"A field
-000039b0: 2069 7320 6d69 7373 696e 6720 666f 7220   is missing for 
-000039c0: 696e 626f 7820 6368 6563 6b07 0000 0007  inbox check.....
-000039d0: 5153 4f46 6f72 6d01 0300 0000 4200 4600  QSOForm.....B.F.
-000039e0: 6500 6800 6c00 6500 6e00 6400 6500 7300  e.h.l.e.n.d.e.s.
-000039f0: 2000 4600 6500 6c00 6400 2000 6600 fc00   .F.e.l.d. .f...
-00003a00: 7200 2000 6400 6500 6e00 2000 4c00 6f00  r. .d.e.n. .L.o.
-00003a10: 6700 2d00 5500 7000 6c00 6f00 6100 6408  g.-.U.p.l.o.a.d.
-00003a20: 0000 0000 0600 0000 2141 2066 6965 6c64  ........!A field
-00003a30: 2069 7320 6d69 7373 696e 6720 666f 7220   is missing for 
-00003a40: 6c6f 6720 7570 6c6f 6164 0700 0000 0751  log upload.....Q
-00003a50: 534f 466f 726d 0103 0000 0038 0046 0065  SOForm.....8.F.e
-00003a60: 0068 006c 0065 0072 0068 0061 0066 0074  .h.l.e.r.h.a.f.t
-00003a70: 0065 0073 0020 0041 0062 0066 0072 0061  .e.s. .A.b.f.r.a
-00003a80: 0067 0065 0065 0072 0067 0065 0062 006e  .g.e.e.r.g.e.b.n
-00003a90: 0069 0073 0800 0000 0006 0000 0012 4261  .i.s..........Ba
-00003aa0: 6420 7265 7175 6573 7420 7265 7375 6c74  d request result
-00003ab0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00003ac0: 003c 0046 0065 0068 006c 0065 0072 0020  .<.F.e.h.l.e.r. 
-00003ad0: 0062 0065 0069 0020 0064 0065 0072 0020  .b.e.i. .d.e.r. 
-00003ae0: 0052 0075 0066 007a 0065 0069 0063 0068  .R.u.f.z.e.i.c.h
-00003af0: 0065 006e 0073 0075 0063 0068 0065 0800  .e.n.s.u.c.h.e..
-00003b00: 0000 0006 0000 0015 4361 6c6c 626f 6f6b  ........Callbook
-00003b10: 2073 6561 7263 6820 6572 726f 7207 0000   search error...
-00003b20: 0007 5153 4f46 6f72 6d01 0300 0000 2a00  ..QSOForm.....*.
-00003b30: 4300 6100 6c00 6c00 6200 6f00 6f00 6b00  C.a.l.l.b.o.o.k.
-00003b40: 2d00 5300 7500 6300 6800 6500 7200 6700  -.S.u.c.h.e.r.g.
-00003b50: 6500 6200 6e00 6900 7308 0000 0000 0600  e.b.n.i.s.......
-00003b60: 0000 1643 616c 6c62 6f6f 6b20 7365 6172  ...Callbook sear
-00003b70: 6368 2072 6573 756c 7407 0000 0007 5153  ch result.....QS
-00003b80: 4f46 6f72 6d01 0300 0000 3200 5200 7500  OForm.....2.R.u.
-00003b90: 6600 7a00 6500 6900 6300 6800 6500 6e00  f.z.e.i.c.h.e.n.
-00003ba0: 2000 6e00 6900 6300 6800 7400 2000 6700   .n.i.c.h.t. .g.
-00003bb0: 6500 6600 7500 6e00 6400 6500 6e08 0000  e.f.u.n.d.e.n...
-00003bc0: 0000 0600 0000 1243 616c 6c73 6967 6e20  .......Callsign 
-00003bd0: 6e6f 7420 666f 756e 6407 0000 0007 5153  not found.....QS
-00003be0: 4f46 6f72 6d01 0300 0000 4200 4600 6500  OForm.....B.F.e.
-00003bf0: 6800 6c00 6500 7200 2000 6200 6500 6900  h.l.e.r. .b.e.i.
-00003c00: 6d00 2000 5000 7200 fc00 6600 6500 6e00  m. .P.r...f.e.n.
-00003c10: 2000 6400 6500 7200 2000 4c00 6f00 5400   .d.e.r. .L.o.T.
-00003c20: 5700 2d00 4900 6e00 6200 6f00 7808 0000  W.-.I.n.b.o.x...
-00003c30: 0000 0600 0000 1643 6865 636b 204c 6f54  .......Check LoT
-00003c40: 5720 496e 626f 7820 6572 726f 7207 0000  W Inbox error...
-00003c50: 0007 5153 4f46 6f72 6d01 0300 0000 3800  ..QSOForm.....8.
-00003c60: 6500 5100 5300 4c00 2d00 4600 6500 6800  e.Q.S.L.-.F.e.h.
-00003c70: 6c00 6500 7200 2000 7000 7200 fc00 6600  l.e.r. .p.r...f.
-00003c80: 6500 6e00 2000 6400 6500 7200 2000 4900  e.n. .d.e.r. .I.
-00003c90: 6e00 6200 6f00 7808 0000 0000 0600 0000  n.b.o.x.........
-00003ca0: 1643 6865 636b 2065 5153 4c20 496e 626f  .Check eQSL Inbo
-00003cb0: 7820 6572 726f 7207 0000 0007 5153 4f46  x error.....QSOF
-00003cc0: 6f72 6d01 0300 0000 2000 4b00 6f00 6e00  orm..... .K.o.n.
-00003cd0: 6600 6900 6700 7500 7200 6900 6500 7200  f.i.g.u.r.i.e.r.
-00003ce0: 7400 6500 2000 4900 4408 0000 0000 0600  t.e. .I.D.......
-00003cf0: 0000 1343 6f6e 6669 6775 7265 6420 6964  ...Configured id
-00003d00: 656e 7469 7479 0700 0000 0751 534f 466f  entity.....QSOFo
-00003d10: 726d 0103 0000 002a 004b 006f 006e 0066  rm.....*.K.o.n.f
-00003d20: 0069 0067 0075 0072 0069 0065 0072 0074  .i.g.u.r.i.e.r.t
-00003d30: 0065 0020 0053 0074 0061 0074 0069 006f  .e. .S.t.a.t.i.o
-00003d40: 006e 0800 0000 0006 0000 0012 436f 6e66  .n..........Conf
-00003d50: 6967 7572 6564 2073 7461 7469 6f6e 0700  igured station..
-00003d60: 0000 0751 534f 466f 726d 0103 0000 006c  ...QSOForm.....l
-00003d70: 0057 00e4 0068 0072 0065 006e 0064 0020  .W...h.r.e.n.d. 
-00003d80: 0064 0065 0072 0020 0052 0075 0066 007a  .d.e.r. .R.u.f.z
-00003d90: 0065 0069 0063 0068 0065 006e 0073 0075  .e.i.c.h.e.n.s.u
-00003da0: 0063 0068 0065 0020 0069 0073 0074 0020  .c.h.e. .i.s.t. 
-00003db0: 0065 0069 006e 0020 0046 0065 0068 006c  .e.i.n. .F.e.h.l
-00003dc0: 0065 0072 0020 0061 0075 0066 0067 0065  .e.r. .a.u.f.g.e
-00003dd0: 0074 0072 0065 0074 0065 006e 0800 0000  .t.r.e.t.e.n....
-00003de0: 0006 0000 0027 4475 7269 6e67 2063 616c  .....'During cal
-00003df0: 6c62 6f6f 6b20 7365 6172 6368 2061 6e20  lbook search an 
-00003e00: 6572 726f 7220 6f63 6375 7265 6407 0000  error occured...
-00003e10: 0007 5153 4f46 6f72 6d01 0300 0000 0c00  ..QSOForm.......
-00003e20: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-00003e30: 0600 0000 0545 7272 6f72 0700 0000 0751  .....Error.....Q
-00003e40: 534f 466f 726d 0103 0000 0024 0065 0051  SOForm.....$.e.Q
-00003e50: 0053 004c 002d 0055 0070 006c 006f 0061  .S.L.-.U.p.l.o.a
-00003e60: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
-00003e70: 0800 0000 0006 0000 000f 4572 726f 7220  ..........Error 
-00003e80: 6f6e 2075 706c 6f61 6407 0000 0007 5153  on upload.....QS
-00003e90: 4f46 6f72 6d01 0300 0000 0400 4900 4408  OForm.......I.D.
-00003ea0: 0000 0000 0600 0000 0849 6465 6e74 6974  .........Identit
-00003eb0: 7907 0000 0007 5153 4f46 6f72 6d01 0300  y.....QSOForm...
-00003ec0: 0000 2600 4c00 6900 6e00 6b00 2000 7a00  ..&.L.i.n.k. .z.
-00003ed0: 7500 7200 2000 6500 5100 5300 4c00 2d00  u.r. .e.Q.S.L.-.
-00003ee0: 4b00 6100 7200 7400 6508 0000 0000 0600  K.a.r.t.e.......
-00003ef0: 0000 114c 696e 6b20 746f 2065 5153 4c20  ...Link to eQSL 
-00003f00: 4361 7264 0700 0000 0751 534f 466f 726d  Card.....QSOForm
-00003f10: 0103 0000 0042 004c 006f 0067 0069 006e  .....B.L.o.g.i.n
-00003f20: 0020 0066 0065 0068 006c 0067 0065 0073  . .f.e.h.l.g.e.s
-00003f30: 0063 0068 006c 0061 0067 0065 006e 0020  .c.h.l.a.g.e.n. 
-00003f40: 0066 00fc 0072 0020 0042 0065 006e 0075  .f...r. .B.e.n.u
-00003f50: 0074 007a 0065 0072 0800 0000 0006 0000  .t.z.e.r........
-00003f60: 0015 4c6f 6769 6e20 6661 696c 6564 2066  ..Login failed f
-00003f70: 6f72 2075 7365 7207 0000 0007 5153 4f46  or user.....QSOF
-00003f80: 6f72 6d01 0300 0000 2600 4b00 6500 6900  orm.....&.K.e.i.
-00003f90: 6e00 2000 6500 5100 5300 4c00 2000 7600  n. .e.Q.S.L. .v.
-00003fa0: 6500 7200 6600 fc00 6700 6200 6100 7208  e.r.f...g.b.a.r.
-00003fb0: 0000 0000 0600 0000 114e 6f20 6551 534c  .........No eQSL
-00003fc0: 2061 7661 696c 6162 6c65 0700 0000 0751   available.....Q
-00003fd0: 534f 466f 726d 0103 0000 002a 0065 0051  SOForm.....*.e.Q
-00003fe0: 0053 004c 002d 004f 0072 0064 006e 0065  .S.L.-.O.r.d.n.e
-00003ff0: 0072 0020 0061 0075 0073 0077 00e4 0068  .r. .a.u.s.w...h
-00004000: 006c 0065 006e 0800 0000 0006 0000 0012  .l.e.n..........
-00004010: 5365 6c65 6374 2065 5153 4c20 666f 6c64  Select eQSL fold
-00004020: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
-00004030: 0000 0036 0053 0065 0072 0076 0065 0072  ...6.S.e.r.v.e.r
-00004040: 006b 006f 006d 006d 0075 006e 0069 006b  .k.o.m.m.u.n.i.k
-00004050: 0061 0074 0069 006f 006e 0073 002d 0046  .a.t.i.o.n.s.-.F
-00004060: 0065 0068 006c 0065 0072 0800 0000 0006  .e.h.l.e.r......
-00004070: 0000 001a 5365 7276 6572 2063 6f6d 6d75  ....Server commu
-00004080: 6e69 6361 7469 6f6e 2065 7272 6f72 0700  nication error..
-00004090: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-000040a0: 0800 0000 0006 0000 0007 5374 6174 696f  ..........Statio
-000040b0: 6e07 0000 0007 5153 4f46 6f72 6d01 0300  n.....QSOForm...
-000040c0: 0000 3000 4400 6100 7300 2000 5100 5300  ..0.D.a.s. .Q.S.
-000040d0: 4f00 2000 6900 7300 7400 2000 6500 6900  O. .i.s.t. .e.i.
-000040e0: 6e00 2000 4400 7500 7000 6c00 6900 6b00  n. .D.u.p.l.i.k.
-000040f0: 6100 7408 0000 0000 0600 0000 1654 6865  a.t..........The
-00004100: 2051 534f 2069 7320 6120 6475 706c 6963   QSO is a duplic
-00004110: 6174 6507 0000 0007 5153 4f46 6f72 6d01  ate.....QSOForm.
-00004120: 0300 0000 2400 6500 5100 5300 4c00 2d00  ....$.e.Q.S.L.-.
-00004130: 5500 7000 6c00 6f00 6100 6400 2d00 4600  U.p.l.o.a.d.-.F.
-00004140: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
-00004150: 0000 1155 706c 6f61 6420 6551 534c 2065  ...Upload eQSL e
-00004160: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
-00004170: 0103 0000 001a 0055 0070 006c 006f 0061  .......U.p.l.o.a
-00004180: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
-00004190: 0800 0000 0006 0000 0010 5570 6c6f 6164  ..........Upload
-000041a0: 206c 6f67 2065 7272 6f72 0700 0000 0751   log error.....Q
-000041b0: 534f 466f 726d 0103 0000 0048 0044 0065  SOForm.....H.D.e
-000041c0: 0072 0020 004e 0075 0074 007a 0065 0072  .r. .N.u.t.z.e.r
-000041d0: 0020 0043 0061 006c 006c 0020 0073 0074  . .C.a.l.l. .s.t
-000041e0: 0069 006d 006d 0074 0020 006e 0069 0063  .i.m.m.t. .n.i.c
-000041f0: 0068 0074 0020 00fc 0062 0065 0072 0065  .h.t. ...b.e.r.e
-00004200: 0069 006e 0800 0000 0006 0000 0018 5573  .i.n..........Us
-00004210: 6572 2063 616c 6c20 646f 6573 206e 6f74  er call does not
-00004220: 206d 6174 6368 0700 0000 0751 534f 466f   match.....QSOFo
-00004230: 726d 0103 0000 0034 0072 0069 0067 0063  rm.....4.r.i.g.c
-00004240: 0074 006c 0064 0020 005a 0065 0069 0074  .t.l.d. .Z.e.i.t
-00004250: 00fc 0062 0065 0072 0073 0063 0068 0072  ...b.e.r.s.c.h.r
-00004260: 0065 0069 0074 0075 006e 0067 0800 0000  .e.i.t.u.n.g....
-00004270: 0006 0000 000f 7269 6763 746c 6420 7469  ......rigctld ti
-00004280: 6d65 6f75 7407 0000 0007 5153 4f46 6f72  meout.....QSOFor
-00004290: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-000042a0: 0220 5707 0000 000d 5153 4f46 6f72 6d44  . W.....QSOFormD
-000042b0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-000042c0: 0600 0000 0420 6b48 7a07 0000 000d 5153  ..... kHz.....QS
-000042d0: 4f46 6f72 6d44 6961 6c6f 6701 03ff ffff  OFormDialog.....
-000042e0: ff08 0000 0000 0600 0000 0235 3907 0000  ...........59...
-000042f0: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-00004300: 0300 0000 1600 4100 6b00 7a00 6500 7000  ......A.k.z.e.p.
-00004310: 7400 6900 6500 7200 7400 3a08 0000 0000  t.i.e.r.t.:.....
-00004320: 0600 0000 0841 6363 6570 7473 3a07 0000  .....Accepts:...
-00004330: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-00004340: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
-00004350: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
-00004360: 656e 6e61 0700 0000 0d51 534f 466f 726d  enna.....QSOForm
-00004370: 4469 616c 6f67 0103 0000 0016 0041 0075  Dialog.......A.u
-00004380: 0074 006f 006d 0061 0074 0069 0073 0063  .t.o.m.a.t.i.s.c
-00004390: 0068 0800 0000 0006 0000 000d 4175 746f  .h..........Auto
-000043a0: 6d61 7469 6361 6c6c 7907 0000 000d 5153  matically.....QS
-000043b0: 4f46 6f72 6d44 6961 6c6f 6701 03ff ffff  OFormDialog.....
-000043c0: ff08 0000 0000 0600 0000 0442 616e 6407  ...........Band.
-000043d0: 0000 000d 5153 4f46 6f72 6d44 6961 6c6f  ....QSOFormDialo
-000043e0: 6701 0300 0000 0800 4200 fc00 7200 6f08  g.......B...r.o.
-000043f0: 0000 0000 0600 0000 0642 7572 6561 7507  .........Bureau.
-00004400: 0000 000d 5153 4f46 6f72 6d44 6961 6c6f  ....QSOFormDialo
-00004410: 6701 0300 0000 1600 4200 fc00 7200 6f00  g.......B...r.o.
-00004420: 2f00 4400 6900 7200 6500 6b00 7408 0000  /.D.i.r.e.k.t...
-00004430: 0000 0600 0000 0d42 7572 6561 752f 4469  .......Bureau/Di
-00004440: 7265 6374 0700 0000 0d51 534f 466f 726d  rect.....QSOForm
-00004450: 4469 616c 6f67 0103 0000 0014 0052 0075  Dialog.......R.u
-00004460: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
-00004470: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
-00004480: 6967 6e07 0000 000d 5153 4f46 6f72 6d44  ign.....QSOFormD
-00004490: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-000044a0: 0600 0000 0843 616c 6c62 6f6f 6b07 0000  .....Callbook...
-000044b0: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-000044c0: 0300 0000 1200 4100 6200 6200 7200 6500  ......A.b.b.r.e.
-000044d0: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
-000044e0: 0643 616e 6365 6c07 0000 000d 5153 4f46  .Cancel.....QSOF
-000044f0: 6f72 6d44 6961 6c6f 6701 0300 0000 0a00  ormDialog.......
-00004500: 4b00 6100 6e00 6100 6c08 0000 0000 0600  K.a.n.a.l.......
-00004510: 0000 0743 6861 6e6e 656c 0700 0000 0d51  ...Channel.....Q
-00004520: 534f 466f 726d 4469 616c 6f67 0103 0000  SOFormDialog....
-00004530: 0016 0050 0072 00fc 0066 0065 0020 0049  ...P.r...f.e. .I
-00004540: 006e 0062 006f 0078 0800 0000 0006 0000  .n.b.o.x........
-00004550: 000b 4368 6563 6b20 496e 626f 7807 0000  ..Check Inbox...
-00004560: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-00004570: 0300 0000 2000 4b00 6f00 6e00 6600 6900  .... .K.o.n.f.i.
-00004580: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
-00004590: 2000 4900 4408 0000 0000 0600 0000 1343   .I.D..........C
-000045a0: 6f6e 6669 6775 7265 6420 6964 656e 7469  onfigured identi
-000045b0: 7479 0700 0000 0d51 534f 466f 726d 4469  ty.....QSOFormDi
-000045c0: 616c 6f67 0103 0000 002a 004b 006f 006e  alog.....*.K.o.n
-000045d0: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
-000045e0: 0074 0065 0020 0053 0074 0061 0074 0069  .t.e. .S.t.a.t.i
-000045f0: 006f 006e 0800 0000 0006 0000 0012 436f  .o.n..........Co
-00004600: 6e66 6967 7572 6564 2073 7461 7469 6f6e  nfigured station
-00004610: 0700 0000 0d51 534f 466f 726d 4469 616c  .....QSOFormDial
-00004620: 6f67 0103 0000 000c 0064 0069 0072 0065  og.......d.i.r.e
-00004630: 006b 0074 0800 0000 0006 0000 0006 4469  .k.t..........Di
-00004640: 7265 6374 0700 0000 0d51 534f 466f 726d  rect.....QSOForm
-00004650: 4469 616c 6f67 0103 0000 001c 0065 0051  Dialog.......e.Q
-00004660: 0053 004c 0020 0073 0070 0065 0069 0063  .S.L. .s.p.e.i.c
-00004670: 0068 0065 0072 006e 0800 0000 0006 0000  .h.e.r.n........
-00004680: 000d 446f 776e 6c6f 6164 2065 5153 4c07  ..Download eQSL.
-00004690: 0000 000d 5153 4f46 6f72 6d44 6961 6c6f  ....QSOFormDialo
-000046a0: 6701 0300 0000 0800 4500 6e00 6400 6508  g.......E.n.d.e.
-000046b0: 0000 0000 0600 0000 0345 6e64 0700 0000  .........End....
-000046c0: 0d51 534f 466f 726d 4469 616c 6f67 0103  .QSOFormDialog..
-000046d0: 0000 0018 0051 0053 004f 0020 0065 0069  .....Q.S.O. .e.i
-000046e0: 006e 0067 0065 0062 0065 006e 0800 0000  .n.g.e.b.e.n....
-000046f0: 0006 0000 0009 456e 7465 7220 5153 4f07  ......Enter QSO.
-00004700: 0000 000d 5153 4f46 6f72 6d44 6961 6c6f  ....QSOFormDialo
-00004710: 6701 0300 0000 1000 4600 7200 6500 7100  g.......F.r.e.q.
-00004720: 7500 6500 6e00 7a08 0000 0000 0600 0000  u.e.n.z.........
-00004730: 0946 7265 7175 656e 6379 0700 0000 0d51  .Frequency.....Q
-00004740: 534f 466f 726d 4469 616c 6f67 0103 ffff  SOFormDialog....
-00004750: ffff 0800 0000 0006 0000 0008 4848 3a6d  ............HH:m
-00004760: 6d3a 7373 0700 0000 0d51 534f 466f 726d  m:ss.....QSOForm
-00004770: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
-00004780: 0006 0000 0006 4861 6d51 5448 0700 0000  ......HamQTH....
-00004790: 0d51 534f 466f 726d 4469 616c 6f67 0103  .QSOFormDialog..
-000047a0: 0000 0026 004c 0069 006e 006b 0020 007a  ...&.L.i.n.k. .z
-000047b0: 0075 0072 0020 0065 0051 0053 004c 002d  .u.r. .e.Q.S.L.-
-000047c0: 004b 0061 0072 0074 0065 0800 0000 0006  .K.a.r.t.e......
-000047d0: 0000 0011 4c69 6e6b 2074 6f20 6551 534c  ....Link to eQSL
-000047e0: 2043 6172 6407 0000 000d 5153 4f46 6f72   Card.....QSOFor
-000047f0: 6d44 6961 6c6f 6701 03ff ffff ff08 0000  mDialog.........
-00004800: 0000 0600 0000 044c 6f54 5707 0000 000d  .......LoTW.....
-00004810: 5153 4f46 6f72 6d44 6961 6c6f 6701 0300  QSOFormDialog...
-00004820: 0000 1c00 4c00 6f00 5400 5700 2000 6500  ....L.o.T.W. .e.
-00004830: 6d00 7000 6600 6100 6e00 6700 6500 6e08  m.p.f.a.n.g.e.n.
-00004840: 0000 0000 0600 0000 0d4c 6f54 5720 7265  .........LoTW re
-00004850: 6365 6976 6564 0700 0000 0d51 534f 466f  ceived.....QSOFo
-00004860: 726d 4469 616c 6f67 0103 0000 001c 004c  rmDialog.......L
-00004870: 006f 0054 0057 0020 0076 0065 0072 0073  .o.T.W. .v.e.r.s
-00004880: 0065 006e 0064 0065 0074 0800 0000 0006  .e.n.d.e.t......
-00004890: 0000 0009 4c6f 5457 2073 656e 7407 0000  ....LoTW sent...
-000048a0: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-000048b0: 03ff ffff ff08 0000 0000 0600 0000 074c  ...............L
-000048c0: 6f63 6174 6f72 0700 0000 0d51 534f 466f  ocator.....QSOFo
-000048d0: 726d 4469 616c 6f67 0103 0000 0014 0048  rmDialog.......H
-000048e0: 0061 0075 0070 0074 0064 0061 0074 0065  .a.u.p.t.d.a.t.e
-000048f0: 006e 0800 0000 0006 0000 0009 4d61 696e  .n..........Main
-00004900: 2064 6174 6107 0000 000d 5153 4f46 6f72   data.....QSOFor
-00004910: 6d44 6961 6c6f 6701 03ff ffff ff08 0000  mDialog.........
-00004920: 0000 0600 0000 044d 6f64 6507 0000 000d  .......Mode.....
-00004930: 5153 4f46 6f72 6d44 6961 6c6f 6701 0300  QSOFormDialog...
-00004940: 0000 1200 7600 6500 7200 e400 6e00 6400  ....v.e.r...n.d.
-00004950: 6500 7200 7408 0000 0000 0600 0000 084d  e.r.t..........M
-00004960: 6f64 6966 6965 6407 0000 000d 5153 4f46  odified.....QSOF
-00004970: 6f72 6d44 6961 6c6f 6701 03ff ffff ff08  ormDialog.......
-00004980: 0000 0000 0600 0000 044e 616d 6507 0000  .........Name...
-00004990: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-000049a0: 0300 0000 0a00 4a00 6500 7400 7a00 7408  ......J.e.t.z.t.
-000049b0: 0000 0000 0600 0000 034e 6f77 0700 0000  .........Now....
-000049c0: 0d51 534f 466f 726d 4469 616c 6f67 0103  .QSOFormDialog..
-000049d0: 0000 0016 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
-000049e0: 0072 0020 0051 0054 0048 0800 0000 0006  .r. .Q.T.H......
-000049f0: 0000 0007 4f77 6e20 5154 4807 0000 000d  ....Own QTH.....
-00004a00: 5153 4f46 6f72 6d44 6961 6c6f 6701 0300  QSOFormDialog...
-00004a10: 0000 2400 4500 6900 6700 6500 6e00 6500  ..$.E.i.g.e.n.e.
-00004a20: 7300 2000 5200 7500 6600 7a00 6500 6900  s. .R.u.f.z.e.i.
-00004a30: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
-00004a40: 0d4f 776e 2063 616c 6c20 7369 676e 0700  .Own call sign..
-00004a50: 0000 0d51 534f 466f 726d 4469 616c 6f67  ...QSOFormDialog
-00004a60: 0103 0000 001e 0045 0069 0067 0065 006e  .......E.i.g.e.n
-00004a70: 0065 0072 0020 004c 006f 0063 0061 0074  .e.r. .L.o.c.a.t
-00004a80: 006f 0072 0800 0000 0006 0000 000b 4f77  .o.r..........Ow
-00004a90: 6e20 6c6f 6361 746f 7207 0000 000d 5153  n locator.....QS
-00004aa0: 4f46 6f72 6d44 6961 6c6f 6701 0300 0000  OFormDialog.....
-00004ab0: 1800 4500 6900 6700 6500 6e00 6500 7200  ..E.i.g.e.n.e.r.
-00004ac0: 2000 4e00 6100 6d00 6508 0000 0000 0600   .N.a.m.e.......
-00004ad0: 0000 084f 776e 206e 616d 6507 0000 000d  ...Own name.....
-00004ae0: 5153 4f46 6f72 6d44 6961 6c6f 6701 0300  QSOFormDialog...
-00004af0: 0000 1c00 4500 6900 6700 6500 6e00 6500  ....E.i.g.e.n.e.
-00004b00: 2000 4e00 6f00 7400 6900 7a00 6500 6e08   .N.o.t.i.z.e.n.
-00004b10: 0000 0000 0600 0000 094f 776e 206e 6f74  .........Own not
-00004b20: 6573 0700 0000 0d51 534f 466f 726d 4469  es.....QSOFormDi
-00004b30: 616c 6f67 0103 0000 0010 004c 0065 0069  alog.......L.e.i
-00004b40: 0073 0074 0075 006e 0067 0800 0000 0006  .s.t.u.n.g......
-00004b50: 0000 0005 506f 7765 7207 0000 000d 5153  ....Power.....QS
-00004b60: 4f46 6f72 6d44 6961 6c6f 6701 03ff ffff  OFormDialog.....
-00004b70: ff08 0000 0000 0600 0000 0351 534c 0700  ...........QSL..
-00004b80: 0000 0d51 534f 466f 726d 4469 616c 6f67  ...QSOFormDialog
-00004b90: 0103 0000 0022 0051 0053 004c 0020 0026  .....".Q.S.L. .&
-00004ba0: 0026 0020 004c 006f 0067 002d 0055 0070  .&. .L.o.g.-.U.p
-00004bb0: 006c 006f 0061 0064 0800 0000 0006 0000  .l.o.a.d........
-00004bc0: 0011 5153 4c20 2626 204c 6f67 2075 706c  ..QSL && Log upl
-00004bd0: 6f61 6407 0000 000d 5153 4f46 6f72 6d44  oad.....QSOFormD
-00004be0: 6961 6c6f 6701 0300 0000 1c00 5100 5300  ialog.......Q.S.
-00004bf0: 4c00 2d00 4b00 6100 7200 7400 6500 6e00  L.-.K.a.r.t.e.n.
-00004c00: 7400 6500 7800 7408 0000 0000 0600 0000  t.e.x.t.........
-00004c10: 1051 534c 2063 6172 6420 6d65 7373 6167  .QSL card messag
-00004c20: 6507 0000 000d 5153 4f46 6f72 6d44 6961  e.....QSOFormDia
-00004c30: 6c6f 6701 0300 0000 1a00 5100 5300 4c00  log.......Q.S.L.
-00004c40: 2000 6500 6d00 7000 6600 6100 6e00 6700   .e.m.p.f.a.n.g.
-00004c50: 6500 6e08 0000 0000 0600 0000 0c51 534c  e.n..........QSL
-00004c60: 2072 6563 6569 7665 6407 0000 000d 5153   received.....QS
-00004c70: 4f46 6f72 6d44 6961 6c6f 6701 0300 0000  OFormDialog.....
-00004c80: 1800 5100 5300 4c00 2000 6700 6500 7300  ..Q.S.L. .g.e.s.
-00004c90: 6500 6e00 6400 6500 7408 0000 0000 0600  e.n.d.e.t.......
-00004ca0: 0000 0851 534c 2073 656e 7407 0000 000d  ...QSL sent.....
-00004cb0: 5153 4f46 6f72 6d44 6961 6c6f 6701 03ff  QSOFormDialog...
-00004cc0: ffff ff08 0000 0000 0600 0000 0751 534c  .............QSL
-00004cd0: 2076 6961 0700 0000 0d51 534f 466f 726d   via.....QSOForm
-00004ce0: 4469 616c 6f67 0103 0000 001c 0051 0053  Dialog.......Q.S
-00004cf0: 004f 002d 004b 006f 006d 006d 0065 006e  .O.-.K.o.m.m.e.n
-00004d00: 0074 0061 0072 0065 0800 0000 0006 0000  .t.a.r.e........
-00004d10: 000c 5153 4f20 636f 6d6d 656e 7473 0700  ..QSO comments..
-00004d20: 0000 0d51 534f 466f 726d 4469 616c 6f67  ...QSOFormDialog
+00000b30: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
+00000b40: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00000b50: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
+00000b60: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
+00000b70: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
+00000b80: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
+00000b90: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
+00000ba0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
+00000bb0: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
+00000bc0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000bd0: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
+00000be0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000bf0: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
+00000c00: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
+00000c10: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
+00000c20: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
+00000c30: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
+00000c40: 616c 6f67 0103 0000 0038 005a 0065 0072  alog.....8.Z.e.r
+00000c50: 0074 0069 0066 0069 006b 0061 0074 0020  .t.i.f.i.k.a.t. 
+00000c60: 0062 0065 006e 00f6 0074 0069 0067 0074  .b.e.n...t.i.g.t
+00000c70: 0020 0050 0061 0073 0073 0077 006f 0072  . .P.a.s.s.w.o.r
+00000c80: 0074 0800 0000 0006 0000 001a 4365 7274  .t..........Cert
+00000c90: 6966 6963 6174 6520 6e65 6564 7320 7061  ificate needs pa
+00000ca0: 7373 776f 7264 0700 0000 0644 6961 6c6f  ssword.....Dialo
+00000cb0: 6701 0300 0000 2400 5300 7000 6100 6c00  g.....$.S.p.a.l.
+00000cc0: 7400 6500 6e00 2000 7600 6500 7200 7300  t.e.n. .v.e.r.s.
+00000cd0: 7400 6500 6300 6b00 6500 6e08 0000 0000  t.e.c.k.e.n.....
+00000ce0: 0600 0000 0f43 6f6c 756d 6e73 2074 6f20  .....Columns to 
+00000cf0: 6869 6465 0700 0000 0644 6961 6c6f 6701  hide.....Dialog.
+00000d00: 0300 0000 2000 5300 7000 6100 6c00 7400  .... .S.p.a.l.t.
+00000d10: 6500 6e00 2000 6100 6e00 7a00 6500 6900  e.n. .a.n.z.e.i.
+00000d20: 6700 6500 6e08 0000 0000 0600 0000 0f43  g.e.n..........C
+00000d30: 6f6c 756d 6e73 2074 6f20 7368 6f77 0700  olumns to show..
+00000d40: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
+00000d50: 4100 6e00 6d00 6500 6c00 6400 6500 6400  A.n.m.e.l.d.e.d.
+00000d60: 6100 7400 6500 6e08 0000 0000 0600 0000  a.t.e.n.........
+00000d70: 0b43 7265 6465 6e74 6961 6c73 0700 0000  .Credentials....
+00000d80: 0644 6961 6c6f 6701 0300 0000 1400 4100  .Dialog.......A.
+00000d90: 6200 7300 7400 6500 6900 6700 6500 6e00  b.s.t.e.i.g.e.n.
+00000da0: 6408 0000 0000 0600 0000 0a44 6573 6365  d..........Desce
+00000db0: 6e64 696e 6707 0000 0006 4469 616c 6f67  nding.....Dialog
+00000dc0: 0103 0000 003e 0057 0069 0072 006b 0073  .....>.W.i.r.k.s
+00000dd0: 0061 006d 0020 006e 0061 0063 0068 0020  .a.m. .n.a.c.h. 
+00000de0: 0041 006e 0077 0065 006e 0064 0075 006e  .A.n.w.e.n.d.u.n
+00000df0: 0067 0073 006e 0065 0075 0073 0074 0061  .g.s.n.e.u.s.t.a
+00000e00: 0072 0074 0800 0000 0006 0000 0023 4566  .r.t.........#Ef
+00000e10: 6665 6374 6976 6520 6166 7465 7220 6170  fective after ap
+00000e20: 706c 6963 6174 696f 6e20 7265 7374 6172  plication restar
+00000e30: 7407 0000 0006 4469 616c 6f67 0103 ffff  t.....Dialog....
+00000e40: ffff 0800 0000 0006 0000 0006 4578 706f  ............Expo
+00000e50: 7274 0700 0000 0644 6961 6c6f 6701 0300  rt.....Dialog...
+00000e60: 0000 3400 4500 7800 7000 6f00 7200 7400  ..4.E.x.p.o.r.t.
+00000e70: 6900 6500 7200 6500 2000 4300 4200 2d00  i.e.r.e. .C.B.-.
+00000e80: 5100 5300 4f00 7300 2000 6900 6e00 2000  Q.S.O.s. .i.n. .
+00000e90: 4100 4400 4900 4608 0000 0000 0600 0000  A.D.I.F.........
+00000ea0: 1645 7870 6f72 7420 4342 2051 534f 7320  .Export CB QSOs 
+00000eb0: 746f 2041 4449 4607 0000 0006 4469 616c  to ADIF.....Dial
+00000ec0: 6f67 0103 0000 0036 0045 0078 0070 006f  og.....6.E.x.p.o
+00000ed0: 0072 0074 0069 0065 0072 0065 0020 006e  .r.t.i.e.r.e. .n
+00000ee0: 0075 0072 0020 006e 0065 0075 0065 0073  .u.r. .n.e.u.e.s
+00000ef0: 0074 0065 0020 0051 0053 004f 0073 0800  .t.e. .Q.S.O.s..
+00000f00: 0000 0006 0000 0017 4578 706f 7274 206f  ........Export o
+00000f10: 6e6c 7920 7265 6365 6e74 2051 534f 7307  nly recent QSOs.
+00000f20: 0000 0006 4469 616c 6f67 0103 0000 0042  ....Dialog.....B
+00000f30: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
+00000f40: 0072 0065 0020 0065 0069 0067 0065 006e  .r.e. .e.i.g.e.n
+00000f50: 0065 0020 004e 006f 0074 0069 007a 0065  .e. .N.o.t.i.z.e
+00000f60: 006e 0020 0069 006e 0020 0041 0044 0049  .n. .i.n. .A.D.I
+00000f70: 0046 0800 0000 0006 0000 0018 4578 706f  .F..........Expo
+00000f80: 7274 206f 776e 206e 6f74 6573 2074 6f20  rt own notes to 
+00000f90: 4144 4946 0700 0000 0644 6961 6c6f 6701  ADIF.....Dialog.
+00000fa0: 03ff ffff ff08 0000 0000 0600 0000 0648  ...............H
+00000fb0: 616d 5154 4807 0000 0006 4469 616c 6f67  amQTH.....Dialog
+00000fc0: 0103 ffff ffff 0800 0000 0006 0000 000e  ................
+00000fd0: 4861 6d6c 6962 2072 6967 6374 6c64 0700  Hamlib rigctld..
+00000fe0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000ff0: 0000 0000 0600 0000 0d49 6d70 6f72 742f  .........Import/
+00001000: 4578 706f 7274 0700 0000 0644 6961 6c6f  Export.....Dialo
+00001010: 6701 0300 0000 1a00 5300 6300 6800 6e00  g.......S.c.h.n.
+00001020: 6900 7400 7400 7300 7400 6500 6c00 6c00  i.t.t.s.t.e.l.l.
+00001030: 6508 0000 0000 0600 0000 0949 6e74 6572  e..........Inter
+00001040: 6661 6365 0700 0000 0644 6961 6c6f 6701  face.....Dialog.
+00001050: 0300 0000 2000 6c00 6500 7400 7a00 7400  .... .l.e.t.z.t.
+00001060: 6500 7300 2000 4800 6100 6c00 6200 6a00  e.s. .H.a.l.b.j.
+00001070: 6100 6800 7208 0000 0000 0600 0000 0e4c  a.h.r..........L
+00001080: 6173 7420 6861 6c66 2079 6561 7207 0000  ast half year...
+00001090: 0006 4469 616c 6f67 0103 0000 001a 006c  ..Dialog.......l
+000010a0: 0065 0074 007a 0074 0065 006e 0020 004d  .e.t.z.t.e.n. .M
+000010b0: 006f 006e 0061 0074 0800 0000 0006 0000  .o.n.a.t........
+000010c0: 000a 4c61 7374 206d 6f6e 7468 0700 0000  ..Last month....
+000010d0: 0644 6961 6c6f 6701 0300 0000 1800 6c00  .Dialog.......l.
+000010e0: 6500 7400 7a00 7400 6500 2000 5700 6f00  e.t.z.t.e. .W.o.
+000010f0: 6300 6800 6508 0000 0000 0600 0000 094c  c.h.e..........L
+00001100: 6173 7420 7765 656b 0700 0000 0644 6961  ast week.....Dia
+00001110: 6c6f 6701 0300 0000 1800 6c00 6500 7400  log.......l.e.t.
+00001120: 7a00 7400 6500 7300 2000 4a00 6100 6800  z.t.e.s. .J.a.h.
+00001130: 7208 0000 0000 0600 0000 094c 6173 7420  r..........Last 
+00001140: 7965 6172 0700 0000 0644 6961 6c6f 6701  year.....Dialog.
+00001150: 0300 0000 0c00 4200 7200 6500 6900 7400  ......B.r.e.i.t.
+00001160: 6508 0000 0000 0600 0000 034c 6174 0700  e..........Lat..
+00001170: 0000 0644 6961 6c6f 6701 0300 0000 0a00  ...Dialog.......
+00001180: 5300 7400 7500 6600 6508 0000 0000 0600  S.t.u.f.e.......
+00001190: 0000 054c 6576 656c 0700 0000 0644 6961  ...Level.....Dia
+000011a0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+000011b0: 0000 044c 6f54 5707 0000 0006 4469 616c  ...LoTW.....Dial
+000011c0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+000011d0: 0007 4c6f 6361 746f 7207 0000 0006 4469  ..Locator.....Di
+000011e0: 616c 6f67 0103 0000 002c 004c 006f 0067  alog.....,.L.o.g
+000011f0: 0020 0069 006e 0020 0044 0061 0074 0065  . .i.n. .D.a.t.e
+00001200: 0069 0020 0073 0063 0068 0072 0065 0069  .i. .s.c.h.r.e.i
+00001210: 0062 0065 006e 0800 0000 0006 0000 000b  .b.e.n..........
+00001220: 4c6f 6720 746f 2066 696c 6507 0000 0006  Log to file.....
+00001230: 4469 616c 6f67 0103 0000 001e 004c 006f  Dialog.......L.o
+00001240: 0067 0067 0069 006e 0067 002d 0041 0075  .g.g.i.n.g.-.A.u
+00001250: 0073 0067 0061 0062 0065 0800 0000 0006  .s.g.a.b.e......
+00001260: 0000 000e 4c6f 6767 696e 6720 6f75 7470  ....Logging outp
+00001270: 7574 0700 0000 0644 6961 6c6f 6701 0300  ut.....Dialog...
+00001280: 0000 0a00 4c00 e400 6e00 6700 6508 0000  ....L...n.g.e...
+00001290: 0000 0600 0000 034c 6f6e 0700 0000 0644  .......Lon.....D
+000012a0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
+000012b0: 0600 0000 044e 616d 6507 0000 0006 4469  .....Name.....Di
+000012c0: 616c 6f67 0103 0000 005e 0043 0042 0020  alog.....^.C.B. 
+000012d0: 0051 0053 004f 0073 0020 0077 0065 0072  .Q.S.O.s. .w.e.r
+000012e0: 0064 0065 006e 0020 0062 0065 0069 006d  .d.e.n. .b.e.i.m
+000012f0: 0020 0049 006d 0070 006f 0072 0074 0020  . .I.m.p.o.r.t. 
+00001300: 0069 006d 006d 0065 0072 0020 0062 0065  .i.m.m.e.r. .b.e
+00001310: 0072 00fc 0063 006b 0073 0069 0063 0068  .r...c.k.s.i.c.h
+00001320: 0074 0069 0067 0074 0800 0000 0006 0000  .t.i.g.t........
+00001330: 0028 4f6e 2069 6d70 6f72 7420 4342 2051  .(On import CB Q
+00001340: 534f 7320 7769 6c6c 2061 6c77 6179 7320  SOs will always 
+00001350: 6265 2068 616e 646c 6564 0700 0000 0644  be handled.....D
+00001360: 6961 6c6f 6701 0300 0000 1000 5000 6100  ialog.......P.a.
+00001370: 7300 7300 7700 6f00 7200 7408 0000 0000  s.s.w.o.r.t.....
+00001380: 0600 0000 0850 6173 7377 6f72 6407 0000  .....Password...
+00001390: 0006 4469 616c 6f67 0103 0000 0070 0050  ..Dialog.....p.P
+000013a0: 0061 0073 0073 0077 006f 0072 0074 0020  .a.s.s.w.o.r.t. 
+000013b0: 0064 0065 0073 0020 004c 006f 0054 0057  .d.e.s. .L.o.T.W
+000013c0: 002d 004f 006e 006c 0069 006e 0065 002d  .-.O.n.l.i.n.e.-
+000013d0: 0041 0063 0063 006f 0075 006e 0074 0073  .A.c.c.o.u.n.t.s
+000013e0: 002c 0020 006e 0069 0063 0068 0074 0020  .,. .n.i.c.h.t. 
+000013f0: 0064 0065 0073 0020 005a 0065 0072 0074  .d.e.s. .Z.e.r.t
+00001400: 0069 0066 0069 006b 0061 0074 0073 0800  .i.f.i.k.a.t.s..
+00001410: 0000 0006 0000 0038 5061 7373 776f 7264  .......8Password
+00001420: 2066 6f72 204c 6f54 5720 6f6e 6c69 6e65   for LoTW online
+00001430: 2061 6363 6f75 6e74 206e 6f74 2066 6f72   account not for
+00001440: 2074 6865 2063 6572 7469 6669 6361 7465   the certificate
+00001450: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
+00001460: ff08 0000 0000 0600 0000 0351 5448 0700  ...........QTH..
+00001470: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00001480: 0000 0000 0600 0000 0552 6164 696f 0700  .........Radio..
+00001490: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
+000014a0: 4e00 6500 7500 6500 7300 7400 6500 2000  N.e.u.e.s.t.e. .
+000014b0: 5100 5300 4f00 7308 0000 0000 0600 0000  Q.S.O.s.........
+000014c0: 0b52 6563 656e 7420 5153 4f73 0700 0000  .Recent QSOs....
+000014d0: 0644 6961 6c6f 6701 0300 0000 1200 4600  .Dialog.......F.
+000014e0: 7500 6e00 6b00 6700 6500 7200 e400 7408  u.n.k.g.e.r...t.
+000014f0: 0000 0000 0600 0000 0352 6967 0700 0000  .........Rig....
+00001500: 0644 6961 6c6f 6701 0300 0000 4c00 5300  .Dialog.....L.S.
+00001510: 6900 6500 6800 6500 2000 4500 6900 6e00  i.e.h.e. .E.i.n.
+00001520: 7300 7400 6500 6c00 6c00 7500 6e00 6700  s.t.e.l.l.u.n.g.
+00001530: 6500 6e00 2000 5200 6500 6900 7400 6500  e.n. .R.e.i.t.e.
+00001540: 7200 2000 2200 4100 6e00 7700 6500 6e00  r. .".A.n.w.e.n.
+00001550: 6400 7500 6e00 6700 2208 0000 0000 0600  d.u.n.g.".......
+00001560: 0000 2253 6565 2073 6574 7469 6e67 7320  .."See settings 
+00001570: 7061 6765 2022 5573 6572 2069 6e74 6572  page "User inter
+00001580: 6661 6365 2207 0000 0006 4469 616c 6f67  face".....Dialog
+00001590: 0103 0000 0034 0043 0042 002d 0042 0061  .....4.C.B.-.B.a
+000015a0: 006e 0064 0020 0061 0075 0074 006f 006d  .n.d. .a.u.t.o.m
+000015b0: 0061 0074 0069 0073 0063 0068 0020 0077  .a.t.i.s.c.h. .w
+000015c0: 00e4 0068 006c 0065 006e 0800 0000 0006  ...h.l.e.n......
+000015d0: 0000 0019 5365 6c65 6374 2043 4220 6261  ....Select CB ba
+000015e0: 6e64 2062 7920 6465 6661 756c 7407 0000  nd by default...
+000015f0: 0006 4469 616c 6f67 0103 0000 001a 0053  ..Dialog.......S
+00001600: 0065 0074 007a 0065 0020 004c 006f 0063  .e.t.z.e. .L.o.c
+00001610: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+00001620: 000b 5365 7420 6c6f 6361 746f 7207 0000  ..Set locator...
+00001630: 0006 4469 616c 6f67 0103 0000 001a 0045  ..Dialog.......E
+00001640: 0069 006e 0073 0074 0065 006c 006c 0075  .i.n.s.t.e.l.l.u
+00001650: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
+00001660: 0008 5365 7474 696e 6773 0700 0000 0644  ..Settings.....D
+00001670: 6961 6c6f 6701 0300 0000 1c00 5a00 6500  ialog.......Z.e.
+00001680: 6900 6700 6500 2000 5100 5300 4f00 7300  i.g.e. .Q.S.O.s.
+00001690: 2000 6600 fc00 7208 0000 0000 0600 0000   .f...r.........
+000016a0: 0e53 686f 7720 5153 4f73 2066 726f 6d07  .Show QSOs from.
+000016b0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
+000016c0: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
+000016d0: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
+000016e0: 6f77 2061 6c6c 0700 0000 0644 6961 6c6f  ow all.....Dialo
+000016f0: 6701 0300 0000 4000 5300 7000 6100 6c00  g.....@.S.p.a.l.
+00001700: 7400 6500 6e00 2000 6100 6e00 7a00 6500  t.e.n. .a.n.z.e.
+00001710: 6900 6700 6500 6e00 2000 6f00 6400 6500  i.g.e.n. .o.d.e.
+00001720: 7200 2000 7600 6500 7200 7300 7400 6500  r. .v.e.r.s.t.e.
+00001730: 6300 6b00 6500 6e08 0000 0000 0600 0000  c.k.e.n.........
+00001740: 1453 686f 7720 6f72 2068 6964 6520 636f  .Show or hide co
+00001750: 6c75 6d6e 7307 0000 0006 4469 616c 6f67  lumns.....Dialog
+00001760: 0103 0000 0028 0053 006f 0072 0074 0069  .....(.S.o.r.t.i
+00001770: 0065 0072 0065 0020 006e 0061 0063 0068  .e.r.e. .n.a.c.h
+00001780: 0020 0053 0070 0061 006c 0074 0065 0800  . .S.p.a.l.t.e..
+00001790: 0000 0006 0000 000e 536f 7274 206f 6e20  ........Sort on 
+000017a0: 636f 6c75 6d6e 0700 0000 0644 6961 6c6f  column.....Dialo
+000017b0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+000017c0: 0553 7461 7274 0700 0000 0644 6961 6c6f  .Start.....Dialo
+000017d0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+000017e0: 0753 7461 7469 6f6e 0700 0000 0644 6961  .Station.....Dia
+000017f0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00001800: 0000 0454 5153 4c07 0000 0006 4469 616c  ...TQSL.....Dial
+00001810: 6f67 0103 0000 0064 0056 0065 0072 0077  og.....d.V.e.r.w
+00001820: 0065 006e 0064 0065 0020 0064 0069 0065  .e.n.d.e. .d.i.e
+00001830: 0020 006b 006f 006e 0066 0069 0067 0075  . .k.o.n.f.i.g.u
+00001840: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
+00001850: 0044 0020 0062 0065 0069 0020 0066 0065  .D. .b.e.i. .f.e
+00001860: 0068 006c 0065 006e 0064 0065 006e 0020  .h.l.e.n.d.e.n. 
+00001870: 0057 0065 0072 0074 0065 006e 0800 0000  .W.e.r.t.e.n....
+00001880: 0006 0000 0024 5573 6520 636f 6e66 6967  .....$Use config
+00001890: 7572 6564 2049 4420 666f 7220 6d69 7373  ured ID for miss
+000018a0: 696e 6720 7661 6c75 6573 0700 0000 0644  ing values.....D
+000018b0: 6961 6c6f 6701 0300 0000 6e00 5600 6500  ialog.....n.V.e.
+000018c0: 7200 7700 6500 6e00 6400 6500 2000 6400  r.w.e.n.d.e. .d.
+000018d0: 6900 6500 2000 6b00 6f00 6e00 6600 6900  i.e. .k.o.n.f.i.
+000018e0: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
+000018f0: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
+00001900: 2000 6200 6500 6900 2000 6600 6500 6800   .b.e.i. .f.e.h.
+00001910: 6c00 6500 6e00 6400 6500 6e00 2000 5700  l.e.n.d.e.n. .W.
+00001920: 6500 7200 7400 6500 6e08 0000 0000 0600  e.r.t.e.n.......
+00001930: 0000 2955 7365 2063 6f6e 6669 6775 7265  ..)Use configure
+00001940: 6420 5374 6174 696f 6e20 666f 7220 6d69  d Station for mi
+00001950: 7373 696e 6720 7661 6c75 6573 0700 0000  ssing values....
+00001960: 0644 6961 6c6f 6701 0300 0000 1200 4100  .Dialog.......A.
+00001970: 6e00 7700 6500 6e00 6400 7500 6e00 6708  n.w.e.n.d.u.n.g.
+00001980: 0000 0000 0600 0000 0e55 7365 7220 696e  .........User in
+00001990: 7465 7266 6163 6507 0000 0006 4469 616c  terface.....Dial
+000019a0: 6f67 0103 0000 0018 0042 0065 006e 0075  og.......B.e.n.u
+000019b0: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
+000019c0: 0800 0000 0006 0000 0008 5573 6572 6e61  ..........Userna
+000019d0: 6d65 0700 0000 0644 6961 6c6f 6701 0300  me.....Dialog...
+000019e0: 0000 7800 4200 6500 6e00 7500 7400 7a00  ..x.B.e.n.u.t.z.
+000019f0: 6500 7200 6e00 6100 6d00 6500 2000 6400  e.r.n.a.m.e. .d.
+00001a00: 6500 7300 2000 4c00 6f00 5400 5700 2d00  e.s. .L.o.T.W.-.
+00001a10: 4f00 6e00 6c00 6900 6e00 6500 2d00 4100  O.n.l.i.n.e.-.A.
+00001a20: 6300 6300 6f00 7500 6e00 7400 7300 2c00  c.c.o.u.n.t.s.,.
+00001a30: 2000 6e00 6900 6300 6800 7400 2000 6400   .n.i.c.h.t. .d.
+00001a40: 6500 7300 2000 5a00 6500 7200 7400 6900  e.s. .Z.e.r.t.i.
+00001a50: 6600 6900 6b00 6100 7400 7308 0000 0000  f.i.k.a.t.s.....
+00001a60: 0600 0000 3855 7365 726e 616d 6520 666f  ....8Username fo
+00001a70: 7220 4c6f 5457 206f 6e6c 696e 6520 6163  r LoTW online ac
+00001a80: 636f 756e 7420 6e6f 7420 666f 7220 7468  count not for th
+00001a90: 6520 6365 7274 6966 6963 6174 6507 0000  e certificate...
+00001aa0: 0006 4469 616c 6f67 0103 0000 0020 0044  ..Dialog..... .D
+00001ab0: 0061 0074 0065 0069 00fc 0062 0065 0072  .a.t.e.i...b.e.r
+00001ac0: 0077 0061 0063 0068 0075 006e 0067 0800  .w.a.c.h.u.n.g..
+00001ad0: 0000 0006 0000 000a 5761 7463 6820 4669  ........Watch Fi
+00001ae0: 6c65 0700 0000 0644 6961 6c6f 6701 03ff  le.....Dialog...
+00001af0: ffff ff08 0000 0000 0600 0000 0465 5153  .............eQS
+00001b00: 4c07 0000 0006 4469 616c 6f67 0103 ffff  L.....Dialog....
+00001b10: ffff 0800 0000 0006 0000 0002 c2b0 0700  ................
+00001b20: 0000 0644 6961 6c6f 6701 0300 0000 9e00  ...Dialog.......
+00001b30: 4500 6900 6e00 2000 4400 6100 7400 6500  E.i.n. .D.a.t.e.
+00001b40: 6e00 6200 6100 6e00 6b00 2d00 4200 6100  n.b.a.n.k.-.B.a.
+00001b50: 6300 6b00 7500 7000 2000 6b00 6f00 6e00  c.k.u.p. .k.o.n.
+00001b60: 6e00 7400 6500 2000 6e00 6900 6300 6800  n.t.e. .n.i.c.h.
+00001b70: 7400 2000 6500 7200 7300 7400 6500 6c00  t. .e.r.s.t.e.l.
+00001b80: 6c00 7400 2000 7700 6500 7200 6400 6500  l.t. .w.e.r.d.e.
+00001b90: 6e00 2e00 0a00 4400 6900 6500 2000 4400  n.....D.i.e. .D.
+00001ba0: 6100 7400 6500 6900 2000 6500 7800 6900  a.t.e.i. .e.x.i.
+00001bb0: 7300 7400 6900 6500 7200 7400 2000 6200  s.t.i.e.r.t. .b.
+00001bc0: 6500 7200 6500 6900 7400 7300 2e08 0000  e.r.e.i.t.s.....
+00001bd0: 0000 0600 0000 4041 2064 6174 6162 6173  ......@A databas
+00001be0: 6520 6261 636b 7570 2063 6f75 6c64 206e  e backup could n
+00001bf0: 6f74 2062 6520 6372 6561 7465 642e 0a54  ot be created..T
+00001c00: 6865 2066 696c 6520 616c 7265 6164 7920  he file already 
+00001c10: 6578 6973 7473 2e07 0000 0009 4472 6167  exists......Drag
+00001c20: 6f6e 4c6f 6701 0300 0000 4e00 4500 6900  onLog.....N.E.i.
+00001c30: 6e00 2000 4100 4400 4900 4600 2d00 4600  n. .A.D.I.F.-.F.
+00001c40: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
+00001c50: 7400 2000 6600 fc00 7200 2000 6400 6500  t. .f...r. .d.e.
+00001c60: 6e00 2000 4c00 6f00 5400 5700 2d00 5500  n. .L.o.T.W.-.U.
+00001c70: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
+00001c80: 0000 1d41 2066 6965 6c64 2069 7320 6d69  ...A field is mi
+00001c90: 7373 696e 6720 666f 7220 7570 6c6f 6164  ssing for upload
+00001ca0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001cb0: ffff ffff 0800 0000 0006 0000 0015 4144  ..............AD
+00001cc0: 4946 2033 2028 2a2e 6164 6920 2a2e 6164  IF 3 (*.adi *.ad
+00001cd0: 6966 2907 0000 0009 4472 6167 6f6e 4c6f  if).....DragonLo
+00001ce0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001cf0: 1b41 4449 4620 3320 282a 2e61 6478 202a  .ADIF 3 (*.adx *
+00001d00: 2e61 6469 202a 2e61 6469 6629 0700 0000  .adi *.adif)....
+00001d10: 0944 7261 676f 6e4c 6f67 0103 0000 0008  .DragonLog......
+00001d20: 00dc 0062 0065 0072 0800 0000 0006 0000  ...b.e.r........
+00001d30: 0005 4162 6f75 7407 0000 0009 4472 6167  ..About.....Drag
+00001d40: 6f6e 4c6f 6701 0300 0000 0e00 dc00 6200  onLog.........b.
+00001d50: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
+00001d60: 0000 0841 626f 7574 2051 7407 0000 0009  ...About Qt.....
+00001d70: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
+00001d80: 4100 6900 7200 6300 7200 6100 6600 7400  A.i.r.c.r.a.f.t.
+00001d90: 2d00 5300 6300 6100 7400 7400 6500 7208  -.S.c.a.t.t.e.r.
+00001da0: 0000 0000 0600 0000 1041 6972 6372 6166  .........Aircraf
+00001db0: 7420 5363 6174 7465 7207 0000 0009 4472  t Scatter.....Dr
+00001dc0: 6167 6f6e 4c6f 6701 0300 0000 0e00 4100  agonLog.......A.
+00001dd0: 6e00 7400 6500 6e00 6e00 6508 0000 0000  n.t.e.n.n.e.....
+00001de0: 0600 0000 0741 6e74 656e 6e61 0700 0000  .....Antenna....
+00001df0: 0944 7261 676f 6e4c 6f67 0103 ffff ffff  .DragonLog......
+00001e00: 0800 0000 0006 0000 0006 4175 726f 7261  ..........Aurora
+00001e10: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001e20: ffff ffff 0800 0000 0006 0000 0008 4175  ..............Au
+00001e30: 726f 7261 2d45 0700 0000 0944 7261 676f  rora-E.....Drago
+00001e40: 6e4c 6f67 0103 0000 000a 0041 0075 0074  nLog.......A.u.t
+00001e50: 006f 0072 0800 0000 0006 0000 0006 4175  .o.r..........Au
+00001e60: 7468 6f72 0700 0000 0944 7261 676f 6e4c  thor.....DragonL
+00001e70: 6f67 0103 0000 0018 0042 0061 0063 006b  og.......B.a.c.k
+00001e80: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
+00001e90: 0800 0000 0006 0000 000c 4261 636b 2073  ..........Back s
+00001ea0: 6361 7474 6572 0700 0000 0944 7261 676f  catter.....Drago
+00001eb0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
+00001ec0: 0000 0004 4261 6e64 0700 0000 0944 7261  ....Band.....Dra
+00001ed0: 676f 6e4c 6f67 0103 0000 0022 0043 0053  gonLog.....".C.S
+00001ee0: 0056 002d 0044 0061 0074 0065 0069 0020  .V.-.D.a.t.e.i. 
+00001ef0: 0028 002a 002e 0063 0073 0076 0029 0800  .(.*...c.s.v.)..
+00001f00: 0000 0006 0000 0010 4353 562d 4669 6c65  ........CSV-File
+00001f10: 2028 2a2e 6373 7629 0700 0000 0944 7261   (*.csv).....Dra
+00001f20: 676f 6e4c 6f67 0103 0000 0014 0052 0075  gonLog.......R.u
+00001f30: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
+00001f40: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
+00001f50: 6967 6e07 0000 0009 4472 6167 6f6e 4c6f  ign.....DragonLo
+00001f60: 6701 0300 0000 0a00 4b00 6100 6e00 6100  g.......K.a.n.a.
+00001f70: 6c08 0000 0000 0600 0000 0743 6861 6e6e  l..........Chann
+00001f80: 656c 0700 0000 0944 7261 676f 6e4c 6f67  el.....DragonLog
+00001f90: 0103 0000 0074 0050 0072 00fc 0066 0075  .....t.P.r...f.u
+00001fa0: 006e 0067 0020 0064 0065 0072 0020 0044  .n.g. .d.e.r. .D
+00001fb0: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
+00001fc0: 0020 0066 0065 0068 006c 0067 0065 0073  . .f.e.h.l.g.e.s
+00001fd0: 0063 0068 006c 0061 0067 0065 006e 002e  .c.h.l.a.g.e.n..
+00001fe0: 0020 0049 006e 0068 0061 006c 0074 0020  . .I.n.h.a.l.t. 
+00001ff0: 006e 0069 0063 0068 0074 0020 006c 0065  .n.i.c.h.t. .l.e
+00002000: 0073 0062 0061 0072 002e 0800 0000 0006  .s.b.a.r........
+00002010: 0000 0034 4368 6563 6b69 6e67 2064 6174  ...4Checking dat
+00002020: 6162 6173 6520 6661 696c 6564 2e20 436f  abase failed. Co
+00002030: 6e74 656e 7420 6973 206e 6f74 2061 6363  ntent is not acc
+00002040: 6573 7361 626c 652e 0700 0000 0944 7261  essable......Dra
+00002050: 676f 6e4c 6f67 0103 0000 0014 004b 006f  gonLog.......K.o
+00002060: 006d 006d 0065 006e 0074 0061 0072 0065  .m.m.e.n.t.a.r.e
+00002070: 0800 0000 0006 0000 0008 436f 6d6d 656e  ..........Commen
+00002080: 7473 0700 0000 0944 7261 676f 6e4c 6f67  ts.....DragonLog
+00002090: 0103 0000 0060 0056 0065 0072 0062 0069  .....`.V.e.r.b.i
+000020a0: 006e 0064 0075 006e 0067 0073 0066 0065  .n.d.u.n.g.s.f.e
+000020b0: 0068 006c 0065 0072 0020 006f 0064 0065  .h.l.e.r. .o.d.e
+000020c0: 0072 0020 004e 0065 0074 007a 0077 0065  .r. .N.e.t.z.w.e
+000020d0: 0072 006b 0020 006e 0069 0063 0068 0074  .r.k. .n.i.c.h.t
+000020e0: 0020 0065 0072 0072 0065 0069 0063 0068  . .e.r.r.e.i.c.h
+000020f0: 0062 0061 0072 0800 0000 0006 0000 0027  .b.a.r.........'
+00002100: 436f 6e6e 6563 7469 6f6e 2065 7272 6f72  Connection error
+00002110: 206f 7220 6e65 7477 6f72 6b20 756e 7265   or network unre
+00002120: 6163 6861 626c 6507 0000 0009 4472 6167  achable.....Drag
+00002130: 6f6e 4c6f 6701 0300 0000 2e00 4400 6100  onLog.......D.a.
+00002140: 7400 6500 6e00 6200 6100 6e00 6b00 2d00  t.e.n.b.a.n.k.-.
+00002150: 4200 6100 6300 6b00 7500 7000 2000 4600  B.a.c.k.u.p. .F.
+00002160: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
+00002170: 0000 1544 6174 6162 6173 6520 6261 636b  ...Database back
+00002180: 7570 2065 7272 6f72 0700 0000 0944 7261  up error.....Dra
+00002190: 676f 6e4c 6f67 0103 0000 002c 0044 0061  gonLog.....,.D.a
+000021a0: 0074 0065 006e 0062 0061 006e 006b 006b  .t.e.n.b.a.n.k.k
+000021b0: 006f 006e 0076 0065 0072 0074 0069 0065  .o.n.v.e.r.t.i.e
+000021c0: 0072 0075 006e 0067 0800 0000 0006 0000  .r.u.n.g........
+000021d0: 0013 4461 7461 6261 7365 2063 6f6e 7665  ..Database conve
+000021e0: 7273 696f 6e07 0000 0009 4472 6167 6f6e  rsion.....Dragon
+000021f0: 4c6f 6701 0300 0000 4800 4400 6100 7400  Log.....H.D.a.t.
+00002200: 6500 6e00 6200 6100 6e00 6b00 6b00 6f00  e.n.b.a.n.k.k.o.
+00002210: 6e00 7600 6500 7200 7400 6900 6500 7200  n.v.e.r.t.i.e.r.
+00002220: 7500 6e00 6700 2000 6100 6200 6700 6500  u.n.g. .a.b.g.e.
+00002230: 7300 6300 6800 6c00 6f00 7300 7300 6500  s.c.h.l.o.s.s.e.
+00002240: 6e08 0000 0000 0600 0000 1c44 6174 6162  n..........Datab
+00002250: 6173 6520 636f 6e76 6572 7369 6f6e 2066  ase conversion f
+00002260: 696e 6973 6865 6407 0000 0009 4472 6167  inished.....Drag
+00002270: 6f6e 4c6f 6701 0300 0000 1e00 4400 6100  onLog.......D.a.
+00002280: 7400 6500 6e00 6200 6100 6e00 6b00 6600  t.e.n.b.a.n.k.f.
+00002290: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
+000022a0: 0000 0e44 6174 6162 6173 6520 6572 726f  ...Database erro
+000022b0: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+000022c0: 0300 0000 3400 4400 6100 7400 6500 6e00  ....4.D.a.t.e.n.
+000022d0: 6200 6100 6e00 6b00 7300 7400 7200 7500  b.a.n.k.s.t.r.u.
+000022e0: 6b00 7400 7500 7200 2000 7600 6500 7200  k.t.u.r. .v.e.r.
+000022f0: 6100 6c00 7400 6500 7408 0000 0000 0600  a.l.t.e.t.......
+00002300: 0000 1c44 6174 6162 6173 6520 7374 7275  ...Database stru
+00002310: 6374 7572 6520 6f75 742d 6461 7465 6407  cture out-dated.
+00002320: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002330: 0000 1e00 4400 6100 7400 7500 6d00 2f00  ....D.a.t.u.m./.
+00002340: 5a00 6500 6900 7400 2000 4500 6e00 6400  Z.e.i.t. .E.n.d.
+00002350: 6508 0000 0000 0600 0000 0d44 6174 652f  e..........Date/
+00002360: 5469 6d65 2065 6e64 0700 0000 0944 7261  Time end.....Dra
+00002370: 676f 6e4c 6f67 0103 0000 0020 0044 0061  gonLog..... .D.a
+00002380: 0074 0075 006d 002f 005a 0065 0069 0074  .t.u.m./.Z.e.i.t
+00002390: 0020 0053 0074 0061 0072 0074 0800 0000  . .S.t.a.r.t....
+000023a0: 0006 0000 000f 4461 7465 2f54 696d 6520  ......Date/Time 
+000023b0: 7374 6172 7407 0000 0009 4472 6167 6f6e  start.....Dragon
+000023c0: 4c6f 6701 0300 0000 1600 5100 5300 4f00  Log.......Q.S.O.
+000023d0: 2000 6c00 f600 7300 6300 6800 6500 6e08   .l...s.c.h.e.n.
+000023e0: 0000 0000 0600 0000 0a44 656c 6574 6520  .........Delete 
+000023f0: 5153 4f07 0000 0009 4472 6167 6f6e 4c6f  QSO.....DragonLo
+00002400: 6701 0300 0000 1400 4500 6e00 7400 6600  g.......E.n.t.f.
+00002410: 6500 7200 6e00 7500 6e00 6708 0000 0000  e.r.n.u.n.g.....
+00002420: 0600 0000 0844 6973 7461 6e63 6507 0000  .....Distance...
+00002430: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002440: 6400 5700 6f00 6c00 6c00 6500 6e00 2000  d.W.o.l.l.e.n. .
+00002450: 7300 6900 6500 2000 6400 6900 6500 2000  s.i.e. .d.i.e. .
+00002460: 7300 6500 6c00 6500 6b00 7400 6900 6500  s.e.l.e.k.t.i.e.
+00002470: 7200 7400 6500 6e00 2000 5100 5300 4f00  r.t.e.n. .Q.S.O.
+00002480: 7300 2000 7700 6900 7200 6b00 6c00 6900  s. .w.i.r.k.l.i.
+00002490: 6300 6800 2000 6c00 f600 7300 6300 6800  c.h. .l...s.c.h.
+000024a0: 6500 6e00 3f08 0000 0000 0600 0000 3144  e.n.?.........1D
+000024b0: 6f20 796f 7520 7265 616c 6c79 2077 616e  o you really wan
+000024c0: 7420 746f 2064 656c 6574 6520 7468 6520  t to delete the 
+000024d0: 7365 6c65 6374 6564 2051 534f 2873 293f  selected QSO(s)?
+000024e0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000024f0: ffff ffff 0800 0000 0006 0000 0010 4561  ..............Ea
+00002500: 7274 682d 4d6f 6f6e 2d45 6172 7468 0700  rth-Moon-Earth..
+00002510: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00002520: ffff 0800 0000 0006 0000 0008 4563 686f  ............Echo
+00002530: 4c69 6e6b 0700 0000 0944 7261 676f 6e4c  Link.....DragonL
+00002540: 6f67 0103 0000 000c 0046 0065 0068 006c  og.......F.e.h.l
+00002550: 0065 0072 0800 0000 0006 0000 0005 4572  .e.r..........Er
+00002560: 726f 7207 0000 0009 4472 6167 6f6e 4c6f  ror.....DragonLo
+00002570: 6701 0300 0000 2800 4500 7800 6300 6500  g.....(.E.x.c.e.
+00002580: 6c00 2d00 4400 6100 7400 6500 6900 2000  l.-.D.a.t.e.i. .
+00002590: 2800 2a00 2e00 7800 6c00 7300 7800 2908  (.*...x.l.s.x.).
+000025a0: 0000 0000 0600 0000 1345 7863 656c 2d46  .........Excel-F
+000025b0: 696c 6520 282a 2e78 6c73 7829 0700 0000  ile (*.xlsx)....
+000025c0: 0944 7261 676f 6e4c 6f67 0103 0000 0024  .DragonLog.....$
+000025d0: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
+000025e0: 0072 0065 0020 0051 0053 004f 0020 006c  .r.e. .Q.S.O. .l
+000025f0: 006f 0067 0800 0000 0006 0000 0010 4578  .o.g..........Ex
+00002600: 706f 7274 6564 2051 534f 206c 6f67 0700  ported QSO log..
+00002610: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002620: 001a 0046 0032 002d 0052 0065 0066 006c  ...F.2.-.R.e.f.l
+00002630: 0065 006b 0074 0069 006f 006e 0800 0000  .e.k.t.i.o.n....
+00002640: 0006 0000 000d 4632 2052 6566 6c65 6374  ......F2 Reflect
+00002650: 696f 6e07 0000 0009 4472 6167 6f6e 4c6f  ion.....DragonLo
+00002660: 6701 0300 0000 3800 4600 6900 6500 6c00  g.....8.F.i.e.l.
+00002670: 6400 2d00 4100 6c00 6900 6700 6e00 6500  d.-.A.l.i.g.n.e.
+00002680: 6400 2d00 4900 7200 7200 6500 6700 7500  d.-.I.r.r.e.g.u.
+00002690: 6c00 6100 7200 6900 7400 6900 6500 7308  l.a.r.i.t.i.e.s.
+000026a0: 0000 0000 0600 0000 1c46 6965 6c64 2041  .........Field A
+000026b0: 6c69 676e 6564 2049 7272 6567 756c 6172  ligned Irregular
+000026c0: 6974 6965 7307 0000 0009 4472 6167 6f6e  ities.....Dragon
+000026d0: 4c6f 6701 0300 0000 1000 4600 7200 6500  Log.......F.r.e.
+000026e0: 7100 7500 6500 6e00 7a08 0000 0000 0600  q.u.e.n.z.......
+000026f0: 0000 0946 7265 7175 656e 6379 0700 0000  ...Frequency....
+00002700: 0944 7261 676f 6e4c 6f67 0103 0000 0014  .DragonLog......
+00002710: 0042 006f 0064 0065 006e 0077 0065 006c  .B.o.d.e.n.w.e.l
+00002720: 006c 0065 0800 0000 0006 0000 000b 4772  .l.e..........Gr
+00002730: 6f75 6e64 2057 6176 6507 0000 0009 4472  ound Wave.....Dr
+00002740: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
+00002750: 0000 0600 0000 0648 616d 5154 4807 0000  .......HamQTH...
+00002760: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+00002770: ff08 0000 0000 0600 0000 0648 616d 6c69  ...........Hamli
+00002780: 6207 0000 0009 4472 6167 6f6e 4c6f 6701  b.....DragonLog.
+00002790: 0300 0000 0a00 4800 6900 6c00 6600 6508  ......H.i.l.f.e.
+000027a0: 0000 0000 0600 0000 0448 656c 7007 0000  .........Help...
+000027b0: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+000027c0: ff08 0000 0000 0600 0000 0449 524c 5007  ...........IRLP.
+000027d0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+000027e0: 0000 2600 4900 6e00 7400 6500 7200 6e00  ..&.I.n.t.e.r.n.
+000027f0: 6500 7400 7500 6e00 7400 6500 7200 7300  e.t.u.n.t.e.r.s.
+00002800: 7400 fc00 7400 7a00 7408 0000 0000 0600  t...t.z.t.......
+00002810: 0000 1149 6e74 6572 6e65 742d 6173 7369  ...Internet-assi
+00002820: 7374 6564 0700 0000 0944 7261 676f 6e4c  sted.....DragonL
+00002830: 6f67 0103 0000 0018 0049 006f 006e 006f  og.......I.o.n.o
+00002840: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
+00002850: 0800 0000 0006 0000 000b 496f 6e6f 7363  ..........Ionosc
+00002860: 6174 7465 7207 0000 0009 4472 6167 6f6e  atter.....Dragon
+00002870: 4c6f 6701 0300 0000 2000 6c00 6500 7400  Log..... .l.e.t.
+00002880: 7a00 7400 6500 7300 2000 4800 6100 6c00  z.t.e.s. .H.a.l.
+00002890: 6200 6a00 6100 6800 7208 0000 0000 0600  b.j.a.h.r.......
+000028a0: 0000 0e4c 6173 7420 6861 6c66 2079 6561  ...Last half yea
+000028b0: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+000028c0: 0300 0000 1a00 6c00 6500 7400 7a00 7400  ......l.e.t.z.t.
+000028d0: 6500 6e00 2000 4d00 6f00 6e00 6100 7408  e.n. .M.o.n.a.t.
+000028e0: 0000 0000 0600 0000 0a4c 6173 7420 6d6f  .........Last mo
+000028f0: 6e74 6807 0000 0009 4472 6167 6f6e 4c6f  nth.....DragonLo
+00002900: 6701 0300 0000 1800 6c00 6500 7400 7a00  g.......l.e.t.z.
+00002910: 7400 6500 2000 5700 6f00 6300 6800 6508  t.e. .W.o.c.h.e.
+00002920: 0000 0000 0600 0000 094c 6173 7420 7765  .........Last we
+00002930: 656b 0700 0000 0944 7261 676f 6e4c 6f67  ek.....DragonLog
+00002940: 0103 0000 0018 006c 0065 0074 007a 0074  .......l.e.t.z.t
+00002950: 0065 0073 0020 004a 0061 0068 0072 0800  .e.s. .J.a.h.r..
+00002960: 0000 0006 0000 0009 4c61 7374 2079 6561  ........Last yea
+00002970: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+00002980: 0300 0000 1e00 5300 6900 6300 6800 7400  ......S.i.c.h.t.
+00002990: 7600 6500 7200 6200 6900 6e00 6400 7500  v.e.r.b.i.n.d.u.
+000029a0: 6e00 6708 0000 0000 0600 0000 0d4c 696e  n.g..........Lin
+000029b0: 6520 6f66 2053 6967 6874 0700 0000 0944  e of Sight.....D
+000029c0: 7261 676f 6e4c 6f67 0103 0000 0020 004c  ragonLog..... .L
+000029d0: 006f 0054 0057 002d 0041 0044 0049 0046  .o.T.W.-.A.D.I.F
+000029e0: 002d 0055 0070 006c 006f 0061 0064 0800  .-.U.p.l.o.a.d..
+000029f0: 0000 0006 0000 0010 4c6f 5457 2041 4449  ........LoTW ADI
+00002a00: 4620 7570 6c6f 6164 0700 0000 0944 7261  F upload.....Dra
+00002a10: 676f 6e4c 6f67 0103 0000 0014 004c 006f  gonLog.......L.o
+00002a20: 0054 0057 0020 0065 006d 0070 0066 002e  .T.W. .e.m.p.f..
+00002a30: 0800 0000 0006 0000 0009 4c6f 5457 2072  ..........LoTW r
+00002a40: 6376 6407 0000 0009 4472 6167 6f6e 4c6f  cvd.....DragonLo
+00002a50: 6701 0300 0000 1400 4c00 6f00 5400 5700  g.......L.o.T.W.
+00002a60: 2000 7600 6500 7200 7300 2e08 0000 0000   .v.e.r.s.......
+00002a70: 0600 0000 094c 6f54 5720 7365 6e74 0700  .....LoTW sent..
+00002a80: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00002a90: ffff 0800 0000 0006 0000 0007 4c6f 6361  ............Loca
+00002aa0: 746f 7207 0000 0009 4472 6167 6f6e 4c6f  tor.....DragonLo
+00002ab0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00002ac0: 0f4c 6f67 2069 6d70 6f72 7420 4144 4946  .Log import ADIF
+00002ad0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002ae0: 0000 001c 004c 006f 0067 0020 0049 006d  .....L.o.g. .I.m
+00002af0: 0070 006f 0072 0074 0020 0043 0053 0056  .p.o.r.t. .C.S.V
+00002b00: 0800 0000 0006 0000 000e 4c6f 6720 696d  ..........Log im
+00002b10: 706f 7274 2043 5356 0700 0000 0944 7261  port CSV.....Dra
+00002b20: 676f 6e4c 6f67 0103 0000 0020 004c 006f  gonLog..... .L.o
+00002b30: 0067 0020 0049 006d 0070 006f 0072 0074  .g. .I.m.p.o.r.t
+00002b40: 0020 0045 0078 0063 0065 006c 0800 0000  . .E.x.c.e.l....
+00002b50: 0006 0000 0010 4c6f 6720 696d 706f 7274  ......Log import
+00002b60: 2045 7863 656c 0700 0000 0944 7261 676f   Excel.....Drago
+00002b70: 6e4c 6f67 0103 0000 001c 004d 0065 0074  nLog.......M.e.t
+00002b80: 0065 006f 0072 002d 0053 0063 0061 0074  .e.o.r.-.S.c.a.t
+00002b90: 0074 0065 0072 0800 0000 0006 0000 000e  .t.e.r..........
+00002ba0: 4d65 7465 6f72 2073 6361 7474 6572 0700  Meteor scatter..
+00002bb0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002bc0: 005a 004b 0065 0069 006e 0065 0020 0053  .Z.K.e.i.n.e. .S
+00002bd0: 0074 0061 0074 0069 006f 006e 0073 006b  .t.a.t.i.o.n.s.k
+00002be0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
+00002bf0: 0074 0069 006f 006e 0020 0069 006e 0020  .t.i.o.n. .i.n. 
+00002c00: 0054 0051 0053 004c 0020 0076 0065 0072  .T.Q.S.L. .v.e.r
+00002c10: 0066 00fc 0067 0062 0061 0072 0800 0000  .f...g.b.a.r....
+00002c20: 0006 0000 0025 4d69 7373 696e 6720 7374  .....%Missing st
+00002c30: 6174 696f 6e20 636f 6e66 6967 7572 6174  ation configurat
+00002c40: 696f 6e20 696e 2054 5153 4c07 0000 0009  ion in TQSL.....
+00002c50: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00002c60: 0000 0000 0600 0000 044d 6f64 6507 0000  .........Mode...
+00002c70: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+00002c80: ff08 0000 0000 0600 0000 044e 616d 6507  ...........Name.
+00002c90: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002ca0: 0000 3400 4b00 6500 6900 6e00 6500 2000  ..4.K.e.i.n.e. .
+00002cb0: 5100 5300 4f00 7300 2000 6600 fc00 7200  Q.S.O.s. .f...r.
+00002cc0: 2000 6400 6500 6e00 2000 4c00 6f00 6300   .d.e.n. .L.o.c.
+00002cd0: 6100 7400 6f00 7208 0000 0000 0600 0000  a.t.o.r.........
+00002ce0: 174e 6f20 7265 636f 7264 7320 666f 7220  .No records for 
+00002cf0: 6c6f 6361 7469 6f6e 0700 0000 0944 7261  location.....Dra
+00002d00: 676f 6e4c 6f67 0103 0000 000e 004e 006f  gonLog.......N.o
+00002d10: 0074 0069 007a 0065 006e 0800 0000 0006  .t.i.z.e.n......
+00002d20: 0000 0005 4e6f 7465 7307 0000 0009 4472  ....Notes.....Dr
+00002d30: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
+00002d40: 0000 0600 0000 024f 6b07 0000 0009 4472  .......Ok.....Dr
+00002d50: 6167 6f6e 4c6f 6701 0300 0000 1e00 4500  agonLog.......E.
+00002d60: 6900 6700 6500 6e00 6500 7200 2000 4c00  i.g.e.n.e.r. .L.
+00002d70: 6f00 6300 6100 7400 6f00 7208 0000 0000  o.c.a.t.o.r.....
+00002d80: 0600 0000 0b4f 776e 204c 6f63 6174 6f72  .....Own Locator
+00002d90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002da0: 0000 0018 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
+00002db0: 0072 0020 004e 0061 006d 0065 0800 0000  .r. .N.a.m.e....
+00002dc0: 0006 0000 0008 4f77 6e20 4e61 6d65 0700  ......Own Name..
+00002dd0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002de0: 0016 0045 0069 0067 0065 006e 0065 0072  ...E.i.g.e.n.e.r
+00002df0: 0020 0051 0054 0048 0800 0000 0006 0000  . .Q.T.H........
+00002e00: 0007 4f77 6e20 5154 4807 0000 0009 4472  ..Own QTH.....Dr
+00002e10: 6167 6f6e 4c6f 6701 0300 0000 2400 4500  agonLog.....$.E.
+00002e20: 6900 6700 6500 6e00 6500 7300 2000 5200  i.g.e.n.e.s. .R.
+00002e30: 7500 6600 7a00 6500 6900 6300 6800 6500  u.f.z.e.i.c.h.e.
+00002e40: 6e08 0000 0000 0600 0000 0d4f 776e 2063  n..........Own c
+00002e50: 616c 6c20 7369 676e 0700 0000 0944 7261  all sign.....Dra
+00002e60: 676f 6e4c 6f67 0103 0000 0010 004c 0065  gonLog.......L.e
+00002e70: 0069 0073 0074 0075 006e 0067 0800 0000  .i.s.t.u.n.g....
+00002e80: 0006 0000 0005 506f 7765 7207 0000 0009  ......Power.....
+00002e90: 4472 6167 6f6e 4c6f 6701 0300 0000 1600  DragonLog.......
+00002ea0: 4100 7500 7300 6200 7200 6500 6900 7400  A.u.s.b.r.e.i.t.
+00002eb0: 7500 6e00 6708 0000 0000 0600 0000 0b50  u.n.g..........P
+00002ec0: 726f 7061 6761 7469 6f6e 0700 0000 0944  ropagation.....D
+00002ed0: 7261 676f 6e4c 6f67 0103 0000 001a 0051  ragonLog.......Q
+00002ee0: 0053 004c 002d 004e 0061 0063 0068 0072  .S.L.-.N.a.c.h.r
+00002ef0: 0069 0063 0068 0074 0800 0000 0006 0000  .i.c.h.t........
+00002f00: 000b 5153 4c20 6d65 7373 6167 6507 0000  ..QSL message...
+00002f10: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002f20: 1000 5100 5300 4c00 2d00 5000 6600 6100  ..Q.S.L.-.P.f.a.
+00002f30: 6408 0000 0000 0600 0000 0851 534c 2070  d..........QSL p
+00002f40: 6174 6807 0000 0009 4472 6167 6f6e 4c6f  ath.....DragonLo
+00002f50: 6701 0300 0000 1200 5100 5300 4c00 2000  g.......Q.S.L. .
+00002f60: 6500 6d00 7000 6600 2e08 0000 0000 0600  e.m.p.f.........
+00002f70: 0000 0851 534c 2072 6376 6407 0000 0009  ...QSL rcvd.....
+00002f80: 4472 6167 6f6e 4c6f 6701 0300 0000 1200  DragonLog.......
+00002f90: 5100 5300 4c00 2000 7600 6500 7200 7300  Q.S.L. .v.e.r.s.
+00002fa0: 2e08 0000 0000 0600 0000 0851 534c 2073  ...........QSL s
+00002fb0: 656e 7407 0000 0009 4472 6167 6f6e 4c6f  ent.....DragonLo
+00002fc0: 6701 0300 0000 0e00 5100 5300 4c00 2d00  g.......Q.S.L.-.
+00002fd0: 5600 6900 6108 0000 0000 0600 0000 0751  V.i.a..........Q
+00002fe0: 534c 2076 6961 0700 0000 0944 7261 676f  SL via.....Drago
+00002ff0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
+00003000: 0000 0003 5153 4f07 0000 0009 4472 6167  ....QSO.....Drag
+00003010: 6f6e 4c6f 6701 0300 0000 4800 5100 5300  onLog.....H.Q.S.
+00003020: 4f00 2d00 4c00 6f00 6700 2000 2800 2a00  O.-.L.o.g. .(.*.
+00003030: 2e00 7100 6c00 6f00 6700 2900 3b00 3b00  ..q.l.o.g.).;.;.
+00003040: 4100 6c00 6c00 6500 2000 4400 6100 7400  A.l.l.e. .D.a.t.
+00003050: 6500 6900 6500 6e00 2000 2800 2a00 2e00  e.i.e.n. .(.*...
+00003060: 2a00 2908 0000 0000 0600 0000 2151 534f  *.).........!QSO
+00003070: 2d4c 6f67 2028 2a2e 716c 6f67 293b 3b41  -Log (*.qlog);;A
+00003080: 6c6c 2046 696c 6573 2028 2a2e 2a29 0700  ll Files (*.*)..
+00003090: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+000030a0: ffff 0800 0000 0006 0000 0003 5154 4807  ............QTH.
+000030b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+000030c0: 0000 1200 5200 5300 5400 2000 6500 6d00  ....R.S.T. .e.m.
+000030d0: 7000 6600 2e08 0000 0000 0600 0000 0852  p.f............R
+000030e0: 5354 2072 6376 6407 0000 0009 4472 6167  ST rcvd.....Drag
+000030f0: 6f6e 4c6f 6701 0300 0000 1000 5200 5300  onLog.......R.S.
+00003100: 5400 2000 6700 6500 7300 2e08 0000 0000  T. .g.e.s.......
+00003110: 0600 0000 0852 5354 2073 656e 7407 0000  .....RST sent...
+00003120: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+00003130: ff08 0000 0000 0600 0000 0552 6164 696f  ...........Radio
+00003140: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003150: 0000 0018 0052 0061 0069 006e 002d 0053  .....R.a.i.n.-.S
+00003160: 0063 0061 0074 0074 0065 0072 0800 0000  .c.a.t.t.e.r....
+00003170: 0006 0000 000c 5261 696e 2073 6361 7474  ......Rain scatt
+00003180: 6572 0700 0000 0944 7261 676f 6e4c 6f67  er.....DragonLog
+00003190: 0103 0000 0032 0052 0065 0070 0065 0061  .....2.R.e.p.e.a
+000031a0: 0074 0065 0072 0020 006f 0064 0065 0072  .t.e.r. .o.d.e.r
+000031b0: 0020 0054 0072 0061 006e 0073 0070 006f  . .T.r.a.n.s.p.o
+000031c0: 006e 0064 0065 0072 0800 0000 0006 0000  .n.d.e.r........
+000031d0: 0017 5265 7065 6174 6572 206f 7220 5472  ..Repeater or Tr
+000031e0: 616e 7370 6f6e 6465 7207 0000 0009 4472  ansponder.....Dr
+000031f0: 6167 6f6e 4c6f 6701 0300 0000 1000 5300  agonLog.......S.
+00003200: 6100 7400 6500 6c00 6c00 6900 7408 0000  a.t.e.l.l.i.t...
+00003210: 0000 0600 0000 0953 6174 656c 6c69 7465  .......Satellite
+00003220: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003230: 0000 002a 0045 0078 0070 006f 0072 0074  ...*.E.x.p.o.r.t
+00003240: 0064 0061 0074 0065 0069 0020 0073 0070  .d.a.t.e.i. .s.p
+00003250: 0065 0069 0063 0068 0065 0072 006e 0800  .e.i.c.h.e.r.n..
+00003260: 0000 0006 0000 0012 5365 6c65 6374 2065  ........Select e
+00003270: 7870 6f72 7420 6669 6c65 0700 0000 0944  xport file.....D
+00003280: 7261 676f 6e4c 6f67 0103 0000 0020 0044  ragonLog..... .D
+00003290: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
+000032a0: 0020 00f6 0066 0066 006e 0065 006e 0800  . ...f.f.n.e.n..
+000032b0: 0000 0006 0000 000b 5365 6c65 6374 2066  ........Select f
+000032c0: 696c 6507 0000 0009 4472 6167 6f6e 4c6f  ile.....DragonLo
+000032d0: 6701 0300 0000 3800 5a00 7500 2000 fc00  g.....8.Z.u. ...
+000032e0: 6200 6500 7200 7700 6100 6300 6800 6500  b.e.r.w.a.c.h.e.
+000032f0: 6e00 6400 6500 2000 4400 6100 7400 6500  n.d.e. .D.a.t.e.
+00003300: 6900 2000 7700 e400 6800 6c00 6500 6e08  i. .w...h.l.e.n.
+00003310: 0000 0000 0600 0000 1453 656c 6563 7420  .........Select 
+00003320: 6669 6c65 2074 6f20 7761 7463 6807 0000  file to watch...
+00003330: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00003340: 2400 4900 6d00 7000 6f00 7200 7400 6400  $.I.m.p.o.r.t.d.
+00003350: 6100 7400 6500 6900 2000 f600 6600 6600  a.t.e.i. ...f.f.
+00003360: 6e00 6500 6e08 0000 0000 0600 0000 1253  n.e.n..........S
+00003370: 656c 6563 7420 696d 706f 7274 2066 696c  elect import fil
+00003380: 6507 0000 0009 4472 6167 6f6e 4c6f 6701  e.....DragonLog.
+00003390: 0300 0000 1a00 5700 e400 6800 6c00 6500  ......W...h.l.e.
+000033a0: 2000 5300 7400 6100 7400 6900 6f00 6e08   .S.t.a.t.i.o.n.
+000033b0: 0000 0000 0600 0000 0e53 656c 6563 7420  .........Select 
+000033c0: 7374 6174 696f 6e07 0000 0009 4472 6167  station.....Drag
+000033d0: 6f6e 4c6f 6701 0300 0000 4400 4c00 6f00  onLog.....D.L.o.
+000033e0: 5400 5700 2d00 5300 6500 7200 7600 6500  T.W.-.S.e.r.v.e.
+000033f0: 7200 2000 6800 6100 7400 2000 6400 6100  r. .h.a.t. .d.a.
+00003400: 7300 2000 4c00 6f00 6700 2000 6100 6200  s. .L.o.g. .a.b.
+00003410: 6700 6500 7700 6900 6500 7300 6500 6e08  g.e.w.i.e.s.e.n.
+00003420: 0000 0000 0600 0000 1353 6572 7665 7220  .........Server 
+00003430: 7265 6a65 6374 6564 206c 6f67 0700 0000  rejected log....
+00003440: 0944 7261 676f 6e4c 6f67 0103 0000 0014  .DragonLog......
+00003450: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
+00003460: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
+00003470: 6f77 2061 6c6c 0700 0000 0944 7261 676f  ow all.....Drago
+00003480: 6e4c 6f67 0103 0000 0014 0053 0070 006f  nLog.......S.p.o
+00003490: 0072 0061 0064 0069 0063 002d 0045 0800  .r.a.d.i.c.-.E..
+000034a0: 0000 0006 0000 000a 5370 6f72 6164 6963  ........Sporadic
+000034b0: 2045 0700 0000 0944 7261 676f 6e4c 6f67   E.....DragonLog
+000034c0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+000034d0: 5375 626d 6f64 6507 0000 0009 4472 6167  Submode.....Drag
+000034e0: 6f6e 4c6f 6701 0300 0000 2a00 5400 5100  onLog.....*.T.Q.
+000034f0: 5300 4c00 2d00 5300 6900 6700 6e00 6100  S.L.-.S.i.g.n.a.
+00003500: 7400 7500 7200 7000 6100 7300 7300 7700  t.u.r.p.a.s.s.w.
+00003510: 6f00 7200 7408 0000 0000 0600 0000 1754  o.r.t..........T
+00003520: 5153 4c20 7369 676e 6174 7572 6520 7061  QSL signature pa
+00003530: 7373 776f 7264 0700 0000 0944 7261 676f  ssword.....Drago
+00003540: 6e4c 6f67 0103 0000 00b2 0044 0069 0065  nLog.......D.i.e
+00003550: 0020 0044 0061 0074 0065 006e 0062 0061  . .D.a.t.e.n.b.a
+00003560: 006e 006b 0073 0074 0072 0075 006b 0074  .n.k.s.t.r.u.k.t
+00003570: 0075 0072 0020 0069 0073 0074 0020 0076  .u.r. .i.s.t. .v
+00003580: 0065 0072 0061 006c 0074 0065 0074 0020  .e.r.a.l.t.e.t. 
+00003590: 0075 006e 0064 0020 006d 0075 0073 0073  .u.n.d. .m.u.s.s
+000035a0: 0020 006b 006f 006e 0076 0065 0072 0074  . .k.o.n.v.e.r.t
+000035b0: 0069 0065 0072 0074 0020 0077 0065 0072  .i.e.r.t. .w.e.r
+000035c0: 0064 0065 006e 000a 000a 0045 0069 006e  .d.e.n.....E.i.n
+000035d0: 0020 0042 0061 0063 006b 0075 0070 0020  . .B.a.c.k.u.p. 
+000035e0: 0077 0069 0072 0064 0020 0065 0072 0073  .w.i.r.d. .e.r.s
+000035f0: 0074 0065 006c 006c 0074 003a 0800 0000  .t.e.l.l.t.:....
+00003600: 0006 0000 0057 5468 6520 6461 7461 6261  .....WThe databa
+00003610: 7365 2073 7472 7563 7475 7265 2069 7320  se structure is 
+00003620: 6f75 742d 6461 7465 6420 616e 6420 6e65  out-dated and ne
+00003630: 6564 7320 6120 636f 6e76 6572 7369 6f6e  eds a conversion
+00003640: 0a0a 4120 6261 636b 7570 2077 696c 6c20  ..A backup will 
+00003650: 6265 2067 656e 6572 6174 6564 3a07 0000  be generated:...
+00003660: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00003670: 1e00 5400 7200 6100 6e00 7300 6500 7100  ..T.r.a.n.s.e.q.
+00003680: 7500 6100 7400 6f00 7200 6900 6100 6c08  u.a.t.o.r.i.a.l.
+00003690: 0000 0000 0600 0000 1054 7261 6e73 2d65  .........Trans-e
+000036a0: 7175 6174 6f72 6961 6c07 0000 0009 4472  quatorial.....Dr
+000036b0: 6167 6f6e 4c6f 6701 0300 0000 2800 5400  agonLog.....(.T.
+000036c0: 7200 6f00 7000 6f00 7300 7000 6800 6500  r.o.p.o.s.p.h.e.
+000036d0: 7200 6900 6300 2d00 4400 7500 6300 7400  r.i.c.-.D.u.c.t.
+000036e0: 6900 6e00 6708 0000 0000 0600 0000 1454  i.n.g..........T
+000036f0: 726f 706f 7370 6865 7269 6320 6475 6374  ropospheric duct
+00003700: 696e 6707 0000 0009 4472 6167 6f6e 4c6f  ing.....DragonLo
+00003710: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00003720: 0756 6572 7369 6f6e 0700 0000 0944 7261  .Version.....Dra
+00003730: 676f 6e4c 6f67 0103 0000 002c 0050 0072  gonLog.....,.P.r
+00003740: 006f 0067 0072 0061 006d 006d 006c 006f  .o.g.r.a.m.m.l.o
+00003750: 0067 0020 00fc 0062 0065 0072 0077 0061  .g. ...b.e.r.w.a
+00003760: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
+00003770: 0015 5761 7463 6820 6170 706c 6963 6174  ..Watch applicat
+00003780: 696f 6e20 6c6f 6707 0000 0009 4472 6167  ion log.....Drag
+00003790: 6f6e 4c6f 6701 0300 0000 2000 4400 6100  onLog..... .D.a.
+000037a0: 7400 6500 6900 fc00 6200 6500 7200 7700  t.e.i...b.e.r.w.
+000037b0: 6100 6300 6800 7500 6e00 6708 0000 0000  a.c.h.u.n.g.....
+000037c0: 0600 0000 0d57 6174 6368 696e 6720 6669  .....Watching fi
+000037d0: 6c65 0700 0000 0944 7261 676f 6e4c 6f67  le.....DragonLog
+000037e0: 0103 0000 0014 0065 0051 0053 004c 0020  .......e.Q.S.L. 
+000037f0: 0065 006d 0070 0066 002e 0800 0000 0006  .e.m.p.f........
+00003800: 0000 0009 6551 534c 2072 6376 6407 0000  ....eQSL rcvd...
+00003810: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00003820: 1400 6500 5100 5300 4c00 2000 7600 6500  ..e.Q.S.L. .v.e.
+00003830: 7200 7300 2e08 0000 0000 0600 0000 0965  r.s............e
+00003840: 5153 4c20 7365 6e74 0700 0000 0944 7261  QSL sent.....Dra
+00003850: 676f 6e4c 6f67 0103 0000 000e 0069 006e  gonLog.......i.n
+00003860: 0061 006b 0074 0069 0076 0800 0000 0006  .a.k.t.i.v......
+00003870: 0000 0007 696e 6163 7469 7607 0000 0009  ....inactiv.....
+00003880: 4472 6167 6f6e 4c6f 6701 0300 0000 0800  DragonLog.......
+00003890: dc00 6200 6500 7208 0000 0000 0600 0000  ..b.e.r.........
+000038a0: 0541 626f 7574 0700 0000 0a4d 6169 6e57  .About.....MainW
+000038b0: 696e 646f 7701 0300 0000 0e00 dc00 6200  indow.........b.
+000038c0: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
+000038d0: 0000 0841 626f 7574 2051 7407 0000 000a  ...About Qt.....
+000038e0: 4d61 696e 5769 6e64 6f77 0103 0000 001a  MainWindow......
+000038f0: 0041 006e 0077 0065 006e 0064 0075 006e  .A.n.w.e.n.d.u.n
+00003900: 0067 0073 006c 006f 0067 0800 0000 0006  .g.s.l.o.g......
+00003910: 0000 000f 4170 706c 6963 6174 696f 6e20  ....Application 
+00003920: 4c6f 6707 0000 000a 4d61 696e 5769 6e64  Log.....MainWind
+00003930: 6f77 0103 0000 0022 0045 0069 006e 0074  ow.....".E.i.n.t
+00003940: 0072 0061 0067 0020 00e4 006e 0064 0065  .r.a.g. ...n.d.e
+00003950: 0072 006e 002e 002e 002e 0800 0000 0006  .r.n............
+00003960: 0000 0013 4368 616e 6765 206c 6f67 2065  ....Change log e
+00003970: 6e74 7279 2e2e 2e07 0000 000a 4d61 696e  ntry........Main
+00003980: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
+00003990: 0006 0000 0006 4374 726c 2b45 0700 0000  ......Ctrl+E....
+000039a0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
+000039b0: ff08 0000 0000 0600 0000 0643 7472 6c2b  ...........Ctrl+
+000039c0: 4c07 0000 000a 4d61 696e 5769 6e64 6f77  L.....MainWindow
+000039d0: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
+000039e0: 4374 726c 2b51 0700 0000 0a4d 6169 6e57  Ctrl+Q.....MainW
+000039f0: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
+00003a00: 0600 0000 0643 7472 6c2b 5707 0000 000a  .....Ctrl+W.....
+00003a10: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
+00003a20: 0800 0000 0006 0000 0006 4374 726c 2b58  ..........Ctrl+X
+00003a30: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003a40: 0300 0000 1e00 4500 6900 6e00 7400 7200  ......E.i.n.t.r.
+00003a50: 6100 6700 2000 6c00 f600 7300 6300 6800  a.g. .l...s.c.h.
+00003a60: 6500 6e08 0000 0000 0600 0000 1044 656c  e.n..........Del
+00003a70: 6574 6520 6c6f 6720 656e 7472 7907 0000  ete log entry...
+00003a80: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
+00003a90: ffff 0800 0000 0006 0000 0009 4472 6167  ............Drag
+00003aa0: 6f6e 4c6f 6707 0000 000a 4d61 696e 5769  onLog.....MainWi
+00003ab0: 6e64 6f77 0103 0000 0014 0042 0065 0061  ndow.......B.e.a
+00003ac0: 0072 0062 0065 0069 0074 0065 006e 0800  .r.b.e.i.t.e.n..
+00003ad0: 0000 0006 0000 0004 4564 6974 0700 0000  ........Edit....
+00003ae0: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
+00003af0: 0e00 4200 6500 6500 6e00 6400 6500 6e08  ..B.e.e.n.d.e.n.
+00003b00: 0000 0000 0600 0000 0445 7869 7407 0000  .........Exit...
+00003b10: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
+00003b20: ffff 0800 0000 0006 0000 0006 4578 706f  ............Expo
+00003b30: 7274 0700 0000 0a4d 6169 6e57 696e 646f  rt.....MainWindo
+00003b40: 7701 0300 0000 1c00 4500 7800 7000 6f00  w.......E.x.p.o.
+00003b50: 7200 7400 6900 6500 7200 6500 6e00 2e00  r.t.i.e.r.e.n...
+00003b60: 2e00 2e08 0000 0000 0600 0000 0945 7870  .............Exp
+00003b70: 6f72 742e 2e2e 0700 0000 0a4d 6169 6e57  ort........MainW
+00003b80: 696e 646f 7701 0300 0000 0a00 4400 6100  indow.......D.a.
+00003b90: 7400 6500 6908 0000 0000 0600 0000 0446  t.e.i..........F
+00003ba0: 696c 6507 0000 000a 4d61 696e 5769 6e64  ile.....MainWind
+00003bb0: 6f77 0103 0000 000a 0048 0069 006c 0066  ow.......H.i.l.f
+00003bc0: 0065 0800 0000 0006 0000 0004 4865 6c70  .e..........Help
+00003bd0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003be0: 03ff ffff ff08 0000 0000 0600 0000 0649  ...............I
+00003bf0: 6d70 6f72 7407 0000 000a 4d61 696e 5769  mport.....MainWi
+00003c00: 6e64 6f77 0103 0000 001c 0049 006d 0070  ndow.......I.m.p
+00003c10: 006f 0072 0074 0069 0065 0072 0065 006e  .o.r.t.i.e.r.e.n
+00003c20: 002e 002e 002e 0800 0000 0006 0000 0009  ................
+00003c30: 496d 706f 7274 2e2e 2e07 0000 000a 4d61  Import........Ma
+00003c40: 696e 5769 6e64 6f77 0103 0000 0018 004c  inWindow.......L
+00003c50: 006f 0067 0067 0065 0020 0051 0053 004f  .o.g.g.e. .Q.S.O
+00003c60: 002e 002e 002e 0800 0000 0006 0000 000a  ................
+00003c70: 4c6f 6720 5153 4f2e 2e2e 0700 0000 0a4d  Log QSO........M
+00003c80: 6169 6e57 696e 646f 7701 0300 0000 1800  ainWindow.......
+00003c90: 5100 5300 4f00 2d00 4600 6f00 7200 6d00  Q.S.O.-.F.o.r.m.
+00003ca0: 7500 6c00 6100 7208 0000 0000 0600 0000  u.l.a.r.........
+00003cb0: 0851 534f 2046 6f72 6d07 0000 000a 4d61  .QSO Form.....Ma
+00003cc0: 696e 5769 6e64 6f77 0103 0000 0026 0044  inWindow.....&.D
+00003cd0: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
+00003ce0: 0020 0077 00e4 0068 006c 0065 006e 002e  . .w...h.l.e.n..
+00003cf0: 002e 002e 0800 0000 0006 0000 0012 5365  ..............Se
+00003d00: 6c65 6374 2064 6174 6162 6173 652e 2e2e  lect database...
+00003d10: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003d20: 0300 0000 1a00 4500 6900 6e00 7300 7400  ......E.i.n.s.t.
+00003d30: 6500 6c00 6c00 7500 6e00 6700 6500 6e08  e.l.l.u.n.g.e.n.
+00003d40: 0000 0000 0600 0000 0853 6574 7469 6e67  .........Setting
+00003d50: 7307 0000 000a 4d61 696e 5769 6e64 6f77  s.....MainWindow
+00003d60: 0103 0000 0026 005a 0065 0069 0067 0065  .....&.Z.e.i.g.e
+00003d70: 0020 0041 006e 0077 0065 006e 0064 0075  . .A.n.w.e.n.d.u
+00003d80: 006e 0067 0073 006c 006f 0067 0800 0000  .n.g.s.l.o.g....
+00003d90: 0006 0000 0008 5368 6f77 206c 6f67 0700  ......Show log..
+00003da0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
+00003db0: 0000 1a00 5300 7400 6100 7200 7400 6500  ....S.t.a.r.t.e.
+00003dc0: 2000 4800 6100 6d00 6c00 6900 6208 0000   .H.a.m.l.i.b...
+00003dd0: 0000 0600 0000 0c53 7461 7274 2068 616d  .......Start ham
+00003de0: 6c69 6207 0000 000a 4d61 696e 5769 6e64  lib.....MainWind
+00003df0: 6f77 0103 0000 001c 0057 0065 0072 006b  ow.......W.e.r.k
+00003e00: 007a 0065 0075 0067 006c 0065 0069 0073  .z.e.u.g.l.e.i.s
+00003e10: 0074 0065 0800 0000 0006 0000 0007 546f  .t.e..........To
+00003e20: 6f6c 6261 7207 0000 000a 4d61 696e 5769  olbar.....MainWi
+00003e30: 6e64 6f77 0103 0000 0032 004c 006f 0067  ndow.....2.L.o.g
+00003e40: 0073 0020 007a 0075 0020 004c 006f 0054  .s. .z.u. .L.o.T
+00003e50: 0057 0020 0068 006f 0063 0068 006c 0061  .W. .h.o.c.h.l.a
+00003e60: 0064 0065 006e 002e 002e 002e 0800 0000  .d.e.n..........
+00003e70: 0006 0000 0016 5570 6c6f 6164 206c 6f67  ......Upload log
+00003e80: 7320 746f 204c 6f54 572e 2e2e 0700 0000  s to LoTW.......
+00003e90: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
+00003ea0: 4200 4400 6100 7400 6500 6900 2000 6100  B.D.a.t.e.i. .a.
+00003eb0: 7500 6600 2000 6e00 6500 7500 6500 2000  u.f. .n.e.u.e. .
+00003ec0: 5100 5300 4f00 7300 2000 fc00 6200 6500  Q.S.O.s. ...b.e.
+00003ed0: 7200 7700 6100 6300 6800 6500 6e00 2e00  r.w.a.c.h.e.n...
+00003ee0: 2e00 2e08 0000 0000 0600 0000 1657 6174  .............Wat
+00003ef0: 6368 2066 696c 6520 666f 7220 5153 4f73  ch file for QSOs
+00003f00: 2e2e 2e07 0000 000a 4d61 696e 5769 6e64  ........MainWind
+00003f10: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00003f20: 0002 2057 0700 0000 0751 534f 466f 726d  .. W.....QSOForm
+00003f30: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+00003f40: 206b 487a 0700 0000 0751 534f 466f 726d   kHz.....QSOForm
+00003f50: 0103 ffff ffff 0800 0000 0006 0000 0002  ................
+00003f60: 3539 0700 0000 0751 534f 466f 726d 0103  59.....QSOForm..
+00003f70: 0000 0048 0045 0069 006e 0020 0046 0065  ...H.E.i.n. .F.e
+00003f80: 006c 0064 0020 0066 0065 0068 006c 0074  .l.d. .f.e.h.l.t
+00003f90: 0020 0066 00fc 0072 0020 0064 0069 0065  . .f...r. .d.i.e
+00003fa0: 0020 0049 006e 0062 006f 0078 002d 0050  . .I.n.b.o.x.-.P
+00003fb0: 0072 00fc 0066 0075 006e 0067 0800 0000  .r...f.u.n.g....
+00003fc0: 0006 0000 0022 4120 6669 656c 6420 6973  ....."A field is
+00003fd0: 206d 6973 7369 6e67 2066 6f72 2069 6e62   missing for inb
+00003fe0: 6f78 2063 6865 636b 0700 0000 0751 534f  ox check.....QSO
+00003ff0: 466f 726d 0103 0000 0042 0046 0065 0068  Form.....B.F.e.h
+00004000: 006c 0065 006e 0064 0065 0073 0020 0046  .l.e.n.d.e.s. .F
+00004010: 0065 006c 0064 0020 0066 00fc 0072 0020  .e.l.d. .f...r. 
+00004020: 0064 0065 006e 0020 004c 006f 0067 002d  .d.e.n. .L.o.g.-
+00004030: 0055 0070 006c 006f 0061 0064 0800 0000  .U.p.l.o.a.d....
+00004040: 0006 0000 0021 4120 6669 656c 6420 6973  .....!A field is
+00004050: 206d 6973 7369 6e67 2066 6f72 206c 6f67   missing for log
+00004060: 2075 706c 6f61 6407 0000 0007 5153 4f46   upload.....QSOF
+00004070: 6f72 6d01 0300 0000 1600 4100 6b00 7a00  orm.......A.k.z.
+00004080: 6500 7000 7400 6900 6500 7200 7400 3a08  e.p.t.i.e.r.t.:.
+00004090: 0000 0000 0600 0000 0841 6363 6570 7473  .........Accepts
+000040a0: 3a07 0000 0007 5153 4f46 6f72 6d01 0300  :.....QSOForm...
+000040b0: 0000 0e00 4100 6e00 7400 6500 6e00 6e00  ....A.n.t.e.n.n.
+000040c0: 6508 0000 0000 0600 0000 0741 6e74 656e  e..........Anten
+000040d0: 6e61 0700 0000 0751 534f 466f 726d 0103  na.....QSOForm..
+000040e0: 0000 0016 0041 0075 0074 006f 006d 0061  .....A.u.t.o.m.a
+000040f0: 0074 0069 0073 0063 0068 0800 0000 0006  .t.i.s.c.h......
+00004100: 0000 000d 4175 746f 6d61 7469 6361 6c6c  ....Automaticall
+00004110: 7907 0000 0007 5153 4f46 6f72 6d01 0300  y.....QSOForm...
+00004120: 0000 3800 4600 6500 6800 6c00 6500 7200  ..8.F.e.h.l.e.r.
+00004130: 6800 6100 6600 7400 6500 7300 2000 4100  h.a.f.t.e.s. .A.
+00004140: 6200 6600 7200 6100 6700 6500 6500 7200  b.f.r.a.g.e.e.r.
+00004150: 6700 6500 6200 6e00 6900 7308 0000 0000  g.e.b.n.i.s.....
+00004160: 0600 0000 1242 6164 2072 6571 7565 7374  .....Bad request
+00004170: 2072 6573 756c 7407 0000 0007 5153 4f46   result.....QSOF
+00004180: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
+00004190: 0000 0442 616e 6407 0000 0007 5153 4f46  ...Band.....QSOF
+000041a0: 6f72 6d01 0300 0000 0800 4200 fc00 7200  orm.......B...r.
+000041b0: 6f08 0000 0000 0600 0000 0642 7572 6561  o..........Burea
+000041c0: 7507 0000 0007 5153 4f46 6f72 6d01 0300  u.....QSOForm...
+000041d0: 0000 1600 4200 fc00 7200 6f00 2f00 4400  ....B...r.o./.D.
+000041e0: 6900 7200 6500 6b00 7408 0000 0000 0600  i.r.e.k.t.......
+000041f0: 0000 0d42 7572 6561 752f 4469 7265 6374  ...Bureau/Direct
+00004200: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004210: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
+00004220: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
+00004230: 4361 6c6c 2073 6967 6e07 0000 0007 5153  Call sign.....QS
+00004240: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00004250: 0600 0000 0843 616c 6c62 6f6f 6b07 0000  .....Callbook...
+00004260: 0007 5153 4f46 6f72 6d01 0300 0000 3c00  ..QSOForm.....<.
+00004270: 4600 6500 6800 6c00 6500 7200 2000 6200  F.e.h.l.e.r. .b.
+00004280: 6500 6900 2000 6400 6500 7200 2000 5200  e.i. .d.e.r. .R.
+00004290: 7500 6600 7a00 6500 6900 6300 6800 6500  u.f.z.e.i.c.h.e.
+000042a0: 6e00 7300 7500 6300 6800 6508 0000 0000  n.s.u.c.h.e.....
+000042b0: 0600 0000 1543 616c 6c62 6f6f 6b20 7365  .....Callbook se
+000042c0: 6172 6368 2065 7272 6f72 0700 0000 0751  arch error.....Q
+000042d0: 534f 466f 726d 0103 0000 002a 0043 0061  SOForm.....*.C.a
+000042e0: 006c 006c 0062 006f 006f 006b 002d 0053  .l.l.b.o.o.k.-.S
+000042f0: 0075 0063 0068 0065 0072 0067 0065 0062  .u.c.h.e.r.g.e.b
+00004300: 006e 0069 0073 0800 0000 0006 0000 0016  .n.i.s..........
+00004310: 4361 6c6c 626f 6f6b 2073 6561 7263 6820  Callbook search 
+00004320: 7265 7375 6c74 0700 0000 0751 534f 466f  result.....QSOFo
+00004330: 726d 0103 0000 0032 0052 0075 0066 007a  rm.....2.R.u.f.z
+00004340: 0065 0069 0063 0068 0065 006e 0020 006e  .e.i.c.h.e.n. .n
+00004350: 0069 0063 0068 0074 0020 0067 0065 0066  .i.c.h.t. .g.e.f
+00004360: 0075 006e 0064 0065 006e 0800 0000 0006  .u.n.d.e.n......
+00004370: 0000 0012 4361 6c6c 7369 676e 206e 6f74  ....Callsign not
+00004380: 2066 6f75 6e64 0700 0000 0751 534f 466f   found.....QSOFo
+00004390: 726d 0103 0000 000a 004b 0061 006e 0061  rm.......K.a.n.a
+000043a0: 006c 0800 0000 0006 0000 0007 4368 616e  .l..........Chan
+000043b0: 6e65 6c07 0000 0007 5153 4f46 6f72 6d01  nel.....QSOForm.
+000043c0: 0300 0000 1600 5000 7200 fc00 6600 6500  ......P.r...f.e.
+000043d0: 2000 4900 6e00 6200 6f00 7808 0000 0000   .I.n.b.o.x.....
+000043e0: 0600 0000 0b43 6865 636b 2049 6e62 6f78  .....Check Inbox
+000043f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004400: 0042 0046 0065 0068 006c 0065 0072 0020  .B.F.e.h.l.e.r. 
+00004410: 0062 0065 0069 006d 0020 0050 0072 00fc  .b.e.i.m. .P.r..
+00004420: 0066 0065 006e 0020 0064 0065 0072 0020  .f.e.n. .d.e.r. 
+00004430: 004c 006f 0054 0057 002d 0049 006e 0062  .L.o.T.W.-.I.n.b
+00004440: 006f 0078 0800 0000 0006 0000 0016 4368  .o.x..........Ch
+00004450: 6563 6b20 4c6f 5457 2049 6e62 6f78 2065  eck LoTW Inbox e
+00004460: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
+00004470: 0103 0000 001c 0050 0072 00fc 0066 0065  .......P.r...f.e
+00004480: 0020 004c 006f 0054 0057 0020 0051 0053  . .L.o.T.W. .Q.S
+00004490: 004c 0800 0000 0006 0000 000e 4368 6563  .L..........Chec
+000044a0: 6b20 4c6f 5457 2051 534c 0700 0000 0751  k LoTW QSL.....Q
+000044b0: 534f 466f 726d 0103 0000 0038 0065 0051  SOForm.....8.e.Q
+000044c0: 0053 004c 002d 0046 0065 0068 006c 0065  .S.L.-.F.e.h.l.e
+000044d0: 0072 0020 0070 0072 00fc 0066 0065 006e  .r. .p.r...f.e.n
+000044e0: 0020 0064 0065 0072 0020 0049 006e 0062  . .d.e.r. .I.n.b
+000044f0: 006f 0078 0800 0000 0006 0000 0016 4368  .o.x..........Ch
+00004500: 6563 6b20 6551 534c 2049 6e62 6f78 2065  eck eQSL Inbox e
+00004510: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
+00004520: 0103 0000 0018 005a 0075 0072 00fc 0063  .......Z.u.r...c
+00004530: 006b 0073 0065 0074 007a 0065 006e 0800  .k.s.e.t.z.e.n..
+00004540: 0000 0006 0000 0005 436c 6561 7207 0000  ........Clear...
+00004550: 0007 5153 4f46 6f72 6d01 0300 0000 2000  ..QSOForm..... .
+00004560: 4b00 6f00 6e00 6600 6900 6700 7500 7200  K.o.n.f.i.g.u.r.
+00004570: 6900 6500 7200 7400 6500 2000 4900 4408  i.e.r.t.e. .I.D.
+00004580: 0000 0000 0600 0000 1343 6f6e 6669 6775  .........Configu
+00004590: 7265 6420 6964 656e 7469 7479 0700 0000  red identity....
+000045a0: 0751 534f 466f 726d 0103 0000 002a 004b  .QSOForm.....*.K
+000045b0: 006f 006e 0066 0069 0067 0075 0072 0069  .o.n.f.i.g.u.r.i
+000045c0: 0065 0072 0074 0065 0020 0053 0074 0061  .e.r.t.e. .S.t.a
+000045d0: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
+000045e0: 0012 436f 6e66 6967 7572 6564 2073 7461  ..Configured sta
+000045f0: 7469 6f6e 0700 0000 0751 534f 466f 726d  tion.....QSOForm
+00004600: 0103 0000 000c 0064 0069 0072 0065 006b  .......d.i.r.e.k
+00004610: 0074 0800 0000 0006 0000 0006 4469 7265  .t..........Dire
+00004620: 6374 0700 0000 0751 534f 466f 726d 0103  ct.....QSOForm..
+00004630: 0000 001c 0065 0051 0053 004c 0020 0073  .....e.Q.S.L. .s
+00004640: 0070 0065 0069 0063 0068 0065 0072 006e  .p.e.i.c.h.e.r.n
+00004650: 0800 0000 0006 0000 000d 446f 776e 6c6f  ..........Downlo
+00004660: 6164 2065 5153 4c07 0000 0007 5153 4f46  ad eQSL.....QSOF
+00004670: 6f72 6d01 0300 0000 6c00 5700 e400 6800  orm.....l.W...h.
+00004680: 7200 6500 6e00 6400 2000 6400 6500 7200  r.e.n.d. .d.e.r.
+00004690: 2000 5200 7500 6600 7a00 6500 6900 6300   .R.u.f.z.e.i.c.
+000046a0: 6800 6500 6e00 7300 7500 6300 6800 6500  h.e.n.s.u.c.h.e.
+000046b0: 2000 6900 7300 7400 2000 6500 6900 6e00   .i.s.t. .e.i.n.
+000046c0: 2000 4600 6500 6800 6c00 6500 7200 2000   .F.e.h.l.e.r. .
+000046d0: 6100 7500 6600 6700 6500 7400 7200 6500  a.u.f.g.e.t.r.e.
+000046e0: 7400 6500 6e08 0000 0000 0600 0000 2744  t.e.n.........'D
+000046f0: 7572 696e 6720 6361 6c6c 626f 6f6b 2073  uring callbook s
+00004700: 6561 7263 6820 616e 2065 7272 6f72 206f  earch an error o
+00004710: 6363 7572 6564 0700 0000 0751 534f 466f  ccured.....QSOFo
+00004720: 726d 0103 0000 0008 0045 006e 0064 0065  rm.......E.n.d.e
+00004730: 0800 0000 0006 0000 0003 456e 6407 0000  ..........End...
+00004740: 0007 5153 4f46 6f72 6d01 0300 0000 0c00  ..QSOForm.......
+00004750: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
+00004760: 0600 0000 0545 7272 6f72 0700 0000 0751  .....Error.....Q
+00004770: 534f 466f 726d 0103 0000 0024 0065 0051  SOForm.....$.e.Q
+00004780: 0053 004c 002d 0055 0070 006c 006f 0061  .S.L.-.U.p.l.o.a
+00004790: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
+000047a0: 0800 0000 0006 0000 000f 4572 726f 7220  ..........Error 
+000047b0: 6f6e 2075 706c 6f61 6407 0000 0007 5153  on upload.....QS
+000047c0: 4f46 6f72 6d01 0300 0000 1000 4600 7200  OForm.......F.r.
+000047d0: 6500 7100 7500 6500 6e00 7a08 0000 0000  e.q.u.e.n.z.....
+000047e0: 0600 0000 0946 7265 7175 656e 6379 0700  .....Frequency..
+000047f0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00004800: 0800 0000 0006 0000 0008 4848 3a6d 6d3a  ..........HH:mm:
+00004810: 7373 0700 0000 0751 534f 466f 726d 0103  ss.....QSOForm..
+00004820: ffff ffff 0800 0000 0006 0000 0006 4861  ..............Ha
+00004830: 6d51 5448 0700 0000 0751 534f 466f 726d  mQTH.....QSOForm
+00004840: 0103 0000 0004 0049 0044 0800 0000 0006  .......I.D......
+00004850: 0000 0008 4964 656e 7469 7479 0700 0000  ....Identity....
+00004860: 0751 534f 466f 726d 0103 0000 0026 004c  .QSOForm.....&.L
+00004870: 0069 006e 006b 0020 007a 0075 0072 0020  .i.n.k. .z.u.r. 
+00004880: 0065 0051 0053 004c 002d 004b 0061 0072  .e.Q.S.L.-.K.a.r
+00004890: 0074 0065 0800 0000 0006 0000 0011 4c69  .t.e..........Li
+000048a0: 6e6b 2074 6f20 6551 534c 2043 6172 6407  nk to eQSL Card.
+000048b0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+000048c0: ff08 0000 0000 0600 0000 044c 6f54 5707  ...........LoTW.
+000048d0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000048e0: 1c00 4c00 6f00 5400 5700 2000 6500 6d00  ..L.o.T.W. .e.m.
+000048f0: 7000 6600 6100 6e00 6700 6500 6e08 0000  p.f.a.n.g.e.n...
+00004900: 0000 0600 0000 0d4c 6f54 5720 7265 6365  .......LoTW rece
+00004910: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
+00004920: 0103 0000 001c 004c 006f 0054 0057 0020  .......L.o.T.W. 
+00004930: 0076 0065 0072 0073 0065 006e 0064 0065  .v.e.r.s.e.n.d.e
+00004940: 0074 0800 0000 0006 0000 0009 4c6f 5457  .t..........LoTW
+00004950: 2073 656e 7407 0000 0007 5153 4f46 6f72   sent.....QSOFor
+00004960: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+00004970: 074c 6f63 6174 6f72 0700 0000 0751 534f  .Locator.....QSO
+00004980: 466f 726d 0103 0000 0042 004c 006f 0067  Form.....B.L.o.g
+00004990: 0069 006e 0020 0066 0065 0068 006c 0067  .i.n. .f.e.h.l.g
+000049a0: 0065 0073 0063 0068 006c 0061 0067 0065  .e.s.c.h.l.a.g.e
+000049b0: 006e 0020 0066 00fc 0072 0020 0042 0065  .n. .f...r. .B.e
+000049c0: 006e 0075 0074 007a 0065 0072 0800 0000  .n.u.t.z.e.r....
+000049d0: 0006 0000 0015 4c6f 6769 6e20 6661 696c  ......Login fail
+000049e0: 6564 2066 6f72 2075 7365 7207 0000 0007  ed for user.....
+000049f0: 5153 4f46 6f72 6d01 0300 0000 1400 4800  QSOForm.......H.
+00004a00: 6100 7500 7000 7400 6400 6100 7400 6500  a.u.p.t.d.a.t.e.
+00004a10: 6e08 0000 0000 0600 0000 094d 6169 6e20  n..........Main 
+00004a20: 6461 7461 0700 0000 0751 534f 466f 726d  data.....QSOForm
+00004a30: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+00004a40: 4d6f 6465 0700 0000 0751 534f 466f 726d  Mode.....QSOForm
+00004a50: 0103 0000 0012 0076 0065 0072 00e4 006e  .......v.e.r...n
+00004a60: 0064 0065 0072 0074 0800 0000 0006 0000  .d.e.r.t........
+00004a70: 0008 4d6f 6469 6669 6564 0700 0000 0751  ..Modified.....Q
+00004a80: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00004a90: 0006 0000 0004 4e61 6d65 0700 0000 0751  ......Name.....Q
+00004aa0: 534f 466f 726d 0103 0000 0024 004b 0065  SOForm.....$.K.e
+00004ab0: 0069 006e 0020 0051 0053 004c 0020 0076  .i.n. .Q.S.L. .v
+00004ac0: 0065 0072 0066 00fc 0067 0062 0061 0072  .e.r.f...g.b.a.r
+00004ad0: 0800 0000 0006 0000 0010 4e6f 2051 534c  ..........No QSL
+00004ae0: 2061 7661 696c 6162 6c65 0700 0000 0751   available.....Q
+00004af0: 534f 466f 726d 0103 0000 0026 004b 0065  SOForm.....&.K.e
+00004b00: 0069 006e 0020 0065 0051 0053 004c 0020  .i.n. .e.Q.S.L. 
+00004b10: 0076 0065 0072 0066 00fc 0067 0062 0061  .v.e.r.f...g.b.a
+00004b20: 0072 0800 0000 0006 0000 0011 4e6f 2065  .r..........No e
+00004b30: 5153 4c20 6176 6169 6c61 626c 6507 0000  QSL available...
+00004b40: 0007 5153 4f46 6f72 6d01 0300 0000 0a00  ..QSOForm.......
+00004b50: 4a00 6500 7400 7a00 7408 0000 0000 0600  J.e.t.z.t.......
+00004b60: 0000 034e 6f77 0700 0000 0751 534f 466f  ...Now.....QSOFo
+00004b70: 726d 0103 0000 0016 0045 0069 0067 0065  rm.......E.i.g.e
+00004b80: 006e 0065 0072 0020 0051 0054 0048 0800  .n.e.r. .Q.T.H..
+00004b90: 0000 0006 0000 0007 4f77 6e20 5154 4807  ........Own QTH.
+00004ba0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00004bb0: 2400 4500 6900 6700 6500 6e00 6500 7300  $.E.i.g.e.n.e.s.
+00004bc0: 2000 5200 7500 6600 7a00 6500 6900 6300   .R.u.f.z.e.i.c.
+00004bd0: 6800 6500 6e08 0000 0000 0600 0000 0d4f  h.e.n..........O
+00004be0: 776e 2063 616c 6c20 7369 676e 0700 0000  wn call sign....
+00004bf0: 0751 534f 466f 726d 0103 0000 001e 0045  .QSOForm.......E
+00004c00: 0069 0067 0065 006e 0065 0072 0020 004c  .i.g.e.n.e.r. .L
+00004c10: 006f 0063 0061 0074 006f 0072 0800 0000  .o.c.a.t.o.r....
+00004c20: 0006 0000 000b 4f77 6e20 6c6f 6361 746f  ......Own locato
+00004c30: 7207 0000 0007 5153 4f46 6f72 6d01 0300  r.....QSOForm...
+00004c40: 0000 1800 4500 6900 6700 6500 6e00 6500  ....E.i.g.e.n.e.
+00004c50: 7200 2000 4e00 6100 6d00 6508 0000 0000  r. .N.a.m.e.....
+00004c60: 0600 0000 084f 776e 206e 616d 6507 0000  .....Own name...
+00004c70: 0007 5153 4f46 6f72 6d01 0300 0000 1c00  ..QSOForm.......
+00004c80: 4500 6900 6700 6500 6e00 6500 2000 4e00  E.i.g.e.n.e. .N.
+00004c90: 6f00 7400 6900 7a00 6500 6e08 0000 0000  o.t.i.z.e.n.....
+00004ca0: 0600 0000 094f 776e 206e 6f74 6573 0700  .....Own notes..
+00004cb0: 0000 0751 534f 466f 726d 0103 0000 0010  ...QSOForm......
+00004cc0: 004c 0065 0069 0073 0074 0075 006e 0067  .L.e.i.s.t.u.n.g
+00004cd0: 0800 0000 0006 0000 0005 506f 7765 7207  ..........Power.
+00004ce0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00004cf0: 1e00 4100 7500 7300 6200 7200 6500 6900  ..A.u.s.b.r.e.i.
+00004d00: 7400 7500 6e00 6700 7300 6100 7200 7408  t.u.n.g.s.a.r.t.
+00004d10: 0000 0000 0600 0000 0b50 726f 7061 6761  .........Propaga
+00004d20: 7469 6f6e 0700 0000 0751 534f 466f 726d  tion.....QSOForm
 00004d30: 0103 ffff ffff 0800 0000 0006 0000 0003  ................
-00004d40: 5154 4807 0000 000d 5153 4f46 6f72 6d44  QTH.....QSOFormD
-00004d50: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-00004d60: 0600 0000 0652 5354 2052 7807 0000 000d  .....RST Rx.....
-00004d70: 5153 4f46 6f72 6d44 6961 6c6f 6701 03ff  QSOFormDialog...
-00004d80: ffff ff08 0000 0000 0600 0000 0652 5354  .............RST
-00004d90: 2054 7807 0000 000d 5153 4f46 6f72 6d44   Tx.....QSOFormD
-00004da0: 6961 6c6f 6701 0300 0000 1a00 5200 5300  ialog.......R.S.
-00004db0: 5400 2000 6500 6d00 7000 6600 6100 6e00  T. .e.m.p.f.a.n.
-00004dc0: 6700 6500 6e08 0000 0000 0600 0000 0c52  g.e.n..........R
-00004dd0: 5354 2072 6563 6569 7665 6407 0000 000d  ST received.....
-00004de0: 5153 4f46 6f72 6d44 6961 6c6f 6701 0300  QSOFormDialog...
-00004df0: 0000 1800 5200 5300 5400 2000 6700 6500  ....R.S.T. .g.e.
-00004e00: 7300 6500 6e00 6400 6500 7408 0000 0000  s.e.n.d.e.t.....
-00004e10: 0600 0000 0852 5354 2073 656e 7407 0000  .....RST sent...
-00004e20: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-00004e30: 03ff ffff ff08 0000 0000 0600 0000 0552  ...............R
-00004e40: 6164 696f 0700 0000 0d51 534f 466f 726d  adio.....QSOForm
-00004e50: 4469 616c 6f67 0103 0000 0012 0053 0070  Dialog.......S.p
-00004e60: 0065 0069 0063 0068 0065 0072 006e 0800  .e.i.c.h.e.r.n..
-00004e70: 0000 0006 0000 0004 5361 7665 0700 0000  ........Save....
-00004e80: 0d51 534f 466f 726d 4469 616c 6f67 0103  .QSOFormDialog..
-00004e90: 0000 0026 0053 0070 0065 0069 0063 0068  ...&.S.p.e.i.c.h
-00004ea0: 0065 0072 006e 0020 0026 0026 0020 0055  .e.r.n. .&.&. .U
-00004eb0: 0070 006c 006f 0061 0064 0800 0000 0006  .p.l.o.a.d......
-00004ec0: 0000 000e 5361 7665 2026 2620 5570 6c6f  ....Save && Uplo
-00004ed0: 6164 0700 0000 0d51 534f 466f 726d 4469  ad.....QSOFormDi
-00004ee0: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
-00004ef0: 0000 0005 5374 6172 7407 0000 000d 5153  ....Start.....QS
-00004f00: 4f46 6f72 6d44 6961 6c6f 6701 0300 0000  OFormDialog.....
-00004f10: b800 4400 6900 6500 2000 5100 5300 4c00  ..D.i.e. .Q.S.L.
-00004f20: 2d00 5200 6f00 7500 7400 6500 2000 6400  -.R.o.u.t.e. .d.
-00004f30: 6500 7200 2000 6b00 6f00 6e00 7400 6100  e.r. .k.o.n.t.a.
-00004f40: 6b00 7400 6900 6500 7200 7400 6500 6e00  k.t.i.e.r.t.e.n.
-00004f50: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
-00004f60: 2e00 0a00 4400 6900 6500 7300 2000 6900  ....D.i.e.s. .i.
-00004f70: 7300 7400 2000 6e00 6900 6300 6800 7400  s.t. .n.i.c.h.t.
-00004f80: 2000 6400 6900 6500 2000 4100 6400 7200   .d.i.e. .A.d.r.
-00004f90: 6500 7300 7300 6500 2000 6400 6500 7300  e.s.s.e. .d.e.s.
-00004fa0: 2000 5100 5300 4c00 2d00 4d00 6100 6e00   .Q.S.L.-.M.a.n.
-00004fb0: 6100 6700 6500 7200 7300 2f00 2d00 4200  a.g.e.r.s./.-.B.
-00004fc0: fc00 7200 6f00 7300 2e08 0000 0000 0600  ..r.o.s.........
-00004fd0: 0000 4c54 6865 2063 6f6e 7461 6374 6564  ..LThe contacted
-00004fe0: 2073 7461 7469 6f6e 2051 534c 2072 6f75   station QSL rou
-00004ff0: 7465 2e0a 5468 6973 2069 7320 6e6f 7420  te..This is not 
-00005000: 7468 6520 5153 4c20 6d61 6e61 6765 722f  the QSL manager/
-00005010: 6275 7265 6175 2061 6464 7265 7373 2e07  bureau address..
-00005020: 0000 000d 5153 4f46 6f72 6d44 6961 6c6f  ....QSOFormDialo
-00005030: 6701 0300 0000 1600 6800 6f00 6300 6800  g.......h.o.c.h.
-00005040: 6700 6500 6c00 6100 6400 6500 6e08 0000  g.e.l.a.d.e.n...
-00005050: 0000 0600 0000 0855 706c 6f61 6465 6407  .......Uploaded.
-00005060: 0000 000d 5153 4f46 6f72 6d44 6961 6c6f  ....QSOFormDialo
-00005070: 6701 0300 0000 6800 5500 7000 6c00 6f00  g.....h.U.p.l.o.
-00005080: 6100 6400 2000 6500 7200 6600 6f00 6c00  a.d. .e.r.f.o.l.
-00005090: 6700 7400 2000 6e00 7500 7200 2000 7700  g.t. .n.u.r. .w.
-000050a0: 6500 6e00 6e00 2000 6100 7500 6600 2000  e.n.n. .a.u.f. .
-000050b0: 6400 6500 7200 2000 5100 5300 4c00 2d00  d.e.r. .Q.S.L.-.
-000050c0: 5300 6500 6900 7400 6500 2000 6100 7500  S.e.i.t.e. .a.u.
-000050d0: 7300 6700 6500 7700 e400 6800 6c00 7408  s.g.e.w...h.l.t.
-000050e0: 0000 0000 0600 0000 2455 706c 6f61 6473  ........$Uploads
-000050f0: 206f 6e6c 7920 6966 2073 656c 6563 7465   only if selecte
-00005100: 6420 6f6e 2051 534c 2070 6167 6507 0000  d on QSL page...
-00005110: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-00005120: 03ff ffff ff08 0000 0000 0600 0000 0465  ...............e
-00005130: 5153 4c07 0000 000d 5153 4f46 6f72 6d44  QSL.....QSOFormD
-00005140: 6961 6c6f 6701 0300 0000 1c00 6500 5100  ialog.......e.Q.
-00005150: 5300 4c00 2000 6500 6d00 7000 6600 6100  S.L. .e.m.p.f.a.
-00005160: 6e00 6700 6500 6e08 0000 0000 0600 0000  n.g.e.n.........
-00005170: 0d65 5153 4c20 7265 6365 6976 6564 0700  .eQSL received..
-00005180: 0000 0d51 534f 466f 726d 4469 616c 6f67  ...QSOFormDialog
-00005190: 0103 0000 001a 0065 0051 0053 004c 0020  .......e.Q.S.L. 
-000051a0: 0067 0065 0073 0065 006e 0064 0065 0074  .g.e.s.e.n.d.e.t
-000051b0: 0800 0000 0006 0000 0009 6551 534c 2073  ..........eQSL s
-000051c0: 656e 7407 0000 000d 5153 4f46 6f72 6d44  ent.....QSOFormD
-000051d0: 6961 6c6f 6701 0300 0000 0800 6b00 2e00  ialog.......k...
-000051e0: 4100 2e08 0000 0000 0600 0000 046e 2e61  A............n.a
-000051f0: 2e07 0000 000d 5153 4f46 6f72 6d44 6961  ......QSOFormDia
-00005200: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00005210: 0000 0a79 7979 792d 4d4d 2d64 6407 0000  ...yyyy-MM-dd...
-00005220: 000d 5153 4f46 6f72 6d44 6961 6c6f 6701  ..QSOFormDialog.
-00005230: 0300 0000 2a00 4800 6100 6d00 6c00 6900  ....*.H.a.m.l.i.
-00005240: 6200 2000 7200 6900 6700 6300 7400 6c00  b. .r.i.g.c.t.l.
-00005250: 6400 2000 7700 e400 6800 6c00 6500 6e08  d. .w...h.l.e.n.
-00005260: 0000 0000 0600 0000 2043 686f 6f73 6520  ........ Choose 
-00005270: 6861 6d6c 6962 2072 6967 6374 6c64 2065  hamlib rigctld e
-00005280: 7865 6375 7461 626c 6507 0000 0008 5365  xecutable.....Se
-00005290: 7474 696e 6773 0103 0000 0020 0044 0061  ttings..... .D.a
-000052a0: 0074 0075 006d 002f 005a 0065 0069 0074  .t.u.m./.Z.e.i.t
-000052b0: 0020 0053 0074 0061 0072 0074 0800 0000  . .S.t.a.r.t....
-000052c0: 0006 0000 000f 4461 7465 2f54 696d 6520  ......Date/Time 
-000052d0: 7374 6172 7407 0000 0008 5365 7474 696e  start.....Settin
-000052e0: 6773 0103 0000 0042 0046 0065 0068 006c  gs.....B.F.e.h.l
-000052f0: 0065 0072 0020 0062 0065 0069 006d 0020  .e.r. .b.e.i.m. 
-00005300: 0041 0075 0073 0066 00fc 0068 0072 0065  .A.u.s.f...h.r.e
-00005310: 006e 0020 0076 006f 006e 0020 0072 0069  .n. .v.o.n. .r.i
-00005320: 0067 0063 0074 006c 0064 0800 0000 0006  .g.c.t.l.d......
-00005330: 0000 0017 4572 726f 7220 6578 6563 7574  ....Error execut
-00005340: 696e 6720 7269 6763 746c 6407 0000 0008  ing rigctld.....
-00005350: 5365 7474 696e 6773 0103 ffff ffff 0800  Settings........
-00005360: 0000 0006 0000 0006 4861 6d6c 6962 0700  ........Hamlib..
-00005370: 0000 0853 6574 7469 6e67 7301 0300 0000  ...Settings.....
-00005380: 4e00 4400 6900 6500 2000 6700 6500 7700  N.D.i.e. .g.e.w.
-00005390: e400 6800 6c00 7400 6500 2000 4400 6100  ..h.l.t.e. .D.a.
-000053a0: 7400 6500 6900 2000 6900 7300 7400 2000  t.e.i. .i.s.t. .
-000053b0: 6e00 6900 6300 6800 7400 2000 6100 7500  n.i.c.h.t. .a.u.
-000053c0: 7300 6600 fc00 6800 7200 6200 6100 7208  s.f...h.r.b.a.r.
-000053d0: 0000 0000 0600 0000 2353 656c 6563 7465  ........#Selecte
-000053e0: 6420 6669 6c65 2069 7320 6e6f 7420 7468  d file is not th
-000053f0: 6520 6578 6563 7574 6162 6c65 0700 0000  e executable....
-00005400: 0853 6574 7469 6e67 7301 0300 0000 1400  .Settings.......
-00005410: 7a00 6500 6900 6700 6500 2000 6100 6c00  z.e.i.g.e. .a.l.
-00005420: 6c00 6508 0000 0000 0600 0000 0853 686f  l.e..........Sho
-00005430: 7720 616c 6c07 0000 0008 5365 7474 696e  w all.....Settin
-00005440: 6773 0103 ffff ffff 0800 0000 0006 0000  gs..............
-00005450: 0005 5374 6172 7407 0000 0008 5365 7474  ..Start.....Sett
-00005460: 696e 6773 0103 0000 001a 0053 0074 0061  ings.......S.t.a
-00005470: 0072 0074 0065 0020 0048 0061 006d 006c  .r.t.e. .H.a.m.l
-00005480: 0069 0062 0800 0000 0006 0000 000c 5374  .i.b..........St
-00005490: 6172 7420 6861 6d6c 6962 0700 0000 0853  art hamlib.....S
-000054a0: 6574 7469 6e67 7301 03ff ffff ff08 0000  ettings.........
-000054b0: 0000 0600 0000 0453 746f 7007 0000 0008  .......Stop.....
-000054c0: 5365 7474 696e 6773 0103 0000 001a 0053  Settings.......S
-000054d0: 0074 006f 0070 0070 0065 0020 0048 0061  .t.o.p.p.e. .H.a
-000054e0: 006d 006c 0069 0062 0800 0000 0006 0000  .m.l.i.b........
-000054f0: 000b 5374 6f70 2068 616d 6c69 6207 0000  ..Stop hamlib...
-00005500: 0008 5365 7474 696e 6773 0103 0000 000a  ..Settings......
-00005510: 0061 006b 0074 0069 0076 0800 0000 0006  .a.k.t.i.v......
-00005520: 0000 0005 6163 7469 7607 0000 0008 5365  ....activ.....Se
-00005530: 7474 696e 6773 0103 0000 000e 0069 006e  ttings.......i.n
-00005540: 0061 006b 0074 0069 0076 0800 0000 0006  .a.k.t.i.v......
-00005550: 0000 0007 696e 6163 7469 7607 0000 0008  ....inactiv.....
-00005560: 5365 7474 696e 6773 0103 0000 004a 0072  Settings.....J.r
-00005570: 0069 0067 0063 0074 006c 0064 0020 006b  .i.g.c.t.l.d. .k
-00005580: 006f 006e 006e 0074 0065 0020 006e 0069  .o.n.n.t.e. .n.i
-00005590: 0063 0068 0074 0020 0067 0065 0073 0074  .c.h.t. .g.e.s.t
-000055a0: 0061 0072 0074 0065 0074 0020 0077 0065  .a.r.t.e.t. .w.e
-000055b0: 0072 0064 0065 006e 0800 0000 0006 0000  .r.d.e.n........
-000055c0: 001e 7269 6763 746c 6420 6469 6420 6e6f  ..rigctld did no
-000055d0: 7420 7374 6172 7420 7072 6f70 6572 6c79  t start properly
-000055e0: 0700 0000 0853 6574 7469 6e67 7301 03ff  .....Settings...
-000055f0: ffff ff08 0000 0000 0600 0000 074a 5338  .............JS8
-00005600: 4361 6c6c 0700 0000 0f61 7070 5365 6c65  Call.....appSele
-00005610: 6374 4469 616c 6f67 0103 ffff ffff 0800  ctDialog........
-00005620: 0000 0006 0000 0005 4f74 6865 7207 0000  ........Other...
-00005630: 000f 6170 7053 656c 6563 7444 6961 6c6f  ..appSelectDialo
-00005640: 6701 0300 0000 2a00 4100 7500 7300 7700  g.....*.A.u.s.w.
-00005650: 6100 6800 6c00 2000 6400 6500 7300 2000  a.h.l. .d.e.s. .
-00005660: 5000 7200 6f00 6700 7200 6100 6d00 6d00  P.r.o.g.r.a.m.m.
-00005670: 7308 0000 0000 0600 0000 1653 656c 6563  s..........Selec
-00005680: 7420 7468 6520 6170 706c 6963 6174 696f  t the applicatio
-00005690: 6e07 0000 000f 6170 7053 656c 6563 7444  n.....appSelectD
-000056a0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-000056b0: 0600 0000 0657 534a 542d 5807 0000 000f  .....WSJT-X.....
-000056c0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
-000056d0: 03ff ffff ff08 0000 0000 0600 0000 0666  ...............f
-000056e0: 6c64 6967 6907 0000 000f 6170 7053 656c  ldigi.....appSel
-000056f0: 6563 7444 6961 6c6f 6701 8800 0000 0201  ectDialog.......
-00005700: 01                                       .
+00004d40: 5153 4c07 0000 0007 5153 4f46 6f72 6d01  QSL.....QSOForm.
+00004d50: 0300 0000 2200 5100 5300 4c00 2000 2600  ....".Q.S.L. .&.
+00004d60: 2600 2000 4c00 6f00 6700 2d00 5500 7000  &. .L.o.g.-.U.p.
+00004d70: 6c00 6f00 6100 6408 0000 0000 0600 0000  l.o.a.d.........
+00004d80: 1151 534c 2026 2620 4c6f 6720 7570 6c6f  .QSL && Log uplo
+00004d90: 6164 0700 0000 0751 534f 466f 726d 0103  ad.....QSOForm..
+00004da0: 0000 001c 0051 0053 004c 002d 004b 0061  .....Q.S.L.-.K.a
+00004db0: 0072 0074 0065 006e 0074 0065 0078 0074  .r.t.e.n.t.e.x.t
+00004dc0: 0800 0000 0006 0000 0010 5153 4c20 6361  ..........QSL ca
+00004dd0: 7264 206d 6573 7361 6765 0700 0000 0751  rd message.....Q
+00004de0: 534f 466f 726d 0103 0000 001a 0051 0053  SOForm.......Q.S
+00004df0: 004c 0020 0065 006d 0070 0066 0061 006e  .L. .e.m.p.f.a.n
+00004e00: 0067 0065 006e 0800 0000 0006 0000 000c  .g.e.n..........
+00004e10: 5153 4c20 7265 6365 6976 6564 0700 0000  QSL received....
+00004e20: 0751 534f 466f 726d 0103 0000 0018 0051  .QSOForm.......Q
+00004e30: 0053 004c 0020 0067 0065 0073 0065 006e  .S.L. .g.e.s.e.n
+00004e40: 0064 0065 0074 0800 0000 0006 0000 0008  .d.e.t..........
+00004e50: 5153 4c20 7365 6e74 0700 0000 0751 534f  QSL sent.....QSO
+00004e60: 466f 726d 0103 0000 000e 0051 0053 004c  Form.......Q.S.L
+00004e70: 002d 0056 0069 0061 0800 0000 0006 0000  .-.V.i.a........
+00004e80: 0007 5153 4c20 7669 6107 0000 0007 5153  ..QSL via.....QS
+00004e90: 4f46 6f72 6d01 0300 0000 1800 5100 5300  OForm.......Q.S.
+00004ea0: 4f00 2d00 4600 6f00 7200 6d00 7500 6c00  O.-.F.o.r.m.u.l.
+00004eb0: 6100 7208 0000 0000 0600 0000 0851 534f  a.r..........QSO
+00004ec0: 2046 6f72 6d07 0000 0007 5153 4f46 6f72   Form.....QSOFor
+00004ed0: 6d01 0300 0000 1c00 5100 5300 4f00 2d00  m.......Q.S.O.-.
+00004ee0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00004ef0: 7200 6508 0000 0000 0600 0000 0c51 534f  r.e..........QSO
+00004f00: 2063 6f6d 6d65 6e74 7307 0000 0007 5153   comments.....QS
+00004f10: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00004f20: 0600 0000 0351 5448 0700 0000 0751 534f  .....QTH.....QSO
+00004f30: 466f 726d 0103 ffff ffff 0800 0000 0006  Form............
+00004f40: 0000 0006 5253 5420 5278 0700 0000 0751  ....RST Rx.....Q
+00004f50: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00004f60: 0006 0000 0006 5253 5420 5478 0700 0000  ......RST Tx....
+00004f70: 0751 534f 466f 726d 0103 0000 001a 0052  .QSOForm.......R
+00004f80: 0053 0054 0020 0065 006d 0070 0066 0061  .S.T. .e.m.p.f.a
+00004f90: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
+00004fa0: 000c 5253 5420 7265 6365 6976 6564 0700  ..RST received..
+00004fb0: 0000 0751 534f 466f 726d 0103 0000 0018  ...QSOForm......
+00004fc0: 0052 0053 0054 0020 0067 0065 0073 0065  .R.S.T. .g.e.s.e
+00004fd0: 006e 0064 0065 0074 0800 0000 0006 0000  .n.d.e.t........
+00004fe0: 0008 5253 5420 7365 6e74 0700 0000 0751  ..RST sent.....Q
+00004ff0: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00005000: 0006 0000 0005 5261 6469 6f07 0000 0007  ......Radio.....
+00005010: 5153 4f46 6f72 6d01 0300 0000 1200 5300  QSOForm.......S.
+00005020: 7000 6500 6900 6300 6800 6500 7200 6e08  p.e.i.c.h.e.r.n.
+00005030: 0000 0000 0600 0000 0453 6176 6507 0000  .........Save...
+00005040: 0007 5153 4f46 6f72 6d01 0300 0000 2600  ..QSOForm.....&.
+00005050: 5300 7000 6500 6900 6300 6800 6500 7200  S.p.e.i.c.h.e.r.
+00005060: 6e00 2000 2600 2600 2000 5500 7000 6c00  n. .&.&. .U.p.l.
+00005070: 6f00 6100 6408 0000 0000 0600 0000 0e53  o.a.d..........S
+00005080: 6176 6520 2626 2055 706c 6f61 6407 0000  ave && Upload...
+00005090: 0007 5153 4f46 6f72 6d01 0300 0000 2a00  ..QSOForm.....*.
+000050a0: 6500 5100 5300 4c00 2d00 4f00 7200 6400  e.Q.S.L.-.O.r.d.
+000050b0: 6e00 6500 7200 2000 6100 7500 7300 7700  n.e.r. .a.u.s.w.
+000050c0: e400 6800 6c00 6500 6e08 0000 0000 0600  ..h.l.e.n.......
+000050d0: 0000 1253 656c 6563 7420 6551 534c 2066  ...Select eQSL f
+000050e0: 6f6c 6465 7207 0000 0007 5153 4f46 6f72  older.....QSOFor
+000050f0: 6d01 0300 0000 3600 5300 6500 7200 7600  m.....6.S.e.r.v.
+00005100: 6500 7200 6b00 6f00 6d00 6d00 7500 6e00  e.r.k.o.m.m.u.n.
+00005110: 6900 6b00 6100 7400 6900 6f00 6e00 7300  i.k.a.t.i.o.n.s.
+00005120: 2d00 4600 6500 6800 6c00 6500 7208 0000  -.F.e.h.l.e.r...
+00005130: 0000 0600 0000 1a53 6572 7665 7220 636f  .......Server co
+00005140: 6d6d 756e 6963 6174 696f 6e20 6572 726f  mmunication erro
+00005150: 7207 0000 0007 5153 4f46 6f72 6d01 03ff  r.....QSOForm...
+00005160: ffff ff08 0000 0000 0600 0000 0553 7461  .............Sta
+00005170: 7274 0700 0000 0751 534f 466f 726d 0103  rt.....QSOForm..
+00005180: ffff ffff 0800 0000 0006 0000 0007 5374  ..............St
+00005190: 6174 696f 6e07 0000 0007 5153 4f46 6f72  ation.....QSOFor
+000051a0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+000051b0: 0753 7562 6d6f 6465 0700 0000 0751 534f  .Submode.....QSO
+000051c0: 466f 726d 0103 0000 0030 0044 0061 0073  Form.....0.D.a.s
+000051d0: 0020 0051 0053 004f 0020 0069 0073 0074  . .Q.S.O. .i.s.t
+000051e0: 0020 0065 0069 006e 0020 0044 0075 0070  . .e.i.n. .D.u.p
+000051f0: 006c 0069 006b 0061 0074 0800 0000 0006  .l.i.k.a.t......
+00005200: 0000 0016 5468 6520 5153 4f20 6973 2061  ....The QSO is a
+00005210: 2064 7570 6c69 6361 7465 0700 0000 0751   duplicate.....Q
+00005220: 534f 466f 726d 0103 0000 00b8 0044 0069  SOForm.......D.i
+00005230: 0065 0020 0051 0053 004c 002d 0052 006f  .e. .Q.S.L.-.R.o
+00005240: 0075 0074 0065 0020 0064 0065 0072 0020  .u.t.e. .d.e.r. 
+00005250: 006b 006f 006e 0074 0061 006b 0074 0069  .k.o.n.t.a.k.t.i
+00005260: 0065 0072 0074 0065 006e 0020 0053 0074  .e.r.t.e.n. .S.t
+00005270: 0061 0074 0069 006f 006e 002e 000a 0044  .a.t.i.o.n.....D
+00005280: 0069 0065 0073 0020 0069 0073 0074 0020  .i.e.s. .i.s.t. 
+00005290: 006e 0069 0063 0068 0074 0020 0064 0069  .n.i.c.h.t. .d.i
+000052a0: 0065 0020 0041 0064 0072 0065 0073 0073  .e. .A.d.r.e.s.s
+000052b0: 0065 0020 0064 0065 0073 0020 0051 0053  .e. .d.e.s. .Q.S
+000052c0: 004c 002d 004d 0061 006e 0061 0067 0065  .L.-.M.a.n.a.g.e
+000052d0: 0072 0073 002f 002d 0042 00fc 0072 006f  .r.s./.-.B...r.o
+000052e0: 0073 002e 0800 0000 0006 0000 004c 5468  .s...........LTh
+000052f0: 6520 636f 6e74 6163 7465 6420 7374 6174  e contacted stat
+00005300: 696f 6e20 5153 4c20 726f 7574 652e 0a54  ion QSL route..T
+00005310: 6869 7320 6973 206e 6f74 2074 6865 2051  his is not the Q
+00005320: 534c 206d 616e 6167 6572 2f62 7572 6561  SL manager/burea
+00005330: 7520 6164 6472 6573 732e 0700 0000 0751  u address......Q
+00005340: 534f 466f 726d 0103 0000 0024 0065 0051  SOForm.....$.e.Q
+00005350: 0053 004c 002d 0055 0070 006c 006f 0061  .S.L.-.U.p.l.o.a
+00005360: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
+00005370: 0800 0000 0006 0000 0011 5570 6c6f 6164  ..........Upload
+00005380: 2065 5153 4c20 6572 726f 7207 0000 0007   eQSL error.....
+00005390: 5153 4f46 6f72 6d01 0300 0000 1a00 5500  QSOForm.......U.
+000053a0: 7000 6c00 6f00 6100 6400 2d00 4600 6500  p.l.o.a.d.-.F.e.
+000053b0: 6800 6c00 6500 7208 0000 0000 0600 0000  h.l.e.r.........
+000053c0: 1055 706c 6f61 6420 6c6f 6720 6572 726f  .Upload log erro
+000053d0: 7207 0000 0007 5153 4f46 6f72 6d01 0300  r.....QSOForm...
+000053e0: 0000 1600 6800 6f00 6300 6800 6700 6500  ....h.o.c.h.g.e.
+000053f0: 6c00 6100 6400 6500 6e08 0000 0000 0600  l.a.d.e.n.......
+00005400: 0000 0855 706c 6f61 6465 6407 0000 0007  ...Uploaded.....
+00005410: 5153 4f46 6f72 6d01 0300 0000 6800 5500  QSOForm.....h.U.
+00005420: 7000 6c00 6f00 6100 6400 2000 6500 7200  p.l.o.a.d. .e.r.
+00005430: 6600 6f00 6c00 6700 7400 2000 6e00 7500  f.o.l.g.t. .n.u.
+00005440: 7200 2000 7700 6500 6e00 6e00 2000 6100  r. .w.e.n.n. .a.
+00005450: 7500 6600 2000 6400 6500 7200 2000 5100  u.f. .d.e.r. .Q.
+00005460: 5300 4c00 2d00 5300 6500 6900 7400 6500  S.L.-.S.e.i.t.e.
+00005470: 2000 6100 7500 7300 6700 6500 7700 e400   .a.u.s.g.e.w...
+00005480: 6800 6c00 7408 0000 0000 0600 0000 2455  h.l.t.........$U
+00005490: 706c 6f61 6473 206f 6e6c 7920 6966 2073  ploads only if s
+000054a0: 656c 6563 7465 6420 6f6e 2051 534c 2070  elected on QSL p
+000054b0: 6167 6507 0000 0007 5153 4f46 6f72 6d01  age.....QSOForm.
+000054c0: 0300 0000 4800 4400 6500 7200 2000 4e00  ....H.D.e.r. .N.
+000054d0: 7500 7400 7a00 6500 7200 2000 4300 6100  u.t.z.e.r. .C.a.
+000054e0: 6c00 6c00 2000 7300 7400 6900 6d00 6d00  l.l. .s.t.i.m.m.
+000054f0: 7400 2000 6e00 6900 6300 6800 7400 2000  t. .n.i.c.h.t. .
+00005500: fc00 6200 6500 7200 6500 6900 6e08 0000  ..b.e.r.e.i.n...
+00005510: 0000 0600 0000 1855 7365 7220 6361 6c6c  .......User call
+00005520: 2064 6f65 7320 6e6f 7420 6d61 7463 6807   does not match.
+00005530: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+00005540: ff08 0000 0000 0600 0000 0465 5153 4c07  ...........eQSL.
+00005550: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005560: 1c00 6500 5100 5300 4c00 2000 6500 6d00  ..e.Q.S.L. .e.m.
+00005570: 7000 6600 6100 6e00 6700 6500 6e08 0000  p.f.a.n.g.e.n...
+00005580: 0000 0600 0000 0d65 5153 4c20 7265 6365  .......eQSL rece
+00005590: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
+000055a0: 0103 0000 001a 0065 0051 0053 004c 0020  .......e.Q.S.L. 
+000055b0: 0067 0065 0073 0065 006e 0064 0065 0074  .g.e.s.e.n.d.e.t
+000055c0: 0800 0000 0006 0000 0009 6551 534c 2073  ..........eQSL s
+000055d0: 656e 7407 0000 0007 5153 4f46 6f72 6d01  ent.....QSOForm.
+000055e0: 0300 0000 0800 6b00 2e00 4100 2e08 0000  ......k...A.....
+000055f0: 0000 0600 0000 046e 2e61 2e07 0000 0007  .......n.a......
+00005600: 5153 4f46 6f72 6d01 0300 0000 3400 7200  QSOForm.....4.r.
+00005610: 6900 6700 6300 7400 6c00 6400 2000 5a00  i.g.c.t.l.d. .Z.
+00005620: 6500 6900 7400 fc00 6200 6500 7200 7300  e.i.t...b.e.r.s.
+00005630: 6300 6800 7200 6500 6900 7400 7500 6e00  c.h.r.e.i.t.u.n.
+00005640: 6708 0000 0000 0600 0000 0f72 6967 6374  g..........rigct
+00005650: 6c64 2074 696d 656f 7574 0700 0000 0751  ld timeout.....Q
+00005660: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00005670: 0006 0000 000a 7979 7979 2d4d 4d2d 6464  ......yyyy-MM-dd
+00005680: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005690: 007a 0043 0041 0054 002d 0045 0069 006e  .z.C.A.T.-.E.i.n
+000056a0: 0073 0074 0065 006c 006c 0075 006e 0067  .s.t.e.l.l.u.n.g
+000056b0: 0020 0077 0075 0072 0064 0020 006e 006f  . .w.u.r.d. .n.o
+000056c0: 0063 0068 0020 006e 0069 0065 0020 0067  .c.h. .n.i.e. .g
+000056d0: 0065 0073 0070 0065 0069 0063 0068 0065  .e.s.p.e.i.c.h.e
+000056e0: 0072 0074 0020 006f 0072 0020 0050 0061  .r.t. .o.r. .P.a
+000056f0: 0072 0061 006d 0065 0074 0065 0072 0020  .r.a.m.e.t.e.r. 
+00005700: 0066 0065 0068 006c 0065 006e 0800 0000  .f.e.h.l.e.n....
+00005710: 0006 0000 003b 4341 5420 636f 6e66 6967  .....;CAT config
+00005720: 7572 6174 696f 6e20 7761 7320 6e65 7665  uration was neve
+00005730: 7220 7361 7665 6420 6f72 2061 2070 6172  r saved or a par
+00005740: 616d 6574 6572 2069 7320 6d69 7373 696e  ameter is missin
+00005750: 6707 0000 0008 5365 7474 696e 6773 0103  g.....Settings..
+00005760: 0000 0030 0043 0041 0054 002d 0045 0069  ...0.C.A.T.-.E.i
+00005770: 006e 0073 0074 0065 006c 006c 0075 006e  .n.s.t.e.l.l.u.n
+00005780: 0067 0065 006e 0020 0046 0065 0068 006c  .g.e.n. .F.e.h.l
+00005790: 0065 0072 0800 0000 0006 0000 0012 4341  .e.r..........CA
+000057a0: 5420 7365 7474 696e 6773 2065 7272 6f72  T settings error
+000057b0: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
+000057c0: 0000 2a00 4800 6100 6d00 6c00 6900 6200  ..*.H.a.m.l.i.b.
+000057d0: 2000 7200 6900 6700 6300 7400 6c00 6400   .r.i.g.c.t.l.d.
+000057e0: 2000 7700 e400 6800 6c00 6500 6e08 0000   .w...h.l.e.n...
+000057f0: 0000 0600 0000 2043 686f 6f73 6520 6861  ...... Choose ha
+00005800: 6d6c 6962 2072 6967 6374 6c64 2065 7865  mlib rigctld exe
+00005810: 6375 7461 626c 6507 0000 0008 5365 7474  cutable.....Sett
+00005820: 696e 6773 0103 0000 0020 0044 0061 0074  ings..... .D.a.t
+00005830: 0075 006d 002f 005a 0065 0069 0074 0020  .u.m./.Z.e.i.t. 
+00005840: 0053 0074 0061 0072 0074 0800 0000 0006  .S.t.a.r.t......
+00005850: 0000 000f 4461 7465 2f54 696d 6520 7374  ....Date/Time st
+00005860: 6172 7407 0000 0008 5365 7474 696e 6773  art.....Settings
+00005870: 0103 0000 0042 0046 0065 0068 006c 0065  .....B.F.e.h.l.e
+00005880: 0072 0020 0062 0065 0069 006d 0020 0041  .r. .b.e.i.m. .A
+00005890: 0075 0073 0066 00fc 0068 0072 0065 006e  .u.s.f...h.r.e.n
+000058a0: 0020 0076 006f 006e 0020 0072 0069 0067  . .v.o.n. .r.i.g
+000058b0: 0063 0074 006c 0064 0800 0000 0006 0000  .c.t.l.d........
+000058c0: 0017 4572 726f 7220 6578 6563 7574 696e  ..Error executin
+000058d0: 6720 7269 6763 746c 6407 0000 0008 5365  g rigctld.....Se
+000058e0: 7474 696e 6773 0103 ffff ffff 0800 0000  ttings..........
+000058f0: 0006 0000 0006 4861 6d6c 6962 0700 0000  ......Hamlib....
+00005900: 0853 6574 7469 6e67 7301 0300 0000 4e00  .Settings.....N.
+00005910: 4400 6900 6500 2000 6700 6500 7700 e400  D.i.e. .g.e.w...
+00005920: 6800 6c00 7400 6500 2000 4400 6100 7400  h.l.t.e. .D.a.t.
+00005930: 6500 6900 2000 6900 7300 7400 2000 6e00  e.i. .i.s.t. .n.
+00005940: 6900 6300 6800 7400 2000 6100 7500 7300  i.c.h.t. .a.u.s.
+00005950: 6600 fc00 6800 7200 6200 6100 7208 0000  f...h.r.b.a.r...
+00005960: 0000 0600 0000 2353 656c 6563 7465 6420  ......#Selected 
+00005970: 6669 6c65 2069 7320 6e6f 7420 7468 6520  file is not the 
+00005980: 6578 6563 7574 6162 6c65 0700 0000 0853  executable.....S
+00005990: 6574 7469 6e67 7301 0300 0000 1400 7a00  ettings.......z.
+000059a0: 6500 6900 6700 6500 2000 6100 6c00 6c00  e.i.g.e. .a.l.l.
+000059b0: 6508 0000 0000 0600 0000 0853 686f 7720  e..........Show 
+000059c0: 616c 6c07 0000 0008 5365 7474 696e 6773  all.....Settings
+000059d0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
+000059e0: 5374 6172 7407 0000 0008 5365 7474 696e  Start.....Settin
+000059f0: 6773 0103 0000 001a 0053 0074 0061 0072  gs.......S.t.a.r
+00005a00: 0074 0065 0020 0048 0061 006d 006c 0069  .t.e. .H.a.m.l.i
+00005a10: 0062 0800 0000 0006 0000 000c 5374 6172  .b..........Star
+00005a20: 7420 6861 6d6c 6962 0700 0000 0853 6574  t hamlib.....Set
+00005a30: 7469 6e67 7301 03ff ffff ff08 0000 0000  tings...........
+00005a40: 0600 0000 0453 746f 7007 0000 0008 5365  .....Stop.....Se
+00005a50: 7474 696e 6773 0103 0000 001a 0053 0074  ttings.......S.t
+00005a60: 006f 0070 0070 0065 0020 0048 0061 006d  .o.p.p.e. .H.a.m
+00005a70: 006c 0069 0062 0800 0000 0006 0000 000b  .l.i.b..........
+00005a80: 5374 6f70 2068 616d 6c69 6207 0000 0008  Stop hamlib.....
+00005a90: 5365 7474 696e 6773 0103 0000 000a 0061  Settings.......a
+00005aa0: 006b 0074 0069 0076 0800 0000 0006 0000  .k.t.i.v........
+00005ab0: 0005 6163 7469 7607 0000 0008 5365 7474  ..activ.....Sett
+00005ac0: 696e 6773 0103 0000 000e 0069 006e 0061  ings.......i.n.a
+00005ad0: 006b 0074 0069 0076 0800 0000 0006 0000  .k.t.i.v........
+00005ae0: 0007 696e 6163 7469 7607 0000 0008 5365  ..inactiv.....Se
+00005af0: 7474 696e 6773 0103 0000 004a 0072 0069  ttings.....J.r.i
+00005b00: 0067 0063 0074 006c 0064 0020 006b 006f  .g.c.t.l.d. .k.o
+00005b10: 006e 006e 0074 0065 0020 006e 0069 0063  .n.n.t.e. .n.i.c
+00005b20: 0068 0074 0020 0067 0065 0073 0074 0061  .h.t. .g.e.s.t.a
+00005b30: 0072 0074 0065 0074 0020 0077 0065 0072  .r.t.e.t. .w.e.r
+00005b40: 0064 0065 006e 0800 0000 0006 0000 001e  .d.e.n..........
+00005b50: 7269 6763 746c 6420 6469 6420 6e6f 7420  rigctld did not 
+00005b60: 7374 6172 7420 7072 6f70 6572 6c79 0700  start properly..
+00005b70: 0000 0853 6574 7469 6e67 7301 03ff ffff  ...Settings.....
+00005b80: ff08 0000 0000 0600 0000 074a 5338 4361  ...........JS8Ca
+00005b90: 6c6c 0700 0000 0f61 7070 5365 6c65 6374  ll.....appSelect
+00005ba0: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
+00005bb0: 0006 0000 0005 4f74 6865 7207 0000 000f  ......Other.....
+00005bc0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
+00005bd0: 0300 0000 2a00 4100 7500 7300 7700 6100  ....*.A.u.s.w.a.
+00005be0: 6800 6c00 2000 6400 6500 7300 2000 5000  h.l. .d.e.s. .P.
+00005bf0: 7200 6f00 6700 7200 6100 6d00 6d00 7308  r.o.g.r.a.m.m.s.
+00005c00: 0000 0000 0600 0000 1653 656c 6563 7420  .........Select 
+00005c10: 7468 6520 6170 706c 6963 6174 696f 6e07  the application.
+00005c20: 0000 000f 6170 7053 656c 6563 7444 6961  ....appSelectDia
+00005c30: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00005c40: 0000 0657 534a 542d 5807 0000 000f 6170  ...WSJT-X.....ap
+00005c50: 7053 656c 6563 7444 6961 6c6f 6701 03ff  pSelectDialog...
+00005c60: ffff ff08 0000 0000 0600 0000 0666 6c64  .............fld
+00005c70: 6967 6907 0000 000f 6170 7053 656c 6563  igi.....appSelec
+00005c80: 7444 6961 6c6f 6701 8800 0000 0201 01    tDialog........
```

### Comparing `DragonLog-0.8.1/dragonlog/data/modes.json` & `DragonLog-1.0/dragonlog/data/modes.json`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/db.png` & `DragonLog-1.0/dragonlog/icons/db.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/edit.png` & `DragonLog-1.0/dragonlog/icons/edit.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/edit_add.png` & `DragonLog-1.0/dragonlog/icons/edit_add.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/edit_addmulti.png` & `DragonLog-1.0/dragonlog/icons/edit_addmulti.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/edit_addmulti.xcf` & `DragonLog-1.0/dragonlog/icons/edit_addmulti.xcf`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/edit_remove.png` & `DragonLog-1.0/dragonlog/icons/edit_remove.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/exit.png` & `DragonLog-1.0/dragonlog/icons/exit.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/file_doc.png` & `DragonLog-1.0/dragonlog/icons/file_doc.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/fileexport.png` & `DragonLog-1.0/dragonlog/icons/fileexport.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/fileimport.png` & `DragonLog-1.0/dragonlog/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/gear.png` & `DragonLog-1.0/dragonlog/icons/gear.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/help.png` & `DragonLog-1.0/dragonlog/icons/help.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/icons8-dragon-96.png` & `DragonLog-1.0/dragonlog/icons/icons8-dragon-96.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/icons8-dragon-96.xcf` & `DragonLog-1.0/dragonlog/icons/icons8-dragon-96.xcf`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/info.png` & `DragonLog-1.0/dragonlog/icons/info.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/logo.ico` & `DragonLog-1.0/dragonlog/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/player_play.png` & `DragonLog-1.0/dragonlog/icons/player_play.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/player_stop.png` & `DragonLog-1.0/dragonlog/icons/player_stop.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/upload_lotw.png` & `DragonLog-1.0/dragonlog/icons/upload_lotw.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/upload_lotw.xcf` & `DragonLog-1.0/dragonlog/icons/upload_lotw.xcf`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/dragonlog/icons/watch.png` & `DragonLog-1.0/dragonlog/icons/watch.png`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/pyproject.toml` & `DragonLog-1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DragonLog-0.8.1/setup_msi.py` & `DragonLog-1.0/setup_msi.py`

 * *Files identical despite different names*

