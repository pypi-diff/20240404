# Comparing `tmp/plex-api-client-0.5.0.tar.gz` & `tmp/plex-api-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.5.0.tar", last modified: Wed Apr  3 01:14:00 2024, max compression
+gzip compressed data, was "plex-api-client-0.6.0.tar", last modified: Thu Apr  4 01:15:06 2024, max compression
```

## Comparing `plex-api-client-0.5.0.tar` & `plex-api-client-0.6.0.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    17401 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14179 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.773893 plex-api-client-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.773893 plex-api-client-0.5.0/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.777893 plex-api-client-0.5.0/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    17617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41590 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.777893 plex-api-client-0.5.0/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.777893 plex-api-client-0.5.0/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.785893 plex-api-client-0.5.0/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryitems.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33733 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17401 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.065644 plex-api-client-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17432 2024-04-04 01:15:06.065644 plex-api-client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:15:06.065644 plex-api-client-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.041644 plex-api-client-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.045644 plex-api-client-0.6.0/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.045644 plex-api-client-0.6.0/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42832 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.045644 plex-api-client-0.6.0/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.045644 plex-api-client-0.6.0/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.053644 plex-api-client-0.6.0/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.065644 plex-api-client-0.6.0/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34761 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28065 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.065644 plex-api-client-0.6.0/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-04 01:14:56.000000 plex-api-client-0.6.0/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:15:06.065644 plex-api-client-0.6.0/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17432 2024-04-04 01:15:05.000000 plex-api-client-0.6.0/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-04 01:15:05.000000 plex-api-client-0.6.0/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:15:05.000000 plex-api-client-0.6.0/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 01:15:05.000000 plex-api-client-0.6.0/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 01:15:05.000000 plex-api-client-0.6.0/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.5.0/LICENSE.md` & `plex-api-client-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/PKG-INFO` & `plex-api-client-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
+Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
             <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
             <a href="https://opensource.org/licenses/MIT">
@@ -158,15 +158,15 @@
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object                             | Status Code                              | Content Type                             |
         | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
         | errors.GetServerCapabilitiesResponseBody | 401                                      | application/json                         |
