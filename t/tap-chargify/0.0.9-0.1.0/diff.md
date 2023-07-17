# Comparing `tmp/tap-chargify-0.0.9.tar.gz` & `tmp/tap-chargify-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-chargify-0.0.9.tar", last modified: Wed Nov 20 14:45:14 2019, max compression
+gzip compressed data, was "tap-chargify-0.1.0.tar", last modified: Mon Jul 17 13:46:56 2023, max compression
```

## Comparing `tap-chargify-0.0.9.tar` & `tap-chargify-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    32387 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/LICENSE
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       13 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      818 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      307 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       62 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       74 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      307 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       86 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/MANIFEST.in
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4263 2019-11-20 14:32:29.000000 tap-chargify-0.0.9/tap_chargify/chargify.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2414 2019-10-30 18:29:33.000000 tap-chargify-0.0.9/tap_chargify/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      815 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/sync.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5346 2019-11-01 14:46:18.000000 tap-chargify-0.0.9/tap_chargify/streams.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       35 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/context.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/tap_chargify/schemas/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7969 2019-11-20 14:32:29.000000 tap-chargify-0.0.9/tap_chargify/schemas/statements.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      475 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/product_families.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6325 2019-11-20 14:32:29.000000 tap-chargify-0.0.9/tap_chargify/schemas/invoices.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2056 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/coupons.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    12571 2019-11-20 14:32:29.000000 tap-chargify-0.0.9/tap_chargify/schemas/subscriptions.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1805 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/components.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2074 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/customers.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      853 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/events.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3211 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/products.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1712 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/schemas/price_points.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2411 2019-11-06 18:57:04.000000 tap-chargify-0.0.9/tap_chargify/schemas/transactions.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2629 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/tap_chargify/discover.py
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)      785 2019-11-20 14:45:03.000000 tap-chargify-0.0.9/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       79 2019-11-20 14:45:14.000000 tap-chargify-0.0.9/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1085 2019-10-17 17:59:02.000000 tap-chargify-0.0.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 13:46:56.590674 tap-chargify-0.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      273 2023-07-17 13:46:56.590674 tap-chargify-0.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5574 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-07-17 13:46:56.590674 tap-chargify-0.1.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      785 2023-07-17 13:42:29.000000 tap-chargify-0.1.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 13:46:56.590674 tap-chargify-0.1.0/tap_chargify/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2414 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4280 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/chargify.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/context.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2629 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 13:46:56.590674 tap-chargify-0.1.0/tap_chargify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3029 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/components.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/coupons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2074 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3346 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6351 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/invoices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1712 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/price_points.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/product_families.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3700 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11972 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/statements.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12506 2023-07-17 13:14:16.000000 tap-chargify-0.1.0/tap_chargify/schemas/subscriptions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3079 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/schemas/transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5340 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      815 2023-07-13 05:11:33.000000 tap-chargify-0.1.0/tap_chargify/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 13:46:56.590674 tap-chargify-0.1.0/tap_chargify.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      273 2023-07-17 13:46:56.000000 tap-chargify-0.1.0/tap_chargify.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      818 2023-07-17 13:46:56.000000 tap-chargify-0.1.0/tap_chargify.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-17 13:46:56.000000 tap-chargify-0.1.0/tap_chargify.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-07-17 13:46:56.000000 tap-chargify-0.1.0/tap_chargify.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-17 13:46:56.000000 tap-chargify-0.1.0/tap_chargify.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-17 13:46:56.000000 tap-chargify-0.1.0/tap_chargify.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-chargify-0.0.9/LICENSE` & `tap-chargify-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-chargify-0.0.9/tap_chargify.egg-info/SOURCES.txt` & `tap-chargify-0.1.0/tap_chargify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-chargify-0.0.9/tap_chargify/chargify.py` & `tap-chargify-0.1.0/tap_chargify/chargify.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         for j in self.get("product_families/{product_family_id}/components.json".format(product_family_id=k["product_family"]["id"])):
           for l in j:
             yield l["component"]
 
 
 
   def subscriptions(self, bookmark=None):
