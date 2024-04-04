# Comparing `tmp/pytypeworks-0.1.0.6515122072-py2.py3-none-any.whl.zip` & `tmp/pytypeworks-0.1.0.8548343949-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 12511 bytes, number of entries: 15
--rw-r--r--  2.0 unx      807 b- defN 23-Oct-14 02:45 typeworks/__init__.py
--rw-r--r--  2.0 unx     4367 b- defN 23-Oct-14 02:45 typeworks/cls_decorator_base.py
--rw-r--r--  2.0 unx     2497 b- defN 23-Oct-14 02:45 typeworks/method_decorator_base.py
--rw-r--r--  2.0 unx      525 b- defN 23-Oct-14 02:45 typeworks/registration_decorator_base.py
--rw-r--r--  2.0 unx     3630 b- defN 23-Oct-14 02:45 typeworks/type_rgy.py
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-14 02:45 typeworks/impl/__init__.py
--rw-r--r--  2.0 unx     1858 b- defN 23-Oct-14 02:45 typeworks/impl/decl_rgy.py
--rw-r--r--  2.0 unx     1011 b- defN 23-Oct-14 02:45 typeworks/impl/method_info.py
--rw-r--r--  2.0 unx      988 b- defN 23-Oct-14 02:45 typeworks/impl/method_proxy.py
--rw-r--r--  2.0 unx      631 b- defN 23-Oct-14 02:45 typeworks/impl/typeinfo.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Oct-14 02:46 pytypeworks-0.1.0.6515122072.dist-info/LICENSE
--rw-r--r--  2.0 unx      426 b- defN 23-Oct-14 02:46 pytypeworks-0.1.0.6515122072.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-14 02:46 pytypeworks-0.1.0.6515122072.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Oct-14 02:46 pytypeworks-0.1.0.6515122072.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1309 b- defN 23-Oct-14 02:46 pytypeworks-0.1.0.6515122072.dist-info/RECORD
-15 files, 29526 bytes uncompressed, 10313 bytes compressed:  65.1%
+Zip file size: 12513 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      807 b- defN 24-Apr-04 02:19 typeworks/__init__.py
+-rw-r--r--  2.0 unx     4373 b- defN 24-Apr-04 02:19 typeworks/cls_decorator_base.py
+-rw-r--r--  2.0 unx     2497 b- defN 24-Apr-04 02:19 typeworks/method_decorator_base.py
+-rw-r--r--  2.0 unx      525 b- defN 24-Apr-04 02:19 typeworks/registration_decorator_base.py
+-rw-r--r--  2.0 unx     3630 b- defN 24-Apr-04 02:19 typeworks/type_rgy.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 02:19 typeworks/impl/__init__.py
+-rw-r--r--  2.0 unx     1858 b- defN 24-Apr-04 02:19 typeworks/impl/decl_rgy.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-04 02:19 typeworks/impl/method_info.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-04 02:19 typeworks/impl/method_proxy.py
+-rw-r--r--  2.0 unx      631 b- defN 24-Apr-04 02:19 typeworks/impl/typeinfo.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-04 02:20 pytypeworks-0.1.0.8548343949.dist-info/LICENSE
+-rw-r--r--  2.0 unx      426 b- defN 24-Apr-04 02:20 pytypeworks-0.1.0.8548343949.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-04 02:20 pytypeworks-0.1.0.8548343949.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-04 02:20 pytypeworks-0.1.0.8548343949.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1309 b- defN 24-Apr-04 02:20 pytypeworks-0.1.0.8548343949.dist-info/RECORD
+15 files, 29532 bytes uncompressed, 10315 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: typeworks/impl/method_proxy.py
 Comment: 
 
 Filename: typeworks/impl/typeinfo.py
 Comment: 
 
-Filename: pytypeworks-0.1.0.6515122072.dist-info/LICENSE
+Filename: pytypeworks-0.1.0.8548343949.dist-info/LICENSE
 Comment: 
 
-Filename: pytypeworks-0.1.0.6515122072.dist-info/METADATA
+Filename: pytypeworks-0.1.0.8548343949.dist-info/METADATA
 Comment: 
 
