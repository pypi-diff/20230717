# Comparing `tmp/ar_ex_sys_worker-1.6.34-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16348 bytes, number of entries: 11
+Zip file size: 16700 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    29611 b- defN 23-Jul-10 07:24 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19901 b- defN 23-Jun-05 10:30 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    31099 b- defN 23-Jul-17 13:54 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    21310 b- defN 23-Jul-17 13:52 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
--rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
+-rw-rw-rw-  2.0 fat    11309 b- defN 23-Jul-17 13:52 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/RECORD
-11 files, 64388 bytes uncompressed, 14632 bytes compressed:  77.3%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-17 14:12 ar_ex_sys_worker-1.6.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      343 b- defN 23-Jul-17 14:12 ar_ex_sys_worker-1.6.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 14:12 ar_ex_sys_worker-1.6.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-17 14:12 ar_ex_sys_worker-1.6.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 23-Jul-17 14:12 ar_ex_sys_worker-1.6.4.dist-info/RECORD
+11 files, 67363 bytes uncompressed, 14994 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.34.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.34.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.4.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.34.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.34.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.34.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -455,15 +455,16 @@
 
 
 class SignAllActsWorkerToken(mixins.TokenAuth, SignallActWorker,
                              mixins.TokenDBAuth,
                              mixins.SignallActDBDeletter,
                              mixins.ExSysActIdExtractor,
                              mixins.SignallActUpdater,
-                             mixins.SignallActDeletter):
+                             mixins.SignallActDeletter,
+                             mixins.ARAPIWork):
     def __init__(self, sql_shell, trash_cats_list, time_start, platform_id,
                  acts_limit=5, gravity_ip=None, gravity_port=8080, test=False,
                  mutex=None):
         super().__init__(sql_shell, trash_cats_list, time_start, acts_limit,
                          auto_auth=False, mutex=mutex)
         self.platform_id = platform_id
         self.gravity_ip = gravity_ip
@@ -478,14 +479,37 @@
             self.link_host = 'https://signalltestdev.qodex.tech'
         self.signall_update_act_link = self.get_full_endpoint(
                 '/v1/gravity/update_act/{}')
         self.signal_del_act_url = self.get_full_endpoint(
             "/v1/acts/delete_act_by_id/{}"
         )
 
