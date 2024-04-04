# Comparing `tmp/hightime-0.2.1-py3-none-any.whl.zip` & `tmp/hightime-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9550 bytes, number of entries: 10
--rw-r--r--  2.0 unx        6 b- defN 21-Aug-13 20:03 hightime/VERSION
--rw-r--r--  2.0 unx     1801 b- defN 21-Aug-13 20:03 hightime/__init__.py
--rw-r--r--  2.0 unx    12526 b- defN 21-Aug-13 20:03 hightime/_datetime.py
--rw-r--r--  2.0 unx     8928 b- defN 21-Aug-13 20:03 hightime/_timedelta.py
--rw-r--r--  2.0 unx     1148 b- defN 21-Aug-13 20:04 hightime-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2581 b- defN 21-Aug-13 20:04 hightime-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Aug-13 20:04 hightime-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 21-Aug-13 20:04 hightime-0.2.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Aug-13 20:04 hightime-0.2.1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      782 b- defN 21-Aug-13 20:04 hightime-0.2.1.dist-info/RECORD
-10 files, 27874 bytes uncompressed, 8216 bytes compressed:  70.5%
+Zip file size: 9705 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-04 16:35 hightime/VERSION
+-rw-r--r--  2.0 unx     1802 b- defN 24-Apr-04 16:35 hightime/__init__.py
+-rw-r--r--  2.0 unx    12526 b- defN 24-Apr-04 16:35 hightime/_datetime.py
+-rw-r--r--  2.0 unx     9528 b- defN 24-Apr-04 16:35 hightime/_timedelta.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Apr-04 16:36 hightime-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2539 b- defN 24-Apr-04 16:36 hightime-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 16:36 hightime-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-04 16:36 hightime-0.2.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 16:36 hightime-0.2.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      782 b- defN 24-Apr-04 16:36 hightime-0.2.2.dist-info/RECORD
+10 files, 28433 bytes uncompressed, 8371 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: hightime/_datetime.py
 Comment: 
 
 Filename: hightime/_timedelta.py
 Comment: 
 
-Filename: hightime-0.2.1.dist-info/LICENSE
+Filename: hightime-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: hightime-0.2.1.dist-info/METADATA
+Filename: hightime-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: hightime-0.2.1.dist-info/WHEEL
+Filename: hightime-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: hightime-0.2.1.dist-info/top_level.txt
+Filename: hightime-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hightime-0.2.1.dist-info/zip-safe
+Filename: hightime-0.2.2.dist-info/zip-safe
 Comment: 
 
-Filename: hightime-0.2.1.dist-info/RECORD
+Filename: hightime-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hightime/VERSION

```diff
@@ -1 +1 @@
-0.2.1
+0.2.2
```

## hightime/__init__.py

```diff
@@ -14,14 +14,15 @@
         An impedance-matched subclass of datetime.timedelta with sub-microsecond
         capabilities.
 
 Please note that due to floating point arithmetic inaccuracies, the ability to specify
 sub-microsecond values in terms of much larger units (weeks, days, seconds) has been
 limited. For the exact limitation, please consult the various methods.
 """
+
 import datetime as _std_datetime
 
 
 from hightime._datetime import datetime
 from hightime._timedelta import timedelta
 
 # Hide that it was defined in a helper file
```

## hightime/_timedelta.py