-Filename: pytypeworks-0.1.0.6515122072.dist-info/WHEEL
+Filename: pytypeworks-0.1.0.8548343949.dist-info/WHEEL
 Comment: 
 
-Filename: pytypeworks-0.1.0.6515122072.dist-info/top_level.txt
+Filename: pytypeworks-0.1.0.8548343949.dist-info/top_level.txt
 Comment: 
 
-Filename: pytypeworks-0.1.0.6515122072.dist-info/RECORD
+Filename: pytypeworks-0.1.0.8548343949.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## typeworks/cls_decorator_base.py

```diff
@@ -27,15 +27,15 @@
         
     def pre_decorate(self, T):
         pass
     
     def pre_init_annotated_fields(self):
         pass
     
-    def init_annotated_field(self, key, value, has_init):
+    def init_annotated_field(self, key, value, has_init, init):
         pass
     
     def post_init_annotated_fields(self):
         pass
     
     def set_field_initial(self, key, init):
         setattr(self.T, key, init)
```

## Comparing `pytypeworks-0.1.0.6515122072.dist-info/LICENSE` & `pytypeworks-0.1.0.8548343949.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytypeworks-0.1.0.6515122072.dist-info/RECORD` & `pytypeworks-0.1.0.8548343949.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 typeworks/__init__.py,sha256=isGXXmUs_6lsRk44UV__0_KdhIbZ1Ggl3MUvYIKveFQ,807
-typeworks/cls_decorator_base.py,sha256=xrOVqnxWcRSV2r7oDj52zfFy0-tzldy18gP4Ejy7WSc,4367
+typeworks/cls_decorator_base.py,sha256=8DxEwQ36Lnxv40it60aBu5u4MurZwf0B6zHN0aqgO6g,4373
 typeworks/method_decorator_base.py,sha256=6ag22dGucBkXFetFQ0mPYj4HzqrS8Cql_o6MT2NTRjM,2497
 typeworks/registration_decorator_base.py,sha256=WTb9dRmEmYLqrCxinIVtSjWtafmezVsmUcPsYHBGRNY,525
 typeworks/type_rgy.py,sha256=TIi6wOrzKGrjmcR3ImUk6ND8mzpIw7g-THc2td9qkeY,3630
 typeworks/impl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 typeworks/impl/decl_rgy.py,sha256=eDExRuepPa_wd2h3hRE5l_LHBuEomCQ_RRzmKVTCXwY,1858
 typeworks/impl/method_info.py,sha256=5iuhBZc3nLiIhwl6RjP-_6KuSkQAj_EHzO5VDFz0-tI,1011
 typeworks/impl/method_proxy.py,sha256=IJYcg9Na11xjqZ2KGjXdWSrQsXYBEqedMF6apLkGQyM,988
 typeworks/impl/typeinfo.py,sha256=D5XOreq9a7qkycFQMq88KPUuR6rFEbCvyCsL_Dyn5vg,631
-pytypeworks-0.1.0.6515122072.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytypeworks-0.1.0.6515122072.dist-info/METADATA,sha256=EBq9vkFAJ31BGQ8kPLzaFWtYbA77qkX-I71rFoqtMA8,426
-pytypeworks-0.1.0.6515122072.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-pytypeworks-0.1.0.6515122072.dist-info/top_level.txt,sha256=lXrs4kKxSmnPMytK1VWynj2Wfp53-DYZOPPsG6VSSYA,10
-pytypeworks-0.1.0.6515122072.dist-info/RECORD,,
+pytypeworks-0.1.0.8548343949.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytypeworks-0.1.0.8548343949.dist-info/METADATA,sha256=5xVaVUK_Jjft6VZPgNmeYEttIziUwV286qRQCdBFoRc,426
+pytypeworks-0.1.0.8548343949.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+pytypeworks-0.1.0.8548343949.dist-info/top_level.txt,sha256=lXrs4kKxSmnPMytK1VWynj2Wfp53-DYZOPPsG6VSSYA,10
+pytypeworks-0.1.0.8548343949.dist-info/RECORD,,
```

