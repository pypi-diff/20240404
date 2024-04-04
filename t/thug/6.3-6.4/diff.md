# Comparing `tmp/thug-6.3.tar.gz` & `tmp/thug-6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thug-6.3.tar", last modified: Wed Feb 28 14:59:39 2024, max compression
+gzip compressed data, was "thug-6.4.tar", last modified: Thu Apr  4 17:17:07 2024, max compression
```

## Comparing `thug-6.3.tar` & `thug-6.4.tar`

### file list

```diff
@@ -1,528 +1,520 @@
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.968904 thug-6.3/
--rw-r--r--   0 buffer    (1000) buffer    (1000)    17987 2022-11-28 09:02:06.000000 thug-6.3/LICENSE.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      130 2023-01-12 15:47:27.000000 thug-6.3/MANIFEST.in
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5534 2024-02-28 14:59:39.968904 thug-6.3/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2695 2024-01-19 09:00:07.000000 thug-6.3/README.rst
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3764 2024-02-28 14:22:02.000000 thug-6.3/pyproject.toml
--rw-r--r--   0 buffer    (1000) buffer    (1000)       38 2024-02-28 14:59:39.968904 thug-6.3/setup.cfg
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.733900 thug-6.3/thug/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.738900 thug-6.3/thug/ActiveX/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7458 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/ActiveX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    46031 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/CLSID.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/ActiveX/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.796901 thug-6.3/thug/ActiveX/modules/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      323 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AOLAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      871 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AcroPDF.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      610 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AdodbRecordset.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2404 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AdodbStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1275 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AnswerWorks.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      948 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AolAmpX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      736 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/AolICQ.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      620 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/BaiduBar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      498 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/BitDefender.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      360 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/CABrightStor.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      531 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/CGAgent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      446 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Comodo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ConnectAndEnterRoom.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/CreativeSoftAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      408 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/DLinkMPEG.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      605 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/DPClient.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      411 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/DVRHOSTWeb.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      548 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/DirectShow.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      342 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/DivX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1651 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Domino.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1170 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/EnjoySAP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      751 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/FacebookPhotoUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3094 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/File.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      441 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/FileUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2252 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Folder.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      460 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/GLIEDown2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      677 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/GatewayWeblaunch.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      383 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Gogago.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      492 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/GomWeb.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2728 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/HPInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      407 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ICQToolbar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      807 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/IMWebControl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      413 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/InternetCleverSuite.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1750 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/JavaDeploymentToolkit.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      368 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Kingsoft.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MSRICHTXT.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      411 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MSVFP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      457 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MSXML2DOMDocument.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3549 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MacrovisionFlexNet.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      295 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MicrosoftWorks7Attack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2119 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MicrosoftXMLDOM.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7787 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MicrosoftXMLHTTP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      430 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Move.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      376 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/MyspaceUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      520 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/NCTAudioFile2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      972 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/NamoInstaller.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      547 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/NeoTracePro.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2210 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/NessusScanCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      945 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/OfficeOCX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      919 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/OurgameGLWorld.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1066 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/PPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      462 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/PTZCamPanel.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      458 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/QuantumStreaming.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      447 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/QvodCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      712 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/RDSDataSpace.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2063 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/RealPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      285 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/RediffBolDownloaderAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      684 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/RegistryPro.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      316 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/RisingScanner.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/RtspVaPgCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      980 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SSReaderPdg2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1032 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ScriptingDictionary.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      342 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ScriptingEncoder.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4975 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ScriptingFileSystemObject.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1184 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ShellApplication.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      298 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Shockwave.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ShockwaveFlash10.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ShockwaveFlash11.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ShockwaveFlash12.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ShockwaveFlash9.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SilverLight.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SinaDLoader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1165 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SnapshotViewer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      646 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      754 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Spreadsheet.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      609 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/StormConfig.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2028 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/StormMps.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      480 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/StreamAudioChainCast.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      854 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SymantecAppStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1949 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/SymantecBackupExec.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4792 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/TextStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      713 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/Toshiba.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      330 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/UUSeeUpdate.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      502 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/UniversalUpload.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1445 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/VLC.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      527 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/VisualStudioDTE80.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      493 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/VsaIDEDTE.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      493 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/VsmIDEDTE.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      815 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WMEncProfileManager.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      132 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WMP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WScriptCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1279 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WScriptExec.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1726 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WScriptNetwork.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8198 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WScriptShell.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      218 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WScriptShortcut.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      590 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WebViewFolderIcon.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1358 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WinNTSystemInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      530 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WinZip.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      145 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/WindowsMediaPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      921 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/XMLDOMParseError.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      888 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/XUpload.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      976 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/YahooJukebox.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      446 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/YahooMessengerCyft.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      939 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/YahooMessengerYVerInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1102 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/YahooMessengerYwcvwr.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1660 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2079 2024-01-17 12:09:54.000000 thug-6.3/thug/ActiveX/modules/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.796901 thug-6.3/thug/Analysis/
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Analysis/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.798901 thug-6.3/thug/Analysis/awis/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3488 2024-01-17 12:09:54.000000 thug-6.3/thug/Analysis/awis/AWIS.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Analysis/awis/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.798901 thug-6.3/thug/Analysis/context/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1609 2024-01-17 12:09:54.000000 thug-6.3/thug/Analysis/context/ContextAnalyzer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Analysis/context/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.799901 thug-6.3/thug/Analysis/favicon/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2024-01-17 12:09:54.000000 thug-6.3/thug/Analysis/favicon/Favicon.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-09-11 08:32:02.000000 thug-6.3/thug/Analysis/favicon/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.800901 thug-6.3/thug/Analysis/honeyagent/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3980 2024-01-17 12:09:54.000000 thug-6.3/thug/Analysis/honeyagent/HoneyAgent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Analysis/honeyagent/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.802901 thug-6.3/thug/Analysis/screenshot/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1309 2024-01-17 12:09:54.000000 thug-6.3/thug/Analysis/screenshot/Screenshot.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Analysis/screenshot/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.802901 thug-6.3/thug/Analysis/shellcode/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8118 2024-01-17 12:09:54.000000 thug-6.3/thug/Analysis/shellcode/Shellcode.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Analysis/shellcode/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.807901 thug-6.3/thug/Classifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5394 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/BaseClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2094 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/CookieClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2147 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/HTMLClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2057 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/ImageClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1996 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/JSClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2230 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/SampleClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2070 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/TextClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2318 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/URLClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2002 2024-01-17 12:09:54.000000 thug-6.3/thug/Classifier/VBSClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Classifier/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.829902 thug-6.3/thug/DOM/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2327 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Alexa.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2236 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/AsyncPrefetcher.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2298 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/CCInterpreter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/Chrome.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1302 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/ClipboardData.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      817 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/Components.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5685 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Console.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1113 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Crypto.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    56116 2024-02-09 06:17:13.000000 thug-6.3/thug/DOM/DFT.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3511 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/External.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2831 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/HTMLInspector.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10997 2024-02-22 09:16:59.000000 thug-6.3/thug/DOM/HTTPSession.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/HTTPSessionException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3717 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/History.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3501 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/JSClass.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8294 2024-02-09 06:17:13.000000 thug-6.3/thug/DOM/JSEngine.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4395 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/JSInspector.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5971 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/JScriptEncode.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/LocalStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4873 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Location.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    18649 2024-02-09 06:17:13.000000 thug-6.3/thug/DOM/MIMEHandler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      762 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/Map.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1195 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/MimeType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4504 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/MimeTypes.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/MozConnection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    13892 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Navigator.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4191 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Personality.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1231 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Plugin.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1469 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Plugins.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1064 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/SchemeHandler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5954 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Screen.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      756 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/SessionStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1775 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Sidebar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2830 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/Storage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2805 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/UserProfile.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/Utils.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.831902 thug-6.3/thug/DOM/W3C/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.840902 thug-6.3/thug/DOM/W3C/Core/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2172 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Attr.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      266 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/CDATASection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1245 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/CharacterData.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3760 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/ClassList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      565 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Comment.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1893 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/DOMException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4988 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/DOMImplementation.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8842 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Document.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2422 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/DocumentFragment.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1512 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/DocumentType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9703 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Element.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      458 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Entity.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      501 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/EntityReference.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1295 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/NamedNodeMap.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    14383 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Node.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      617 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/NodeList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/NodeType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Notation.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      507 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/ProcessingInstruction.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      804 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/Text.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      939 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      362 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Core/abstractmethod.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/DOMParser.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1453 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/DOMTokenList.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.846902 thug-6.3/thug/DOM/W3C/Events/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      828 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/DocumentEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4094 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/Event.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      477 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/EventException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/EventListener.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9365 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/EventTarget.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      389 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/HTMLEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1174 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/MessageEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2068 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/MouseEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1557 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/MutationEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1113 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/StorageEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      634 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/UIEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      628 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Events/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.847902 thug-6.3/thug/DOM/W3C/File/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2380 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/File/Blob.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1377 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/File/File.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       74 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/File/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.878903 thug-6.3/thug/DOM/W3C/HTML/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      194 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/AudioTrackList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      611 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/Dataset.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      374 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLAllCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1878 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLAnchorElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      626 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLAppletElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLAudioElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      252 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLBRElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLBaseElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      329 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1484 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLBodyElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      561 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLButtonElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1278 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      265 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLDListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      263 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLDivElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16355 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLDocument.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      952 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4438 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      332 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      320 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLFontElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1689 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLFormElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      948 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLFrameElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      400 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLHRElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLHeadElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLHeadingElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLHtmlElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1219 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLIFrameElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1233 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLImageElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1330 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLInputElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      275 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      290 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLLIElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      366 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLLabelElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      367 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLLegendElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      532 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLLinkElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4236 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLMediaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      264 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLMenuElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      651 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLMetaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      292 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLModElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      373 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLOListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2550 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLObjectElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      663 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLOptionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      227 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      259 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLParagraphElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      364 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLParamElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLPreElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLQuoteElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      963 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLScriptElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1594 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLSelectElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      177 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLSpanElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      309 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLStyleElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      262 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      893 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTableCellElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      436 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTableColElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4449 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTableElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2865 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTableRowElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2075 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1004 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLTitleElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      333 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLUListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      654 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/HTMLVideoElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1042 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/TAnimateColor.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      281 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/TextTrackList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      683 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/TimeRanges.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4769 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      462 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/attr_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/bool_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      463 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/form_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      841 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/HTML/text_property.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.878903 thug-6.3/thug/DOM/W3C/Style/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.880903 thug-6.3/thug/DOM/W3C/Style/CSS/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1339 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      456 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/Style/CSS/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/Style/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.881903 thug-6.3/thug/DOM/W3C/URL/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5148 2024-02-09 06:17:13.000000 thug-6.3/thug/DOM/W3C/URL/URL.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2728 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/URL/URLSearchParams.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      104 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/URL/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.883903 thug-6.3/thug/DOM/W3C/Views/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      217 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/Views/AbstractView.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      211 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/Views/DocumentView.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/W3C/Views/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       34 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      365 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/W3C/w3c.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      829 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/WebStore.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    35463 2024-02-09 06:17:13.000000 thug-6.3/thug/DOM/Window.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/DOM/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4750 2024-01-17 12:09:54.000000 thug-6.3/thug/DOM/w3c_bindings.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.884903 thug-6.3/thug/Encoding/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2024-01-17 12:09:54.000000 thug-6.3/thug/Encoding/Encoding.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Encoding/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.886903 thug-6.3/thug/Java/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1109 2024-01-17 12:09:54.000000 thug-6.3/thug/Java/System.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Java/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      763 2022-11-28 09:02:06.000000 thug-6.3/thug/Java/java.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      771 2022-11-28 09:02:06.000000 thug-6.3/thug/Java/lang.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.889903 thug-6.3/thug/Logging/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2493 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/BaseLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3897 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/Features.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      902 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/LoggingModules.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4946 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/SampleLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    15290 2024-02-09 06:17:13.000000 thug-6.3/thug/Logging/ThugLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Logging/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.892903 thug-6.3/thug/Logging/modules/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2479 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/modules/ElasticSearch.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1293 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/modules/ExploitGraph.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    13218 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/modules/JSON.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10257 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/modules/Mapper.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16005 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/modules/MongoDB.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2024-01-17 12:09:54.000000 thug-6.3/thug/Logging/modules/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.894903 thug-6.3/thug/Magic/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1592 2024-01-17 12:09:54.000000 thug-6.3/thug/Magic/Magic.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Magic/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.894903 thug-6.3/thug/OS/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3503 2024-01-17 12:09:54.000000 thug-6.3/thug/OS/Windows.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/OS/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.896903 thug-6.3/thug/Plugins/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      956 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/IPlugin.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3438 2024-01-17 12:09:54.000000 thug-6.3/thug/Plugins/ThugPlugins.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.896903 thug-6.3/thug/Plugins/plugins/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.897903 thug-6.3/thug/Plugins/plugins/POST-TestPlugin-999/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.898903 thug-6.3/thug/Plugins/plugins/PRE-TestPlugin-999/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/Plugins/plugins/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.904903 thug-6.3/thug/ThugAPI/
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19217 2024-02-22 09:16:59.000000 thug-6.3/thug/ThugAPI/IThugAPI.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      787 2022-11-28 09:02:06.000000 thug-6.3/thug/ThugAPI/OpaqueFilter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16307 2024-02-22 09:16:59.000000 thug-6.3/thug/ThugAPI/ThugAPI.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10186 2024-02-22 09:16:59.000000 thug-6.3/thug/ThugAPI/ThugOpts.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4382 2024-01-17 12:09:54.000000 thug-6.3/thug/ThugAPI/ThugVulnModules.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1661 2024-01-17 12:09:54.000000 thug-6.3/thug/ThugAPI/Watchdog.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      147 2024-01-17 12:09:54.000000 thug-6.3/thug/ThugAPI/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-01-17 12:09:54.000000 thug-6.3/thug/ThugAPI/abstractmethod.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.906903 thug-6.3/thug/WebTracking/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3100 2024-01-17 12:09:54.000000 thug-6.3/thug/WebTracking/Cookies.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1176 2022-11-28 09:02:06.000000 thug-6.3/thug/WebTracking/WebStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1594 2024-01-17 12:09:54.000000 thug-6.3/thug/WebTracking/WebTracking.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.3/thug/WebTracking/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2203 2024-02-28 14:54:44.000000 thug-6.3/thug/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.907903 thug-6.3/thug/conf/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.908903 thug-6.3/thug/conf/hooks/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       45 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/hooks/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)      174 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/inspector.json
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.932904 thug-6.3/thug/conf/personalities/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/galaxy2chrome18.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/galaxy2chrome25.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      743 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/galaxy2chrome29.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      793 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome33.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome35.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome37.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome38.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome39.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome45.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome46.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      729 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadchrome47.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      692 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadsafari7.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      688 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadsafari8.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      680 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/ipadsafari9.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxchrome26.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxchrome30.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxchrome44.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxchrome54.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxchrome98.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxfirefox19.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/linuxfirefox40.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      748 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/nexuschrome18.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/osx10chrome19.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      690 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/osx10chrome80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/osx10chrome97.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/osx10safari5.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      682 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/osx11safari14.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      396 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/prefix_allocation.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2851 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win10edge20.json.review
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3826 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win10ie110.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win2kie60.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      915 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win2kie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7chrome20.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7chrome40.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7chrome45.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7chrome49.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      579 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7firefox3.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3769 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7ie100.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3800 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7ie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3820 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7ie90.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      678 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/win7safari5.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      674 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpchrome20.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      564 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpfirefox12.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2876 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpie60.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2896 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpie61.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2871 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpie70.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2968 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      666 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/personalities/winxpsafari5.json
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.933904 thug-6.3/thug/conf/plugins/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/plugins/README
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.937904 thug-6.3/thug/conf/rules/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.938904 thug-6.3/thug/conf/rules/cookieclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/cookieclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/cookieclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.938904 thug-6.3/thug/conf/rules/cookiefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/cookiefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/cookiefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.939904 thug-6.3/thug/conf/rules/htmlclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/htmlclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/htmlclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.939904 thug-6.3/thug/conf/rules/htmlfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/htmlfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/htmlfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.940904 thug-6.3/thug/conf/rules/imageclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      115 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/imageclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/imageclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.940904 thug-6.3/thug/conf/rules/imagefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      103 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/imagefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/imagefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.941904 thug-6.3/thug/conf/rules/jsclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/jsclassifier/plugindetect.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/jsclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.941904 thug-6.3/thug/conf/rules/jsfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       97 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/jsfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/jsfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.942904 thug-6.3/thug/conf/rules/sampleclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/sampleclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/sampleclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.942904 thug-6.3/thug/conf/rules/samplefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/samplefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/samplefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.943904 thug-6.3/thug/conf/rules/textclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/textclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/textclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.943904 thug-6.3/thug/conf/rules/textfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/textfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/textfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.955904 thug-6.3/thug/conf/rules/urlclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3005 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/blackhole.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/cool.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/crimeboss.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      641 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/critxpack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1000 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/fiesta.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      870 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/g01pack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      387 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/impact.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      808 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/neutrino.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      612 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/nuclear.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      969 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/popads.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      765 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/redkit.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      427 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/safepack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      176 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/sakura.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      478 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/sofosfo.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2400 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/styx.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      849 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/sweetorange.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier/tds.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.956904 thug-6.3/thug/conf/rules/urlfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/urlfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.957904 thug-6.3/thug/conf/rules/vbsclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/vbsclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/vbsclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.957904 thug-6.3/thug/conf/rules/vbsfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/vbsfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/rules/vbsfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.961904 thug-6.3/thug/conf/scripts/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3837 2024-02-09 06:17:13.000000 thug-6.3/thug/conf/scripts/atob.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1821 2024-02-09 06:17:13.000000 thug-6.3/thug/conf/scripts/btoa.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)       69 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/scripts/date.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      197 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/scripts/eval.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)       87 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/scripts/message-event.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/scripts/storage.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      753 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/scripts/thug.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      205 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/scripts/write.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      325 2023-01-12 15:47:27.000000 thug-6.3/thug/conf/thug.conf
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.965904 thug-6.3/thug/thug.egg-info/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4017 2022-12-08 08:47:59.000000 thug-6.3/thug/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19264 2022-12-08 08:47:59.000000 thug-6.3/thug/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-08 08:47:59.000000 thug-6.3/thug/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2022-12-08 08:47:59.000000 thug-6.3/thug/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2022-12-08 08:47:59.000000 thug-6.3/thug/thug.egg-info/requires.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       91 2022-12-08 08:47:59.000000 thug-6.3/thug/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-07 11:50:03.000000 thug-6.3/thug/thug.egg-info/zip-safe
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19877 2024-02-22 09:16:59.000000 thug-6.3/thug/thug.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-02-28 14:59:39.965904 thug-6.3/thug.egg-info/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5534 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16137 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      693 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/requires.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       10 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2024-02-28 14:59:39.000000 thug-6.3/thug.egg-info/zip-safe
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.693176 thug-6.4/
+-rw-r--r--   0 buffer     (501) staff       (20)    17987 2024-03-21 15:01:28.000000 thug-6.4/LICENSE.txt
+-rw-r--r--   0 buffer     (501) staff       (20)      130 2024-03-21 15:01:28.000000 thug-6.4/MANIFEST.in
+-rw-r--r--   0 buffer     (501) staff       (20)     5535 2024-04-04 17:17:07.692989 thug-6.4/PKG-INFO
+-rw-r--r--   0 buffer     (501) staff       (20)     2695 2024-03-21 15:01:28.000000 thug-6.4/README.rst
+-rw-r--r--   0 buffer     (501) staff       (20)     3765 2024-04-03 20:13:22.000000 thug-6.4/pyproject.toml
+-rw-r--r--   0 buffer     (501) staff       (20)       38 2024-04-04 17:17:07.693216 thug-6.4/setup.cfg
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.629256 thug-6.4/thug/
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.631259 thug-6.4/thug/ActiveX/
+-rw-r--r--   0 buffer     (501) staff       (20)     7458 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/ActiveX.py
+-rw-r--r--   0 buffer     (501) staff       (20)    46031 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/CLSID.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647273 thug-6.4/thug/ActiveX/modules/
+-rw-r--r--   0 buffer     (501) staff       (20)      323 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AOLAttack.py
+-rw-r--r--   0 buffer     (501) staff       (20)      871 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AcroPDF.py
+-rw-r--r--   0 buffer     (501) staff       (20)      610 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AdodbRecordset.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2404 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AdodbStream.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1275 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AnswerWorks.py
+-rw-r--r--   0 buffer     (501) staff       (20)      948 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AolAmpX.py
+-rw-r--r--   0 buffer     (501) staff       (20)      736 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AolICQ.py
+-rw-r--r--   0 buffer     (501) staff       (20)      620 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/BaiduBar.py
+-rw-r--r--   0 buffer     (501) staff       (20)      498 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/BitDefender.py
+-rw-r--r--   0 buffer     (501) staff       (20)      360 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/CABrightStor.py
+-rw-r--r--   0 buffer     (501) staff       (20)      531 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/CGAgent.py
+-rw-r--r--   0 buffer     (501) staff       (20)      446 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Comodo.py
+-rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ConnectAndEnterRoom.py
+-rw-r--r--   0 buffer     (501) staff       (20)      245 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/CreativeSoftAttack.py
+-rw-r--r--   0 buffer     (501) staff       (20)      408 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DLinkMPEG.py
+-rw-r--r--   0 buffer     (501) staff       (20)      605 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DPClient.py
+-rw-r--r--   0 buffer     (501) staff       (20)      411 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DVRHOSTWeb.py
+-rw-r--r--   0 buffer     (501) staff       (20)      548 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DirectShow.py
+-rw-r--r--   0 buffer     (501) staff       (20)      342 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DivX.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1651 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Domino.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1170 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/EnjoySAP.py
+-rw-r--r--   0 buffer     (501) staff       (20)      751 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/FacebookPhotoUploader.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3094 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/File.py
+-rw-r--r--   0 buffer     (501) staff       (20)      441 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/FileUploader.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2252 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Folder.py
+-rw-r--r--   0 buffer     (501) staff       (20)      460 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/GLIEDown2.py
+-rw-r--r--   0 buffer     (501) staff       (20)      677 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/GatewayWeblaunch.py
+-rw-r--r--   0 buffer     (501) staff       (20)      383 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Gogago.py
+-rw-r--r--   0 buffer     (501) staff       (20)      492 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/GomWeb.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2728 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/HPInfo.py
+-rw-r--r--   0 buffer     (501) staff       (20)      407 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ICQToolbar.py
+-rw-r--r--   0 buffer     (501) staff       (20)      807 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/IMWebControl.py
+-rw-r--r--   0 buffer     (501) staff       (20)      413 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/InternetCleverSuite.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1750 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/JavaDeploymentToolkit.py
+-rw-r--r--   0 buffer     (501) staff       (20)      932 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
+-rw-r--r--   0 buffer     (501) staff       (20)      368 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Kingsoft.py
+-rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MSRICHTXT.py
+-rw-r--r--   0 buffer     (501) staff       (20)      411 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MSVFP.py
+-rw-r--r--   0 buffer     (501) staff       (20)      457 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MSXML2DOMDocument.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3549 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MacrovisionFlexNet.py
+-rw-r--r--   0 buffer     (501) staff       (20)      295 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MicrosoftWorks7Attack.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2119 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MicrosoftXMLDOM.py
+-rw-r--r--   0 buffer     (501) staff       (20)     7787 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MicrosoftXMLHTTP.py
+-rw-r--r--   0 buffer     (501) staff       (20)      430 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Move.py
+-rw-r--r--   0 buffer     (501) staff       (20)      376 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MyspaceUploader.py
+-rw-r--r--   0 buffer     (501) staff       (20)      520 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NCTAudioFile2.py
+-rw-r--r--   0 buffer     (501) staff       (20)      972 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NamoInstaller.py
+-rw-r--r--   0 buffer     (501) staff       (20)      547 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NeoTracePro.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2210 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NessusScanCtrl.py
+-rw-r--r--   0 buffer     (501) staff       (20)      945 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/OfficeOCX.py
+-rw-r--r--   0 buffer     (501) staff       (20)      919 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/OurgameGLWorld.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1066 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/PPlayer.py
+-rw-r--r--   0 buffer     (501) staff       (20)      462 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/PTZCamPanel.py
+-rw-r--r--   0 buffer     (501) staff       (20)      458 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/QuantumStreaming.py
+-rw-r--r--   0 buffer     (501) staff       (20)      447 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/QvodCtrl.py
+-rw-r--r--   0 buffer     (501) staff       (20)      712 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RDSDataSpace.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2063 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RealPlayer.py
+-rw-r--r--   0 buffer     (501) staff       (20)      285 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RediffBolDownloaderAttack.py
+-rw-r--r--   0 buffer     (501) staff       (20)      684 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RegistryPro.py
+-rw-r--r--   0 buffer     (501) staff       (20)      316 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RisingScanner.py
+-rw-r--r--   0 buffer     (501) staff       (20)      412 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RtspVaPgCtrl.py
+-rw-r--r--   0 buffer     (501) staff       (20)      980 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SSReaderPdg2.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1032 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ScriptingDictionary.py
+-rw-r--r--   0 buffer     (501) staff       (20)      342 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ScriptingEncoder.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4975 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ScriptingFileSystemObject.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1184 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShellApplication.py
+-rw-r--r--   0 buffer     (501) staff       (20)      298 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Shockwave.py
+-rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash10.py
+-rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash11.py
+-rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash12.py
+-rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash9.py
+-rw-r--r--   0 buffer     (501) staff       (20)      274 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SilverLight.py
+-rw-r--r--   0 buffer     (501) staff       (20)      752 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SinaDLoader.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1165 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SnapshotViewer.py
+-rw-r--r--   0 buffer     (501) staff       (20)      646 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
+-rw-r--r--   0 buffer     (501) staff       (20)      754 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Spreadsheet.py
+-rw-r--r--   0 buffer     (501) staff       (20)      609 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/StormConfig.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2028 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/StormMps.py
+-rw-r--r--   0 buffer     (501) staff       (20)      480 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/StreamAudioChainCast.py
+-rw-r--r--   0 buffer     (501) staff       (20)      854 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SymantecAppStream.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1949 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SymantecBackupExec.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4792 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/TextStream.py
+-rw-r--r--   0 buffer     (501) staff       (20)      713 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Toshiba.py
+-rw-r--r--   0 buffer     (501) staff       (20)      330 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/UUSeeUpdate.py
+-rw-r--r--   0 buffer     (501) staff       (20)      502 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/UniversalUpload.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1445 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VLC.py
+-rw-r--r--   0 buffer     (501) staff       (20)      527 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VisualStudioDTE80.py
+-rw-r--r--   0 buffer     (501) staff       (20)      493 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VsaIDEDTE.py
+-rw-r--r--   0 buffer     (501) staff       (20)      493 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VsmIDEDTE.py
+-rw-r--r--   0 buffer     (501) staff       (20)      815 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WMEncProfileManager.py
+-rw-r--r--   0 buffer     (501) staff       (20)      132 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WMP.py
+-rw-r--r--   0 buffer     (501) staff       (20)      257 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptCollection.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1279 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptExec.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1726 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptNetwork.py
+-rw-r--r--   0 buffer     (501) staff       (20)     8198 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptShell.py
+-rw-r--r--   0 buffer     (501) staff       (20)      218 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptShortcut.py
+-rw-r--r--   0 buffer     (501) staff       (20)      590 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WebViewFolderIcon.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1358 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WinNTSystemInfo.py
+-rw-r--r--   0 buffer     (501) staff       (20)      530 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WinZip.py
+-rw-r--r--   0 buffer     (501) staff       (20)      145 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WindowsMediaPlayer.py
+-rw-r--r--   0 buffer     (501) staff       (20)      921 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/XMLDOMParseError.py
+-rw-r--r--   0 buffer     (501) staff       (20)      888 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/XUpload.py
+-rw-r--r--   0 buffer     (501) staff       (20)      976 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooJukebox.py
+-rw-r--r--   0 buffer     (501) staff       (20)      446 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooMessengerCyft.py
+-rw-r--r--   0 buffer     (501) staff       (20)      939 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooMessengerYVerInfo.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1102 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooMessengerYwcvwr.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1660 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2079 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647395 thug-6.4/thug/Analysis/
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647600 thug-6.4/thug/Analysis/awis/
+-rw-r--r--   0 buffer     (501) staff       (20)     3488 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/awis/AWIS.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/awis/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647798 thug-6.4/thug/Analysis/context/
+-rw-r--r--   0 buffer     (501) staff       (20)     1609 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/context/ContextAnalyzer.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/context/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647995 thug-6.4/thug/Analysis/favicon/
+-rw-r--r--   0 buffer     (501) staff       (20)      394 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/favicon/Favicon.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/favicon/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.648198 thug-6.4/thug/Analysis/honeyagent/
+-rw-r--r--   0 buffer     (501) staff       (20)     3980 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/honeyagent/HoneyAgent.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/honeyagent/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.648432 thug-6.4/thug/Analysis/screenshot/
+-rw-r--r--   0 buffer     (501) staff       (20)     1309 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/screenshot/Screenshot.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/screenshot/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.648717 thug-6.4/thug/Analysis/shellcode/
+-rw-r--r--   0 buffer     (501) staff       (20)     8118 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/shellcode/Shellcode.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/shellcode/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.649960 thug-6.4/thug/Classifier/
+-rw-r--r--   0 buffer     (501) staff       (20)     5394 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/BaseClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2094 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/CookieClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2147 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/HTMLClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2057 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/ImageClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1996 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/JSClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2230 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/SampleClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2070 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/TextClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2318 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/URLClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2002 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/VBSClassifier.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.657016 thug-6.4/thug/DOM/
+-rw-r--r--   0 buffer     (501) staff       (20)     2327 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Alexa.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2236 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/AsyncPrefetcher.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2298 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/CCInterpreter.py
+-rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Chrome.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1302 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/ClipboardData.py
+-rw-r--r--   0 buffer     (501) staff       (20)      817 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Components.py
+-rw-r--r--   0 buffer     (501) staff       (20)     5685 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Console.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1113 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Crypto.py
+-rw-r--r--   0 buffer     (501) staff       (20)    56116 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/DFT.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3511 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/External.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2831 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/HTMLInspector.py
+-rw-r--r--   0 buffer     (501) staff       (20)    10997 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/HTTPSession.py
+-rw-r--r--   0 buffer     (501) staff       (20)      932 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/HTTPSessionException.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3717 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/History.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3501 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JSClass.py
+-rw-r--r--   0 buffer     (501) staff       (20)     8294 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JSEngine.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4395 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JSInspector.py
+-rw-r--r--   0 buffer     (501) staff       (20)     5971 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JScriptEncode.py
+-rw-r--r--   0 buffer     (501) staff       (20)      752 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/LocalStorage.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4873 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Location.py
+-rw-r--r--   0 buffer     (501) staff       (20)    18649 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MIMEHandler.py
+-rw-r--r--   0 buffer     (501) staff       (20)      762 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Map.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1195 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MimeType.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4504 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MimeTypes.py
+-rw-r--r--   0 buffer     (501) staff       (20)      782 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MozConnection.py
+-rw-r--r--   0 buffer     (501) staff       (20)    13892 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Navigator.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4191 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Personality.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1231 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Plugin.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1469 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Plugins.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1064 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/SchemeHandler.py
+-rw-r--r--   0 buffer     (501) staff       (20)     5954 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Screen.py
+-rw-r--r--   0 buffer     (501) staff       (20)      756 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/SessionStorage.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1775 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Sidebar.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2830 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Storage.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2805 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/UserProfile.py
+-rw-r--r--   0 buffer     (501) staff       (20)      766 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Utils.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.657648 thug-6.4/thug/DOM/W3C/
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.660670 thug-6.4/thug/DOM/W3C/Core/
+-rw-r--r--   0 buffer     (501) staff       (20)     2172 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Attr.py
+-rw-r--r--   0 buffer     (501) staff       (20)      266 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/CDATASection.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1245 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/CharacterData.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3760 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/ClassList.py
+-rw-r--r--   0 buffer     (501) staff       (20)      565 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Comment.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1893 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DOMException.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4988 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DOMImplementation.py
+-rw-r--r--   0 buffer     (501) staff       (20)     8842 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Document.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2422 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DocumentFragment.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1512 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DocumentType.py
+-rw-r--r--   0 buffer     (501) staff       (20)     9703 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Element.py
+-rw-r--r--   0 buffer     (501) staff       (20)      458 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Entity.py
+-rw-r--r--   0 buffer     (501) staff       (20)      501 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/EntityReference.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1295 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/NamedNodeMap.py
+-rw-r--r--   0 buffer     (501) staff       (20)    14383 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Node.py
+-rw-r--r--   0 buffer     (501) staff       (20)      617 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/NodeList.py
+-rw-r--r--   0 buffer     (501) staff       (20)      341 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/NodeType.py
+-rw-r--r--   0 buffer     (501) staff       (20)      486 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Notation.py
+-rw-r--r--   0 buffer     (501) staff       (20)      507 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/ProcessingInstruction.py
+-rw-r--r--   0 buffer     (501) staff       (20)      804 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Text.py
+-rw-r--r--   0 buffer     (501) staff       (20)      939 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)      362 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/abstractmethod.py
+-rw-r--r--   0 buffer     (501) staff       (20)      274 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/DOMParser.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1453 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/DOMTokenList.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.662004 thug-6.4/thug/DOM/W3C/Events/
+-rw-r--r--   0 buffer     (501) staff       (20)      828 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/DocumentEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4094 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/Event.py
+-rw-r--r--   0 buffer     (501) staff       (20)      477 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/EventException.py
+-rw-r--r--   0 buffer     (501) staff       (20)      274 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/EventListener.py
+-rw-r--r--   0 buffer     (501) staff       (20)     9365 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/EventTarget.py
+-rw-r--r--   0 buffer     (501) staff       (20)      389 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/HTMLEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1174 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/MessageEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2068 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/MouseEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1557 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/MutationEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1113 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/StorageEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)      634 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/UIEvent.py
+-rw-r--r--   0 buffer     (501) staff       (20)      628 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.662329 thug-6.4/thug/DOM/W3C/File/
+-rw-r--r--   0 buffer     (501) staff       (20)     2380 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/File/Blob.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1377 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/File/File.py
+-rw-r--r--   0 buffer     (501) staff       (20)       74 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/File/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673074 thug-6.4/thug/DOM/W3C/HTML/
+-rw-r--r--   0 buffer     (501) staff       (20)      194 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/AudioTrackList.py
+-rw-r--r--   0 buffer     (501) staff       (20)      611 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/Dataset.py
+-rw-r--r--   0 buffer     (501) staff       (20)      374 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAllCollection.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1878 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAnchorElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      626 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAppletElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      247 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAudioElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      252 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBRElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      289 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBaseElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      329 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1484 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBodyElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      561 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLButtonElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1278 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLCollection.py
+-rw-r--r--   0 buffer     (501) staff       (20)      265 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDListElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      263 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      253 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDivElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)    16355 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDocument.py
+-rw-r--r--   0 buffer     (501) staff       (20)      952 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
+-rw-r--r--   0 buffer     (501) staff       (20)      412 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4438 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      332 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      320 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFontElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      204 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1689 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFormElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      948 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFrameElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      289 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      400 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHRElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      258 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHeadElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      257 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHeadingElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      258 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHtmlElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1219 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLIFrameElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1233 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLImageElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1330 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLInputElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      275 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      290 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLIElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      366 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLabelElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      367 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLegendElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      532 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLinkElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4236 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLMediaElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      264 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLMenuElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      651 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLMetaElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      292 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLModElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      373 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOListElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2550 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLObjectElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      340 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      663 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOptionElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      227 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
+-rw-r--r--   0 buffer     (501) staff       (20)      259 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLParagraphElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      364 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLParamElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      258 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLPreElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      253 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLQuoteElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      963 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLScriptElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1594 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLSelectElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      177 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLSpanElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      309 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLStyleElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      262 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      893 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableCellElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      436 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableColElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4449 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2865 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableRowElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2075 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1004 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      247 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTitleElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      333 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLUListElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)      654 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLVideoElement.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1042 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/TAnimateColor.py
+-rw-r--r--   0 buffer     (501) staff       (20)      281 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/TextTrackList.py
+-rw-r--r--   0 buffer     (501) staff       (20)      683 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/TimeRanges.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4769 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)      462 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/attr_property.py
+-rw-r--r--   0 buffer     (501) staff       (20)      418 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/bool_property.py
+-rw-r--r--   0 buffer     (501) staff       (20)      463 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/form_property.py
+-rw-r--r--   0 buffer     (501) staff       (20)      841 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/text_property.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673183 thug-6.4/thug/DOM/W3C/Style/
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673523 thug-6.4/thug/DOM/W3C/Style/CSS/
+-rw-r--r--   0 buffer     (501) staff       (20)     1339 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
+-rw-r--r--   0 buffer     (501) staff       (20)      456 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/CSS/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673862 thug-6.4/thug/DOM/W3C/URL/
+-rw-r--r--   0 buffer     (501) staff       (20)     5148 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/URL/URL.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2728 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/URL/URLSearchParams.py
+-rw-r--r--   0 buffer     (501) staff       (20)      104 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/URL/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.674233 thug-6.4/thug/DOM/W3C/Views/
+-rw-r--r--   0 buffer     (501) staff       (20)      217 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Views/AbstractView.py
+-rw-r--r--   0 buffer     (501) staff       (20)      211 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Views/DocumentView.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Views/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)       34 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)      365 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/w3c.py
+-rw-r--r--   0 buffer     (501) staff       (20)      829 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/WebStore.py
+-rw-r--r--   0 buffer     (501) staff       (20)    35463 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Window.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4750 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/w3c_bindings.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.674418 thug-6.4/thug/Encoding/
+-rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/Encoding/Encoding.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Encoding/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.674783 thug-6.4/thug/Java/
+-rw-r--r--   0 buffer     (501) staff       (20)     1109 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/System.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)      763 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/java.py
+-rw-r--r--   0 buffer     (501) staff       (20)      771 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/lang.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.675626 thug-6.4/thug/Logging/
+-rw-r--r--   0 buffer     (501) staff       (20)     2493 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/BaseLogging.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3897 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/Features.py
+-rw-r--r--   0 buffer     (501) staff       (20)      902 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/LoggingModules.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4946 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/SampleLogging.py
+-rw-r--r--   0 buffer     (501) staff       (20)    15290 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/ThugLogging.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.676559 thug-6.4/thug/Logging/modules/
+-rw-r--r--   0 buffer     (501) staff       (20)     2479 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/ElasticSearch.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1293 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/ExploitGraph.py
+-rw-r--r--   0 buffer     (501) staff       (20)    13218 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/JSON.py
+-rw-r--r--   0 buffer     (501) staff       (20)    10257 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/Mapper.py
+-rw-r--r--   0 buffer     (501) staff       (20)    16005 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/MongoDB.py
+-rw-r--r--   0 buffer     (501) staff       (20)       47 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.676895 thug-6.4/thug/Magic/
+-rw-r--r--   0 buffer     (501) staff       (20)     1592 2024-03-21 15:01:28.000000 thug-6.4/thug/Magic/Magic.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Magic/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677177 thug-6.4/thug/OS/
+-rw-r--r--   0 buffer     (501) staff       (20)     3503 2024-03-21 15:01:28.000000 thug-6.4/thug/OS/Windows.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/OS/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677635 thug-6.4/thug/Plugins/
+-rw-r--r--   0 buffer     (501) staff       (20)      956 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/IPlugin.py
+-rw-r--r--   0 buffer     (501) staff       (20)     3438 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/ThugPlugins.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677726 thug-6.4/thug/Plugins/plugins/
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677938 thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/
+-rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.678144 thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/
+-rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.679514 thug-6.4/thug/ThugAPI/
+-rw-r--r--   0 buffer     (501) staff       (20)    19217 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/IThugAPI.py
+-rw-r--r--   0 buffer     (501) staff       (20)      787 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/OpaqueFilter.py
+-rw-r--r--   0 buffer     (501) staff       (20)    16307 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/ThugAPI.py
+-rw-r--r--   0 buffer     (501) staff       (20)    10186 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/ThugOpts.py
+-rw-r--r--   0 buffer     (501) staff       (20)     4382 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/ThugVulnModules.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1661 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/Watchdog.py
+-rw-r--r--   0 buffer     (501) staff       (20)      147 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)      341 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/abstractmethod.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.680003 thug-6.4/thug/WebTracking/
+-rw-r--r--   0 buffer     (501) staff       (20)     3100 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/Cookies.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1176 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/WebStorage.py
+-rw-r--r--   0 buffer     (501) staff       (20)     1594 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/WebTracking.py
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/__init__.py
+-rw-r--r--   0 buffer     (501) staff       (20)     2203 2024-04-04 16:35:48.000000 thug-6.4/thug/__init__.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.680210 thug-6.4/thug/conf/
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.680322 thug-6.4/thug/conf/hooks/
+-rw-r--r--   0 buffer     (501) staff       (20)       45 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/hooks/README
+-rw-r--r--   0 buffer     (501) staff       (20)      174 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/inspector.json
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.685898 thug-6.4/thug/conf/personalities/
+-rw-r--r--   0 buffer     (501) staff       (20)      747 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/galaxy2chrome18.json
+-rw-r--r--   0 buffer     (501) staff       (20)      747 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/galaxy2chrome25.json
+-rw-r--r--   0 buffer     (501) staff       (20)      743 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/galaxy2chrome29.json
+-rw-r--r--   0 buffer     (501) staff       (20)      793 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome33.json
+-rw-r--r--   0 buffer     (501) staff       (20)      739 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome35.json
+-rw-r--r--   0 buffer     (501) staff       (20)      739 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome37.json
+-rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome38.json
+-rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome39.json
+-rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome45.json
+-rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome46.json
+-rw-r--r--   0 buffer     (501) staff       (20)      729 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome47.json
+-rw-r--r--   0 buffer     (501) staff       (20)      692 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadsafari7.json
+-rw-r--r--   0 buffer     (501) staff       (20)      688 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadsafari8.json
+-rw-r--r--   0 buffer     (501) staff       (20)      680 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadsafari9.json
+-rw-r--r--   0 buffer     (501) staff       (20)      648 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome26.json
+-rw-r--r--   0 buffer     (501) staff       (20)      648 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome30.json
+-rw-r--r--   0 buffer     (501) staff       (20)      648 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome44.json
+-rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome54.json
+-rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome98.json
+-rw-r--r--   0 buffer     (501) staff       (20)      524 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxfirefox19.json
+-rw-r--r--   0 buffer     (501) staff       (20)      524 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxfirefox40.json
+-rw-r--r--   0 buffer     (501) staff       (20)      748 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/nexuschrome18.json
+-rw-r--r--   0 buffer     (501) staff       (20)      679 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10chrome19.json
+-rw-r--r--   0 buffer     (501) staff       (20)      690 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10chrome80.json
+-rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10chrome97.json
+-rw-r--r--   0 buffer     (501) staff       (20)      679 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10safari5.json
+-rw-r--r--   0 buffer     (501) staff       (20)      682 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx11safari14.json
+-rw-r--r--   0 buffer     (501) staff       (20)      396 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/prefix_allocation.txt
+-rw-r--r--   0 buffer     (501) staff       (20)     2851 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win10edge20.json.review
+-rw-r--r--   0 buffer     (501) staff       (20)     3826 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win10ie110.json
+-rw-r--r--   0 buffer     (501) staff       (20)      782 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win2kie60.json
+-rw-r--r--   0 buffer     (501) staff       (20)      915 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win2kie80.json
+-rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome20.json
+-rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome40.json
+-rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome45.json
+-rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome49.json
+-rw-r--r--   0 buffer     (501) staff       (20)      579 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7firefox3.json
+-rw-r--r--   0 buffer     (501) staff       (20)     3769 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7ie100.json
+-rw-r--r--   0 buffer     (501) staff       (20)     3800 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7ie80.json
+-rw-r--r--   0 buffer     (501) staff       (20)     3820 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7ie90.json
+-rw-r--r--   0 buffer     (501) staff       (20)      678 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7safari5.json
+-rw-r--r--   0 buffer     (501) staff       (20)      674 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpchrome20.json
+-rw-r--r--   0 buffer     (501) staff       (20)      564 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpfirefox12.json
+-rw-r--r--   0 buffer     (501) staff       (20)     2876 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie60.json
+-rw-r--r--   0 buffer     (501) staff       (20)     2896 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie61.json
+-rw-r--r--   0 buffer     (501) staff       (20)     2871 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie70.json
+-rw-r--r--   0 buffer     (501) staff       (20)     2968 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie80.json
+-rw-r--r--   0 buffer     (501) staff       (20)      666 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpsafari5.json
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.686010 thug-6.4/thug/conf/plugins/
+-rw-r--r--   0 buffer     (501) staff       (20)       47 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/plugins/README
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687280 thug-6.4/thug/conf/rules/
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687356 thug-6.4/thug/conf/rules/cookieclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      117 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookieclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookieclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687469 thug-6.4/thug/conf/rules/cookiefilter/
+-rw-r--r--   0 buffer     (501) staff       (20)      105 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookiefilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookiefilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687578 thug-6.4/thug/conf/rules/htmlclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      113 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687689 thug-6.4/thug/conf/rules/htmlfilter/
+-rw-r--r--   0 buffer     (501) staff       (20)      101 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlfilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlfilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687804 thug-6.4/thug/conf/rules/imageclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      115 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imageclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imageclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687924 thug-6.4/thug/conf/rules/imagefilter/
+-rw-r--r--   0 buffer     (501) staff       (20)      103 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imagefilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imagefilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688035 thug-6.4/thug/conf/rules/jsclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      245 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsclassifier/plugindetect.yar
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688147 thug-6.4/thug/conf/rules/jsfilter/
+-rw-r--r--   0 buffer     (501) staff       (20)       97 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsfilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsfilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688261 thug-6.4/thug/conf/rules/sampleclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      117 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/sampleclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/sampleclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688388 thug-6.4/thug/conf/rules/samplefilter/
+-rw-r--r--   0 buffer     (501) staff       (20)      105 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/samplefilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/samplefilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688503 thug-6.4/thug/conf/rules/textclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      113 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688615 thug-6.4/thug/conf/rules/textfilter/
+-rw-r--r--   0 buffer     (501) staff       (20)      101 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textfilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textfilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690628 thug-6.4/thug/conf/rules/urlclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      111 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)     3005 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/blackhole.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      418 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/cool.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      766 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/crimeboss.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      641 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/critxpack.yar
+-rw-r--r--   0 buffer     (501) staff       (20)     1000 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/fiesta.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      870 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/g01pack.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      387 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/impact.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      808 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/neutrino.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      612 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/nuclear.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      969 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/popads.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      765 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/redkit.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      427 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/safepack.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      176 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/sakura.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      478 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/sofosfo.yar
+-rw-r--r--   0 buffer     (501) staff       (20)     2400 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/styx.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      849 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/sweetorange.yar
+-rw-r--r--   0 buffer     (501) staff       (20)      340 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/tds.yar
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690757 thug-6.4/thug/conf/rules/urlfilter/
+-rw-r--r--   0 buffer     (501) staff       (20)       99 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlfilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlfilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690873 thug-6.4/thug/conf/rules/vbsclassifier/
+-rw-r--r--   0 buffer     (501) staff       (20)      111 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsclassifier/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsclassifier.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690983 thug-6.4/thug/conf/rules/vbsfilter/
+-rw-r--r--   0 buffer     (501) staff       (20)       99 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsfilter/README
+-rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsfilter.yar
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.691900 thug-6.4/thug/conf/scripts/
+-rw-r--r--   0 buffer     (501) staff       (20)     3837 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/atob.js
+-rw-r--r--   0 buffer     (501) staff       (20)     1821 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/btoa.js
+-rw-r--r--   0 buffer     (501) staff       (20)       69 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/date.js
+-rw-r--r--   0 buffer     (501) staff       (20)      197 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/eval.js
+-rw-r--r--   0 buffer     (501) staff       (20)       87 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/message-event.js
+-rw-r--r--   0 buffer     (501) staff       (20)      204 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/storage.js
+-rw-r--r--   0 buffer     (501) staff       (20)      753 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/thug.js
+-rw-r--r--   0 buffer     (501) staff       (20)      205 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/write.js
+-rw-r--r--   0 buffer     (501) staff       (20)      325 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/thug.conf
+-rw-r--r--   0 buffer     (501) staff       (20)    19877 2024-03-21 15:01:28.000000 thug-6.4/thug/thug.py
+drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.692071 thug-6.4/thug.egg-info/
+-rw-r--r--   0 buffer     (501) staff       (20)     5535 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/PKG-INFO
+-rw-r--r--   0 buffer     (501) staff       (20)    15909 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 buffer     (501) staff       (20)        1 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 buffer     (501) staff       (20)       40 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/entry_points.txt
+-rw-r--r--   0 buffer     (501) staff       (20)      694 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/requires.txt
+-rw-r--r--   0 buffer     (501) staff       (20)       10 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/top_level.txt
+-rw-r--r--   0 buffer     (501) staff       (20)        1 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/zip-safe
```

### Comparing `thug-6.3/LICENSE.txt` & `thug-6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thug-6.3/PKG-INFO` & `thug-6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 6.3
+Version: 6.4
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
@@ -26,32 +26,32 @@
 Classifier: Topic :: Security
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: cssutils==2.9.0
+Requires-Dist: cssutils==2.10.2
 Requires-Dist: dhash==1.4
 Requires-Dist: html5lib==1.1
