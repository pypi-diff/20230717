# Comparing `tmp/odoo14_addons_oca_edi-14.0.20230521.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_edi-14.0.20230715.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1669 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2999 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/RECORD
-4 files, 3485 bytes uncompressed, 895 bytes compressed:  74.3%
+Zip file size: 1675 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3051 b- defN 23-Jul-17 03:18 odoo14_addons_oca_edi-14.0.20230715.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 03:18 odoo14_addons_oca_edi-14.0.20230715.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-17 03:18 odoo14_addons_oca_edi-14.0.20230715.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      393 b- defN 23-Jul-17 03:18 odoo14_addons_oca_edi-14.0.20230715.0.dist-info/RECORD
+4 files, 3537 bytes uncompressed, 901 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/METADATA
+Filename: odoo14_addons_oca_edi-14.0.20230715.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_edi-14.0.20230715.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_edi-14.0.20230715.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/RECORD
+Filename: odoo14_addons_oca_edi-14.0.20230715.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_edi-14.0.20230521.0.dist-info/METADATA` & `odoo14_addons_oca_edi-14.0.20230715.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-edi
-Version: 14.0.20230521.0
+Version: 14.0.20230715.0
 Summary: Meta package for oca-edi Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -49,14 +49,15 @@
 Requires-Dist: odoo14-addon-edi-webservice-oca
 Requires-Dist: odoo14-addon-edi-xml-oca
 Requires-Dist: odoo14-addon-partner-identification-import
 Requires-Dist: odoo14-addon-pdf-helper
 Requires-Dist: odoo14-addon-product-import
 Requires-Dist: odoo14-addon-product-import-ubl
 Requires-Dist: odoo14-addon-purchase-order-ubl
+Requires-Dist: odoo14-addon-purchase-order-ubl-py3o
 Requires-Dist: odoo14-addon-purchase-stock-ubl
 Requires-Dist: odoo14-addon-sale-order-customer-free-ref
 Requires-Dist: odoo14-addon-sale-order-import
 Requires-Dist: odoo14-addon-sale-order-import-ubl
 Requires-Dist: odoo14-addon-sale-order-import-ubl-customer-free-ref
 Requires-Dist: odoo14-addon-sale-order-import-ubl-line-customer-ref
 Requires-Dist: odoo14-addon-sale-order-packaging-import
```