-    for i in self.get("subscriptions.json", start_datetime=bookmark, date_field="updated_at"):
+    for i in self.get("subscriptions.json", start_datetime=bookmark, date_field="updated_at", direction="asc"):
       for j in i:
         yield j["subscription"]
 
 
   def transactions(self, bookmark=None):
     since_date = utils.strptime_with_tz(bookmark).strftime('%Y-%m-%d')
     for i in self.get("transactions.json", since_date=since_date, direction="asc"):
```

### Comparing `tap-chargify-0.0.9/tap_chargify/__init__.py` & `tap-chargify-0.1.0/tap_chargify/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-chargify-0.0.9/tap_chargify/sync.py` & `tap-chargify-0.1.0/tap_chargify/sync.py`

 * *Files identical despite different names*

### Comparing `tap-chargify-0.0.9/tap_chargify/streams.py` & `tap-chargify-0.1.0/tap_chargify/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-# 
+#
 # Module dependencies.
-# 
+#
 
 import os
 import json
 import datetime
 import pytz
 import singer
 import time
@@ -84,29 +84,29 @@
         schema_file = "schemas/{}.json".format(self.name)
         with open(get_abs_path(schema_file)) as f:
             schema = json.load(f)
         return schema
 
 
     def load_metadata(self):
-        return metadata.get_standard_metadata(schema=self.load_schema(), 
-                                              key_properties=self.key_properties, 
-                                              valid_replication_keys=[self.replication_key], 
+        return metadata.get_standard_metadata(schema=self.load_schema(),
+                                              key_properties=self.key_properties,
+                                              valid_replication_keys=[self.replication_key],
                                               replication_method=self.replication_method)
 
 
     # The main sync function.
     def sync(self, state):
         get_data = getattr(self.client, self.name)
         bookmark = self.get_bookmark(state)
         # res = get_data(self.replication_key, bookmark)
         res = get_data(bookmark)
 
         if self.replication_method == "INCREMENTAL":
-            # These streams results may not be ordered, 
+            # These streams results may not be ordered,
             # so store highest value bookmark in session.
             for item in res:
                 # if item is bigger than bookmark, then
                 if self.is_bookmark_old(state, item[self.replication_key]):
                     self.update_bookmark(state, item[self.replication_key])
                     yield (self.stream, item)
         else:
@@ -144,37 +144,37 @@
 class Components(Stream):
     name = "components"
     replication_method = "FULL_TABLE"
 
 
 class Subscriptions(Stream):
     name = "subscriptions"
-    replication_method = "INCREMENTAL"
-    replication_key = "updated_at"
+    replication_method = "FULL_TABLE"
+    # replication_key = "updated_at"
 
 
 class Transactions(Stream):
     name = "transactions"
     replication_method = "INCREMENTAL"
     replication_key = "created_at"
     # since API endpoint filter is only on date (and not datetime),
     # make sure to filter out redundant rows.
 
 
 class Statements(Stream):
     name = "statements"
-    replication_method = "INCREMENTAL"
-    replication_key = "updated_at"
+    replication_method = "FULL_TABLE"
+    # replication_key = "updated_at"
 
 
 class Invoices(Stream):
     name = "invoices"
     replication_method = "INCREMENTAL"
-    replication_key = "updated_at"
-    # replication_key = "due_date"
+    # replication_key = "updated_at"
+    replication_key = "due_date"
     # API endpoint filters only on `due_date`.
 
 
 class Events(Stream):
     name = "events"
     replication_method = "FULL_TABLE"
 
@@ -189,9 +189,7 @@
     "components": Components,
     "subscriptions": Subscriptions,
     "transactions": Transactions,
     "statements": Statements,
     "invoices": Invoices,
     "events": Events
 }
