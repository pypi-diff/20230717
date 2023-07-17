# Comparing `tmp/atomicshop-1.8.6-py3-none-any.whl.zip` & `tmp/atomicshop-1.8.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 205519 bytes, number of entries: 139
--rw-rw-rw-  2.0 fat      122 b- defN 23-Jul-17 09:50 atomicshop/__init__.py
+Zip file size: 205513 bytes, number of entries: 139
+-rw-rw-rw-  2.0 fat      122 b- defN 23-Jul-17 10:18 atomicshop/__init__.py
 -rw-rw-rw-  2.0 fat     3699 b- defN 23-Jul-10 11:38 atomicshop/_basics_temp.py
 -rw-rw-rw-  2.0 fat     7257 b- defN 23-Jul-10 11:38 atomicshop/appointment_management.py
 -rw-rw-rw-  2.0 fat     4763 b- defN 23-Jul-10 11:38 atomicshop/archiver.py
 -rw-rw-rw-  2.0 fat      297 b- defN 23-Jul-10 11:38 atomicshop/certificates.py
 -rw-rw-rw-  2.0 fat     1038 b- defN 23-Jul-10 11:38 atomicshop/command_line_processing.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 23-Jul-10 11:38 atomicshop/console_output.py
 -rw-rw-rw-  2.0 fat     3234 b- defN 23-Jul-10 11:38 atomicshop/console_user_response.py
@@ -127,15 +127,15 @@
 -rw-rw-rw-  2.0 fat    39756 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/dns_server.py
 -rw-rw-rw-  2.0 fat     4061 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/get_process.py
 -rw-rw-rw-  2.0 fat     8652 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/receiver.py
 -rw-rw-rw-  2.0 fat     3680 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/sender.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/sni.py
 -rw-rw-rw-  2.0 fat    18928 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/socket_client.py
 -rw-rw-rw-  2.0 fat     6314 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/socket_server_tester.py
--rw-rw-rw-  2.0 fat    26718 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/socket_wrapper.py
+-rw-rw-rw-  2.0 fat    26681 b- defN 23-Jul-17 10:12 atomicshop/wrappers/socketw/socket_wrapper.py
 -rw-rw-rw-  2.0 fat      598 b- defN 23-Jul-10 11:38 atomicshop/wrappers/socketw/ssl_base.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-17 09:52 atomicshop-1.8.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     9057 b- defN 23-Jul-17 09:52 atomicshop-1.8.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 09:52 atomicshop-1.8.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-17 09:52 atomicshop-1.8.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    12692 b- defN 23-Jul-17 09:52 atomicshop-1.8.6.dist-info/RECORD
-139 files, 656541 bytes uncompressed, 185163 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-17 10:19 atomicshop-1.8.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     9057 b- defN 23-Jul-17 10:19 atomicshop-1.8.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 10:19 atomicshop-1.8.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-17 10:19 atomicshop-1.8.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    12692 b- defN 23-Jul-17 10:19 atomicshop-1.8.7.dist-info/RECORD
+139 files, 656504 bytes uncompressed, 185157 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -396,23 +396,23 @@
 
 Filename: atomicshop/wrappers/socketw/socket_wrapper.py
 Comment: 
 
 Filename: atomicshop/wrappers/socketw/ssl_base.py
 Comment: 
 
-Filename: atomicshop-1.8.6.dist-info/LICENSE.txt
+Filename: atomicshop-1.8.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: atomicshop-1.8.6.dist-info/METADATA
+Filename: atomicshop-1.8.7.dist-info/METADATA
 Comment: 
 
-Filename: atomicshop-1.8.6.dist-info/WHEEL
+Filename: atomicshop-1.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: atomicshop-1.8.6.dist-info/top_level.txt
+Filename: atomicshop-1.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: atomicshop-1.8.6.dist-info/RECORD
+Filename: atomicshop-1.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atomicshop/__init__.py

```diff
@@ -1,4 +1,4 @@
 """Atomic Basic functions and classes to make developer life easier"""
 
 __author__ = "Den Kras"
-__version__ = '1.8.6'
+__version__ = '1.8.7'
```

## atomicshop/wrappers/socketw/socket_wrapper.py

```diff
@@ -82,16 +82,15 @@
 
         domain_list = self.config['certificates']['domains_all_times']
         server_certificate_file_name_no_extension = self.config['certificates']['default_server_certificate_name']
 
         server_certificate_file_path, default_server_certificate_san = \
             self.certauth_wrapper.create_overwrite_server_certificate_ca_signed_return_path_and_san(
                 domain_list=domain_list,
-                server_certificate_file_name_no_extension=server_certificate_file_name_no_extension,
-                logger=self.logger
+                server_certificate_file_name_no_extension=server_certificate_file_name_no_extension
             )
 
         return server_certificate_file_path, default_server_certificate_san
 
     def select_server_ssl_context_certificate(self):
         # We need to nullify the variable, since we have several checks if the variable was set or not.
         self.server_certificate_file_path: str = str()
```

