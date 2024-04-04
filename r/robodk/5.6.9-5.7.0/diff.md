# Comparing `tmp/robodk-5.6.9-py3-none-any.whl.zip` & `tmp/robodk-5.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 119596 bytes, number of entries: 15
+Zip file size: 119598 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-02 02:24 pylint_robodk/__init__.py
 -rw-rw-rw-  2.0 fat     1551 b- defN 22-Feb-02 02:24 pylint_robodk/pylint_robodk.py
 -rw-rw-rw-  2.0 fat     1516 b- defN 24-Feb-05 17:58 robodk/__init__.py
 -rw-rw-rw-  2.0 fat    53776 b- defN 24-Feb-15 12:30 robodk/roboapps.py
 -rw-rw-rw-  2.0 fat    47706 b- defN 24-Feb-15 12:23 robodk/robodialogs.py
 -rw-rw-rw-  2.0 fat    16997 b- defN 24-Feb-21 18:37 robodk/robofileio.py
--rw-rw-rw-  2.0 fat   345438 b- defN 24-Feb-21 18:38 robodk/robolink.py
+-rw-rw-rw-  2.0 fat   345444 b- defN 24-Apr-03 12:53 robodk/robolink.py
 -rw-rw-rw-  2.0 fat    10591 b- defN 24-Feb-15 12:23 robodk/robolinkutils.py
 -rw-rw-rw-  2.0 fat    80686 b- defN 24-Feb-15 12:21 robodk/robomath.py
 -rw-rw-rw-  2.0 fat     1210 b- defN 22-Feb-02 02:29 robolink/__init__.py
--rw-rw-rw-  2.0 fat      587 b- defN 24-Feb-21 18:48 robodk-5.6.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13082 b- defN 24-Feb-21 18:48 robodk-5.6.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-21 18:48 robodk-5.6.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-Feb-21 18:48 robodk-5.6.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1166 b- defN 24-Feb-21 18:48 robodk-5.6.9.dist-info/RECORD
-15 files, 574428 bytes uncompressed, 117704 bytes compressed:  79.5%
+-rw-rw-rw-  2.0 fat      587 b- defN 24-Apr-04 12:29 robodk-5.7.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13082 b- defN 24-Apr-04 12:29 robodk-5.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 12:29 robodk-5.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-04 12:29 robodk-5.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1166 b- defN 24-Apr-04 12:29 robodk-5.7.0.dist-info/RECORD
+15 files, 574434 bytes uncompressed, 117706 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: robodk/robomath.py
 Comment: 
 
 Filename: robolink/__init__.py
 Comment: 
 
-Filename: robodk-5.6.9.dist-info/LICENSE
+Filename: robodk-5.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: robodk-5.6.9.dist-info/METADATA
+Filename: robodk-5.7.0.dist-info/METADATA
 Comment: 
 
-Filename: robodk-5.6.9.dist-info/WHEEL
+Filename: robodk-5.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: robodk-5.6.9.dist-info/top_level.txt
+Filename: robodk-5.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: robodk-5.6.9.dist-info/RECORD
+Filename: robodk-5.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## robodk/robolink.py

```diff
@@ -1188,15 +1188,15 @@
             if type(args) is str:
                 if args != "":
                     args = [args]
                 else:
                     args = []
 
             self.IP = robodk_ip
-            self.ARGUMENTS = args
+            self.ARGUMENTS = list(args)
             self.CLOSE_STD_OUT = close_std_out
             self.QUIT_ON_CLOSE = quit_on_close
 
             if robodk_path is not None:
                 self.APPLICATION_DIR = robodk_path
             else:
                 self.APPLICATION_DIR = getPathRoboDK()
```

## Comparing `robodk-5.6.9.dist-info/LICENSE` & `robodk-5.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `robodk-5.6.9.dist-info/METADATA` & `robodk-5.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodk
-Version: 5.6.9
+Version: 5.7.0
 Summary: RoboDK tools for simulating and programming industrial robots (implements the RoboDK API)
 Home-page: https://robodk.com/doc/en/PythonAPI/index.html
 Author: RoboDK Inc.
 Author-email: info@robodk.com
 License: Apache Software License
 Keywords: industrial robot,simulation,offline programming,robot programming,robotics,online programming,3D simulator,post processors
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `robodk-5.6.9.dist-info/RECORD` & `robodk-5.7.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pylint_robodk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pylint_robodk/pylint_robodk.py,sha256=iYjRh4qyQKnB-lTY_YJuRu8931imrzzKH9JLNwPUC1c,1551
 robodk/__init__.py,sha256=AKKmH90Q2slRJHJwWCjbPMdPDuU1Nm_bBTxH5HXHi18,1516
 robodk/roboapps.py,sha256=wubsX6eEDrhtivGBdU89HN3BClhV6_L3TDO5vpAEMyk,53776
 robodk/robodialogs.py,sha256=3nrTf2hnFtxIzX49c5cECNeC6RYzM9bL0_xzaREgaFo,47706
 robodk/robofileio.py,sha256=x0Y__WKTRL1eZFWuP9Zgog3ucGrN9_VdRkgqxl2Ivko,16997
-robodk/robolink.py,sha256=65nK7nkjCdc--OsKr67B3fPcbkp80-Msr3Y6GsVrZPQ,345438
+robodk/robolink.py,sha256=kfLzf7b-OnIbIqN9dis9LxFttoeCJi0sh2DcBGpDgAg,345444
 robodk/robolinkutils.py,sha256=I94rlzlo0UcnljY2n4kB8NeZIG2NTtbLZxr7wdbmZLw,10591
 robodk/robomath.py,sha256=-0cme6thvZx75mECnAVXwY97Ew_obuNS1dI2HCMyqSw,80686
 robolink/__init__.py,sha256=RqchTjeRBU7Hnko58B9xHigsffzo9R6nlNs83zA5NhU,1210
-robodk-5.6.9.dist-info/LICENSE,sha256=D5sOGFtT_R0frDUaM9bm7RVnQJ_G2ivMdr1DRZCu8WU,587
-robodk-5.6.9.dist-info/METADATA,sha256=6Iaec1Ijbyp6IxR6ERn1ac52cv6gIBMUOAxqon5a-Nw,13082
-robodk-5.6.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-robodk-5.6.9.dist-info/top_level.txt,sha256=3CTL620vD_h4LfM0G4AXCDqkk8qr2UpQZMQU_gYi9Sc,30
-robodk-5.6.9.dist-info/RECORD,,
+robodk-5.7.0.dist-info/LICENSE,sha256=D5sOGFtT_R0frDUaM9bm7RVnQJ_G2ivMdr1DRZCu8WU,587
+robodk-5.7.0.dist-info/METADATA,sha256=6WM3lfqF4cT7cQ_XFRPmcbdrEMIy37hVazM6DIUkvA8,13082
+robodk-5.7.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+robodk-5.7.0.dist-info/top_level.txt,sha256=3CTL620vD_h4LfM0G4AXCDqkk8qr2UpQZMQU_gYi9Sc,30
+robodk-5.7.0.dist-info/RECORD,,
```

