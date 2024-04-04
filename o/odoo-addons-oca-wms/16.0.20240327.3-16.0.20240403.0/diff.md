# Comparing `tmp/odoo_addons_oca_wms-16.0.20240327.3-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_wms-16.0.20240403.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1562 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2248 b- defN 24-Mar-29 08:38 odoo_addons_oca_wms-16.0.20240327.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 08:38 odoo_addons_oca_wms-16.0.20240327.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-29 08:38 odoo_addons_oca_wms-16.0.20240327.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Mar-29 08:38 odoo_addons_oca_wms-16.0.20240327.3.dist-info/RECORD
-4 files, 2726 bytes uncompressed, 804 bytes compressed:  70.5%
+Zip file size: 1565 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2337 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/RECORD
+4 files, 2815 bytes uncompressed, 807 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_wms-16.0.20240327.3.dist-info/METADATA
+Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240327.3.dist-info/WHEEL
+Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240327.3.dist-info/top_level.txt
+Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240327.3.dist-info/RECORD
+Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_wms-16.0.20240327.3.dist-info/METADATA` & `odoo_addons_oca_wms-16.0.20240403.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-wms
-Version: 16.0.20240327.3
+Version: 16.0.20240403.0
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -20,14 +20,15 @@
 Requires-Dist: odoo-addon-stock-release-channel-batch-mode-commercial-partner <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-cutoff <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-delivery <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-geoengine <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-partner-delivery-window <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-partner-public-holidays <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-plan <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-release-channel-plan-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-propagate-channel-picking <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-advice <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-lead-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-show-volume <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-show-weight <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-storage-type <16.1dev,>=16.0dev
```