## Comparing `atomicshop-1.8.6.dist-info/LICENSE.txt` & `atomicshop-1.8.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `atomicshop-1.8.6.dist-info/METADATA` & `atomicshop-1.8.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicshop
-Version: 1.8.6
+Version: 1.8.7
 Summary: Atomic functions and classes to make developer life easier
 Author: Denis Kras
 License: MIT License
         
         Copyright (c) 2023 Bugsec, Denis Kras
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `atomicshop-1.8.6.dist-info/RECORD` & `atomicshop-1.8.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-atomicshop/__init__.py,sha256=vHHtjNhZYT_x_mPY0cGstKv8ZRwxW4tCbWBC9y4lO70,122
+atomicshop/__init__.py,sha256=h36I831zLzGvHJxRRCNwwMaqkU_sLLcJWCpVSh9EYfo,122
 atomicshop/_basics_temp.py,sha256=6cu2dd6r2dLrd1BRNcVDKTHlsHs_26Gpw8QS6v32lQ0,3699
 atomicshop/appointment_management.py,sha256=IsaO1O9Lgso_BPm79QNQkIyunYIr7KuAkTYlityM0nw,7257
 atomicshop/archiver.py,sha256=KKdNI150yiMO_Y1TZdKjXtw4TP5LI5FJzI8VbvFKVwo,4763
 atomicshop/certificates.py,sha256=nxuq6HPBT7RfwRTSipOxoRHBS-nZLsaHR9m6UdHmDn4,297
 atomicshop/command_line_processing.py,sha256=u5yT9Ger_cu7ni5ID0VFlRbVD46ARHeNC9tRM-_YXrQ,1038
 atomicshop/console_output.py,sha256=G-6jxnWooT1nJSaPxcCqIuw8S22R_0lOJcfrdovRhwE,1372
 atomicshop/console_user_response.py,sha256=31HIy9QGXa7f-GVR8MzJauQ79E_ZqAeagF3Ks4GGdDU,3234
@@ -126,14 +126,14 @@
 atomicshop/wrappers/socketw/dns_server.py,sha256=XhJdQ1b78y2iSkZfWKsHrAUPSgP5UEcFOQmeTXtRssA,39756
 atomicshop/wrappers/socketw/get_process.py,sha256=NGy8ShYJ400UB7a3SJj9W8d1wyLYyte-EOJK7Og8kU4,4061
 atomicshop/wrappers/socketw/receiver.py,sha256=jkvvzih4H3giIGLsiUygSzXjYPWpTpA76OdgWjhf9wU,8652
 atomicshop/wrappers/socketw/sender.py,sha256=hHpBLc0LCfOIUErq2mc0ATfp0tDDQ5XhcYT4hRAZARU,3680
 atomicshop/wrappers/socketw/sni.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atomicshop/wrappers/socketw/socket_client.py,sha256=O7PVQF3i4heKptwmck5Y1ELjMQ9tm-R_cdqqFVfIFLc,18928
 atomicshop/wrappers/socketw/socket_server_tester.py,sha256=7-G1t2yyDA-cNQF8zCpQSNlXEqVrMVIsq6IiYIYeKZg,6314
-atomicshop/wrappers/socketw/socket_wrapper.py,sha256=b37dTJyBpiBW01pML2FSdXHfgEvaTFe20j2Lz-2gFJc,26718
+atomicshop/wrappers/socketw/socket_wrapper.py,sha256=SEa8qs1BznnAUNyLDtawZ75rzfuuvHM_AWGdb4zsjvo,26681
 atomicshop/wrappers/socketw/ssl_base.py,sha256=sD2LBwbrRwMS4k2d4CsDpzgpHaMrE4goNATQN-YtyOI,598
-atomicshop-1.8.6.dist-info/LICENSE.txt,sha256=lLU7EYycfYcK2NR_1gfnhnRC8b8ccOTElACYplgZN88,1094
-atomicshop-1.8.6.dist-info/METADATA,sha256=Hmwx4byOWd1rEVa2amNlbqYH9TV0rvrWqGykbS06zic,9057
-atomicshop-1.8.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-atomicshop-1.8.6.dist-info/top_level.txt,sha256=EgKJB-7xcrAPeqTRF2laD_Np2gNGYkJkd4OyXqpJphA,11
-atomicshop-1.8.6.dist-info/RECORD,,
+atomicshop-1.8.7.dist-info/LICENSE.txt,sha256=lLU7EYycfYcK2NR_1gfnhnRC8b8ccOTElACYplgZN88,1094
+atomicshop-1.8.7.dist-info/METADATA,sha256=AQ-ZzReJhrrpzGgwvTvJSQPfgmA73h83ow6EGX3X9To,9057
+atomicshop-1.8.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+atomicshop-1.8.7.dist-info/top_level.txt,sha256=EgKJB-7xcrAPeqTRF2laD_Np2gNGYkJkd4OyXqpJphA,11
+atomicshop-1.8.7.dist-info/RECORD,,
```

