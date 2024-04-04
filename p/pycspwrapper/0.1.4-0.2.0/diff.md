# Comparing `tmp/pycspwrapper-0.1.4-py3-none-any.whl.zip` & `tmp/pycspwrapper-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4006 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     3352 b- defN 24-Apr-02 14:56 pycspwrapper/LVStat.py
+Zip file size: 4138 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     3414 b- defN 24-Apr-04 11:07 pycspwrapper/LVStat.py
 -rw-rw-r--  2.0 unx       74 b- defN 24-Mar-21 09:50 pycspwrapper/__init__.py
--rw-rw-r--  2.0 unx     1075 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1595 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      569 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/RECORD
-7 files, 6770 bytes uncompressed, 2992 bytes compressed:  55.8%
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1814 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/RECORD
+7 files, 7051 bytes uncompressed, 3124 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycspwrapper/LVStat.py
 Comment: 
 
 Filename: pycspwrapper/__init__.py
 Comment: 
 
-Filename: pycspwrapper-0.1.4.dist-info/LICENSE
+Filename: pycspwrapper-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pycspwrapper-0.1.4.dist-info/METADATA
+Filename: pycspwrapper-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pycspwrapper-0.1.4.dist-info/WHEEL
+Filename: pycspwrapper-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pycspwrapper-0.1.4.dist-info/top_level.txt
+Filename: pycspwrapper-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pycspwrapper-0.1.4.dist-info/RECORD
+Filename: pycspwrapper-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycspwrapper/LVStat.py

```diff
@@ -34,28 +34,28 @@
         if len(self.ids[-1]) >= 3:
             try:
                 int(self.ids[-1][3])
             except ValueError:
                 return self.url_out + '__'.join(self.ids[:-1]) + '/' + self.ids[-1]
         return self.url_out + '__'.join(self.ids)
 
-    def get_variables(self):
-        """ Returns a dictionary of variables and their ranges for the bottom node. """
+    def get_variables(self, values=True):
+        """ Returns a dictionary of variables and their ranges for the bottom node. 
+        
+        :param values specifies whether the variables will be returned by code value (default) or by text value."""
         response = self.info()
         val_dict = {}
         try:
             variables = response['variables']
         except TypeError:
             print("Error: You are not in a leaf node.")
             return
         for item in variables:
-            val = list(item.values())
-            for i in range(1, len(val), 4):
-                for j in range(3, len(val), 4):
-                    val_dict[val[i]] = val[j]
+            val_dict[item['code']] = item['values']\
+                if values else item['valueTexts']
         return val_dict
 
     def clear_query(self):
         """ Clears the query. Mostly an internal function to use in others. """
         self.query = {"query": [], 
                       "response": {"format": "json"}
                       }
```

## Comparing `pycspwrapper-0.1.4.dist-info/LICENSE` & `pycspwrapper-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycspwrapper-0.1.4.dist-info/METADATA` & `pycspwrapper-0.2.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycspwrapper
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python wrapper for Latvian official statistics portal API: https://stat.gov.lv/en/api-and-code-list-registry.
 Home-page: https://github.com/vf42/pycspwrapper
 Author: Vadim Fedorov
 Author-email: vadim@vf42.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,20 @@
 from pycspwrapper import LVStat
 ```
 
 For info on usage, see the included notebooks.
 
 ## Changelog
 
+News in version 0.2.0:
+Changed the behavior of .get_variables() to return the text/code values by default.
+
+News in version 0.1.4:
+Caching info data while in the same location. Updated examples in Latvian and English.
+
 News in version 0.1.3:
 Updated query generation code to use variable and value codes instead of text values.
 
 News in version 0.1.2:
 Fixed the module name to avoid conflicts with the original version.
 
 News in version 0.1.1:
```

