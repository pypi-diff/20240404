# Comparing `tmp/itkdb_gtk-0.0.9.tar.gz` & `tmp/itkdb_gtk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.9.tar", last modified: Tue May 30 07:07:48 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.9.0.tar", last modified: Thu Apr  4 08:12:35 2024, max compression
```

## Comparing `itkdb_gtk-0.0.9.tar` & `itkdb_gtk-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-30 07:07:48.484977 itkdb_gtk-0.0.9/
--rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-30 07:07:48.484562 itkdb_gtk-0.0.9/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     2187 2023-05-24 15:05:26.000000 itkdb_gtk-0.0.9/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-30 07:07:48.480496 itkdb_gtk-0.0.9/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.9/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDB.desktop
--rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDB.svg
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-05-30 06:57:54.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14824 2023-05-25 13:27:59.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4693 2023-05-24 15:19:53.000000 itkdb_gtk-0.0.9/itkdb_gtk/ShowAttachments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2989 2023-05-24 13:13:04.000000 itkdb_gtk-0.0.9/itkdb_gtk/ShowComments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3329 2023-05-24 13:24:38.000000 itkdb_gtk-0.0.9/itkdb_gtk/ShowDefects.py
--rw-r--r--   0 lacasta    (503) staff       (20)      691 2023-05-30 07:07:43.000000 itkdb_gtk-0.0.9/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3731 2023-05-24 13:12:38.000000 itkdb_gtk-0.0.9/itkdb_gtk/checkComponent.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.9/itkdb_gtk/checkJSon.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4412 2023-05-25 15:33:11.000000 itkdb_gtk-0.0.9/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20713 2023-05-24 14:24:41.000000 itkdb_gtk-0.0.9/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.9/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7142 2023-05-24 13:24:49.000000 itkdb_gtk-0.0.9/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19379 2023-05-30 07:01:45.000000 itkdb_gtk-0.0.9/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.9/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.9/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    19648 2023-05-26 18:33:54.000000 itkdb_gtk-0.0.9/itkdb_gtk/uploadMultipleTests.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    22252 2023-05-24 13:37:58.000000 itkdb_gtk-0.0.9/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    12154 2023-05-24 16:04:02.000000 itkdb_gtk-0.0.9/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-30 07:07:48.484099 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      767 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      291 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       56 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)     1130 2023-05-30 07:06:48.000000 itkdb_gtk-0.0.9/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-30 07:07:48.485070 itkdb_gtk-0.0.9/setup.cfg
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.518084 itkdb_gtk-0.9.0/
+-rw-r--r--   0 lacasta    (501) staff       (20)     3148 2024-04-04 08:12:35.517901 itkdb_gtk-0.9.0/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)     2443 2024-04-01 19:21:18.000000 itkdb_gtk-0.9.0/README.md
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.516713 itkdb_gtk-0.9.0/itkdb_gtk/
+-rw-r--r--   0 lacasta    (501) staff       (20)    13159 2024-04-03 15:10:25.000000 itkdb_gtk-0.9.0/itkdb_gtk/CreateShipments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    18739 2024-04-03 15:10:34.000000 itkdb_gtk-0.9.0/itkdb_gtk/GetShipments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    12247 2024-04-03 15:13:45.000000 itkdb_gtk-0.9.0/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     9214 2024-04-03 15:11:24.000000 itkdb_gtk-0.9.0/itkdb_gtk/GroundVITests.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (501) staff       (20)    24242 2024-04-01 21:45:02.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (501) staff       (20)     9916 2024-04-03 15:11:28.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    14862 2024-04-03 15:55:55.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     8407 2024-02-29 19:12:17.000000 itkdb_gtk-0.9.0/itkdb_gtk/ShowAttachments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3154 2024-02-29 19:16:49.000000 itkdb_gtk-0.9.0/itkdb_gtk/ShowComments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3533 2024-02-29 19:17:50.000000 itkdb_gtk-0.9.0/itkdb_gtk/ShowDefects.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    28135 2024-04-03 15:15:38.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadModuleIV.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    22120 2024-04-03 15:16:30.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadMultipleTests.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    22194 2024-04-03 15:16:49.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadPetalInformation.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    16511 2024-04-03 15:16:59.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadTest.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    25761 2024-04-03 15:17:14.000000 itkdb_gtk-0.9.0/itkdb_gtk/WireBondGui.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1106 2024-04-04 08:12:34.000000 itkdb_gtk-0.9.0/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     6321 2024-04-01 19:22:49.000000 itkdb_gtk-0.9.0/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    25071 2024-04-03 15:12:56.000000 itkdb_gtk-0.9.0/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    19394 2024-04-03 15:15:12.000000 itkdb_gtk-0.9.0/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     2673 2024-04-03 15:15:17.000000 itkdb_gtk-0.9.0/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      757 2024-04-03 15:15:24.000000 itkdb_gtk-0.9.0/itkdb_gtk/untrash_component.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.517701 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (501) staff       (20)     3148 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)      821 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      433 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       83 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       10 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)     1320 2024-04-04 08:09:10.000000 itkdb_gtk-0.9.0/pyproject.toml
+-rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-04-04 08:12:35.518119 itkdb_gtk-0.9.0/setup.cfg
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.517392 itkdb_gtk-0.9.0/test/
+-rw-r--r--   0 lacasta    (501) staff       (20)     4165 2024-04-03 15:09:05.000000 itkdb_gtk-0.9.0/test/test_holes.py
```

### Comparing `itkdb_gtk-0.0.9/PKG-INFO` & `itkdb_gtk-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.0.9
+Version: 0.9.0
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: itkdb>=0.4.0
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
+Requires-Dist: pyserial
+Requires-Dist: python_dateutil
+Requires-Dist: requests
+Requires-Dist: PyGObject
 
 # Interaction with the ITk PDB.
 
 This folder contains a collection of scripts that help interacting with the DB
 using a Gtk based GUI, which includes a first attempt of reauthentication.
 
 You need to install itkdb and serial. The former for obvious reasons. The latter
@@ -32,33 +40,36 @@
 updated before expiration. This is usefull for very long sessions in the GUI.
 
 ## uploadPetalInformation.py
 Reads the AVS Production Sheet and FAT reports. With this information it creates
 the petal core in the DB, if not yet there, make the assembly of the components,
 and uploadas the test runs made at AVS.
 
-## uploadTest.py
+## UploadTest.py
 A GUI to upload the JSON files corresponding to a test and, also, to add
 attachmetns.
 
-## uploadMultipleTests.py
+## UploadMultipleTests.py
 This will allow to select various test files, or even scan a whole directory to
 find them, and assign comments, defects or attachments to each of the tests found.
 
-## getShipments.py
+## GetShipments.py
 Find all shipments to be received at a given site and list them. It handles a
 barcode reader that helps identifying the items actually received for the
 reception. It will finally make the DB aware of the items receptioned.
 
-## sendShipments.py
+## CreateShipments.py
 Create a new shipment. Allows to add items with the QR reader as well as from a
 GUI dialog. One can add comments and attachments to the shipment.
 
-## groundingTest.py
-Allows to enter valueos, comments and defects for those ot items in the gounding
+## GroundVITests.py
+Allows to upload and enter valueos, comments and defects for those items in the gounding
 and visual instpections tests of the petal core.
 
+## UploadModuleIV.py
+The idea behind this is that we messure the IV on a Ring module and on only one of the to Half modules. The IV of the remaining half modules is derived from the other 2. Eventually the IV test can be uploaded to the DB.
+
 ## dashBoard.py
 This is an launcher application from which we can start most of the other
 applications. It is a very good starting point. There is a Gnome desktop file (ITkDB.desktop)
-that needs to be copied to $HOME/.local/share/applications and an icon (ITkDB.svg) that
-needs to go to $HOME/.local/share/icons
+that needs to be copied to `$HOME/.local/share/applications` and an icon (ITkDB.svg) that
+needs to go to `$HOME/.local/share/icons`
```

### Comparing `itkdb_gtk-0.0.9/README.md` & `itkdb_gtk-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,33 +20,36 @@
 updated before expiration. This is usefull for very long sessions in the GUI.
 
 ## uploadPetalInformation.py
 Reads the AVS Production Sheet and FAT reports. With this information it creates
 the petal core in the DB, if not yet there, make the assembly of the components,
 and uploadas the test runs made at AVS.
 
-## uploadTest.py
+## UploadTest.py
 A GUI to upload the JSON files corresponding to a test and, also, to add
 attachmetns.
 
-## uploadMultipleTests.py
+## UploadMultipleTests.py
 This will allow to select various test files, or even scan a whole directory to
 find them, and assign comments, defects or attachments to each of the tests found.
 
-## getShipments.py
+## GetShipments.py
 Find all shipments to be received at a given site and list them. It handles a
 barcode reader that helps identifying the items actually received for the
 reception. It will finally make the DB aware of the items receptioned.
 
-## sendShipments.py
+## CreateShipments.py
 Create a new shipment. Allows to add items with the QR reader as well as from a
 GUI dialog. One can add comments and attachments to the shipment.
 
-## groundingTest.py
-Allows to enter valueos, comments and defects for those ot items in the gounding
+## GroundVITests.py
+Allows to upload and enter valueos, comments and defects for those items in the gounding
 and visual instpections tests of the petal core.
 
+## UploadModuleIV.py
+The idea behind this is that we messure the IV on a Ring module and on only one of the to Half modules. The IV of the remaining half modules is derived from the other 2. Eventually the IV test can be uploaded to the DB.
+
 ## dashBoard.py
 This is an launcher application from which we can start most of the other
 applications. It is a very good starting point. There is a Gnome desktop file (ITkDB.desktop)
-that needs to be copied to $HOME/.local/share/applications and an icon (ITkDB.svg) that
-needs to go to $HOME/.local/share/icons
+that needs to be copied to `$HOME/.local/share/applications` and an icon (ITkDB.svg) that
+needs to go to `$HOME/.local/share/icons`
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.9.0/itkdb_gtk/GlueWeight.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 import argparse
 import json
 import sys
 from copy import deepcopy
 from pathlib import Path
 
 try:
-    import dbGtkUtils
-    import ITkDBlogin
-    import ITkDButils
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+    import itkdb_gtk
+    
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio
 
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
@@ -26,20 +29,18 @@
     return v.lower() in ("yes", "true", "t", "1")
 
 
 def find_module(ifile, module_sn="MODULE_SN"):
     """Find the starting line of a module.
 
     Args:
-    ----
         ifile: the input file object.
         module_sn: tag t ostar t a new module.
 
-    Return:
-    ------
+    Returns:
         the SN of the module.
 
     """
     line = ifile.readline()
     if line is None:
         return None
 
@@ -60,20 +61,18 @@
     return None
 
 
 def remove_defaul_keys(data, default_value=-9999):
     """Remove keys with deafault value.
 
     Args:
-    ----
         data: Input dictionary
         default_value: Defaultvalue. Defaults to -9999.
 
-    Returns
-    -------
+    Returns:
         data: trimmed dictionary
 
     """
     keys = []
     for key, val in data.items():
         if val == default_value:
             keys.append(key)
@@ -85,17 +84,16 @@
 
 
 class GlueWeight(Gtk.Window):
     """Upluead Glue Weight test."""
 
     def __init__(self, session, ifile=None):
         """Initialization.
-
+    
         Args:
-        ----
             session: ITkDB session_
             ifile (optional): Input file. Defaults to None.
 
         """
         global gtk_runs
         self.ifile = ifile
         self.session = session
@@ -198,21 +196,19 @@
         self.hide()
         self.destroy()
 
     def create_test_window(self, test_json, test_name, label):
         """Create the dialog for a DB test and add it to the notebook.
 
         Args:
-        ----
             test_json: The JSon-like dict with the values
             test_name: The name of the test for internal indexing
             label: The label for the Notebook
 
-        Return:
-        ------
+        Returns:
             The box containing the data.
 
         """
         scrolled, gM = dbGtkUtils.create_scrolled_dictdialog(test_json)
         self.test_list.append(gM)
         self.test_index[test_name] = len(self.test_list) - 1
         box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
@@ -264,20 +260,18 @@
         with open(path, "r") as ifile:
             self.modules = self.parse_file(ifile)
 
     def parse_file(self, ifile, module_sep="MODULE_SN"):
         """Parse a data file.
 
         Args:
-        ----
             ifile (): A file object.
             module_sep: tag to idenntify a new module.
 
-        Returns
-        -------
+        Returns:
             a list of tests (json)
 
         """
         ifile.seek(0, 0)
 
         # Now get the modules in the file
         modules = []
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/ITkDB.svg` & `itkdb_gtk-0.9.0/itkdb_gtk/ITkDB.svg`

 * *Files 1% similar despite different names*

```diff
@@ -15,1486 +15,1502 @@
 000000e0: 3020 3735 2036 302e 3030 3030 3031 220a  0 75 60.000001".
 000000f0: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
 00000100: 6573 6572 7665 220a 2020 2073 6f64 6970  eserve".   sodip
 00000110: 6f64 693a 646f 636e 616d 653d 2249 546b  odi:docname="ITk
 00000120: 4442 2e73 7667 220a 2020 2077 6964 7468  DB.svg".   width
 00000130: 3d22 3735 220a 2020 2068 6569 6768 743d  ="75".   height=
 00000140: 2236 3022 0a20 2020 696e 6b73 6361 7065  "60".   inkscape
-00000150: 3a76 6572 7369 6f6e 3d22 312e 3220 2864  :version="1.2 (d
-00000160: 6332 6165 6461 2c20 3230 3232 2d30 352d  c2aeda, 2022-05-
-00000170: 3135 2922 0a20 2020 786d 6c6e 733a 696e  15)".   xmlns:in
-00000180: 6b73 6361 7065 3d22 6874 7470 3a2f 2f77  kscape="http://w
-00000190: 7777 2e69 6e6b 7363 6170 652e 6f72 672f  ww.inkscape.org/
-000001a0: 6e61 6d65 7370 6163 6573 2f69 6e6b 7363  namespaces/inksc
-000001b0: 6170 6522 0a20 2020 786d 6c6e 733a 736f  ape".   xmlns:so
-000001c0: 6469 706f 6469 3d22 6874 7470 3a2f 2f73  dipodi="http://s
-000001d0: 6f64 6970 6f64 692e 736f 7572 6365 666f  odipodi.sourcefo
-000001e0: 7267 652e 6e65 742f 4454 442f 736f 6469  rge.net/DTD/sodi
-000001f0: 706f 6469 2d30 2e64 7464 220a 2020 2078  podi-0.dtd".   x
-00000200: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
-00000210: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00000220: 220a 2020 2078 6d6c 6e73 3a73 7667 3d22  ".   xmlns:svg="
-00000230: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00000240: 672f 3230 3030 2f73 7667 223e 3c64 6566  g/2000/svg"><def
-00000250: 730a 2020 2069 643d 2264 6566 7331 3737  s.   id="defs177
-00000260: 223e 3c63 6c69 7050 6174 680a 2020 2020  "><clipPath.    
-00000270: 2069 643d 2263 6c69 7050 6174 6831 3622   id="clipPath16"
-00000280: 0a20 2020 2020 636c 6970 5061 7468 556e  .     clipPathUn
-00000290: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
-000002a0: 5573 6522 3e3c 7061 7468 0a20 2020 2020  Use"><path.     
-000002b0: 2020 6964 3d22 7061 7468 3138 220a 2020    id="path18".  
-000002c0: 2020 2020 2064 3d22 4d20 302c 3631 3220       d="M 0,612 
-000002d0: 4820 3739 3220 5620 3020 4820 3020 5a22  H 792 V 0 H 0 Z"
-000002e0: 202f 3e3c 2f63 6c69 7050 6174 683e 3c63   /></clipPath><c
-000002f0: 6c69 7050 6174 680a 2020 2020 2069 643d  lipPath.     id=
-00000300: 2263 6c69 7050 6174 6834 3822 0a20 2020  "clipPath48".   
-00000310: 2020 636c 6970 5061 7468 556e 6974 733d    clipPathUnits=
-00000320: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
-00000330: 3e3c 7061 7468 0a20 2020 2020 2020 6964  ><path.       id
-00000340: 3d22 7061 7468 3530 220a 2020 2020 2020  ="path50".      
-00000350: 2064 3d22 4d20 302c 3631 3220 4820 3739   d="M 0,612 H 79
-00000360: 3220 5620 3020 4820 3020 5a22 202f 3e3c  2 V 0 H 0 Z" /><
-00000370: 2f63 6c69 7050 6174 683e 3c63 6c69 7050  /clipPath><clipP
-00000380: 6174 680a 2020 2020 2069 643d 2263 6c69  ath.     id="cli
-00000390: 7050 6174 6831 3038 220a 2020 2020 2063  pPath108".     c
-000003a0: 6c69 7050 6174 6855 6e69 7473 3d22 7573  lipPathUnits="us
-000003b0: 6572 5370 6163 654f 6e55 7365 223e 3c70  erSpaceOnUse"><p
-000003c0: 6174 680a 2020 2020 2020 2069 643d 2270  ath.       id="p
-000003d0: 6174 6831 3130 220a 2020 2020 2020 2064  ath110".       d
-000003e0: 3d22 4d20 302c 3631 3220 4820 3739 3220  ="M 0,612 H 792 
-000003f0: 5620 3020 4820 3020 5a22 202f 3e3c 2f63  V 0 H 0 Z" /></c
-00000400: 6c69 7050 6174 683e 3c2f 6465 6673 3e3c  lipPath></defs><
-00000410: 736f 6469 706f 6469 3a6e 616d 6564 7669  sodipodi:namedvi
-00000420: 6577 0a20 2020 6964 3d22 6e61 6d65 6476  ew.   id="namedv
-00000430: 6965 7731 3735 220a 2020 2070 6167 6563  iew175".   pagec
-00000440: 6f6c 6f72 3d22 2366 6666 6666 6622 0a20  olor="#ffffff". 
-00000450: 2020 626f 7264 6572 636f 6c6f 723d 2223    bordercolor="#
-00000460: 3636 3636 3636 220a 2020 2062 6f72 6465  666666".   borde
-00000470: 726f 7061 6369 7479 3d22 312e 3022 0a20  ropacity="1.0". 
-00000480: 2020 696e 6b73 6361 7065 3a73 686f 7770    inkscape:showp
-00000490: 6167 6573 6861 646f 773d 2232 220a 2020  ageshadow="2".  
-000004a0: 2069 6e6b 7363 6170 653a 7061 6765 6f70   inkscape:pageop
-000004b0: 6163 6974 793d 2230 2e30 220a 2020 2069  acity="0.0".   i
-000004c0: 6e6b 7363 6170 653a 7061 6765 6368 6563  nkscape:pagechec
-000004d0: 6b65 7262 6f61 7264 3d22 3022 0a20 2020  kerboard="0".   
-000004e0: 696e 6b73 6361 7065 3a64 6573 6b63 6f6c  inkscape:deskcol
-000004f0: 6f72 3d22 2364 3164 3164 3122 0a20 2020  or="#d1d1d1".   
-00000500: 7368 6f77 6772 6964 3d22 6661 6c73 6522  showgrid="false"
-00000510: 0a20 2020 696e 6b73 6361 7065 3a7a 6f6f  .   inkscape:zoo
-00000520: 6d3d 2231 302e 3134 3330 3934 220a 2020  m="10.143094".  
-00000530: 2069 6e6b 7363 6170 653a 6378 3d22 3338   inkscape:cx="38
-00000540: 2e37 3934 3836 3922 0a20 2020 696e 6b73  .794869".   inks
-00000550: 6361 7065 3a63 793d 2231 382e 3837 3938  cape:cy="18.8798
-00000560: 3431 220a 2020 2069 6e6b 7363 6170 653a  41".   inkscape:
-00000570: 6375 7272 656e 742d 6c61 7965 723d 2267  current-layer="g
-00000580: 3130 2220 2f3e 0a3c 670a 2020 2069 643d  10" />.<g.   id=
-00000590: 2267 3134 3222 0a20 2020 7472 616e 7366  "g142".   transf
-000005a0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
-000005b0: 342e 3832 3837 3439 2c2d 312e 3537 3430  4.828749,-1.5740
-000005c0: 3435 3929 223e 0a09 0a09 0a09 0a09 0a09  459)">..........
-000005d0: 0a3c 670a 2020 2069 643d 2267 3935 3432  .<g.   id="g9542
-000005e0: 220a 2020 2074 7261 6e73 666f 726d 3d22  ".   transform="
-000005f0: 7472 616e 736c 6174 6528 322e 3537 3435  translate(2.5745
-00000600: 2c32 2e34 3733 3534 3539 2922 3e3c 670a  ,2.4735459)"><g.
-00000610: 2020 2020 2069 643d 2267 3936 3632 223e       id="g9662">
-00000620: 3c70 6174 680a 2020 2020 2020 2064 3d22  <path.       d="
-00000630: 6d20 3532 2e35 3234 2c34 352e 3533 3720  m 52.524,45.537 
-00000640: 6320 2d30 2e34 3239 2c2d 342e 3130 3720  c -0.429,-4.107 
-00000650: 2d33 2e38 3532 2c2d 372e 3333 3220 2d37  -3.852,-7.332 -7
-00000660: 2e39 3533 2c2d 372e 3333 3220 2d32 2e35  .953,-7.332 -2.5
-00000670: 3634 2c30 202d 342e 3938 342c 312e 3238  64,0 -4.984,1.28
-00000680: 3620 2d36 2e34 382c 332e 3430 3220 2d30  6 -6.48,3.402 -0
-00000690: 2e32 3931 2c2d 302e 3035 3120 2d30 2e35  .291,-0.051 -0.5
-000006a0: 3836 2c2d 302e 3037 3620 2d30 2e38 3833  86,-0.076 -0.883
-000006b0: 2c2d 302e 3037 3620 2d32 2e33 322c 3020  ,-0.076 -2.32,0 
-000006c0: 2d34 2e33 3831 2c31 2e35 3737 202d 352e  -4.381,1.577 -5.
-000006d0: 3036 362c 332e 3831 3320 2d31 2e39 3037  066,3.813 -1.907
-000006e0: 2c31 2e31 3331 202d 332e 3131 362c 332e  ,1.131 -3.116,3.
-000006f0: 3234 3120 2d33 2e31 3136 2c35 2e35 3032  241 -3.116,5.502
-00000700: 2030 2c33 2e35 3037 2032 2e37 3835 2c36   0,3.507 2.785,6
-00000710: 2e33 3539 2036 2e32 3038 2c36 2e33 3539  .359 6.208,6.359
-00000720: 2068 2031 302e 3737 3420 6320 302e 3036   h 10.774 c 0.06
-00000730: 2c30 2030 2e31 3138 2c2d 302e 3030 3420  ,0 0.118,-0.004 
-00000740: 302e 3137 312c 2d30 2e30 3038 2030 2e30  0.171,-0.008 0.0
-00000750: 3632 2c30 2e30 3034 2030 2e31 3234 2c30  62,0.004 0.124,0
-00000760: 2e30 3038 2030 2e31 3838 2c30 2e30 3038  .008 0.188,0.008
-00000770: 2068 2034 2e33 3120 6320 332e 3232 352c   h 4.31 c 3.225,
-00000780: 3020 352e 3834 392c 2d32 2e36 3837 2035  0 5.849,-2.687 5
-00000790: 2e38 3439 2c2d 352e 3938 3920 2d30 2e30  .849,-5.989 -0.0
-000007a0: 3031 2c2d 322e 3620 2d31 2e36 3432 2c2d  01,-2.6 -1.642,-
-000007b0: 342e 3837 3420 2d34 2e30 3032 2c2d 352e  4.874 -4.002,-5.
-000007c0: 3637 3920 7a20 6d20 2d31 2e38 3437 2c39  679 z m -1.847,9
-000007d0: 2e36 3638 202d 342e 3335 322c 2d30 2e30  .668 -4.352,-0.0
-000007e0: 3033 202d 302e 3137 2c2d 302e 3030 3620  03 -0.17,-0.006 
-000007f0: 2d31 302e 3932 322c 302e 3030 3920 6320  -10.922,0.009 c 
-00000800: 2d32 2e33 322c 3020 2d34 2e32 3038 2c2d  -2.32,0 -4.208,-
-00000810: 312e 3935 3620 2d34 2e32 3038 2c2d 342e  1.956 -4.208,-4.
-00000820: 3335 3920 302c 2d31 2e36 3635 2030 2e39  359 0,-1.665 0.9
-00000830: 3439 2c2d 332e 3231 2032 2e34 3137 2c2d  49,-3.21 2.417,-
-00000840: 332e 3933 3520 6c20 302e 3433 352c 2d30  3.935 l 0.435,-0
-00000850: 2e32 3134 2030 2e31 3032 2c2d 302e 3437  .214 0.102,-0.47
-00000860: 3520 6320 302e 3333 312c 2d31 2e35 3620  5 c 0.331,-1.56 
-00000870: 312e 3638 392c 2d32 2e36 3931 2033 2e32  1.689,-2.691 3.2
-00000880: 3239 2c2d 322e 3639 3120 302e 3334 352c  29,-2.691 0.345,
-00000890: 3020 302e 3638 382c 302e 3035 3720 312e  0 0.688,0.057 1.
-000008a0: 3032 2c30 2e31 3638 206c 2030 2e37 3737  02,0.168 l 0.777
-000008b0: 2c30 2e32 3631 2030 2e34 3038 2c2d 302e  ,0.261 0.408,-0.
-000008c0: 3731 3120 6320 312e 3039 362c 2d31 2e39  711 c 1.096,-1.9
-000008d0: 3036 2033 2e30 3234 2c2d 332e 3034 3420  06 3.024,-3.044 
-000008e0: 352e 3135 382c 2d33 2e30 3434 2033 2e32  5.158,-3.044 3.2
-000008f0: 3635 2c30 2035 2e39 3535 2c32 2e37 3437  65,0 5.955,2.747
-00000900: 2035 2e39 3938 2c36 2e31 3233 206c 2030   5.998,6.123 l 0
-00000910: 2e30 3131 2c30 2e38 3133 2030 2e37 3939  .011,0.813 0.799
-00000920: 2c30 2e31 3535 2063 2031 2e38 3233 2c30  ,0.155 c 1.823,0
-00000930: 2e33 3534 2033 2e31 3436 2c32 2e30 3032  .354 3.146,2.002
-00000940: 2033 2e31 3436 2c33 2e39 3139 2030 2c32   3.146,3.919 0,2
-00000950: 2e32 202d 312e 3732 362c 332e 3939 202d  .2 -1.726,3.99 -
-00000960: 332e 3834 382c 332e 3939 207a 220a 2020  3.848,3.99 z".  
-00000970: 2020 2020 2069 643d 2270 6174 6831 3332       id="path132
-00000980: 2220 2f3e 3c70 6174 680a 2020 2020 2020  " /><path.      
-00000990: 2064 3d22 6d20 3239 2e38 3735 2c34 332e   d="m 29.875,43.
-000009a0: 3034 3420 6320 312e 3336 332c 2d32 2e36  044 c 1.363,-2.6
-000009b0: 3138 2033 2e39 362c 2d34 2e33 3337 2036  18 3.96,-4.337 6
-000009c0: 2e38 3732 2c2d 342e 3520 322e 3036 362c  .872,-4.5 2.066,
-000009d0: 2d32 2e31 3237 2034 2e38 3934 2c2d 332e  -2.127 4.894,-3.
-000009e0: 3333 3920 372e 3832 342c 2d33 2e33 3339  339 7.824,-3.339
-000009f0: 2032 2e35 3331 2c30 2034 2e39 3136 2c30   2.531,0 4.916,0
-00000a00: 2e39 3136 2036 2e38 3138 2c32 2e34 3535  .916 6.818,2.455
-00000a10: 2030 2e30 3935 2c2d 302e 3038 3720 302e   0.095,-0.087 0.
-00000a20: 3230 332c 2d30 2e31 3733 2030 2e32 3837  203,-0.173 0.287
-00000a30: 2c2d 302e 3236 2076 202d 312e 3238 3920  ,-0.26 v -1.289 
-00000a40: 2d30 2e35 202d 302e 3520 5620 3238 2063  -0.5 -0.5 V 28 c
-00000a50: 202d 312e 3331 382c 302e 3930 3520 2d33   -1.318,0.905 -3
-00000a60: 2e30 3238 2c31 2e36 3937 202d 352e 3032  .028,1.697 -5.02
-00000a70: 352c 322e 3336 3720 2d34 2e32 312c 312e  5,2.367 -4.21,1.
-00000a80: 3437 3220 2d31 302e 3034 382c 322e 3530  472 -10.048,2.50
-00000a90: 3220 2d31 372e 3336 392c 322e 3730 3320  2 -17.369,2.703 
-00000aa0: 2d30 2e38 372c 302e 3032 3720 2d31 2e37  -0.87,0.027 -1.7
-00000ab0: 342c 302e 3034 3120 2d32 2e36 3036 2c30  4,0.041 -2.606,0
-00000ac0: 2e30 3431 202d 302e 3836 392c 3020 2d31  .041 -0.869,0 -1
-00000ad0: 2e37 3432 2c2d 302e 3031 3420 2d32 2e36  .742,-0.014 -2.6
-00000ae0: 3134 2c2d 302e 3034 3220 4320 3136 2e37  14,-0.042 C 16.7
-00000af0: 3231 2c33 322e 3836 3820 3130 2e38 3731  21,32.868 10.871
-00000b00: 2c33 312e 3833 3120 362e 3635 392c 3330  ,31.831 6.659,30
-00000b10: 2e33 3532 2034 2e36 382c 3239 2e36 3835  .352 4.68,29.685
-00000b20: 2032 2e39 3834 2c32 382e 3839 3920 312e   2.984,28.899 1.
-00000b30: 3637 362c 3238 2076 2037 2e31 3131 2030  676,28 v 7.111 0
-00000b40: 2e35 2030 2e35 2031 2e32 3839 2063 2032  .5 0.5 1.289 c 2
-00000b50: 2e38 3436 2c32 2e39 3731 2031 322e 3339  .846,2.971 12.39
-00000b60: 342c 352e 3731 3120 3235 2c35 2e37 3131  4,5.711 25,5.711
-00000b70: 2031 2e30 3933 2c30 2032 2e31 3534 2c2d   1.093,0 2.154,-
-00000b80: 302e 3032 3820 332e 3139 392c 2d30 2e30  0.028 3.199,-0.0
-00000b90: 3637 207a 220a 2020 2020 2020 2069 643d  67 z".       id=
-00000ba0: 2270 6174 6831 3334 2220 2f3e 3c70 6174  "path134" /><pat
-00000bb0: 680a 2020 2020 2020 2064 3d22 6d20 3234  h.       d="m 24
-00000bc0: 2e33 3131 2c32 392e 3936 3520 6320 302e  .311,29.965 c 0.
-00000bd0: 3332 362c 302e 3030 3920 302e 3635 312c  326,0.009 0.651,
-00000be0: 302e 3031 3820 302e 3938 322c 302e 3032  0.018 0.982,0.02
-00000bf0: 3320 302e 3435 362c 302e 3030 3820 302e  3 0.456,0.008 0.
-00000c00: 3931 372c 302e 3031 3220 312e 3338 332c  917,0.012 1.383,
-00000c10: 302e 3031 3220 302e 3436 362c 3020 302e  0.012 0.466,0 0.
-00000c20: 3932 362c 2d30 2e30 3034 2031 2e33 3833  926,-0.004 1.383
-00000c30: 2c2d 302e 3031 3120 302e 3333 2c2d 302e  ,-0.011 0.33,-0.
-00000c40: 3030 3520 302e 3635 362c 2d30 2e30 3135  005 0.656,-0.015
-00000c50: 2030 2e39 3832 2c2d 302e 3032 3320 302e   0.982,-0.023 0.
-00000c60: 3131 362c 2d30 2e30 3033 2030 2e32 3334  116,-0.003 0.234
-00000c70: 2c2d 302e 3030 3520 302e 3334 392c 2d30  ,-0.005 0.349,-0
-00000c80: 2e30 3038 2031 312e 3235 332c 2d30 2e33  .008 11.253,-0.3
-00000c90: 3539 2031 392e 3634 382c 2d32 2e39 3135  59 19.648,-2.915
-00000ca0: 2032 322e 3238 362c 2d35 2e36 3638 2056   22.286,-5.668 V
-00000cb0: 2032 3320 3232 2e35 2032 3220 3134 2e38   23 22.5 22 14.8
-00000cc0: 3839 2043 2034 362e 3830 382c 3138 2e32  89 C 46.808,18.2
-00000cd0: 3332 2033 362e 3532 2c32 3020 3236 2e36  32 36.52,20 26.6
-00000ce0: 3736 2c32 3020 3136 2e38 3332 2c32 3020  76,20 16.832,20 
-00000cf0: 362e 3534 332c 3138 2e32 3332 2031 2e36  6.543,18.232 1.6
-00000d00: 3736 2c31 342e 3838 3920 5620 3232 2032  76,14.889 V 22 2
-00000d10: 322e 3520 3233 2032 342e 3238 3920 6320  2.5 23 24.289 c 
-00000d20: 322e 3633 382c 322e 3735 3420 3131 2e30  2.638,2.754 11.0
-00000d30: 3333 2c35 2e33 3120 3232 2e32 3836 2c35  33,5.31 22.286,5
-00000d40: 2e36 3638 2030 2e31 3135 2c30 2e30 3033  .668 0.115,0.003
-00000d50: 2030 2e32 3333 2c30 2e30 3035 2030 2e33   0.233,0.005 0.3
-00000d60: 3439 2c30 2e30 3038 207a 220a 2020 2020  49,0.008 z".    
-00000d70: 2020 2069 643d 2270 6174 6831 3336 2220     id="path136" 
-00000d80: 2f3e 3c70 6174 680a 2020 2020 2020 2064  /><path.       d
-00000d90: 3d22 4d20 3531 2e36 3736 2c31 312e 3330  ="M 51.676,11.30
-00000da0: 3620 5620 392e 3520 3920 4320 3531 2e36  6 V 9.5 9 C 51.6
-00000db0: 3736 2c38 2e38 3332 2035 312e 3632 2c38  76,8.832 51.62,8
-00000dc0: 2e36 3831 2035 312e 3534 312c 382e 3534  .681 51.541,8.54
-00000dd0: 3220 3530 2e34 3138 2c34 2e32 3431 2034  2 50.418,4.241 4
-00000de0: 312e 3739 312c 3020 3236 2e36 3736 2c30  1.791,0 26.676,0
-00000df0: 2031 312e 3539 382c 3020 322e 3937 392c   11.598,0 2.979,
-00000e00: 342e 3232 2031 2e38 3232 2c38 2e35 3120  4.22 1.822,8.51 
-00000e10: 312e 3733 372c 382e 3635 3720 312e 3637  1.737,8.657 1.67
-00000e20: 362c 382e 3831 3820 312e 3637 362c 3920  6,8.818 1.676,9 
-00000e30: 7620 302e 3520 312e 3830 3620 6320 322e  v 0.5 1.806 c 2.
-00000e40: 3833 362c 322e 3936 3120 3132 2e33 3136  836,2.961 12.316
-00000e50: 2c35 2e36 3934 2032 352c 352e 3639 3420  ,5.694 25,5.694 
-00000e60: 3132 2e36 3834 2c30 2032 322e 3136 332c  12.684,0 22.163,
-00000e70: 2d32 2e37 3333 2032 352c 2d35 2e36 3934  -2.733 25,-5.694
-00000e80: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-00000e90: 6174 6831 3338 2220 2f3e 3c70 6174 680a  ath138" /><path.
-00000ea0: 2020 2020 2020 2064 3d22 6d20 3236 2e30         d="m 26.0
-00000eb0: 3235 2c35 302e 3834 3520 6320 302c 2d31  25,50.845 c 0,-1
-00000ec0: 2e36 3532 2030 2e34 3531 2c2d 332e 3234  .652 0.451,-3.24
-00000ed0: 3920 312e 3234 392c 2d34 2e36 3531 202d  9 1.249,-4.651 -
-00000ee0: 302e 3230 312c 3130 652d 3420 2d30 2e33  0.201,10e-4 -0.3
-00000ef0: 3935 2c30 2e30 3037 202d 302e 3539 392c  95,0.007 -0.599,
-00000f00: 302e 3030 3720 2d31 322e 3334 362c 3020  0.007 -12.346,0 
-00000f10: 2d32 302e 3836 362c 2d32 2e32 3920 2d32  -20.866,-2.29 -2
-00000f20: 352c 2d35 2e32 3031 2076 2038 2e32 3031  5,-5.201 v 8.201
-00000f30: 2063 2030 2c30 2e31 3632 2030 2e30 3433   c 0,0.162 0.043
-00000f40: 2c30 2e33 3135 2030 2e31 3137 2c30 2e34  ,0.315 0.117,0.4
-00000f50: 3531 2031 2e31 3831 2c34 2e38 3935 2031  51 1.181,4.895 1
-00000f60: 312e 3734 372c 382e 3534 3920 3234 2e38  1.747,8.549 24.8
-00000f70: 3833 2c38 2e35 3439 2030 2e39 352c 3020  83,8.549 0.95,0 
-00000f80: 312e 3838 312c 2d30 2e30 3234 2032 2e38  1.881,-0.024 2.8
-00000f90: 3031 2c2d 302e 3036 3220 2d32 2e31 2c2d  01,-0.062 -2.1,-
-00000fa0: 312e 3731 3720 2d33 2e34 3531 2c2d 342e  1.717 -3.451,-4.
-00000fb0: 3334 3720 2d33 2e34 3531 2c2d 372e 3239  347 -3.451,-7.29
-00000fc0: 3420 7a22 0a20 2020 2020 2020 6964 3d22  4 z".       id="
-00000fd0: 7061 7468 3134 3022 202f 3e3c 2f67 3e3c  path140" /></g><
-00000fe0: 670a 2020 2020 2074 7261 6e73 666f 726d  g.     transform
-00000ff0: 3d22 6d61 7472 6978 2830 2c2d 302e 3431  ="matrix(0,-0.41
-00001000: 3031 3839 3332 2c2d 302e 3339 3331 3335  018932,-0.393135
-00001010: 3432 2c30 2c32 3138 2e38 3635 3736 2c33  42,0,218.86576,3
-00001020: 3138 2e31 3931 3434 2922 0a20 2020 2020  18.19144)".     
-00001030: 6964 3d22 6731 3022 0a20 2020 2020 7374  id="g10".     st
-00001040: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
-00001050: 6622 3e3c 670a 2020 2069 643d 2267 3132  f"><g.   id="g12
-00001060: 220a 2020 2073 7479 6c65 3d22 6669 6c6c  ".   style="fill
-00001070: 3a23 3030 3030 6666 223e 3c67 0a20 2020  :#0000ff"><g.   
-00001080: 2020 636c 6970 2d70 6174 683d 2275 726c    clip-path="url
-00001090: 2823 636c 6970 5061 7468 3136 2922 0a20  (#clipPath16)". 
-000010a0: 2020 2020 6964 3d22 6731 3422 0a20 2020      id="g14".   
-000010b0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-000010c0: 3030 3066 6622 3e3c 670a 2020 2020 2020  000ff"><g.      
-000010d0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-000010e0: 736c 6174 6528 3730 382e 3330 3437 2c35  slate(708.3047,5
-000010f0: 3636 2e30 3735 3229 220a 2020 2020 2020  66.0752)".      
-00001100: 2069 643d 2267 3230 220a 2020 2020 2020   id="g20".      
-00001110: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
-00001120: 3030 6666 223e 3c70 6174 680a 2020 2020  00ff"><path.    
-00001130: 2020 2020 2069 643d 2270 6174 6832 3222       id="path22"
-00001140: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00001150: 2266 696c 6c3a 2330 3030 3066 663b 6669  "fill:#0000ff;fi
-00001160: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
-00001170: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
-00001180: 7472 6f6b 653a 6e6f 6e65 220a 2020 2020  troke:none".    
-00001190: 2020 2020 2064 3d22 6d20 302c 3020 6320       d="m 0,0 c 
-000011a0: 302e 3034 322c 2d31 2e35 3233 202d 302e  0.042,-1.523 -0.
-000011b0: 3437 372c 2d32 2e37 3632 202d 312e 3535  477,-2.762 -1.55
-000011c0: 322c 2d33 2e37 3120 2d31 2e30 3737 2c2d  2,-3.71 -1.077,-
-000011d0: 302e 3934 3720 2d32 2e35 3935 2c2d 312e  0.947 -2.595,-1.
-000011e0: 3438 3320 2d34 2e35 362c 2d31 2e36 3036  483 -4.56,-1.606
-000011f0: 202d 312e 3830 382c 2d30 2e31 3136 202d   -1.808,-0.116 -
-00001200: 332e 3431 342c 302e 3132 3520 2d34 2e38  3.414,0.125 -4.8
-00001210: 3234 2c30 2e37 3134 206c 202d 302e 3039  24,0.714 l -0.09
-00001220: 2c33 2e33 3331 2063 2031 2e31 3537 2c2d  ,3.331 c 1.157,-
-00001230: 302e 3433 3920 322e 3133 342c 2d30 2e37  0.439 2.134,-0.7
-00001240: 3335 2032 2e39 332c 2d30 2e38 3933 2030  35 2.93,-0.893 0
-00001250: 2e37 3939 2c2d 302e 3135 3820 312e 3532  .799,-0.158 1.52
-00001260: 372c 2d30 2e32 3137 2032 2e31 3833 2c2d  7,-0.217 2.183,-
-00001270: 302e 3137 3620 302e 3738 382c 302e 3035  0.176 0.788,0.05
-00001280: 3120 312e 3339 2c30 2e32 3420 312e 3830  1 1.39,0.24 1.80
-00001290: 312c 302e 3536 3320 302e 3431 322c 302e  1,0.563 0.412,0.
-000012a0: 3332 3920 302e 3631 2c30 2e37 3920 302e  329 0.61,0.79 0.
-000012b0: 3539 352c 312e 3338 3220 2d30 2e30 312c  595,1.382 -0.01,
-000012c0: 302e 3333 3220 2d30 2e31 312c 302e 3632  0.332 -0.11,0.62
-000012d0: 3320 2d30 2e33 3031 2c30 2e38 3638 202d  3 -0.301,0.868 -
-000012e0: 302e 3139 342c 302e 3234 3620 2d30 2e34  0.194,0.246 -0.4
-000012f0: 3734 2c30 2e34 3738 202d 302e 3833 382c  74,0.478 -0.838,
-00001300: 302e 3639 3520 2d30 2e33 3637 2c30 2e32  0.695 -0.367,0.2
-00001310: 3135 202d 312e 3130 392c 302e 3535 3120  15 -1.109,0.551 
-00001320: 2d32 2e32 332c 312e 3030 3420 2d31 2e30  -2.23,1.004 -1.0
-00001330: 3437 2c30 2e34 3234 202d 312e 3833 362c  47,0.424 -1.836,
-00001340: 302e 3834 202d 322e 3336 352c 312e 3235  0.84 -2.365,1.25
-00001350: 3420 2d30 2e35 332c 302e 3431 3520 2d30  4 -0.53,0.415 -0
-00001360: 2e39 3539 2c30 2e39 3039 202d 312e 3238  .959,0.909 -1.28
-00001370: 322c 312e 3438 3320 2d30 2e33 3235 2c30  2,1.483 -0.325,0
-00001380: 2e35 3731 202d 302e 352c 312e 3235 3720  .571 -0.5,1.257 
-00001390: 2d30 2e35 3232 2c32 2e30 3532 202d 302e  -0.522,2.052 -0.
-000013a0: 3034 312c 312e 3439 3320 302e 3433 372c  041,1.493 0.437,
-000013b0: 322e 3730 3120 312e 3432 372c 332e 3632  2.701 1.427,3.62
-000013c0: 2030 2e39 3933 2c30 2e39 3139 2032 2e33   0.993,0.919 2.3
-000013d0: 3836 2c31 2e34 3335 2034 2e31 3737 2c31  86,1.435 4.177,1
-000013e0: 2e35 3520 302e 3838 312c 302e 3035 3520  .55 0.881,0.055 
-000013f0: 312e 3732 322c 302e 3030 3520 322e 3532  1.722,0.005 2.52
-00001400: 382c 2d30 2e31 3533 2030 2e38 3037 2c2d  8,-0.153 0.807,-
-00001410: 302e 3135 3820 312e 3634 392c 2d30 2e34  0.158 1.649,-0.4
-00001420: 2032 2e35 3335 2c2d 302e 3732 3120 4c20   2.535,-0.721 L 
-00001430: 2d31 2e34 3732 2c38 2e33 3936 2043 202d  -1.472,8.396 C -
-00001440: 322e 3338 352c 382e 3731 3220 2d33 2e31  2.385,8.712 -3.1
-00001450: 3339 2c38 2e39 3232 202d 332e 3733 342c  39,8.922 -3.734,
-00001460: 392e 3033 3120 2d34 2e33 3239 2c39 2e31  9.031 -4.329,9.1
-00001470: 3420 2d34 2e39 3131 2c39 2e31 3738 202d  4 -4.911,9.178 -
-00001480: 352e 3438 342c 392e 3134 202d 362e 3136  5.484,9.14 -6.16
-00001490: 352c 392e 3039 3820 2d36 2e36 3832 2c38  5,9.098 -6.682,8
-000014a0: 2e39 3038 202d 372e 3033 362c 382e 3536  .908 -7.036,8.56
-000014b0: 3720 2d37 2e33 3932 2c38 2e32 3239 202d  7 -7.392,8.229 -
-000014c0: 372e 3536 312c 372e 3830 3720 2d37 2e35  7.561,7.807 -7.5
-000014d0: 3436 2c37 2e32 3936 202d 372e 3533 382c  46,7.296 -7.538,
-000014e0: 362e 3937 3920 2d37 2e34 3537 2c36 2e37  6.979 -7.457,6.7
-000014f0: 3120 2d37 2e33 3034 2c36 2e34 3832 202d  1 -7.304,6.482 -
-00001500: 372e 3135 312c 362e 3235 3820 2d36 2e39  7.151,6.258 -6.9
-00001510: 312c 362e 3034 3620 2d36 2e35 3832 2c35  1,6.046 -6.582,5
-00001520: 2e38 3438 202d 362e 3236 2c35 2e36 3436  .848 -6.26,5.646
-00001530: 202d 352e 3438 362c 352e 3239 3920 2d34   -5.486,5.299 -4
-00001540: 2e32 3735 2c34 2e38 3035 202d 322e 3637  .275,4.805 -2.67
-00001550: 312c 342e 3135 202d 312e 3536 342c 332e  1,4.15 -1.564,3.
-00001560: 3436 3120 2d30 2e39 3535 2c32 2e37 3420  461 -0.955,2.74 
-00001570: 2d30 2e33 3439 2c32 2e30 3134 202d 302e  -0.349,2.014 -0.
-00001580: 3032 392c 312e 3130 3220 302c 3022 202f  029,1.102 0,0" /
-00001590: 3e3c 2f67 3e3c 670a 2020 2020 2020 2074  ></g><g.       t
-000015a0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-000015b0: 6174 6528 3635 312e 3439 3032 2c35 3631  ate(651.4902,561
-000015c0: 2e30 3034 3929 220a 2020 2020 2020 2069  .0049)".       i
-000015d0: 643d 2267 3234 220a 2020 2020 2020 2073  d="g24".       s
-000015e0: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
-000015f0: 6666 223e 3c70 6174 680a 2020 2020 2020  ff"><path.      
-00001600: 2020 2069 643d 2270 6174 6832 3622 0a20     id="path26". 
-00001610: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00001620: 696c 6c3a 2330 3030 3066 663b 6669 6c6c  ill:#0000ff;fill
-00001630: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
-00001640: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
-00001650: 6f6b 653a 6e6f 6e65 220a 2020 2020 2020  oke:none".      
-00001660: 2020 2064 3d22 4d20 302c 3020 2d31 2e32     d="M 0,0 -1.2
-00001670: 3238 2c34 2e30 3331 2048 202d 372e 3430  28,4.031 H -7.40
-00001680: 3220 4c20 2d38 2e36 3331 2c30 2048 202d  2 L -8.631,0 H -
-00001690: 3132 2e35 206c 2035 2e39 3738 2c31 372e  12.5 l 5.978,17.
-000016a0: 3030 3620 6820 342e 3339 204c 2033 2e38  006 h 4.39 L 3.8
-000016b0: 3638 2c30 205a 206d 202d 322e 3038 362c  68,0 Z m -2.086,
-000016c0: 372e 3034 3420 6320 2d31 2e31 3336 2c33  7.044 c -1.136,3
-000016d0: 2e36 3531 202d 312e 3737 332c 352e 3731  .651 -1.773,5.71
-000016e0: 3820 2d31 2e39 3138 2c36 2e31 3936 202d  8 -1.918,6.196 -
-000016f0: 302e 3134 322c 302e 3437 3920 2d30 2e32  0.142,0.479 -0.2
-00001700: 3433 2c30 2e38 3536 202d 302e 3330 362c  43,0.856 -0.306,
-00001710: 312e 3133 3520 2d30 2e32 3533 2c2d 302e  1.135 -0.253,-0.
-00001720: 3938 3820 2d30 2e39 3835 2c2d 332e 3433  988 -0.985,-3.43
-00001730: 3420 2d32 2e31 3838 2c2d 372e 3333 3120  4 -2.188,-7.331 
-00001740: 7a22 202f 3e3c 2f67 3e3c 670a 2020 2020  z" /></g><g.    
-00001750: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00001760: 616e 736c 6174 6528 3636 312e 3239 3539  anslate(661.2959
-00001770: 2c35 3631 2e30 3034 3929 220a 2020 2020  ,561.0049)".    
-00001780: 2020 2069 643d 2267 3238 220a 2020 2020     id="g28".    
-00001790: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-000017a0: 3030 3030 6666 223e 3c70 6174 680a 2020  0000ff"><path.  
-000017b0: 2020 2020 2020 2069 643d 2270 6174 6833         id="path3
-000017c0: 3022 0a20 2020 2020 2020 2020 7374 796c  0".         styl
-000017d0: 653d 2266 696c 6c3a 2330 3030 3066 663b  e="fill:#0000ff;
-000017e0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-000017f0: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-00001800: 3b73 7472 6f6b 653a 6e6f 6e65 220a 2020  ;stroke:none".  
-00001810: 2020 2020 2020 2064 3d22 4d20 302c 3020         d="M 0,0 
-00001820: 4820 2d33 2e35 3932 2056 2031 332e 3934  H -3.592 V 13.94
-00001830: 3720 4820 2d38 2e31 3920 7620 322e 3938  7 H -8.19 v 2.98
-00001840: 3820 4820 342e 3539 3920 5620 3133 2e39  8 H 4.599 V 13.9
-00001850: 3437 2048 2030 205a 2220 2f3e 3c2f 673e  47 H 0 Z" /></g>
-00001860: 3c67 0a20 2020 2020 2020 7472 616e 7366  <g.       transf
-00001870: 6f72 6d3d 2274 7261 6e73 6c61 7465 2836  orm="translate(6
-00001880: 3638 2e30 3930 382c 3536 312e 3030 3439  68.0908,561.0049
-00001890: 2922 0a20 2020 2020 2020 6964 3d22 6733  )".       id="g3
-000018a0: 3222 0a20 2020 2020 2020 7374 796c 653d  2".       style=
-000018b0: 2266 696c 6c3a 2330 3030 3066 6622 3e3c  "fill:#0000ff"><
-000018c0: 7061 7468 0a20 2020 2020 2020 2020 6964  path.         id
-000018d0: 3d22 7061 7468 3334 220a 2020 2020 2020  ="path34".      
-000018e0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-000018f0: 3030 3030 6666 3b66 696c 6c2d 6f70 6163  0000ff;fill-opac
-00001900: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-00001910: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
-00001920: 6f6e 6522 0a20 2020 2020 2020 2020 643d  one".         d=
-00001930: 224d 2030 2c30 2056 2031 362e 3933 3520  "M 0,0 V 16.935 
-00001940: 4820 332e 3539 3120 5620 322e 3936 3520  H 3.591 V 2.965 
-00001950: 6820 362e 3837 2056 2030 205a 2220 2f3e  h 6.87 V 0 Z" />
-00001960: 3c2f 673e 3c67 0a20 2020 2020 2020 7472  </g><g.       tr
-00001970: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00001980: 7465 2836 3932 2e33 3434 372c 3536 312e  te(692.3447,561.
-00001990: 3030 3439 2922 0a20 2020 2020 2020 6964  0049)".       id
-000019a0: 3d22 6733 3622 0a20 2020 2020 2020 7374  ="g36".       st
-000019b0: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
-000019c0: 6622 3e3c 7061 7468 0a20 2020 2020 2020  f"><path.       
-000019d0: 2020 6964 3d22 7061 7468 3338 220a 2020    id="path38".  
-000019e0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000019f0: 6c6c 3a23 3030 3030 6666 3b66 696c 6c2d  ll:#0000ff;fill-
-00001a00: 6f70 6163 6974 793a 313b 6669 6c6c 2d72  opacity:1;fill-r
-00001a10: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
-00001a20: 6b65 3a6e 6f6e 6522 0a20 2020 2020 2020  ke:none".       
-00001a30: 2020 643d 224d 2030 2c30 202d 312e 3232    d="M 0,0 -1.22
-00001a40: 392c 342e 3033 3120 4820 2d37 2e34 3032  9,4.031 H -7.402
-00001a50: 204c 202d 382e 3633 2c30 2068 202d 332e   L -8.63,0 h -3.
-00001a60: 3837 3120 6c20 352e 3937 382c 3137 2e30  871 l 5.978,17.0
-00001a70: 3036 2068 2034 2e33 3932 204c 2033 2e38  06 h 4.392 L 3.8
-00001a80: 3639 2c30 205a 206d 202d 322e 3038 372c  69,0 Z m -2.087,
-00001a90: 372e 3034 3420 6320 2d31 2e31 3335 2c33  7.044 c -1.135,3
-00001aa0: 2e36 3531 202d 312e 3737 342c 352e 3731  .651 -1.774,5.71
-00001ab0: 3820 2d31 2e39 3136 2c36 2e31 3936 202d  8 -1.916,6.196 -
-00001ac0: 302e 3134 332c 302e 3437 3920 2d30 2e32  0.143,0.479 -0.2
-00001ad0: 3434 2c30 2e38 3536 202d 302e 3330 382c  44,0.856 -0.308,
-00001ae0: 312e 3133 3520 2d30 2e32 3535 2c2d 302e  1.135 -0.255,-0.
-00001af0: 3938 3820 2d30 2e39 3832 2c2d 332e 3433  988 -0.982,-3.43
-00001b00: 3420 2d32 2e31 392c 2d37 2e33 3331 207a  4 -2.19,-7.331 z
-00001b10: 2220 2f3e 3c2f 673e 3c2f 673e 3c2f 673e  " /></g></g></g>
-00001b20: 3c74 6578 740a 2020 2069 643d 2274 6578  <text.   id="tex
-00001b30: 7434 3022 0a20 2020 7374 796c 653d 2266  t40".   style="f
-00001b40: 6f6e 742d 7661 7269 616e 743a 6e6f 726d  ont-variant:norm
-00001b50: 616c 3b66 6f6e 742d 7765 6967 6874 3a62  al;font-weight:b
-00001b60: 6f6c 643b 666f 6e74 2d73 7472 6574 6368  old;font-stretch
-00001b70: 3a63 6f6e 6465 6e73 6564 3b66 6f6e 742d  :condensed;font-
-00001b80: 7369 7a65 3a32 372e 3230 3337 7078 3b66  size:27.2037px;f
-00001b90: 6f6e 742d 6661 6d69 6c79 3a27 4865 6c76  ont-family:'Helv
-00001ba0: 6574 6963 6120 4e65 7565 273b 2d69 6e6b  etica Neue';-ink
-00001bb0: 7363 6170 652d 666f 6e74 2d73 7065 6369  scape-font-speci
-00001bc0: 6669 6361 7469 6f6e 3a48 656c 7665 7469  fication:Helveti
-00001bd0: 6361 4e65 7565 2d43 6f6e 6465 6e73 6564  caNeue-Condensed
-00001be0: 426c 6163 6b3b 7772 6974 696e 672d 6d6f  Black;writing-mo
-00001bf0: 6465 3a6c 722d 7462 3b66 696c 6c3a 2330  de:lr-tb;fill:#0
-00001c00: 3030 3066 663b 6669 6c6c 2d6f 7061 6369  000ff;fill-opaci
-00001c10: 7479 3a31 3b66 696c 6c2d 7275 6c65 3a6e  ty:1;fill-rule:n
-00001c20: 6f6e 7a65 726f 3b73 7472 6f6b 653a 6e6f  onzero;stroke:no
-00001c30: 6e65 220a 2020 2074 7261 6e73 666f 726d  ne".   transform
-00001c40: 3d22 6d61 7472 6978 2831 2c30 2c30 2c2d  ="matrix(1,0,0,-
-00001c50: 312c 3733 322e 3739 3339 2c35 3631 2e30  1,732.7939,561.0
-00001c60: 3639 3329 223e 3c74 7370 616e 0a20 2020  693)"><tspan.   
-00001c70: 2020 6964 3d22 7473 7061 6e34 3222 0a20    id="tspan42". 
-00001c80: 2020 2020 793d 2230 220a 2020 2020 2078      y="0".     x
-00001c90: 3d22 3020 372e 3037 3239 3631 3820 3139  ="0 7.0729618 19
-00001ca0: 2e36 3431 3037 3122 0a20 2020 2020 7374  .641071".     st
-00001cb0: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
-00001cc0: 6622 3e49 546b 3c2f 7473 7061 6e3e 3c2f  f">ITk</tspan></
-00001cd0: 7465 7874 3e0a 3c67 0a20 2020 6964 3d22  text>.<g.   id="
-00001ce0: 6734 3422 0a20 2020 7374 796c 653d 2266  g44".   style="f
-00001cf0: 696c 6c3a 2330 3030 3066 6622 3e3c 670a  ill:#0000ff"><g.
-00001d00: 2020 2020 2063 6c69 702d 7061 7468 3d22       clip-path="
-00001d10: 7572 6c28 2363 6c69 7050 6174 6834 3829  url(#clipPath48)
-00001d20: 220a 2020 2020 2069 643d 2267 3436 220a  ".     id="g46".
-00001d30: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00001d40: 3a23 3030 3030 6666 223e 3c67 0a20 2020  :#0000ff"><g.   
-00001d50: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-00001d60: 7261 6e73 6c61 7465 2837 3138 2e30 3834  ranslate(718.084
-00001d70: 2c35 3833 2e30 3531 3829 220a 2020 2020  ,583.0518)".    
-00001d80: 2020 2069 643d 2267 3532 220a 2020 2020     id="g52".    
-00001d90: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00001da0: 3030 3030 6666 223e 3c70 6174 680a 2020  0000ff"><path.  
-00001db0: 2020 2020 2020 2069 643d 2270 6174 6835         id="path5
-00001dc0: 3422 0a20 2020 2020 2020 2020 7374 796c  4".         styl
-00001dd0: 653d 2266 696c 6c3a 2330 3030 3066 663b  e="fill:#0000ff;
-00001de0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-00001df0: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-00001e00: 3b73 7472 6f6b 653a 6e6f 6e65 220a 2020  ;stroke:none".  
-00001e10: 2020 2020 2020 2064 3d22 6d20 302c 3020         d="m 0,0 
-00001e20: 6320 2d33 2e30 3132 2c2d 302e 3930 3420  c -3.012,-0.904 
-00001e30: 2d34 2e36 372c 2d30 2e37 3236 202d 342e  -4.67,-0.726 -4.
-00001e40: 3937 382c 2d30 2e31 3331 206c 202d 302e  978,-0.131 l -0.
-00001e50: 3533 2c2d 302e 3237 3320 6320 302e 3238  53,-0.273 c 0.28
-00001e60: 332c 2d30 2e35 3438 2030 2e39 3933 2c2d  3,-0.548 0.993,-
-00001e70: 302e 3832 3320 322e 3035 362c 2d30 2e38  0.823 2.056,-0.8
-00001e80: 3233 2030 2e39 3836 2c30 2032 2e32 3734  23 0.986,0 2.274
-00001e90: 2c30 2e32 3338 2033 2e38 3036 2c30 2e37  ,0.238 3.806,0.7
-00001ea0: 3120 4320 302e 3233 342c 2d30 2e33 3436  1 C 0.234,-0.346
-00001eb0: 2030 2e31 3136 2c2d 302e 3137 3320 302c   0.116,-0.173 0,
-00001ec0: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
-00001ed0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00001ee0: 616e 736c 6174 6528 3732 322e 3131 3034  anslate(722.1104
-00001ef0: 2c35 3932 2e31 3035 3529 220a 2020 2020  ,592.1055)".    
-00001f00: 2020 2069 643d 2267 3536 220a 2020 2020     id="g56".    
-00001f10: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00001f20: 3030 3030 6666 223e 3c70 6174 680a 2020  0000ff"><path.  
-00001f30: 2020 2020 2020 2069 643d 2270 6174 6835         id="path5
-00001f40: 3822 0a20 2020 2020 2020 2020 7374 796c  8".         styl
-00001f50: 653d 2266 696c 6c3a 2330 3030 3066 663b  e="fill:#0000ff;
-00001f60: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-00001f70: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-00001f80: 3b73 7472 6f6b 653a 6e6f 6e65 220a 2020  ;stroke:none".  
-00001f90: 2020 2020 2020 2064 3d22 6d20 302c 3020         d="m 0,0 
-00001fa0: 6320 302e 3138 392c 302e 3038 3720 302e  c 0.189,0.087 0.
-00001fb0: 3337 382c 302e 3137 3320 302e 3536 372c  378,0.173 0.567,
-00001fc0: 302e 3235 3520 2d32 2e36 392c 332e 3135  0.255 -2.69,3.15
-00001fd0: 3120 2d35 2e32 3638 2c34 2e35 3439 202d  1 -5.268,4.549 -
-00001fe0: 362e 3733 372c 332e 3635 3120 6c20 302e  6.737,3.651 l 0.
-00001ff0: 3331 312c 2d30 2e35 3120 4320 2d34 2e37  311,-0.51 C -4.7
-00002000: 3134 2c34 2e30 3939 202d 322e 3337 342c  14,4.099 -2.374,
-00002010: 322e 3733 3620 302c 3022 202f 3e3c 2f67  2.736 0,0" /></g
-00002020: 3e3c 670a 2020 2020 2020 2074 7261 6e73  ><g.       trans
-00002030: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00002040: 3733 322e 3130 3934 2c35 3932 2e37 3439  732.1094,592.749
-00002050: 2922 0a20 2020 2020 2020 6964 3d22 6736  )".       id="g6
-00002060: 3022 0a20 2020 2020 2020 7374 796c 653d  0".       style=
-00002070: 2266 696c 6c3a 2330 3030 3066 6622 3e3c  "fill:#0000ff"><
-00002080: 7061 7468 0a20 2020 2020 2020 2020 6964  path.         id
-00002090: 3d22 7061 7468 3632 220a 2020 2020 2020  ="path62".      
-000020a0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-000020b0: 3030 3030 6666 3b66 696c 6c2d 6f70 6163  0000ff;fill-opac
-000020c0: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-000020d0: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
-000020e0: 6f6e 6522 0a20 2020 2020 2020 2020 643d  one".         d=
-000020f0: 224d 2030 2c30 202d 302e 3532 392c 2d30  "M 0,0 -0.529,-0
-00002100: 2e32 3733 2043 202d 302e 3433 332c 2d30  .273 C -0.433,-0
-00002110: 2e34 3632 202d 302e 3434 2c2d 302e 3731  .462 -0.44,-0.71
-00002120: 202d 302e 3534 372c 2d31 2e30 3034 202d   -0.547,-1.004 -
-00002130: 312e 3334 312c 312e 3532 3520 2d32 2e39  1.341,1.525 -2.9
-00002140: 3939 2c33 2e34 3437 202d 352e 3233 312c  99,3.447 -5.231,
-00002150: 342e 3431 3520 4c20 2d35 2e34 372c 332e  4.415 L -5.47,3.
-00002160: 3836 3720 6320 322e 3130 372c 2d30 2e39  867 c 2.107,-0.9
-00002170: 3133 2033 2e36 3638 2c2d 322e 3734 3920  13 3.668,-2.749 
-00002180: 342e 3339 342c 2d35 2e31 3732 2030 2e30  4.394,-5.172 0.0
-00002190: 3435 2c2d 302e 3134 3820 302e 3038 352c  45,-0.148 0.085,
-000021a0: 2d30 2e32 3936 2030 2e31 3232 2c2d 302e  -0.296 0.122,-0.
-000021b0: 3434 3520 2d30 2e37 382c 2d31 2e31 3139  445 -0.78,-1.119
-000021c0: 202d 322e 3436 342c 2d32 2e36 3038 202d   -2.464,-2.608 -
-000021d0: 342e 3834 392c 2d34 2e31 3132 202d 302e  4.849,-4.112 -0.
-000021e0: 3333 382c 302e 3636 3120 2d30 2e37 3037  338,0.661 -0.707
-000021f0: 2c31 2e33 3235 202d 312e 3130 392c 312e  ,1.325 -1.109,1.
-00002200: 3938 3320 2d30 2e33 3633 2c30 2e35 3920  983 -0.363,0.59 
-00002210: 2d30 2e37 3433 2c31 2e31 3634 202d 312e  -0.743,1.164 -1.
-00002220: 3133 362c 312e 3731 3420 2d30 2e31 3831  136,1.714 -0.181
-00002230: 2c2d 302e 3037 3820 2d30 2e33 3638 2c2d  ,-0.078 -0.368,-
-00002240: 302e 3135 3820 2d30 2e35 3538 2c2d 302e  0.158 -0.558,-0.
-00002250: 3234 3220 302e 3430 392c 2d30 2e35 3720  242 0.409,-0.57 
-00002260: 302e 3830 372c 2d31 2e31 3639 2031 2e31  0.807,-1.169 1.1
-00002270: 3834 2c2d 312e 3738 3420 302e 3430 342c  84,-1.784 0.404,
-00002280: 2d30 2e36 3632 2030 2e37 3734 2c2d 312e  -0.662 0.774,-1.
-00002290: 3332 3820 312e 3130 392c 2d31 2e39 3836  328 1.109,-1.986
-000022a0: 202d 302e 3639 312c 2d30 2e34 3139 202d   -0.691,-0.419 -
-000022b0: 312e 3433 322c 2d30 2e38 3339 202d 322e  1.432,-0.839 -2.
-000022c0: 3232 372c 2d31 2e32 3438 202d 312e 3132  227,-1.248 -1.12
-000022d0: 362c 2d30 2e35 3832 202d 322e 3235 322c  6,-0.582 -2.252,
-000022e0: 2d31 2e30 3935 202d 332e 3335 332c 2d31  -1.095 -3.353,-1
-000022f0: 2e35 3238 2030 2e31 322c 2d30 2e31 3720  .528 0.12,-0.17 
-00002300: 302e 3233 392c 2d30 2e33 3336 2030 2e33  0.239,-0.336 0.3
-00002310: 3538 2c2d 302e 3439 3820 312e 3037 352c  58,-0.498 1.075,
-00002320: 302e 3433 2032 2e31 3734 2c30 2e39 3320  0.43 2.174,0.93 
-00002330: 332e 3237 312c 312e 3439 3820 302e 3735  3.271,1.498 0.75
-00002340: 312c 302e 3338 3820 312e 3439 352c 302e  1,0.388 1.495,0.
-00002350: 3830 3620 322e 3231 352c 312e 3234 3120  806 2.215,1.241 
-00002360: 302e 3734 312c 2d31 2e35 3433 2031 2e32  0.741,-1.543 1.2
-00002370: 3735 2c2d 332e 3034 3620 312e 3534 362c  75,-3.046 1.546,
-00002380: 2d34 2e33 3834 2030 2e31 3334 2c2d 302e  -4.384 0.134,-0.
-00002390: 3637 2030 2e31 3936 2c2d 312e 3236 3920  67 0.196,-1.269 
-000023a0: 302e 3139 312c 2d31 2e37 3932 202d 322e  0.191,-1.792 -2.
-000023b0: 3634 362c 2d32 2e35 3335 202d 362e 3235  646,-2.535 -6.25
-000023c0: 352c 2d33 2e35 3036 202d 392e 3335 332c  5,-3.506 -9.353,
-000023d0: 2d32 2e31 3635 204c 202d 3133 2e39 2c2d  -2.165 L -13.9,-
-000023e0: 3135 2e36 2063 2031 2e30 322c 2d30 2e34  15.6 c 1.02,-0.4
-000023f0: 3432 2032 2e30 3931 2c2d 302e 3635 3220  42 2.091,-0.652 
-00002400: 332e 3136 392c 2d30 2e36 3532 2032 2e32  3.169,-0.652 2.2
-00002410: 3232 2c30 2034 2e34 3636 2c30 2e38 3934  22,0 4.466,0.894
-00002420: 2036 2e33 3236 2c32 2e34 3739 202d 302e   6.326,2.479 -0.
-00002430: 3131 372c 2d30 2e35 3136 202d 302e 3334  117,-0.516 -0.34
-00002440: 332c 2d30 2e38 3920 2d30 2e36 3732 2c2d  3,-0.89 -0.672,-
-00002450: 312e 3039 3120 6c20 302e 3331 312c 2d30  1.091 l 0.311,-0
-00002460: 2e35 3039 2063 2030 2e36 3331 2c30 2e33  .509 c 0.631,0.3
-00002470: 3837 2030 2e39 3832 2c31 2e31 3533 2031  87 0.982,1.153 1
-00002480: 2e30 3431 2c32 2e32 3237 2031 2e30 3637  .041,2.227 1.067
-00002490: 2c31 2e30 3636 2031 2e39 3733 2c32 2e33  ,1.066 1.973,2.3
-000024a0: 3733 2032 2e36 3237 2c33 2e38 3834 2031  73 2.627,3.884 1
-000024b0: 2e30 3436 2c32 2e34 3135 2031 2e33 3133  .046,2.415 1.313
-000024c0: 2c35 2e30 3131 2030 2e37 3833 2c37 2e33  ,5.011 0.783,7.3
-000024d0: 3936 2043 2030 2e31 3235 2c2d 312e 3135  96 C 0.125,-1.15
-000024e0: 3520 302e 3236 382c 2d30 2e35 3134 2030  5 0.268,-0.514 0
-000024f0: 2c30 206d 202d 312e 3634 362c 2d39 2e30  ,0 m -1.646,-9.0
-00002500: 3234 2063 202d 302e 3533 372c 2d31 2e32  24 c -0.537,-1.2
-00002510: 3431 202d 312e 3235 322c 2d32 2e33 3339  41 -1.252,-2.339
-00002520: 202d 322e 3038 392c 2d33 2e32 3637 202d   -2.089,-3.267 -
-00002530: 302e 3033 2c30 2e34 3038 202d 302e 3039  0.03,0.408 -0.09
-00002540: 2c30 2e38 3436 202d 302e 3138 352c 312e  ,0.846 -0.185,1.
-00002550: 3331 3420 2d30 2e32 3833 2c31 2e34 3032  314 -0.283,1.402
-00002560: 202d 302e 3834 322c 322e 3937 3320 2d31   -0.842,2.973 -1
-00002570: 2e36 3137 2c34 2e35 3831 2031 2e39 3932  .617,4.581 1.992
-00002580: 2c31 2e32 3536 2033 2e37 3333 2c32 2e36  ,1.256 3.733,2.6
-00002590: 3334 2034 2e37 3434 2c33 2e38 3639 2030  34 4.744,3.869 0
-000025a0: 2e33 3535 2c2d 322e 3131 3420 302e 3036  .355,-2.114 0.06
-000025b0: 362c 2d34 2e33 3737 202d 302e 3835 332c  6,-4.377 -0.853,
-000025c0: 2d36 2e34 3937 2220 2f3e 3c2f 673e 3c67  -6.497" /></g><g
-000025d0: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-000025e0: 6d3d 2274 7261 6e73 6c61 7465 2837 3232  m="translate(722
-000025f0: 2e35 3432 2c35 3938 2e32 3632 3729 220a  .542,598.2627)".
-00002600: 2020 2020 2020 2069 643d 2267 3634 220a         id="g64".
-00002610: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00002620: 6c6c 3a23 3030 3030 6666 223e 3c70 6174  ll:#0000ff"><pat
-00002630: 680a 2020 2020 2020 2020 2069 643d 2270  h.         id="p
-00002640: 6174 6836 3622 0a20 2020 2020 2020 2020  ath66".         
-00002650: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00002660: 3066 663b 6669 6c6c 2d6f 7061 6369 7479  0ff;fill-opacity
-00002670: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-00002680: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-00002690: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
-000026a0: 302c 3020 6320 2d36 2e31 3035 2c30 202d  0,0 c -6.105,0 -
-000026b0: 3131 2e30 3736 2c2d 342e 3937 202d 3131  11.076,-4.97 -11
-000026c0: 2e30 3736 2c2d 3131 2e30 3737 2030 2c2d  .076,-11.077 0,-
-000026d0: 362e 3130 3820 342e 3937 312c 2d31 312e  6.108 4.971,-11.
-000026e0: 3037 3620 3131 2e30 3736 2c2d 3131 2e30  076 11.076,-11.0
-000026f0: 3736 2036 2e31 3038 2c30 2031 312e 3037  76 6.108,0 11.07
-00002700: 382c 342e 3936 3820 3131 2e30 3738 2c31  8,4.968 11.078,1
-00002710: 312e 3037 3620 4320 3131 2e30 3738 2c2d  1.076 C 11.078,-
-00002720: 342e 3937 2036 2e31 3038 2c30 2030 2c30  4.97 6.108,0 0,0
-00002730: 204d 2037 2e37 3631 2c2d 342e 3535 3920   M 7.761,-4.559 
-00002740: 4320 372e 3130 392c 2d34 2e35 3036 2036  C 7.109,-4.506 6
-00002750: 2e33 3035 2c2d 342e 3537 3820 352e 3335  .305,-4.578 5.35
-00002760: 322c 2d34 2e37 3820 332e 3332 392c 2d35  2,-4.78 3.329,-5
-00002770: 2e32 3037 2030 2e37 3939 2c2d 362e 3137  .207 0.799,-6.17
-00002780: 3820 2d31 2e37 3739 2c2d 372e 3531 2063  8 -1.779,-7.51 c
-00002790: 202d 312e 3335 2c2d 302e 3639 3820 2d32   -1.35,-0.698 -2
-000027a0: 2e36 3634 2c2d 312e 3437 3720 2d33 2e38  .664,-1.477 -3.8
-000027b0: 342c 2d32 2e32 3833 202d 302e 3436 392c  4,-2.283 -0.469,
-000027c0: 312e 3133 3420 2d30 2e38 3132 2c32 2e32  1.134 -0.812,2.2
-000027d0: 3237 202d 312e 3030 362c 332e 3232 3720  27 -1.006,3.227 
-000027e0: 2d30 2e30 3635 2c30 2e33 3432 202d 302e  -0.065,0.342 -0.
-000027f0: 3131 332c 302e 3636 3720 2d30 2e31 3431  113,0.667 -0.141
-00002800: 2c30 2e39 3639 2032 2e30 3436 2c32 2e39  ,0.969 2.046,2.9
-00002810: 3639 2035 2e32 3136 2c34 2e36 3920 382e  69 5.216,4.69 8.
-00002820: 3238 372c 342e 3534 3420 322e 3439 312c  287,4.544 2.491,
-00002830: 2d30 2e33 3736 2034 2e36 3836 2c2d 312e  -0.376 4.686,-1.
-00002840: 3636 3120 362e 3234 2c2d 332e 3530 3620  661 6.24,-3.506 
-00002850: 6d20 2d31 342e 3030 332c 312e 3436 3320  m -14.003,1.463 
-00002860: 6320 312e 3038 352c 302e 3835 2032 2e33  c 1.085,0.85 2.3
-00002870: 3436 2c31 2e34 3839 2033 2e37 3138 2c31  46,1.489 3.718,1
-00002880: 2e38 3339 202d 312e 3539 352c 2d30 2e37  .839 -1.595,-0.7
-00002890: 3035 202d 332e 3037 352c 2d31 2e38 3533  05 -3.075,-1.853
-000028a0: 202d 342e 3236 322c 2d33 2e33 3538 2030   -4.262,-3.358 0
-000028b0: 2e30 3433 2c30 2e36 3938 2030 2e32 3236  .043,0.698 0.226
-000028c0: 2c31 2e32 3138 2030 2e35 3434 2c31 2e35  ,1.218 0.544,1.5
-000028d0: 3139 206d 202d 312e 3238 2c2d 332e 3735  19 m -1.28,-3.75
-000028e0: 3220 6320 302e 3231 392c 2d31 2e30 3920  2 c 0.219,-1.09 
-000028f0: 302e 3630 322c 2d32 2e32 3737 2031 2e31  0.602,-2.277 1.1
-00002900: 3232 2c2d 332e 3520 2d30 2e39 3934 2c2d  22,-3.5 -0.994,-
-00002910: 302e 3733 202d 312e 3835 372c 2d31 2e34  0.73 -1.857,-1.4
-00002920: 3731 202d 322e 3531 342c 2d32 2e31 3833  71 -2.514,-2.183
-00002930: 202d 302e 3032 312c 312e 3538 3520 302e   -0.021,1.585 0.
-00002940: 3239 372c 332e 3234 3720 302e 3939 332c  297,3.247 0.993,
-00002950: 342e 3835 3720 302e 3132 352c 302e 3238  4.857 0.125,0.28
-00002960: 3220 302e 3235 372c 302e 3535 3720 302e  2 0.257,0.557 0.
-00002970: 3339 392c 302e 3832 3620 6d20 2d30 2e31  399,0.826 m -0.1
-00002980: 3935 2c32 2e33 3338 2063 202d 302e 3032  95,2.338 c -0.02
-00002990: 392c 2d30 2e34 3231 202d 302e 3031 332c  9,-0.421 -0.013,
-000029a0: 2d30 2e38 3836 2030 2e30 3434 2c2d 312e  -0.886 0.044,-1.
-000029b0: 3338 3920 2d30 2e32 3933 2c2d 302e 3438  389 -0.293,-0.48
-000029c0: 3720 2d30 2e35 3539 2c2d 302e 3939 3920  7 -0.559,-0.999 
-000029d0: 2d30 2e37 3934 2c2d 312e 3533 3920 2d30  -0.794,-1.539 -0
-000029e0: 2e38 3239 2c2d 312e 3931 3520 2d31 2e31  .829,-1.915 -1.1
-000029f0: 3437 2c2d 332e 3930 3320 2d31 2e30 3134  47,-3.903 -1.014
-00002a00: 2c2d 352e 3736 3820 2d30 2e31 322c 2d30  ,-5.768 -0.12,-0
-00002a10: 2e31 3538 202d 302e 3232 352c 2d30 2e33  .158 -0.225,-0.3
-00002a20: 3135 202d 302e 3331 392c 2d30 2e34 3639  15 -0.319,-0.469
-00002a30: 202d 302e 3232 2c30 2e38 3331 202d 302e   -0.22,0.831 -0.
-00002a40: 3333 392c 312e 3720 2d30 2e33 3339 2c32  339,1.7 -0.339,2
-00002a50: 2e35 3938 2030 2c32 2e35 3033 2030 2e39  .598 0,2.503 0.9
-00002a60: 3134 2c34 2e37 3937 2032 2e34 3232 2c36  14,4.797 2.422,6
-00002a70: 2e35 3637 206d 202d 312e 3535 392c 2d31  .567 m -1.559,-1
-00002a80: 302e 3137 3820 6320 302e 3037 362c 2d30  0.178 c 0.076,-0
-00002a90: 2e33 3620 302e 3137 2c2d 302e 3731 3120  .36 0.17,-0.711 
-00002aa0: 302e 3237 382c 2d31 2e30 3534 202d 302e  0.278,-1.054 -0.
-00002ab0: 3132 2c30 2e32 3333 202d 302e 3233 342c  12,0.233 -0.234,
-00002ac0: 302e 3437 202d 302e 3333 392c 302e 3731  0.47 -0.339,0.71
-00002ad0: 3420 2d31 3065 2d34 2c30 2e31 2030 2e30  4 -10e-4,0.1 0.0
-00002ae0: 3139 2c30 2e32 3133 2030 2e30 3631 2c30  19,0.213 0.061,0
-00002af0: 2e33 3420 6d20 3133 2e34 3637 2c2d 352e  .34 m 13.467,-5.
-00002b00: 3631 3820 6320 2d30 2e37 3939 2c2d 302e  618 c -0.799,-0.
-00002b10: 3230 3820 2d32 2e30 3738 2c30 2e33 3431  208 -2.078,0.341
-00002b20: 202d 332e 3532 332c 312e 3535 3320 302e   -3.523,1.553 0.
-00002b30: 3033 392c 2d30 2e32 3639 2030 2e30 3137  039,-0.269 0.017
-00002b40: 2c2d 302e 3534 3620 2d30 2e30 3933 2c2d  ,-0.546 -0.093,-
-00002b50: 302e 3830 3620 2d30 2e30 3338 2c2d 302e  0.806 -0.038,-0.
-00002b60: 3038 3920 2d30 2e30 3738 2c2d 302e 3137  089 -0.078,-0.17
-00002b70: 3220 2d30 2e31 3138 2c2d 302e 3235 3420  2 -0.118,-0.254 
-00002b80: 302e 3634 372c 2d30 2e34 3939 2031 2e32  0.647,-0.499 1.2
-00002b90: 3735 2c2d 302e 3838 3120 312e 3836 352c  75,-0.881 1.865,
-00002ba0: 2d31 2e31 3331 2043 2031 2e35 3736 2c2d  -1.131 C 1.576,-
-00002bb0: 3231 2e31 3220 302e 382c 2d32 312e 3231  21.12 0.8,-21.21
-00002bc0: 3720 302c 2d32 312e 3231 3720 6320 2d32  7 0,-21.217 c -2
-00002bd0: 2e35 3432 2c30 202d 342e 3836 392c 302e  .542,0 -4.869,0.
-00002be0: 3934 3520 2d36 2e36 352c 322e 3439 3720  945 -6.65,2.497 
-00002bf0: 2d31 2e31 3633 2c31 2e32 3932 202d 312e  -1.163,1.292 -1.
-00002c00: 3930 382c 322e 3938 3920 2d32 2e31 3635  908,2.989 -2.165
-00002c10: 2c34 2e38 3535 2030 2e35 3337 2c30 2e37  ,4.855 0.537,0.7
-00002c20: 3331 2031 2e34 3736 2c31 2e36 3439 2032  31 1.476,1.649 2
-00002c30: 2e38 3035 2c32 2e36 3434 2030 2e34 3137  .805,2.644 0.417
-00002c40: 2c2d 302e 3838 3320 302e 3839 392c 2d31  ,-0.883 0.899,-1
-00002c50: 2e37 3737 2031 2e34 342c 2d32 2e36 3539  .777 1.44,-2.659
-00002c60: 2030 2e38 3231 2c2d 312e 3334 3420 312e   0.821,-1.344 1.
-00002c70: 3639 352c 2d32 2e35 3420 322e 3537 342c  695,-2.54 2.574,
-00002c80: 2d33 2e35 3631 2030 2e32 3634 2c30 2e31  -3.561 0.264,0.1
-00002c90: 3835 2030 2e35 3831 2c30 2e32 3932 2030  85 0.581,0.292 0
-00002ca0: 2e39 3236 2c30 2e32 3932 2030 2e30 3238  .926,0.292 0.028
-00002cb0: 2c30 2030 2e30 3539 2c2d 302e 3030 3320  ,0 0.059,-0.003 
-00002cc0: 302e 3038 382c 2d30 2e30 3036 202d 302e  0.088,-0.006 -0.
-00002cd0: 3933 342c 312e 3033 202d 312e 3838 392c  934,1.03 -1.889,
-00002ce0: 322e 3239 3220 2d32 2e37 392c 332e 3736  2.292 -2.79,3.76
-00002cf0: 3420 2d30 2e35 3535 2c30 2e39 3038 202d  4 -0.555,0.908 -
-00002d00: 312e 3034 362c 312e 3832 3720 2d31 2e34  1.046,1.827 -1.4
-00002d10: 3634 2c32 2e37 3238 2031 2e30 3838 2c30  64,2.728 1.088,0
-00002d20: 2e37 3536 2032 2e33 3834 2c31 2e35 3435  .756 2.384,1.545
-00002d30: 2033 2e38 3837 2c32 2e33 3231 2032 2e35   3.887,2.321 2.5
-00002d40: 3034 2c31 2e32 3935 2034 2e39 3533 2c32  04,1.295 4.953,2
-00002d50: 2e32 3336 2036 2e38 3936 2c32 2e36 3436  .236 6.896,2.646
-00002d60: 2031 2e39 3735 2c30 2e34 3137 2032 2e39   1.975,0.417 2.9
-00002d70: 3339 2c30 2e31 3731 2033 2e31 352c 2d30  39,0.171 3.15,-0
-00002d80: 2e31 3735 2030 2e39 3135 2c2d 312e 3532  .175 0.915,-1.52
-00002d90: 3420 312e 3434 322c 2d33 2e33 3035 2031  4 1.442,-3.305 1
-00002da0: 2e34 3432 2c2d 352e 3230 3620 302c 2d34  .442,-5.206 0,-4
-00002db0: 2e30 3938 202d 322e 3434 342c 2d37 2e36  .098 -2.444,-7.6
-00002dc0: 3332 202d 352e 3934 382c 2d39 2e32 3239  32 -5.948,-9.229
-00002dd0: 2220 2f3e 3c2f 673e 3c67 0a20 2020 2020  " /></g><g.     
-00002de0: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
-00002df0: 6e73 6c61 7465 2837 3238 2e31 3830 372c  nslate(728.1807,
-00002e00: 3537 372e 3733 3933 2922 0a20 2020 2020  577.7393)".     
-00002e10: 2020 6964 3d22 6736 3822 0a20 2020 2020    id="g68".     
-00002e20: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-00002e30: 3030 3066 6622 3e3c 7061 7468 0a20 2020  000ff"><path.   
-00002e40: 2020 2020 2020 6964 3d22 7061 7468 3730        id="path70
-00002e50: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
-00002e60: 3d22 6669 6c6c 3a23 3030 3030 6666 3b66  ="fill:#0000ff;f
-00002e70: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
-00002e80: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
-00002e90: 7374 726f 6b65 3a6e 6f6e 6522 0a20 2020  stroke:none".   
-00002ea0: 2020 2020 2020 643d 226d 2030 2c30 2063        d="m 0,0 c
-00002eb0: 202d 302e 3036 322c 2d30 2e30 3539 202d   -0.062,-0.059 -
-00002ec0: 302e 3234 322c 2d30 2e32 3938 202d 302e  0.242,-0.298 -0.
-00002ed0: 3338 322c 2d30 2e33 3038 202d 302e 3133  382,-0.308 -0.13
-00002ee0: 382c 2d30 2e30 3131 202d 302e 3739 352c  8,-0.011 -0.795,
-00002ef0: 2d30 2e31 3334 202d 302e 3738 342c 2d30  -0.134 -0.784,-0
-00002f00: 2e33 3736 202d 302e 3538 352c 2d30 2e32  .376 -0.585,-0.2
-00002f10: 3636 202d 312e 3637 332c 2d30 2e35 3238  66 -1.673,-0.528
-00002f20: 202d 322e 3032 2c2d 302e 3637 3520 2d30   -2.02,-0.675 -0
-00002f30: 2e36 3131 2c30 2e32 3532 202d 312e 3036  .611,0.252 -1.06
-00002f40: 352c 302e 3420 2d31 2e38 3234 2c30 2e34  5,0.4 -1.824,0.4
-00002f50: 3420 2d30 2e36 3534 2c30 2e33 3720 2d31  4 -0.654,0.37 -1
-00002f60: 2e30 3534 2c30 2e34 3839 202d 312e 3339  .054,0.489 -1.39
-00002f70: 322c 302e 3534 3220 6c20 2d30 2e32 3135  2,0.542 l -0.215
-00002f80: 2c30 2e30 3631 2030 2e31 3138 2c30 2e33  ,0.061 0.118,0.3
-00002f90: 3835 2063 2030 2e34 3738 2c30 2e31 3135  85 c 0.478,0.115
-00002fa0: 2030 2e38 3633 2c30 2e35 3838 2030 2e39   0.863,0.588 0.9
-00002fb0: 3738 2c31 2e30 3836 2030 2e31 372c 302e  78,1.086 0.17,0.
-00002fc0: 3735 202d 302e 3230 312c 312e 3337 3720  75 -0.201,1.377 
-00002fd0: 2d30 2e37 3235 2c31 2e36 3139 202d 302e  -0.725,1.619 -0.
-00002fe0: 3733 392c 302e 3334 202d 312e 3538 362c  739,0.34 -1.586,
-00002ff0: 2d30 2e31 3931 202d 312e 3632 372c 2d31  -0.191 -1.627,-1
-00003000: 2e31 3231 202d 302e 3031 392c 2d30 2e35  .121 -0.019,-0.5
-00003010: 3032 2030 2e31 3137 2c2d 302e 3734 2030  02 0.117,-0.74 0
-00003020: 2e31 3634 2c2d 302e 3933 3920 302e 3030  .164,-0.939 0.00
-00003030: 352c 2d30 2e30 3138 2030 2e30 3134 2c2d  5,-0.018 0.014,-
-00003040: 302e 3033 3620 302e 3032 312c 2d30 2e30  0.036 0.021,-0.0
-00003050: 3537 202d 302e 3034 362c 2d30 2e31 3538  57 -0.046,-0.158
-00003060: 202d 302e 3130 362c 2d30 2e33 3234 202d   -0.106,-0.324 -
-00003070: 302e 3137 312c 2d30 2e34 3736 202d 302e  0.171,-0.476 -0.
-00003080: 3433 342c 302e 3136 3120 2d31 2e31 2c30  434,0.161 -1.1,0
-00003090: 2e32 3335 202d 312e 3339 382c 302e 3237  .235 -1.398,0.27
-000030a0: 3920 2d31 2e31 3932 2c30 2e37 3032 202d  9 -1.192,0.702 -
-000030b0: 322e 3432 312c 302e 3733 3820 2d32 2e39  2.421,0.738 -2.9
-000030c0: 3933 2c30 2e39 3334 202d 302e 3339 372c  93,0.934 -0.397,
-000030d0: 302e 3438 3720 2d31 2e33 3833 2c30 2e38  0.487 -1.383,0.8
-000030e0: 3839 202d 322e 3232 372c 312e 3635 3520  89 -2.227,1.655 
-000030f0: 2d30 2e30 3531 2c30 2e30 3437 2030 2e31  -0.051,0.047 0.1
-00003100: 312c 302e 3438 3320 2d30 2e33 3238 2c30  1,0.483 -0.328,0
-00003110: 2e37 3835 202d 302e 3331 2c30 2e33 3031  .785 -0.31,0.301
-00003120: 202d 302e 3336 342c 302e 3435 3420 2d30   -0.364,0.454 -0
-00003130: 2e35 3634 2c30 2e38 3935 202d 302e 3137  .564,0.895 -0.17
-00003140: 312c 302e 3137 3220 2d30 2e33 3638 2c30  1,0.172 -0.368,0
-00003150: 2e33 3037 202d 302e 3536 382c 302e 3233  .307 -0.568,0.23
-00003160: 3620 302e 3032 322c 2d30 2e31 3531 2030  6 0.022,-0.151 0
-00003170: 2e31 3533 2c2d 302e 3334 3220 302e 3230  .153,-0.342 0.20
-00003180: 312c 2d30 2e37 3637 2030 2e30 3638 2c2d  1,-0.767 0.068,-
-00003190: 302e 3630 3120 302e 3337 362c 2d30 2e39  0.601 0.376,-0.9
-000031a0: 3931 2030 2e36 3735 2c2d 312e 3436 3620  91 0.675,-1.466 
-000031b0: 302e 3536 342c 2d31 2e30 3837 2031 2e31  0.564,-1.087 1.1
-000031c0: 3334 2c2d 312e 3735 3920 322e 3030 342c  34,-1.759 2.004,
-000031d0: 2d32 2e34 3239 2031 2e31 3734 2c2d 302e  -2.429 1.174,-0.
-000031e0: 3834 3520 312e 3837 312c 2d31 2e31 3232  845 1.871,-1.122
-000031f0: 2032 2e39 382c 2d31 2e35 3036 2030 2e30   2.98,-1.506 0.0
-00003200: 3131 2c2d 302e 3638 3720 302e 3134 392c  11,-0.687 0.149,
-00003210: 2d31 2e35 3120 302e 3330 312c 2d32 2e32  -1.51 0.301,-2.2
-00003220: 3132 2030 2e30 3837 2c2d 302e 3430 3420  12 0.087,-0.404 
-00003230: 302e 3231 332c 2d30 2e36 3937 2030 2e32  0.213,-0.697 0.2
-00003240: 3032 2c2d 302e 3938 3120 2d30 2e30 3231  02,-0.981 -0.021
-00003250: 2c2d 302e 3631 3720 2d30 2e30 3632 2c2d  ,-0.617 -0.062,-
-00003260: 302e 3532 3920 2d30 2e33 3632 2c2d 312e  0.529 -0.362,-1.
-00003270: 3135 3220 2d30 2e37 3834 2c2d 312e 3631  152 -0.784,-1.61
-00003280: 3820 2d30 2e35 3735 2c2d 342e 3036 3520  8 -0.575,-4.065 
-00003290: 2d30 2e35 3332 2c2d 352e 3231 3320 302e  -0.532,-5.213 0.
-000032a0: 3030 322c 2d30 2e30 3532 2030 2e30 3033  002,-0.052 0.003
-000032b0: 2c2d 302e 3130 3220 302e 3030 342c 2d30  ,-0.102 0.004,-0
-000032c0: 2e31 3520 2d30 2e30 3035 2c2d 302e 3131  .15 -0.005,-0.11
-000032d0: 202d 302e 3035 352c 2d30 2e32 3320 2d30   -0.055,-0.23 -0
-000032e0: 2e32 3937 2c2d 302e 3235 3520 2d30 2e38  .297,-0.255 -0.8
-000032f0: 3031 2c2d 302e 3034 3620 2d31 2e38 3435  01,-0.046 -1.845
-00003300: 2c2d 302e 3536 3620 2d32 2e37 3335 2c2d  ,-0.566 -2.735,-
-00003310: 312e 3632 3520 2d30 2e37 3337 2c2d 302e  1.625 -0.737,-0.
-00003320: 3837 3820 2d31 2e34 3238 2c2d 312e 3133  878 -1.428,-1.13
-00003330: 3920 2d32 2e31 3438 2c2d 312e 3035 3420  9 -2.148,-1.054 
-00003340: 2d30 2e36 3236 2c30 2e30 3737 202d 302e  -0.626,0.077 -0.
-00003350: 3837 2c2d 302e 3236 3520 2d30 2e36 3132  87,-0.265 -0.612
-00003360: 2c2d 302e 3736 2030 2e32 3733 2c2d 302e  ,-0.76 0.273,-0.
-00003370: 3533 3420 302e 3139 312c 2d30 2e37 3134  534 0.191,-0.714
-00003380: 2030 2e31 3237 2c2d 312e 3232 3320 2d30   0.127,-1.223 -0
-00003390: 2e30 3433 2c2d 302e 3334 3220 2d30 2e31  .043,-0.342 -0.1
-000033a0: 3431 2c2d 302e 3536 3820 302e 3133 392c  41,-0.568 0.139,
-000033b0: 2d30 2e39 3039 2030 2e33 3433 2c2d 302e  -0.909 0.343,-0.
-000033c0: 3431 3720 312e 3330 392c 2d30 2e32 3139  417 1.309,-0.219
-000033d0: 2031 2e31 3038 2c2d 302e 3131 3320 2d30   1.108,-0.113 -0
-000033e0: 2e35 3937 2c30 2e33 3133 202d 302e 3130  .597,0.313 -0.10
-000033f0: 392c 312e 3036 3120 302e 3038 342c 312e  9,1.061 0.084,1.
-00003400: 3437 3720 312e 3633 372c 312e 3530 3520  477 1.637,1.505 
-00003410: 342e 3338 312c 322e 3336 3820 342e 3733  4.381,2.368 4.73
-00003420: 322c 322e 3535 3620 302e 3532 362c 302e  2,2.556 0.526,0.
-00003430: 3235 3620 312e 3139 332c 302e 3239 3620  256 1.193,0.296 
-00003440: 312e 3333 362c 302e 3930 3820 302e 3030  1.336,0.908 0.00
-00003450: 332c 302e 3031 3520 302e 3535 2c32 2e31  3,0.015 0.55,2.1
-00003460: 3134 2030 2e39 2c33 2e33 3834 2030 2e30  14 0.9,3.384 0.0
-00003470: 3539 2c30 2e32 3132 2030 2e32 3137 2c30  59,0.212 0.217,0
-00003480: 2e34 3535 2030 2e34 3339 2c30 2e33 3435  .455 0.439,0.345
-00003490: 2030 2e30 3639 2c2d 302e 3033 3320 302e   0.069,-0.033 0.
-000034a0: 3134 2c2d 302e 3038 3220 302e 3234 312c  14,-0.082 0.241,
-000034b0: 2d30 2e31 3634 2030 2e36 3036 2c2d 302e  -0.164 0.606,-0.
-000034c0: 3530 3620 312e 3432 382c 2d30 2e39 3334  506 1.428,-0.934
-000034d0: 2031 2e39 3239 2c2d 312e 3234 3420 302e   1.929,-1.244 0.
-000034e0: 3134 372c 2d30 2e30 3920 302e 3130 362c  147,-0.09 0.106,
-000034f0: 2d30 2e33 3032 2030 2e30 3038 2c2d 302e  -0.302 0.008,-0.
-00003500: 3339 3220 2d30 2e37 3935 2c2d 302e 3732  392 -0.795,-0.72
-00003510: 3520 2d30 2e39 3831 2c2d 312e 3830 3520  5 -0.981,-1.805 
-00003520: 2d30 2e39 3333 2c2d 322e 3434 3820 302e  -0.933,-2.448 0.
-00003530: 3035 322c 2d30 2e37 3038 202d 302e 3137  052,-0.708 -0.17
-00003540: 342c 2d32 2e33 3835 202d 302e 3531 352c  4,-2.385 -0.515,
-00003550: 2d33 2e30 3836 202d 302e 3336 342c 2d30  -3.086 -0.364,-0
-00003560: 2e37 3520 2d30 2e32 3737 2c2d 312e 3038  .75 -0.277,-1.08
-00003570: 3820 302e 3533 322c 2d30 2e39 3820 302e  8 0.532,-0.98 0.
-00003580: 3930 312c 302e 3131 3820 312e 3131 332c  901,0.118 1.113,
-00003590: 2d30 2e31 3732 2031 2e36 3432 2c2d 302e  -0.172 1.642,-0.
-000035a0: 3235 3620 302e 3532 362c 2d30 2e30 3835  256 0.526,-0.085
-000035b0: 2031 2e31 3234 2c30 2e34 3120 302e 3836   1.124,0.41 0.86
-000035c0: 372c 302e 3531 202d 302e 3233 352c 302e  7,0.51 -0.235,0.
-000035d0: 3039 3320 2d31 2e33 3339 2c30 2e32 3232  093 -1.339,0.222
-000035e0: 202d 312e 3737 362c 302e 3932 3520 302e   -1.776,0.925 0.
-000035f0: 3131 322c 312e 3330 3520 322e 3333 392c  112,1.305 2.339,
-00003600: 352e 3432 3520 322e 3434 322c 362e 3034  5.425 2.442,6.04
-00003610: 3320 2d30 2e32 3233 2c31 2e34 3120 2d32  3 -0.223,1.41 -2
-00003620: 2e35 3936 2c32 2e39 3936 202d 322e 3933  .596,2.996 -2.93
-00003630: 372c 332e 3239 3820 2d30 2e30 3433 2c30  7,3.298 -0.043,0
-00003640: 2e32 3134 202d 302e 3038 362c 302e 3638  .214 -0.086,0.68
-00003650: 3220 2d30 2e30 3637 2c31 2e31 3734 2030  2 -0.067,1.174 0
-00003660: 2e31 3031 2c30 2e34 3731 2030 2e36 3436  .101,0.471 0.646
-00003670: 2c31 2e38 3720 302e 3634 322c 322e 3231  ,1.87 0.642,2.21
-00003680: 3320 302e 3639 312c 2d30 2e30 3738 2031  3 0.691,-0.078 1
-00003690: 2e39 3631 2c2d 302e 3138 3420 322e 3437  .961,-0.184 2.47
-000036a0: 2c30 2e30 3836 2030 2e37 3736 2c30 2e31  ,0.086 0.776,0.1
-000036b0: 3931 2031 2e37 3638 2c30 2e39 3836 2032  91 1.768,0.986 2
-000036c0: 2e30 3139 2c31 2e32 3938 2030 2e32 3034  .019,1.298 0.204
-000036d0: 2c30 2e31 3836 2030 2e35 3732 2c30 2e31  ,0.186 0.572,0.1
-000036e0: 3938 2030 2e37 3336 2c30 2e33 3437 2030  98 0.736,0.347 0
-000036f0: 2e32 3136 2c30 2e31 3932 2030 2e33 3132  .216,0.192 0.312
-00003700: 2c30 2e33 3220 302e 3537 322c 302e 3835  ,0.32 0.572,0.85
-00003710: 3820 4320 302e 3636 362c 302e 3338 3120  8 C 0.666,0.381 
-00003720: 302e 3230 372c 302e 3139 3820 302c 3022  0.207,0.198 0,0"
-00003730: 202f 3e3c 2f67 3e3c 2f67 3e3c 2f67 3e3c   /></g></g></g><
-00003740: 670a 2020 2074 7261 6e73 666f 726d 3d22  g.   transform="
-00003750: 7472 616e 736c 6174 6528 3736 362e 3132  translate(766.12
-00003760: 372c 3538 332e 3232 3735 2922 0a20 2020  7,583.2275)".   
-00003770: 6964 3d22 6737 3222 0a20 2020 7374 796c  id="g72".   styl
-00003780: 653d 2266 696c 6c3a 2330 3030 3066 6622  e="fill:#0000ff"
-00003790: 3e3c 7061 7468 0a20 2020 2020 6964 3d22  ><path.     id="
-000037a0: 7061 7468 3734 220a 2020 2020 2073 7479  path74".     sty
-000037b0: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
-000037c0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-000037d0: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
-000037e0: 6f3b 7374 726f 6b65 3a6e 6f6e 6522 0a20  o;stroke:none". 
-000037f0: 2020 2020 643d 226d 2030 2c30 2068 202d      d="m 0,0 h -
-00003800: 3333 2e37 3920 6c20 302e 3434 352c 342e  33.79 l 0.445,4.
-00003810: 3833 3320 2d31 2e32 3139 2c34 2e39 3338  833 -1.219,4.938
-00003820: 204c 2030 2c39 2e37 3336 205a 2220 2f3e   L 0,9.736 Z" />
-00003830: 3c2f 673e 3c67 0a20 2020 7472 616e 7366  </g><g.   transf
-00003840: 6f72 6d3d 2274 7261 6e73 6c61 7465 2837  orm="translate(7
-00003850: 3336 2e39 3239 372c 3539 332e 3035 3537  36.9297,593.0557
-00003860: 2922 0a20 2020 6964 3d22 6737 3622 0a20  )".   id="g76". 
-00003870: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-00003880: 3030 3066 6622 3e3c 7061 7468 0a20 2020  000ff"><path.   
-00003890: 2020 6964 3d22 7061 7468 3738 220a 2020    id="path78".  
-000038a0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-000038b0: 3030 3030 6666 3b73 7472 6f6b 653a 2366  0000ff;stroke:#f
-000038c0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000038d0: 7468 3a30 2e33 3536 3b73 7472 6f6b 652d  th:0.356;stroke-
-000038e0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-000038f0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00003900: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00003910: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00003920: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00003930: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00003940: 2020 2020 643d 224d 2030 2c30 2056 202d      d="M 0,0 V -
-00003950: 392e 3837 3422 202f 3e3c 2f67 3e3c 670a  9.874" /></g><g.
-00003960: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00003970: 616e 736c 6174 6528 3734 312e 3738 3133  anslate(741.7813
-00003980: 2c35 3933 2e30 3233 3929 220a 2020 2069  ,593.0239)".   i
-00003990: 643d 2267 3830 220a 2020 2073 7479 6c65  d="g80".   style
-000039a0: 3d22 6669 6c6c 3a23 3030 3030 6666 223e  ="fill:#0000ff">
-000039b0: 3c70 6174 680a 2020 2020 2069 643d 2270  <path.     id="p
-000039c0: 6174 6838 3222 0a20 2020 2020 7374 796c  ath82".     styl
-000039d0: 653d 2266 696c 6c3a 2330 3030 3066 663b  e="fill:#0000ff;
-000039e0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-000039f0: 7472 6f6b 652d 7769 6474 683a 302e 3335  troke-width:0.35
-00003a00: 363b 7374 726f 6b65 2d6c 696e 6563 6170  6;stroke-linecap
-00003a10: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00003a20: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00003a30: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00003a40: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00003a50: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00003a60: 6369 7479 3a31 220a 2020 2020 2064 3d22  city:1".     d="
-00003a70: 4d20 302c 3020 5620 2d39 2e38 3734 2220  M 0,0 V -9.874" 
-00003a80: 2f3e 3c2f 673e 3c67 0a20 2020 7472 616e  /></g><g.   tran
-00003a90: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00003aa0: 2837 3436 2e36 3336 372c 3539 332e 3035  (746.6367,593.05
-00003ab0: 3537 2922 0a20 2020 6964 3d22 6738 3422  57)".   id="g84"
-00003ac0: 0a20 2020 7374 796c 653d 2266 696c 6c3a  .   style="fill:
-00003ad0: 2330 3030 3066 6622 3e3c 7061 7468 0a20  #0000ff"><path. 
-00003ae0: 2020 2020 6964 3d22 7061 7468 3836 220a      id="path86".
-00003af0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00003b00: 3a23 3030 3030 6666 3b73 7472 6f6b 653a  :#0000ff;stroke:
-00003b10: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00003b20: 6964 7468 3a30 2e33 3536 3b73 7472 6f6b  idth:0.356;strok
-00003b30: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00003b40: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00003b50: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00003b60: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00003b70: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00003b80: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00003b90: 0a20 2020 2020 643d 224d 2030 2c30 2056  .     d="M 0,0 V
-00003ba0: 202d 392e 3837 3422 202f 3e3c 2f67 3e3c   -9.874" /></g><
-00003bb0: 670a 2020 2074 7261 6e73 666f 726d 3d22  g.   transform="
-00003bc0: 7472 616e 736c 6174 6528 3735 312e 3438  translate(751.48
-00003bd0: 3933 2c35 3933 2e30 3233 3929 220a 2020  93,593.0239)".  
-00003be0: 2069 643d 2267 3838 220a 2020 2073 7479   id="g88".   sty
-00003bf0: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
-00003c00: 223e 3c70 6174 680a 2020 2020 2069 643d  "><path.     id=
-00003c10: 2270 6174 6839 3022 0a20 2020 2020 7374  "path90".     st
-00003c20: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
-00003c30: 663b 7374 726f 6b65 3a23 6666 6666 6666  f;stroke:#ffffff
-00003c40: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00003c50: 3335 363b 7374 726f 6b65 2d6c 696e 6563  356;stroke-linec
-00003c60: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00003c70: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00003c80: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00003c90: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00003ca0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00003cb0: 7061 6369 7479 3a31 220a 2020 2020 2064  pacity:1".     d
-00003cc0: 3d22 4d20 302c 3020 5620 2d39 2e38 3734  ="M 0,0 V -9.874
-00003cd0: 2220 2f3e 3c2f 673e 3c67 0a20 2020 7472  " /></g><g.   tr
-00003ce0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00003cf0: 7465 2837 3536 2e33 3431 382c 3539 332e  te(756.3418,593.
-00003d00: 3035 3537 2922 0a20 2020 6964 3d22 6739  0557)".   id="g9
-00003d10: 3222 0a20 2020 7374 796c 653d 2266 696c  2".   style="fil
-00003d20: 6c3a 2330 3030 3066 6622 3e3c 7061 7468  l:#0000ff"><path
-00003d30: 0a20 2020 2020 6964 3d22 7061 7468 3934  .     id="path94
-00003d40: 220a 2020 2020 2073 7479 6c65 3d22 6669  ".     style="fi
-00003d50: 6c6c 3a23 3030 3030 6666 3b73 7472 6f6b  ll:#0000ff;strok
-00003d60: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00003d70: 2d77 6964 7468 3a30 2e33 3536 3b73 7472  -width:0.356;str
-00003d80: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00003d90: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00003da0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-00003db0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00003dc0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00003dd0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00003de0: 3122 0a20 2020 2020 643d 224d 2030 2c30  1".     d="M 0,0
-00003df0: 2056 202d 392e 3837 3422 202f 3e3c 2f67   V -9.874" /></g
-00003e00: 3e3c 670a 2020 2074 7261 6e73 666f 726d  ><g.   transform
-00003e10: 3d22 7472 616e 736c 6174 6528 3736 312e  ="translate(761.
-00003e20: 3139 3533 2c35 3933 2e30 3233 3929 220a  1953,593.0239)".
-00003e30: 2020 2069 643d 2267 3936 220a 2020 2073     id="g96".   s
-00003e40: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
-00003e50: 6666 223e 3c70 6174 680a 2020 2020 2069  ff"><path.     i
-00003e60: 643d 2270 6174 6839 3822 0a20 2020 2020  d="path98".     
-00003e70: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00003e80: 3066 663b 7374 726f 6b65 3a23 6666 6666  0ff;stroke:#ffff
-00003e90: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00003ea0: 302e 3335 363b 7374 726f 6b65 2d6c 696e  0.356;stroke-lin
-00003eb0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00003ec0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00003ed0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00003ee0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00003ef0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00003f00: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00003f10: 2064 3d22 4d20 302c 3020 5620 2d39 2e38   d="M 0,0 V -9.8
-00003f20: 3734 2220 2f3e 3c2f 673e 3c67 0a20 2020  74" /></g><g.   
-00003f30: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00003f40: 6c61 7465 2837 3332 2e35 3239 332c 3538  late(732.5293,58
-00003f50: 382e 3032 3239 2922 0a20 2020 6964 3d22  8.0229)".   id="
-00003f60: 6731 3030 220a 2020 2073 7479 6c65 3d22  g100".   style="
-00003f70: 6669 6c6c 3a23 3030 3030 6666 223e 3c70  fill:#0000ff"><p
-00003f80: 6174 680a 2020 2020 2069 643d 2270 6174  ath.     id="pat
-00003f90: 6831 3032 220a 2020 2020 2073 7479 6c65  h102".     style
-00003fa0: 3d22 6669 6c6c 3a23 3030 3030 6666 3b73  ="fill:#0000ff;s
-00003fb0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00003fc0: 726f 6b65 2d77 6964 7468 3a30 2e33 3536  roke-width:0.356
-00003fd0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00003fe0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00003ff0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00004000: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00004010: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00004020: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00004030: 6974 793a 3122 0a20 2020 2020 643d 224d  ity:1".     d="M
-00004040: 2030 2c30 2033 332e 3533 392c 302e 3030   0,0 33.539,0.00
-00004050: 3822 202f 3e3c 2f67 3e3c 670a 2020 2069  8" /></g><g.   i
-00004060: 643d 2267 3130 3422 0a20 2020 7374 796c  d="g104".   styl
-00004070: 653d 2266 696c 6c3a 2330 3030 3066 6622  e="fill:#0000ff"
-00004080: 3e3c 670a 2020 2020 2063 6c69 702d 7061  ><g.     clip-pa
-00004090: 7468 3d22 7572 6c28 2363 6c69 7050 6174  th="url(#clipPat
-000040a0: 6831 3038 2922 0a20 2020 2020 6964 3d22  h108)".     id="
-000040b0: 6731 3036 220a 2020 2020 2073 7479 6c65  g106".     style
-000040c0: 3d22 6669 6c6c 3a23 3030 3030 6666 223e  ="fill:#0000ff">
-000040d0: 3c67 0a20 2020 2020 2020 7472 616e 7366  <g.       transf
-000040e0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2837  orm="translate(7
-000040f0: 3333 2e32 3430 322c 3539 302e 3439 3137  33.2402,590.4917
-00004100: 2922 0a20 2020 2020 2020 6964 3d22 6731  )".       id="g1
-00004110: 3132 220a 2020 2020 2020 2073 7479 6c65  12".       style
-00004120: 3d22 6669 6c6c 3a23 3030 3030 6666 223e  ="fill:#0000ff">
-00004130: 3c70 6174 680a 2020 2020 2020 2020 2069  <path.         i
-00004140: 643d 2270 6174 6831 3134 220a 2020 2020  d="path114".    
-00004150: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00004160: 3a23 3030 3030 6666 3b66 696c 6c2d 6f70  :#0000ff;fill-op
-00004170: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-00004180: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-00004190: 3a6e 6f6e 6522 0a20 2020 2020 2020 2020  :none".         
-000041a0: 643d 224d 2030 2c30 2043 2030 2c30 2e36  d="M 0,0 C 0,0.6
-000041b0: 3920 302e 3535 392c 312e 3235 3120 312e  9 0.559,1.251 1.
-000041c0: 3234 372c 312e 3235 3120 312e 3933 382c  247,1.251 1.938,
-000041d0: 312e 3235 3120 322e 3530 342c 302e 3639  1.251 2.504,0.69
-000041e0: 2032 2e35 3034 2c30 2032 2e35 3034 2c2d   2.504,0 2.504,-
-000041f0: 302e 3639 3120 312e 3933 382c 2d31 2e32  0.691 1.938,-1.2
-00004200: 3520 312e 3234 372c 2d31 2e32 3520 302e  5 1.247,-1.25 0.
-00004210: 3535 392c 2d31 2e32 3520 302c 2d30 2e36  559,-1.25 0,-0.6
-00004220: 3931 2030 2c30 2220 2f3e 3c2f 673e 3c67  91 0,0" /></g><g
-00004230: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-00004240: 6d3d 2274 7261 6e73 6c61 7465 2837 3333  m="translate(733
-00004250: 2e32 3039 2c35 3835 2e36 3033 3529 220a  .209,585.6035)".
-00004260: 2020 2020 2020 2069 643d 2267 3131 3622         id="g116"
-00004270: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00004280: 696c 6c3a 2330 3030 3066 6622 3e3c 7061  ill:#0000ff"><pa
-00004290: 7468 0a20 2020 2020 2020 2020 6964 3d22  th.         id="
-000042a0: 7061 7468 3131 3822 0a20 2020 2020 2020  path118".       
-000042b0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-000042c0: 3030 3066 663b 6669 6c6c 2d6f 7061 6369  000ff;fill-opaci
-000042d0: 7479 3a31 3b66 696c 6c2d 7275 6c65 3a6e  ty:1;fill-rule:n
-000042e0: 6f6e 7a65 726f 3b73 7472 6f6b 653a 6e6f  onzero;stroke:no
-000042f0: 6e65 220a 2020 2020 2020 2020 2064 3d22  ne".         d="
-00004300: 4d20 302c 3020 4320 302c 302e 3639 2030  M 0,0 C 0,0.69 0
-00004310: 2e35 3537 2c31 2e32 3438 2031 2e32 3436  .557,1.248 1.246
-00004320: 2c31 2e32 3438 2031 2e39 3338 2c31 2e32  ,1.248 1.938,1.2
-00004330: 3438 2032 2e35 3032 2c30 2e36 3920 322e  48 2.502,0.69 2.
-00004340: 3530 322c 3020 322e 3530 322c 2d30 2e36  502,0 2.502,-0.6
-00004350: 3932 2031 2e39 3338 2c2d 312e 3235 3120  92 1.938,-1.251 
-00004360: 312e 3234 362c 2d31 2e32 3531 2030 2e35  1.246,-1.251 0.5
-00004370: 3537 2c2d 312e 3235 3120 302c 2d30 2e36  57,-1.251 0,-0.6
-00004380: 3932 2030 2c30 2220 2f3e 3c2f 673e 3c67  92 0,0" /></g><g
-00004390: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-000043a0: 6d3d 2274 7261 6e73 6c61 7465 2837 3338  m="translate(738
-000043b0: 2e30 3333 322c 3539 302e 3439 3137 2922  .0332,590.4917)"
-000043c0: 0a20 2020 2020 2020 6964 3d22 6731 3230  .       id="g120
-000043d0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-000043e0: 6669 6c6c 3a23 3030 3030 6666 223e 3c70  fill:#0000ff"><p
-000043f0: 6174 680a 2020 2020 2020 2020 2069 643d  ath.         id=
-00004400: 2270 6174 6831 3232 220a 2020 2020 2020  "path122".      
-00004410: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00004420: 3030 3030 6666 3b66 696c 6c2d 6f70 6163  0000ff;fill-opac
-00004430: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-00004440: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
-00004450: 6f6e 6522 0a20 2020 2020 2020 2020 643d  one".         d=
-00004460: 224d 2030 2c30 2043 2030 2c30 2e36 3920  "M 0,0 C 0,0.69 
-00004470: 302e 3535 382c 312e 3235 3120 312e 3234  0.558,1.251 1.24
-00004480: 382c 312e 3235 3120 312e 3933 392c 312e  8,1.251 1.939,1.
-00004490: 3235 3120 322e 352c 302e 3639 2032 2e35  251 2.5,0.69 2.5
-000044a0: 2c30 2032 2e35 2c2d 302e 3639 3120 312e  ,0 2.5,-0.691 1.
-000044b0: 3933 392c 2d31 2e32 3520 312e 3234 382c  939,-1.25 1.248,
-000044c0: 2d31 2e32 3520 302e 3535 382c 2d31 2e32  -1.25 0.558,-1.2
-000044d0: 3520 302c 2d30 2e36 3931 2030 2c30 2220  5 0,-0.691 0,0" 
-000044e0: 2f3e 3c2f 673e 3c67 0a20 2020 2020 2020  /></g><g.       
-000044f0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00004500: 6c61 7465 2837 3338 2e30 3031 2c35 3835  late(738.001,585
-00004510: 2e36 3033 3529 220a 2020 2020 2020 2069  .6035)".       i
-00004520: 643d 2267 3132 3422 0a20 2020 2020 2020  d="g124".       
-00004530: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00004540: 3066 6622 3e3c 7061 7468 0a20 2020 2020  0ff"><path.     
-00004550: 2020 2020 6964 3d22 7061 7468 3132 3622      id="path126"
-00004560: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00004570: 2266 696c 6c3a 2330 3030 3066 663b 6669  "fill:#0000ff;fi
-00004580: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
-00004590: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
-000045a0: 7472 6f6b 653a 6e6f 6e65 220a 2020 2020  troke:none".    
-000045b0: 2020 2020 2064 3d22 4d20 302c 3020 4320       d="M 0,0 C 
-000045c0: 302c 302e 3639 2030 2e35 3538 2c31 2e32  0,0.69 0.558,1.2
-000045d0: 3438 2031 2e32 3437 2c31 2e32 3438 2031  48 1.247,1.248 1
-000045e0: 2e39 3338 2c31 2e32 3438 2032 2e35 3034  .938,1.248 2.504
-000045f0: 2c30 2e36 3920 322e 3530 342c 3020 322e  ,0.69 2.504,0 2.
-00004600: 3530 342c 2d30 2e36 3932 2031 2e39 3338  504,-0.692 1.938
-00004610: 2c2d 312e 3235 3120 312e 3234 372c 2d31  ,-1.251 1.247,-1
-00004620: 2e32 3531 2030 2e35 3538 2c2d 312e 3235  .251 0.558,-1.25
-00004630: 3120 302c 2d30 2e36 3932 2030 2c30 2220  1 0,-0.692 0,0" 
-00004640: 2f3e 3c2f 673e 3c67 0a20 2020 2020 2020  /></g><g.       
-00004650: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00004660: 6c61 7465 2837 3432 2e39 3439 322c 3539  late(742.9492,59
-00004670: 302e 3439 3137 2922 0a20 2020 2020 2020  0.4917)".       
-00004680: 6964 3d22 6731 3238 220a 2020 2020 2020  id="g128".      
-00004690: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
-000046a0: 3030 6666 223e 3c70 6174 680a 2020 2020  00ff"><path.    
-000046b0: 2020 2020 2069 643d 2270 6174 6831 3330       id="path130
-000046c0: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
-000046d0: 3d22 6669 6c6c 3a23 3030 3030 6666 3b66  ="fill:#0000ff;f
-000046e0: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
-000046f0: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
-00004700: 7374 726f 6b65 3a6e 6f6e 6522 0a20 2020  stroke:none".   
-00004710: 2020 2020 2020 643d 224d 2030 2c30 2043        d="M 0,0 C
-00004720: 2030 2c30 2e36 3920 302e 3535 372c 312e   0,0.69 0.557,1.
-00004730: 3235 3120 312e 3234 362c 312e 3235 3120  251 1.246,1.251 
-00004740: 312e 3933 382c 312e 3235 3120 322e 352c  1.938,1.251 2.5,
-00004750: 302e 3639 2032 2e35 2c30 2032 2e35 2c2d  0.69 2.5,0 2.5,-
-00004760: 302e 3639 3120 312e 3933 382c 2d31 2e32  0.691 1.938,-1.2
-00004770: 3520 312e 3234 362c 2d31 2e32 3520 302e  5 1.246,-1.25 0.
-00004780: 3535 372c 2d31 2e32 3520 302c 2d30 2e36  557,-1.25 0,-0.6
-00004790: 3931 2030 2c30 2220 2f3e 3c2f 673e 3c67  91 0,0" /></g><g
-000047a0: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-000047b0: 6d3d 2274 7261 6e73 6c61 7465 2837 3432  m="translate(742
-000047c0: 2e39 3136 2c35 3835 2e36 3033 3529 220a  .916,585.6035)".
-000047d0: 2020 2020 2020 2069 643d 2267 3133 3222         id="g132"
-000047e0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000047f0: 696c 6c3a 2330 3030 3066 6622 3e3c 7061  ill:#0000ff"><pa
-00004800: 7468 0a20 2020 2020 2020 2020 6964 3d22  th.         id="
-00004810: 7061 7468 3133 342d 3922 0a20 2020 2020  path134-9".     
-00004820: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00004830: 2330 3030 3066 663b 6669 6c6c 2d6f 7061  #0000ff;fill-opa
-00004840: 6369 7479 3a31 3b66 696c 6c2d 7275 6c65  city:1;fill-rule
-00004850: 3a6e 6f6e 7a65 726f 3b73 7472 6f6b 653a  :nonzero;stroke:
-00004860: 6e6f 6e65 220a 2020 2020 2020 2020 2064  none".         d
-00004870: 3d22 4d20 302c 3020 4320 302c 302e 3639  ="M 0,0 C 0,0.69
-00004880: 2030 2e35 3537 2c31 2e32 3438 2031 2e32   0.557,1.248 1.2
-00004890: 3436 2c31 2e32 3438 2031 2e39 3338 2c31  46,1.248 1.938,1
-000048a0: 2e32 3438 2032 2e35 2c30 2e36 3920 322e  .248 2.5,0.69 2.
-000048b0: 352c 3020 322e 352c 2d30 2e36 3932 2031  5,0 2.5,-0.692 1
-000048c0: 2e39 3338 2c2d 312e 3235 3120 312e 3234  .938,-1.251 1.24
-000048d0: 362c 2d31 2e32 3531 2030 2e35 3537 2c2d  6,-1.251 0.557,-
-000048e0: 312e 3235 3120 302c 2d30 2e36 3932 2030  1.251 0,-0.692 0
-000048f0: 2c30 2220 2f3e 3c2f 673e 3c67 0a20 2020  ,0" /></g><g.   
-00004900: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-00004910: 7261 6e73 6c61 7465 2837 3437 2e37 3339  ranslate(747.739
-00004920: 332c 3539 302e 3439 3137 2922 0a20 2020  3,590.4917)".   
-00004930: 2020 2020 6964 3d22 6731 3336 220a 2020      id="g136".  
-00004940: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00004950: 3a23 3030 3030 6666 223e 3c70 6174 680a  :#0000ff"><path.
-00004960: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00004970: 6831 3338 2d33 220a 2020 2020 2020 2020  h138-3".        
-00004980: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
-00004990: 3030 6666 3b66 696c 6c2d 6f70 6163 6974  00ff;fill-opacit
-000049a0: 793a 313b 6669 6c6c 2d72 756c 653a 6e6f  y:1;fill-rule:no
-000049b0: 6e7a 6572 6f3b 7374 726f 6b65 3a6e 6f6e  nzero;stroke:non
-000049c0: 6522 0a20 2020 2020 2020 2020 643d 224d  e".         d="M
-000049d0: 2030 2c30 2043 2030 2c30 2e36 3920 302e   0,0 C 0,0.69 0.
-000049e0: 3535 372c 312e 3235 3120 312e 3234 372c  557,1.251 1.247,
-000049f0: 312e 3235 3120 312e 3933 382c 312e 3235  1.251 1.938,1.25
-00004a00: 3120 322e 3530 322c 302e 3639 2032 2e35  1 2.502,0.69 2.5
-00004a10: 3032 2c30 2032 2e35 3032 2c2d 302e 3639  02,0 2.502,-0.69
-00004a20: 3120 312e 3933 382c 2d31 2e32 3520 312e  1 1.938,-1.25 1.
-00004a30: 3234 372c 2d31 2e32 3520 302e 3535 372c  247,-1.25 0.557,
-00004a40: 2d31 2e32 3520 302c 2d30 2e36 3931 2030  -1.25 0,-0.691 0
-00004a50: 2c30 2220 2f3e 3c2f 673e 3c67 0a20 2020  ,0" /></g><g.   
-00004a60: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-00004a70: 7261 6e73 6c61 7465 2837 3437 2e37 3036  ranslate(747.706
-00004a80: 312c 3538 352e 3630 3335 2922 0a20 2020  1,585.6035)".   
-00004a90: 2020 2020 6964 3d22 6731 3430 220a 2020      id="g140".  
-00004aa0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00004ab0: 3a23 3030 3030 6666 223e 3c70 6174 680a  :#0000ff"><path.
-00004ac0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00004ad0: 6831 3432 220a 2020 2020 2020 2020 2073  h142".         s
-00004ae0: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
-00004af0: 6666 3b66 696c 6c2d 6f70 6163 6974 793a  ff;fill-opacity:
-00004b00: 313b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  1;fill-rule:nonz
-00004b10: 6572 6f3b 7374 726f 6b65 3a6e 6f6e 6522  ero;stroke:none"
-00004b20: 0a20 2020 2020 2020 2020 643d 224d 2030  .         d="M 0
-00004b30: 2c30 2043 2030 2c30 2e36 3920 302e 3536  ,0 C 0,0.69 0.56
-00004b40: 2c31 2e32 3438 2031 2e32 3437 2c31 2e32  ,1.248 1.247,1.2
-00004b50: 3438 2031 2e39 3338 2c31 2e32 3438 2032  48 1.938,1.248 2
-00004b60: 2e35 3033 2c30 2e36 3920 322e 3530 332c  .503,0.69 2.503,
-00004b70: 3020 322e 3530 332c 2d30 2e36 3932 2031  0 2.503,-0.692 1
-00004b80: 2e39 3338 2c2d 312e 3235 3120 312e 3234  .938,-1.251 1.24
-00004b90: 372c 2d31 2e32 3531 2030 2e35 362c 2d31  7,-1.251 0.56,-1
-00004ba0: 2e32 3531 2030 2c2d 302e 3639 3220 302c  .251 0,-0.692 0,
-00004bb0: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
-00004bc0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00004bd0: 616e 736c 6174 6528 3735 322e 3635 3433  anslate(752.6543
-00004be0: 2c35 3930 2e34 3931 3729 220a 2020 2020  ,590.4917)".    
-00004bf0: 2020 2069 643d 2267 3134 342d 3822 0a20     id="g144-8". 
-00004c00: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00004c10: 6c3a 2330 3030 3066 6622 3e3c 7061 7468  l:#0000ff"><path
-00004c20: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00004c30: 7468 3134 3622 0a20 2020 2020 2020 2020  th146".         
-00004c40: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00004c50: 3066 663b 6669 6c6c 2d6f 7061 6369 7479  0ff;fill-opacity
-00004c60: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-00004c70: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-00004c80: 220a 2020 2020 2020 2020 2064 3d22 4d20  ".         d="M 
-00004c90: 302c 3020 4320 302c 302e 3639 2030 2e35  0,0 C 0,0.69 0.5
-00004ca0: 3537 2c31 2e32 3531 2031 2e32 3435 2c31  57,1.251 1.245,1
-00004cb0: 2e32 3531 2031 2e39 3338 2c31 2e32 3531  .251 1.938,1.251
-00004cc0: 2032 2e35 3032 2c30 2e36 3920 322e 3530   2.502,0.69 2.50
-00004cd0: 322c 3020 322e 3530 322c 2d30 2e36 3931  2,0 2.502,-0.691
-00004ce0: 2031 2e39 3338 2c2d 312e 3235 2031 2e32   1.938,-1.25 1.2
-00004cf0: 3435 2c2d 312e 3235 2030 2e35 3537 2c2d  45,-1.25 0.557,-
-00004d00: 312e 3235 2030 2c2d 302e 3639 3120 302c  1.25 0,-0.691 0,
-00004d10: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
-00004d20: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00004d30: 616e 736c 6174 6528 3735 322e 3632 3131  anslate(752.6211
-00004d40: 2c35 3835 2e36 3033 3529 220a 2020 2020  ,585.6035)".    
-00004d50: 2020 2069 643d 2267 3134 382d 3022 0a20     id="g148-0". 
-00004d60: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00004d70: 6c3a 2330 3030 3066 6622 3e3c 7061 7468  l:#0000ff"><path
-00004d80: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00004d90: 7468 3135 3022 0a20 2020 2020 2020 2020  th150".         
-00004da0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00004db0: 3066 663b 6669 6c6c 2d6f 7061 6369 7479  0ff;fill-opacity
-00004dc0: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-00004dd0: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-00004de0: 220a 2020 2020 2020 2020 2064 3d22 4d20  ".         d="M 
-00004df0: 302c 3020 4320 302c 302e 3639 2030 2e35  0,0 C 0,0.69 0.5
-00004e00: 3539 2c31 2e32 3438 2031 2e32 3436 2c31  59,1.248 1.246,1
-00004e10: 2e32 3438 2031 2e39 3339 2c31 2e32 3438  .248 1.939,1.248
-00004e20: 2032 2e35 3032 2c30 2e36 3920 322e 3530   2.502,0.69 2.50
-00004e30: 322c 3020 322e 3530 322c 2d30 2e36 3932  2,0 2.502,-0.692
-00004e40: 2031 2e39 3339 2c2d 312e 3235 3120 312e   1.939,-1.251 1.
-00004e50: 3234 362c 2d31 2e32 3531 2030 2e35 3539  246,-1.251 0.559
-00004e60: 2c2d 312e 3235 3120 302c 2d30 2e36 3932  ,-1.251 0,-0.692
-00004e70: 2030 2c30 2220 2f3e 3c2f 673e 3c67 0a20   0,0" /></g><g. 
-00004e80: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00004e90: 2274 7261 6e73 6c61 7465 2837 3537 2e34  "translate(757.4
-00004ea0: 3435 332c 3539 302e 3439 3137 2922 0a20  453,590.4917)". 
-00004eb0: 2020 2020 2020 6964 3d22 6731 3532 2d32        id="g152-2
-00004ec0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-00004ed0: 6669 6c6c 3a23 3030 3030 6666 223e 3c70  fill:#0000ff"><p
-00004ee0: 6174 680a 2020 2020 2020 2020 2069 643d  ath.         id=
-00004ef0: 2270 6174 6831 3534 220a 2020 2020 2020  "path154".      
-00004f00: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00004f10: 3030 3030 6666 3b66 696c 6c2d 6f70 6163  0000ff;fill-opac
-00004f20: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-00004f30: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
-00004f40: 6f6e 6522 0a20 2020 2020 2020 2020 643d  one".         d=
-00004f50: 224d 2030 2c30 2043 2030 2c30 2e36 3920  "M 0,0 C 0,0.69 
-00004f60: 302e 3535 392c 312e 3235 3120 312e 3234  0.559,1.251 1.24
-00004f70: 362c 312e 3235 3120 312e 3934 312c 312e  6,1.251 1.941,1.
-00004f80: 3235 3120 322e 3530 312c 302e 3639 2032  251 2.501,0.69 2
-00004f90: 2e35 3031 2c30 2032 2e35 3031 2c2d 302e  .501,0 2.501,-0.
-00004fa0: 3639 3120 312e 3934 312c 2d31 2e32 3520  691 1.941,-1.25 
-00004fb0: 312e 3234 362c 2d31 2e32 3520 302e 3535  1.246,-1.25 0.55
-00004fc0: 392c 2d31 2e32 3520 302c 2d30 2e36 3931  9,-1.25 0,-0.691
-00004fd0: 2030 2c30 2220 2f3e 3c2f 673e 3c67 0a20   0,0" /></g><g. 
-00004fe0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00004ff0: 2274 7261 6e73 6c61 7465 2837 3537 2e34  "translate(757.4
-00005000: 3136 2c35 3835 2e36 3033 3529 220a 2020  16,585.6035)".  
-00005010: 2020 2020 2069 643d 2267 3135 362d 3422       id="g156-4"
-00005020: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00005030: 696c 6c3a 2330 3030 3066 6622 3e3c 7061  ill:#0000ff"><pa
-00005040: 7468 0a20 2020 2020 2020 2020 6964 3d22  th.         id="
-00005050: 7061 7468 3135 3822 0a20 2020 2020 2020  path158".       
-00005060: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-00005070: 3030 3066 663b 6669 6c6c 2d6f 7061 6369  000ff;fill-opaci
-00005080: 7479 3a31 3b66 696c 6c2d 7275 6c65 3a6e  ty:1;fill-rule:n
-00005090: 6f6e 7a65 726f 3b73 7472 6f6b 653a 6e6f  onzero;stroke:no
-000050a0: 6e65 220a 2020 2020 2020 2020 2064 3d22  ne".         d="
-000050b0: 4d20 302c 3020 4320 302c 302e 3639 2030  M 0,0 C 0,0.69 0
-000050c0: 2e35 3537 2c31 2e32 3438 2031 2e32 3434  .557,1.248 1.244
-000050d0: 2c31 2e32 3438 2031 2e39 3337 2c31 2e32  ,1.248 1.937,1.2
-000050e0: 3438 2032 2e34 3939 2c30 2e36 3920 322e  48 2.499,0.69 2.
-000050f0: 3439 392c 3020 322e 3439 392c 2d30 2e36  499,0 2.499,-0.6
-00005100: 3932 2031 2e39 3337 2c2d 312e 3235 3120  92 1.937,-1.251 
-00005110: 312e 3234 342c 2d31 2e32 3531 2030 2e35  1.244,-1.251 0.5
-00005120: 3537 2c2d 312e 3235 3120 302c 2d30 2e36  57,-1.251 0,-0.6
-00005130: 3932 2030 2c30 2220 2f3e 3c2f 673e 3c67  92 0,0" /></g><g
-00005140: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-00005150: 6d3d 2274 7261 6e73 6c61 7465 2837 3632  m="translate(762
-00005160: 2e33 3630 342c 3539 302e 3439 3137 2922  .3604,590.4917)"
-00005170: 0a20 2020 2020 2020 6964 3d22 6731 3630  .       id="g160
-00005180: 2d38 220a 2020 2020 2020 2073 7479 6c65  -8".       style
-00005190: 3d22 6669 6c6c 3a23 3030 3030 6666 223e  ="fill:#0000ff">
-000051a0: 3c70 6174 680a 2020 2020 2020 2020 2069  <path.         i
-000051b0: 643d 2270 6174 6831 3632 220a 2020 2020  d="path162".    
-000051c0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000051d0: 3a23 3030 3030 6666 3b66 696c 6c2d 6f70  :#0000ff;fill-op
-000051e0: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-000051f0: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-00005200: 3a6e 6f6e 6522 0a20 2020 2020 2020 2020  :none".         
-00005210: 643d 224d 2030 2c30 2043 2030 2c30 2e36  d="M 0,0 C 0,0.6
-00005220: 3920 302e 3535 392c 312e 3235 3120 312e  9 0.559,1.251 1.
-00005230: 3234 372c 312e 3235 3120 312e 3934 2c31  247,1.251 1.94,1
-00005240: 2e32 3531 2032 2e35 3031 2c30 2e36 3920  .251 2.501,0.69 
-00005250: 322e 3530 312c 3020 322e 3530 312c 2d30  2.501,0 2.501,-0
-00005260: 2e36 3931 2031 2e39 342c 2d31 2e32 3520  .691 1.94,-1.25 
-00005270: 312e 3234 372c 2d31 2e32 3520 302e 3535  1.247,-1.25 0.55
-00005280: 392c 2d31 2e32 3520 302c 2d30 2e36 3931  9,-1.25 0,-0.691
-00005290: 2030 2c30 2220 2f3e 3c2f 673e 3c67 0a20   0,0" /></g><g. 
-000052a0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-000052b0: 2274 7261 6e73 6c61 7465 2837 3632 2e33  "translate(762.3
-000052c0: 3238 312c 3538 352e 3630 3335 2922 0a20  281,585.6035)". 
-000052d0: 2020 2020 2020 6964 3d22 6731 3634 2d33        id="g164-3
-000052e0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-000052f0: 6669 6c6c 3a23 3030 3030 6666 223e 3c70  fill:#0000ff"><p
-00005300: 6174 680a 2020 2020 2020 2020 2069 643d  ath.         id=
-00005310: 2270 6174 6831 3636 220a 2020 2020 2020  "path166".      
-00005320: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00005330: 3030 3030 6666 3b66 696c 6c2d 6f70 6163  0000ff;fill-opac
-00005340: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-00005350: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
-00005360: 6f6e 6522 0a20 2020 2020 2020 2020 643d  one".         d=
-00005370: 224d 2030 2c30 2043 2030 2c30 2e36 3920  "M 0,0 C 0,0.69 
-00005380: 302e 3535 372c 312e 3234 3820 312e 3234  0.557,1.248 1.24
-00005390: 362c 312e 3234 3820 312e 3934 2c31 2e32  6,1.248 1.94,1.2
-000053a0: 3438 2032 2e35 3032 2c30 2e36 3920 322e  48 2.502,0.69 2.
-000053b0: 3530 322c 3020 322e 3530 322c 2d30 2e36  502,0 2.502,-0.6
-000053c0: 3932 2031 2e39 342c 2d31 2e32 3531 2031  92 1.94,-1.251 1
-000053d0: 2e32 3436 2c2d 312e 3235 3120 302e 3535  .246,-1.251 0.55
-000053e0: 372c 2d31 2e32 3531 2030 2c2d 302e 3639  7,-1.251 0,-0.69
-000053f0: 3220 302c 3022 202f 3e3c 2f67 3e3c 2f67  2 0,0" /></g></g
-00005400: 3e3c 2f67 3e3c 670a 2020 2074 7261 6e73  ></g><g.   trans
-00005410: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00005420: 3731 322e 3434 3334 2c35 3834 2e35 3830  712.4434,584.580
-00005430: 3129 220a 2020 2069 643d 2267 3136 382d  1)".   id="g168-
-00005440: 3922 0a20 2020 7374 796c 653d 2266 696c  9".   style="fil
-00005450: 6c3a 2330 3030 3066 663b 7374 726f 6b65  l:#0000ff;stroke
-00005460: 3a23 3030 3030 6666 3b73 7472 6f6b 652d  :#0000ff;stroke-
-00005470: 6f70 6163 6974 793a 3122 3e3c 7061 7468  opacity:1"><path
-00005480: 0a20 2020 2020 6964 3d22 7061 7468 3137  .     id="path17
-00005490: 3022 0a20 2020 2020 7374 796c 653d 2266  0".     style="f
-000054a0: 696c 6c3a 2330 3030 3066 663b 7374 726f  ill:#0000ff;stro
-000054b0: 6b65 3a23 3030 3030 6666 3b73 7472 6f6b  ke:#0000ff;strok
-000054c0: 652d 7769 6474 683a 313b 7374 726f 6b65  e-width:1;stroke
-000054d0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-000054e0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-000054f0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-00005500: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00005510: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00005520: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00005530: 2020 2020 2064 3d22 4d20 302c 3020 4820       d="M 0,0 H 
-00005540: 2d37 332e 3433 3622 202f 3e3c 2f67 3e3c  -73.436" /></g><
-00005550: 670a 2020 2074 7261 6e73 666f 726d 3d22  g.   transform="
-00005560: 7472 616e 736c 6174 6528 3731 322e 3935  translate(712.95
-00005570: 3231 2c35 3931 2e35 3335 3229 220a 2020  21,591.5352)".  
-00005580: 2069 643d 2267 3137 322d 3022 0a20 2020   id="g172-0".   
-00005590: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-000055a0: 3066 663b 7374 726f 6b65 3a23 3030 3030  0ff;stroke:#0000
-000055b0: 6666 3b73 7472 6f6b 652d 6f70 6163 6974  ff;stroke-opacit
-000055c0: 793a 3122 3e3c 7061 7468 0a20 2020 2020  y:1"><path.     
-000055d0: 6964 3d22 7061 7468 3137 3422 0a20 2020  id="path174".   
-000055e0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-000055f0: 3030 3066 663b 7374 726f 6b65 3a23 3030  000ff;stroke:#00
-00005600: 3030 6666 3b73 7472 6f6b 652d 7769 6474  00ff;stroke-widt
-00005610: 683a 313b 7374 726f 6b65 2d6c 696e 6563  h:1;stroke-linec
-00005620: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00005630: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00005640: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00005650: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00005660: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00005670: 7061 6369 7479 3a31 220a 2020 2020 2064  pacity:1".     d
-00005680: 3d22 4d20 302c 3020 4820 2d37 332e 3934  ="M 0,0 H -73.94
-00005690: 3422 202f 3e3c 2f67 3e3c 670a 2020 2074  4" /></g><g.   t
-000056a0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-000056b0: 6174 6528 3731 322e 3434 3334 2c35 3837  ate(712.4434,587
-000056c0: 2e39 3131 3129 220a 2020 2069 643d 2267  .9111)".   id="g
-000056d0: 3137 3622 0a20 2020 7374 796c 653d 2266  176".   style="f
-000056e0: 696c 6c3a 2330 3030 3066 663b 7374 726f  ill:#0000ff;stro
-000056f0: 6b65 3a23 3030 3030 6666 3b73 7472 6f6b  ke:#0000ff;strok
-00005700: 652d 6f70 6163 6974 793a 3122 3e3c 7061  e-opacity:1"><pa
-00005710: 7468 0a20 2020 2020 6964 3d22 7061 7468  th.     id="path
-00005720: 3137 3822 0a20 2020 2020 7374 796c 653d  178".     style=
-00005730: 2266 696c 6c3a 2330 3030 3066 663b 7374  "fill:#0000ff;st
-00005740: 726f 6b65 3a23 3030 3030 6666 3b73 7472  roke:#0000ff;str
-00005750: 6f6b 652d 7769 6474 683a 313b 7374 726f  oke-width:1;stro
-00005760: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-00005770: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-00005780: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-00005790: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-000057a0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-000057b0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-000057c0: 220a 2020 2020 2064 3d22 4d20 302c 3020  ".     d="M 0,0 
-000057d0: 2d37 332e 3431 332c 302e 3038 3622 202f  -73.413,0.086" /
-000057e0: 3e3c 2f67 3e3c 7061 7468 0a20 2020 6964  ></g><path.   id
-000057f0: 3d22 7061 7468 3138 3022 0a20 2020 7374  ="path180".   st
-00005800: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
-00005810: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
-00005820: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-00005830: 726f 3b73 7472 6f6b 653a 6e6f 6e65 220a  ro;stroke:none".
-00005840: 2020 2064 3d22 6d20 3639 332e 3037 372c     d="m 693.077,
-00005850: 3538 362e 3034 3520 6820 392e 3838 3520  586.045 h 9.885 
-00005860: 7620 2d32 2e39 3320 6820 2d39 2e38 3835  v -2.93 h -9.885
-00005870: 207a 2220 2f3e 3c70 6174 680a 2020 2069   z" /><path.   i
-00005880: 643d 2270 6174 6831 3832 220a 2020 2073  d="path182".   s
-00005890: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
-000058a0: 6666 3b66 696c 6c2d 6f70 6163 6974 793a  ff;fill-opacity:
-000058b0: 313b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  1;fill-rule:nonz
-000058c0: 6572 6f3b 7374 726f 6b65 3a6e 6f6e 6522  ero;stroke:none"
-000058d0: 0a20 2020 643d 226d 2036 3737 2e30 3036  .   d="m 677.006
-000058e0: 2c35 3839 2e35 3235 2068 2039 2e38 3833  ,589.525 h 9.883
-000058f0: 2076 202d 322e 3933 2068 202d 392e 3838   v -2.93 h -9.88
-00005900: 3320 7a22 202f 3e3c 7061 7468 0a20 2020  3 z" /><path.   
-00005910: 6964 3d22 7061 7468 3138 3422 0a20 2020  id="path184".   
-00005920: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00005930: 3066 663b 6669 6c6c 2d6f 7061 6369 7479  0ff;fill-opacity
-00005940: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-00005950: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-00005960: 220a 2020 2064 3d22 6d20 3639 322e 3835  ".   d="m 692.85
-00005970: 352c 3539 332e 3232 3920 6820 392e 3838  5,593.229 h 9.88
-00005980: 3320 7620 2d32 2e39 3320 6820 2d39 2e38  3 v -2.93 h -9.8
-00005990: 3833 207a 2220 2f3e 3c2f 673e 3c2f 673e  83 z" /></g></g>
-000059a0: 3c2f 673e 0a3c 670a 2020 2069 643d 2267  </g>.<g.   id="g
-000059b0: 3134 3422 0a20 2020 7472 616e 7366 6f72  144".   transfor
-000059c0: 6d3d 2274 7261 6e73 6c61 7465 2831 332e  m="translate(13.
-000059d0: 3735 3739 3938 2c2d 322e 3437 3335 3435  757998,-2.473545
-000059e0: 3929 223e 0a3c 2f67 3e0a 3c67 0a20 2020  9)">.</g>.<g.   
-000059f0: 6964 3d22 6731 3436 220a 2020 2074 7261  id="g146".   tra
-00005a00: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00005a10: 6528 3133 2e37 3537 3939 382c 2d32 2e34  e(13.757998,-2.4
-00005a20: 3733 3534 3539 2922 3e0a 3c2f 673e 0a3c  735459)">.</g>.<
-00005a30: 670a 2020 2069 643d 2267 3134 3822 0a20  g.   id="g148". 
-00005a40: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
-00005a50: 6e73 6c61 7465 2831 332e 3735 3739 3938  nslate(13.757998
-00005a60: 2c2d 322e 3437 3335 3435 3929 223e 0a3c  ,-2.4735459)">.<
-00005a70: 2f67 3e0a 3c67 0a20 2020 6964 3d22 6731  /g>.<g.   id="g1
-00005a80: 3530 220a 2020 2074 7261 6e73 666f 726d  50".   transform
-00005a90: 3d22 7472 616e 736c 6174 6528 3133 2e37  ="translate(13.7
-00005aa0: 3537 3939 382c 2d32 2e34 3733 3534 3539  57998,-2.4735459
-00005ab0: 2922 3e0a 3c2f 673e 0a3c 670a 2020 2069  )">.</g>.<g.   i
-00005ac0: 643d 2267 3135 3222 0a20 2020 7472 616e  d="g152".   tran
-00005ad0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00005ae0: 2831 332e 3735 3739 3938 2c2d 322e 3437  (13.757998,-2.47
-00005af0: 3335 3435 3929 223e 0a3c 2f67 3e0a 3c67  35459)">.</g>.<g
-00005b00: 0a20 2020 6964 3d22 6731 3534 220a 2020  .   id="g154".  
-00005b10: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-00005b20: 736c 6174 6528 3133 2e37 3537 3939 382c  slate(13.757998,
-00005b30: 2d32 2e34 3733 3534 3539 2922 3e0a 3c2f  -2.4735459)">.</
-00005b40: 673e 0a3c 670a 2020 2069 643d 2267 3135  g>.<g.   id="g15
-00005b50: 3622 0a20 2020 7472 616e 7366 6f72 6d3d  6".   transform=
-00005b60: 2274 7261 6e73 6c61 7465 2831 332e 3735  "translate(13.75
-00005b70: 3739 3938 2c2d 322e 3437 3335 3435 3929  7998,-2.4735459)
-00005b80: 223e 0a3c 2f67 3e0a 3c67 0a20 2020 6964  ">.</g>.<g.   id
-00005b90: 3d22 6731 3538 220a 2020 2074 7261 6e73  ="g158".   trans
-00005ba0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00005bb0: 3133 2e37 3537 3939 382c 2d32 2e34 3733  13.757998,-2.473
-00005bc0: 3534 3539 2922 3e0a 3c2f 673e 0a3c 670a  5459)">.</g>.<g.
-00005bd0: 2020 2069 643d 2267 3136 3022 0a20 2020     id="g160".   
-00005be0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00005bf0: 6c61 7465 2831 332e 3735 3739 3938 2c2d  late(13.757998,-
-00005c00: 322e 3437 3335 3435 3929 223e 0a3c 2f67  2.4735459)">.</g
-00005c10: 3e0a 3c67 0a20 2020 6964 3d22 6731 3632  >.<g.   id="g162
-00005c20: 220a 2020 2074 7261 6e73 666f 726d 3d22  ".   transform="
-00005c30: 7472 616e 736c 6174 6528 3133 2e37 3537  translate(13.757
-00005c40: 3939 382c 2d32 2e34 3733 3534 3539 2922  998,-2.4735459)"
-00005c50: 3e0a 3c2f 673e 0a3c 670a 2020 2069 643d  >.</g>.<g.   id=
-00005c60: 2267 3136 3422 0a20 2020 7472 616e 7366  "g164".   transf
-00005c70: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
-00005c80: 332e 3735 3739 3938 2c2d 322e 3437 3335  3.757998,-2.4735
-00005c90: 3435 3929 223e 0a3c 2f67 3e0a 3c67 0a20  459)">.</g>.<g. 
-00005ca0: 2020 6964 3d22 6731 3636 220a 2020 2074    id="g166".   t
-00005cb0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00005cc0: 6174 6528 3133 2e37 3537 3939 382c 2d32  ate(13.757998,-2
-00005cd0: 2e34 3733 3534 3539 2922 3e0a 3c2f 673e  .4735459)">.</g>
-00005ce0: 0a3c 670a 2020 2069 643d 2267 3136 3822  .<g.   id="g168"
-00005cf0: 0a20 2020 7472 616e 7366 6f72 6d3d 2274  .   transform="t
-00005d00: 7261 6e73 6c61 7465 2831 332e 3735 3739  ranslate(13.7579
-00005d10: 3938 2c2d 322e 3437 3335 3435 3929 223e  98,-2.4735459)">
-00005d20: 0a3c 2f67 3e0a 3c67 0a20 2020 6964 3d22  .</g>.<g.   id="
-00005d30: 6731 3730 220a 2020 2074 7261 6e73 666f  g170".   transfo
-00005d40: 726d 3d22 7472 616e 736c 6174 6528 3133  rm="translate(13
-00005d50: 2e37 3537 3939 382c 2d32 2e34 3733 3534  .757998,-2.47354
-00005d60: 3539 2922 3e0a 3c2f 673e 0a3c 670a 2020  59)">.</g>.<g.  
-00005d70: 2069 643d 2267 3137 3222 0a20 2020 7472   id="g172".   tr
-00005d80: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00005d90: 7465 2831 332e 3735 3739 3938 2c2d 322e  te(13.757998,-2.
-00005da0: 3437 3335 3435 3929 223e 0a3c 2f67 3e0a  4735459)">.</g>.
-00005db0: 3c2f 7376 673e 0a                        </svg>.
+00000150: 3a76 6572 7369 6f6e 3d22 312e 332e 3220  :version="1.3.2 
+00000160: 2830 3931 6532 3065 2c20 3230 3233 2d31  (091e20e, 2023-1
+00000170: 312d 3235 2922 0a20 2020 696e 6b73 6361  1-25)".   inksca
+00000180: 7065 3a65 7870 6f72 742d 6669 6c65 6e61  pe:export-filena
+00000190: 6d65 3d22 4954 6b44 422e 706e 6722 0a20  me="ITkDB.png". 
+000001a0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+000001b0: 742d 7864 7069 3d22 3936 220a 2020 2069  t-xdpi="96".   i
+000001c0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+000001d0: 6470 693d 2239 3622 0a20 2020 786d 6c6e  dpi="96".   xmln
+000001e0: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
+000001f0: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
+00000200: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
+00000210: 6e6b 7363 6170 6522 0a20 2020 786d 6c6e  nkscape".   xmln
+00000220: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
+00000230: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
+00000240: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
+00000250: 736f 6469 706f 6469 2d30 2e64 7464 220a  sodipodi-0.dtd".
+00000260: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
+00000270: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+00000280: 2f73 7667 220a 2020 2078 6d6c 6e73 3a73  /svg".   xmlns:s
+00000290: 7667 3d22 6874 7470 3a2f 2f77 7777 2e77  vg="http://www.w
+000002a0: 332e 6f72 672f 3230 3030 2f73 7667 223e  3.org/2000/svg">
+000002b0: 3c64 6566 730a 2020 2069 643d 2264 6566  <defs.   id="def
+000002c0: 7331 3737 223e 3c63 6c69 7050 6174 680a  s177"><clipPath.
+000002d0: 2020 2020 2069 643d 2263 6c69 7050 6174       id="clipPat
+000002e0: 6831 3622 0a20 2020 2020 636c 6970 5061  h16".     clipPa
+000002f0: 7468 556e 6974 733d 2275 7365 7253 7061  thUnits="userSpa
+00000300: 6365 4f6e 5573 6522 3e3c 7061 7468 0a20  ceOnUse"><path. 
+00000310: 2020 2020 2020 6964 3d22 7061 7468 3138        id="path18
+00000320: 220a 2020 2020 2020 2064 3d22 4d20 302c  ".       d="M 0,
+00000330: 3631 3220 4820 3739 3220 5620 3020 4820  612 H 792 V 0 H 
+00000340: 3020 5a22 202f 3e3c 2f63 6c69 7050 6174  0 Z" /></clipPat
+00000350: 683e 3c63 6c69 7050 6174 680a 2020 2020  h><clipPath.    
+00000360: 2069 643d 2263 6c69 7050 6174 6834 3822   id="clipPath48"
+00000370: 0a20 2020 2020 636c 6970 5061 7468 556e  .     clipPathUn
+00000380: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
+00000390: 5573 6522 3e3c 7061 7468 0a20 2020 2020  Use"><path.     
+000003a0: 2020 6964 3d22 7061 7468 3530 220a 2020    id="path50".  
+000003b0: 2020 2020 2064 3d22 4d20 302c 3631 3220       d="M 0,612 
+000003c0: 4820 3739 3220 5620 3020 4820 3020 5a22  H 792 V 0 H 0 Z"
+000003d0: 202f 3e3c 2f63 6c69 7050 6174 683e 3c63   /></clipPath><c
+000003e0: 6c69 7050 6174 680a 2020 2020 2069 643d  lipPath.     id=
+000003f0: 2263 6c69 7050 6174 6831 3038 220a 2020  "clipPath108".  
+00000400: 2020 2063 6c69 7050 6174 6855 6e69 7473     clipPathUnits
+00000410: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
+00000420: 223e 3c70 6174 680a 2020 2020 2020 2069  "><path.       i
+00000430: 643d 2270 6174 6831 3130 220a 2020 2020  d="path110".    
+00000440: 2020 2064 3d22 4d20 302c 3631 3220 4820     d="M 0,612 H 
+00000450: 3739 3220 5620 3020 4820 3020 5a22 202f  792 V 0 H 0 Z" /
+00000460: 3e3c 2f63 6c69 7050 6174 683e 3c2f 6465  ></clipPath></de
+00000470: 6673 3e3c 736f 6469 706f 6469 3a6e 616d  fs><sodipodi:nam
+00000480: 6564 7669 6577 0a20 2020 6964 3d22 6e61  edview.   id="na
+00000490: 6d65 6476 6965 7731 3735 220a 2020 2070  medview175".   p
+000004a0: 6167 6563 6f6c 6f72 3d22 2366 6666 6666  agecolor="#fffff
+000004b0: 6622 0a20 2020 626f 7264 6572 636f 6c6f  f".   bordercolo
+000004c0: 723d 2223 3636 3636 3636 220a 2020 2062  r="#666666".   b
+000004d0: 6f72 6465 726f 7061 6369 7479 3d22 312e  orderopacity="1.
+000004e0: 3022 0a20 2020 696e 6b73 6361 7065 3a73  0".   inkscape:s
+000004f0: 686f 7770 6167 6573 6861 646f 773d 2232  howpageshadow="2
+00000500: 220a 2020 2069 6e6b 7363 6170 653a 7061  ".   inkscape:pa
+00000510: 6765 6f70 6163 6974 793d 2230 2e30 220a  geopacity="0.0".
+00000520: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
+00000530: 6368 6563 6b65 7262 6f61 7264 3d22 3022  checkerboard="0"
+00000540: 0a20 2020 696e 6b73 6361 7065 3a64 6573  .   inkscape:des
+00000550: 6b63 6f6c 6f72 3d22 2364 3164 3164 3122  kcolor="#d1d1d1"
+00000560: 0a20 2020 7368 6f77 6772 6964 3d22 6661  .   showgrid="fa
+00000570: 6c73 6522 0a20 2020 696e 6b73 6361 7065  lse".   inkscape
+00000580: 3a7a 6f6f 6d3d 2231 302e 3134 3330 3934  :zoom="10.143094
+00000590: 220a 2020 2069 6e6b 7363 6170 653a 6378  ".   inkscape:cx
+000005a0: 3d22 3338 2e37 3934 3836 3922 0a20 2020  ="38.794869".   
+000005b0: 696e 6b73 6361 7065 3a63 793d 2231 382e  inkscape:cy="18.
+000005c0: 3932 3931 3335 220a 2020 2069 6e6b 7363  929135".   inksc
+000005d0: 6170 653a 6375 7272 656e 742d 6c61 7965  ape:current-laye
+000005e0: 723d 2267 3935 3432 220a 2020 2069 6e6b  r="g9542".   ink
+000005f0: 7363 6170 653a 7769 6e64 6f77 2d77 6964  scape:window-wid
+00000600: 7468 3d22 3133 3638 220a 2020 2069 6e6b  th="1368".   ink
+00000610: 7363 6170 653a 7769 6e64 6f77 2d68 6569  scape:window-hei
+00000620: 6768 743d 2231 3038 3722 0a20 2020 696e  ght="1087".   in
+00000630: 6b73 6361 7065 3a77 696e 646f 772d 783d  kscape:window-x=
+00000640: 2230 220a 2020 2069 6e6b 7363 6170 653a  "0".   inkscape:
+00000650: 7769 6e64 6f77 2d79 3d22 3434 220a 2020  window-y="44".  
+00000660: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00000670: 2d6d 6178 696d 697a 6564 3d22 3022 202f  -maximized="0" /
+00000680: 3e0a 3c67 0a20 2020 6964 3d22 6731 3432  >.<g.   id="g142
+00000690: 220a 2020 2074 7261 6e73 666f 726d 3d22  ".   transform="
+000006a0: 7472 616e 736c 6174 6528 3134 2e38 3238  translate(14.828
+000006b0: 3734 392c 2d31 2e35 3734 3034 3539 2922  749,-1.5740459)"
+000006c0: 3e0a 090a 090a 090a 090a 090a 3c67 0a20  >...........<g. 
+000006d0: 2020 6964 3d22 6739 3534 3222 0a20 2020    id="g9542".   
+000006e0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+000006f0: 6c61 7465 2832 2e35 3734 352c 322e 3437  late(2.5745,2.47
+00000700: 3335 3435 3929 223e 3c67 0a20 2020 2020  35459)"><g.     
+00000710: 6964 3d22 6739 3636 3222 3e3c 7061 7468  id="g9662"><path
+00000720: 0a20 2020 2020 2020 643d 226d 2035 322e  .       d="m 52.
+00000730: 3532 342c 3435 2e35 3337 2063 202d 302e  524,45.537 c -0.
+00000740: 3432 392c 2d34 2e31 3037 202d 332e 3835  429,-4.107 -3.85
+00000750: 322c 2d37 2e33 3332 202d 372e 3935 332c  2,-7.332 -7.953,
+00000760: 2d37 2e33 3332 202d 322e 3536 342c 3020  -7.332 -2.564,0 
+00000770: 2d34 2e39 3834 2c31 2e32 3836 202d 362e  -4.984,1.286 -6.
+00000780: 3438 2c33 2e34 3032 202d 302e 3239 312c  48,3.402 -0.291,
+00000790: 2d30 2e30 3531 202d 302e 3538 362c 2d30  -0.051 -0.586,-0
+000007a0: 2e30 3736 202d 302e 3838 332c 2d30 2e30  .076 -0.883,-0.0
+000007b0: 3736 202d 322e 3332 2c30 202d 342e 3338  76 -2.32,0 -4.38
+000007c0: 312c 312e 3537 3720 2d35 2e30 3636 2c33  1,1.577 -5.066,3
+000007d0: 2e38 3133 202d 312e 3930 372c 312e 3133  .813 -1.907,1.13
+000007e0: 3120 2d33 2e31 3136 2c33 2e32 3431 202d  1 -3.116,3.241 -
+000007f0: 332e 3131 362c 352e 3530 3220 302c 332e  3.116,5.502 0,3.
+00000800: 3530 3720 322e 3738 352c 362e 3335 3920  507 2.785,6.359 
+00000810: 362e 3230 382c 362e 3335 3920 6820 3130  6.208,6.359 h 10
+00000820: 2e37 3734 2063 2030 2e30 362c 3020 302e  .774 c 0.06,0 0.
+00000830: 3131 382c 2d30 2e30 3034 2030 2e31 3731  118,-0.004 0.171
+00000840: 2c2d 302e 3030 3820 302e 3036 322c 302e  ,-0.008 0.062,0.
+00000850: 3030 3420 302e 3132 342c 302e 3030 3820  004 0.124,0.008 
+00000860: 302e 3138 382c 302e 3030 3820 6820 342e  0.188,0.008 h 4.
+00000870: 3331 2063 2033 2e32 3235 2c30 2035 2e38  31 c 3.225,0 5.8
+00000880: 3439 2c2d 322e 3638 3720 352e 3834 392c  49,-2.687 5.849,
+00000890: 2d35 2e39 3839 202d 302e 3030 312c 2d32  -5.989 -0.001,-2
+000008a0: 2e36 202d 312e 3634 322c 2d34 2e38 3734  .6 -1.642,-4.874
+000008b0: 202d 342e 3030 322c 2d35 2e36 3739 207a   -4.002,-5.679 z
+000008c0: 206d 202d 312e 3834 372c 392e 3636 3820   m -1.847,9.668 
+000008d0: 2d34 2e33 3532 2c2d 302e 3030 3320 2d30  -4.352,-0.003 -0
+000008e0: 2e31 372c 2d30 2e30 3036 202d 3130 2e39  .17,-0.006 -10.9
+000008f0: 3232 2c30 2e30 3039 2063 202d 322e 3332  22,0.009 c -2.32
+00000900: 2c30 202d 342e 3230 382c 2d31 2e39 3536  ,0 -4.208,-1.956
+00000910: 202d 342e 3230 382c 2d34 2e33 3539 2030   -4.208,-4.359 0
+00000920: 2c2d 312e 3636 3520 302e 3934 392c 2d33  ,-1.665 0.949,-3
+00000930: 2e32 3120 322e 3431 372c 2d33 2e39 3335  .21 2.417,-3.935
+00000940: 206c 2030 2e34 3335 2c2d 302e 3231 3420   l 0.435,-0.214 
+00000950: 302e 3130 322c 2d30 2e34 3735 2063 2030  0.102,-0.475 c 0
+00000960: 2e33 3331 2c2d 312e 3536 2031 2e36 3839  .331,-1.56 1.689
+00000970: 2c2d 322e 3639 3120 332e 3232 392c 2d32  ,-2.691 3.229,-2
+00000980: 2e36 3931 2030 2e33 3435 2c30 2030 2e36  .691 0.345,0 0.6
+00000990: 3838 2c30 2e30 3537 2031 2e30 322c 302e  88,0.057 1.02,0.
+000009a0: 3136 3820 6c20 302e 3737 372c 302e 3236  168 l 0.777,0.26
+000009b0: 3120 302e 3430 382c 2d30 2e37 3131 2063  1 0.408,-0.711 c
+000009c0: 2031 2e30 3936 2c2d 312e 3930 3620 332e   1.096,-1.906 3.
+000009d0: 3032 342c 2d33 2e30 3434 2035 2e31 3538  024,-3.044 5.158
+000009e0: 2c2d 332e 3034 3420 332e 3236 352c 3020  ,-3.044 3.265,0 
+000009f0: 352e 3935 352c 322e 3734 3720 352e 3939  5.955,2.747 5.99
+00000a00: 382c 362e 3132 3320 6c20 302e 3031 312c  8,6.123 l 0.011,
+00000a10: 302e 3831 3320 302e 3739 392c 302e 3135  0.813 0.799,0.15
+00000a20: 3520 6320 312e 3832 332c 302e 3335 3420  5 c 1.823,0.354 
+00000a30: 332e 3134 362c 322e 3030 3220 332e 3134  3.146,2.002 3.14
+00000a40: 362c 332e 3931 3920 302c 322e 3220 2d31  6,3.919 0,2.2 -1
+00000a50: 2e37 3236 2c33 2e39 3920 2d33 2e38 3438  .726,3.99 -3.848
+00000a60: 2c33 2e39 3920 7a22 0a20 2020 2020 2020  ,3.99 z".       
+00000a70: 6964 3d22 7061 7468 3133 3222 202f 3e3c  id="path132" /><
+00000a80: 7061 7468 0a20 2020 2020 2020 643d 226d  path.       d="m
+00000a90: 2032 392e 3837 352c 3433 2e30 3434 2063   29.875,43.044 c
+00000aa0: 2031 2e33 3633 2c2d 322e 3631 3820 332e   1.363,-2.618 3.
+00000ab0: 3936 2c2d 342e 3333 3720 362e 3837 322c  96,-4.337 6.872,
+00000ac0: 2d34 2e35 2032 2e30 3636 2c2d 322e 3132  -4.5 2.066,-2.12
+00000ad0: 3720 342e 3839 342c 2d33 2e33 3339 2037  7 4.894,-3.339 7
+00000ae0: 2e38 3234 2c2d 332e 3333 3920 322e 3533  .824,-3.339 2.53
+00000af0: 312c 3020 342e 3931 362c 302e 3931 3620  1,0 4.916,0.916 
+00000b00: 362e 3831 382c 322e 3435 3520 302e 3039  6.818,2.455 0.09
+00000b10: 352c 2d30 2e30 3837 2030 2e32 3033 2c2d  5,-0.087 0.203,-
+00000b20: 302e 3137 3320 302e 3238 372c 2d30 2e32  0.173 0.287,-0.2
+00000b30: 3620 7620 2d31 2e32 3839 202d 302e 3520  6 v -1.289 -0.5 
+00000b40: 2d30 2e35 2056 2032 3820 6320 2d31 2e33  -0.5 V 28 c -1.3
+00000b50: 3138 2c30 2e39 3035 202d 332e 3032 382c  18,0.905 -3.028,
+00000b60: 312e 3639 3720 2d35 2e30 3235 2c32 2e33  1.697 -5.025,2.3
+00000b70: 3637 202d 342e 3231 2c31 2e34 3732 202d  67 -4.21,1.472 -
+00000b80: 3130 2e30 3438 2c32 2e35 3032 202d 3137  10.048,2.502 -17
+00000b90: 2e33 3639 2c32 2e37 3033 202d 302e 3837  .369,2.703 -0.87
+00000ba0: 2c30 2e30 3237 202d 312e 3734 2c30 2e30  ,0.027 -1.74,0.0
+00000bb0: 3431 202d 322e 3630 362c 302e 3034 3120  41 -2.606,0.041 
+00000bc0: 2d30 2e38 3639 2c30 202d 312e 3734 322c  -0.869,0 -1.742,
+00000bd0: 2d30 2e30 3134 202d 322e 3631 342c 2d30  -0.014 -2.614,-0
+00000be0: 2e30 3432 2043 2031 362e 3732 312c 3332  .042 C 16.721,32
+00000bf0: 2e38 3638 2031 302e 3837 312c 3331 2e38  .868 10.871,31.8
+00000c00: 3331 2036 2e36 3539 2c33 302e 3335 3220  31 6.659,30.352 
+00000c10: 342e 3638 2c32 392e 3638 3520 322e 3938  4.68,29.685 2.98
+00000c20: 342c 3238 2e38 3939 2031 2e36 3736 2c32  4,28.899 1.676,2
+00000c30: 3820 7620 372e 3131 3120 302e 3520 302e  8 v 7.111 0.5 0.
+00000c40: 3520 312e 3238 3920 6320 322e 3834 362c  5 1.289 c 2.846,
+00000c50: 322e 3937 3120 3132 2e33 3934 2c35 2e37  2.971 12.394,5.7
+00000c60: 3131 2032 352c 352e 3731 3120 312e 3039  11 25,5.711 1.09
+00000c70: 332c 3020 322e 3135 342c 2d30 2e30 3238  3,0 2.154,-0.028
+00000c80: 2033 2e31 3939 2c2d 302e 3036 3720 7a22   3.199,-0.067 z"
+00000c90: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00000ca0: 3133 3422 202f 3e3c 7061 7468 0a20 2020  134" /><path.   
+00000cb0: 2020 2020 643d 226d 2032 342e 3331 312c      d="m 24.311,
+00000cc0: 3239 2e39 3635 2063 2030 2e33 3236 2c30  29.965 c 0.326,0
+00000cd0: 2e30 3039 2030 2e36 3531 2c30 2e30 3138  .009 0.651,0.018
+00000ce0: 2030 2e39 3832 2c30 2e30 3233 2030 2e34   0.982,0.023 0.4
+00000cf0: 3536 2c30 2e30 3038 2030 2e39 3137 2c30  56,0.008 0.917,0
+00000d00: 2e30 3132 2031 2e33 3833 2c30 2e30 3132  .012 1.383,0.012
+00000d10: 2030 2e34 3636 2c30 2030 2e39 3236 2c2d   0.466,0 0.926,-
+00000d20: 302e 3030 3420 312e 3338 332c 2d30 2e30  0.004 1.383,-0.0
+00000d30: 3131 2030 2e33 332c 2d30 2e30 3035 2030  11 0.33,-0.005 0
+00000d40: 2e36 3536 2c2d 302e 3031 3520 302e 3938  .656,-0.015 0.98
+00000d50: 322c 2d30 2e30 3233 2030 2e31 3136 2c2d  2,-0.023 0.116,-
+00000d60: 302e 3030 3320 302e 3233 342c 2d30 2e30  0.003 0.234,-0.0
+00000d70: 3035 2030 2e33 3439 2c2d 302e 3030 3820  05 0.349,-0.008 
+00000d80: 3131 2e32 3533 2c2d 302e 3335 3920 3139  11.253,-0.359 19
+00000d90: 2e36 3438 2c2d 322e 3931 3520 3232 2e32  .648,-2.915 22.2
+00000da0: 3836 2c2d 352e 3636 3820 5620 3233 2032  86,-5.668 V 23 2
+00000db0: 322e 3520 3232 2031 342e 3838 3920 4320  2.5 22 14.889 C 
+00000dc0: 3436 2e38 3038 2c31 382e 3233 3220 3336  46.808,18.232 36
+00000dd0: 2e35 322c 3230 2032 362e 3637 362c 3230  .52,20 26.676,20
+00000de0: 2031 362e 3833 322c 3230 2036 2e35 3433   16.832,20 6.543
+00000df0: 2c31 382e 3233 3220 312e 3637 362c 3134  ,18.232 1.676,14
+00000e00: 2e38 3839 2056 2032 3220 3232 2e35 2032  .889 V 22 22.5 2
+00000e10: 3320 3234 2e32 3839 2063 2032 2e36 3338  3 24.289 c 2.638
+00000e20: 2c32 2e37 3534 2031 312e 3033 332c 352e  ,2.754 11.033,5.
+00000e30: 3331 2032 322e 3238 362c 352e 3636 3820  31 22.286,5.668 
+00000e40: 302e 3131 352c 302e 3030 3320 302e 3233  0.115,0.003 0.23
+00000e50: 332c 302e 3030 3520 302e 3334 392c 302e  3,0.005 0.349,0.
+00000e60: 3030 3820 7a22 0a20 2020 2020 2020 6964  008 z".       id
+00000e70: 3d22 7061 7468 3133 3622 202f 3e3c 7061  ="path136" /><pa
+00000e80: 7468 0a20 2020 2020 2020 643d 224d 2035  th.       d="M 5
+00000e90: 312e 3637 362c 3131 2e33 3036 2056 2039  1.676,11.306 V 9
+00000ea0: 2e35 2039 2043 2035 312e 3637 362c 382e  .5 9 C 51.676,8.
+00000eb0: 3833 3220 3531 2e36 322c 382e 3638 3120  832 51.62,8.681 
+00000ec0: 3531 2e35 3431 2c38 2e35 3432 2035 302e  51.541,8.542 50.
+00000ed0: 3431 382c 342e 3234 3120 3431 2e37 3931  418,4.241 41.791
+00000ee0: 2c30 2032 362e 3637 362c 3020 3131 2e35  ,0 26.676,0 11.5
+00000ef0: 3938 2c30 2032 2e39 3739 2c34 2e32 3220  98,0 2.979,4.22 
+00000f00: 312e 3832 322c 382e 3531 2031 2e37 3337  1.822,8.51 1.737
+00000f10: 2c38 2e36 3537 2031 2e36 3736 2c38 2e38  ,8.657 1.676,8.8
+00000f20: 3138 2031 2e36 3736 2c39 2076 2030 2e35  18 1.676,9 v 0.5
+00000f30: 2031 2e38 3036 2063 2032 2e38 3336 2c32   1.806 c 2.836,2
+00000f40: 2e39 3631 2031 322e 3331 362c 352e 3639  .961 12.316,5.69
+00000f50: 3420 3235 2c35 2e36 3934 2031 322e 3638  4 25,5.694 12.68
+00000f60: 342c 3020 3232 2e31 3633 2c2d 322e 3733  4,0 22.163,-2.73
+00000f70: 3320 3235 2c2d 352e 3639 3420 7a22 0a20  3 25,-5.694 z". 
+00000f80: 2020 2020 2020 6964 3d22 7061 7468 3133        id="path13
+00000f90: 3822 202f 3e3c 7061 7468 0a20 2020 2020  8" /><path.     
+00000fa0: 2020 643d 226d 2032 362e 3032 352c 3530    d="m 26.025,50
+00000fb0: 2e38 3435 2063 2030 2c2d 312e 3635 3220  .845 c 0,-1.652 
+00000fc0: 302e 3435 312c 2d33 2e32 3439 2031 2e32  0.451,-3.249 1.2
+00000fd0: 3439 2c2d 342e 3635 3120 2d30 2e32 3031  49,-4.651 -0.201
+00000fe0: 2c31 3065 2d34 202d 302e 3339 352c 302e  ,10e-4 -0.395,0.
+00000ff0: 3030 3720 2d30 2e35 3939 2c30 2e30 3037  007 -0.599,0.007
+00001000: 202d 3132 2e33 3436 2c30 202d 3230 2e38   -12.346,0 -20.8
+00001010: 3636 2c2d 322e 3239 202d 3235 2c2d 352e  66,-2.29 -25,-5.
+00001020: 3230 3120 7620 382e 3230 3120 6320 302c  201 v 8.201 c 0,
+00001030: 302e 3136 3220 302e 3034 332c 302e 3331  0.162 0.043,0.31
+00001040: 3520 302e 3131 372c 302e 3435 3120 312e  5 0.117,0.451 1.
+00001050: 3138 312c 342e 3839 3520 3131 2e37 3437  181,4.895 11.747
+00001060: 2c38 2e35 3439 2032 342e 3838 332c 382e  ,8.549 24.883,8.
+00001070: 3534 3920 302e 3935 2c30 2031 2e38 3831  549 0.95,0 1.881
+00001080: 2c2d 302e 3032 3420 322e 3830 312c 2d30  ,-0.024 2.801,-0
+00001090: 2e30 3632 202d 322e 312c 2d31 2e37 3137  .062 -2.1,-1.717
+000010a0: 202d 332e 3435 312c 2d34 2e33 3437 202d   -3.451,-4.347 -
+000010b0: 332e 3435 312c 2d37 2e32 3934 207a 220a  3.451,-7.294 z".
+000010c0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000010d0: 3430 2220 2f3e 3c2f 673e 3c67 0a20 2020  40" /></g><g.   
+000010e0: 2020 7472 616e 7366 6f72 6d3d 226d 6174    transform="mat
+000010f0: 7269 7828 302c 2d30 2e34 3130 3138 3933  rix(0,-0.4101893
+00001100: 322c 2d30 2e33 3933 3133 3534 322c 302c  2,-0.39313542,0,
+00001110: 3231 382e 3836 3537 362c 3331 382e 3139  218.86576,318.19
+00001120: 3134 3429 220a 2020 2020 2069 643d 2267  144)".     id="g
+00001130: 3130 220a 2020 2020 2073 7479 6c65 3d22  10".     style="
+00001140: 6669 6c6c 3a23 3030 3030 6666 223e 3c67  fill:#0000ff"><g
+00001150: 0a20 2020 6964 3d22 6731 3222 0a20 2020  .   id="g12".   
+00001160: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00001170: 3066 6622 3e3c 670a 2020 2020 2063 6c69  0ff"><g.     cli
+00001180: 702d 7061 7468 3d22 7572 6c28 2363 6c69  p-path="url(#cli
+00001190: 7050 6174 6831 3629 220a 2020 2020 2069  pPath16)".     i
+000011a0: 643d 2267 3134 220a 2020 2020 2073 7479  d="g14".     sty
+000011b0: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
+000011c0: 223e 3c67 0a20 2020 2020 2020 7472 616e  "><g.       tran
+000011d0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+000011e0: 2837 3038 2e33 3034 372c 3536 362e 3037  (708.3047,566.07
+000011f0: 3532 2922 0a20 2020 2020 2020 6964 3d22  52)".       id="
+00001200: 6732 3022 0a20 2020 2020 2020 7374 796c  g20".       styl
+00001210: 653d 2266 696c 6c3a 2330 3030 3066 6622  e="fill:#0000ff"
+00001220: 3e3c 7061 7468 0a20 2020 2020 2020 2020  ><path.         
+00001230: 6964 3d22 7061 7468 3232 220a 2020 2020  id="path22".    
+00001240: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00001250: 3a23 3030 3030 6666 3b66 696c 6c2d 6f70  :#0000ff;fill-op
+00001260: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
+00001270: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
+00001280: 3a6e 6f6e 6522 0a20 2020 2020 2020 2020  :none".         
+00001290: 643d 226d 2030 2c30 2063 2030 2e30 3432  d="m 0,0 c 0.042
+000012a0: 2c2d 312e 3532 3320 2d30 2e34 3737 2c2d  ,-1.523 -0.477,-
+000012b0: 322e 3736 3220 2d31 2e35 3532 2c2d 332e  2.762 -1.552,-3.
+000012c0: 3731 202d 312e 3037 372c 2d30 2e39 3437  71 -1.077,-0.947
+000012d0: 202d 322e 3539 352c 2d31 2e34 3833 202d   -2.595,-1.483 -
+000012e0: 342e 3536 2c2d 312e 3630 3620 2d31 2e38  4.56,-1.606 -1.8
+000012f0: 3038 2c2d 302e 3131 3620 2d33 2e34 3134  08,-0.116 -3.414
+00001300: 2c30 2e31 3235 202d 342e 3832 342c 302e  ,0.125 -4.824,0.
+00001310: 3731 3420 6c20 2d30 2e30 392c 332e 3333  714 l -0.09,3.33
+00001320: 3120 6320 312e 3135 372c 2d30 2e34 3339  1 c 1.157,-0.439
+00001330: 2032 2e31 3334 2c2d 302e 3733 3520 322e   2.134,-0.735 2.
+00001340: 3933 2c2d 302e 3839 3320 302e 3739 392c  93,-0.893 0.799,
+00001350: 2d30 2e31 3538 2031 2e35 3237 2c2d 302e  -0.158 1.527,-0.
+00001360: 3231 3720 322e 3138 332c 2d30 2e31 3736  217 2.183,-0.176
+00001370: 2030 2e37 3838 2c30 2e30 3531 2031 2e33   0.788,0.051 1.3
+00001380: 392c 302e 3234 2031 2e38 3031 2c30 2e35  9,0.24 1.801,0.5
+00001390: 3633 2030 2e34 3132 2c30 2e33 3239 2030  63 0.412,0.329 0
+000013a0: 2e36 312c 302e 3739 2030 2e35 3935 2c31  .61,0.79 0.595,1
+000013b0: 2e33 3832 202d 302e 3031 2c30 2e33 3332  .382 -0.01,0.332
+000013c0: 202d 302e 3131 2c30 2e36 3233 202d 302e   -0.11,0.623 -0.
+000013d0: 3330 312c 302e 3836 3820 2d30 2e31 3934  301,0.868 -0.194
+000013e0: 2c30 2e32 3436 202d 302e 3437 342c 302e  ,0.246 -0.474,0.
+000013f0: 3437 3820 2d30 2e38 3338 2c30 2e36 3935  478 -0.838,0.695
+00001400: 202d 302e 3336 372c 302e 3231 3520 2d31   -0.367,0.215 -1
+00001410: 2e31 3039 2c30 2e35 3531 202d 322e 3233  .109,0.551 -2.23
+00001420: 2c31 2e30 3034 202d 312e 3034 372c 302e  ,1.004 -1.047,0.
+00001430: 3432 3420 2d31 2e38 3336 2c30 2e38 3420  424 -1.836,0.84 
+00001440: 2d32 2e33 3635 2c31 2e32 3534 202d 302e  -2.365,1.254 -0.
+00001450: 3533 2c30 2e34 3135 202d 302e 3935 392c  53,0.415 -0.959,
+00001460: 302e 3930 3920 2d31 2e32 3832 2c31 2e34  0.909 -1.282,1.4
+00001470: 3833 202d 302e 3332 352c 302e 3537 3120  83 -0.325,0.571 
+00001480: 2d30 2e35 2c31 2e32 3537 202d 302e 3532  -0.5,1.257 -0.52
+00001490: 322c 322e 3035 3220 2d30 2e30 3431 2c31  2,2.052 -0.041,1
+000014a0: 2e34 3933 2030 2e34 3337 2c32 2e37 3031  .493 0.437,2.701
+000014b0: 2031 2e34 3237 2c33 2e36 3220 302e 3939   1.427,3.62 0.99
+000014c0: 332c 302e 3931 3920 322e 3338 362c 312e  3,0.919 2.386,1.
+000014d0: 3433 3520 342e 3137 372c 312e 3535 2030  435 4.177,1.55 0
+000014e0: 2e38 3831 2c30 2e30 3535 2031 2e37 3232  .881,0.055 1.722
+000014f0: 2c30 2e30 3035 2032 2e35 3238 2c2d 302e  ,0.005 2.528,-0.
+00001500: 3135 3320 302e 3830 372c 2d30 2e31 3538  153 0.807,-0.158
+00001510: 2031 2e36 3439 2c2d 302e 3420 322e 3533   1.649,-0.4 2.53
+00001520: 352c 2d30 2e37 3231 204c 202d 312e 3437  5,-0.721 L -1.47
+00001530: 322c 382e 3339 3620 4320 2d32 2e33 3835  2,8.396 C -2.385
+00001540: 2c38 2e37 3132 202d 332e 3133 392c 382e  ,8.712 -3.139,8.
+00001550: 3932 3220 2d33 2e37 3334 2c39 2e30 3331  922 -3.734,9.031
+00001560: 202d 342e 3332 392c 392e 3134 202d 342e   -4.329,9.14 -4.
+00001570: 3931 312c 392e 3137 3820 2d35 2e34 3834  911,9.178 -5.484
+00001580: 2c39 2e31 3420 2d36 2e31 3635 2c39 2e30  ,9.14 -6.165,9.0
+00001590: 3938 202d 362e 3638 322c 382e 3930 3820  98 -6.682,8.908 
+000015a0: 2d37 2e30 3336 2c38 2e35 3637 202d 372e  -7.036,8.567 -7.
+000015b0: 3339 322c 382e 3232 3920 2d37 2e35 3631  392,8.229 -7.561
+000015c0: 2c37 2e38 3037 202d 372e 3534 362c 372e  ,7.807 -7.546,7.
+000015d0: 3239 3620 2d37 2e35 3338 2c36 2e39 3739  296 -7.538,6.979
+000015e0: 202d 372e 3435 372c 362e 3731 202d 372e   -7.457,6.71 -7.
+000015f0: 3330 342c 362e 3438 3220 2d37 2e31 3531  304,6.482 -7.151
+00001600: 2c36 2e32 3538 202d 362e 3931 2c36 2e30  ,6.258 -6.91,6.0
+00001610: 3436 202d 362e 3538 322c 352e 3834 3820  46 -6.582,5.848 
+00001620: 2d36 2e32 362c 352e 3634 3620 2d35 2e34  -6.26,5.646 -5.4
+00001630: 3836 2c35 2e32 3939 202d 342e 3237 352c  86,5.299 -4.275,
+00001640: 342e 3830 3520 2d32 2e36 3731 2c34 2e31  4.805 -2.671,4.1
+00001650: 3520 2d31 2e35 3634 2c33 2e34 3631 202d  5 -1.564,3.461 -
+00001660: 302e 3935 352c 322e 3734 202d 302e 3334  0.955,2.74 -0.34
+00001670: 392c 322e 3031 3420 2d30 2e30 3239 2c31  9,2.014 -0.029,1
+00001680: 2e31 3032 2030 2c30 2220 2f3e 3c2f 673e  .102 0,0" /></g>
+00001690: 3c67 0a20 2020 2020 2020 7472 616e 7366  <g.       transf
+000016a0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2836  orm="translate(6
+000016b0: 3531 2e34 3930 322c 3536 312e 3030 3439  51.4902,561.0049
+000016c0: 2922 0a20 2020 2020 2020 6964 3d22 6732  )".       id="g2
+000016d0: 3422 0a20 2020 2020 2020 7374 796c 653d  4".       style=
+000016e0: 2266 696c 6c3a 2330 3030 3066 6622 3e3c  "fill:#0000ff"><
+000016f0: 7061 7468 0a20 2020 2020 2020 2020 6964  path.         id
+00001700: 3d22 7061 7468 3236 220a 2020 2020 2020  ="path26".      
+00001710: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00001720: 3030 3030 6666 3b66 696c 6c2d 6f70 6163  0000ff;fill-opac
+00001730: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
+00001740: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
+00001750: 6f6e 6522 0a20 2020 2020 2020 2020 643d  one".         d=
+00001760: 224d 2030 2c30 202d 312e 3232 382c 342e  "M 0,0 -1.228,4.
+00001770: 3033 3120 4820 2d37 2e34 3032 204c 202d  031 H -7.402 L -
+00001780: 382e 3633 312c 3020 4820 2d31 322e 3520  8.631,0 H -12.5 
+00001790: 6c20 352e 3937 382c 3137 2e30 3036 2068  l 5.978,17.006 h
+000017a0: 2034 2e33 3920 4c20 332e 3836 382c 3020   4.39 L 3.868,0 
+000017b0: 5a20 6d20 2d32 2e30 3836 2c37 2e30 3434  Z m -2.086,7.044
+000017c0: 2063 202d 312e 3133 362c 332e 3635 3120   c -1.136,3.651 
+000017d0: 2d31 2e37 3733 2c35 2e37 3138 202d 312e  -1.773,5.718 -1.
+000017e0: 3931 382c 362e 3139 3620 2d30 2e31 3432  918,6.196 -0.142
+000017f0: 2c30 2e34 3739 202d 302e 3234 332c 302e  ,0.479 -0.243,0.
+00001800: 3835 3620 2d30 2e33 3036 2c31 2e31 3335  856 -0.306,1.135
+00001810: 202d 302e 3235 332c 2d30 2e39 3838 202d   -0.253,-0.988 -
+00001820: 302e 3938 352c 2d33 2e34 3334 202d 322e  0.985,-3.434 -2.
+00001830: 3138 382c 2d37 2e33 3331 207a 2220 2f3e  188,-7.331 z" />
+00001840: 3c2f 673e 3c67 0a20 2020 2020 2020 7472  </g><g.       tr
+00001850: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00001860: 7465 2836 3631 2e32 3935 392c 3536 312e  te(661.2959,561.
+00001870: 3030 3439 2922 0a20 2020 2020 2020 6964  0049)".       id
+00001880: 3d22 6732 3822 0a20 2020 2020 2020 7374  ="g28".       st
+00001890: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+000018a0: 6622 3e3c 7061 7468 0a20 2020 2020 2020  f"><path.       
+000018b0: 2020 6964 3d22 7061 7468 3330 220a 2020    id="path30".  
+000018c0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+000018d0: 6c6c 3a23 3030 3030 6666 3b66 696c 6c2d  ll:#0000ff;fill-
+000018e0: 6f70 6163 6974 793a 313b 6669 6c6c 2d72  opacity:1;fill-r
+000018f0: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
+00001900: 6b65 3a6e 6f6e 6522 0a20 2020 2020 2020  ke:none".       
+00001910: 2020 643d 224d 2030 2c30 2048 202d 332e    d="M 0,0 H -3.
+00001920: 3539 3220 5620 3133 2e39 3437 2048 202d  592 V 13.947 H -
+00001930: 382e 3139 2076 2032 2e39 3838 2048 2034  8.19 v 2.988 H 4
+00001940: 2e35 3939 2056 2031 332e 3934 3720 4820  .599 V 13.947 H 
+00001950: 3020 5a22 202f 3e3c 2f67 3e3c 670a 2020  0 Z" /></g><g.  
+00001960: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+00001970: 7472 616e 736c 6174 6528 3636 382e 3039  translate(668.09
+00001980: 3038 2c35 3631 2e30 3034 3929 220a 2020  08,561.0049)".  
+00001990: 2020 2020 2069 643d 2267 3332 220a 2020       id="g32".  
+000019a0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+000019b0: 3a23 3030 3030 6666 223e 3c70 6174 680a  :#0000ff"><path.
+000019c0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+000019d0: 6833 3422 0a20 2020 2020 2020 2020 7374  h34".         st
+000019e0: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+000019f0: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+00001a00: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+00001a10: 726f 3b73 7472 6f6b 653a 6e6f 6e65 220a  ro;stroke:none".
+00001a20: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+00001a30: 3020 5620 3136 2e39 3335 2048 2033 2e35  0 V 16.935 H 3.5
+00001a40: 3931 2056 2032 2e39 3635 2068 2036 2e38  91 V 2.965 h 6.8
+00001a50: 3720 5620 3020 5a22 202f 3e3c 2f67 3e3c  7 V 0 Z" /></g><
+00001a60: 670a 2020 2020 2020 2074 7261 6e73 666f  g.       transfo
+00001a70: 726d 3d22 7472 616e 736c 6174 6528 3639  rm="translate(69
+00001a80: 322e 3334 3437 2c35 3631 2e30 3034 3929  2.3447,561.0049)
+00001a90: 220a 2020 2020 2020 2069 643d 2267 3336  ".       id="g36
+00001aa0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+00001ab0: 6669 6c6c 3a23 3030 3030 6666 223e 3c70  fill:#0000ff"><p
+00001ac0: 6174 680a 2020 2020 2020 2020 2069 643d  ath.         id=
+00001ad0: 2270 6174 6833 3822 0a20 2020 2020 2020  "path38".       
+00001ae0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+00001af0: 3030 3066 663b 6669 6c6c 2d6f 7061 6369  000ff;fill-opaci
+00001b00: 7479 3a31 3b66 696c 6c2d 7275 6c65 3a6e  ty:1;fill-rule:n
+00001b10: 6f6e 7a65 726f 3b73 7472 6f6b 653a 6e6f  onzero;stroke:no
+00001b20: 6e65 220a 2020 2020 2020 2020 2064 3d22  ne".         d="
+00001b30: 4d20 302c 3020 2d31 2e32 3239 2c34 2e30  M 0,0 -1.229,4.0
+00001b40: 3331 2048 202d 372e 3430 3220 4c20 2d38  31 H -7.402 L -8
+00001b50: 2e36 332c 3020 6820 2d33 2e38 3731 206c  .63,0 h -3.871 l
+00001b60: 2035 2e39 3738 2c31 372e 3030 3620 6820   5.978,17.006 h 
+00001b70: 342e 3339 3220 4c20 332e 3836 392c 3020  4.392 L 3.869,0 
+00001b80: 5a20 6d20 2d32 2e30 3837 2c37 2e30 3434  Z m -2.087,7.044
+00001b90: 2063 202d 312e 3133 352c 332e 3635 3120   c -1.135,3.651 
+00001ba0: 2d31 2e37 3734 2c35 2e37 3138 202d 312e  -1.774,5.718 -1.
+00001bb0: 3931 362c 362e 3139 3620 2d30 2e31 3433  916,6.196 -0.143
+00001bc0: 2c30 2e34 3739 202d 302e 3234 342c 302e  ,0.479 -0.244,0.
+00001bd0: 3835 3620 2d30 2e33 3038 2c31 2e31 3335  856 -0.308,1.135
+00001be0: 202d 302e 3235 352c 2d30 2e39 3838 202d   -0.255,-0.988 -
+00001bf0: 302e 3938 322c 2d33 2e34 3334 202d 322e  0.982,-3.434 -2.
+00001c00: 3139 2c2d 372e 3333 3120 7a22 202f 3e3c  19,-7.331 z" /><
+00001c10: 2f67 3e3c 2f67 3e3c 2f67 3e3c 7465 7874  /g></g></g><text
+00001c20: 0a20 2020 6964 3d22 7465 7874 3430 220a  .   id="text40".
+00001c30: 2020 2073 7479 6c65 3d22 666f 6e74 2d76     style="font-v
+00001c40: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
+00001c50: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
+00001c60: 6f6e 742d 7374 7265 7463 683a 636f 6e64  ont-stretch:cond
+00001c70: 656e 7365 643b 666f 6e74 2d73 697a 653a  ensed;font-size:
+00001c80: 3237 2e32 3033 3770 783b 666f 6e74 2d66  27.2037px;font-f
+00001c90: 616d 696c 793a 2748 656c 7665 7469 6361  amily:'Helvetica
+00001ca0: 204e 6575 6527 3b2d 696e 6b73 6361 7065   Neue';-inkscape
+00001cb0: 2d66 6f6e 742d 7370 6563 6966 6963 6174  -font-specificat
+00001cc0: 696f 6e3a 4865 6c76 6574 6963 614e 6575  ion:HelveticaNeu
+00001cd0: 652d 436f 6e64 656e 7365 6442 6c61 636b  e-CondensedBlack
+00001ce0: 3b77 7269 7469 6e67 2d6d 6f64 653a 6c72  ;writing-mode:lr
+00001cf0: 2d74 623b 6669 6c6c 3a23 3030 3030 6666  -tb;fill:#0000ff
+00001d00: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00001d10: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
+00001d20: 6f3b 7374 726f 6b65 3a6e 6f6e 6522 0a20  o;stroke:none". 
+00001d30: 2020 7472 616e 7366 6f72 6d3d 226d 6174    transform="mat
+00001d40: 7269 7828 312c 302c 302c 2d31 2c37 3332  rix(1,0,0,-1,732
+00001d50: 2e37 3933 392c 3536 312e 3036 3933 2922  .7939,561.0693)"
+00001d60: 3e3c 7473 7061 6e0a 2020 2020 2069 643d  ><tspan.     id=
+00001d70: 2274 7370 616e 3432 220a 2020 2020 2079  "tspan42".     y
+00001d80: 3d22 3022 0a20 2020 2020 783d 2230 2037  ="0".     x="0 7
+00001d90: 2e30 3732 3936 3138 2031 392e 3634 3130  .0729618 19.6410
+00001da0: 3731 220a 2020 2020 2073 7479 6c65 3d22  71".     style="
+00001db0: 6669 6c6c 3a23 3030 3030 6666 223e 4954  fill:#0000ff">IT
+00001dc0: 6b3c 2f74 7370 616e 3e3c 2f74 6578 743e  k</tspan></text>
+00001dd0: 0a3c 670a 2020 2069 643d 2267 3434 220a  .<g.   id="g44".
+00001de0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00001df0: 3030 3030 6666 223e 3c67 0a20 2020 2020  0000ff"><g.     
+00001e00: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+00001e10: 636c 6970 5061 7468 3438 2922 0a20 2020  clipPath48)".   
+00001e20: 2020 6964 3d22 6734 3622 0a20 2020 2020    id="g46".     
+00001e30: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00001e40: 3066 6622 3e3c 670a 2020 2020 2020 2074  0ff"><g.       t
+00001e50: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00001e60: 6174 6528 3731 382e 3038 342c 3538 332e  ate(718.084,583.
+00001e70: 3035 3138 2922 0a20 2020 2020 2020 6964  0518)".       id
+00001e80: 3d22 6735 3222 0a20 2020 2020 2020 7374  ="g52".       st
+00001e90: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+00001ea0: 6622 3e3c 7061 7468 0a20 2020 2020 2020  f"><path.       
+00001eb0: 2020 6964 3d22 7061 7468 3534 220a 2020    id="path54".  
+00001ec0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00001ed0: 6c6c 3a23 3030 3030 6666 3b66 696c 6c2d  ll:#0000ff;fill-
+00001ee0: 6f70 6163 6974 793a 313b 6669 6c6c 2d72  opacity:1;fill-r
+00001ef0: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
+00001f00: 6b65 3a6e 6f6e 6522 0a20 2020 2020 2020  ke:none".       
+00001f10: 2020 643d 226d 2030 2c30 2063 202d 332e    d="m 0,0 c -3.
+00001f20: 3031 322c 2d30 2e39 3034 202d 342e 3637  012,-0.904 -4.67
+00001f30: 2c2d 302e 3732 3620 2d34 2e39 3738 2c2d  ,-0.726 -4.978,-
+00001f40: 302e 3133 3120 6c20 2d30 2e35 332c 2d30  0.131 l -0.53,-0
+00001f50: 2e32 3733 2063 2030 2e32 3833 2c2d 302e  .273 c 0.283,-0.
+00001f60: 3534 3820 302e 3939 332c 2d30 2e38 3233  548 0.993,-0.823
+00001f70: 2032 2e30 3536 2c2d 302e 3832 3320 302e   2.056,-0.823 0.
+00001f80: 3938 362c 3020 322e 3237 342c 302e 3233  986,0 2.274,0.23
+00001f90: 3820 332e 3830 362c 302e 3731 2043 2030  8 3.806,0.71 C 0
+00001fa0: 2e32 3334 2c2d 302e 3334 3620 302e 3131  .234,-0.346 0.11
+00001fb0: 362c 2d30 2e31 3733 2030 2c30 2220 2f3e  6,-0.173 0,0" />
+00001fc0: 3c2f 673e 3c67 0a20 2020 2020 2020 7472  </g><g.       tr
+00001fd0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00001fe0: 7465 2837 3232 2e31 3130 342c 3539 322e  te(722.1104,592.
+00001ff0: 3130 3535 2922 0a20 2020 2020 2020 6964  1055)".       id
+00002000: 3d22 6735 3622 0a20 2020 2020 2020 7374  ="g56".       st
+00002010: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+00002020: 6622 3e3c 7061 7468 0a20 2020 2020 2020  f"><path.       
+00002030: 2020 6964 3d22 7061 7468 3538 220a 2020    id="path58".  
+00002040: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00002050: 6c6c 3a23 3030 3030 6666 3b66 696c 6c2d  ll:#0000ff;fill-
+00002060: 6f70 6163 6974 793a 313b 6669 6c6c 2d72  opacity:1;fill-r
+00002070: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
+00002080: 6b65 3a6e 6f6e 6522 0a20 2020 2020 2020  ke:none".       
+00002090: 2020 643d 226d 2030 2c30 2063 2030 2e31    d="m 0,0 c 0.1
+000020a0: 3839 2c30 2e30 3837 2030 2e33 3738 2c30  89,0.087 0.378,0
+000020b0: 2e31 3733 2030 2e35 3637 2c30 2e32 3535  .173 0.567,0.255
+000020c0: 202d 322e 3639 2c33 2e31 3531 202d 352e   -2.69,3.151 -5.
+000020d0: 3236 382c 342e 3534 3920 2d36 2e37 3337  268,4.549 -6.737
+000020e0: 2c33 2e36 3531 206c 2030 2e33 3131 2c2d  ,3.651 l 0.311,-
+000020f0: 302e 3531 2043 202d 342e 3731 342c 342e  0.51 C -4.714,4.
+00002100: 3039 3920 2d32 2e33 3734 2c32 2e37 3336  099 -2.374,2.736
+00002110: 2030 2c30 2220 2f3e 3c2f 673e 3c67 0a20   0,0" /></g><g. 
+00002120: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+00002130: 2274 7261 6e73 6c61 7465 2837 3332 2e31  "translate(732.1
+00002140: 3039 342c 3539 322e 3734 3929 220a 2020  094,592.749)".  
+00002150: 2020 2020 2069 643d 2267 3630 220a 2020       id="g60".  
+00002160: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00002170: 3a23 3030 3030 6666 223e 3c70 6174 680a  :#0000ff"><path.
+00002180: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00002190: 6836 3222 0a20 2020 2020 2020 2020 7374  h62".         st
+000021a0: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+000021b0: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+000021c0: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+000021d0: 726f 3b73 7472 6f6b 653a 6e6f 6e65 220a  ro;stroke:none".
+000021e0: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+000021f0: 3020 2d30 2e35 3239 2c2d 302e 3237 3320  0 -0.529,-0.273 
+00002200: 4320 2d30 2e34 3333 2c2d 302e 3436 3220  C -0.433,-0.462 
+00002210: 2d30 2e34 342c 2d30 2e37 3120 2d30 2e35  -0.44,-0.71 -0.5
+00002220: 3437 2c2d 312e 3030 3420 2d31 2e33 3431  47,-1.004 -1.341
+00002230: 2c31 2e35 3235 202d 322e 3939 392c 332e  ,1.525 -2.999,3.
+00002240: 3434 3720 2d35 2e32 3331 2c34 2e34 3135  447 -5.231,4.415
+00002250: 204c 202d 352e 3437 2c33 2e38 3637 2063   L -5.47,3.867 c
+00002260: 2032 2e31 3037 2c2d 302e 3931 3320 332e   2.107,-0.913 3.
+00002270: 3636 382c 2d32 2e37 3439 2034 2e33 3934  668,-2.749 4.394
+00002280: 2c2d 352e 3137 3220 302e 3034 352c 2d30  ,-5.172 0.045,-0
+00002290: 2e31 3438 2030 2e30 3835 2c2d 302e 3239  .148 0.085,-0.29
+000022a0: 3620 302e 3132 322c 2d30 2e34 3435 202d  6 0.122,-0.445 -
+000022b0: 302e 3738 2c2d 312e 3131 3920 2d32 2e34  0.78,-1.119 -2.4
+000022c0: 3634 2c2d 322e 3630 3820 2d34 2e38 3439  64,-2.608 -4.849
+000022d0: 2c2d 342e 3131 3220 2d30 2e33 3338 2c30  ,-4.112 -0.338,0
+000022e0: 2e36 3631 202d 302e 3730 372c 312e 3332  .661 -0.707,1.32
+000022f0: 3520 2d31 2e31 3039 2c31 2e39 3833 202d  5 -1.109,1.983 -
+00002300: 302e 3336 332c 302e 3539 202d 302e 3734  0.363,0.59 -0.74
+00002310: 332c 312e 3136 3420 2d31 2e31 3336 2c31  3,1.164 -1.136,1
+00002320: 2e37 3134 202d 302e 3138 312c 2d30 2e30  .714 -0.181,-0.0
+00002330: 3738 202d 302e 3336 382c 2d30 2e31 3538  78 -0.368,-0.158
+00002340: 202d 302e 3535 382c 2d30 2e32 3432 2030   -0.558,-0.242 0
+00002350: 2e34 3039 2c2d 302e 3537 2030 2e38 3037  .409,-0.57 0.807
+00002360: 2c2d 312e 3136 3920 312e 3138 342c 2d31  ,-1.169 1.184,-1
+00002370: 2e37 3834 2030 2e34 3034 2c2d 302e 3636  .784 0.404,-0.66
+00002380: 3220 302e 3737 342c 2d31 2e33 3238 2031  2 0.774,-1.328 1
+00002390: 2e31 3039 2c2d 312e 3938 3620 2d30 2e36  .109,-1.986 -0.6
+000023a0: 3931 2c2d 302e 3431 3920 2d31 2e34 3332  91,-0.419 -1.432
+000023b0: 2c2d 302e 3833 3920 2d32 2e32 3237 2c2d  ,-0.839 -2.227,-
+000023c0: 312e 3234 3820 2d31 2e31 3236 2c2d 302e  1.248 -1.126,-0.
+000023d0: 3538 3220 2d32 2e32 3532 2c2d 312e 3039  582 -2.252,-1.09
+000023e0: 3520 2d33 2e33 3533 2c2d 312e 3532 3820  5 -3.353,-1.528 
+000023f0: 302e 3132 2c2d 302e 3137 2030 2e32 3339  0.12,-0.17 0.239
+00002400: 2c2d 302e 3333 3620 302e 3335 382c 2d30  ,-0.336 0.358,-0
+00002410: 2e34 3938 2031 2e30 3735 2c30 2e34 3320  .498 1.075,0.43 
+00002420: 322e 3137 342c 302e 3933 2033 2e32 3731  2.174,0.93 3.271
+00002430: 2c31 2e34 3938 2030 2e37 3531 2c30 2e33  ,1.498 0.751,0.3
+00002440: 3838 2031 2e34 3935 2c30 2e38 3036 2032  88 1.495,0.806 2
+00002450: 2e32 3135 2c31 2e32 3431 2030 2e37 3431  .215,1.241 0.741
+00002460: 2c2d 312e 3534 3320 312e 3237 352c 2d33  ,-1.543 1.275,-3
+00002470: 2e30 3436 2031 2e35 3436 2c2d 342e 3338  .046 1.546,-4.38
+00002480: 3420 302e 3133 342c 2d30 2e36 3720 302e  4 0.134,-0.67 0.
+00002490: 3139 362c 2d31 2e32 3639 2030 2e31 3931  196,-1.269 0.191
+000024a0: 2c2d 312e 3739 3220 2d32 2e36 3436 2c2d  ,-1.792 -2.646,-
+000024b0: 322e 3533 3520 2d36 2e32 3535 2c2d 332e  2.535 -6.255,-3.
+000024c0: 3530 3620 2d39 2e33 3533 2c2d 322e 3136  506 -9.353,-2.16
+000024d0: 3520 4c20 2d31 332e 392c 2d31 352e 3620  5 L -13.9,-15.6 
+000024e0: 6320 312e 3032 2c2d 302e 3434 3220 322e  c 1.02,-0.442 2.
+000024f0: 3039 312c 2d30 2e36 3532 2033 2e31 3639  091,-0.652 3.169
+00002500: 2c2d 302e 3635 3220 322e 3232 322c 3020  ,-0.652 2.222,0 
+00002510: 342e 3436 362c 302e 3839 3420 362e 3332  4.466,0.894 6.32
+00002520: 362c 322e 3437 3920 2d30 2e31 3137 2c2d  6,2.479 -0.117,-
+00002530: 302e 3531 3620 2d30 2e33 3433 2c2d 302e  0.516 -0.343,-0.
+00002540: 3839 202d 302e 3637 322c 2d31 2e30 3931  89 -0.672,-1.091
+00002550: 206c 2030 2e33 3131 2c2d 302e 3530 3920   l 0.311,-0.509 
+00002560: 6320 302e 3633 312c 302e 3338 3720 302e  c 0.631,0.387 0.
+00002570: 3938 322c 312e 3135 3320 312e 3034 312c  982,1.153 1.041,
+00002580: 322e 3232 3720 312e 3036 372c 312e 3036  2.227 1.067,1.06
+00002590: 3620 312e 3937 332c 322e 3337 3320 322e  6 1.973,2.373 2.
+000025a0: 3632 372c 332e 3838 3420 312e 3034 362c  627,3.884 1.046,
+000025b0: 322e 3431 3520 312e 3331 332c 352e 3031  2.415 1.313,5.01
+000025c0: 3120 302e 3738 332c 372e 3339 3620 4320  1 0.783,7.396 C 
+000025d0: 302e 3132 352c 2d31 2e31 3535 2030 2e32  0.125,-1.155 0.2
+000025e0: 3638 2c2d 302e 3531 3420 302c 3020 6d20  68,-0.514 0,0 m 
+000025f0: 2d31 2e36 3436 2c2d 392e 3032 3420 6320  -1.646,-9.024 c 
+00002600: 2d30 2e35 3337 2c2d 312e 3234 3120 2d31  -0.537,-1.241 -1
+00002610: 2e32 3532 2c2d 322e 3333 3920 2d32 2e30  .252,-2.339 -2.0
+00002620: 3839 2c2d 332e 3236 3720 2d30 2e30 332c  89,-3.267 -0.03,
+00002630: 302e 3430 3820 2d30 2e30 392c 302e 3834  0.408 -0.09,0.84
+00002640: 3620 2d30 2e31 3835 2c31 2e33 3134 202d  6 -0.185,1.314 -
+00002650: 302e 3238 332c 312e 3430 3220 2d30 2e38  0.283,1.402 -0.8
+00002660: 3432 2c32 2e39 3733 202d 312e 3631 372c  42,2.973 -1.617,
+00002670: 342e 3538 3120 312e 3939 322c 312e 3235  4.581 1.992,1.25
+00002680: 3620 332e 3733 332c 322e 3633 3420 342e  6 3.733,2.634 4.
+00002690: 3734 342c 332e 3836 3920 302e 3335 352c  744,3.869 0.355,
+000026a0: 2d32 2e31 3134 2030 2e30 3636 2c2d 342e  -2.114 0.066,-4.
+000026b0: 3337 3720 2d30 2e38 3533 2c2d 362e 3439  377 -0.853,-6.49
+000026c0: 3722 202f 3e3c 2f67 3e3c 670a 2020 2020  7" /></g><g.    
+000026d0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+000026e0: 616e 736c 6174 6528 3732 322e 3534 322c  anslate(722.542,
+000026f0: 3539 382e 3236 3237 2922 0a20 2020 2020  598.2627)".     
+00002700: 2020 6964 3d22 6736 3422 0a20 2020 2020    id="g64".     
+00002710: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+00002720: 3030 3066 6622 3e3c 7061 7468 0a20 2020  000ff"><path.   
+00002730: 2020 2020 2020 6964 3d22 7061 7468 3636        id="path66
+00002740: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+00002750: 3d22 6669 6c6c 3a23 3030 3030 6666 3b66  ="fill:#0000ff;f
+00002760: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
+00002770: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00002780: 7374 726f 6b65 3a6e 6f6e 6522 0a20 2020  stroke:none".   
+00002790: 2020 2020 2020 643d 226d 2030 2c30 2063        d="m 0,0 c
+000027a0: 202d 362e 3130 352c 3020 2d31 312e 3037   -6.105,0 -11.07
+000027b0: 362c 2d34 2e39 3720 2d31 312e 3037 362c  6,-4.97 -11.076,
+000027c0: 2d31 312e 3037 3720 302c 2d36 2e31 3038  -11.077 0,-6.108
+000027d0: 2034 2e39 3731 2c2d 3131 2e30 3736 2031   4.971,-11.076 1
+000027e0: 312e 3037 362c 2d31 312e 3037 3620 362e  1.076,-11.076 6.
+000027f0: 3130 382c 3020 3131 2e30 3738 2c34 2e39  108,0 11.078,4.9
+00002800: 3638 2031 312e 3037 382c 3131 2e30 3736  68 11.078,11.076
+00002810: 2043 2031 312e 3037 382c 2d34 2e39 3720   C 11.078,-4.97 
+00002820: 362e 3130 382c 3020 302c 3020 4d20 372e  6.108,0 0,0 M 7.
+00002830: 3736 312c 2d34 2e35 3539 2043 2037 2e31  761,-4.559 C 7.1
+00002840: 3039 2c2d 342e 3530 3620 362e 3330 352c  09,-4.506 6.305,
+00002850: 2d34 2e35 3738 2035 2e33 3532 2c2d 342e  -4.578 5.352,-4.
+00002860: 3738 2033 2e33 3239 2c2d 352e 3230 3720  78 3.329,-5.207 
+00002870: 302e 3739 392c 2d36 2e31 3738 202d 312e  0.799,-6.178 -1.
+00002880: 3737 392c 2d37 2e35 3120 6320 2d31 2e33  779,-7.51 c -1.3
+00002890: 352c 2d30 2e36 3938 202d 322e 3636 342c  5,-0.698 -2.664,
+000028a0: 2d31 2e34 3737 202d 332e 3834 2c2d 322e  -1.477 -3.84,-2.
+000028b0: 3238 3320 2d30 2e34 3639 2c31 2e31 3334  283 -0.469,1.134
+000028c0: 202d 302e 3831 322c 322e 3232 3720 2d31   -0.812,2.227 -1
+000028d0: 2e30 3036 2c33 2e32 3237 202d 302e 3036  .006,3.227 -0.06
+000028e0: 352c 302e 3334 3220 2d30 2e31 3133 2c30  5,0.342 -0.113,0
+000028f0: 2e36 3637 202d 302e 3134 312c 302e 3936  .667 -0.141,0.96
+00002900: 3920 322e 3034 362c 322e 3936 3920 352e  9 2.046,2.969 5.
+00002910: 3231 362c 342e 3639 2038 2e32 3837 2c34  216,4.69 8.287,4
+00002920: 2e35 3434 2032 2e34 3931 2c2d 302e 3337  .544 2.491,-0.37
+00002930: 3620 342e 3638 362c 2d31 2e36 3631 2036  6 4.686,-1.661 6
+00002940: 2e32 342c 2d33 2e35 3036 206d 202d 3134  .24,-3.506 m -14
+00002950: 2e30 3033 2c31 2e34 3633 2063 2031 2e30  .003,1.463 c 1.0
+00002960: 3835 2c30 2e38 3520 322e 3334 362c 312e  85,0.85 2.346,1.
+00002970: 3438 3920 332e 3731 382c 312e 3833 3920  489 3.718,1.839 
+00002980: 2d31 2e35 3935 2c2d 302e 3730 3520 2d33  -1.595,-0.705 -3
+00002990: 2e30 3735 2c2d 312e 3835 3320 2d34 2e32  .075,-1.853 -4.2
+000029a0: 3632 2c2d 332e 3335 3820 302e 3034 332c  62,-3.358 0.043,
+000029b0: 302e 3639 3820 302e 3232 362c 312e 3231  0.698 0.226,1.21
+000029c0: 3820 302e 3534 342c 312e 3531 3920 6d20  8 0.544,1.519 m 
+000029d0: 2d31 2e32 382c 2d33 2e37 3532 2063 2030  -1.28,-3.752 c 0
+000029e0: 2e32 3139 2c2d 312e 3039 2030 2e36 3032  .219,-1.09 0.602
+000029f0: 2c2d 322e 3237 3720 312e 3132 322c 2d33  ,-2.277 1.122,-3
+00002a00: 2e35 202d 302e 3939 342c 2d30 2e37 3320  .5 -0.994,-0.73 
+00002a10: 2d31 2e38 3537 2c2d 312e 3437 3120 2d32  -1.857,-1.471 -2
+00002a20: 2e35 3134 2c2d 322e 3138 3320 2d30 2e30  .514,-2.183 -0.0
+00002a30: 3231 2c31 2e35 3835 2030 2e32 3937 2c33  21,1.585 0.297,3
+00002a40: 2e32 3437 2030 2e39 3933 2c34 2e38 3537  .247 0.993,4.857
+00002a50: 2030 2e31 3235 2c30 2e32 3832 2030 2e32   0.125,0.282 0.2
+00002a60: 3537 2c30 2e35 3537 2030 2e33 3939 2c30  57,0.557 0.399,0
+00002a70: 2e38 3236 206d 202d 302e 3139 352c 322e  .826 m -0.195,2.
+00002a80: 3333 3820 6320 2d30 2e30 3239 2c2d 302e  338 c -0.029,-0.
+00002a90: 3432 3120 2d30 2e30 3133 2c2d 302e 3838  421 -0.013,-0.88
+00002aa0: 3620 302e 3034 342c 2d31 2e33 3839 202d  6 0.044,-1.389 -
+00002ab0: 302e 3239 332c 2d30 2e34 3837 202d 302e  0.293,-0.487 -0.
+00002ac0: 3535 392c 2d30 2e39 3939 202d 302e 3739  559,-0.999 -0.79
+00002ad0: 342c 2d31 2e35 3339 202d 302e 3832 392c  4,-1.539 -0.829,
+00002ae0: 2d31 2e39 3135 202d 312e 3134 372c 2d33  -1.915 -1.147,-3
+00002af0: 2e39 3033 202d 312e 3031 342c 2d35 2e37  .903 -1.014,-5.7
+00002b00: 3638 202d 302e 3132 2c2d 302e 3135 3820  68 -0.12,-0.158 
+00002b10: 2d30 2e32 3235 2c2d 302e 3331 3520 2d30  -0.225,-0.315 -0
+00002b20: 2e33 3139 2c2d 302e 3436 3920 2d30 2e32  .319,-0.469 -0.2
+00002b30: 322c 302e 3833 3120 2d30 2e33 3339 2c31  2,0.831 -0.339,1
+00002b40: 2e37 202d 302e 3333 392c 322e 3539 3820  .7 -0.339,2.598 
+00002b50: 302c 322e 3530 3320 302e 3931 342c 342e  0,2.503 0.914,4.
+00002b60: 3739 3720 322e 3432 322c 362e 3536 3720  797 2.422,6.567 
+00002b70: 6d20 2d31 2e35 3539 2c2d 3130 2e31 3738  m -1.559,-10.178
+00002b80: 2063 2030 2e30 3736 2c2d 302e 3336 2030   c 0.076,-0.36 0
+00002b90: 2e31 372c 2d30 2e37 3131 2030 2e32 3738  .17,-0.711 0.278
+00002ba0: 2c2d 312e 3035 3420 2d30 2e31 322c 302e  ,-1.054 -0.12,0.
+00002bb0: 3233 3320 2d30 2e32 3334 2c30 2e34 3720  233 -0.234,0.47 
+00002bc0: 2d30 2e33 3339 2c30 2e37 3134 202d 3130  -0.339,0.714 -10
+00002bd0: 652d 342c 302e 3120 302e 3031 392c 302e  e-4,0.1 0.019,0.
+00002be0: 3231 3320 302e 3036 312c 302e 3334 206d  213 0.061,0.34 m
+00002bf0: 2031 332e 3436 372c 2d35 2e36 3138 2063   13.467,-5.618 c
+00002c00: 202d 302e 3739 392c 2d30 2e32 3038 202d   -0.799,-0.208 -
+00002c10: 322e 3037 382c 302e 3334 3120 2d33 2e35  2.078,0.341 -3.5
+00002c20: 3233 2c31 2e35 3533 2030 2e30 3339 2c2d  23,1.553 0.039,-
+00002c30: 302e 3236 3920 302e 3031 372c 2d30 2e35  0.269 0.017,-0.5
+00002c40: 3436 202d 302e 3039 332c 2d30 2e38 3036  46 -0.093,-0.806
+00002c50: 202d 302e 3033 382c 2d30 2e30 3839 202d   -0.038,-0.089 -
+00002c60: 302e 3037 382c 2d30 2e31 3732 202d 302e  0.078,-0.172 -0.
+00002c70: 3131 382c 2d30 2e32 3534 2030 2e36 3437  118,-0.254 0.647
+00002c80: 2c2d 302e 3439 3920 312e 3237 352c 2d30  ,-0.499 1.275,-0
+00002c90: 2e38 3831 2031 2e38 3635 2c2d 312e 3133  .881 1.865,-1.13
+00002ca0: 3120 4320 312e 3537 362c 2d32 312e 3132  1 C 1.576,-21.12
+00002cb0: 2030 2e38 2c2d 3231 2e32 3137 2030 2c2d   0.8,-21.217 0,-
+00002cc0: 3231 2e32 3137 2063 202d 322e 3534 322c  21.217 c -2.542,
+00002cd0: 3020 2d34 2e38 3639 2c30 2e39 3435 202d  0 -4.869,0.945 -
+00002ce0: 362e 3635 2c32 2e34 3937 202d 312e 3136  6.65,2.497 -1.16
+00002cf0: 332c 312e 3239 3220 2d31 2e39 3038 2c32  3,1.292 -1.908,2
+00002d00: 2e39 3839 202d 322e 3136 352c 342e 3835  .989 -2.165,4.85
+00002d10: 3520 302e 3533 372c 302e 3733 3120 312e  5 0.537,0.731 1.
+00002d20: 3437 362c 312e 3634 3920 322e 3830 352c  476,1.649 2.805,
+00002d30: 322e 3634 3420 302e 3431 372c 2d30 2e38  2.644 0.417,-0.8
+00002d40: 3833 2030 2e38 3939 2c2d 312e 3737 3720  83 0.899,-1.777 
+00002d50: 312e 3434 2c2d 322e 3635 3920 302e 3832  1.44,-2.659 0.82
+00002d60: 312c 2d31 2e33 3434 2031 2e36 3935 2c2d  1,-1.344 1.695,-
+00002d70: 322e 3534 2032 2e35 3734 2c2d 332e 3536  2.54 2.574,-3.56
+00002d80: 3120 302e 3236 342c 302e 3138 3520 302e  1 0.264,0.185 0.
+00002d90: 3538 312c 302e 3239 3220 302e 3932 362c  581,0.292 0.926,
+00002da0: 302e 3239 3220 302e 3032 382c 3020 302e  0.292 0.028,0 0.
+00002db0: 3035 392c 2d30 2e30 3033 2030 2e30 3838  059,-0.003 0.088
+00002dc0: 2c2d 302e 3030 3620 2d30 2e39 3334 2c31  ,-0.006 -0.934,1
+00002dd0: 2e30 3320 2d31 2e38 3839 2c32 2e32 3932  .03 -1.889,2.292
+00002de0: 202d 322e 3739 2c33 2e37 3634 202d 302e   -2.79,3.764 -0.
+00002df0: 3535 352c 302e 3930 3820 2d31 2e30 3436  555,0.908 -1.046
+00002e00: 2c31 2e38 3237 202d 312e 3436 342c 322e  ,1.827 -1.464,2.
+00002e10: 3732 3820 312e 3038 382c 302e 3735 3620  728 1.088,0.756 
+00002e20: 322e 3338 342c 312e 3534 3520 332e 3838  2.384,1.545 3.88
+00002e30: 372c 322e 3332 3120 322e 3530 342c 312e  7,2.321 2.504,1.
+00002e40: 3239 3520 342e 3935 332c 322e 3233 3620  295 4.953,2.236 
+00002e50: 362e 3839 362c 322e 3634 3620 312e 3937  6.896,2.646 1.97
+00002e60: 352c 302e 3431 3720 322e 3933 392c 302e  5,0.417 2.939,0.
+00002e70: 3137 3120 332e 3135 2c2d 302e 3137 3520  171 3.15,-0.175 
+00002e80: 302e 3931 352c 2d31 2e35 3234 2031 2e34  0.915,-1.524 1.4
+00002e90: 3432 2c2d 332e 3330 3520 312e 3434 322c  42,-3.305 1.442,
+00002ea0: 2d35 2e32 3036 2030 2c2d 342e 3039 3820  -5.206 0,-4.098 
+00002eb0: 2d32 2e34 3434 2c2d 372e 3633 3220 2d35  -2.444,-7.632 -5
+00002ec0: 2e39 3438 2c2d 392e 3232 3922 202f 3e3c  .948,-9.229" /><
+00002ed0: 2f67 3e3c 670a 2020 2020 2020 2074 7261  /g><g.       tra
+00002ee0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00002ef0: 6528 3732 382e 3138 3037 2c35 3737 2e37  e(728.1807,577.7
+00002f00: 3339 3329 220a 2020 2020 2020 2069 643d  393)".       id=
+00002f10: 2267 3638 220a 2020 2020 2020 2073 7479  "g68".       sty
+00002f20: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
+00002f30: 223e 3c70 6174 680a 2020 2020 2020 2020  "><path.        
+00002f40: 2069 643d 2270 6174 6837 3022 0a20 2020   id="path70".   
+00002f50: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00002f60: 6c3a 2330 3030 3066 663b 6669 6c6c 2d6f  l:#0000ff;fill-o
+00002f70: 7061 6369 7479 3a31 3b66 696c 6c2d 7275  pacity:1;fill-ru
+00002f80: 6c65 3a6e 6f6e 7a65 726f 3b73 7472 6f6b  le:nonzero;strok
+00002f90: 653a 6e6f 6e65 220a 2020 2020 2020 2020  e:none".        
+00002fa0: 2064 3d22 6d20 302c 3020 6320 2d30 2e30   d="m 0,0 c -0.0
+00002fb0: 3632 2c2d 302e 3035 3920 2d30 2e32 3432  62,-0.059 -0.242
+00002fc0: 2c2d 302e 3239 3820 2d30 2e33 3832 2c2d  ,-0.298 -0.382,-
+00002fd0: 302e 3330 3820 2d30 2e31 3338 2c2d 302e  0.308 -0.138,-0.
+00002fe0: 3031 3120 2d30 2e37 3935 2c2d 302e 3133  011 -0.795,-0.13
+00002ff0: 3420 2d30 2e37 3834 2c2d 302e 3337 3620  4 -0.784,-0.376 
+00003000: 2d30 2e35 3835 2c2d 302e 3236 3620 2d31  -0.585,-0.266 -1
+00003010: 2e36 3733 2c2d 302e 3532 3820 2d32 2e30  .673,-0.528 -2.0
+00003020: 322c 2d30 2e36 3735 202d 302e 3631 312c  2,-0.675 -0.611,
+00003030: 302e 3235 3220 2d31 2e30 3635 2c30 2e34  0.252 -1.065,0.4
+00003040: 202d 312e 3832 342c 302e 3434 202d 302e   -1.824,0.44 -0.
+00003050: 3635 342c 302e 3337 202d 312e 3035 342c  654,0.37 -1.054,
+00003060: 302e 3438 3920 2d31 2e33 3932 2c30 2e35  0.489 -1.392,0.5
+00003070: 3432 206c 202d 302e 3231 352c 302e 3036  42 l -0.215,0.06
+00003080: 3120 302e 3131 382c 302e 3338 3520 6320  1 0.118,0.385 c 
+00003090: 302e 3437 382c 302e 3131 3520 302e 3836  0.478,0.115 0.86
+000030a0: 332c 302e 3538 3820 302e 3937 382c 312e  3,0.588 0.978,1.
+000030b0: 3038 3620 302e 3137 2c30 2e37 3520 2d30  086 0.17,0.75 -0
+000030c0: 2e32 3031 2c31 2e33 3737 202d 302e 3732  .201,1.377 -0.72
+000030d0: 352c 312e 3631 3920 2d30 2e37 3339 2c30  5,1.619 -0.739,0
+000030e0: 2e33 3420 2d31 2e35 3836 2c2d 302e 3139  .34 -1.586,-0.19
+000030f0: 3120 2d31 2e36 3237 2c2d 312e 3132 3120  1 -1.627,-1.121 
+00003100: 2d30 2e30 3139 2c2d 302e 3530 3220 302e  -0.019,-0.502 0.
+00003110: 3131 372c 2d30 2e37 3420 302e 3136 342c  117,-0.74 0.164,
+00003120: 2d30 2e39 3339 2030 2e30 3035 2c2d 302e  -0.939 0.005,-0.
+00003130: 3031 3820 302e 3031 342c 2d30 2e30 3336  018 0.014,-0.036
+00003140: 2030 2e30 3231 2c2d 302e 3035 3720 2d30   0.021,-0.057 -0
+00003150: 2e30 3436 2c2d 302e 3135 3820 2d30 2e31  .046,-0.158 -0.1
+00003160: 3036 2c2d 302e 3332 3420 2d30 2e31 3731  06,-0.324 -0.171
+00003170: 2c2d 302e 3437 3620 2d30 2e34 3334 2c30  ,-0.476 -0.434,0
+00003180: 2e31 3631 202d 312e 312c 302e 3233 3520  .161 -1.1,0.235 
+00003190: 2d31 2e33 3938 2c30 2e32 3739 202d 312e  -1.398,0.279 -1.
+000031a0: 3139 322c 302e 3730 3220 2d32 2e34 3231  192,0.702 -2.421
+000031b0: 2c30 2e37 3338 202d 322e 3939 332c 302e  ,0.738 -2.993,0.
+000031c0: 3933 3420 2d30 2e33 3937 2c30 2e34 3837  934 -0.397,0.487
+000031d0: 202d 312e 3338 332c 302e 3838 3920 2d32   -1.383,0.889 -2
+000031e0: 2e32 3237 2c31 2e36 3535 202d 302e 3035  .227,1.655 -0.05
+000031f0: 312c 302e 3034 3720 302e 3131 2c30 2e34  1,0.047 0.11,0.4
+00003200: 3833 202d 302e 3332 382c 302e 3738 3520  83 -0.328,0.785 
+00003210: 2d30 2e33 312c 302e 3330 3120 2d30 2e33  -0.31,0.301 -0.3
+00003220: 3634 2c30 2e34 3534 202d 302e 3536 342c  64,0.454 -0.564,
+00003230: 302e 3839 3520 2d30 2e31 3731 2c30 2e31  0.895 -0.171,0.1
+00003240: 3732 202d 302e 3336 382c 302e 3330 3720  72 -0.368,0.307 
+00003250: 2d30 2e35 3638 2c30 2e32 3336 2030 2e30  -0.568,0.236 0.0
+00003260: 3232 2c2d 302e 3135 3120 302e 3135 332c  22,-0.151 0.153,
+00003270: 2d30 2e33 3432 2030 2e32 3031 2c2d 302e  -0.342 0.201,-0.
+00003280: 3736 3720 302e 3036 382c 2d30 2e36 3031  767 0.068,-0.601
+00003290: 2030 2e33 3736 2c2d 302e 3939 3120 302e   0.376,-0.991 0.
+000032a0: 3637 352c 2d31 2e34 3636 2030 2e35 3634  675,-1.466 0.564
+000032b0: 2c2d 312e 3038 3720 312e 3133 342c 2d31  ,-1.087 1.134,-1
+000032c0: 2e37 3539 2032 2e30 3034 2c2d 322e 3432  .759 2.004,-2.42
+000032d0: 3920 312e 3137 342c 2d30 2e38 3435 2031  9 1.174,-0.845 1
+000032e0: 2e38 3731 2c2d 312e 3132 3220 322e 3938  .871,-1.122 2.98
+000032f0: 2c2d 312e 3530 3620 302e 3031 312c 2d30  ,-1.506 0.011,-0
+00003300: 2e36 3837 2030 2e31 3439 2c2d 312e 3531  .687 0.149,-1.51
+00003310: 2030 2e33 3031 2c2d 322e 3231 3220 302e   0.301,-2.212 0.
+00003320: 3038 372c 2d30 2e34 3034 2030 2e32 3133  087,-0.404 0.213
+00003330: 2c2d 302e 3639 3720 302e 3230 322c 2d30  ,-0.697 0.202,-0
+00003340: 2e39 3831 202d 302e 3032 312c 2d30 2e36  .981 -0.021,-0.6
+00003350: 3137 202d 302e 3036 322c 2d30 2e35 3239  17 -0.062,-0.529
+00003360: 202d 302e 3336 322c 2d31 2e31 3532 202d   -0.362,-1.152 -
+00003370: 302e 3738 342c 2d31 2e36 3138 202d 302e  0.784,-1.618 -0.
+00003380: 3537 352c 2d34 2e30 3635 202d 302e 3533  575,-4.065 -0.53
+00003390: 322c 2d35 2e32 3133 2030 2e30 3032 2c2d  2,-5.213 0.002,-
+000033a0: 302e 3035 3220 302e 3030 332c 2d30 2e31  0.052 0.003,-0.1
+000033b0: 3032 2030 2e30 3034 2c2d 302e 3135 202d  02 0.004,-0.15 -
+000033c0: 302e 3030 352c 2d30 2e31 3120 2d30 2e30  0.005,-0.11 -0.0
+000033d0: 3535 2c2d 302e 3233 202d 302e 3239 372c  55,-0.23 -0.297,
+000033e0: 2d30 2e32 3535 202d 302e 3830 312c 2d30  -0.255 -0.801,-0
+000033f0: 2e30 3436 202d 312e 3834 352c 2d30 2e35  .046 -1.845,-0.5
+00003400: 3636 202d 322e 3733 352c 2d31 2e36 3235  66 -2.735,-1.625
+00003410: 202d 302e 3733 372c 2d30 2e38 3738 202d   -0.737,-0.878 -
+00003420: 312e 3432 382c 2d31 2e31 3339 202d 322e  1.428,-1.139 -2.
+00003430: 3134 382c 2d31 2e30 3534 202d 302e 3632  148,-1.054 -0.62
+00003440: 362c 302e 3037 3720 2d30 2e38 372c 2d30  6,0.077 -0.87,-0
+00003450: 2e32 3635 202d 302e 3631 322c 2d30 2e37  .265 -0.612,-0.7
+00003460: 3620 302e 3237 332c 2d30 2e35 3334 2030  6 0.273,-0.534 0
+00003470: 2e31 3931 2c2d 302e 3731 3420 302e 3132  .191,-0.714 0.12
+00003480: 372c 2d31 2e32 3233 202d 302e 3034 332c  7,-1.223 -0.043,
+00003490: 2d30 2e33 3432 202d 302e 3134 312c 2d30  -0.342 -0.141,-0
+000034a0: 2e35 3638 2030 2e31 3339 2c2d 302e 3930  .568 0.139,-0.90
+000034b0: 3920 302e 3334 332c 2d30 2e34 3137 2031  9 0.343,-0.417 1
+000034c0: 2e33 3039 2c2d 302e 3231 3920 312e 3130  .309,-0.219 1.10
+000034d0: 382c 2d30 2e31 3133 202d 302e 3539 372c  8,-0.113 -0.597,
+000034e0: 302e 3331 3320 2d30 2e31 3039 2c31 2e30  0.313 -0.109,1.0
+000034f0: 3631 2030 2e30 3834 2c31 2e34 3737 2031  61 0.084,1.477 1
+00003500: 2e36 3337 2c31 2e35 3035 2034 2e33 3831  .637,1.505 4.381
+00003510: 2c32 2e33 3638 2034 2e37 3332 2c32 2e35  ,2.368 4.732,2.5
+00003520: 3536 2030 2e35 3236 2c30 2e32 3536 2031  56 0.526,0.256 1
+00003530: 2e31 3933 2c30 2e32 3936 2031 2e33 3336  .193,0.296 1.336
+00003540: 2c30 2e39 3038 2030 2e30 3033 2c30 2e30  ,0.908 0.003,0.0
+00003550: 3135 2030 2e35 352c 322e 3131 3420 302e  15 0.55,2.114 0.
+00003560: 392c 332e 3338 3420 302e 3035 392c 302e  9,3.384 0.059,0.
+00003570: 3231 3220 302e 3231 372c 302e 3435 3520  212 0.217,0.455 
+00003580: 302e 3433 392c 302e 3334 3520 302e 3036  0.439,0.345 0.06
+00003590: 392c 2d30 2e30 3333 2030 2e31 342c 2d30  9,-0.033 0.14,-0
+000035a0: 2e30 3832 2030 2e32 3431 2c2d 302e 3136  .082 0.241,-0.16
+000035b0: 3420 302e 3630 362c 2d30 2e35 3036 2031  4 0.606,-0.506 1
+000035c0: 2e34 3238 2c2d 302e 3933 3420 312e 3932  .428,-0.934 1.92
+000035d0: 392c 2d31 2e32 3434 2030 2e31 3437 2c2d  9,-1.244 0.147,-
+000035e0: 302e 3039 2030 2e31 3036 2c2d 302e 3330  0.09 0.106,-0.30
+000035f0: 3220 302e 3030 382c 2d30 2e33 3932 202d  2 0.008,-0.392 -
+00003600: 302e 3739 352c 2d30 2e37 3235 202d 302e  0.795,-0.725 -0.
+00003610: 3938 312c 2d31 2e38 3035 202d 302e 3933  981,-1.805 -0.93
+00003620: 332c 2d32 2e34 3438 2030 2e30 3532 2c2d  3,-2.448 0.052,-
+00003630: 302e 3730 3820 2d30 2e31 3734 2c2d 322e  0.708 -0.174,-2.
+00003640: 3338 3520 2d30 2e35 3135 2c2d 332e 3038  385 -0.515,-3.08
+00003650: 3620 2d30 2e33 3634 2c2d 302e 3735 202d  6 -0.364,-0.75 -
+00003660: 302e 3237 372c 2d31 2e30 3838 2030 2e35  0.277,-1.088 0.5
+00003670: 3332 2c2d 302e 3938 2030 2e39 3031 2c30  32,-0.98 0.901,0
+00003680: 2e31 3138 2031 2e31 3133 2c2d 302e 3137  .118 1.113,-0.17
+00003690: 3220 312e 3634 322c 2d30 2e32 3536 2030  2 1.642,-0.256 0
+000036a0: 2e35 3236 2c2d 302e 3038 3520 312e 3132  .526,-0.085 1.12
+000036b0: 342c 302e 3431 2030 2e38 3637 2c30 2e35  4,0.41 0.867,0.5
+000036c0: 3120 2d30 2e32 3335 2c30 2e30 3933 202d  1 -0.235,0.093 -
+000036d0: 312e 3333 392c 302e 3232 3220 2d31 2e37  1.339,0.222 -1.7
+000036e0: 3736 2c30 2e39 3235 2030 2e31 3132 2c31  76,0.925 0.112,1
+000036f0: 2e33 3035 2032 2e33 3339 2c35 2e34 3235  .305 2.339,5.425
+00003700: 2032 2e34 3432 2c36 2e30 3433 202d 302e   2.442,6.043 -0.
+00003710: 3232 332c 312e 3431 202d 322e 3539 362c  223,1.41 -2.596,
+00003720: 322e 3939 3620 2d32 2e39 3337 2c33 2e32  2.996 -2.937,3.2
+00003730: 3938 202d 302e 3034 332c 302e 3231 3420  98 -0.043,0.214 
+00003740: 2d30 2e30 3836 2c30 2e36 3832 202d 302e  -0.086,0.682 -0.
+00003750: 3036 372c 312e 3137 3420 302e 3130 312c  067,1.174 0.101,
+00003760: 302e 3437 3120 302e 3634 362c 312e 3837  0.471 0.646,1.87
+00003770: 2030 2e36 3432 2c32 2e32 3133 2030 2e36   0.642,2.213 0.6
+00003780: 3931 2c2d 302e 3037 3820 312e 3936 312c  91,-0.078 1.961,
+00003790: 2d30 2e31 3834 2032 2e34 372c 302e 3038  -0.184 2.47,0.08
+000037a0: 3620 302e 3737 362c 302e 3139 3120 312e  6 0.776,0.191 1.
+000037b0: 3736 382c 302e 3938 3620 322e 3031 392c  768,0.986 2.019,
+000037c0: 312e 3239 3820 302e 3230 342c 302e 3138  1.298 0.204,0.18
+000037d0: 3620 302e 3537 322c 302e 3139 3820 302e  6 0.572,0.198 0.
+000037e0: 3733 362c 302e 3334 3720 302e 3231 362c  736,0.347 0.216,
+000037f0: 302e 3139 3220 302e 3331 322c 302e 3332  0.192 0.312,0.32
+00003800: 2030 2e35 3732 2c30 2e38 3538 2043 2030   0.572,0.858 C 0
+00003810: 2e36 3636 2c30 2e33 3831 2030 2e32 3037  .666,0.381 0.207
+00003820: 2c30 2e31 3938 2030 2c30 2220 2f3e 3c2f  ,0.198 0,0" /></
+00003830: 673e 3c2f 673e 3c2f 673e 3c67 0a20 2020  g></g></g><g.   
+00003840: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00003850: 6c61 7465 2837 3636 2e31 3237 2c35 3833  late(766.127,583
+00003860: 2e32 3237 3529 220a 2020 2069 643d 2267  .2275)".   id="g
+00003870: 3732 220a 2020 2073 7479 6c65 3d22 6669  72".   style="fi
+00003880: 6c6c 3a23 3030 3030 6666 223e 3c70 6174  ll:#0000ff"><pat
+00003890: 680a 2020 2020 2069 643d 2270 6174 6837  h.     id="path7
+000038a0: 3422 0a20 2020 2020 7374 796c 653d 2266  4".     style="f
+000038b0: 696c 6c3a 2330 3030 3066 663b 6669 6c6c  ill:#0000ff;fill
+000038c0: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
+000038d0: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
+000038e0: 6f6b 653a 6e6f 6e65 220a 2020 2020 2064  oke:none".     d
+000038f0: 3d22 6d20 302c 3020 6820 2d33 332e 3739  ="m 0,0 h -33.79
+00003900: 206c 2030 2e34 3435 2c34 2e38 3333 202d   l 0.445,4.833 -
+00003910: 312e 3231 392c 342e 3933 3820 4c20 302c  1.219,4.938 L 0,
+00003920: 392e 3733 3620 5a22 202f 3e3c 2f67 3e3c  9.736 Z" /></g><
+00003930: 670a 2020 2074 7261 6e73 666f 726d 3d22  g.   transform="
+00003940: 7472 616e 736c 6174 6528 3733 362e 3932  translate(736.92
+00003950: 3937 2c35 3933 2e30 3535 3729 220a 2020  97,593.0557)".  
+00003960: 2069 643d 2267 3736 220a 2020 2073 7479   id="g76".   sty
+00003970: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
+00003980: 223e 3c70 6174 680a 2020 2020 2069 643d  "><path.     id=
+00003990: 2270 6174 6837 3822 0a20 2020 2020 7374  "path78".     st
+000039a0: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+000039b0: 663b 7374 726f 6b65 3a23 6666 6666 6666  f;stroke:#ffffff
+000039c0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+000039d0: 3335 363b 7374 726f 6b65 2d6c 696e 6563  356;stroke-linec
+000039e0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+000039f0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00003a00: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00003a10: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00003a20: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+00003a30: 7061 6369 7479 3a31 220a 2020 2020 2064  pacity:1".     d
+00003a40: 3d22 4d20 302c 3020 5620 2d39 2e38 3734  ="M 0,0 V -9.874
+00003a50: 2220 2f3e 3c2f 673e 3c67 0a20 2020 7472  " /></g><g.   tr
+00003a60: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00003a70: 7465 2837 3431 2e37 3831 332c 3539 332e  te(741.7813,593.
+00003a80: 3032 3339 2922 0a20 2020 6964 3d22 6738  0239)".   id="g8
+00003a90: 3022 0a20 2020 7374 796c 653d 2266 696c  0".   style="fil
+00003aa0: 6c3a 2330 3030 3066 6622 3e3c 7061 7468  l:#0000ff"><path
+00003ab0: 0a20 2020 2020 6964 3d22 7061 7468 3832  .     id="path82
+00003ac0: 220a 2020 2020 2073 7479 6c65 3d22 6669  ".     style="fi
+00003ad0: 6c6c 3a23 3030 3030 6666 3b73 7472 6f6b  ll:#0000ff;strok
+00003ae0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00003af0: 2d77 6964 7468 3a30 2e33 3536 3b73 7472  -width:0.356;str
+00003b00: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00003b10: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00003b20: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+00003b30: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00003b40: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00003b50: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00003b60: 3122 0a20 2020 2020 643d 224d 2030 2c30  1".     d="M 0,0
+00003b70: 2056 202d 392e 3837 3422 202f 3e3c 2f67   V -9.874" /></g
+00003b80: 3e3c 670a 2020 2074 7261 6e73 666f 726d  ><g.   transform
+00003b90: 3d22 7472 616e 736c 6174 6528 3734 362e  ="translate(746.
+00003ba0: 3633 3637 2c35 3933 2e30 3535 3729 220a  6367,593.0557)".
+00003bb0: 2020 2069 643d 2267 3834 220a 2020 2073     id="g84".   s
+00003bc0: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
+00003bd0: 6666 223e 3c70 6174 680a 2020 2020 2069  ff"><path.     i
+00003be0: 643d 2270 6174 6838 3622 0a20 2020 2020  d="path86".     
+00003bf0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00003c00: 3066 663b 7374 726f 6b65 3a23 6666 6666  0ff;stroke:#ffff
+00003c10: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00003c20: 302e 3335 363b 7374 726f 6b65 2d6c 696e  0.356;stroke-lin
+00003c30: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00003c40: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00003c50: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00003c60: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00003c70: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00003c80: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00003c90: 2064 3d22 4d20 302c 3020 5620 2d39 2e38   d="M 0,0 V -9.8
+00003ca0: 3734 2220 2f3e 3c2f 673e 3c67 0a20 2020  74" /></g><g.   
+00003cb0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00003cc0: 6c61 7465 2837 3531 2e34 3839 332c 3539  late(751.4893,59
+00003cd0: 332e 3032 3339 2922 0a20 2020 6964 3d22  3.0239)".   id="
+00003ce0: 6738 3822 0a20 2020 7374 796c 653d 2266  g88".   style="f
+00003cf0: 696c 6c3a 2330 3030 3066 6622 3e3c 7061  ill:#0000ff"><pa
+00003d00: 7468 0a20 2020 2020 6964 3d22 7061 7468  th.     id="path
+00003d10: 3930 220a 2020 2020 2073 7479 6c65 3d22  90".     style="
+00003d20: 6669 6c6c 3a23 3030 3030 6666 3b73 7472  fill:#0000ff;str
+00003d30: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00003d40: 6b65 2d77 6964 7468 3a30 2e33 3536 3b73  ke-width:0.356;s
+00003d50: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00003d60: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00003d70: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00003d80: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00003d90: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00003da0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00003db0: 793a 3122 0a20 2020 2020 643d 224d 2030  y:1".     d="M 0
+00003dc0: 2c30 2056 202d 392e 3837 3422 202f 3e3c  ,0 V -9.874" /><
+00003dd0: 2f67 3e3c 670a 2020 2074 7261 6e73 666f  /g><g.   transfo
+00003de0: 726d 3d22 7472 616e 736c 6174 6528 3735  rm="translate(75
+00003df0: 362e 3334 3138 2c35 3933 2e30 3535 3729  6.3418,593.0557)
+00003e00: 220a 2020 2069 643d 2267 3932 220a 2020  ".   id="g92".  
+00003e10: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+00003e20: 3030 6666 223e 3c70 6174 680a 2020 2020  00ff"><path.    
+00003e30: 2069 643d 2270 6174 6839 3422 0a20 2020   id="path94".   
+00003e40: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+00003e50: 3030 3066 663b 7374 726f 6b65 3a23 6666  000ff;stroke:#ff
+00003e60: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00003e70: 683a 302e 3335 363b 7374 726f 6b65 2d6c  h:0.356;stroke-l
+00003e80: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00003e90: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00003ea0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00003eb0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00003ec0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00003ed0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00003ee0: 2020 2064 3d22 4d20 302c 3020 5620 2d39     d="M 0,0 V -9
+00003ef0: 2e38 3734 2220 2f3e 3c2f 673e 3c67 0a20  .874" /></g><g. 
+00003f00: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00003f10: 6e73 6c61 7465 2837 3631 2e31 3935 332c  nslate(761.1953,
+00003f20: 3539 332e 3032 3339 2922 0a20 2020 6964  593.0239)".   id
+00003f30: 3d22 6739 3622 0a20 2020 7374 796c 653d  ="g96".   style=
+00003f40: 2266 696c 6c3a 2330 3030 3066 6622 3e3c  "fill:#0000ff"><
+00003f50: 7061 7468 0a20 2020 2020 6964 3d22 7061  path.     id="pa
+00003f60: 7468 3938 220a 2020 2020 2073 7479 6c65  th98".     style
+00003f70: 3d22 6669 6c6c 3a23 3030 3030 6666 3b73  ="fill:#0000ff;s
+00003f80: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00003f90: 726f 6b65 2d77 6964 7468 3a30 2e33 3536  roke-width:0.356
+00003fa0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00003fb0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00003fc0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00003fd0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00003fe0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00003ff0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00004000: 6974 793a 3122 0a20 2020 2020 643d 224d  ity:1".     d="M
+00004010: 2030 2c30 2056 202d 392e 3837 3422 202f   0,0 V -9.874" /
+00004020: 3e3c 2f67 3e3c 670a 2020 2074 7261 6e73  ></g><g.   trans
+00004030: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00004040: 3733 322e 3532 3933 2c35 3838 2e30 3232  732.5293,588.022
+00004050: 3929 220a 2020 2069 643d 2267 3130 3022  9)".   id="g100"
+00004060: 0a20 2020 7374 796c 653d 2266 696c 6c3a  .   style="fill:
+00004070: 2330 3030 3066 6622 3e3c 7061 7468 0a20  #0000ff"><path. 
+00004080: 2020 2020 6964 3d22 7061 7468 3130 3222      id="path102"
+00004090: 0a20 2020 2020 7374 796c 653d 2266 696c  .     style="fil
+000040a0: 6c3a 2330 3030 3066 663b 7374 726f 6b65  l:#0000ff;stroke
+000040b0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+000040c0: 7769 6474 683a 302e 3335 363b 7374 726f  width:0.356;stro
+000040d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+000040e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000040f0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00004100: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00004110: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00004120: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00004130: 220a 2020 2020 2064 3d22 4d20 302c 3020  ".     d="M 0,0 
+00004140: 3333 2e35 3339 2c30 2e30 3038 2220 2f3e  33.539,0.008" />
+00004150: 3c2f 673e 3c67 0a20 2020 6964 3d22 6731  </g><g.   id="g1
+00004160: 3034 220a 2020 2073 7479 6c65 3d22 6669  04".   style="fi
+00004170: 6c6c 3a23 3030 3030 6666 223e 3c67 0a20  ll:#0000ff"><g. 
+00004180: 2020 2020 636c 6970 2d70 6174 683d 2275      clip-path="u
+00004190: 726c 2823 636c 6970 5061 7468 3130 3829  rl(#clipPath108)
+000041a0: 220a 2020 2020 2069 643d 2267 3130 3622  ".     id="g106"
+000041b0: 0a20 2020 2020 7374 796c 653d 2266 696c  .     style="fil
+000041c0: 6c3a 2330 3030 3066 6622 3e3c 670a 2020  l:#0000ff"><g.  
+000041d0: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+000041e0: 7472 616e 736c 6174 6528 3733 332e 3234  translate(733.24
+000041f0: 3032 2c35 3930 2e34 3931 3729 220a 2020  02,590.4917)".  
+00004200: 2020 2020 2069 643d 2267 3131 3222 0a20       id="g112". 
+00004210: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00004220: 6c3a 2330 3030 3066 6622 3e3c 7061 7468  l:#0000ff"><path
+00004230: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00004240: 7468 3131 3422 0a20 2020 2020 2020 2020  th114".         
+00004250: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00004260: 3066 663b 6669 6c6c 2d6f 7061 6369 7479  0ff;fill-opacity
+00004270: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
+00004280: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
+00004290: 220a 2020 2020 2020 2020 2064 3d22 4d20  ".         d="M 
+000042a0: 302c 3020 4320 302c 302e 3639 2030 2e35  0,0 C 0,0.69 0.5
+000042b0: 3539 2c31 2e32 3531 2031 2e32 3437 2c31  59,1.251 1.247,1
+000042c0: 2e32 3531 2031 2e39 3338 2c31 2e32 3531  .251 1.938,1.251
+000042d0: 2032 2e35 3034 2c30 2e36 3920 322e 3530   2.504,0.69 2.50
+000042e0: 342c 3020 322e 3530 342c 2d30 2e36 3931  4,0 2.504,-0.691
+000042f0: 2031 2e39 3338 2c2d 312e 3235 2031 2e32   1.938,-1.25 1.2
+00004300: 3437 2c2d 312e 3235 2030 2e35 3539 2c2d  47,-1.25 0.559,-
+00004310: 312e 3235 2030 2c2d 302e 3639 3120 302c  1.25 0,-0.691 0,
+00004320: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
+00004330: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+00004340: 616e 736c 6174 6528 3733 332e 3230 392c  anslate(733.209,
+00004350: 3538 352e 3630 3335 2922 0a20 2020 2020  585.6035)".     
+00004360: 2020 6964 3d22 6731 3136 220a 2020 2020    id="g116".    
+00004370: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00004380: 3030 3030 6666 223e 3c70 6174 680a 2020  0000ff"><path.  
+00004390: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000043a0: 3138 220a 2020 2020 2020 2020 2073 7479  18".         sty
+000043b0: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
+000043c0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+000043d0: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
+000043e0: 6f3b 7374 726f 6b65 3a6e 6f6e 6522 0a20  o;stroke:none". 
+000043f0: 2020 2020 2020 2020 643d 224d 2030 2c30          d="M 0,0
+00004400: 2043 2030 2c30 2e36 3920 302e 3535 372c   C 0,0.69 0.557,
+00004410: 312e 3234 3820 312e 3234 362c 312e 3234  1.248 1.246,1.24
+00004420: 3820 312e 3933 382c 312e 3234 3820 322e  8 1.938,1.248 2.
+00004430: 3530 322c 302e 3639 2032 2e35 3032 2c30  502,0.69 2.502,0
+00004440: 2032 2e35 3032 2c2d 302e 3639 3220 312e   2.502,-0.692 1.
+00004450: 3933 382c 2d31 2e32 3531 2031 2e32 3436  938,-1.251 1.246
+00004460: 2c2d 312e 3235 3120 302e 3535 372c 2d31  ,-1.251 0.557,-1
+00004470: 2e32 3531 2030 2c2d 302e 3639 3220 302c  .251 0,-0.692 0,
+00004480: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
+00004490: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+000044a0: 616e 736c 6174 6528 3733 382e 3033 3332  anslate(738.0332
+000044b0: 2c35 3930 2e34 3931 3729 220a 2020 2020  ,590.4917)".    
+000044c0: 2020 2069 643d 2267 3132 3022 0a20 2020     id="g120".   
+000044d0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+000044e0: 2330 3030 3066 6622 3e3c 7061 7468 0a20  #0000ff"><path. 
+000044f0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00004500: 3132 3222 0a20 2020 2020 2020 2020 7374  122".         st
+00004510: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+00004520: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+00004530: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+00004540: 726f 3b73 7472 6f6b 653a 6e6f 6e65 220a  ro;stroke:none".
+00004550: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+00004560: 3020 4320 302c 302e 3639 2030 2e35 3538  0 C 0,0.69 0.558
+00004570: 2c31 2e32 3531 2031 2e32 3438 2c31 2e32  ,1.251 1.248,1.2
+00004580: 3531 2031 2e39 3339 2c31 2e32 3531 2032  51 1.939,1.251 2
+00004590: 2e35 2c30 2e36 3920 322e 352c 3020 322e  .5,0.69 2.5,0 2.
+000045a0: 352c 2d30 2e36 3931 2031 2e39 3339 2c2d  5,-0.691 1.939,-
+000045b0: 312e 3235 2031 2e32 3438 2c2d 312e 3235  1.25 1.248,-1.25
+000045c0: 2030 2e35 3538 2c2d 312e 3235 2030 2c2d   0.558,-1.25 0,-
+000045d0: 302e 3639 3120 302c 3022 202f 3e3c 2f67  0.691 0,0" /></g
+000045e0: 3e3c 670a 2020 2020 2020 2074 7261 6e73  ><g.       trans
+000045f0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00004600: 3733 382e 3030 312c 3538 352e 3630 3335  738.001,585.6035
+00004610: 2922 0a20 2020 2020 2020 6964 3d22 6731  )".       id="g1
+00004620: 3234 220a 2020 2020 2020 2073 7479 6c65  24".       style
+00004630: 3d22 6669 6c6c 3a23 3030 3030 6666 223e  ="fill:#0000ff">
+00004640: 3c70 6174 680a 2020 2020 2020 2020 2069  <path.         i
+00004650: 643d 2270 6174 6831 3236 220a 2020 2020  d="path126".    
+00004660: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00004670: 3a23 3030 3030 6666 3b66 696c 6c2d 6f70  :#0000ff;fill-op
+00004680: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
+00004690: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
+000046a0: 3a6e 6f6e 6522 0a20 2020 2020 2020 2020  :none".         
+000046b0: 643d 224d 2030 2c30 2043 2030 2c30 2e36  d="M 0,0 C 0,0.6
+000046c0: 3920 302e 3535 382c 312e 3234 3820 312e  9 0.558,1.248 1.
+000046d0: 3234 372c 312e 3234 3820 312e 3933 382c  247,1.248 1.938,
+000046e0: 312e 3234 3820 322e 3530 342c 302e 3639  1.248 2.504,0.69
+000046f0: 2032 2e35 3034 2c30 2032 2e35 3034 2c2d   2.504,0 2.504,-
+00004700: 302e 3639 3220 312e 3933 382c 2d31 2e32  0.692 1.938,-1.2
+00004710: 3531 2031 2e32 3437 2c2d 312e 3235 3120  51 1.247,-1.251 
+00004720: 302e 3535 382c 2d31 2e32 3531 2030 2c2d  0.558,-1.251 0,-
+00004730: 302e 3639 3220 302c 3022 202f 3e3c 2f67  0.692 0,0" /></g
+00004740: 3e3c 670a 2020 2020 2020 2074 7261 6e73  ><g.       trans
+00004750: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00004760: 3734 322e 3934 3932 2c35 3930 2e34 3931  742.9492,590.491
+00004770: 3729 220a 2020 2020 2020 2069 643d 2267  7)".       id="g
+00004780: 3132 3822 0a20 2020 2020 2020 7374 796c  128".       styl
+00004790: 653d 2266 696c 6c3a 2330 3030 3066 6622  e="fill:#0000ff"
+000047a0: 3e3c 7061 7468 0a20 2020 2020 2020 2020  ><path.         
+000047b0: 6964 3d22 7061 7468 3133 3022 0a20 2020  id="path130".   
+000047c0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+000047d0: 6c3a 2330 3030 3066 663b 6669 6c6c 2d6f  l:#0000ff;fill-o
+000047e0: 7061 6369 7479 3a31 3b66 696c 6c2d 7275  pacity:1;fill-ru
+000047f0: 6c65 3a6e 6f6e 7a65 726f 3b73 7472 6f6b  le:nonzero;strok
+00004800: 653a 6e6f 6e65 220a 2020 2020 2020 2020  e:none".        
+00004810: 2064 3d22 4d20 302c 3020 4320 302c 302e   d="M 0,0 C 0,0.
+00004820: 3639 2030 2e35 3537 2c31 2e32 3531 2031  69 0.557,1.251 1
+00004830: 2e32 3436 2c31 2e32 3531 2031 2e39 3338  .246,1.251 1.938
+00004840: 2c31 2e32 3531 2032 2e35 2c30 2e36 3920  ,1.251 2.5,0.69 
+00004850: 322e 352c 3020 322e 352c 2d30 2e36 3931  2.5,0 2.5,-0.691
+00004860: 2031 2e39 3338 2c2d 312e 3235 2031 2e32   1.938,-1.25 1.2
+00004870: 3436 2c2d 312e 3235 2030 2e35 3537 2c2d  46,-1.25 0.557,-
+00004880: 312e 3235 2030 2c2d 302e 3639 3120 302c  1.25 0,-0.691 0,
+00004890: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
+000048a0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+000048b0: 616e 736c 6174 6528 3734 322e 3931 362c  anslate(742.916,
+000048c0: 3538 352e 3630 3335 2922 0a20 2020 2020  585.6035)".     
+000048d0: 2020 6964 3d22 6731 3332 220a 2020 2020    id="g132".    
+000048e0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+000048f0: 3030 3030 6666 223e 3c70 6174 680a 2020  0000ff"><path.  
+00004900: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00004910: 3334 2d39 220a 2020 2020 2020 2020 2073  34-9".         s
+00004920: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
+00004930: 6666 3b66 696c 6c2d 6f70 6163 6974 793a  ff;fill-opacity:
+00004940: 313b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  1;fill-rule:nonz
+00004950: 6572 6f3b 7374 726f 6b65 3a6e 6f6e 6522  ero;stroke:none"
+00004960: 0a20 2020 2020 2020 2020 643d 224d 2030  .         d="M 0
+00004970: 2c30 2043 2030 2c30 2e36 3920 302e 3535  ,0 C 0,0.69 0.55
+00004980: 372c 312e 3234 3820 312e 3234 362c 312e  7,1.248 1.246,1.
+00004990: 3234 3820 312e 3933 382c 312e 3234 3820  248 1.938,1.248 
+000049a0: 322e 352c 302e 3639 2032 2e35 2c30 2032  2.5,0.69 2.5,0 2
+000049b0: 2e35 2c2d 302e 3639 3220 312e 3933 382c  .5,-0.692 1.938,
+000049c0: 2d31 2e32 3531 2031 2e32 3436 2c2d 312e  -1.251 1.246,-1.
+000049d0: 3235 3120 302e 3535 372c 2d31 2e32 3531  251 0.557,-1.251
+000049e0: 2030 2c2d 302e 3639 3220 302c 3022 202f   0,-0.692 0,0" /
+000049f0: 3e3c 2f67 3e3c 670a 2020 2020 2020 2074  ></g><g.       t
+00004a00: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00004a10: 6174 6528 3734 372e 3733 3933 2c35 3930  ate(747.7393,590
+00004a20: 2e34 3931 3729 220a 2020 2020 2020 2069  .4917)".       i
+00004a30: 643d 2267 3133 3622 0a20 2020 2020 2020  d="g136".       
+00004a40: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00004a50: 3066 6622 3e3c 7061 7468 0a20 2020 2020  0ff"><path.     
+00004a60: 2020 2020 6964 3d22 7061 7468 3133 382d      id="path138-
+00004a70: 3322 0a20 2020 2020 2020 2020 7374 796c  3".         styl
+00004a80: 653d 2266 696c 6c3a 2330 3030 3066 663b  e="fill:#0000ff;
+00004a90: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
+00004aa0: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+00004ab0: 3b73 7472 6f6b 653a 6e6f 6e65 220a 2020  ;stroke:none".  
+00004ac0: 2020 2020 2020 2064 3d22 4d20 302c 3020         d="M 0,0 
+00004ad0: 4320 302c 302e 3639 2030 2e35 3537 2c31  C 0,0.69 0.557,1
+00004ae0: 2e32 3531 2031 2e32 3437 2c31 2e32 3531  .251 1.247,1.251
+00004af0: 2031 2e39 3338 2c31 2e32 3531 2032 2e35   1.938,1.251 2.5
+00004b00: 3032 2c30 2e36 3920 322e 3530 322c 3020  02,0.69 2.502,0 
+00004b10: 322e 3530 322c 2d30 2e36 3931 2031 2e39  2.502,-0.691 1.9
+00004b20: 3338 2c2d 312e 3235 2031 2e32 3437 2c2d  38,-1.25 1.247,-
+00004b30: 312e 3235 2030 2e35 3537 2c2d 312e 3235  1.25 0.557,-1.25
+00004b40: 2030 2c2d 302e 3639 3120 302c 3022 202f   0,-0.691 0,0" /
+00004b50: 3e3c 2f67 3e3c 670a 2020 2020 2020 2074  ></g><g.       t
+00004b60: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00004b70: 6174 6528 3734 372e 3730 3631 2c35 3835  ate(747.7061,585
+00004b80: 2e36 3033 3529 220a 2020 2020 2020 2069  .6035)".       i
+00004b90: 643d 2267 3134 3022 0a20 2020 2020 2020  d="g140".       
+00004ba0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00004bb0: 3066 6622 3e3c 7061 7468 0a20 2020 2020  0ff"><path.     
+00004bc0: 2020 2020 6964 3d22 7061 7468 3134 3222      id="path142"
+00004bd0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00004be0: 2266 696c 6c3a 2330 3030 3066 663b 6669  "fill:#0000ff;fi
+00004bf0: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00004c00: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+00004c10: 7472 6f6b 653a 6e6f 6e65 220a 2020 2020  troke:none".    
+00004c20: 2020 2020 2064 3d22 4d20 302c 3020 4320       d="M 0,0 C 
+00004c30: 302c 302e 3639 2030 2e35 362c 312e 3234  0,0.69 0.56,1.24
+00004c40: 3820 312e 3234 372c 312e 3234 3820 312e  8 1.247,1.248 1.
+00004c50: 3933 382c 312e 3234 3820 322e 3530 332c  938,1.248 2.503,
+00004c60: 302e 3639 2032 2e35 3033 2c30 2032 2e35  0.69 2.503,0 2.5
+00004c70: 3033 2c2d 302e 3639 3220 312e 3933 382c  03,-0.692 1.938,
+00004c80: 2d31 2e32 3531 2031 2e32 3437 2c2d 312e  -1.251 1.247,-1.
+00004c90: 3235 3120 302e 3536 2c2d 312e 3235 3120  251 0.56,-1.251 
+00004ca0: 302c 2d30 2e36 3932 2030 2c30 2220 2f3e  0,-0.692 0,0" />
+00004cb0: 3c2f 673e 3c67 0a20 2020 2020 2020 7472  </g><g.       tr
+00004cc0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00004cd0: 7465 2837 3532 2e36 3534 332c 3539 302e  te(752.6543,590.
+00004ce0: 3439 3137 2922 0a20 2020 2020 2020 6964  4917)".       id
+00004cf0: 3d22 6731 3434 2d38 220a 2020 2020 2020  ="g144-8".      
+00004d00: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+00004d10: 3030 6666 223e 3c70 6174 680a 2020 2020  00ff"><path.    
+00004d20: 2020 2020 2069 643d 2270 6174 6831 3436       id="path146
+00004d30: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+00004d40: 3d22 6669 6c6c 3a23 3030 3030 6666 3b66  ="fill:#0000ff;f
+00004d50: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
+00004d60: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00004d70: 7374 726f 6b65 3a6e 6f6e 6522 0a20 2020  stroke:none".   
+00004d80: 2020 2020 2020 643d 224d 2030 2c30 2043        d="M 0,0 C
+00004d90: 2030 2c30 2e36 3920 302e 3535 372c 312e   0,0.69 0.557,1.
+00004da0: 3235 3120 312e 3234 352c 312e 3235 3120  251 1.245,1.251 
+00004db0: 312e 3933 382c 312e 3235 3120 322e 3530  1.938,1.251 2.50
+00004dc0: 322c 302e 3639 2032 2e35 3032 2c30 2032  2,0.69 2.502,0 2
+00004dd0: 2e35 3032 2c2d 302e 3639 3120 312e 3933  .502,-0.691 1.93
+00004de0: 382c 2d31 2e32 3520 312e 3234 352c 2d31  8,-1.25 1.245,-1
+00004df0: 2e32 3520 302e 3535 372c 2d31 2e32 3520  .25 0.557,-1.25 
+00004e00: 302c 2d30 2e36 3931 2030 2c30 2220 2f3e  0,-0.691 0,0" />
+00004e10: 3c2f 673e 3c67 0a20 2020 2020 2020 7472  </g><g.       tr
+00004e20: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00004e30: 7465 2837 3532 2e36 3231 312c 3538 352e  te(752.6211,585.
+00004e40: 3630 3335 2922 0a20 2020 2020 2020 6964  6035)".       id
+00004e50: 3d22 6731 3438 2d30 220a 2020 2020 2020  ="g148-0".      
+00004e60: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+00004e70: 3030 6666 223e 3c70 6174 680a 2020 2020  00ff"><path.    
+00004e80: 2020 2020 2069 643d 2270 6174 6831 3530       id="path150
+00004e90: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+00004ea0: 3d22 6669 6c6c 3a23 3030 3030 6666 3b66  ="fill:#0000ff;f
+00004eb0: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
+00004ec0: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00004ed0: 7374 726f 6b65 3a6e 6f6e 6522 0a20 2020  stroke:none".   
+00004ee0: 2020 2020 2020 643d 224d 2030 2c30 2043        d="M 0,0 C
+00004ef0: 2030 2c30 2e36 3920 302e 3535 392c 312e   0,0.69 0.559,1.
+00004f00: 3234 3820 312e 3234 362c 312e 3234 3820  248 1.246,1.248 
+00004f10: 312e 3933 392c 312e 3234 3820 322e 3530  1.939,1.248 2.50
+00004f20: 322c 302e 3639 2032 2e35 3032 2c30 2032  2,0.69 2.502,0 2
+00004f30: 2e35 3032 2c2d 302e 3639 3220 312e 3933  .502,-0.692 1.93
+00004f40: 392c 2d31 2e32 3531 2031 2e32 3436 2c2d  9,-1.251 1.246,-
+00004f50: 312e 3235 3120 302e 3535 392c 2d31 2e32  1.251 0.559,-1.2
+00004f60: 3531 2030 2c2d 302e 3639 3220 302c 3022  51 0,-0.692 0,0"
+00004f70: 202f 3e3c 2f67 3e3c 670a 2020 2020 2020   /></g><g.      
+00004f80: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00004f90: 736c 6174 6528 3735 372e 3434 3533 2c35  slate(757.4453,5
+00004fa0: 3930 2e34 3931 3729 220a 2020 2020 2020  90.4917)".      
+00004fb0: 2069 643d 2267 3135 322d 3222 0a20 2020   id="g152-2".   
+00004fc0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00004fd0: 2330 3030 3066 6622 3e3c 7061 7468 0a20  #0000ff"><path. 
+00004fe0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00004ff0: 3135 3422 0a20 2020 2020 2020 2020 7374  154".         st
+00005000: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+00005010: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+00005020: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+00005030: 726f 3b73 7472 6f6b 653a 6e6f 6e65 220a  ro;stroke:none".
+00005040: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+00005050: 3020 4320 302c 302e 3639 2030 2e35 3539  0 C 0,0.69 0.559
+00005060: 2c31 2e32 3531 2031 2e32 3436 2c31 2e32  ,1.251 1.246,1.2
+00005070: 3531 2031 2e39 3431 2c31 2e32 3531 2032  51 1.941,1.251 2
+00005080: 2e35 3031 2c30 2e36 3920 322e 3530 312c  .501,0.69 2.501,
+00005090: 3020 322e 3530 312c 2d30 2e36 3931 2031  0 2.501,-0.691 1
+000050a0: 2e39 3431 2c2d 312e 3235 2031 2e32 3436  .941,-1.25 1.246
+000050b0: 2c2d 312e 3235 2030 2e35 3539 2c2d 312e  ,-1.25 0.559,-1.
+000050c0: 3235 2030 2c2d 302e 3639 3120 302c 3022  25 0,-0.691 0,0"
+000050d0: 202f 3e3c 2f67 3e3c 670a 2020 2020 2020   /></g><g.      
+000050e0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000050f0: 736c 6174 6528 3735 372e 3431 362c 3538  slate(757.416,58
+00005100: 352e 3630 3335 2922 0a20 2020 2020 2020  5.6035)".       
+00005110: 6964 3d22 6731 3536 2d34 220a 2020 2020  id="g156-4".    
+00005120: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00005130: 3030 3030 6666 223e 3c70 6174 680a 2020  0000ff"><path.  
+00005140: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00005150: 3538 220a 2020 2020 2020 2020 2073 7479  58".         sty
+00005160: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
+00005170: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00005180: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
+00005190: 6f3b 7374 726f 6b65 3a6e 6f6e 6522 0a20  o;stroke:none". 
+000051a0: 2020 2020 2020 2020 643d 224d 2030 2c30          d="M 0,0
+000051b0: 2043 2030 2c30 2e36 3920 302e 3535 372c   C 0,0.69 0.557,
+000051c0: 312e 3234 3820 312e 3234 342c 312e 3234  1.248 1.244,1.24
+000051d0: 3820 312e 3933 372c 312e 3234 3820 322e  8 1.937,1.248 2.
+000051e0: 3439 392c 302e 3639 2032 2e34 3939 2c30  499,0.69 2.499,0
+000051f0: 2032 2e34 3939 2c2d 302e 3639 3220 312e   2.499,-0.692 1.
+00005200: 3933 372c 2d31 2e32 3531 2031 2e32 3434  937,-1.251 1.244
+00005210: 2c2d 312e 3235 3120 302e 3535 372c 2d31  ,-1.251 0.557,-1
+00005220: 2e32 3531 2030 2c2d 302e 3639 3220 302c  .251 0,-0.692 0,
+00005230: 3022 202f 3e3c 2f67 3e3c 670a 2020 2020  0" /></g><g.    
+00005240: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+00005250: 616e 736c 6174 6528 3736 322e 3336 3034  anslate(762.3604
+00005260: 2c35 3930 2e34 3931 3729 220a 2020 2020  ,590.4917)".    
+00005270: 2020 2069 643d 2267 3136 302d 3822 0a20     id="g160-8". 
+00005280: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00005290: 6c3a 2330 3030 3066 6622 3e3c 7061 7468  l:#0000ff"><path
+000052a0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+000052b0: 7468 3136 3222 0a20 2020 2020 2020 2020  th162".         
+000052c0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+000052d0: 3066 663b 6669 6c6c 2d6f 7061 6369 7479  0ff;fill-opacity
+000052e0: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
+000052f0: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
+00005300: 220a 2020 2020 2020 2020 2064 3d22 4d20  ".         d="M 
+00005310: 302c 3020 4320 302c 302e 3639 2030 2e35  0,0 C 0,0.69 0.5
+00005320: 3539 2c31 2e32 3531 2031 2e32 3437 2c31  59,1.251 1.247,1
+00005330: 2e32 3531 2031 2e39 342c 312e 3235 3120  .251 1.94,1.251 
+00005340: 322e 3530 312c 302e 3639 2032 2e35 3031  2.501,0.69 2.501
+00005350: 2c30 2032 2e35 3031 2c2d 302e 3639 3120  ,0 2.501,-0.691 
+00005360: 312e 3934 2c2d 312e 3235 2031 2e32 3437  1.94,-1.25 1.247
+00005370: 2c2d 312e 3235 2030 2e35 3539 2c2d 312e  ,-1.25 0.559,-1.
+00005380: 3235 2030 2c2d 302e 3639 3120 302c 3022  25 0,-0.691 0,0"
+00005390: 202f 3e3c 2f67 3e3c 670a 2020 2020 2020   /></g><g.      
+000053a0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000053b0: 736c 6174 6528 3736 322e 3332 3831 2c35  slate(762.3281,5
+000053c0: 3835 2e36 3033 3529 220a 2020 2020 2020  85.6035)".      
+000053d0: 2069 643d 2267 3136 342d 3322 0a20 2020   id="g164-3".   
+000053e0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+000053f0: 2330 3030 3066 6622 3e3c 7061 7468 0a20  #0000ff"><path. 
+00005400: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00005410: 3136 3622 0a20 2020 2020 2020 2020 7374  166".         st
+00005420: 796c 653d 2266 696c 6c3a 2330 3030 3066  yle="fill:#0000f
+00005430: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+00005440: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+00005450: 726f 3b73 7472 6f6b 653a 6e6f 6e65 220a  ro;stroke:none".
+00005460: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+00005470: 3020 4320 302c 302e 3639 2030 2e35 3537  0 C 0,0.69 0.557
+00005480: 2c31 2e32 3438 2031 2e32 3436 2c31 2e32  ,1.248 1.246,1.2
+00005490: 3438 2031 2e39 342c 312e 3234 3820 322e  48 1.94,1.248 2.
+000054a0: 3530 322c 302e 3639 2032 2e35 3032 2c30  502,0.69 2.502,0
+000054b0: 2032 2e35 3032 2c2d 302e 3639 3220 312e   2.502,-0.692 1.
+000054c0: 3934 2c2d 312e 3235 3120 312e 3234 362c  94,-1.251 1.246,
+000054d0: 2d31 2e32 3531 2030 2e35 3537 2c2d 312e  -1.251 0.557,-1.
+000054e0: 3235 3120 302c 2d30 2e36 3932 2030 2c30  251 0,-0.692 0,0
+000054f0: 2220 2f3e 3c2f 673e 3c2f 673e 3c2f 673e  " /></g></g></g>
+00005500: 3c67 0a20 2020 7472 616e 7366 6f72 6d3d  <g.   transform=
+00005510: 2274 7261 6e73 6c61 7465 2837 3132 2e34  "translate(712.4
+00005520: 3433 342c 3538 342e 3538 3031 2922 0a20  434,584.5801)". 
+00005530: 2020 6964 3d22 6731 3638 2d39 220a 2020    id="g168-9".  
+00005540: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+00005550: 3030 6666 3b73 7472 6f6b 653a 2330 3030  00ff;stroke:#000
+00005560: 3066 663b 7374 726f 6b65 2d6f 7061 6369  0ff;stroke-opaci
+00005570: 7479 3a31 223e 3c70 6174 680a 2020 2020  ty:1"><path.    
+00005580: 2069 643d 2270 6174 6831 3730 220a 2020   id="path170".  
+00005590: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+000055a0: 3030 3030 6666 3b73 7472 6f6b 653a 2330  0000ff;stroke:#0
+000055b0: 3030 3066 663b 7374 726f 6b65 2d77 6964  000ff;stroke-wid
+000055c0: 7468 3a31 3b73 7472 6f6b 652d 6c69 6e65  th:1;stroke-line
+000055d0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+000055e0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+000055f0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00005600: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00005610: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00005620: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00005630: 643d 224d 2030 2c30 2048 202d 3733 2e34  d="M 0,0 H -73.4
+00005640: 3336 2220 2f3e 3c2f 673e 3c67 0a20 2020  36" /></g><g.   
+00005650: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00005660: 6c61 7465 2837 3132 2e39 3532 312c 3539  late(712.9521,59
+00005670: 312e 3533 3532 2922 0a20 2020 6964 3d22  1.5352)".   id="
+00005680: 6731 3732 2d30 220a 2020 2073 7479 6c65  g172-0".   style
+00005690: 3d22 6669 6c6c 3a23 3030 3030 6666 3b73  ="fill:#0000ff;s
+000056a0: 7472 6f6b 653a 2330 3030 3066 663b 7374  troke:#0000ff;st
+000056b0: 726f 6b65 2d6f 7061 6369 7479 3a31 223e  roke-opacity:1">
+000056c0: 3c70 6174 680a 2020 2020 2069 643d 2270  <path.     id="p
+000056d0: 6174 6831 3734 220a 2020 2020 2073 7479  ath174".     sty
+000056e0: 6c65 3d22 6669 6c6c 3a23 3030 3030 6666  le="fill:#0000ff
+000056f0: 3b73 7472 6f6b 653a 2330 3030 3066 663b  ;stroke:#0000ff;
+00005700: 7374 726f 6b65 2d77 6964 7468 3a31 3b73  stroke-width:1;s
+00005710: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00005720: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00005730: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00005740: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00005750: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00005760: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00005770: 793a 3122 0a20 2020 2020 643d 224d 2030  y:1".     d="M 0
+00005780: 2c30 2048 202d 3733 2e39 3434 2220 2f3e  ,0 H -73.944" />
+00005790: 3c2f 673e 3c67 0a20 2020 7472 616e 7366  </g><g.   transf
+000057a0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2837  orm="translate(7
+000057b0: 3132 2e34 3433 342c 3538 372e 3931 3131  12.4434,587.9111
+000057c0: 2922 0a20 2020 6964 3d22 6731 3736 220a  )".   id="g176".
+000057d0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+000057e0: 3030 3030 6666 3b73 7472 6f6b 653a 2330  0000ff;stroke:#0
+000057f0: 3030 3066 663b 7374 726f 6b65 2d6f 7061  000ff;stroke-opa
+00005800: 6369 7479 3a31 223e 3c70 6174 680a 2020  city:1"><path.  
+00005810: 2020 2069 643d 2270 6174 6831 3738 220a     id="path178".
+00005820: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00005830: 3a23 3030 3030 6666 3b73 7472 6f6b 653a  :#0000ff;stroke:
+00005840: 2330 3030 3066 663b 7374 726f 6b65 2d77  #0000ff;stroke-w
+00005850: 6964 7468 3a31 3b73 7472 6f6b 652d 6c69  idth:1;stroke-li
+00005860: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00005870: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00005880: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00005890: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000058a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000058b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000058c0: 2020 643d 224d 2030 2c30 202d 3733 2e34    d="M 0,0 -73.4
+000058d0: 3133 2c30 2e30 3836 2220 2f3e 3c2f 673e  13,0.086" /></g>
+000058e0: 3c70 6174 680a 2020 2069 643d 2270 6174  <path.   id="pat
+000058f0: 6831 3830 220a 2020 2073 7479 6c65 3d22  h180".   style="
+00005900: 6669 6c6c 3a23 3030 3030 6666 3b66 696c  fill:#0000ff;fil
+00005910: 6c2d 6f70 6163 6974 793a 313b 6669 6c6c  l-opacity:1;fill
+00005920: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
+00005930: 726f 6b65 3a6e 6f6e 6522 0a20 2020 643d  roke:none".   d=
+00005940: 226d 2036 3933 2e30 3737 2c35 3836 2e30  "m 693.077,586.0
+00005950: 3435 2068 2039 2e38 3835 2076 202d 322e  45 h 9.885 v -2.
+00005960: 3933 2068 202d 392e 3838 3520 7a22 202f  93 h -9.885 z" /
+00005970: 3e3c 7061 7468 0a20 2020 6964 3d22 7061  ><path.   id="pa
+00005980: 7468 3138 3222 0a20 2020 7374 796c 653d  th182".   style=
+00005990: 2266 696c 6c3a 2330 3030 3066 663b 6669  "fill:#0000ff;fi
+000059a0: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+000059b0: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+000059c0: 7472 6f6b 653a 6e6f 6e65 220a 2020 2064  troke:none".   d
+000059d0: 3d22 6d20 3637 372e 3030 362c 3538 392e  ="m 677.006,589.
+000059e0: 3532 3520 6820 392e 3838 3320 7620 2d32  525 h 9.883 v -2
+000059f0: 2e39 3320 6820 2d39 2e38 3833 207a 2220  .93 h -9.883 z" 
+00005a00: 2f3e 3c70 6174 680a 2020 2069 643d 2270  /><path.   id="p
+00005a10: 6174 6831 3834 220a 2020 2073 7479 6c65  ath184".   style
+00005a20: 3d22 6669 6c6c 3a23 3030 3030 6666 3b66  ="fill:#0000ff;f
+00005a30: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
+00005a40: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00005a50: 7374 726f 6b65 3a6e 6f6e 6522 0a20 2020  stroke:none".   
+00005a60: 643d 226d 2036 3932 2e38 3535 2c35 3933  d="m 692.855,593
+00005a70: 2e32 3239 2068 2039 2e38 3833 2076 202d  .229 h 9.883 v -
+00005a80: 322e 3933 2068 202d 392e 3838 3320 7a22  2.93 h -9.883 z"
+00005a90: 202f 3e3c 2f67 3e3c 2f67 3e3c 2f67 3e0a   /></g></g></g>.
+00005aa0: 3c67 0a20 2020 6964 3d22 6731 3434 220a  <g.   id="g144".
+00005ab0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+00005ac0: 616e 736c 6174 6528 3133 2e37 3537 3939  anslate(13.75799
+00005ad0: 382c 2d32 2e34 3733 3534 3539 2922 3e0a  8,-2.4735459)">.
+00005ae0: 3c2f 673e 0a3c 670a 2020 2069 643d 2267  </g>.<g.   id="g
+00005af0: 3134 3622 0a20 2020 7472 616e 7366 6f72  146".   transfor
+00005b00: 6d3d 2274 7261 6e73 6c61 7465 2831 332e  m="translate(13.
+00005b10: 3735 3739 3938 2c2d 322e 3437 3335 3435  757998,-2.473545
+00005b20: 3929 223e 0a3c 2f67 3e0a 3c67 0a20 2020  9)">.</g>.<g.   
+00005b30: 6964 3d22 6731 3438 220a 2020 2074 7261  id="g148".   tra
+00005b40: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00005b50: 6528 3133 2e37 3537 3939 382c 2d32 2e34  e(13.757998,-2.4
+00005b60: 3733 3534 3539 2922 3e0a 3c2f 673e 0a3c  735459)">.</g>.<
+00005b70: 670a 2020 2069 643d 2267 3135 3022 0a20  g.   id="g150". 
+00005b80: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00005b90: 6e73 6c61 7465 2831 332e 3735 3739 3938  nslate(13.757998
+00005ba0: 2c2d 322e 3437 3335 3435 3929 223e 0a3c  ,-2.4735459)">.<
+00005bb0: 2f67 3e0a 3c67 0a20 2020 6964 3d22 6731  /g>.<g.   id="g1
+00005bc0: 3532 220a 2020 2074 7261 6e73 666f 726d  52".   transform
+00005bd0: 3d22 7472 616e 736c 6174 6528 3133 2e37  ="translate(13.7
+00005be0: 3537 3939 382c 2d32 2e34 3733 3534 3539  57998,-2.4735459
+00005bf0: 2922 3e0a 3c2f 673e 0a3c 670a 2020 2069  )">.</g>.<g.   i
+00005c00: 643d 2267 3135 3422 0a20 2020 7472 616e  d="g154".   tran
+00005c10: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00005c20: 2831 332e 3735 3739 3938 2c2d 322e 3437  (13.757998,-2.47
+00005c30: 3335 3435 3929 223e 0a3c 2f67 3e0a 3c67  35459)">.</g>.<g
+00005c40: 0a20 2020 6964 3d22 6731 3536 220a 2020  .   id="g156".  
+00005c50: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00005c60: 736c 6174 6528 3133 2e37 3537 3939 382c  slate(13.757998,
+00005c70: 2d32 2e34 3733 3534 3539 2922 3e0a 3c2f  -2.4735459)">.</
+00005c80: 673e 0a3c 670a 2020 2069 643d 2267 3135  g>.<g.   id="g15
+00005c90: 3822 0a20 2020 7472 616e 7366 6f72 6d3d  8".   transform=
+00005ca0: 2274 7261 6e73 6c61 7465 2831 332e 3735  "translate(13.75
+00005cb0: 3739 3938 2c2d 322e 3437 3335 3435 3929  7998,-2.4735459)
+00005cc0: 223e 0a3c 2f67 3e0a 3c67 0a20 2020 6964  ">.</g>.<g.   id
+00005cd0: 3d22 6731 3630 220a 2020 2074 7261 6e73  ="g160".   trans
+00005ce0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00005cf0: 3133 2e37 3537 3939 382c 2d32 2e34 3733  13.757998,-2.473
+00005d00: 3534 3539 2922 3e0a 3c2f 673e 0a3c 670a  5459)">.</g>.<g.
+00005d10: 2020 2069 643d 2267 3136 3222 0a20 2020     id="g162".   
+00005d20: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00005d30: 6c61 7465 2831 332e 3735 3739 3938 2c2d  late(13.757998,-
+00005d40: 322e 3437 3335 3435 3929 223e 0a3c 2f67  2.4735459)">.</g
+00005d50: 3e0a 3c67 0a20 2020 6964 3d22 6731 3634  >.<g.   id="g164
+00005d60: 220a 2020 2074 7261 6e73 666f 726d 3d22  ".   transform="
+00005d70: 7472 616e 736c 6174 6528 3133 2e37 3537  translate(13.757
+00005d80: 3939 382c 2d32 2e34 3733 3534 3539 2922  998,-2.4735459)"
+00005d90: 3e0a 3c2f 673e 0a3c 670a 2020 2069 643d  >.</g>.<g.   id=
+00005da0: 2267 3136 3622 0a20 2020 7472 616e 7366  "g166".   transf
+00005db0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
+00005dc0: 332e 3735 3739 3938 2c2d 322e 3437 3335  3.757998,-2.4735
+00005dd0: 3435 3929 223e 0a3c 2f67 3e0a 3c67 0a20  459)">.</g>.<g. 
+00005de0: 2020 6964 3d22 6731 3638 220a 2020 2074    id="g168".   t
+00005df0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00005e00: 6174 6528 3133 2e37 3537 3939 382c 2d32  ate(13.757998,-2
+00005e10: 2e34 3733 3534 3539 2922 3e0a 3c2f 673e  .4735459)">.</g>
+00005e20: 0a3c 670a 2020 2069 643d 2267 3137 3022  .<g.   id="g170"
+00005e30: 0a20 2020 7472 616e 7366 6f72 6d3d 2274  .   transform="t
+00005e40: 7261 6e73 6c61 7465 2831 332e 3735 3739  ranslate(13.7579
+00005e50: 3938 2c2d 322e 3437 3335 3435 3929 223e  98,-2.4735459)">
+00005e60: 0a3c 2f67 3e0a 3c67 0a20 2020 6964 3d22  .</g>.<g.   id="
+00005e70: 6731 3732 220a 2020 2074 7261 6e73 666f  g172".   transfo
+00005e80: 726d 3d22 7472 616e 736c 6174 6528 3133  rm="translate(13
+00005e90: 2e37 3537 3939 382c 2d32 2e34 3733 3534  .757998,-2.47354
+00005ea0: 3539 2922 3e0a 3c2f 673e 0a3c 2f73 7667  59)">.</g>.</svg
+00005eb0: 3e0a                                     >.
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.9.0/itkdb_gtk/ITkDBlogin.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 
         if self.token:
             self.T.start()
             return
 
         if gtk_runs:
             self.create_window()
+            self.present()
             self.run()
 
         else:
             access1 = getpass.getpass("Access 1: ")
             access2 = getpass.getpass("Access 2: ")
             self.user._access_code1 = access1
             self.user._access_code2 = access2
@@ -249,15 +250,14 @@
 
         self.show_all()
 
     def complain(self, main_title, second_text):
         """Opens an error dialog.
 
         Args:
-        ----
             main_title: Main text in window
             second_text: Second text
 
         """
         dialog = Gtk.MessageDialog(
             transient_for=self,
             flags=0,
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.9.0/itkdb_gtk/ITkDButils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     return db_response
 
 
 def get_db_date(timestamp=None):
     """Convert a date string into the expected DB format.
 
     Args:
-    ----
         timestamp: A date in string format
 
     """
     def date2string(the_date):
         out = the_date.isoformat(timespec='milliseconds')
         if out[-1] not in ['zZ']:
             out += 'Z'
@@ -77,21 +76,19 @@
     return out
 
 
 def registerPetalCore(client, SN, alias, HC_id=None):
     """Register a Petal Core in the DB.
 
     Args:
-    ----
         SN: Serial Number
         alias: The alias of the Petal
         HC_id: Comma separated list of HC identifiers.
 
-    Returns
-    -------
+    Returns:
         _type_: _description_
 
     """
     global db_response
     dto = {
         "project": 'S',
         "subproject": "SE",
@@ -112,15 +109,14 @@
         return None
 
 
 def create_component_attachment(client, SN, file_path, title=None, description="", item_type="component"):
     """Create an attachment to the given component.
 
     Args:
-    ----
         client: The DB client
         SN: The SN of the component.
         file_path: The pat to th efile to be attached.
         title: title of the file
         description: Description of the attachment
         item_type: the type of DB object to attach the information
 
@@ -163,15 +159,14 @@
     return db_response
 
 
 def set_component_property(client, SN, property, value):
     """Set the value of an object property.
 
     Args:
-    ----
         client: The DB client
         SN: The object SN
         property: The property name
         value: The property value
 
     """
     global db_response
@@ -188,15 +183,14 @@
         return None
 
 
 def assemble_component(client, parent, child):
     """Assemble child into parent.
 
     Args:
-    ----
         client: The DB client
         parent: The parent object or container.
         child: The child to be assembled.
 
     """
     global db_response
     try:
@@ -210,15 +204,14 @@
         return None
 
 
 def set_object_stage(client, SN, stage):
     """Set stage of object
 
     Args:
-    ----
         client: DB session
         SN: Serial number
         stage: Stage
 
     """
     global db_response
     try:
@@ -231,46 +224,49 @@
             SN, stage, str(e)))
         return None
 
 
 def get_DB_component(client, SN):
     """Get ta component by its serial number."""
     global db_response
-    db_response = client.get('getComponent', json={'component': SN})
-    return db_response
+    try:
+        db_response = client.get('getComponent', json={'component': SN})
+        return db_response
 
+    except Exception as e:
+        db_response = str(e)
+        return None
 
 def upload_test(client, data, attachments=None):
     """Upload a test to the DB.
 
     Args:
-    ----
         client: The DB client
         data (dict): A dictionary with all the elements of thee test.
-        attachments (Attachments): one or more (in a list) Attachments to the test
+        attachments ([Attachment]): one or more (in a list) Attachment to the test
 
     Return:
-    ------
         resp: The response of the DB session.
 
     """
     global db_response
     try:
         db_response = client.post("uploadTestRunResults", json=data)
+        testRun = db_response["testRun"]["id"]
         if attachments is not None:
             if not isinstance(attachments, Iterable):
                 attachments = (attachments)
 
             for att in attachments:
                 path = Path(att.path).expanduser().resolve()
                 if not path.exists():
                     print("File {} does not exist".format(path))
                     continue
 
-                data = {"testRun": db_response["testRun"]["id"],
+                data = {"testRun": testRun,
                         "title": att.title if att.title is not None else path.name,
                         "description": att.desc if att.desc is not None else path.name,
                         "type": "file",
                         }
                 filetype = mimetypes.guess_type(path.name)
                 attachment = {'data': (path.name, open(path.as_posix(), 'rb'), filetype[0])}
                 db_response = client.post('createTestRunAttachment',
@@ -279,28 +275,27 @@
 
         return None
 
     except Exception as e:
         return (str(e))
 
 
-def create_shipment(session, sender, recipient, items, name=None, send=False, type="domestic",
-                    attachment=None, comments=None):
+def create_shipment(session, sender, recipient, items, name=None, send=False, 
+                    type="domestic", attachment=None, comments=None):
     """Create a chipment.
 
     Args:
-    ----
         session : The itkdb session
         sender : The sender ID
         recipient : The recipient ID
         items : A list of SN of the items to be shipped.
         name: the name of the shipment.
         send: If true, the status of the shipment is updated to inTransit
         type (optional): Type of shipment. Defaults to "domestic".
-        attachment (optional): Attachment object.
+        attachment (optional, :class:`Attachment`): :class:`Attachment` object.
         comments (optional): comments for the shipment
 
     """
     global db_response
     if name is None:
         name = "From {} to {}".format(sender, recipient)
 
@@ -428,15 +423,14 @@
     return test
 
 
 def get_testrun(session, test_id, out_type="object"):
     """Retrieve information about a given test.
 
     Args:
-    ----
         session : The itkdb session
         test_id : The ID of the test.
         out_type (optional): Type of output (full or object). Defaults to "object".
 
     """
     global db_response
     try:
@@ -447,15 +441,14 @@
         return None
 
 
 def get_test_skeleton(session, component, test_code, userdef={}, uservalues={}):
     """Get the skeleton of the given test.
 
     Args:
-    ----
         session: The DB session
         component: The component which is tested
         test_code: The test code
         userdef: default values of test parameters, propertines and results.
         uservalues: default values for different types.
 
     """
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/ShowAttachments.py` & `itkdb_gtk-0.9.0/itkdb_gtk/ShowDefects.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,103 @@
-from pathlib import Path
+
 try:
-    import dbGtkUtils
-    import ITkDButils
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDButils
+    import itkdb_gtk
+    
+except ImportError:
+    import sys
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import dbGtkUtils
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio, Gdk
 
 
-def add_attachment_dialog():
-    """Create the add attachment dialog."""
-    dlg = Gtk.Dialog(title="Add Attachment")
-    dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
-                    Gtk.STOCK_OK, Gtk.ResponseType.OK)
-    grid = Gtk.Grid(column_spacing=5, row_spacing=1)
-    box = dlg.get_content_area()
-    box.add(grid)
-
-    lbl = Gtk.Label(label="File")
-    lbl.set_xalign(0)
-    grid.attach(lbl, 0, 0, 1, 1)
-
-    lbl = Gtk.Label(label="Title")
-    lbl.set_xalign(0)
-    grid.attach(lbl, 0, 1, 1, 1)
-
-    lbl = Gtk.Label(label="Description")
-    lbl.set_xalign(0)
-    grid.attach(lbl, 0, 2, 1, 1)
-
-    dlg.fC = Gtk.FileChooserButton()
-    grid.attach(dlg.fC, 1, 0, 1, 1)
-
-    dlg.att_title = Gtk.Entry()
-    grid.attach(dlg.att_title, 1, 1, 1, 1)
-
-    dlg.att_desc = Gtk.Entry()
-    grid.attach(dlg.att_desc, 1, 2, 1, 1)
-
-    dlg.show_all()
-    return dlg
-
-
-class ShowAttachments(Gtk.Dialog):
-    """Window to show attachments."""
-    def __init__(self, title, session, attachments=[], parent=None):
+class ShowDefects(Gtk.Dialog):
+    """Edit defects"""
+    
+    def __init__(self, title, defects=None, parent=None):
         """Initialization."""
         super().__init__(title=title, transient_for=parent)
-        self.session = session
-        self.attachments = [A for A in attachments]
+        if defects:
+            self.defects = [C for C in defects]
+        else:
+            self.defects = []
+            
         self.init_window()
 
     def init_window(self):
-        """Prepares the window."""
+        """Preapare the window."""
         self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                          Gtk.STOCK_OK, Gtk.ResponseType.OK)
 
         self.mainBox = self.get_content_area()
         # The "Add attachment" button.
         box = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL)
         self.mainBox.pack_start(box, False, False, 0)
 
-        dbGtkUtils.add_button_to_container(box, "Add attachment",
-                                           "Click to add a new attachment.",
-                                           self.add_attachment)
-
-        dbGtkUtils.add_button_to_container(box, "Remove attachment",
-                                           "Click to remove selected attachment.",
-                                           self.remove_attachment)
+        dbGtkUtils.add_button_to_container(box, "Add Defect",
+                                           "Click to add a new defect.",
+                                           self.add_defect)
+
+        dbGtkUtils.add_button_to_container(box, "Remove Defect",
+                                           "Click to remove selected defect.",
+                                           self.remove_defect)
 
         # the list of attachments
         tree_view = self.create_tree_view()
         self.mainBox.pack_start(tree_view, True, True, 0)
-        for A in self.attachments:
-            self.append_attachment_to_view(A)
+        for C in self.defects:
+            self.append_defect_to_view(C)
 
         self.show_all()
 
     def create_tree_view(self, size=150):
-        """Creates the tree vew with the attachments."""
-        model = Gtk.ListStore(str, str, str, str)
+        """Create the tree view."""
+        model = Gtk.ListStore(str, str)
         self.tree = Gtk.TreeView(model=model)
         scrolled = Gtk.ScrolledWindow()
         scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
         scrolled.add(self.tree)
         scrolled.set_size_request(-1, size)
 
         renderer = Gtk.CellRendererText()
-        column = Gtk.TreeViewColumn("Attachment", renderer, text=0)
-        self.tree.append_column(column)
-
-        renderer = Gtk.CellRendererText()
-        column = Gtk.TreeViewColumn("Title", renderer, text=1)
+        column = Gtk.TreeViewColumn("Defect Type", renderer, text=0)
         self.tree.append_column(column)
 
         renderer = Gtk.CellRendererText()
-        column = Gtk.TreeViewColumn("Description", renderer, text=2)
+        column = Gtk.TreeViewColumn("Description", renderer, text=1)
         self.tree.append_column(column)
 
         return scrolled
 
-    def add_attachment(self, *args):
-        """Add Attachment button clicked."""
-        dlg = add_attachment_dialog()
-        rc = dlg.run()
-        if rc == Gtk.ResponseType.OK:
-            path = Path(dlg.fC.get_filename())
-            A = ITkDButils.Attachment(path, dlg.att_title.get_text().strip(), dlg.att_desc.get_text().strip())
-            self.append_attachment_to_view(A)
-            self.attachments.append(A)
+    def add_defect(self, *args):
+        """A new defect."""
+        values = dbGtkUtils.get_a_list_of_values("Insert new defect", ("Type", "Description/v"))
+        if len(values):
+            defect = {"name": values[0], "description": values[1]}
+            self.defects.append(defect)
+            self.append_defect_to_view(defect)
 
-        dlg.hide()
-        dlg.destroy()
-
-    def append_attachment_to_view(self, A):
-        """Insert attachment to tree view."""
-        model = self.tree.get_model()
-        model.append([A.path.name, A.title, A.desc, A.path.as_posix()])
-
-    def remove_attachment(self, *args):
-        """Remove selected attachment."""
+    def remove_defect(self, *args):
+        """Remove a defect."""
         select = self.tree.get_selection()
         model, iter = select.get_selected()
         if iter:
             values = model[iter]
-            for a in self.attachments:
-                if a.path == values[3]:
-                    rc = dbGtkUtils.ask_for_confirmation("Remove this attachment ?",
-                                                         "{} - {}\n{}".format(a.title, a.desc, values[0]))
+            for C in self.defects:
+                if C["name"] == values[0] and C["description"] == values[1]:
+                    rc = dbGtkUtils.ask_for_confirmation("Remove this Defect ?",
+                                                         "{}\n{}\n".format(values[0], values[1]))
                     if rc:
-                        self.attachments.remove(a)
+                        self.defects.remove(C)
                         model.remove(iter)
 
                     break
+
+    def append_defect_to_view(self, C):
+        """Append a new defect to the triee view."""
+        model = self.tree.get_model()
+        model.append([C["name"], C["description"]])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/ShowComments.py` & `itkdb_gtk-0.9.0/itkdb_gtk/ShowComments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+#!/usr/bin/env python3
+"""Shows comments."""
+
 try:
-    import dbGtkUtils
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils
+    import itkdb_gtk
+    
+except ImportError:
+    import sys
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+    
+from itkdb_gtk import dbGtkUtils
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio, Gdk
 
 
 class ShowComments(Gtk.Dialog):
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/__init__.py` & `itkdb_gtk-0.9.0/itkdb_gtk/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,57 @@
-from . import dashBoard
-
-__version__ = "0.0.9"
+__version__ = "0.9.0"
 
 
 def dash_board():
     """Launches the dash board."""
+    from .dashBoard import main
     dashBoard.main()
 
 
 def getShipments():
     """getShipments."""
-    from .getShipments import main
+    from .GetShipments import main
     main()
 
 
 def glueWeight():
     """glue weight."""
     from .GlueWeight import main
     main()
 
 
-def groundingTest():
+def groundVITests():
     """GND/VI tests."""
-    from .groundingTest import main
+    from .GroundVITests import main
     main()
 
 
-def sendShipments():
+def createShipments():
     """Send items."""
-    from .sendShipments import main
+    from .CreateShipments import main
     main()
 
-
 def uploadTest():
-    """Upload tests."""
-    from .uploadTest import main
+    """Upload a single tests."""
+    from .UploadTest import main
     main()
 
 
 def uploadMultipleTests():
     """Upload multiple tests."""
-    from .uploadMultipleTests import main
+    from .UploadMultipleTests import main
+    main()
+
+def uploadModuleIV():
+    """Upload IV files of single and double modules"""
+    from .UploadModuleIV import main
+    main()
+
+def wirebondTest():
+    """Inputs data and eventually upload wirebod test."""
+    from .WireBondGui import main
+    main()
+
+def uploadPetalInformation():
+    """Read files from AVS nd create Petal core in PDB."""
+    from .UploadPetalInformation import main
     main()
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.9.0/itkdb_gtk/dashBoard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 #!/usr/bin/env python3
 """Test dashboard."""
 import sys
 
 try:
-    import dbGtkUtils
-    import getShipments
-    import groundingTest
-    import ITkDBlogin
-    import sendShipments
-    import uploadMultipleTests
-    import GlueWeight
-
-except Exception:
-    from itkdb_gtk import dbGtkUtils, getShipments, groundingTest, ITkDBlogin, sendShipments, uploadMultipleTests, GlueWeight
+    import itkdb_gtk
+    
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+    
+    
+from itkdb_gtk import dbGtkUtils
+from itkdb_gtk import GetShipments
+from itkdb_gtk import GroundVITests
+from itkdb_gtk import ITkDBlogin
+from itkdb_gtk import CreateShipments
+from itkdb_gtk import UploadTest
+from itkdb_gtk import UploadMultipleTests
+from itkdb_gtk import GlueWeight
+from itkdb_gtk import UploadModuleIV
+from itkdb_gtk import WireBondGui
 
 import gi
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 
 
 class DashWindow(dbGtkUtils.ITkDBWindow):
     """Dashboard class."""
-
+    UPLOAD_TEST = 1
+    UPLOAD_MANY_TESTS = 2
+    CREATE_SHIPMNT = 3
+    RECV_SHIPMNT = 4
+    PETAL_GND = 5
+    GLUE_WEIGHT = 6
+    MOD_IV = 7
+    WIRE_BOND = 8
+    
     def __init__(self, session):
         """Initialization."""
         super().__init__(title="ITkDB Dashboard", session=session)
         self.mask = 0
 
         # set border width
         self.set_border_width(10)
@@ -42,26 +58,41 @@
         irow = 0
         lbl = Gtk.Label()
         lbl.set_markup("<b>Tests</b>")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, irow, 1, 1)
 
         irow += 1
-        btnTest = Gtk.Button(label="Upload Tests (json)")
+        btnTest = Gtk.Button(label="Upload Single Test")
         btnTest.connect("clicked", self.upload_test)
         grid.attach(btnTest, 0, irow, 1, 1)
 
+        btnTest = Gtk.Button(label="Upload Multiple Tests")
+        btnTest.connect("clicked", self.upload_multiple_tests)
+        grid.attach(btnTest, 1, irow, 1, 1)
+
+        irow += 1
         btnGnd = Gtk.Button(label="Petal VI/GND")
         btnGnd.connect("clicked", self.petal_gnd)
-        grid.attach(btnGnd, 1, irow, 1, 1)
+        grid.attach(btnGnd, 0, irow, 1, 1)
 
-        irow += 1
         btnWeight = Gtk.Button(label="GlueWeight")
         btnWeight.connect("clicked", self.glue_weight)
-        grid.attach(btnWeight, 0, irow, 1, 1)
+        grid.attach(btnWeight, 1, irow, 1, 1)
+
+        irow += 1
+        btnModIV = Gtk.Button(label="Module IV")
+        btnModIV.connect("clicked", self.module_IV)
+        grid.attach(btnModIV, 0, irow, 1, 1)
+
+        btnWireBond = Gtk.Button(label="Wire Bond")
+        btnWireBond.connect("clicked", self.wire_bond)
+        grid.attach(btnWireBond, 1, irow, 1, 1)
+
+
 
         irow += 1
         grid.attach(Gtk.Label(), 0, irow, 1, 1)
 
         irow += 1
         lbl = Gtk.Label()
         lbl.set_markup("<b>Shipments</b>")
@@ -79,72 +110,105 @@
 
         self.mainBox.pack_start(Gtk.Separator(orientation=Gtk.Orientation.HORIZONTAL), False, True, 5)
 
         self.show_all()
 
     def upload_test(self, *args):
         """Launch upload test."""
-        bitn = 1
+        bitn = DashWindow.UPLOAD_TEST
+        bt = 1 << bitn
+        if self.mask & bt:
+            return
+
+        self.mask |= bt
+        W = UploadTest.UploadTest(self.session)
+        W.connect("destroy", self.app_closed, bitn)
+
+    def upload_multiple_tests(self, *args):
+        """Launch upload multiple test."""
+        bitn = DashWindow.UPLOAD_MANY_TESTS
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = uploadMultipleTests.UploadMultipleTests(self.session)
+        W = UploadMultipleTests.UploadMultipleTests(self.session)
         W.connect("destroy", self.app_closed, bitn)
 
     def create_shipment(self, *args):
-        """Launch sendShipment."""
-        bitn = 2
+        """Launch createShipment."""
+        bitn = DashWindow.CREATE_SHIPMNT
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = sendShipments.SendShipments(self.session)
+        W = CreateShipments.CreateShipments(self.session)
         W.connect("destroy", self.app_closed, bitn)
 
     def receive_shipment(self, *args):
         """Launch getShipments."""
-        bitn = 3
+        bitn = DashWindow.RECV_SHIPMNT
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = getShipments.ReceiveShipments(self.session)
+        W = GetShipments.ReceiveShipments(self.session)
         W.connect("destroy", self.app_closed, bitn)
 
     def petal_gnd(self, *args):
         """Petal GND/VI test."""
-        bitn = 4
+        bitn = DashWindow.PETAL_GND
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = groundingTest.GroundingTest(self.session)
+        W = GroundVITests.GroundingTest(self.session)
         W.connect("destroy", self.app_closed, bitn)
 
     def glue_weight(self, *args):
         """Glue Weight test."""
-        bitn = 5
+        bitn = DashWindow.GLUE_WEIGHT
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
         W = GlueWeight.GlueWeight(self.session)
         W.connect("destroy", self.app_closed, bitn)
 
+    def module_IV(self, *args):
+        """Module IV tests."""
+        bitn = DashWindow.MOD_IV
+        bt = 1 << bitn
+        if self.mask & bt:
+            return
+
+        self.mask |= bt
+        W = UploadModuleIV.IVwindow(self.session)
+        W.connect("destroy", self.app_closed, bitn)
+
+    def wire_bond(self, *args):
+        """Module IV tests."""
+        bitn = DashWindow.WIRE_BOND
+        bt = 1 << bitn
+        if self.mask & bt:
+            return
+
+        self.mask |= bt
+        W = WireBondGui.WireBond(session=self.session, title="Wirebond")
+        W.connect("destroy", self.app_closed, bitn)
+
     def app_closed(self, *args):
         """Application window closed. Clear mask."""
         bt = 1 << args[1]
         self.mask &= ~bt
-        print(bt, self.mask)
+        # print(bt, self.mask)
 
 
 def main():
     # DB login
     dlg = ITkDBlogin.ITkDBlogin()
     client = dlg.get_client()
     if client is None:
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.9.0/itkdb_gtk/dbGtkUtils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,41 +3,80 @@
 import time
 from collections.abc import Iterable
 from copy import deepcopy
 from datetime import datetime
 
 import dateutil.parser
 import gi
+import numpy as np
+
 
 gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gio, GLib
+from gi.repository import Gtk, GObject, Gio, GLib
 
+def parse_date(txt):
+    """Parse a date."""
+    try:
+        return dateutil.parser.parse(txt, fuzzy=False)
+
+    except Exception:
+        return None
+def parse_date_as_string(txt):
+    """Parse data and return DB compatible string."""
+    D = parse_date(txt)
+    if D is None:
+        return D
+
+    out = D.isoformat(timespec='milliseconds')
+    if out[-1] not in ['zZ']:
+        out += 'Z'
 
-def set_combo_iter(combo, txt, col=0):
-    """Set scombo active iter to that containing txt in column col."""
-    model = combo.get_model()
-    iter = model.get_iter_first()
-    while iter:
-        val = model.get_value(iter, col)
-        if val == txt:
-            combo.set_active_iter(iter)
-            break
+    return out
 
-        iter = model.iter_next(iter)
+def is_a_date(txt):
+    """check tha the input string is a date."""
+    try:
+        dateutil.parser.parse(txt, fuzzy=False)
+        return True
+
+    except Exception:
+        return False
 
+def new_small_text_entry():
+    """Returs a new, smaller Gtk.Entry."""
+    entry = Gtk.Entry()
+    provider = Gtk.CssProvider()
+    style_context = entry.get_style_context()
+    font_size = 2.25*style_context.get_property("font-size", 0)
+    css = "entry {{ min-height: {}px; }}".format(font_size)
+    provider.load_from_data(css.encode())
+    style_context.add_provider(provider, Gtk.STYLE_PROVIDER_PRIORITY_SETTINGS)
+    return entry
 
 def set_entry_style(container):
     """Set max entry."""
     provider = Gtk.CssProvider()
-    print(container.get_name())
     style_context = container.get_style_context()
     font_size = 2.25*style_context.get_property("font-size", 0)
     css = "{} {{ min-height: {}px; }}".format(container.get_name(), font_size)
     provider.load_from_data(css.encode())
     style_context.add_provider(provider, Gtk.STYLE_PROVIDER_PRIORITY_SETTINGS)
+    return container    
+
+def set_combo_iter(combo, txt, col=0):
+    """Set scombo active iter to that containing txt in column col."""
+    model = combo.get_model()
+    iter = model.get_iter_first()
+    while iter:
+        val = model.get_value(iter, col)
+        if val == txt:
+            combo.set_active_iter(iter)
+            break
+
+        iter = model.iter_next(iter)
 
 
 def is_iterable(obj):
     """Tell if an object is iterable. Strings are not considered iterables."""
     if isinstance(obj, Iterable):
         if isinstance(obj, str) or isinstance(obj, bytes):
             return False
@@ -51,36 +90,40 @@
     """To truncate the number of decimals in floats."""
 
     def default(self, o):
         """Format floats or deletate to JSonEncoder."""
         if isinstance(o, datetime):
             text = o.astimezone().isoformat()
             return text
+        elif isinstance(o, np.integer):
+            return int(o)
+        elif isinstance(o, np.floating):
+            return float(o)
+        elif isinstance(o, np.ndarray):
+            return o.tolist()
         else:
             return super().default(o)
 
 
 def empty_container(container):
     """Remove all children from a container.
 
     Args:
-    ----
         container: The container.
 
     """
     chilren = [C for C in container.get_children()]
     for C in chilren:
         container.remove(C)
 
 
 def replace_in_container(container, child):
     """Replace a child from a single-child container.
 
     Args:
-    ----
         container: the container
         child: the new child to be added
 
     """
     empty_container(container)
     if isinstance(container, Gtk.Box):
         container.pack_end(child, True, True, 0)
@@ -89,15 +132,14 @@
     container.show_all()
 
 
 def complain(main_title, second_text="", parent=None):
     """Open an error dialog.
 
     Args:
-    ----
         main_title: Main text in window
         second_text: Second text
         parent: dialog parent
 
     """
     dialog = Gtk.MessageDialog(
         transient_for=parent,
@@ -111,21 +153,19 @@
     dialog.destroy()
 
 
 def ask_for_confirmation(main_title, second_text, parent=None):
     """Ask for action cofirmation.
 
     Args:
-    ----
         main_title: Main title in the message window
         second_text: Secondary text in the message widow
         parent (optional): The parent window. Defaults to None.
 
     Return:
-    ------
         OK: True if OK button clicked.
 
     """
     dialog = Gtk.MessageDialog(
         transient_for=parent,
         flags=0,
         message_type=Gtk.MessageType.INFO,
@@ -134,74 +174,106 @@
     dialog.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL, Gtk.STOCK_OK, Gtk.ResponseType.OK)
     dialog.format_secondary_text(second_text)
     out = dialog.run()
     dialog.destroy()
     return (out == Gtk.ResponseType.OK)
 
 
-class TextEntry(object):
+class TextEntry(GObject.GObject):
     """Create a Gtk text entry/view object."""
+    __gsignals__ = {
+        "text_changed": (GObject.SIGNAL_RUN_FIRST, None, (str,))
+    }
 
-    def __init__(self, n_lines=1):
+    def __init__(self, n_lines=1, small=False):
         """Init."""
+        GObject.GObject.__init__(self)
+        self.tmp_txt = ""
         self.nlines = n_lines
         if self.nlines > 1:
             self.widget = Gtk.Frame()
             scrolled = Gtk.ScrolledWindow()
             scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
             scrolled.set_hexpand(True)
             scrolled.set_vexpand(True)
 
             self.widget.add(scrolled)
             self.entry = Gtk.TextView()
             scrolled.add(self.entry)
 
         else:
-            self.widget = Gtk.Entry()
+            if small:
+                self.widget = new_small_text_entry()
+            else:
+                self.widget = Gtk.Entry()
+                
+            self.widget.connect("focus-in-event", self.on_enter)
+            self.widget.connect("focus-out-event", self.on_leave)
+
             self.entry = self.widget
 
+    def do_my_signal(self, *args):
+        """Signal handler."""
+        pass
+
+    def on_enter(self, *args):
+        """On enter."""
+        self.tmp_txt = self.widget.get_text().strip()
+        return False
+
+    def on_leave(self, *args):
+        """On leave."""
+        val = self.widget.get_text().strip()
+        if val != self.tmp_txt:
+            self.emit("text_changed", val)
+
     def get_text(self):
         """Return the text."""
         if self.nlines > 1:
             buff = self.entry.get_buffer()
             start = buff.get_start_iter()
             end = buff.get_end_iter()
             return buff.get_text(start, end, False)
 
         else:
             return self.entry.get_text()
 
+    def set_text(self, text):
+        """Sets text."""
+        if self.nlines > 1:
+            self.entry.get_buffer().set_text(text)
+        else:
+            self.entry.set_text(text)
+
 
 def get_a_value(main_title, second_text=None, is_tv=False, parent=None):
     """Open a dialog to get a value.
 
     Args:
-    ----
         main_title: Main title in the message window
         is_tv: If true show a text view rathar than an entry.
         second_text: Secondary text in the message widow
         parent (optional): The parent window. Defaults to None.
 
     Return:
-    ------
         value: The value in the entry
 
     """
     dlg = Gtk.Dialog(title="Add Attachment",
                      transient_for=parent,
                      flags=0)
     dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                     Gtk.STOCK_OK, Gtk.ResponseType.OK)
     area = dlg.get_content_area()
     box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
     area.add(box)
 
-    box.pack_start(Gtk.Label(main_title), False, True, 0)
+    box.pack_start(Gtk.Label(label=main_title), False, True, 0)
     if second_text and len(second_text):
-        box.pack_start(Gtk.Label(second_text), False, True, 0)
+        box.pack_start(Gtk.Label(label=second_text), False, True, 0)
 
     entry = TextEntry(3 if is_tv else -1)
 
     box.pack_start(entry.widget, False, True, 0)
     dlg.show_all()
 
     rc = dlg.run()
@@ -212,26 +284,25 @@
 
     dlg.hide()
     dlg.destroy()
 
     return out
 
 
-def get_a_list_of_values(main_title, labels, second_text=None, parent=None):
+def get_a_list_of_values(main_title, labels, defaults=None, second_text=None, parent=None):
     """Get a list of values.
 
     Args:
-    ----
         main_title: Main title for window
         labels: List of labes to get the values. If the label ends with /v
                 then a TextView will be shown instead of a TextEntry.
+        defaults (optional): default values-
         second_text (optional): Second title for window-. Defaults to None.
 
-    Returns
-    -------
+    Returns:
         list with values
 
     """
     dlg = Gtk.Dialog(title="Get List of values",
                      transient_for=parent,
                      flags=0)
 
@@ -241,35 +312,40 @@
     box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
     area.pack_start(box, False, True, 2)
 
     lbl = Gtk.Label()
     lbl.set_markup("<b>{}</b>".format(main_title))
     box.pack_start(lbl, False, True, 5)
     if second_text and len(second_text):
-        box.pack_start(Gtk.Label(second_text), False, True, 0)
+        box.pack_start(Gtk.Label(label=second_text), False, True, 0)
 
     entries = []
     values = []
     is_text_view = []
     vbox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
     area.pack_start(vbox, False, True, 0)
-    for txt in labels:
+    for i, txt in enumerate(labels):
         use_tv = False
         if txt.endswith("/v"):
             is_text_view.append(True)
             use_tv = True
             txt = txt[:-2]
         else:
             is_text_view.append(False)
 
-        lbl = Gtk.Label(txt)
+        lbl = Gtk.Label(label=txt)
         lbl.set_justify(Gtk.Justification.LEFT)
         vbox.pack_start(lbl, False, False, 0)
 
         entry = TextEntry(3 if use_tv else -1)
+        try:
+            entry.set_text(defaults[i])
+        except Exception:
+            pass
+
         vbox.pack_start(entry.widget, False, False, 0)
         entries.append(entry)
 
     dlg.show_all()
     rc = dlg.run()
     if rc == Gtk.ResponseType.OK:
         for entry, is_tv in zip(entries, is_text_view):
@@ -280,15 +356,14 @@
     return values
 
 
 def add_button_to_container(box, label, tooltip=None, callback=None):
     """Creates a buttons and adds to container.
 
     Args:
-    ----
         box: The container.
         label: The button label
         tooltip (optional): Tooltip message. Defaults to None.
         callback (optional): callback function. Defaults to None.
 
     """
     btn = Gtk.Button(label=label)
@@ -297,40 +372,99 @@
         btn.set_tooltip_text(tooltip)
 
     if callback:
         btn.connect("clicked", callback)
 
     box.pack_start(btn, True, False, 0)
 
+    return btn
+
+
+class MessagePanel(object):
+    """Encapsulates a TExtView object to show messages."""
+
+    def __init__(self, size=100):
+        """Initializarion."""
+        self.frame = None
+        self.text_view = Gtk.TextView()
+        self.textbuffer = self.text_view.get_buffer()
+
+        self.__create_message_panel(size)
+
+
+    def __create_message_panel(self, size):
+        """Creates a message panel within a frame.
+
+        Args:
+            size: size of the panel
+
+        Returns:
+            Gtk.TextBuffer, Gtk.Frame
+        """
+        frame = Gtk.Frame()
+        frame.set_shadow_type(Gtk.ShadowType.IN)
+
+        box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
+        box.set_size_request(-1, size)
+        frame.add(box)
+
+        # The title for the tet view
+        box.pack_start(Gtk.Label(label="Messages"), False, True, 0)
+
+        # A scroll window with the text view
+        scrolled = Gtk.ScrolledWindow()
+        scrolled.set_policy(Gtk.PolicyType.AUTOMATIC, Gtk.PolicyType.AUTOMATIC)
+        scrolled.add(self.text_view)
+        box.pack_start(scrolled, True, True, 0)
+        self.frame = frame
+
+    def scroll_to_end(self):
+        """Scrolls text view to end."""
+        end = self.textbuffer.get_end_iter()
+        self.text_view.scroll_to_iter(end, 0, False, 0, 0)
+
+    def write_message(self, text):
+        """Writes text to Text Viewer."""
+        nlines = self.textbuffer.get_line_count()
+        if nlines > 100:
+            start = self.textbuffer.get_iter_at_line(0)
+            end = self.textbuffer.get_iter_at_line(75)
+            self.textbuffer.delete(start, end)
+
+        end = self.textbuffer.get_end_iter()
+        msg = "[{}]  {}".format(time.strftime("%d/%m/%y %T"), text)
+        self.textbuffer.insert(end, msg)
+        GLib.idle_add(self.scroll_to_end)
+
 
 class ITkDBWindow(Gtk.Window):
     """Base class for GUI main windows."""
 
-    def __init__(self, title="", session=None, show_search=None, gtk_runs=True):
+    def __init__(self, title="", session=None, show_search=None, gtk_runs=True, panel_size=100):
         """Initialization.
 
         Args:
-        ----
             title: The title of the window.
             session: ITkDB session.
             show_search: tooltip for search button in header (calls to query_db).
                          No search button if this is None.
             gtk_runs: If False, Gtk could not be loaded and app should be
                       terminal only.
 
         """
         self.session = session
         self.inst2code = {}
         self.code2inst = {}
+        self.message_panel = None
 
         if gtk_runs:
             super().__init__(title=title)
-            self.prepare_window(show_search)
+            self.prepare_window(show_search, panel_size)
 
-    def prepare_window(self, show_search):
+    def prepare_window(self, show_search, panel_size):
         """Inititalizes GUI."""
         # Prepare HeaderBar
         self.hb = Gtk.HeaderBar()
         self.hb.set_show_close_button(True)
         self.set_titlebar(self.hb)
 
         self.userLabel = Gtk.Button.new_with_label(self.session.user.name)
@@ -347,19 +481,21 @@
             button.add(image)
             button.set_tooltip_text(show_search)
             button.connect("clicked", self.query_db)
             self.hb.pack_end(button)
 
         # Create main content box
         self.mainBox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
+        self.mainBox.set_property("margin-left", 6)
+        self.mainBox.set_property("margin-right", 6)
+
         self.add(self.mainBox)
 
         # The text view and buffer
-        self.text_view = Gtk.TextView()
-        self.textbuffer = self.text_view.get_buffer()
+        self.message_panel = MessagePanel(size=panel_size)
 
         # The button box
         btnBox = Gtk.ButtonBox(orientation=Gtk.Orientation.HORIZONTAL)
 
         btn = Gtk.Button(label="Quit")
         btn.connect("clicked", self.quit)
         btnBox.add(btn)
@@ -374,15 +510,16 @@
     def query_db(self, *args):
         """Search button clicked."""
         pass
 
     def new_login(self, obj, msg):
         """A new user logged in."""
         if msg == "<OK>":
-            self.session = self.session.user_gui.get_client()
+            if hasattr(self.session, "user_gui"):
+                self.session = self.session.user_gui.get_client()
             self.userLabel.get_child().set_text(self.session.user.name)
 
         else:
             self.write_message("Could not login.\n{}".format(msg))
 
     def reconnect(self, *args):
         """Reconnects."""
@@ -446,54 +583,45 @@
         scrolled = Gtk.ScrolledWindow()
         scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
         scrolled.add(self.text_view)
         box.pack_start(scrolled, True, True, 0)
 
         return frame
 
-    def scroll_to_end(self):
-        """Scrolls text view to end."""
-        end = self.textbuffer.get_end_iter()
-        self.text_view.scroll_to_iter(end, 0, False, 0, 0)
-
     def write_message(self, text):
         """Writes text to Text Viewer."""
-        nlines = self.textbuffer.get_line_count()
-        if nlines > 100:
-            start = self.textbuffer.get_iter_at_line(0)
-            end = self.textbuffer.get_iter_at_line(75)
-            self.textbuffer.delete(start, end)
-
-        end = self.textbuffer.get_end_iter()
-        msg = "[{}]  {}".format(time.strftime("%d/%m/%y %T"), text)
-        self.textbuffer.insert(end, msg)
-        GLib.idle_add(self.scroll_to_end)
+        self.message_panel.write_message(text)
 
 
 class DictDialog(Gtk.Grid):
     """Creates a dialog to show and edit variables in a JSon dict."""
 
-    def __init__(self, values, hidden_keys={}):
+    def __init__(self, values, hidden_keys=None):
         """Create the Gtk.Grid.
 
         Args:
-        ----
             values: A dict (JSon-like)
             hidden_keys: keys tha twill not be shown.
 
         """
         super().__init__(column_spacing=5, row_spacing=1)
 
         self.set_border_width(10)
+        self.factory = deepcopy(values)
         self.values = deepcopy(values)
         self.keys = {}
         self.containers = {}
-        self.hidden_keys = hidden_keys
+        self.hidden_keys = hidden_keys if hidden_keys else {}
         self.show_values()
 
+    def factory_reset(self):
+        """Set values to original values."""
+        self.values = deepcopy(self.factory)
+        self.refresh()
+
     def on_enter(self, entry, *args):
         """Get the value when we first enter into the Entry."""
         self.keys[args[2]] = entry.get_text()
 
     def on_leave(self, entry, event, value, name):
         """Check, when leaving the entry, if the value has changed."""
         def str2bool(v):
@@ -515,14 +643,23 @@
 
             elif isinstance(itm[last_key], bool):
                 itm[last_key] = str2bool(txt)
 
             elif isinstance(itm[last_key], datetime):
                 itm[last_key] = dateutil.parser.parse(txt)
 
+            elif is_a_date(itm[last_key]):
+                D = dateutil.parser.parse(txt)
+                out = D.isoformat(timespec='milliseconds')
+                if out[-1] not in ['zZ']:
+                    out += 'Z'
+
+                itm[last_key] = out
+                self.containers[name].set_text(out)
+
             else:
                 tp = type(itm[last_key])
                 itm[last_key] = tp(txt)
 
     def show_item(self, value, name=None):
         """Handle a single item."""
         if isinstance(value, list) or isinstance(value, tuple):
@@ -577,15 +714,14 @@
         except KeyError:
             complain("Key {} does not exist in DictDialog".format(key))
 
     def show_values(self):
         """Show the keys and values of a dictionary (JSON).
 
         Args:
-        ----
             values: The dictionary object
 
         """
         irow = 0
         self.set_row_spacing(5)
         for key, value in self.values.items():
             if key in self.hidden_keys:
@@ -611,16 +747,18 @@
         self.show_all()
         self.queue_draw()
 
 
 def create_scrolled_dictdialog(the_dict, hidden=("component", "testType")):
     """Create a DictDialog within a scrolled window.
 
-    Return:
-    ------
+    Args:
+        the_dict: the input dictionary with values.
+        
+    Returns:
         scrolled: the scrolled window
         gM: the DictDialog
 
     """
     gM = DictDialog(the_dict, hidden)
     scrolled = Gtk.ScrolledWindow()
     scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.9.0/itkdb_gtk/GetShipments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 """GEt shipments to a particular site (default is IFIC)."""
 import pathlib
 import sys
 
 try:
-    import dbGtkUtils
-    import ITkDBlogin
-    import ITkDButils
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+    import itkdb_gtk
+    
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
 
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
 import gi
 import serial
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio, GLib
 
 # Check if Gtk can be open
@@ -23,15 +25,14 @@
 class ReceiveShipments(dbGtkUtils.ITkDBWindow):
     """Find shipments related to given recipient."""
 
     def __init__(self, session, recipient="IFIC"):
         """Initialization.
 
         Args:
-        ----
             session: ITkDB session.
             recipient: default recipient
 
         """
         self.recipient = recipient
         self.state = "inTransit"
         self.institute = None
@@ -121,16 +122,15 @@
         self.mainBox.pack_start(paned, True, True, 0)
 
         # The main TreeView
         tree_view = self.create_tree_view()
         paned.add1(tree_view)
 
         # The text view
-        frame = self.create_text_view()
-        paned.add2(frame)
+        paned.add2(self.message_panel.frame)
 
         self.show_all()
 
     def create_tree_view(self, size=150):
         """Create a tree view with the shipment items."""
         store = Gtk.ListStore(str, str, str, bool)
         self.tree = Gtk.TreeView(model=store)
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.9.0/itkdb_gtk/GroundVITests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 #!/usr/bin/env python3
 """Test dashboard."""
 import json
 import sys
 
 try:
-    import dbGtkUtils
-    import ITkDBlogin
-    import ITkDButils
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+    import itkdb_gtk
+    
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
 
-import gi
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
 
+import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio
 
 
+def find_children(W):
+    """Find DictDialog among the children."""
+    try:
+        for c in W.get_children():
+            if "DictDialog" in c.get_name():
+                return c
+
+            else:
+                return find_children(c)
+
+    except Exception:
+        return None
+
+    return None
+
+
 class GroundingTest(dbGtkUtils.ITkDBWindow):
     """Dashboard class."""
 
     def __init__(self, session):
         """Initialization."""
         super().__init__(title="ITkDB Dashboard",
                          session=session,
@@ -29,28 +47,36 @@
         self.dbObject = None
 
         # action button in header
         button = Gtk.Button()
         icon = Gio.ThemedIcon(name="document-send-symbolic")
         image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
         button.add(image)
-        button.set_tooltip_text("Click to upload tests.")
+        button.set_tooltip_text("Click to upload ALL tests.")
         button.connect("clicked", self.upload_tests)
         self.hb.pack_end(button)
 
         grid = Gtk.Grid(column_spacing=5, row_spacing=1)
         self.mainBox.pack_start(grid, False, False, 5)
 
         lbl = Gtk.Label(label="Serial Number")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, 0, 1, 1)
 
         self.SN = Gtk.Entry()
+        self.SN.connect("focus-in-event", self.on_sn_enter)
+        self.SN.connect("focus-out-event", self.on_sn_leave)
         grid.attach(self.SN, 1, 0, 1, 1)
 
+        self.alias = Gtk.Label(label="")
+        grid.attach(self.alias, 2, 0, 1, 1)
+
+        self.stage = Gtk.Label(label="")
+        grid.attach(self.stage, 3, 0, 1, 1)
+
         lbl = Gtk.Label(label="Institute")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, 1, 1, 1)
 
         self.institute = "IFIC"
         inst = self.create_institute_combo()
         inst.connect("changed", self.new_institute)
@@ -58,38 +84,61 @@
         grid.attach(inst, 1, 1, 1, 1)
         self.inst_cmb = inst
 
         # The "Add/Remove/Send Item" buttons.
         box = Gtk.ButtonBox(orientation=Gtk.Orientation.HORIZONTAL)
         box.set_layout(Gtk.ButtonBoxStyle.END)
         self.mainBox.pack_start(box, False, False, 0)
+        dbGtkUtils.add_button_to_container(box, "Upload test", "Upload this test", self.upload_single_test)
         dbGtkUtils.add_button_to_container(box, "Add Defect", "Click to add a defect", self.add_defect)
         dbGtkUtils.add_button_to_container(box, "Add Comment", "Click to add a comment", self.add_comment)
 
         # The notebook
         self.notebook = Gtk.Notebook()
         self.notebook.set_tab_pos(Gtk.PositionType.LEFT)
         self.notebook.set_size_request(-1, 250)
         self.mainBox.pack_start(self.notebook, True, True, 0)
 
         # Create the Notebook pages
         self.create_test_box("Visual Inspection", "VISUAL_INSPECTION")
         self.create_test_box("Grounding", "GROUNDING_CHECK")
+        self.create_test_box("Pipe bending", "BENDING120")
 
         # The text view
-        frame = self.create_text_view()
-        self.mainBox.pack_end(frame, True, True, 5)
+        self.mainBox.pack_end(self.message_panel.frame, True, True, 5)
 
         self.show_all()
 
+    def on_sn_enter(self, entry, *args):
+        """Enter in SN entry."""
+        self._sn = entry.get_text()
+
+    def on_sn_leave(self, entry, *args):
+        """Leave SN entry."""
+        sn = entry.get_text()
+        if sn != self._sn:
+            self.query_db()
+            current_location = self.dbObject["currentLocation"]["code"]
+            dbGtkUtils.set_combo_iter(self.inst_cmb, current_location, 0)
+
+            stg = self.dbObject["currentStage"]["name"]
+            self.stage.set_text(stg)
+
+            alias = self.dbObject["alternativeIdentifier"]
+            self.alias.set_text(alias)
+
+            npages = self.notebook.get_n_pages()
+            for i in range(npages):
+                page = self.notebook.get_nth_page(i)
+                page.dict_dialog.factory_reset()
+
     def create_test_box(self, label, test_name, institute="IFIC"):
         """Create and add to notebook a test dialog.
 
         Args:
-        ----
             label: The label for the Notebook
             test_name: The DB name of the test
             institute: The institute.
 
         """
         defaults = {
             "institution": institute,
@@ -155,51 +204,60 @@
 
             npages = self.notebook.get_n_pages()
             for i in range(npages):
                 page = self.notebook.get_nth_page(i)
                 page.dict_dialog.values["institution"] = self.institute
                 page.dict_dialog.refresh()
 
-    def upload_tests(self, *args):
+    def upload_single_test(self, *args):
         """Upload the current test."""
         SN = self.SN.get_text()
         if len(SN) == 0:
             dbGtkUtils.complain("Petal SN is empty")
             return
 
-        def find_children(W):
-            try:
-                for c in W.get_children():
-                    if "DictDialog" in c.get_name():
-                        return c
-
-                    else:
-                        return find_children(c)
-
-            except Exception:
-                return None
-
-            return None
-
         page = self.notebook.get_nth_page(self.notebook.get_current_page())
         dctD = find_children(page)
         if dctD is None:
             return
 
         values = dctD.values
         values["component"] = SN
-        print(json.dumps(values, indent=2))
+        # print(json.dumps(values, indent=2))
         rc = ITkDButils.upload_test(self.session, values)
         if rc is not None:
             dbGtkUtils.complain("Could not upload test", rc)
 
         else:
             dbGtkUtils.ask_for_confirmation("Test uploaded.",
                                             "{} - {}".format(values["component"], values["testType"]))
 
+    def upload_tests(self, *args):
+        """Upload the current test."""
+        SN = self.SN.get_text()
+        if len(SN) == 0:
+            dbGtkUtils.complain("Petal SN is empty")
+            return
+
+        for ipage in range(self.notebook.get_n_pages()):
+            page = self.notebook.get_nth_page(ipage)
+            dctD = find_children(page)
+            if dctD is None:
+                continue
+
+            values = dctD.values
+            values["component"] = SN
+            # print(json.dumps(values, indent=2))
+            rc = ITkDButils.upload_test(self.session, values)
+            if rc is not None:
+                dbGtkUtils.complain("Could not upload test", rc)
+
+            else:
+                self.write_message("Test uploaded. {} - {}\n".format(values["component"], values["testType"]))
+
 
 def main():
     """Main entry."""
     # DB login
     dlg = ITkDBlogin.ITkDBlogin()
     client = dlg.get_client()
     if client is None:
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.9.0/itkdb_gtk/readAVSdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env pythoon3
 """Read AVS dats file."""
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 
 try:
-    import ITkDBlogin
-    import ITkDButils
-except ModuleNotFoundError:
-    from itkdb_gtk import ITkDBlogin, ITkDButils
+    import itkdb_gtk
+    
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import ITkDBlogin, ITkDButils
 
 import dateutil.parser
 import openpyxl as XL
 from openpyxl.cell.cell import MergedCell
 from openpyxl.utils.exceptions import InvalidFileException
 
 sk_defaults = {
@@ -29,15 +33,14 @@
         super().__init__(message)
 
 
 def create_weight(session, SN, the_date=None, manager="", passed=True, problems=False, comments=[]):
     """Creates the dictionary for a WEIGHT test.
 
     Args:
-    ----
         session: the DB session
         SN: Serial Number
         the_date: the date of the test
         manager: manager name
         passed: if test passed or not
         problems: if problems were found during test
         comments: list of comments to append to the test
@@ -54,15 +57,14 @@
     return out
 
 
 def create_manufacturing(session, SN, the_date=None, manager="", passed=True, problems=False, comments=[]):
     """Create the dictionary or the MANUFACTURING test.
 
     Args:
-    ----
         session: the DB session
         SN: Serial Number
         the_date: the date of the test
         manager: manager name
         passed: if test passed or not
         problems: if problems were found during test
         comments: list of comments to append to the test
@@ -94,15 +96,14 @@
     return out
 
 
 def create_delamination_test(session, SN, the_date=None, operator="", passed=True, problems=False, comments=[]):
     """Create the delamination test JSON.
 
     Args:
-    ----
         session: the DB session
         SN: Serial Number
         the_date: the date of the test
         operator: operator name
         passed: if test passed or not
         problems: if problems were found during test
         comments: list of comments to append to the test
@@ -120,15 +121,14 @@
     return out
 
 
 def create_grounding_test(session, SN, the_date=None, operator="", passed=True, problems=False, comments=[]):
     """Create grounding test.
 
     Args:
-    ----
         session: the DB session
         SN: Serial Number
         the_date: the date of the test
         operator: operator name
         passed: if test passed or not
         problems: if problems were found during test
         comments: list of comments to append to the test
@@ -146,15 +146,14 @@
     return out
 
 
 def create_metrology_test(session, SN, the_date=None, operator="", passed=True, problems=False, comments=[]):
     """Metrology test.
 
     Args:
-    ----
         session: the DB session
         SN: Serial Number
         the_date: the date of the test
         operator: operator name
         passed: if test passed or not
         problems: if problems were found during test
         comments: list of comments to append to the test
@@ -308,15 +307,14 @@
     return SN
 
 
 def readFATfile(session, fnam, SN=None):
     """Read data from FAT excel file.
 
     Args:
-    ----
         session: the DB session
         fnam: File path
         SN: COre serial number
 
     """
     # Open spreadsheet
     try:
@@ -455,15 +453,14 @@
     return vi_test, delamination_test, grounding_test, metrology_test, batch, petal_weight
 
 
 def readProductionSheet(session, fnam, SN):
     """Read data fro AVS PS.
 
     Args:
-    ----
         session: the DB session
         fnam: path of input file
         SN: The serial number
         write_json: if true, test json is writen to file.
 
     """
     try:
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.9.0/itkdb_gtk/readGoogleSheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from googleapiclient.discovery import build
 
 # If modifying these scopes, delete the file token.json.
 SCOPES = ['https://www.googleapis.com/auth/spreadsheets.readonly']
 
 
 # Get spreadsheet ID from share link
-re_sheet_id = re.compile(r"https://docs.google.com/spreadsheets/d/(?P<ID>\w+)", re.DOTALL)
+re_sheet_id = re.compile(r"https://docs.google.com/spreadsheets/d/(?P<ID>[\w-]+)", re.DOTALL)
 
 
 def get_spreadsheet_service():
     """Return the spreadsheet service."""
     creds = None
     # The file token.json stores the user's access and refresh tokens, and is
     # created automatically when the authorization flow completes for the first
@@ -51,15 +51,14 @@
     return spread_sheet_id
 
 
 def get_spreadsheet_data(url, data_range):
     """Get the data from the given range in teh google sheet.
 
     Args:
-    ----
         url: google sheet document url
         data_range: the data range, ej. inventory!A2:Z
 
     """
     service = get_spreadsheet_service()
 
     spread_sheet_id = get_sheet_id(url)
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.9.0/itkdb_gtk/CreateShipments.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,37 +3,39 @@
 
 Items can be added via a QR reader.
 """
 import pathlib
 import sys
 
 try:
-    import dbGtkUtils
-    import ITkDBlogin
-    import ITkDButils
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+    import itkdb_gtk
+    
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
 
 import gi
 import serial
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio, GLib
 
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
 
 
-class SendShipments(dbGtkUtils.ITkDBWindow):
+class CreateShipments(dbGtkUtils.ITkDBWindow):
     """Create a shipment from input."""
 
     def __init__(self, session):
         """Initialization.
 
         Args:
-        ----
             session: ITkDB session.
 
         """
         self.model = None
         self.tree = None
         self.shipments = {}
         self.attachment = None
@@ -121,16 +123,15 @@
         self.mainBox.pack_start(paned, True, True, 0)
 
         # The list of items
         tree_view = self.create_tree_view()
         paned.add1(tree_view)
 
         # The text view
-        frame = self.create_text_view()
-        paned.add2(frame)
+        paned.add2(self.message_panel.frame)
 
         self.show_all()
 
     def create_tree_view(self, size=150):
         """Creates tree view with the list of items."""
         model = self.get_tree_view_model()
         self.tree = Gtk.TreeView(model=model)
@@ -367,15 +368,15 @@
     client = dlg.get_client()
     if client is None:
         print("Could not connect to DB with provided credentials.")
         dlg.die()
         sys.exit()
 
     client.user_gui = dlg
-    IS = SendShipments(client)
+    IS = CreateShipments(client)
     IS.set_accept_focus(True)
     IS.present()
     IS.connect("destroy", Gtk.main_quit)
 
     try:
         Gtk.main()
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/uploadMultipleTests.py` & `itkdb_gtk-0.9.0/itkdb_gtk/UploadMultipleTests.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 import fnmatch
 import json
 import os
 import sys
 from pathlib import Path
 
 try:
-    import dbGtkUtils
-    import ITkDBlogin
-    import ITkDButils
-    from ShowComments import ShowComments
-    from ShowAttachments import ShowAttachments
-    from ShowDefects import ShowDefects
-    from uploadTest import create_json_data_editor
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
-    from itkdb_gtk.ShowComments import ShowComments
-    from itkdb_gtk.ShowAttachments import ShowAttachments
-    from itkdb_gtk.ShowDefects import ShowDefects
-    from itkdb_gtk.uploadTest import create_json_data_editor
+    import itkdb_gtk
+
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+from itkdb_gtk.ShowComments import ShowComments
+from itkdb_gtk.ShowAttachments import ShowAttachments
+from itkdb_gtk.ShowDefects import ShowDefects
+from itkdb_gtk.UploadTest import create_json_data_editor
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio, Gdk
 
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
@@ -36,22 +35,20 @@
     return the_date
 
 
 def all_files(root, patterns='*', single_level=False, yield_folders=False):
     """A generator that reruns all files in the given folder.
 
     Args:
-    ----
         root (file path): The folder
         patterns (str, optional): The pattern of the files. Defaults to '*'.
         single_level (bool, optional): If true, do not go into sub folders. Defaults to False.
         yield_folders (bool, optional): If True, return folders as well. Defaults to False.
 
-    Yields
-    ------
+    Yields:
         str: file path name
 
     """
     patterns = patterns.split(';')
     for path, subdirs, files in os.walk(root):
         if yield_folders:
             files.extend(subdirs)
@@ -64,25 +61,24 @@
                     break
 
         if single_level:
             break
 
 
 class TestList(object):
-    SN, TestType, RunNumber, Date, Institute, Path, Json, Nattch, Attachments, Ncomm, Comments, Ndef, Defects, ALL = range(14)
+    SN, TestType, RunNumber, Date, Institute, Stage, currentStage, Path, Json, Nattch, Attachments, Ncomm, Comments, Ndef, Defects, ALL = range(16)
 
 
 def check_data(data):
     """Checks validity of JSon data.
 
     Args:
-    ----
         data (): The json data
 
-    Returns
+    Returns:
     -------
         boolean: True if valid, False otherwise.
 
     """
     errors = []
     missing = []
     if "component" not in data:
@@ -107,15 +103,14 @@
 class UploadMultipleTests(dbGtkUtils.ITkDBWindow):
     """Collects information to upload a test and its attachments."""
 
     def __init__(self, session):
         """Initialization.
 
         Args:
-        ----
             session: ITkDB session
 
         """
         super().__init__(session=session, title="Upload Tests", gtk_runs=gtk_runs)
         self.tests = []
 
         self.init_window()
@@ -168,22 +163,21 @@
         self.mainBox.pack_start(paned, True, True, 5)
 
         # the list of attachments
         tree_view = self.create_tree_view()
         paned.add1(tree_view)
 
         # The text view
-        frame = self.create_text_view()
-        paned.add2(frame)
+        paned.add2(self.message_panel.frame)
 
         self.show_all()
 
     def create_tree_view(self, size=150):
         """Creates the tree vew with the attachments."""
-        model = Gtk.ListStore(str, str, str, str, str, str, object, int, object, int, object, int, object)
+        model = Gtk.ListStore(str, str, str, str, str, str, str, str, object, int, object, int, object, int, object)
         self.tree = Gtk.TreeView(model=model)
         self.tree.connect("button-press-event", self.button_pressed)
         scrolled = Gtk.ScrolledWindow()
         scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
         scrolled.add(self.tree)
         scrolled.set_size_request(-1, size)
 
@@ -200,14 +194,18 @@
         self.tree.append_column(column)
 
         renderer = Gtk.CellRendererText()
         column = Gtk.TreeViewColumn("Institute", renderer, text=TestList.Institute)
         self.tree.append_column(column)
 
         renderer = Gtk.CellRendererText()
+        column = Gtk.TreeViewColumn("Stage", renderer, text=TestList.Stage)
+        self.tree.append_column(column)
+
+        renderer = Gtk.CellRendererText()
         column = Gtk.TreeViewColumn("N. att.", renderer, text=TestList.Nattch)
         self.tree.append_column(column)
 
         renderer = Gtk.CellRendererText()
         column = Gtk.TreeViewColumn("N. comm.", renderer, text=TestList.Ncomm)
         self.tree.append_column(column)
 
@@ -226,15 +224,16 @@
         # double click shows attachments
         if event.button == 1 and event.type == Gdk.EventType.DOUBLE_BUTTON_PRESS:
             select = self.tree.get_selection()
             model, iter = select.get_selected()
             if not iter:
                 return
 
-            self.on_show_attachments(None, (model, iter, model[iter]))
+            self.on_show_json(None, (model, iter, model[iter]))
+            # self.on_show_attachments(None, (model, iter, model[iter]))
             return
 
         if event.button != 3:
             return
 
         # Create popup menu
         select = self.tree.get_selection()
@@ -254,14 +253,18 @@
             return
 
         menu = Gtk.Menu()
         item_show = Gtk.MenuItem(label="Show JSOn")
         item_show.connect("activate", self.on_show_json, (model, iter, values))
         menu.append(item_show)
 
+        item_set_stage = Gtk.MenuItem(label="Set Stage")
+        item_set_stage.connect("activate", self.on_set_stage, (model, iter, values))
+        menu.append(item_set_stage)
+
         item_show_att = Gtk.MenuItem(label="Edit Attachments")
         item_show_att.connect("activate", self.on_show_attachments, (model, iter, values))
         menu.append(item_show_att)
 
         item_show_com = Gtk.MenuItem(label="Edit Comments")
         item_show_com.connect("activate", self.on_show_comments, (model, iter, values))
         menu.append(item_show_com)
@@ -282,16 +285,19 @@
         model, iter, val = data
         payload = val[TestList.Json]
         value, dlg = create_json_data_editor(payload)
         rc = dlg.run()
         if rc == Gtk.ResponseType.OK:
             payload = value.values
             model.set_value(iter, TestList.Json, payload)
+            model.set_value(iter, TestList.SN, payload["component"])
             model.set_value(iter, TestList.RunNumber, payload["runNumber"])
             model.set_value(iter, TestList.Date, handle_test_date(payload["date"]))
+            model.set_value(iter, TestList.Institute, handle_test_date(payload["institution"]))
+
 
         dlg.hide()
         dlg.destroy()
 
     def on_show_attachments(self, item, data):
         """Show the attachmetns."""
         model, iter, val = data
@@ -361,14 +367,74 @@
             out = self.get_institute_from_combo(combo)
 
         use_default = btn.get_active()
         dlg.hide()
         dlg.destroy()
         return out, use_default
 
+    def on_set_stage(self, item, data):
+        """Set the test stage."""
+        model, iter, val = data
+        SN = val[TestList.SN]
+        combo, currentStage = self.get_component_stages(SN)
+
+        dlg = Gtk.Dialog(title="Add Attachment")
+
+        dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
+                        Gtk.STOCK_OK, Gtk.ResponseType.OK)
+        area = dlg.get_content_area()
+        box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
+        area.add(box)
+
+        box.pack_start(Gtk.Label(label="Select Stage"), False, True, 0)
+        box.pack_start(combo, False, True, 0)
+        dlg.show_all()
+
+        rc = dlg.run()
+        if rc == Gtk.ResponseType.OK:
+            new_stage = combo.get_active_text()
+            model[iter][TestList.Stage] = new_stage
+            data = model[iter][TestList.Json]
+            changed = (new_stage != model[iter][TestList.currentStage])
+            data["isRetroactive"] = changed
+            if changed:
+                data["stage"] = new_stage
+            else:
+                if "stage" in data:
+                    del data["stage"]
+
+            model[iter][TestList.Json] = data
+
+
+        dlg.hide()
+        dlg.destroy()
+
+
+    def get_component_stages(self, SN):
+        """Create a combo with the stages."""
+        try:
+            obj = ITkDButils.get_DB_component(self.session, SN)
+            currentStage = obj["currentStage"]["code"]
+
+            combo = Gtk.ComboBoxText.new_with_entry()
+            combo.remove_all()
+            indx = 0
+            for i, stg in enumerate(obj["stages"]):
+                S = stg["code"]
+                combo.append_text(S)
+                if S == currentStage:
+                    indx = i
+
+            combo.set_active(indx)
+            return combo, currentStage
+
+        except Exception:
+            self.write_message("Something went wring with the stages")
+            return [None, None]
+
     def add_tests_to_view(self, files):
         """Add the input fiels to the treeview."""
         default_site = None
         for ifile in files:
             try:
                 has_errors = False
                 data = json.loads(open(ifile).read())
@@ -413,16 +479,18 @@
                         # We need to delete tis, which is "unofficial"
                         del data["attachments"]
 
                     model = self.tree.get_model()
                     comments = data.get("comments", [])
                     defects = data.get("defects", [])
                     the_date = handle_test_date(data["date"])
+                    combo, currentStage = self.get_component_stages(data["component"])
                     model.append([data["component"], data["testType"], data["runNumber"], the_date,
-                                  data["institution"], ifile, data, len(attachments), attachments,
+                                  data["institution"], currentStage, currentStage,
+                                  ifile, data, len(attachments), attachments,
                                   len(comments), comments, len(defects), defects])
 
             except Exception as E:
                 self.write_message("Cannot load file {}\n".format(ifile))
                 self.write_message("{}\n".format(str(E)))
 
     def on_select_folder(self, *args):
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.9.0/itkdb_gtk/UploadPetalInformation.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 import dateutil.parser
 import gi
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio
 
 try:
-    import readAVSdata
-    import ITkDBlogin
-    import ITkDButils
-
-    from dbGtkUtils import replace_in_container, complain, DictDialog, ask_for_confirmation
-
-except ModuleNotFoundError:
-    from itkdb_gtk import readAVSdata, ITkDBlogin, ITkDButils
-    from itkdb_gtk.dbGtkUtils import replace_in_container, complain, DictDialog, ask_for_confirmation
+    import itkdb_gtk
+
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import readAVSdata, ITkDBlogin, ITkDButils
+from itkdb_gtk.dbGtkUtils import replace_in_container, complain, DictDialog, ask_for_confirmation
 
 
 def create_scrolled_dictdialog(the_dict, hidden=("component", "testType")):
     """Create a DictDialog within a scrolled window.
 
     Return:
     ------
@@ -40,19 +40,17 @@
     return scrolled, gM
 
 
 def get_type(child):
     """Return object type
 
     Args:
-    -----
         child (): object
 
-    Returns
-    -------
+    Returns:
         str: object type
 
     """
     if child["type"] is not None:
         ctype = child["type"]["code"]
     else:
         ctype = child["componentType"]["code"]
@@ -225,21 +223,19 @@
         self.mainBox.pack_start(btnBox, False, True, 0)
         self.connect("destroy", Gtk.main_quit)
 
     def create_test_window(self, test_json, test_name, label):
         """Create the dialog for a DB test and add it to the notebook.
 
         Args:
-        ----
             test_json: The JSon-like dict with the values
             test_name: The name of the test for internal indexing
             label: The label for the Notebook
 
-        Return:
-        ------
+        Returns:
             The box containing the data.
 
         """
         scrolled, gM = create_scrolled_dictdialog(test_json)
         self.test_list.append(gM)
         self.test_index[test_name] = len(self.test_list) - 1
         self.test_map[test_json["testType"]] = test_name
@@ -257,18 +253,17 @@
     def update_scroll_window(self, key, data):
         """Update panel for a given test."""
         scrolled, gM = create_scrolled_dictdialog(data, ("component", "testType"))
         self.test_list[self.test_index[key]] = gM
         replace_in_container(self.test_panel[key], scrolled)
 
     def check_register_petal(self, SN):
-        """Register teal core in DB.
+        """Register petal core in DB.
 
         Args:
-        ----
             SN: The petal Serial Number.
 
         """
         if self.petal_core:
             return
 
         self.find_petal(SN, silent=True)
@@ -606,15 +601,16 @@
             values = test.values
             print(values["testType"])
             res = ITkDButils.upload_test(self.db_session, values)
             if res is not None:
                 complain("Could not upload test {}".format(values["testType"]), res)
 
 
-if __name__ == "__main__":
+def main():
+    """The main entry."""
     # Parse command line options
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
     parser.add_argument("--SN", dest="SN", type=str, default=None,
                         help="Module serial number")
     parser.add_argument("--PS", dest="PS", type=str, default=None,
                         help="Produc tion Sheet file")
@@ -636,7 +632,10 @@
         Gtk.main()
     except KeyboardInterrupt:
         print("Arrggggg !!!")
 
     print("Bye !!")
     dlg.die()
     sys.exit()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.9.0/itkdb_gtk/UploadTest.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 """GUI to upload tests."""
 import argparse
 import json
 import sys
 from pathlib import Path
 
 try:
-    import dbGtkUtils
-    import ITkDBlogin
-    import ITkDButils
-    from ShowComments import ShowComments
-    from ShowAttachments import ShowAttachments
-    from ShowDefects import ShowDefects
-
-except ModuleNotFoundError:
-    from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
-    from itkdb_gtk.ShowComments import ShowComments
-    from itkdb_gtk.ShowAttachments import ShowAttachments
-    from itkdb_gtk.ShowDefects import ShowDefects
+    import itkdb_gtk
+
+except ImportError:
+    from pathlib import Path
+    cwd = Path(sys.argv[0]).parent.parent
+    sys.path.append(cwd.as_posix())
+
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+from itkdb_gtk.ShowComments import ShowComments
+from itkdb_gtk.ShowAttachments import ShowAttachments
+from itkdb_gtk.ShowDefects import ShowDefects
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio
 
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
@@ -45,19 +44,17 @@
     return value, dlg
 
 
 def check_data(data):
     """Checks validity of JSon data.
 
     Args:
-    ----
         data (): The json data
 
-    Returns
-    -------
+    Returns:
         boolean: True if valid, False otherwise.
 
     """
     errors = []
     missing = []
     if "component" not in data:
         errors.append("Need reference to component, hex string")
@@ -81,31 +78,36 @@
 class UploadTest(dbGtkUtils.ITkDBWindow):
     """Collects information to upload a test and its attachments."""
 
     def __init__(self, session, payload=None, attachment=None):
         """Initialization.
 
         Args:
-        ----
             session: ITkDB session
             payload: path of test file
-            attachment: an Attachment object.
+            attachment: an Attachment object or list of attachments.
 
         """
         self.payload = payload
         self.data = None
+        self.folder = None
         self.attachments = []
         self.comments = []
         self.defects = []
         if attachment is not None:
             if isinstance(attachment, ITkDButils.Attachment):
                 if attachment.path is not None:
                     self.attachments.append(attachment)
             else:
-                print("Wrong attachment: {}".format(attachment))
+                try:
+                    for att in attachment:
+                        self.attachments.append(att)
+
+                except TypeError:
+                    print("Wrong attachment: {}".format(attachment))
 
         global gtk_runs
         if gtk_runs:
             super().__init__(session=session, title="Upload Test", gtk_runs=gtk_runs)
             self.init_window()
 
     def init_window(self):
@@ -161,54 +163,76 @@
         lbl = Gtk.Label(label="Test Type")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, 2, 1, 1)
 
         self.entryTest = Gtk.Entry()
         grid.attach(self.entryTest, 1, 2, 1, 1)
 
+        # Object Stage
+        lbl = Gtk.Label(label="Object Stage")
+        lbl.set_xalign(0)
+        grid.attach(lbl, 0, 3, 1, 1)
+
+        self.objStage = Gtk.ComboBoxText.new()
+        self.objStage.connect("changed", self.on_new_stage)
+        grid.attach(self.objStage, 1, 3, 1, 1)
+
+        self.isRetroactive = Gtk.ToggleButton.new_with_label("RetroActive")
+        grid.attach(self.isRetroactive, 2, 3, 1, 1)
+
+
         # The "Add attachment" button.
         box = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL)
         self.mainBox.pack_start(box, False, False, 0)
-        dbGtkUtils.add_button_to_container(box, "Attachments",
+        self.btn_attch = dbGtkUtils.add_button_to_container(box, "Attachments",
                                            "Click to edit attachments.",
                                            self.edit_attachments)
 
-        dbGtkUtils.add_button_to_container(box, "Comments",
+        self.btn_comments = dbGtkUtils.add_button_to_container(box, "Comments",
                                            "Click to edit comments.",
                                            self.edit_comments)
 
-        dbGtkUtils.add_button_to_container(box, "Defects",
+        self.btn_defects = dbGtkUtils.add_button_to_container(box, "Defects",
                                            "Click to edit defects.",
                                            self.edit_defects)
 
         dbGtkUtils.add_button_to_container(box, "Upload Test",
                                            "Click to upload test.",
                                            self.upload_test_gui)
 
         # The text view
-        frame = self.create_text_view()
-        self.mainBox.pack_start(frame, True, True, 0)
+        self.mainBox.pack_start(self.message_panel.frame, True, True, 0)
 
         self.show_all()
 
         if self.payload:
-            the_path = Path(self.payload).expanduser().resolve()
-            if the_path.exists():
-                ifile = Path(self.payload).expanduser().resolve().as_posix()
-                self.testF.set_filename(ifile)
-                self.on_test_file(self.testF)
+            try:
+                the_path = Path(self.payload).expanduser().resolve()
+                if the_path.exists():
+                    ifile = Path(self.payload).expanduser().resolve().as_posix()
+                    self.testF.set_filename(ifile)
+                    self.on_test_file(self.testF)
+                    self.write_message("Loaded {}".format(the_path.name))
 
-            else:
-                print("Input file does not exists: {}".format(self.payload))
+                else:
+                    print("Input file does not exists: {}".format(self.payload))
+
+            except TypeError:
+                self.load_payload(self.payload)
+                self.write_message("Loaded memory payload.")
+
+        if len(self.attachments) > 0:
+            self.btn_attch.set_label("Attachments ({})".format(len(self.attachments)))
+
+        if len(self.comments) > 0:
+            self.btn_comments.set_label("Comments ({})".format(len(self.comments)))
+
+        if len(self.defects) > 0:
+            self.btn_defects.set_label("Defects ({})".format(len(self.defects)))
 
-        if len(self.attachments):
-            dC = [A for A in self.attachments]
-            self.attachments.clear()
-            for A in dC:
-                self.append_attachment_to_view(A)
 
     def get_test_institute(self):
         """Select an institue."""
         dlg = Gtk.Dialog(title="Select Institution.", flags=0)
         dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                         Gtk.STOCK_OK, Gtk.ResponseType.OK)
         area = dlg.get_content_area()
@@ -227,101 +251,201 @@
         if rc == Gtk.ResponseType.OK:
             out = self.get_institute_from_combo(combo)
 
         dlg.hide()
         dlg.destroy()
         return out
 
+    def load_payload(self, data):
+        """Payload is given as a dict."""
+        self.data = data
+        errors, missing = check_data(self.data)
+        self.complete_missing(missing, errors)
+        self.set_stages()
+
+    def on_new_stage(self, *args):
+        """New stage selected."""
+        stg = self.objStage.get_active_text()
+        changed = (stg != self.currentStage)
+        self.isRetroactive.set_active(changed)
+        self.data["isRetroactive"] = changed
+        if changed:
+            self.data["stage"] = stg
+        else:
+            if "stage" in self.data:
+                del self.data["stage"]
+
+    def set_stages(self):
+        """Prepare the stages combo."""
+        # Check the object stage
+        SN = self.data["component"]
+        try:
+            obj = ITkDButils.get_DB_component(self.session, SN)
+            self.currentStage = obj["currentStage"]["code"]
+
+            self.objStage.remove_all()
+            indx = 0
+            for i, stg in enumerate(obj["stages"]):
+                S = stg["code"]
+                self.objStage.append_text(S)
+                if S == self.currentStage:
+                    indx = i
+
+            self.objStage.set_active(indx)
+
+        except Exception:
+            self.write_message("Something went wring with the stages")
+
+
     def on_test_file(self, fdlg):
         """Test file browser clicked."""
         fnam = fdlg.get_filename()
+        self.folder = Path(fnam).parent
 
         # The file exists by definition
         try:
             self.data = json.loads(open(fnam).read())
             errors, missing = check_data(self.data)
-
-            if len(missing):
-                self.write_message("Some keys are missing in the JSon file.\n")
-                self.write_message("{}\n".format("\n".join(['\t'+line for line in missing])))
-
-                if "institution" in missing and len(missing) == 1:
-                    site = self.get_test_institute()
-                    if site:
-                        self.data["institution"] = site
-                        self.write_message("Setting Institution to {}\n".format(self.data["institution"]))
-
-                else:
-                    dbGtkUtils.complain("Invalid JSON file\n{}".format('\n'.join(errors)), fnam)
-
-            self.entrySN.set_text(self.data["component"])
-            self.entryTest.set_text(self.data["testType"])
-            self.comments = self.data.get("comments", [])
-            self.defects = self.data.get("defects", [])
+            self.complete_missing(missing, errors)
+            self.set_stages()
 
         except Exception as E:
             self.data = None
             self.write_message("Cannot load file {}\n".format(fnam))
             self.write_message("{}\n".format(str(E)))
 
+    def complete_missing(self, missing, errors):
+        """Completes missing parts."""
+        if len(missing):
+            self.write_message("Some keys are missing in the JSon file.\n")
+            self.write_message("{}\n".format("\n".join(['\t'+line for line in missing])))
+
+            if "institution" in missing and len(missing) == 1:
+                site = self.get_test_institute()
+                if site:
+                    self.data["institution"] = site
+                    self.write_message("Setting Institution to {}\n".format(self.data["institution"]))
+
+            else:
+                dbGtkUtils.complain("Invalid JSON data".format('\n'.join(errors)))
+
+        self.find_attachments()
+        self.find_comments()
+        self.find_defects()
+        
+        self.entrySN.set_text(self.data["component"] if self.data["component"] else "")
+        self.entryTest.set_text(self.data["testType"])
+        self.comments = self.data.get("comments", [])
+        self.defects = self.data.get("defects", [])
+
+
     def show_data(self, *args):
         """Show data button clicked."""
         if self.data is None:
             return
 
         value, dlg = create_json_data_editor(self.data)
         rc = dlg.run()
         if rc == Gtk.ResponseType.OK:
             self.data = value.values
 
         dlg.hide()
         dlg.destroy()
 
+    def find_attachments(self):
+        """Find Attachments in payload."""
+        self.attachments = []
+        if "attachments" in self.data:
+            for A in self.data["attachments"]:
+                if not Path(A["path"]).exists():
+                    if self.folder:
+                        the_path = self.folder.joinpath(A["path"])
+                    else:
+                        continue
+                else:
+                    the_path = Path(A["path"]).expanduser().resolve()
+                    
+                self.attachments.append(ITkDButils.Attachment(the_path, A["title"], A["description"]))
+
+        if len(self.attachments) > 0:
+            self.btn_attch.set_label("Attachments ({})".format(len(self.attachments)))
+
     def edit_attachments(self, *args):
         """Edit test attachmetns."""
         SA = ShowAttachments("Test Attachments", self.session, self.attachments, parent=self)
         response = SA.run()
         if response == Gtk.ResponseType.OK:
             self.attachments = SA.attachments
 
         SA.hide()
         SA.destroy()
 
+        if len(self.attachments) > 0:
+            self.btn_attch.set_label("Attachments ({})".format(len(self.attachments)))
+
+    def find_comments(self):
+        """Find comments in payload"""
+        self.comments = []
+        if "comments" in self.data:
+            for C in self.data["comments"]:
+                self.comments.append(C)
+                
+        if len(self.comments) > 0:
+            self.btn_comments.set_label("Comments ({})".format(len(self.comments)))
+
     def edit_comments(self, *args):
         """Edit test comments."""
         SC = ShowComments("Test Comments", self.comments, self)
         rc = SC.run()
         if rc == Gtk.ResponseType.OK:
             self.comments = SC.comments
 
         SC.hide()
         SC.destroy()
 
+        if len(self.comments) > 0:
+            self.btn_comments.set_label("Comments ({})".format(len(self.comments)))
+
+
+    def find_defects(self):
+        """Find defects in payload."""
+        self.defects = []
+        if "defects" in self.data:
+            for D in self.data["defects"]:
+                self.defects.append(D)
+                
+        if len(self.defects) > 0:
+            self.btn_defects.set_label("Defects ({})".format(len(self.defects)))
+
     def edit_defects(self, *args):
         """Edit test defects."""
         SD = ShowDefects("Test Defects", self.defects, self)
         rc = SD.run()
         if rc == Gtk.ResponseType.OK:
             self.defects = SD.defects
 
         SD.hide()
         SD.destroy()
 
+        if len(self.defects) > 0:
+            self.btn_defects.set_label("Defects ({})".format(len(self.defects)))
+
     def upload_test_gui(self, *args):
         """Uploads test and attachments."""
         self.upload_test()
 
     def upload_test(self):
         """Uploads test and attachments."""
         if self.data is None:
             self.write_message("No data available to upload\n")
             return
 
         self.data["comments"] = self.comments
         self.data["defects"] = self.defects
+            
         rc = ITkDButils.upload_test(self.session, self.data, self.attachments)
         if rc:
             ipos = rc.find("The following details may help:")
             msg = rc[ipos:]
             dbGtkUtils.complain("Failed uploading test", msg)
 
         else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.9.0/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
-Name: itkdb-gtk
-Version: 0.0.9
+Name: itkdb_gtk
+Version: 0.9.0
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: itkdb>=0.4.0
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
+Requires-Dist: pyserial
+Requires-Dist: python_dateutil
+Requires-Dist: requests
+Requires-Dist: PyGObject
 
 # Interaction with the ITk PDB.
 
 This folder contains a collection of scripts that help interacting with the DB
 using a Gtk based GUI, which includes a first attempt of reauthentication.
 
 You need to install itkdb and serial. The former for obvious reasons. The latter
@@ -32,33 +40,36 @@
 updated before expiration. This is usefull for very long sessions in the GUI.
 
 ## uploadPetalInformation.py
 Reads the AVS Production Sheet and FAT reports. With this information it creates
 the petal core in the DB, if not yet there, make the assembly of the components,
 and uploadas the test runs made at AVS.
 
-## uploadTest.py
+## UploadTest.py
 A GUI to upload the JSON files corresponding to a test and, also, to add
 attachmetns.
 
-## uploadMultipleTests.py
+## UploadMultipleTests.py
 This will allow to select various test files, or even scan a whole directory to
 find them, and assign comments, defects or attachments to each of the tests found.
 
-## getShipments.py
+## GetShipments.py
 Find all shipments to be received at a given site and list them. It handles a
 barcode reader that helps identifying the items actually received for the
 reception. It will finally make the DB aware of the items receptioned.
 
-## sendShipments.py
+## CreateShipments.py
 Create a new shipment. Allows to add items with the QR reader as well as from a
 GUI dialog. One can add comments and attachments to the shipment.
 
-## groundingTest.py
-Allows to enter valueos, comments and defects for those ot items in the gounding
+## GroundVITests.py
+Allows to upload and enter valueos, comments and defects for those items in the gounding
 and visual instpections tests of the petal core.
 
+## UploadModuleIV.py
+The idea behind this is that we messure the IV on a Ring module and on only one of the to Half modules. The IV of the remaining half modules is derived from the other 2. Eventually the IV test can be uploaded to the DB.
+
 ## dashBoard.py
 This is an launcher application from which we can start most of the other
 applications. It is a very good starting point. There is a Gnome desktop file (ITkDB.desktop)
-that needs to be copied to $HOME/.local/share/applications and an icon (ITkDB.svg) that
-needs to go to $HOME/.local/share/icons
+that needs to be copied to `$HOME/.local/share/applications` and an icon (ITkDB.svg) that
+needs to go to `$HOME/.local/share/icons`
```

### Comparing `itkdb_gtk-0.0.9/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.9.0/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 README.md
 pyproject.toml
+itkdb_gtk/CreateShipments.py
+itkdb_gtk/GetShipments.py
 itkdb_gtk/GlueWeight.py
+itkdb_gtk/GroundVITests.py
 itkdb_gtk/ITkDB.desktop
 itkdb_gtk/ITkDB.svg
 itkdb_gtk/ITkDBlogin.py
 itkdb_gtk/ITkDButils.py
 itkdb_gtk/ShowAttachments.py
 itkdb_gtk/ShowComments.py
 itkdb_gtk/ShowDefects.py
+itkdb_gtk/UploadModuleIV.py
+itkdb_gtk/UploadMultipleTests.py
+itkdb_gtk/UploadPetalInformation.py
+itkdb_gtk/UploadTest.py
+itkdb_gtk/WireBondGui.py
 itkdb_gtk/__init__.py
-itkdb_gtk/checkComponent.py
-itkdb_gtk/checkJSon.py
 itkdb_gtk/dashBoard.py
 itkdb_gtk/dbGtkUtils.py
-itkdb_gtk/getShipments.py
-itkdb_gtk/groundingTest.py
 itkdb_gtk/readAVSdata.py
 itkdb_gtk/readGoogleSheet.py
-itkdb_gtk/sendShipments.py
-itkdb_gtk/uploadMultipleTests.py
-itkdb_gtk/uploadPetalInformation.py
-itkdb_gtk/uploadTest.py
+itkdb_gtk/untrash_component.py
 itkdb_gtk.egg-info/PKG-INFO
 itkdb_gtk.egg-info/SOURCES.txt
 itkdb_gtk.egg-info/dependency_links.txt
 itkdb_gtk.egg-info/entry_points.txt
 itkdb_gtk.egg-info/requires.txt
-itkdb_gtk.egg-info/top_level.txt
+itkdb_gtk.egg-info/top_level.txt
+test/test_holes.py
```

### Comparing `itkdb_gtk-0.0.9/pyproject.toml` & `itkdb_gtk-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.9"
+version = "0.9.0"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "itkdb>=0.4.0",
+  "numpy",
+  "matplotlib",
   "openpyxl",
   "pyserial",
   "python_dateutil",
-  "requests"
+  "requests",
+  "PyGObject"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.gui-scripts]
 itkdb_dashBoard = "itkdb_gtk:dash_board"
 getShipments = "itkdb_gtk:getShipments"
 glueWeight = "itkdb_gtk:glueWeight"
-groundingTest = "itkdb_gtk:groundingTest"
-sendShipments = "itkdb_gtk:sendShipments"
+groundVITests = "itkdb_gtk:groundVITests"
+createShipments = "itkdb_gtk:createShipments"
 uploadTest = "itkdb_gtk:uploadTest"
 uploadMultipleTests = "itkdb_gtk:uploadMultipleTests"
+uploadModuleIV = "itkdb_gtk:uploadModuleIV"
+wirebondTest = "itkdb_gtk:wirebondTest"
+iploadPetalInformation = "itkdb_gtk:uploadPetalInformation"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 itkdb_gtk = ["*.desktop", "*.svg"]
```