```diff
@@ -1,19 +1,21 @@
 import datetime as std_datetime
+import decimal
+from decimal import Decimal
 from fractions import Fraction
 
-_YS_PER_S = 10 ** 24
-_YS_PER_US = 10 ** 18
-_YS_PER_FS = 10 ** 9
+_YS_PER_S = 10**24
+_YS_PER_US = 10**18
+_YS_PER_FS = 10**9
 _YS_PER_DAY = 60 * 60 * 24 * _YS_PER_S
 
 _US_PER_DAY = 24 * 60 * 60 * 1000 * 1000
 _US_PER_WEEK = 7 * _US_PER_DAY
-_NS_PER_HOUR = 60 * 60 * (10 ** 9)
-_PS_PER_MINUTE = 60 * (10 ** 12)
+_NS_PER_HOUR = 60 * 60 * (10**9)
+_PS_PER_MINUTE = 60 * (10**12)
 
 _FIELD_NAMES = [
     "days",
     "seconds",
     "microseconds",
     "femtoseconds",
     "yoctoseconds",
@@ -98,15 +100,18 @@
 
         days, yoctoseconds = divmod(yoctoseconds, _YS_PER_DAY)
         seconds, yoctoseconds = divmod(yoctoseconds, _YS_PER_S)
         microseconds, yoctoseconds = divmod(yoctoseconds, _YS_PER_US)
         femtoseconds, yoctoseconds = divmod(yoctoseconds, _YS_PER_FS)
 
         self = super().__new__(
-            cls, days=days, seconds=seconds, microseconds=microseconds,
+            cls,
+            days=days,
+            seconds=seconds,
+            microseconds=microseconds,
         )
 
         self._femtoseconds = femtoseconds
         self._yoctoseconds = round(yoctoseconds)
         return self
 
     # Public properties
@@ -128,19 +133,34 @@
     # Public methods
 
     def total_seconds(self):
         """Total seconds in the duration."""
         return (
             (self.days * 86400)
             + self.seconds
-            + (self.microseconds / 10 ** 6)
-            + (self.femtoseconds / 10 ** 15)
-            + (self.yoctoseconds / 10 ** 24)
+            + (self.microseconds / 10**6)
+            + (self.femtoseconds / 10**15)
+            + (self.yoctoseconds / 10**24)
         )
 
+    def precision_total_seconds(self):
+        """Precise total seconds in the duration.
+
+        Note: up to 64 significant digits are used in computation.
+        """
+        with decimal.localcontext() as ctx:
+            ctx.prec = 64
+            return Decimal(
+                (self.days * 86400)
+                + self.seconds
+                + Decimal(self.microseconds) / Decimal(10**6)
+                + Decimal(self.femtoseconds) / Decimal(10**15)
+                + Decimal(self.yoctoseconds) / Decimal(10**24)
+            )
+
     # String operators
 
     def __repr__(self):
         # Follow newer repr: https://github.com/python/cpython/pull/3687
         r = "{}.{}".format(self.__class__.__module__, self.__class__.__qualname__)
         r += "("
         r += ", ".join(
```

## Comparing `hightime-0.2.1.dist-info/LICENSE` & `hightime-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hightime-0.2.1.dist-info/METADATA` & `hightime-0.2.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: hightime
-Version: 0.2.1
+Version: 0.2.2
 Summary: Hightime Python API
 Home-page: https://github.com/ni/hightime
 Author: National Instruments
 Author-email: opensource@ni.com
 Maintainer: National Instruments
 Maintainer-email: opensource@ni.com
 License: MIT
 Keywords: hightime
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 
 # Hightime
 
 ## Overview
```

## Comparing `hightime-0.2.1.dist-info/RECORD` & `hightime-0.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-hightime/VERSION,sha256=cQFcl5zLD8igvnygroMEarBFzcLI-qCfsvD35ED5tKY,6
-hightime/__init__.py,sha256=TIZpYKrdx9OPre_flewrLuJUeKjrS5HuinZXcLEaMEs,1801
+hightime/VERSION,sha256=mY9riH7Xpu9E6EIQ0CN7cVvtQupyVPSNxBiv7ApIQQM,6
+hightime/__init__.py,sha256=WoX5gWrwr1qsmO2zoAYkVOmF9sXhQkepoUR0ufON53s,1802
 hightime/_datetime.py,sha256=fGjvNXHm7-svFcqU3T6jFiRym_EWkyiKVlvVE3Csm_A,12526
-hightime/_timedelta.py,sha256=exPj9WKgpwN_tus2CUSG_ExwsG-ke5AL-l52shNEiBs,8928
-hightime-0.2.1.dist-info/LICENSE,sha256=9cmSCHyJhrXFez2u9DQJ6t03cK68bFuHVOJU-vewUV4,1148
-hightime-0.2.1.dist-info/METADATA,sha256=5zRmlbSP-zch3V9XiS7mtSmtR831sw9t1ngY4harS5c,2581
-hightime-0.2.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-hightime-0.2.1.dist-info/top_level.txt,sha256=oG8A3Wbyj4iOfxQY8VDBTum2sMWGHTQHEqulY2b8fpM,9
-hightime-0.2.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-hightime-0.2.1.dist-info/RECORD,,
+hightime/_timedelta.py,sha256=_gpn1lhna5Zd9VOavO-0n-lubSLXVWOLlUfBozHte9E,9528
+hightime-0.2.2.dist-info/LICENSE,sha256=9cmSCHyJhrXFez2u9DQJ6t03cK68bFuHVOJU-vewUV4,1148
+hightime-0.2.2.dist-info/METADATA,sha256=af1_pe-uBWXrD363HiVrthNRA3yvVP-DT__BqytrMNA,2539
+hightime-0.2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+hightime-0.2.2.dist-info/top_level.txt,sha256=oG8A3Wbyj4iOfxQY8VDBTum2sMWGHTQHEqulY2b8fpM,9
+hightime-0.2.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+hightime-0.2.2.dist-info/RECORD,,
```

