# Comparing `tmp/tmsproviderapisdk-0.1.1.tar.gz` & `tmp/tmsproviderapisdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmsproviderapisdk-0.1.1.tar", last modified: Tue May 18 14:55:32 2021, max compression
+gzip compressed data, was "tmsproviderapisdk-0.1.2.tar", last modified: Mon Jul 17 13:59:50 2023, max compression
```

## Comparing `tmsproviderapisdk-0.1.1.tar` & `tmsproviderapisdk-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 14:55:32.156195 tmsproviderapisdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      929 2021-05-18 14:55:32.156195 tmsproviderapisdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-18 14:55:32.156195 tmsproviderapisdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-05-18 14:55:31.000000 tmsproviderapisdk-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 14:55:32.152195 tmsproviderapisdk-0.1.1/tmsproviderapisdk/
--rw-r--r--   0 runner    (1001) docker     (121)      535 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_account_subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3356 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_device_subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_extended_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_tarif.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-05-18 14:55:25.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_tarif_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 14:55:32.156195 tmsproviderapisdk-0.1.1/tmsproviderapisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      929 2021-05-18 14:55:32.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      685 2021-05-18 14:55:32.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-18 14:55:32.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-18 14:55:32.000000 tmsproviderapisdk-0.1.1/tmsproviderapisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-17 13:59:49.000000 tmsproviderapisdk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/tmsproviderapisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_extended_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/top_level.txt
```

### Comparing `tmsproviderapisdk-0.1.1/LICENSE` & `tmsproviderapisdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/setup.py` & `tmsproviderapisdk-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmsproviderapisdk",
-    version="0.1.1",
+    version="0.1.2",
     author="Tvip",
     author_email="td@tvip.ru",
     description="TVIP TMS provider api sdk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tvip/tmsproviderapisdk",
     packages=setuptools.find_packages(),
```

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/__init__.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,7 +3,8 @@
 from tmsproviderapisdk.tms_account_subscription import TmsAccountSubscription
 from tmsproviderapisdk.tms_channel import TmsChannel
 from tmsproviderapisdk.tms_device import TmsDevice
 from tmsproviderapisdk.tms_device_subscription import TmsDeviceSubscription
 from tmsproviderapisdk.tms_tarif import TmsTarif
 from tmsproviderapisdk.tms_tarif_tag import TmsTarifTag
 from tmsproviderapisdk.tms_region import TmsRegion
+from tmsproviderapisdk.tms_account_network import TmsAccountNetwork
```

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_account.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,47 @@
 from tmsproviderapisdk.tms_extended_model import TmsExtendedModel
 import hashlib
 
 
 class TmsAccount(TmsExtendedModel):
     _path_url = '/accounts/'
 
-    def __init__(self, login: str, fullname: str, account_desc: str = "", contract_info: str = "",
-                 devices_per_account_limit: int = None, enabled: bool = True, main_address: str = "", pin_md5: str = "",
-                 remote_custom_field: str = "", provider: int = None, id: int = None, region_tag=None):
+    def __init__(self,
+                 login: str,
+                 fullname: str,
+                 account_desc: str = "",
+                 contract_info: str = "",
+                 devices_per_account_limit: int = None,
+                 enabled: bool = True,
+                 main_address: str = "",
+                 pin_md5: str = "",
+                 remote_custom_field: str = "",
+                 provider: int = None,
+                 id: int = None,
+                 region_tag: int = None,
+                 last_online: int = None,
+                 created: int = None,
+                 updated: int = None
+                 ):
 
         self.login = login
         self.fullname = fullname
         self.account_desc = account_desc
         self.contract_info = contract_info
         self.devices_per_account_limit = devices_per_account_limit
         self.enabled = enabled
         self.main_address = main_address
         self.pin_md5 = pin_md5
         self.remote_custom_field = remote_custom_field
         self.provider = provider
         self.id = id
         self.region_tag = region_tag
+        self.last_online = last_online
+        self.created = created
+        self.updated = updated
 
     @staticmethod
     def get_md5_pin(clear_text_password: str) -> str:
         hash_password = hashlib.md5(clear_text_password.encode())
         pin_md5 = hash_password.hexdigest()
 
         return pin_md5
@@ -39,39 +56,48 @@
                                    enabled=account_dict["enabled"],
                                    fullname=account_dict["fullname"],
                                    main_address=account_dict["main_address"],
                                    pin_md5=account_dict["pin_md5"],
                                    remote_custom_field=account_dict["remote_custom_field"],
                                    provider=account_dict["provider"],
                                    id=account_dict["id"],