-
-
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/statements.json` & `tap-chargify-0.1.0/tap_chargify/schemas/invoices.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7723577235772358%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'subscription_id': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'statement_id': "*

 * *                 "OrderedDict([('type', ['null', 'integer'])]), 'site_id': OrderedDict([('type', "*

 * *                 "['null', 'integer'])]), 'state': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'total_amount_in_cents': OrderedDict([('type', ['null', 'integer'])]), "*

 * *                 "'paid_at': OrderedDict […]*

```diff
@@ -1,402 +1,280 @@
 {
     "properties": {
-        "basic_html_view": {
+        "amount_due_in_cents": {
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "closed_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "created_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_billing_address": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_billing_address_2": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_billing_city": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_billing_country": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_billing_state": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_billing_zip": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_first_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_last_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_organization": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_shipping_address": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_shipping_address_2": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_shipping_city": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_shipping_country": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         },
-        "customer_shipping_state": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_shipping_zip": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ending_balance_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "events": {
+        "charges": {
             "items": {
                 "properties": {
-                    "event": {
-                        "properties": {
-                            "created_at": {
-                                "format": "date-time",
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "event_specific_data": {
-                                "properties": {
-                                    "account_transaction_id": {
-                                        "type": [
-                                            "null",
-                                            "number"
-                                        ]
-                                    },
-                                    "product_id": {
-                                        "type": [
-                                            "null",
-                                            "number"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "number"
-                                ]
-                            },
-                            "key": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "message": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "subscription_id": {
-                                "type": [
-                                    "null",
-                                    "number"
-                                ]
-                            }
-                        },
+                    "amount_in_cents": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "component_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "created_at": {
+                        "format": "date-time",
                         "type": [
                             "null",
-                            "object"
+                            "string"
+                        ]
+                    },
+                    "customer_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "ending_balance_in_cents": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "gateway_order_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "gateway_transaction_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "kind": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "memo": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "payment_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "product_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "starting_balance_in_cents": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "subscription_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "success": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "tax_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "transaction_type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
                         ]
                     }
                 },
                 "type": [
                     "null",
                     "object"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "future_payments": {
-            "items": {},
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "html_view": {
+        "created_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "memo": {
+        "number": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "opened_at": {
+        "paid_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "settled_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "starting_balance_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "subscription_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "text_view": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "total_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "transactions": {
+        "payments_and_credits": {
             "items": {
                 "properties": {
                     "amount_in_cents": {
                         "type": [
                             "null",
-                            "number"
+                            "integer"
                         ]
                     },
-                    "component_id": {
+                    "card_expiration": {
                         "type": [
                             "null",
-                            "number"
+                            "string"
                         ]
                     },
-                    "created_at": {
-                        "format": "date-time",
+                    "card_number": {
                         "type": [
                             "null",
                             "string"
                         ]
                     },
-                    "customer_id": {
+                    "card_type": {
                         "type": [
                             "null",
-                            "number"
+                            "string"
                         ]
                     },
-                    "discount_amount_in_cents": {
+                    "component_id": {
                         "type": [
                             "null",
-                            "number"
+                            "integer"
                         ]
                     },
-                    "ending_balance_in_cents": {
+                    "created_at": {
+                        "format": "date-time",
                         "type": [
                             "null",
-                            "number"
+                            "string"
                         ]
                     },
-                    "gateway_order_id": {
+                    "customer_id": {
                         "type": [
                             "null",
-                            "number"
+                            "integer"
                         ]
                     },
-                    "gateway_transaction_id": {
+                    "ending_balance_in_cents": {
                         "type": [
                             "null",
-                            "string"
+                            "integer"
                         ]
                     },
-                    "gateway_used": {
+                    "gateway_order_id": {
                         "type": [
                             "null",
                             "string"
                         ]
                     },
-                    "id": {
+                    "gateway_transaction_id": {
                         "type": [
                             "null",
-                            "number"
+                            "string"
                         ]
                     },
-                    "item_name": {
+                    "id": {
                         "type": [
                             "null",
-                            "string"
+                            "integer"
                         ]
                     },
                     "kind": {
                         "type": [
                             "null",
                             "string"
                         ]
                     },
                     "memo": {
                         "type": [
                             "null",
                             "string"
                         ]
                     },
-                    "original_amount_in_cents": {
-                        "type": [
-                            "null",
-                            "number"
-                        ]
-                    },
                     "payment_id": {
                         "type": [
                             "null",
-                            "number"
+                            "integer"
                         ]
                     },
                     "product_id": {
                         "type": [
                             "null",
-                            "number"
+                            "integer"
                         ]
                     },
                     "starting_balance_in_cents": {
                         "type": [
                             "null",
-                            "number"
-                        ]
-                    },
-                    "statement_id": {
-                        "type": [
-                            "null",
-                            "number"
+                            "integer"
                         ]
                     },
                     "subscription_id": {
                         "type": [
                             "null",
-                            "number"
+                            "integer"
                         ]
                     },
                     "success": {
                         "type": [
                             "null",
                             "boolean"
                         ]
                     },
                     "tax_id": {
                         "type": [
                             "null",
-                            "number"
-                        ]
-                    },
-                    "taxable_amount_in_cents": {
-                        "type": [
-                            "null",
-                            "number"
-                        ]
-                    },
-                    "taxations": {
-                        "items": {},
-                        "type": [
-                            "null",
-                            "array"
+                            "integer"
                         ]
                     },
                     "transaction_type": {
                         "type": [
                             "null",
                             "string"
                         ]
@@ -414,14 +292,44 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
+        "site_id": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "state": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "statement_id": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "subscription_id": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "total_amount_in_cents": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
         "updated_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/coupons.json` & `tap-chargify-0.1.0/tap_chargify/schemas/coupons.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945436507936507%*

 * *Differences: {"'properties'": "{'amount_in_cents': {'type': {insert: [(1, 'integer')], delete: [1]}}, "*

 * *                 "'conversion_limit': {'type': {insert: [(1, 'integer')], delete: [1]}}, "*

 * *                 "'coupon_restrictions': {'items': {replace: OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', ['null', "*

 * *                 "'integer'])])), ('item_type', OrderedDict([('type', ['null', 'string'])])), "*

 * *                 "('item_id', OrderedDict([('type',  […]*

```diff
@@ -5,15 +5,15 @@
                 "null",
                 "boolean"
             ]
         },
         "amount_in_cents": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "archived_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
