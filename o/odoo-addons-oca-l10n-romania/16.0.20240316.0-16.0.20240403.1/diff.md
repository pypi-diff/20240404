# Comparing `tmp/odoo_addons_oca_l10n_romania-16.0.20240316.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_l10n_romania-16.0.20240403.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1646 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2772 b- defN 24-Mar-17 05:06 odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-17 05:06 odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-17 05:06 odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      421 b- defN 24-Mar-17 05:06 odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/RECORD
-4 files, 3286 bytes uncompressed, 816 bytes compressed:  75.2%
+Zip file size: 1671 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-04 04:34 odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 04:34 odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 04:34 odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      421 b- defN 24-Apr-04 04:34 odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/RECORD
+4 files, 3438 bytes uncompressed, 841 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/METADATA
+Filename: odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/WHEEL
+Filename: odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/RECORD
+Filename: odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_l10n_romania-16.0.20240316.0.dist-info/METADATA` & `odoo_addons_oca_l10n_romania-16.0.20240403.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-l10n-romania
-Version: 16.0.20240316.0
+Version: 16.0.20240403.1
 Summary: Meta package for oca-l10n-romania Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -23,24 +23,26 @@
 Requires-Dist: odoo-addon-l10n-ro-account-period-close <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-account-report-invoice <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-city <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-config <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-dvi <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-etransport <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-fiscal-validation <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-l10n-ro-nondeductible-vat <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-partner-create-by-vat <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-partner-unique <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-payment-receipt-report <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-payment-to-statement <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-pos <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-account <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-account-date <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-account-date-wizard <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-account-notice <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-account-reception-in-progress <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-l10n-ro-stock-picking-valued-report <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-price-difference <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-stock-report <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-l10n-ro-vat-on-payment <16.1dev,>=16.0dev
 
 UNKNOWN
```

