# Comparing `tmp/requestsbankrko-0.2.1.tar.gz` & `tmp/requestsbankrko-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.1.tar", last modified: Thu Jun 22 14:41:56 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.2.tar", last modified: Mon Jul 17 06:14:04 2023, max compression
```

## Comparing `requestsbankrko-0.2.1.tar` & `requestsbankrko-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 14:41:56.000000 requestsbankrko-0.2.1/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:41:56.074725 requestsbankrko-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-06-22 14:41:34.000000 requestsbankrko-0.2.1/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:04.317904 requestsbankrko-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 06:14:04.317904 requestsbankrko-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:14:04.317904 requestsbankrko-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:04.317904 requestsbankrko-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:04.317904 requestsbankrko-0.2.2/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 06:14:04.000000 requestsbankrko-0.2.2/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 06:14:04.000000 requestsbankrko-0.2.2/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:14:04.000000 requestsbankrko-0.2.2/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 06:14:04.000000 requestsbankrko-0.2.2/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 06:14:04.000000 requestsbankrko-0.2.2/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:04.317904 requestsbankrko-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56956 2023-07-17 06:13:44.000000 requestsbankrko-0.2.2/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.1/LICENSE` & `requestsbankrko-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.1/PKG-INFO` & `requestsbankrko-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.1
+Version: 0.2.2
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.1/pyproject.toml` & `requestsbankrko-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.1"
+version = "0.2.2"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.1/src/bank_methods.py` & `requestsbankrko-0.2.2/src/bank_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -838,7 +838,53 @@
         }
 
     def do_json(self):
         if 'success' in self.response_json:
             if 'id' in self.response_json:
                 self.success = True
                 return self.response_json['id']
+
+
+class Kontur(RequestsGarantTestBaseUrl):
+    base_url = 'https://api-crm-billing.kontur.ru'
+    base_url_test = 'https://api-billy-crm.testkontur.ru/'
+
+
+    def __init__(self, json, test):
+        super().__init__()
+        self.test = test
+        self.json = json
+        self.headers = {'x-Auth-CustomToken': os.environ.get('kontur_token')}
+
+    def do_json(self):
+        prospective_sale_id = self.response_json.get('ProspectiveSaleId')
+        if prospective_sale_id is not None:
+            self.success = True
+            return prospective_sale_id
+        results = self.response_json.get('Results')
+        if results is not None:
+            if results:
+                message = results[0].get('Message')
+                if message is not None:
+                    if message in self.invalids:
+                        self.success = True
+                        return inn_busy
+
+
+class KonturCanCreate(Kontur):
+    invalids = ['Есть такая же потенциальная продажа в запрашиваемом PartnerCode']
+    def __init__(self, json, test):
+        super().__init__(json, test)
+        self.endpoint = '/prospectivesales/cancreate/v2'
+        self.method = 'post'
+
+
+
+
+class KonturProspectiveSales(Kontur):
+    invalids = ['Потенциальная продажа с таким Id уже существует']
+    def __init__(self, json, test):
+        super().__init__(json, test)
+        self.endpoint = '/prospectivesales/create/v4'
+        self.method = 'post'
+
+
```

### Comparing `requestsbankrko-0.2.1/src/open_methods.py` & `requestsbankrko-0.2.2/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.1/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.2/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.1
+Version: 0.2.2
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.1/src/zip_functions.py` & `requestsbankrko-0.2.2/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.1/tests/test_bank_methods.py` & `requestsbankrko-0.2.2/tests/test_bank_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1259,8 +1259,132 @@
         print(obj.response.request.headers)
         print(obj.response.text)
         print(obj.response.content)
         print(obj.response.json())
 #         {"success":true,"id":2192696}
 
 