+    def get_region_operators(self):
+        resp = requests.get(url=self.get_full_endpoint("/v1/gravity/get_ro"),
+                            headers=self.headers)
+        for ro in resp.json()["ro"]:
+            self.insert_client_to_gravity(name=ro['name'],
+                                          inn=ro['inn'], kpp=ro['kpp'],
+                                          push_to_cm=False)
+            self.make_client_region_operator(inn=ro['inn'], kpp=ro['kpp'],
+                                             push_to_cm=False)
+
+    def get_tko_carriers(self):
+        resp = requests.get(
+            url=self.get_full_endpoint("/v1/gravity/transporter"),
+            headers=self.headers)
+        for client in resp.json()['transporters']:
+            self.insert_client_to_gravity(name=client['name'],
+                                          inn=client['inn'],
+                                          kpp=client['kpp'],
+                                          push_to_cm=False)
+            self.make_client_tko_carrier(inn=client['inn'],
+                                         push_to_cm=False,
+                                         kpp=client['kpp'])
+
     def del_act(self, record_id):
         signal_id = self.extract_act_ex_id(record_id)
         if not signal_id:
             return
         if signal_id.strip() == 'this carrier was not found':
             self.delete_act_from_send_reports(record_id)
             return {'error': {f'Act has not been delivered cos {signal_id}. '
@@ -669,33 +693,39 @@
         self.login = login
         self.password = password
         self.headers = self.get_headers()
         self.working_link = self.get_full_endpoint(
             '/v1/gravity/transporter')
         self.ar_ip = ar_ip
 
+    def get_region_operators(self):
+        resp = self.get_cars(self.get_full_endpoint("/v1/gravity/get_ro"))
+        print(resp)
+
     def import_clients(self):
         resp = self.get_cars()
         for client in resp['transporters']:
             self.insert_client_to_gravity(name=client['name'],
                                           inn=client['inn'],
                                           kpp=client['kpp'],
                                           push_to_cm=False)
             self.make_client_tko_carrier(inn=client['inn'],
-                                         push_to_cm=False)
+                                         push_to_cm=False,
+                                         kpp=client['kpp'])
 
     def insert_client_to_gravity(self, name, inn, kpp, push_to_cm):
         return requests.post(url=f'{self.ar_ip}:8080/add_client',
                              params=
                              {'name': name,
                               'inn': inn,
                               'kpp': kpp,
                               'push_to_cm': push_to_cm,
                               })
 
-    def make_client_tko_carrier(self, inn, push_to_cm):
+    def make_client_tko_carrier(self, inn, push_to_cm, kpp):
         return requests.post(url=f'{self.ar_ip}:8080/make_client_tko_carrier',
                              params=
                              {
                                  'inn': inn,
-                                 'push_to_cm': push_to_cm
+                                 'push_to_cm': push_to_cm,
+                                 'kpp': kpp
                              })
```

## ar_external_sys_worker/mixins.py

```diff
@@ -223,21 +223,54 @@
     def get_carriers_po(self):
         if not self.get_carriers_po_link:
             return {'error': 'There are not link for route get_carriers'}
         response = requests.get(self.get_carriers_po_link,
                                 headers=self.headers)
         return response
 
+class ARAPIWork:
+    gravity_ip = None
+    gravity_port = 8080
+
+    def insert_client_to_gravity(self, name, inn, kpp, push_to_cm):
+        return requests.post(url=f'http://{self.gravity_ip}:{self.gravity_port}/add_client',
+                             params=
+                             {'name': name,
+                              'inn': inn,
+                              'kpp': kpp,
+                              'push_to_cm': push_to_cm,
+                              })
+
+    def make_client_tko_carrier(self, inn, push_to_cm, kpp):
+        return requests.post(url=f'http://{self.gravity_ip}:{self.gravity_port}/make_client_tko_carrier',
+                             params=
+                             {
+                                 'inn': inn,
+                                 'push_to_cm': push_to_cm,
+                                 'kpp': kpp
+                             })
+
+    def make_client_region_operator(self, inn, kpp, push_to_cm):
+        return requests.post(url=f'http://{self.gravity_ip}:{self.gravity_port}/make_client_region_operator',
+                             params=
+                             {
+                                 'inn': inn,
+                                 'push_to_cm': push_to_cm,
+                                 'kpp': kpp
+                             })
+
 
 class SignAllCarsGetter:
     headers = None
     working_link = None
 
-    def get_cars(self):
-        response = requests.get(self.working_link,
+    def get_cars(self, link=None):
+        if not link:
+            link = self.working_link
+        response = requests.get(link,
                                 headers=self.headers)
         return response.json()
 
 
 class ExSysActIdExtractor:
     sql_shell = None
     ex_sys_id = None
```

## ar_external_sys_worker/tests/main_test.py

```diff
@@ -180,14 +180,22 @@
             resp = inst.insert_client_to_gravity(name=client['name'],
                                                  inn=client['inn'],
                                                  kpp=client['kpp'])
             inst.make_client_tko_carrier(inn=client['inn'])
             print(resp.json())
 
     @unittest.SkipTest
+    def test_ro_getter(self):
+        inst = main.SignallClientsGetter(self.sql_shell,
+                                         'http://127.0.0.1',
+                                         login='1@signal.com',
+                                         password='d4GExhec')
+        inst.get_region_operators()
+
+    @unittest.SkipTest
     def test_get_platforms(self):
         car_nums = [
             'О539КН102',
             '2267УК01',
             'В106ХУ02',
             'В662СН702',
             'Х237ТМ702',
@@ -211,32 +219,26 @@
         for car_num in car_nums:
             print('\n')
             print(car_num)
             res = inst.get_route_info('В292МР702', '05.12.2022')
             print(res)
 
     def test_mutex(self):
-        print("first_go")
         inst = main.SignAllActsWorkerToken(self.sql_shell,
                                            ['ТКО', 'Прочее', 'ПО', 'Хвосты'],
                                            '2023.04.24',
                                            1,
-                                           gravity_ip='172.16.9.20',
+                                           gravity_ip='80.87.199.109',
+                                           gravity_port=8080,
                                            test=True)
-        inst.set_signall_test()
-        #inst.link_host = 'https://signalltestdev.qodex.tech'
         inst.auth()
-        threading.Thread(target=inst.send_unsend_acts).start()
-        time.sleep(2)
-        print("second_go")
-        threading.Thread(target=inst.send_unsend_acts).start()
-        time.sleep(2)
-        print("third_go")
-        threading.Thread(target=inst.send_unsend_acts).start()
+        inst.get_region_operators()
+        inst.get_tko_carriers()
 
+    @unittest.SkipTest
     def signall_worker_token(self):
         inst = main.SignAllActsWorkerToken(self.sql_shell,
                                            ['ТКО', 'Прочее', 'ПО', 'Хвосты'],
                                            '2023.04.24',
                                            1,
                                            gravity_ip='172.16.9.20',
                                            test=True)
```

## Comparing `ar_ex_sys_worker-1.6.34.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.6.34.dist-info/RECORD` & `ar_ex_sys_worker-1.6.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/main.py,sha256=siK5hgjkjs-W872amUkUx8lxqXXyQ6Qyinoxxc2ghF0,29611
-ar_external_sys_worker/mixins.py,sha256=SNDYlBYQXTvm5jx-SwDwxUu4E-gP76rmAgYncQ6hAJc,19901
+ar_external_sys_worker/main.py,sha256=PqPpZTVSQ1BmIgC6CyOZSc7MZccrHmjKxiec9eAwtvE,31099
+ar_external_sys_worker/mixins.py,sha256=Q84Si-8316BkgLnwRVjsHxMUom9wyeffeSfoaYyA2go,21310
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/tests/main_test.py,sha256=eOqy3_5sPoq7knV5fjESJ6FVWEXehwSOLTd8qXckdXw,11225
+ar_external_sys_worker/tests/main_test.py,sha256=2UbA-og0LvYWJXLUfTyRH0x7KEZMdZMYWuCJ7DBHM5k,11309
 ar_external_sys_worker/tests/mixins_test.py,sha256=NTPOm74h7bL5ra_acU3AxLgDhn75waGOGKtbkkGSxoc,1107
-ar_ex_sys_worker-1.6.34.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.6.34.dist-info/METADATA,sha256=fzufr7vP-5IWc_YVZal6Hmmv3IFtggPWK9nJTXFG0Cs,344
-ar_ex_sys_worker-1.6.34.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ar_ex_sys_worker-1.6.34.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.6.34.dist-info/RECORD,,
+ar_ex_sys_worker-1.6.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.6.4.dist-info/METADATA,sha256=JHFvixOj9sHtNca2Zp7A78-CER6KxuFJbF4CnWtdHn0,343
+ar_ex_sys_worker-1.6.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ar_ex_sys_worker-1.6.4.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.6.4.dist-info/RECORD,,
```