-Requires-Dist: lxml==5.1.0
+Requires-Dist: lxml==5.2.1
 Requires-Dist: networkx==3.2.1
 Requires-Dist: pefile==2023.2.7
-Requires-Dist: pillow==10.2.0
+Requires-Dist: pillow==10.3.0
 Requires-Dist: promise==2.3
 Requires-Dist: pylibemu==1.0
-Requires-Dist: pymongo==4.6.2
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: pysocks==1.7.1
 Requires-Dist: python-magic==0.4.27
-Requires-Dist: rarfile==4.1
+Requires-Dist: rarfile==4.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-futures==1.0.1
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: ssdeep==3.4
-Requires-Dist: stpyv8==12.2.281.19
+Requires-Dist: stpyv8==12.3.219.16
 Requires-Dist: yara-python==4.5.0
 Requires-Dist: zope.interface==6.2
 Requires-Dist: importlib-resources==6.0.1; python_version < "3.9"
 Provides-Extra: elasticsearch
 Requires-Dist: elasticsearch; extra == "elasticsearch"
 Provides-Extra: exploitgraph
 Requires-Dist: pygraphviz; extra == "exploitgraph"
```

### Comparing `thug-6.3/README.rst` & `thug-6.4/README.rst`

 * *Files identical despite different names*

### Comparing `thug-6.3/pyproject.toml` & `thug-6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,32 +35,32 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Security",
 ]
 dependencies = [
     "appdirs==1.4.4",
     "beautifulsoup4==4.12.3",
     "charset-normalizer==3.3.2",
-    "cssutils==2.9.0",
+    "cssutils==2.10.2",
     "dhash==1.4",
     "html5lib==1.1",
-    "lxml==5.1.0",
+    "lxml==5.2.1",
     "networkx==3.2.1",
     "pefile==2023.2.7",
-    "pillow==10.2.0",
+    "pillow==10.3.0",
     "promise==2.3",
     "pylibemu==1.0",
-    "pymongo==4.6.2",
+    "pymongo==4.6.3",
     "pysocks==1.7.1",
     "python-magic==0.4.27",
-    "rarfile==4.1",
+    "rarfile==4.2",
     "requests==2.31.0",
     "requests-futures==1.0.1",
     "setuptools>=65.5.1",
     "ssdeep==3.4",
-    "stpyv8==12.2.281.19",
+    "stpyv8==12.3.219.16",
     "yara-python==4.5.0",
     "zope.interface==6.2",
 
     # Conditional
     'importlib-resources==6.0.1; python_version < "3.9"',
 ]
 keywords = [
```

### Comparing `thug-6.3/thug/ActiveX/ActiveX.py` & `thug-6.4/thug/ActiveX/ActiveX.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/CLSID.py` & `thug-6.4/thug/ActiveX/CLSID.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/AcroPDF.py` & `thug-6.4/thug/ActiveX/modules/AcroPDF.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/AdodbRecordset.py` & `thug-6.4/thug/ActiveX/modules/AdodbRecordset.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/AdodbStream.py` & `thug-6.4/thug/ActiveX/modules/AdodbStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/AnswerWorks.py` & `thug-6.4/thug/ActiveX/modules/AnswerWorks.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/AolAmpX.py` & `thug-6.4/thug/ActiveX/modules/AolAmpX.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/AolICQ.py` & `thug-6.4/thug/ActiveX/modules/AolICQ.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/BaiduBar.py` & `thug-6.4/thug/ActiveX/modules/BaiduBar.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/CGAgent.py` & `thug-6.4/thug/ActiveX/modules/CGAgent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/ConnectAndEnterRoom.py` & `thug-6.4/thug/ActiveX/modules/ConnectAndEnterRoom.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/DPClient.py` & `thug-6.4/thug/ActiveX/modules/DPClient.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/DirectShow.py` & `thug-6.4/thug/ActiveX/modules/DirectShow.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/Domino.py` & `thug-6.4/thug/ActiveX/modules/Domino.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/EnjoySAP.py` & `thug-6.4/thug/ActiveX/modules/EnjoySAP.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/FacebookPhotoUploader.py` & `thug-6.4/thug/ActiveX/modules/FacebookPhotoUploader.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/File.py` & `thug-6.4/thug/ActiveX/modules/File.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/Folder.py` & `thug-6.4/thug/ActiveX/modules/Folder.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/GatewayWeblaunch.py` & `thug-6.4/thug/ActiveX/modules/GatewayWeblaunch.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/HPInfo.py` & `thug-6.4/thug/ActiveX/modules/HPInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/IMWebControl.py` & `thug-6.4/thug/ActiveX/modules/IMWebControl.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/JavaDeploymentToolkit.py` & `thug-6.4/thug/ActiveX/modules/JavaDeploymentToolkit.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py` & `thug-6.4/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/MSRICHTXT.py` & `thug-6.4/thug/ActiveX/modules/MSRICHTXT.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/MacrovisionFlexNet.py` & `thug-6.4/thug/ActiveX/modules/MacrovisionFlexNet.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/MicrosoftXMLDOM.py` & `thug-6.4/thug/ActiveX/modules/MicrosoftXMLDOM.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/MicrosoftXMLHTTP.py` & `thug-6.4/thug/ActiveX/modules/MicrosoftXMLHTTP.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/NCTAudioFile2.py` & `thug-6.4/thug/ActiveX/modules/NCTAudioFile2.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/NamoInstaller.py` & `thug-6.4/thug/ActiveX/modules/NamoInstaller.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/NeoTracePro.py` & `thug-6.4/thug/ActiveX/modules/NeoTracePro.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/NessusScanCtrl.py` & `thug-6.4/thug/ActiveX/modules/NessusScanCtrl.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/OfficeOCX.py` & `thug-6.4/thug/ActiveX/modules/OfficeOCX.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/OurgameGLWorld.py` & `thug-6.4/thug/ActiveX/modules/OurgameGLWorld.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/PPlayer.py` & `thug-6.4/thug/ActiveX/modules/PPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/RDSDataSpace.py` & `thug-6.4/thug/ActiveX/modules/RDSDataSpace.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/RealPlayer.py` & `thug-6.4/thug/ActiveX/modules/RealPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/RegistryPro.py` & `thug-6.4/thug/ActiveX/modules/RegistryPro.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/SSReaderPdg2.py` & `thug-6.4/thug/ActiveX/modules/SSReaderPdg2.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/ScriptingDictionary.py` & `thug-6.4/thug/ActiveX/modules/ScriptingDictionary.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/ScriptingFileSystemObject.py` & `thug-6.4/thug/ActiveX/modules/ScriptingFileSystemObject.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/ShellApplication.py` & `thug-6.4/thug/ActiveX/modules/ShellApplication.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/SinaDLoader.py` & `thug-6.4/thug/ActiveX/modules/SinaDLoader.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/SnapshotViewer.py` & `thug-6.4/thug/ActiveX/modules/SnapshotViewer.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py` & `thug-6.4/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/Spreadsheet.py` & `thug-6.4/thug/ActiveX/modules/Spreadsheet.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/StormConfig.py` & `thug-6.4/thug/ActiveX/modules/StormConfig.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/StormMps.py` & `thug-6.4/thug/ActiveX/modules/StormMps.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/SymantecAppStream.py` & `thug-6.4/thug/ActiveX/modules/SymantecAppStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/SymantecBackupExec.py` & `thug-6.4/thug/ActiveX/modules/SymantecBackupExec.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/TextStream.py` & `thug-6.4/thug/ActiveX/modules/TextStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/Toshiba.py` & `thug-6.4/thug/ActiveX/modules/Toshiba.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/VLC.py` & `thug-6.4/thug/ActiveX/modules/VLC.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/VisualStudioDTE80.py` & `thug-6.4/thug/ActiveX/modules/VisualStudioDTE80.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WMEncProfileManager.py` & `thug-6.4/thug/ActiveX/modules/WMEncProfileManager.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WScriptExec.py` & `thug-6.4/thug/ActiveX/modules/WScriptExec.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WScriptNetwork.py` & `thug-6.4/thug/ActiveX/modules/WScriptNetwork.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WScriptShell.py` & `thug-6.4/thug/ActiveX/modules/WScriptShell.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WebViewFolderIcon.py` & `thug-6.4/thug/ActiveX/modules/WebViewFolderIcon.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WinNTSystemInfo.py` & `thug-6.4/thug/ActiveX/modules/WinNTSystemInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/WinZip.py` & `thug-6.4/thug/ActiveX/modules/WinZip.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/XMLDOMParseError.py` & `thug-6.4/thug/ActiveX/modules/XMLDOMParseError.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/XUpload.py` & `thug-6.4/thug/ActiveX/modules/XUpload.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/YahooJukebox.py` & `thug-6.4/thug/ActiveX/modules/YahooJukebox.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/YahooMessengerYVerInfo.py` & `thug-6.4/thug/ActiveX/modules/YahooMessengerYVerInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/YahooMessengerYwcvwr.py` & `thug-6.4/thug/ActiveX/modules/YahooMessengerYwcvwr.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py` & `thug-6.4/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ActiveX/modules/__init__.py` & `thug-6.4/thug/ActiveX/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Analysis/awis/AWIS.py` & `thug-6.4/thug/Analysis/awis/AWIS.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Analysis/context/ContextAnalyzer.py` & `thug-6.4/thug/Analysis/context/ContextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Analysis/honeyagent/HoneyAgent.py` & `thug-6.4/thug/Analysis/honeyagent/HoneyAgent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Analysis/screenshot/Screenshot.py` & `thug-6.4/thug/Analysis/screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Analysis/shellcode/Shellcode.py` & `thug-6.4/thug/Analysis/shellcode/Shellcode.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/BaseClassifier.py` & `thug-6.4/thug/Classifier/BaseClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/CookieClassifier.py` & `thug-6.4/thug/Classifier/CookieClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/HTMLClassifier.py` & `thug-6.4/thug/Classifier/HTMLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/ImageClassifier.py` & `thug-6.4/thug/Classifier/ImageClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/JSClassifier.py` & `thug-6.4/thug/Classifier/JSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/SampleClassifier.py` & `thug-6.4/thug/Classifier/SampleClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/TextClassifier.py` & `thug-6.4/thug/Classifier/TextClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/URLClassifier.py` & `thug-6.4/thug/Classifier/URLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Classifier/VBSClassifier.py` & `thug-6.4/thug/Classifier/VBSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Alexa.py` & `thug-6.4/thug/DOM/Alexa.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/AsyncPrefetcher.py` & `thug-6.4/thug/DOM/AsyncPrefetcher.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/CCInterpreter.py` & `thug-6.4/thug/DOM/CCInterpreter.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Chrome.py` & `thug-6.4/thug/DOM/Chrome.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/ClipboardData.py` & `thug-6.4/thug/DOM/ClipboardData.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Components.py` & `thug-6.4/thug/DOM/Components.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Console.py` & `thug-6.4/thug/DOM/Console.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Crypto.py` & `thug-6.4/thug/DOM/Crypto.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/DFT.py` & `thug-6.4/thug/DOM/DFT.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/External.py` & `thug-6.4/thug/DOM/External.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/HTMLInspector.py` & `thug-6.4/thug/DOM/HTMLInspector.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/HTTPSession.py` & `thug-6.4/thug/DOM/HTTPSession.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/HTTPSessionException.py` & `thug-6.4/thug/DOM/HTTPSessionException.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/History.py` & `thug-6.4/thug/DOM/History.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/JSClass.py` & `thug-6.4/thug/DOM/JSClass.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/JSEngine.py` & `thug-6.4/thug/DOM/JSEngine.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/JSInspector.py` & `thug-6.4/thug/DOM/JSInspector.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/JScriptEncode.py` & `thug-6.4/thug/DOM/JScriptEncode.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/LocalStorage.py` & `thug-6.4/thug/DOM/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Location.py` & `thug-6.4/thug/DOM/Location.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/MIMEHandler.py` & `thug-6.4/thug/DOM/MIMEHandler.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Map.py` & `thug-6.4/thug/DOM/Map.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/MimeType.py` & `thug-6.4/thug/DOM/MimeType.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/MimeTypes.py` & `thug-6.4/thug/DOM/MimeTypes.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/MozConnection.py` & `thug-6.4/thug/DOM/MozConnection.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Navigator.py` & `thug-6.4/thug/DOM/Navigator.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Personality.py` & `thug-6.4/thug/DOM/Personality.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Plugin.py` & `thug-6.4/thug/DOM/Plugin.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Plugins.py` & `thug-6.4/thug/DOM/Plugins.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/SchemeHandler.py` & `thug-6.4/thug/DOM/SchemeHandler.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Screen.py` & `thug-6.4/thug/DOM/Screen.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/SessionStorage.py` & `thug-6.4/thug/DOM/SessionStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Sidebar.py` & `thug-6.4/thug/DOM/Sidebar.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Storage.py` & `thug-6.4/thug/DOM/Storage.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/UserProfile.py` & `thug-6.4/thug/DOM/UserProfile.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Utils.py` & `thug-6.4/thug/DOM/Utils.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/Attr.py` & `thug-6.4/thug/DOM/W3C/Core/Attr.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/CharacterData.py` & `thug-6.4/thug/DOM/W3C/Core/CharacterData.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/ClassList.py` & `thug-6.4/thug/DOM/W3C/Core/ClassList.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/Comment.py` & `thug-6.4/thug/DOM/W3C/Core/Comment.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/DOMException.py` & `thug-6.4/thug/DOM/W3C/Core/DOMException.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/DOMImplementation.py` & `thug-6.4/thug/DOM/W3C/Core/DOMImplementation.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/Document.py` & `thug-6.4/thug/DOM/W3C/Core/Document.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/DocumentFragment.py` & `thug-6.4/thug/DOM/W3C/Core/DocumentFragment.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/DocumentType.py` & `thug-6.4/thug/DOM/W3C/Core/DocumentType.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/Element.py` & `thug-6.4/thug/DOM/W3C/Core/Element.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/NamedNodeMap.py` & `thug-6.4/thug/DOM/W3C/Core/NamedNodeMap.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/Node.py` & `thug-6.4/thug/DOM/W3C/Core/Node.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/NodeList.py` & `thug-6.4/thug/DOM/W3C/Core/NodeList.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/Text.py` & `thug-6.4/thug/DOM/W3C/Core/Text.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Core/__init__.py` & `thug-6.4/thug/DOM/W3C/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/DOMTokenList.py` & `thug-6.4/thug/DOM/W3C/DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/DocumentEvent.py` & `thug-6.4/thug/DOM/W3C/Events/DocumentEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/Event.py` & `thug-6.4/thug/DOM/W3C/Events/Event.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/EventTarget.py` & `thug-6.4/thug/DOM/W3C/Events/EventTarget.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/MessageEvent.py` & `thug-6.4/thug/DOM/W3C/Events/MessageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/MouseEvent.py` & `thug-6.4/thug/DOM/W3C/Events/MouseEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/MutationEvent.py` & `thug-6.4/thug/DOM/W3C/Events/MutationEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/StorageEvent.py` & `thug-6.4/thug/DOM/W3C/Events/StorageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/UIEvent.py` & `thug-6.4/thug/DOM/W3C/Events/UIEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Events/__init__.py` & `thug-6.4/thug/DOM/W3C/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/File/Blob.py` & `thug-6.4/thug/DOM/W3C/File/Blob.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/File/File.py` & `thug-6.4/thug/DOM/W3C/File/File.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/Dataset.py` & `thug-6.4/thug/DOM/W3C/HTML/Dataset.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLAnchorElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLAnchorElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLAppletElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLAppletElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLBodyElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLBodyElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLButtonElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLButtonElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLCollection.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLCollection.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLDocument.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLFormElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLFormElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLFrameElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLIFrameElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLIFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLImageElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLImageElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLInputElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLInputElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLLinkElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLLinkElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLMediaElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLMediaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLMetaElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLMetaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLObjectElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLObjectElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLOptionElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLOptionElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLScriptElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLScriptElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLSelectElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLSelectElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLTableCellElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLTableCellElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLTableElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLTableElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLTableRowElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLTableRowElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLTableSectionElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLTableSectionElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLTextAreaElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLTextAreaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/HTMLVideoElement.py` & `thug-6.4/thug/DOM/W3C/HTML/HTMLVideoElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/TAnimateColor.py` & `thug-6.4/thug/DOM/W3C/HTML/TAnimateColor.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/TimeRanges.py` & `thug-6.4/thug/DOM/W3C/HTML/TimeRanges.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/__init__.py` & `thug-6.4/thug/DOM/W3C/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/HTML/text_property.py` & `thug-6.4/thug/DOM/W3C/HTML/text_property.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py` & `thug-6.4/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/URL/URL.py` & `thug-6.4/thug/DOM/W3C/URL/URL.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/W3C/URL/URLSearchParams.py` & `thug-6.4/thug/DOM/W3C/URL/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/WebStore.py` & `thug-6.4/thug/DOM/WebStore.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/Window.py` & `thug-6.4/thug/DOM/Window.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/DOM/w3c_bindings.py` & `thug-6.4/thug/DOM/w3c_bindings.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Encoding/Encoding.py` & `thug-6.4/thug/Encoding/Encoding.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Java/System.py` & `thug-6.4/thug/Java/System.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Java/java.py` & `thug-6.4/thug/Java/java.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Java/lang.py` & `thug-6.4/thug/Java/lang.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/BaseLogging.py` & `thug-6.4/thug/Logging/BaseLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/Features.py` & `thug-6.4/thug/Logging/Features.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/LoggingModules.py` & `thug-6.4/thug/Logging/LoggingModules.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/SampleLogging.py` & `thug-6.4/thug/Logging/SampleLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/ThugLogging.py` & `thug-6.4/thug/Logging/ThugLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/modules/ElasticSearch.py` & `thug-6.4/thug/Logging/modules/ElasticSearch.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/modules/ExploitGraph.py` & `thug-6.4/thug/Logging/modules/ExploitGraph.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/modules/JSON.py` & `thug-6.4/thug/Logging/modules/JSON.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/modules/Mapper.py` & `thug-6.4/thug/Logging/modules/Mapper.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Logging/modules/MongoDB.py` & `thug-6.4/thug/Logging/modules/MongoDB.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Magic/Magic.py` & `thug-6.4/thug/Magic/Magic.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/OS/Windows.py` & `thug-6.4/thug/OS/Windows.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Plugins/IPlugin.py` & `thug-6.4/thug/Plugins/IPlugin.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Plugins/ThugPlugins.py` & `thug-6.4/thug/Plugins/ThugPlugins.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py` & `thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py` & `thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ThugAPI/IThugAPI.py` & `thug-6.4/thug/ThugAPI/IThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ThugAPI/OpaqueFilter.py` & `thug-6.4/thug/ThugAPI/OpaqueFilter.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ThugAPI/ThugAPI.py` & `thug-6.4/thug/ThugAPI/ThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ThugAPI/ThugOpts.py` & `thug-6.4/thug/ThugAPI/ThugOpts.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ThugAPI/ThugVulnModules.py` & `thug-6.4/thug/ThugAPI/ThugVulnModules.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/ThugAPI/Watchdog.py` & `thug-6.4/thug/ThugAPI/Watchdog.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/WebTracking/Cookies.py` & `thug-6.4/thug/WebTracking/Cookies.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/WebTracking/WebStorage.py` & `thug-6.4/thug/WebTracking/WebStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/WebTracking/WebTracking.py` & `thug-6.4/thug/WebTracking/WebTracking.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/__init__.py` & `thug-6.4/thug/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import importlib.resources
 
 import appdirs
 
-__version__ = "6.3"
+__version__ = "6.4"
 __jsengine__ = ""
 __jsengine_version__ = ""
 
 __global_configuration_path__ = "/etc/thug"
 __user_configuration_path__ = f"{appdirs.user_config_dir()}/thug"
 __package_configuration_path__ = os.path.join(importlib.resources.files("thug"), "conf")
 __configuration_path__ = __package_configuration_path__
```

### Comparing `thug-6.3/thug/conf/personalities/galaxy2chrome18.json` & `thug-6.4/thug/conf/personalities/galaxy2chrome18.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/galaxy2chrome25.json` & `thug-6.4/thug/conf/personalities/galaxy2chrome25.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/galaxy2chrome29.json` & `thug-6.4/thug/conf/personalities/galaxy2chrome29.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome33.json` & `thug-6.4/thug/conf/personalities/ipadchrome33.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome35.json` & `thug-6.4/thug/conf/personalities/ipadchrome35.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome37.json` & `thug-6.4/thug/conf/personalities/ipadchrome37.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome38.json` & `thug-6.4/thug/conf/personalities/ipadchrome38.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome39.json` & `thug-6.4/thug/conf/personalities/ipadchrome39.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome45.json` & `thug-6.4/thug/conf/personalities/ipadchrome45.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome46.json` & `thug-6.4/thug/conf/personalities/ipadchrome46.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadchrome47.json` & `thug-6.4/thug/conf/personalities/ipadchrome47.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadsafari7.json` & `thug-6.4/thug/conf/personalities/ipadsafari7.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadsafari8.json` & `thug-6.4/thug/conf/personalities/ipadsafari8.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/ipadsafari9.json` & `thug-6.4/thug/conf/personalities/ipadsafari9.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxchrome26.json` & `thug-6.4/thug/conf/personalities/linuxchrome26.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxchrome30.json` & `thug-6.4/thug/conf/personalities/linuxchrome30.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxchrome44.json` & `thug-6.4/thug/conf/personalities/linuxchrome44.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxchrome54.json` & `thug-6.4/thug/conf/personalities/linuxchrome54.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxchrome98.json` & `thug-6.4/thug/conf/personalities/linuxchrome98.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxfirefox19.json` & `thug-6.4/thug/conf/personalities/linuxfirefox19.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/linuxfirefox40.json` & `thug-6.4/thug/conf/personalities/linuxfirefox40.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/nexuschrome18.json` & `thug-6.4/thug/conf/personalities/nexuschrome18.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/osx10chrome19.json` & `thug-6.4/thug/conf/personalities/osx10chrome19.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/osx10chrome80.json` & `thug-6.4/thug/conf/personalities/osx10chrome80.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/osx10chrome97.json` & `thug-6.4/thug/conf/personalities/osx10chrome97.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/osx10safari5.json` & `thug-6.4/thug/conf/personalities/osx10safari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/osx11safari14.json` & `thug-6.4/thug/conf/personalities/osx11safari14.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win10edge20.json.review` & `thug-6.4/thug/conf/personalities/win10edge20.json.review`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win10ie110.json` & `thug-6.4/thug/conf/personalities/win10ie110.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win2kie60.json` & `thug-6.4/thug/conf/personalities/win2kie60.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win2kie80.json` & `thug-6.4/thug/conf/personalities/win2kie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7chrome20.json` & `thug-6.4/thug/conf/personalities/win7chrome20.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7chrome40.json` & `thug-6.4/thug/conf/personalities/win7chrome40.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7chrome45.json` & `thug-6.4/thug/conf/personalities/win7chrome45.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7chrome49.json` & `thug-6.4/thug/conf/personalities/win7chrome49.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7firefox3.json` & `thug-6.4/thug/conf/personalities/win7firefox3.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7ie100.json` & `thug-6.4/thug/conf/personalities/win7ie100.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7ie80.json` & `thug-6.4/thug/conf/personalities/win7ie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7ie90.json` & `thug-6.4/thug/conf/personalities/win7ie90.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/win7safari5.json` & `thug-6.4/thug/conf/personalities/win7safari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpchrome20.json` & `thug-6.4/thug/conf/personalities/winxpchrome20.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpfirefox12.json` & `thug-6.4/thug/conf/personalities/winxpfirefox12.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpie60.json` & `thug-6.4/thug/conf/personalities/winxpie60.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpie61.json` & `thug-6.4/thug/conf/personalities/winxpie61.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpie70.json` & `thug-6.4/thug/conf/personalities/winxpie70.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpie80.json` & `thug-6.4/thug/conf/personalities/winxpie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/personalities/winxpsafari5.json` & `thug-6.4/thug/conf/personalities/winxpsafari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/blackhole.yar` & `thug-6.4/thug/conf/rules/urlclassifier/blackhole.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/crimeboss.yar` & `thug-6.4/thug/conf/rules/urlclassifier/crimeboss.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/critxpack.yar` & `thug-6.4/thug/conf/rules/urlclassifier/critxpack.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/fiesta.yar` & `thug-6.4/thug/conf/rules/urlclassifier/fiesta.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/g01pack.yar` & `thug-6.4/thug/conf/rules/urlclassifier/g01pack.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/neutrino.yar` & `thug-6.4/thug/conf/rules/urlclassifier/neutrino.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/nuclear.yar` & `thug-6.4/thug/conf/rules/urlclassifier/nuclear.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/popads.yar` & `thug-6.4/thug/conf/rules/urlclassifier/popads.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/redkit.yar` & `thug-6.4/thug/conf/rules/urlclassifier/redkit.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/styx.yar` & `thug-6.4/thug/conf/rules/urlclassifier/styx.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/rules/urlclassifier/sweetorange.yar` & `thug-6.4/thug/conf/rules/urlclassifier/sweetorange.yar`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/scripts/atob.js` & `thug-6.4/thug/conf/scripts/atob.js`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/scripts/btoa.js` & `thug-6.4/thug/conf/scripts/btoa.js`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/conf/scripts/thug.js` & `thug-6.4/thug/conf/scripts/thug.js`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug/thug.py` & `thug-6.4/thug/thug.py`

 * *Files identical despite different names*

### Comparing `thug-6.3/thug.egg-info/PKG-INFO` & `thug-6.4/thug.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 6.3
+Version: 6.4
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
@@ -26,32 +26,32 @@
 Classifier: Topic :: Security
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: cssutils==2.9.0
+Requires-Dist: cssutils==2.10.2
 Requires-Dist: dhash==1.4
 Requires-Dist: html5lib==1.1
-Requires-Dist: lxml==5.1.0
+Requires-Dist: lxml==5.2.1
 Requires-Dist: networkx==3.2.1
 Requires-Dist: pefile==2023.2.7
-Requires-Dist: pillow==10.2.0
+Requires-Dist: pillow==10.3.0
 Requires-Dist: promise==2.3
 Requires-Dist: pylibemu==1.0
-Requires-Dist: pymongo==4.6.2
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: pysocks==1.7.1
 Requires-Dist: python-magic==0.4.27
-Requires-Dist: rarfile==4.1
+Requires-Dist: rarfile==4.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-futures==1.0.1
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: ssdeep==3.4
-Requires-Dist: stpyv8==12.2.281.19
+Requires-Dist: stpyv8==12.3.219.16
 Requires-Dist: yara-python==4.5.0
 Requires-Dist: zope.interface==6.2
 Requires-Dist: importlib-resources==6.0.1; python_version < "3.9"
 Provides-Extra: elasticsearch
 Requires-Dist: elasticsearch; extra == "elasticsearch"
 Provides-Extra: exploitgraph
 Requires-Dist: pygraphviz; extra == "exploitgraph"
```

### Comparing `thug-6.3/thug.egg-info/SOURCES.txt` & `thug-6.4/thug.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -454,15 +454,8 @@
 thug/conf/scripts/atob.js
 thug/conf/scripts/btoa.js
 thug/conf/scripts/date.js
 thug/conf/scripts/eval.js
 thug/conf/scripts/message-event.js
 thug/conf/scripts/storage.js
 thug/conf/scripts/thug.js
-thug/conf/scripts/write.js
-thug/thug.egg-info/PKG-INFO
-thug/thug.egg-info/SOURCES.txt
-thug/thug.egg-info/dependency_links.txt
-thug/thug.egg-info/entry_points.txt
-thug/thug.egg-info/requires.txt
-thug/thug.egg-info/top_level.txt
-thug/thug.egg-info/zip-safe
+thug/conf/scripts/write.js
```

### Comparing `thug-6.3/thug.egg-info/requires.txt` & `thug-6.4/thug.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 appdirs==1.4.4
 beautifulsoup4==4.12.3
 charset-normalizer==3.3.2
-cssutils==2.9.0
+cssutils==2.10.2
 dhash==1.4
 html5lib==1.1
-lxml==5.1.0
+lxml==5.2.1
 networkx==3.2.1
 pefile==2023.2.7
-pillow==10.2.0
+pillow==10.3.0
 promise==2.3
 pylibemu==1.0
-pymongo==4.6.2
+pymongo==4.6.3
 pysocks==1.7.1
 python-magic==0.4.27
-rarfile==4.1
+rarfile==4.2
 requests==2.31.0
 requests-futures==1.0.1
 setuptools>=65.5.1
 ssdeep==3.4
-stpyv8==12.2.281.19
+stpyv8==12.3.219.16
 yara-python==4.5.0
 zope.interface==6.2
 
 [:python_version < "3.9"]
 importlib-resources==6.0.1
 
 [elasticsearch]
```