-                                   region_tag=account_dict["region_tag"])
+                                   region_tag=account_dict["region_tag"],
+                                   last_online=account_dict["last_online"],
+                                   created=account_dict["created"],
+                                   updated=account_dict["updated"],
+                                   )
 
         return a
 
     @classmethod
-    def get_list(cls, start: int = 0, limit: int = 50, sort: str = "", provider: int = None, enabled: bool = None,
-                 login: int = None, remote_custom_field: str = "",
+    def get_list(cls, start: int = 0, limit: int = 50, sort: str = "", provider: int = None, region_tag: int = None,
+                 enabled: bool = None, login: int = None, remote_custom_field: str = "",
                  quick_search: str = "") -> Optional[Tuple[List[object], int]]:
 
         accounts: Optional[Tuple[List[object], int]] = super().get_list(start, limit, sort=sort, provider=provider,
-                                                                        enabled=enabled, login=login,
+                                                                        region_tag=region_tag, enabled=enabled,
+                                                                        login=login,
                                                                         remote_custom_field=remote_custom_field,
                                                                         quick_search=quick_search)
 
         return accounts
 
     def __str__(self):
         return """id:{}, login:{}, fullname:{}, remote_custom_field:{}, pin_md5:{}, contract_info:{},\
- main_address:{}, account_desc:{}, provider:{}, enabled:{}, devices_per_account_limit:{}, region_tag:{}""".format(
+ main_address:{}, account_desc:{}, provider:{}, enabled:{}, devices_per_account_limit:{}, region_tag:{}, last_online:{},
+ created:{}, updated:{} """.format(
             self.id,
             self.login,
             self.fullname,
             self.remote_custom_field,
             self.pin_md5,
             self.contract_info,
             self.main_address,
             self.account_desc,
             self.provider,
             self.enabled,
             self.devices_per_account_limit,
-            self.region_tag
+            self.region_tag,
+            self.last_online,
+            self.created,
+            self.updated
         )
```

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_account_subscription.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from typing import Optional, List, Tuple
 from tmsproviderapisdk.tms_extended_model import TmsExtendedModel
 
 
 class TmsAccountSubscription(TmsExtendedModel):
     _path_url = "/account_subscriptions/"
 
-    def __init__(self, account: int, start: str, tarif: int, id: int = None, stop: str = None):
+    def __init__(self, account: int, start: str, tarif: int, id: int = None, stop: str = None,
+                 time_shift_depth: int = None):
         self.account = account
         self.start = start
         self.tarif = tarif
         self.id = id
         self.stop = stop
+        self.time_shift_depth = time_shift_depth
 
     @staticmethod
     def _dict_to_object(as_dict: dict) -> object:
         account_subscription = TmsAccountSubscription(
             account=as_dict["account"],
             id=as_dict["id"],
             start=as_dict["start"],
             stop=as_dict["stop"],
-            tarif=as_dict["tarif"]
+            tarif=as_dict["tarif"],
+            time_shift_depth=as_dict["time_shift_depth"]
         )
+
         return account_subscription
 
     @classmethod
     def get_list(cls, start: int = 0, limit: int = 50, sort: str = "", account: int = None, tarif: int = None,
                  quick_search: str = "") -> Optional[Tuple[List[object], int]]:
         account_subscriptions = super().get_list(start=start, limit=limit, sort=sort, account=account,
                                                  tarif=tarif, quick_search=quick_search)
 
         return account_subscriptions
 
     def __str__(self):
-        return """id:{}, account:{}, start:{}, stop:{}, tarif:{}""".format(
+        return """id:{}, account:{}, start:{}, stop:{}, tarif:{}, time_shift_depth:{}""".format(
             self.id,
             self.account,
             self.start,
             self.stop,
-            self.tarif
+            self.tarif,
+            self.time_shift_depth
         )
```

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_base_model.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_base_model.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_channel.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_channel.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,48 +2,51 @@
 from tmsproviderapisdk.tms_base_model import TmsBaseModel
 
 
 class TmsChannel(TmsBaseModel):
     _path_url = "/channels/"
 
     def __init__(self, id: int, name: str = "", text_name: str = "", display_number: str = "", logo_url: str = "",
-                 enabled: bool = False, time_shift_depth: int = None):
+                 enabled: bool = False, time_shift_depth: int = None, favorites: List = None):
 
         self.id = id
         self.name = name
         self.text_name = text_name
         self.display_number = display_number
         self.logo_url = logo_url
         self.enabled = enabled
         self.time_shift_depth = time_shift_depth
+        self.favorites = favorites
 
     @staticmethod
     def _dict_to_object(channel_dict: dict) -> object:
         channel = TmsChannel(
             id=channel_dict["id"],
             name=channel_dict["name"],
             text_name=channel_dict["text_name"],
             display_number=channel_dict["display_number"],
             logo_url=channel_dict["logo_url"],
             enabled=channel_dict["enabled"],
-            time_shift_depth=channel_dict["time_shift_depth"]
+            time_shift_depth=channel_dict["time_shift_depth"],
+            favorites=channel_dict["favorites"]
         )
         return channel
 
     @classmethod
     def get_list(cls, start: int = 0, limit: int = 50, sort: str = "", tarif: int = None, enabled: bool = None,
                  quick_search: str = "") -> Optional[Tuple[List[object], int]]:
         channels = super().get_list(start=start, limit=limit, sort=sort, tarif=tarif, quick_search=quick_search)
 
         return channels
 
     def __str__(self):
         return """id:{}, name:{}, text_name:{}, display_number:{}, logo_url:{}, \
-            enabled: {}, time_shift_depth: {}""".format(
+            enabled: {}, time_shift_depth: {}, favorites: {}""".format(
                 self.id,
                 self.name,
                 self.text_name,
                 self.display_number,
                 self.logo_url,
                 self.enabled,
-                self.time_shift_depth
+                self.time_shift_depth,
+                self.favorites
             )
```

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_config.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_config.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_device.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_device_subscription.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from typing import List, Optional, Tuple
 from tmsproviderapisdk.tms_extended_model import TmsExtendedModel
 
 
 class TmsDeviceSubscription(TmsExtendedModel):
     _path_url = "/device_subscriptions/"
 
-    def __init__(self, device: int, start: str, tarif: int, id: int = None, stop: str = None):
+    def __init__(self, device: int, start: str, tarif: int, id: int = None, stop: str = None,
+                 time_shift_depth: int = None):
 
         self.device = device
         self.start = start
         self.tarif = tarif
         self.id = id
         self.stop = stop
+        self.time_shift_depth = time_shift_depth
 
     @staticmethod
-    def _dict_to_object(as_dict: dict) -> object:
+    def _dict_to_object(ds_dict: dict) -> object:
         device_subscription = TmsDeviceSubscription(
-            device=as_dict["device"],
-            id=as_dict["id"],
-            start=as_dict["start"],
-            stop=as_dict["stop"],
-            tarif=as_dict["tarif"]
+            device=ds_dict["device"],
+            id=ds_dict["id"],
+            start=ds_dict["start"],
+            stop=ds_dict["stop"],
+            tarif=ds_dict["tarif"],
+            time_shift_depth=ds_dict["time_shift_depth"]
         )
         return device_subscription
 
     @classmethod
     def get_list(cls, start: int = 0, limit: int = 50, sort: str = "", device: int = None, tarif: int = None,
                  quick_search: str = "") -> Optional[Tuple[List[object], int]]:
 
         device_subscriptions = super().get_list(start=start, limit=limit, sort=sort, device=device, tarif=tarif,
                                                 quick_search=quick_search)
 
         return device_subscriptions
 
     def __str__(self):
-        return """id:{}, device:{}, start:{}, stop:{}, tarif:{}""".format(
+        return """id:{}, device:{}, start:{}, stop:{}, tarif:{}, time_shift_depth:{}""".format(
             self.id,
             self.device,
             self.start,
             self.stop,
-            self.tarif
+            self.tarif,
+            self.time_shift_depth
         )
```

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_exceptions.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_exceptions.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_extended_model.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_extended_model.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_provider.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_provider.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_region.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_region.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_tarif.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk/tms_tarif_tag.py` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif_tag.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.1/tmsproviderapisdk.egg-info/SOURCES.txt` & `tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 tmsproviderapisdk/__init__.py
 tmsproviderapisdk/tms_account.py
+tmsproviderapisdk/tms_account_network.py
 tmsproviderapisdk/tms_account_subscription.py
 tmsproviderapisdk/tms_base_model.py
 tmsproviderapisdk/tms_channel.py
 tmsproviderapisdk/tms_config.py
 tmsproviderapisdk/tms_device.py
 tmsproviderapisdk/tms_device_subscription.py
 tmsproviderapisdk/tms_exceptions.py
```