+class KonturTestCase(TestCase):
+    def test_0(self):
+        # json = {
+        #     "ProspectiveSaleId": "8d1a3f97-fabd-46b9-972c-eb3c2437a913",
+        #     "Organization": {
+        #         "Inn": "7654776644",
+        #         "IsPhysical": False,
+        #         "Name": "ООО «Боевые Робоединороги»",
+        #         "Region": "66",
+        #         "City": "Екатеринбург",
+        #         "Address": "ул. Малопрудная, д. 5"
+        #     },
+        #     "CountryCode": "RU",
+        #
+        #     "InternalProductId": "Evrika",
+        #     "PartnerCode": "0800",
+        #     "ManagerCode": "08001",
+        #     "Supplier": {
+        #         "PartnerCode": "1000",
+        #         "Inn": "0300797309",
+        #         "Kpp": "030001001"
+        #     },
+        #     "Type": 1,
+        #     "LifeTime": "2023-08-12T10:14:06",
+        #
+        #     "Brief": {
+        #         "Type": "05a05a89-2c0c-4087-a3bf-f45df4af3e79"
+        #     },
+        #     "SpecialScheme": 0,
+        # }
+        json = {
+            # "ProspectiveSaleId": "6c2ee486-eb32-4515-a3aa-0bc40825b39a",
+            "Organization": {
+                "Inn": "7654776644",
+                # "Kpp": "765401001",
+                "IsPhysical": False,
+                "Name": "ООО «Боевые Робоединороги»",
+                "Region": "66",
+                "City": "Екатеринбург",
+                "Address": "ул. Малопрудная, д. 5"
+            },
+            "CountryCode": "RU",
+            "ForeignOrganization": None,
+            "ExternalProductId": None,
+            "InternalProductId": "Evrika",
+            "PartnerCode": "b0000",
+            # "ManagerCode": "08001",
+            # "Supplier": {
+            #     "PartnerCode": "1000",
+            #     "Inn": "0300797309",
+            #     "Kpp": "030001001"
+            # },
+            "Type": 1,
+        }
+        print(KonturCanCreate(json, True).get_rezult())
 
+    def test_2(self):
+        json = {
+            # "ProspectiveSaleId": "7cd28409-4c7c-4b55-af5e-f388a3326124",
+            "Organization": {
+                "Inn": "7654776644",
+                # "Kpp": "765401001",
+                "IsPhysical": False,
+                "Name": "ООО «Боевые Робоединороги»",
+                "Region": "66",
+                "City": "Екатеринбург",
+                "Address": "ул. Малопрудная, д. 5"
+            },
+            "Contacts": [
+                {
+                    "Name": "Кропоткин Василий Павлович",
+                    "Position": "Директор",
+                    "Phones": [
+                        {
+                            "Id": "98da9a79-55f2-46a0-bfa8-a50b8cbce3c4",
+                            "Number": "+75554440011",
+                            "AdditionalNumber": "123"
+                        }
+                    ],
+                    "Emails": [
+                        {
+                            "Address": "ooo@yandex.ru"
+                        }
+                    ]
+                }
+            ],
+            "Source": "www.source.ru",
+            "CountryCode": "RU",
+            "ForeignOrganization": None,
+            "ExternalProductId": None,
+            "InternalProductId": "Evrika",
+            "PartnerCode": "b0000",
+            # "ManagerCode": "08001",
+            # "Supplier": {
+            #     "PartnerCode": "1000",
+            #     "Inn": "0300797309",
+            #     "Kpp": "030001001"
+            # },
+            "Type": 1,
+        }
+
+        # json = {
+        #     'ProspectiveSaleId': 'adf1e209-1308-4713-87a1-18f8c01995ef',
+        #     "Contacts": [
+        #         {
+        #             "Name": "Кропоткин Василий Павлович",
+        #             "Position": "Директор",
+        #             "Phones": [
+        #                 {
+        #                     "Id": "98da9a79-55f2-46a0-bfa8-a50b8cbce3c4",
+        #                     "Number": "+75554440011",
+        #                     "AdditionalNumber": "123"
+        #                 }
+        #             ],
+        #             "Emails": [
+        #                 {
+        #                     "Address": "ooo@yandex.ru"
+        #                 }
+        #             ]
+        #         }
+        #     ],
+        #     "InternalProductId": "Evrika",
+
+        # }
+        print(KonturProspectiveSales(json, True).get_rezult())
```