-        | errors.SDKError                          | 4x-5xx                                   | */*                                      |
+        | errors.SDKError                          | 4xx-5xx                                  | */*                                      |
         
         ### Example
         
         ```python
         import plex_api
         from plex_api.models import errors
         
@@ -280,15 +280,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import plex_api
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = plex_api.PlexAPI(client: http_client)
+        s = plex_api.PlexAPI(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         <!-- Start Authentication [security] -->
         ## Authentication
         
         ### Per-Client Security Schemes
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.5.0 Summary: Python
-Client SDK Generated by Speakeasy Home-page: UNKNOWN Author: LukeHagar License:
-UNKNOWN Description: # plexpy
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.0 Summary: Python
+Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
+plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
 ( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
@@ -96,15 +96,15 @@
 Error Handling Handling errors in this SDK should largely match your
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
-errors.SDKError | 4x-5xx | */* | ### Example ```python import plex_api from
+errors.SDKError | 4xx-5xx | */* | ### Example ```python import plex_api from
 plex_api.models import errors s = plex_api.PlexAPI( access_token="",
 x_plex_client_identifier='', ) res = None try: res =
 s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
@@ -134,15 +134,15 @@
 ``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
 (https://pypi.org/project/requests/) HTTP library. In order to provide a
 convenient way to configure timeouts, cookies, proxies, custom headers, and
 other low-level configuration, you can initialize the SDK client with a custom
 `requests.Session` object. For example, you could specify a header for every
 request that this sdk makes as follows: ```python import plex_api import
 requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = plex_api.PlexAPI(client: http_client) ``` ##
+custom-header': 'someValue'}) s = plex_api.PlexAPI(client=http_client) ``` ##
 Authentication ### Per-Client Security Schemes This SDK supports the following
 security scheme globally: | Name | Type | Scheme | | -------------- | ---------
 ----- | -------------- | | `access_token` | apiKey | API key | To authenticate
 with the API the `access_token` parameter must be set when initializing the SDK
 client instance. For example: ```python import plex_api s = plex_api.PlexAPI
 ( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
```

### Comparing `plex-api-client-0.5.0/README.md` & `plex-api-client-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object                             | Status Code                              | Content Type                             |
 | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
 | errors.GetServerCapabilitiesResponseBody | 401                                      | application/json                         |
-| errors.SDKError                          | 4x-5xx                                   | */*                                      |
+| errors.SDKError                          | 4xx-5xx                                  | */*                                      |
 
 ### Example
 
 ```python
 import plex_api
 from plex_api.models import errors
 
@@ -273,15 +273,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import plex_api
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = plex_api.PlexAPI(client: http_client)
+s = plex_api.PlexAPI(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 <!-- Start Authentication [security] -->
 ## Authentication
 
 ### Per-Client Security Schemes
```

#### html2text {}

```diff
@@ -94,15 +94,15 @@
 Error Handling Handling errors in this SDK should largely match your
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
-errors.SDKError | 4x-5xx | */* | ### Example ```python import plex_api from
+errors.SDKError | 4xx-5xx | */* | ### Example ```python import plex_api from
 plex_api.models import errors s = plex_api.PlexAPI( access_token="",
 x_plex_client_identifier='', ) res = None try: res =
 s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
@@ -132,15 +132,15 @@
 ``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
 (https://pypi.org/project/requests/) HTTP library. In order to provide a
 convenient way to configure timeouts, cookies, proxies, custom headers, and
 other low-level configuration, you can initialize the SDK client with a custom
 `requests.Session` object. For example, you could specify a header for every
 request that this sdk makes as follows: ```python import plex_api import
 requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = plex_api.PlexAPI(client: http_client) ``` ##
+custom-header': 'someValue'}) s = plex_api.PlexAPI(client=http_client) ``` ##
 Authentication ### Per-Client Security Schemes This SDK supports the following
 security scheme globally: | Name | Type | Scheme | | -------------- | ---------
 ----- | -------------- | | `access_token` | apiKey | API key | To authenticate
 with the API the `access_token` parameter must be set when initializing the SDK
 client instance. For example: ```python import plex_api s = plex_api.PlexAPI
 ( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
```

### Comparing `plex-api-client-0.5.0/setup.py` & `plex-api-client-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="plex-api-client",
-    version="0.5.0",
+    version="0.6.0",
     author="LukeHagar",
     description="Python Client SDK Generated by Speakeasy",
+    url="https://github.com/LukeHagar/plexpy.git",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4",
```

### Comparing `plex-api-client-0.5.0/src/plex_api/_hooks/registration.py` & `plex-api-client-0.6.0/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.6.0/src/plex_api/_hooks/sdkhooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
 from .registration import init_hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -27,27 +27,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `plex-api-client-0.5.0/src/plex_api/_hooks/types.py` & `plex-api-client-0.6.0/src/plex_api/_hooks/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
```

### Comparing `plex-api-client-0.5.0/src/plex_api/activities.py` & `plex-api-client-0.6.0/src/plex_api/activities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Activities:
     r"""Activities are awesome. They provide a way to monitor and control asynchronous operations on the server. In order to receive real-time updates for activities, a client would normally subscribe via either EventSource or Websocket endpoints.
     Activities are associated with HTTP replies via a special `X-Plex-Activity` header which contains the UUID of the activity.
     Activities are optional cancellable. If cancellable, they may be cancelled via the `DELETE` endpoint. Other details:
@@ -38,47 +38,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetServerActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetServerActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerActivitiesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerActivitiesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -107,42 +106,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CancelServerActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CancelServerActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.CancelServerActivitiesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/authentication.py` & `plex-api-client-0.6.0/src/plex_api/video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,144 +1,132 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 
-class Authentication:
-    r"""API Calls regarding authentication for Plex Media Server"""
+class Video:
+    r"""API Calls that perform operations with Plex Media Server Videos"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get_transient_token(self, type_: operations.GetTransientTokenQueryParamType, scope: operations.Scope) -> operations.GetTransientTokenResponse:
-        r"""Get a Transient Token.
-        This endpoint provides the caller with a temporary token with the same access level as the caller's token. These tokens are valid for up to 48 hours and are destroyed if the server instance is restarted.
+    def get_timeline(self, request: operations.GetTimelineRequest) -> operations.GetTimelineResponse:
+        r"""Get the timeline for a media item
+        Get the timeline for a media item
         """
-        hook_ctx = HookContext(operation_id='getTransientToken', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetTransientTokenRequest(
-            type=type_,
-            scope=scope,
-        )
-        
+        hook_ctx = HookContext(operation_id='getTimeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/security/token'
+        url = base_url + '/:/timeline'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTransientTokenRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(operations.GetTimelineRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetTransientTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetTimelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.GetTransientTokenResponseBody)
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.GetTimelineResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_source_connection_information(self, source: str) -> operations.GetSourceConnectionInformationResponse:
-        r"""Get Source Connection Information
-        If a caller requires connection details and a transient token for a source that is known to the server, for example a cloud media provider or shared PMS, then this endpoint can be called. This endpoint is only accessible with either an admin token or a valid transient token generated from an admin token.
-        Note: requires Plex Media Server >= 1.15.4.
+    def start_universal_transcode(self, request: operations.StartUniversalTranscodeRequest) -> operations.StartUniversalTranscodeResponse:
+        r"""Start Universal Transcode
+        Begin a Universal Transcode Session
         """
-        hook_ctx = HookContext(operation_id='getSourceConnectionInformation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetSourceConnectionInformationRequest(
-            source=source,
-        )
-        
+        hook_ctx = HookContext(operation_id='startUniversalTranscode', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/security/resources'
+        url = base_url + '/video/:/transcode/universal/start.mpd'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetSourceConnectionInformationRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(operations.StartUniversalTranscodeRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetSourceConnectionInformationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.StartUniversalTranscodeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.GetSourceConnectionInformationResponseBody)
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.StartUniversalTranscodeResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.5.0/src/plex_api/butler.py` & `plex-api-client-0.6.0/src/plex_api/butler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Butler:
     r"""Butler is the task manager of the Plex Media Server Ecosystem."""
     sdk_configuration: SDKConfiguration
 
@@ -31,47 +31,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetButlerTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetButlerTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetButlerTasksResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetButlerTasksResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -100,42 +99,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.StartAllTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.StartAllTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StartAllTasksResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -160,42 +158,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.StopAllTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.StopAllTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StopAllTasksResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -228,42 +225,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.StartTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.StartTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code in [200, 202]:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StartTaskResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -292,42 +288,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','404','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.StopTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.StopTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code == 404 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StopTaskResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/hubs.py` & `plex-api-client-0.6.0/src/plex_api/hubs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Hubs:
     r"""Hubs are a structured two-dimensional container for media, generally represented by multiple horizontal rows."""
     sdk_configuration: SDKConfiguration
 
@@ -37,47 +37,46 @@
         
         query_params = { **utils.get_query_params(operations.GetGlobalHubsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetGlobalHubsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetGlobalHubsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetGlobalHubsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetGlobalHubsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -109,47 +108,46 @@
         
         query_params = { **utils.get_query_params(operations.GetLibraryHubsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetLibraryHubsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetLibraryHubsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryHubsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetLibraryHubsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/library.py` & `plex-api-client-0.6.0/src/plex_api/library.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Library:
     r"""API Calls interacting with Plex Media Server Libraries"""
     sdk_configuration: SDKConfiguration
 
@@ -37,42 +37,41 @@
         
         query_params = { **utils.get_query_params(operations.GetFileHashRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetFileHashResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetFileHashResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetFileHashResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -97,47 +96,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetRecentlyAddedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetRecentlyAddedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetRecentlyAddedResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetRecentlyAddedResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -167,47 +165,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetLibrariesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetLibrariesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibrariesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetLibrariesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -276,47 +273,46 @@
         
         query_params = { **utils.get_query_params(operations.GetLibraryRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetLibraryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -345,42 +341,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeleteLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.DeleteLibraryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -429,38 +424,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetLibraryItemsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetLibraryItemsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryItemsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -490,42 +484,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.RefreshLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.RefreshLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.RefreshLibraryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -573,38 +566,37 @@
         
         query_params = { **utils.get_query_params(operations.SearchLibraryRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.SearchLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.SearchLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchLibraryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -634,47 +626,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetMetadataResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetMetadataResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -703,47 +694,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetMetadataChildrenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetMetadataChildrenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetMetadataChildrenResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetMetadataChildrenResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -768,47 +758,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetOnDeckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetOnDeckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOnDeckResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetOnDeckResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/log.py` & `plex-api-client-0.6.0/src/plex_api/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 
 class Log:
     r"""Submit logs to the Log Handler for Plex Media Server"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -37,42 +37,41 @@
         
         query_params = { **utils.get_query_params(operations.LogLineRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.LogLineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.LogLineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.LogLineResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -122,42 +121,41 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.LogMultiLineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.LogMultiLineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.LogMultiLineResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -182,42 +180,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.EnablePaperTrailResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.EnablePaperTrailResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code == 403 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.EnablePaperTrailResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/media.py` & `plex-api-client-0.6.0/src/plex_api/media.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 
 class Media:
     r"""API Calls interacting with Plex Media Server Media"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -35,42 +35,41 @@
         
         query_params = { **utils.get_query_params(operations.MarkPlayedRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.MarkPlayedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.MarkPlayedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.MarkPlayedResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -100,42 +99,41 @@
         
         query_params = { **utils.get_query_params(operations.MarkUnplayedRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.MarkUnplayedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.MarkUnplayedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.MarkUnplayedResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -167,42 +165,41 @@
         
         query_params = { **utils.get_query_params(operations.UpdatePlayProgressRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UpdatePlayProgressResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UpdatePlayProgressResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UpdatePlayProgressResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/logline.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryitems.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getlibraryitems.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/logline.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/searchlibrary.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/searchlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.6.0/src/plex_api/models/operations/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api/playlists.py` & `plex-api-client-0.6.0/src/plex_api/playlists.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Playlists:
     r"""Playlists are ordered collections of media. They can be dumb (just a list of media) or smart (based on a media query, such as \\"all albums from 2017\\").
     They can be organized in (optionally nesting) folders.
     Retrieving a playlist, or its items, will trigger a refresh of its metadata. 
@@ -38,47 +38,46 @@
         
         query_params = { **utils.get_query_params(operations.CreatePlaylistRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreatePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreatePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreatePlaylistResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.CreatePlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -109,47 +108,46 @@
         
         query_params = { **utils.get_query_params(operations.GetPlaylistsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetPlaylistsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetPlaylistsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlaylistsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPlaylistsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -179,47 +177,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetPlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetPlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlaylistResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -248,42 +245,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeletePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeletePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.DeletePlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -315,42 +311,41 @@
         
         query_params = { **utils.get_query_params(operations.UpdatePlaylistRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UpdatePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UpdatePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UpdatePlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -384,47 +379,46 @@
         
         query_params = { **utils.get_query_params(operations.GetPlaylistContentsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlaylistContentsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPlaylistContentsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -453,42 +447,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.ClearPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ClearPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ClearPlaylistContentsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -521,47 +514,46 @@
         
         query_params = { **utils.get_query_params(operations.AddPlaylistContentsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.AddPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.AddPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.AddPlaylistContentsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.AddPlaylistContentsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -592,42 +584,41 @@
         
         query_params = { **utils.get_query_params(operations.UploadPlaylistRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UploadPlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UploadPlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UploadPlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/plex.py` & `plex-api-client-0.6.0/src/plex_api/plex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Plex:
     r"""API Calls that perform operations directly against https://Plex.tv"""
     sdk_configuration: SDKConfiguration
 
@@ -39,45 +39,44 @@
         headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         query_params = { **utils.get_query_params(operations.GetPinRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetPinResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetPinResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPinResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPinResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,40 +109,39 @@
         
         headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetTokenResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/sdk.py` & `plex-api-client-0.6.0/src/plex_api/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .plex import Plex
 from .sdkconfiguration import SDKConfiguration, ServerProtocol
 from .search import Search
 from .server import Server
 from .sessions import Sessions
 from .statistics import Statistics
 from .updater import Updater
+from .utils.retries import RetryConfig
 from .video import Video
 from plex_api import utils
 from plex_api._hooks import SDKHooks
 from plex_api.models import components
 from typing import Callable, Dict, Optional, Union
 
 class PlexAPI:
@@ -78,15 +79,15 @@
                  protocol: ServerProtocol = None,
                  ip: str = None,
                  port: str = None,
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param access_token: The access_token required for authentication
         :type access_token: Union[str, Callable[[], str]]
         :param x_plex_client_identifier: Configures the x_plex_client_identifier parameter for all supported operations
         :type x_plex_client_identifier: str
@@ -101,15 +102,15 @@
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(access_token):
             def security():
                 return components.Security(access_token = access_token())
```

### Comparing `plex-api-client-0.5.0/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.6.0/src/plex_api/sdkconfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass, field
 from enum import Enum
 from plex_api.models import components
-from typing import Any, Callable, Dict, List, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 
 SERVERS = [
     '{protocol}://{ip}:{port}',
     # The full address of your Plex Server
 ]
 """Contains the list of servers available to the SDK"""
@@ -23,28 +23,28 @@
     HTTPS = 'https'
 
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
     globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.5.0'
-    gen_version: str = '2.292.0'
-    user_agent: str = 'speakeasy-sdk/python 0.5.0 2.292.0 0.0.3 plex-api-client'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '0.6.0'
+    gen_version: str = '2.298.0'
+    user_agent: str = 'speakeasy-sdk/python 0.6.0 2.298.0 0.0.3 plex-api-client'
+    retry_config: Optional[RetryConfig] = None
+    _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], self.server_defaults[self.server_idx]
```

### Comparing `plex-api-client-0.5.0/src/plex_api/search.py` & `plex-api-client-0.6.0/src/plex_api/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Search:
     r"""API Calls that perform search operations with Plex Media Server"""
     sdk_configuration: SDKConfiguration
 
@@ -49,42 +49,41 @@
         
         query_params = { **utils.get_query_params(operations.PerformSearchRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.PerformSearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.PerformSearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.PerformSearchResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -119,42 +118,41 @@
         
         query_params = { **utils.get_query_params(operations.PerformVoiceSearchRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.PerformVoiceSearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.PerformVoiceSearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.PerformVoiceSearchResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -184,47 +182,46 @@
         
         query_params = { **utils.get_query_params(operations.GetSearchResultsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetSearchResultsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetSearchResultsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetSearchResultsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSearchResultsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/server.py` & `plex-api-client-0.6.0/src/plex_api/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Server:
     r"""Operations against the Plex Media Server System."""
     sdk_configuration: SDKConfiguration
 
@@ -31,47 +31,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetServerCapabilitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetServerCapabilitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerCapabilitiesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerCapabilitiesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -96,47 +95,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetServerPreferencesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetServerPreferencesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerPreferencesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerPreferencesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -161,47 +159,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetAvailableClientsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetAvailableClientsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAvailableClientsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetAvailableClientsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -226,47 +223,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetDevicesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetDevicesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDevicesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetDevicesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -291,47 +287,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetServerIdentityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetServerIdentityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerIdentityResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerIdentityResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -356,47 +351,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetMyPlexAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetMyPlexAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetMyPlexAccountResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetMyPlexAccountResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -422,42 +416,41 @@
         
         query_params = { **utils.get_query_params(operations.GetResizedPhotoRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetResizedPhotoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetResizedPhotoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetResizedPhotoResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -482,47 +475,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetServerListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetServerListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerListResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerListResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/sessions.py` & `plex-api-client-0.6.0/src/plex_api/sessions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Sessions:
     r"""API Calls that perform search operations with Plex Media Server Sessions"""
     sdk_configuration: SDKConfiguration
 
@@ -31,47 +31,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetSessionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetSessionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetSessionsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSessionsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -96,47 +95,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetSessionHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetSessionHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetSessionHistoryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSessionHistoryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -161,47 +159,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetTranscodeSessionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetTranscodeSessionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetTranscodeSessionsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetTranscodeSessionsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -230,42 +227,41 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.StopTranscodeSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.StopTranscodeSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StopTranscodeSessionResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/statistics.py` & `plex-api-client-0.6.0/src/plex_api/statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Statistics:
     r"""API Calls that perform operations with Plex Media Server Statistics"""
     sdk_configuration: SDKConfiguration
 
@@ -36,47 +36,46 @@
         
         query_params = { **utils.get_query_params(operations.GetStatisticsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetStatisticsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetStatisticsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetStatisticsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetStatisticsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/updater.py` & `plex-api-client-0.6.0/src/plex_api/updater.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from plex_api import utils
-from plex_api._hooks import HookContext
+from plex_api._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from plex_api.models import errors, operations
 from typing import Optional
 
 class Updater:
     r"""This describes the API for searching and applying updates to the Plex Media Server.
     Updates to the status can be observed via the Event API.
     """
@@ -33,47 +33,46 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetUpdateStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetUpdateStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetUpdateStatusResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetUpdateStatusResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -103,42 +102,41 @@
         
         query_params = { **utils.get_query_params(operations.CheckForUpdatesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CheckForUpdatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CheckForUpdatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.CheckForUpdatesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -169,42 +167,41 @@
         
         query_params = { **utils.get_query_params(operations.ApplyUpdatesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.ApplyUpdatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ApplyUpdatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code == 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ApplyUpdatesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `plex-api-client-0.5.0/src/plex_api/utils/retries.py` & `plex-api-client-0.6.0/src/plex_api/utils/retries.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
```

### Comparing `plex-api-client-0.5.0/src/plex_api/utils/utils.py` & `plex-api-client-0.6.0/src/plex_api/utils/utils.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.5.0/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.6.0/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
+Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
             <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
             <a href="https://opensource.org/licenses/MIT">
@@ -158,15 +158,15 @@
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object                             | Status Code                              | Content Type                             |
         | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
         | errors.GetServerCapabilitiesResponseBody | 401                                      | application/json                         |
-        | errors.SDKError                          | 4x-5xx                                   | */*                                      |
+        | errors.SDKError                          | 4xx-5xx                                  | */*                                      |
         
         ### Example
         
         ```python
         import plex_api
         from plex_api.models import errors
         
@@ -280,15 +280,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import plex_api
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = plex_api.PlexAPI(client: http_client)
+        s = plex_api.PlexAPI(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         <!-- Start Authentication [security] -->
         ## Authentication
         
         ### Per-Client Security Schemes
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.5.0 Summary: Python
-Client SDK Generated by Speakeasy Home-page: UNKNOWN Author: LukeHagar License:
-UNKNOWN Description: # plexpy
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.0 Summary: Python
+Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
+plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
 ( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
@@ -96,15 +96,15 @@
 Error Handling Handling errors in this SDK should largely match your
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
-errors.SDKError | 4x-5xx | */* | ### Example ```python import plex_api from
+errors.SDKError | 4xx-5xx | */* | ### Example ```python import plex_api from
 plex_api.models import errors s = plex_api.PlexAPI( access_token="",
 x_plex_client_identifier='', ) res = None try: res =
 s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
@@ -134,15 +134,15 @@
 ``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
 (https://pypi.org/project/requests/) HTTP library. In order to provide a
 convenient way to configure timeouts, cookies, proxies, custom headers, and
 other low-level configuration, you can initialize the SDK client with a custom
 `requests.Session` object. For example, you could specify a header for every
 request that this sdk makes as follows: ```python import plex_api import
 requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = plex_api.PlexAPI(client: http_client) ``` ##
+custom-header': 'someValue'}) s = plex_api.PlexAPI(client=http_client) ``` ##
 Authentication ### Per-Client Security Schemes This SDK supports the following
 security scheme globally: | Name | Type | Scheme | | -------------- | ---------
 ----- | -------------- | | `access_token` | apiKey | API key | To authenticate
 with the API the `access_token` parameter must be set when initializing the SDK
 client instance. For example: ```python import plex_api s = plex_api.PlexAPI
 ( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
```

### Comparing `plex-api-client-0.5.0/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.6.0/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