@@ -30,19 +30,53 @@
                 "null",
                 "string"
             ]
         },
         "conversion_limit": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "coupon_restrictions": {
-            "items": {},
+            "items": {
+                "properties": {
+                    "handle": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "item_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "item_type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": "object"
+            },
             "type": [
                 "null",
                 "array"
             ]
         },
         "created_at": {
             "format": "date-time",
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/subscriptions.json` & `tap-chargify-0.1.0/tap_chargify/schemas/subscriptions.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603800550577895%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'balance_in_cents': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'total_revenue_in_cents': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'product_price_in_cents': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'product_version_number': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'cancel_at_end_of_period': "*

 * *                 "{'type' […]*

```diff
@@ -6,21 +6,21 @@
                 "null",
                 "string"
             ]
         },
         "balance_in_cents": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "cancel_at_end_of_period": {
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
         "canceled_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
@@ -34,32 +34,20 @@
         },
         "cancellation_method": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "coupon_code": {
+        "coupon_codes": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "coupon_use_count": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "coupon_uses_allowed": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "created_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
@@ -112,15 +100,15 @@
                         "null",
                         "string"
                     ]
                 },
                 "customer_id": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "customer_vault_token": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -142,15 +130,15 @@
                         "null",
                         "string"
                     ]
                 },
                 "id": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "last_name": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -243,15 +231,15 @@
                         "null",
                         "string"
                     ]
                 },
                 "id": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "last_name": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -272,30 +260,31 @@
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "portal_invite_last_accepted_at": {
+                    "format": "date-time",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
                 "portal_invite_last_sent_at": {
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "reference": {
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
                 "state": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -312,15 +301,15 @@
                         "null",
                         "string"
                     ]
                 },
                 "vat_number": {
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
                 "verified": {
                     "type": [
                         "null",
                         "boolean"
                     ]
@@ -334,49 +323,50 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "delayed_cancel_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "expires_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "net_terms": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "next_assessment_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "next_product_id": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "payment_collection_method": {
             "type": [
                 "null",
                 "string"
             ]
@@ -398,17 +388,18 @@
                 "accounting_code": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "archived_at": {
+                    "format": "date-time",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
                 "created_at": {
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
@@ -419,15 +410,15 @@
                         "null",
                         "string"
                     ]
                 },
                 "expiration_interval": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "expiration_interval_unit": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -437,33 +428,33 @@
                         "null",
                         "string"
                     ]
                 },
                 "id": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "initial_charge_after_trial": {
                     "type": [
                         "null",
                         "boolean"
                     ]
                 },
                 "initial_charge_in_cents": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "interval": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "interval_unit": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -473,23 +464,23 @@
                         "null",
                         "string"
                     ]
                 },
                 "price_in_cents": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "product_family": {
                     "properties": {
                         "accounting_code": {
                             "type": [
                                 "null",
-                                "number"
+                                "string"
                             ]
                         },
                         "description": {
                             "type": [
                                 "null",
                                 "string"
                             ]
@@ -499,15 +490,15 @@
                                 "null",
                                 "string"
                             ]
                         },
                         "id": {
                             "type": [
                                 "null",
-                                "number"
+                                "integer"
                             ]
                         },
                         "name": {
                             "type": [
                                 "null",
                                 "string"
                             ]
@@ -520,15 +511,15 @@
                 },
                 "public_signup_pages": {
                     "items": {
                         "properties": {
                             "id": {
                                 "type": [
                                     "null",
-                                    "number"
+                                    "integer"
                                 ]
                             },
                             "url": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
@@ -567,27 +558,27 @@
                         "null",
                         "boolean"
                     ]
                 },
                 "trial_interval": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "trial_interval_unit": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "trial_price_in_cents": {
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
                 "update_return_params": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -616,21 +607,21 @@
                 "null",
                 "object"
             ]
         },
         "product_price_in_cents": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "product_version_number": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "reason_code": {
             "type": [
                 "null",
                 "string"
             ]
@@ -652,39 +643,39 @@
                 "null",
                 "number"
             ]
         },
         "signup_revenue": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "snap_day": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "state": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "stored_credential_transaction_id": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "total_revenue_in_cents": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "trial_ended_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/components.json` & `tap-chargify-0.1.0/tap_chargify/schemas/customers.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7614583333333333%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'first_name': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'last_name': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'cc_emails': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'organization': OrderedDict([('type', ['null', 'string'])]), 'reference': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'updated_at': OrderedDict([('type', "*

 * *                 "['null […]*

```diff
@@ -1,125 +1,141 @@
 {
     "properties": {
-        "archived": {
+        "address": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "created_at": {
-            "format": "date-time",
+        "address_2": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "cc_emails": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "default_price_point_id": {
+        "city": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "description": {
+        "country": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "downgrade_credit": {
+        "created_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "handle": {
+        "first_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "kind": {
+        "last_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
+        "organization": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "price_per_unit_in_cents": {
+        "parent_id": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "price_point_count": {
+        "phone": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "price_points_url": {
+        "portal_customer_created_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "pricing_scheme": {
+        "portal_invite_last_accepted_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "product_family_id": {
+        "portal_invite_last_sent_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "recurring": {
+        "reference": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "tax_code": {
+        "state": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "taxable": {
+        "tax_exempt": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "unit_name": {
+        "updated_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "unit_price": {
+        "vat_number": {
             "type": [
                 "null",
-                "number"
+                "string"
+            ]
+        },
+        "verified": {
+            "type": [
+                "null",
+                "boolean"
             ]
         },
-        "upgrade_charge": {
+        "zip": {
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/customers.json` & `tap-chargify-0.1.0/tap_chargify/schemas/components.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7616279069767442%*

 * *Differences: {"'properties'": "{'name': OrderedDict([('type', ['null', 'string'])]), 'handle': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'pricing_scheme': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'unit_name': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'unit_price': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'product_family_id': OrderedDict([('type', ['null', 'integer'])]), "*

 * *                 "'price_per_unit_in_cents': OrderedDict […]*

```diff
@@ -1,141 +1,190 @@
 {
     "properties": {
-        "address": {
+        "archived": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "address_2": {
+        "created_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "cc_emails": {
+        "default_price_point_id": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "city": {
+        "default_price_point_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "country": {
+        "description": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "created_at": {
-            "format": "date-time",
+        "downgrade_credit": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "first_name": {
+        "handle": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "last_name": {
+        "kind": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "organization": {
+        "name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "parent_id": {
+        "price_per_unit_in_cents": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "phone": {
+        "price_point_count": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "portal_customer_created_at": {
-            "format": "date-time",
+        "price_points_url": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "portal_invite_last_accepted_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
+        "prices": {
+            "items": {
+                "properties": {
+                    "component_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "ending_quantity": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "formatted_unit_price": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "price_point_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "starting_quantity": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "unit_price": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": "object"
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
-        "portal_invite_last_sent_at": {
-            "format": "date-time",
+        "pricing_scheme": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "reference": {
+        "product_family_id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "state": {
+        "product_family_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tax_exempt": {
+        "recurring": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "tax_code": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "vat_number": {
+        "taxable": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "unit_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "verified": {
+        "unit_price": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "zip": {
+        "upgrade_charge": {
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/products.json` & `tap-chargify-0.1.0/tap_chargify/schemas/transactions.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7583333333333333%*

 * *Differences: {"'properties'": "{'subscription_id': OrderedDict([('type', ['null', 'integer'])]), 'type': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'kind': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'transaction_type': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'success': OrderedDict([('type', ['null', 'boolean'])]), "*

 * *                 "'amount_in_cents': OrderedDict([('type', ['null', 'integer'])]), 'memo': "*

 * *                 "OrderedDict([('type', ['nul […]*

```diff
@@ -1,212 +1,213 @@
 {
     "properties": {
-        "accounting_code": {
+        "amount_in_cents": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "archived_at": {
-            "format": "date-time",
+        "card_expiration": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "created_at": {
-            "format": "date-time",
+        "card_number": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "description": {
+        "card_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "expiration_interval": {
+        "component_handle": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "expiration_interval_unit": {
+        "component_id": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "handle": {
+        "component_price_point_handle": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "component_price_point_id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "initial_charge_after_trial": {
+        "created_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "initial_charge_in_cents": {
+        "customer_id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "interval": {
+        "ending_balance_in_cents": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "interval_unit": {
+        "gateway_order_id": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "gateway_transaction_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
+        "gateway_used": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "price_in_cents": {
+        "id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "product_family": {
-            "properties": {
-                "accounting_code": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "description": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "handle": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "id": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "item_name": {
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "public_signup_pages": {
-            "items": {},
+        "kind": {
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "request_credit_card": {
+        "memo": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "require_credit_card": {
+        "parent_id": {
             "type": [
                 "null",
-                "boolean"
+                "integer"
             ]
         },
-        "return_params": {
+        "payment_id": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "period_range_end": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tax_code": {
+        "period_range_start": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "taxable": {
+        "price_point_handle": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "trial_interval": {
+        "price_point_id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "trial_interval_unit": {
+        "product_id": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "trial_price_in_cents": {
+        "refunded_amount_in_cents": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "update_return_params": {
+        "role": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "update_return_url": {
+        "starting_balance_in_cents": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "statement_id": {
             "type": [
                 "null",
-                "string"
+                "integer"
+            ]
+        },
+        "subscription_id": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "success": {
+            "type": [
+                "null",
+                "boolean"
             ]
         },
-        "version_number": {
+        "tax_id": {
             "type": [
                 "null",
                 "integer"
             ]
+        },
+        "transaction_type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "type": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/price_points.json` & `tap-chargify-0.1.0/tap_chargify/schemas/price_points.json`

 * *Files identical despite different names*

### Comparing `tap-chargify-0.0.9/tap_chargify/schemas/transactions.json` & `tap-chargify-0.1.0/tap_chargify/schemas/events.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7722222222222221%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'subscription_id': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'key': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'message': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'event_specific_data': OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('account_transaction_id', OrderedDict([('type', ['null', "*

 * *                 "'integ […]*

```diff
@@ -1,170 +1,190 @@
 {
     "properties": {
-        "amount_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "card_expiration": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "card_number": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "card_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "component_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "created_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "customer_id": {
+        "event_specific_data": {
+            "properties": {
+                "account_transaction_id": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "current_step": {
+                    "properties": {
+                        "action": {
+                            "type": "string"
+                        },
+                        "day_threshold": {
+                            "type": "integer"
+                        },
+                        "email_body": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "email_subject": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "send_bcc_email": {
+                            "type": "boolean"
+                        },
+                        "send_email": {
+                            "type": "boolean"
+                        },
+                        "send_sms": {
+                            "type": "boolean"
+                        },
+                        "sms_body": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "dunner": {
+                    "properties": {
+                        "attempts": {
+                            "type": "integer"
+                        },
+                        "created_at": {
+                            "type": "string"
+                        },
+                        "last_attempted_at": {
+                            "type": "string"
+                        },
+                        "revenue_at_risk_in_cents": {
+                            "type": "integer"
+                        },
+                        "state": {
+                            "type": "string"
+                        },
+                        "subscription_id": {
+                            "type": "integer"
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "new_product_id": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "new_subscription_state": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "next_step": {
+                    "properties": {
+                        "action": {
+                            "type": "string"
+                        },
+                        "day_threshold": {
+                            "type": "integer"
+                        },
+                        "email_body": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "email_subject": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "send_bcc_email": {
+                            "type": "boolean"
+                        },
+                        "send_email": {
+                            "type": "boolean"
+                        },
+                        "send_sms": {
+                            "type": "boolean"
+                        },
+                        "sms_body": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "previous_product_id": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "previous_subscription_state": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "product_id": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                }
+            },
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "ending_balance_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "gateway_order_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "gateway_transaction_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "gateway_used": {
-            "type": [
-                "null",
-                "string"
+                "object"
             ]
         },
         "id": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "item_name": {
+        "key": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "kind": {
+        "message": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "memo": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "parent_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "payment_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "product_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "refunded_amount_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "role": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "starting_balance_in_cents": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "statement_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "subscription_id": {
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "success": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "tax_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "transaction_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "type": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `tap-chargify-0.0.9/tap_chargify/discover.py` & `tap-chargify-0.1.0/tap_chargify/discover.py`

 * *Files identical despite different names*

### Comparing `tap-chargify-0.0.9/setup.py` & `tap-chargify-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-chargify",
-    version="0.0.9",
+    version="0.1.0",
     description="Singer.io tap for extracting Chargify data",
     author="Stitch",
     url="http://github.com/singer-io/tap-chargify",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_chargify"],
     install_requires=[
         "singer-python==5.6.1",
```

