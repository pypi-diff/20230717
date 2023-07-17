# Comparing `tmp/ipfabric-6.3.1b2.tar.gz` & `tmp/ipfabric-6.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.3.1b2.tar", max compression
+gzip compressed data, was "ipfabric-6.3.2b0.tar", max compression
```

## Comparing `ipfabric-6.3.1b2.tar` & `ipfabric-6.3.2b0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1498 2023-07-17 15:20:24.288289 ipfabric-6.3.1b2/ipfabric/__init__.py
--rw-r--r--   0        0        0    17287 2023-07-17 15:20:24.293213 ipfabric-6.3.1b2/ipfabric/api.py
--rw-r--r--   0        0        0    11597 2023-07-14 16:09:22.706505 ipfabric-6.3.1b2/ipfabric/client.py
--rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.3.1b2/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    14821 2023-07-13 12:33:49.973872 ipfabric-6.3.1b2/ipfabric/models/device.py
--rw-r--r--   0        0        0     5842 2023-06-01 16:01:19.099648 ipfabric-6.3.1b2/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.3.1b2/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2219 2023-07-17 12:44:51.298382 ipfabric-6.3.1b2/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     6964 2023-07-13 12:33:49.979894 ipfabric-6.3.1b2/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    12421 2023-07-13 12:33:49.985397 ipfabric-6.3.1b2/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    25472 2023-07-17 15:20:24.297305 ipfabric-6.3.1b2/ipfabric/models/table.py
--rw-r--r--   0        0        0     2988 2023-07-17 15:01:32.974051 ipfabric-6.3.1b2/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.3.1b2/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.3.1b2/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.3.1b2/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.3.1b2/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.3.1b2/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.3.1b2/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.3.1b2/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.3.1b2/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.3.1b2/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.3.1b2/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.3.1b2/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1076 2023-07-17 12:44:51.298382 ipfabric-6.3.1b2/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     5549 2023-07-17 12:44:51.299382 ipfabric-6.3.1b2/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2158 2023-07-17 12:44:51.299382 ipfabric-6.3.1b2/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.3.1b2/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.3.1b2/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2094 2023-07-17 12:44:51.300385 ipfabric-6.3.1b2/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.3.1b2/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.3.1b2/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.3.1b2/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3342 2023-07-13 12:33:49.997188 ipfabric-6.3.1b2/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.3.1b2/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.3.1b2/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.3.1b2/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.3.1b2/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.3.1b2/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     5137 2023-07-13 12:33:50.002187 ipfabric-6.3.1b2/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.3.1b2/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.3.1b2/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.3.1b2/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.3.1b2/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.3.1b2/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125000 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125000 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/dashboard.json
--rw-r--r--   0        0        0     5852 2023-07-14 17:28:19.475539 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/groups.json
--rw-r--r--   0        0        0   122055 2023-07-14 17:21:35.755499 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.3.1b2/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     6141 2023-07-14 16:43:51.555959 ipfabric-6.3.1b2/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.3.1b2/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.3.1b2/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.3.1b2/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.3.1b2/LICENSE
--rw-r--r--   0        0        0     2020 2023-07-17 15:20:49.946414 ipfabric-6.3.1b2/pyproject.toml
--rw-r--r--   0        0        0     3951 2023-07-17 15:20:24.284079 ipfabric-6.3.1b2/README.md
--rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 ipfabric-6.3.1b2/setup.py
--rw-r--r--   0        0        0     5423 1970-01-01 00:00:00.000000 ipfabric-6.3.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-17 13:27:31.248851 ipfabric-6.3.2b0/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17429 2023-07-17 15:07:10.627331 ipfabric-6.3.2b0/ipfabric/api.py
+-rw-r--r--   0        0        0    11597 2023-07-17 13:27:31.249861 ipfabric-6.3.2b0/ipfabric/client.py
+-rw-r--r--   0        0        0      434 2023-07-17 13:27:21.289009 ipfabric-6.3.2b0/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    15080 2023-07-17 13:46:34.405047 ipfabric-6.3.2b0/ipfabric/models/device.py
+-rw-r--r--   0        0        0     5842 2023-07-17 13:27:21.290017 ipfabric-6.3.2b0/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2811 2023-07-17 14:07:09.268500 ipfabric-6.3.2b0/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2226 2023-07-17 13:34:01.704572 ipfabric-6.3.2b0/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     6971 2023-07-17 13:34:02.413182 ipfabric-6.3.2b0/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12533 2023-07-17 13:44:06.895048 ipfabric-6.3.2b0/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    25465 2023-07-17 15:13:21.542445 ipfabric-6.3.2b0/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2995 2023-07-17 15:14:05.898205 ipfabric-6.3.2b0/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-17 13:34:02.934785 ipfabric-6.3.2b0/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      495 2023-07-17 13:34:02.783756 ipfabric-6.3.2b0/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2180 2023-07-17 13:34:03.476365 ipfabric-6.3.2b0/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1009 2023-07-17 13:34:03.368850 ipfabric-6.3.2b0/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7025 2023-07-17 13:34:05.294652 ipfabric-6.3.2b0/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      331 2023-07-17 13:34:03.697396 ipfabric-6.3.2b0/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      850 2023-07-17 13:34:03.944945 ipfabric-6.3.2b0/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      477 2023-07-17 13:34:04.104459 ipfabric-6.3.2b0/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5651 2023-07-17 13:34:06.077775 ipfabric-6.3.2b0/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2052 2023-07-17 13:34:05.025112 ipfabric-6.3.2b0/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2790 2023-07-17 13:34:05.386169 ipfabric-6.3.2b0/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      766 2023-07-17 13:34:05.534200 ipfabric-6.3.2b0/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      640 2023-07-17 13:34:05.701713 ipfabric-6.3.2b0/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3536 2023-07-17 13:34:06.858899 ipfabric-6.3.2b0/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1238 2023-07-17 13:34:06.169289 ipfabric-6.3.2b0/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1083 2023-07-17 13:34:06.185288 ipfabric-6.3.2b0/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     5556 2023-07-17 13:34:07.919016 ipfabric-6.3.2b0/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2165 2023-07-17 13:34:07.104931 ipfabric-6.3.2b0/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      438 2023-07-17 13:34:06.569351 ipfabric-6.3.2b0/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2069 2023-07-17 13:34:07.141447 ipfabric-6.3.2b0/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2101 2023-07-17 13:34:07.568754 ipfabric-6.3.2b0/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      863 2023-07-17 13:34:07.409477 ipfabric-6.3.2b0/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      874 2023-07-17 13:34:07.466240 ipfabric-6.3.2b0/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-07-17 13:27:21.302869 ipfabric-6.3.2b0/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3356 2023-07-17 13:48:25.369402 ipfabric-6.3.2b0/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-07-17 13:27:21.303868 ipfabric-6.3.2b0/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8754 2023-07-17 13:34:10.302334 ipfabric-6.3.2b0/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2023-07-17 13:27:21.305868 ipfabric-6.3.2b0/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-07-17 13:27:21.305868 ipfabric-6.3.2b0/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-07-17 13:27:21.305868 ipfabric-6.3.2b0/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5155 2023-07-17 14:10:37.579326 ipfabric-6.3.2b0/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-07-17 13:27:21.306870 ipfabric-6.3.2b0/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6350 2023-07-17 13:34:13.481859 ipfabric-6.3.2b0/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      430 2023-07-17 13:27:21.308881 ipfabric-6.3.2b0/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7876 2023-07-17 13:27:21.308881 ipfabric-6.3.2b0/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-07-17 13:27:21.309887 ipfabric-6.3.2b0/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.310886 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.310886 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2023-07-17 13:27:21.311886 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2023-07-17 13:27:21.311886 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2023-07-17 13:27:21.312886 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.312886 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.313912 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2023-07-17 13:27:21.313912 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2023-07-17 13:27:21.314893 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2023-07-17 13:27:21.315888 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.315888 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.318355 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2023-07-17 13:27:21.318355 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2023-07-17 13:27:21.318355 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2023-07-17 13:27:21.319668 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:31.255244 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/__init__.py
+-rw-r--r--   0        0        0     3152 2023-07-17 13:27:31.256248 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/dashboard.json
+-rw-r--r--   0        0        0     5852 2023-07-17 13:27:31.256248 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/groups.json
+-rw-r--r--   0        0        0   122055 2023-07-17 13:27:31.278422 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/intents.json
+-rw-r--r--   0        0        0        0 2023-07-17 13:27:21.319668 ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4511 2023-07-17 13:27:21.320674 ipfabric-6.3.2b0/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     6141 2023-07-17 13:27:31.279424 ipfabric-6.3.2b0/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0     2519 2023-07-17 13:27:21.321674 ipfabric-6.3.2b0/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2396 2023-07-17 13:27:21.321674 ipfabric-6.3.2b0/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2594 2023-07-17 13:34:12.282004 ipfabric-6.3.2b0/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2023-07-17 13:27:21.263717 ipfabric-6.3.2b0/LICENSE
+-rw-r--r--   0        0        0     2049 2023-07-17 15:21:22.551934 ipfabric-6.3.2b0/pyproject.toml
+-rw-r--r--   0        0        0     3951 2023-07-17 13:27:31.247569 ipfabric-6.3.2b0/README.md
+-rw-r--r--   0        0        0     5594 1970-01-01 00:00:00.000000 ipfabric-6.3.2b0/setup.py
+-rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 ipfabric-6.3.2b0/PKG-INFO
```

### Comparing `ipfabric-6.3.1b2/ipfabric/__init__.py` & `ipfabric-6.3.2b0/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/api.py` & `ipfabric-6.3.2b0/ipfabric/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from typing import Optional, Union, Dict, List, Generator, Any
 from urllib.parse import urljoin
 from uuid import UUID
 
 import dotenv
 import httpx
 from httpx import Client, URL
-from pydantic import BaseSettings, validator
+from pydantic import field_validator
 
 from ipfabric.models import Snapshot, SNAPSHOT_COLUMNS
 from ipfabric.settings.user_mgmt import User
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 logger = logging.getLogger("ipfabric")
 
 LAST_ID, PREV_ID, LASTLOCKED_ID = "$last", "$prev", "$lastLocked"
 VALID_REFS = [LAST_ID, PREV_ID, LASTLOCKED_ID]
 
 
@@ -35,47 +36,46 @@
                 resp.raise_for_status()  # Response updates accessToken in shared CookieJar
                 request.headers["Cookie"] = "accessToken=" + self.client.cookies["accessToken"]  # Update request
                 yield request
         return response
 
 
 class Settings(BaseSettings):
-    ipf_url: Optional[str]
-    ipf_version: Optional[Union[int, float, str]]
-    ipf_token: Optional[str]
-    ipf_username: Optional[str]
-    ipf_password: Optional[str]
-    ipf_snapshot: Optional[str]
-    ipf_verify: Union[bool, str] = True
-    ipf_timeout: Optional[float] = None
+    model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8", env_prefix="ipf_")
+    url: Optional[str] = None
+    version: Optional[Union[int, float, str]] = None
+    token: Optional[str] = None
+    username: Optional[str] = None
+    password: Optional[str] = None
+    snapshot: Optional[str] = None
+    verify: Union[bool, str] = True
+    timeout: Optional[float] = None
 
-    @validator("ipf_version")
+    @field_validator("version")
+    @classmethod
     def _valid_version(cls, v):
         if v is None:
             return v
         if v and isinstance(v, (int, float)):
             v = "v" + str(v)
         if re.match(r"v\d(\.\d)?", v) or not v:
             return v
         else:
             raise ValueError(f"IPF_VERSION ({v}) is not valid, must be like `v#` or `v#.#`.")
 
-    @validator("ipf_snapshot")
+    @field_validator("snapshot")
+    @classmethod
     def _valid_snapshot(cls, v):
         if v is None or v in VALID_REFS:
             return v
         elif re.match(r"^[\da-f]{8}-([\da-f]{4}-){3}[\da-f]{12}$", v.lower()):
             return v.lower()
         else:
             raise ValueError(f"IPF_SNAPSHOT ({v}) is not valid, must be a UUID or one of {VALID_REFS}.")
 
-    class Config:
-        env_file = ".env"
-        env_file_encoding = "utf-8"
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Needed for context"""
         pass
 
@@ -104,35 +104,35 @@
             logger.warning(
                 "Use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` authentication will be deprecated "
                 "in v7.0.X, please use `auth='<TOKEN>'` or `auth=('<USER>','<PASS>')` instead.\n"
                 "This does not apply to .env file or environment variables (IPF_TOKEN, IPF_USERNAME, IPF_PASSWORD).\n"
                 "This is to support custom authentication methods that will be passed directly to HTTPX."
             )
         self.unloaded = unloaded
-        # find env file
-        dotenv.load_dotenv(dotenv.find_dotenv())
-        with Settings() as settings:
+        env_file = dotenv.find_dotenv()
+        logger.debug(f'Using .env file located at "{env_file}".')
+        with Settings(_env_file=env_file) as settings:
             cookie_jar = CookieJar()
             super().__init__(
                 cookies=cookie_jar,
-                **self._httpx_kwargs(kwargs, kwargs.get("verify", settings.ipf_verify), settings.ipf_timeout),
+                **self._httpx_kwargs(kwargs, kwargs.get("verify", settings.verify), settings.timeout),
             )
-            base_url = base_url or settings.ipf_url
+            base_url = base_url or settings.url
             if not base_url:
                 raise RuntimeError("IP Fabric base_url not provided or IPF_URL not set")
 
-            self.api_version, self.os_version = self.check_version(api_version or settings.ipf_version, base_url)
+            self.api_version, self.os_version = self.check_version(api_version or settings.version, base_url)
             self.base_url = urljoin(base_url, f"api/{self.api_version}/")
-            snapshot_id = snapshot_id or settings.ipf_snapshot
+            snapshot_id = snapshot_id or settings.snapshot
             if auth:
                 token, username, password = None, None, None
             else:
-                token = kwargs.get("token", settings.ipf_token)  # TODO: Update this in v7.0
-                username = kwargs.get("username", settings.ipf_username)
-                password = kwargs.get("password", settings.ipf_password)
+                token = kwargs.get("token", settings.token)  # TODO: Update this in v7.0
+                username = kwargs.get("username", settings.username)
+                password = kwargs.get("password", settings.password)
 
         if token:
             self._login(token)
         elif username and password:
             self._login((username, password), base_url=base_url, cookie_jar=cookie_jar)
         else:
             self._login(auth, base_url=base_url, cookie_jar=cookie_jar)  # TODO: Keep only this in v7.0
```

### Comparing `ipfabric-6.3.1b2/ipfabric/client.py` & `ipfabric-6.3.2b0/ipfabric/client.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/models/device.py` & `ipfabric-6.3.2b0/ipfabric/models/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,49 +17,49 @@
 
 
 logger = logging.getLogger("ipfabric")
 
 
 class DeviceConfig(BaseModel):
     status: str
-    current: Optional[str] = Field(alias="currentConfig")
-    start: Optional[str] = Field(alias="startupConfig")
+    current: Optional[str] = Field(alias="currentConfig", default=None)
+    start: Optional[str] = Field(alias="startupConfig", default=None)
 
 
 class Device(BaseModel):
     attributes: dict
-    domain: Optional[str]
-    family: Optional[str]
-    fqdn: Optional[str]
+    domain: Optional[str] = None
+    family: Optional[str] = None
+    fqdn: Optional[str] = None
     hostname: str
-    image: Optional[str]
-    model: Optional[str]
-    platform: Optional[str]
-    processor: Optional[str]
-    reload: Optional[str]
+    image: Optional[str] = None
+    model: Optional[str] = None
+    platform: Optional[str] = None
+    processor: Optional[str] = None
+    reload: Optional[str] = None
     sn: str
-    uptime: Optional[timedelta]
+    uptime: Optional[timedelta] = None
     vendor: str
     version: str
-    blob_key: Optional[str] = Field(alias="blobKey")
-    config_reg: Optional[str] = Field(alias="configReg")
+    blob_key: Optional[str] = Field(alias="blobKey", default=None)
+    config_reg: Optional[str] = Field(alias="configReg", default=None)
     dev_type: str = Field(alias="devType")
-    hostname_original: Optional[str] = Field(alias="hostnameOriginal")
-    hostname_processed: Optional[str] = Field(alias="hostnameProcessed")
-    login_ip: Optional[IPv4Interface] = Field(alias="loginIp")
+    hostname_original: Optional[str] = Field(alias="hostnameOriginal", default=None)
+    hostname_processed: Optional[str] = Field(alias="hostnameProcessed", default=None)
+    login_ip: Optional[IPv4Interface] = Field(alias="loginIp", default=None)
     login_type: str = Field(alias="loginType")
-    mem_total_bytes: Optional[float] = Field(alias="memoryTotalBytes")
-    mem_used_bytes: Optional[float] = Field(alias="memoryUsedBytes")
-    mem_utilization: Optional[float] = Field(alias="memoryUtilization")
-    object_id: Optional[str] = Field(alias="objectId")
-    routing_domain: Optional[int] = Field(alias="rd")
+    mem_total_bytes: Optional[float] = Field(alias="memoryTotalBytes", default=None)
+    mem_used_bytes: Optional[float] = Field(alias="memoryUsedBytes", default=None)
+    mem_utilization: Optional[float] = Field(alias="memoryUtilization", default=None)
+    object_id: Optional[str] = Field(alias="objectId", default=None)
+    routing_domain: Optional[int] = Field(alias="rd", default=None)
     site: str = Field(alias="siteName")
     sn_hw: str = Field(alias="snHw")
-    stp_domain: Optional[int] = Field(alias="stpDomain")
-    task_key: Optional[str] = Field(alias="taskKey")
+    stp_domain: Optional[int] = Field(alias="stpDomain", default=None)
+    task_key: Optional[str] = Field(alias="taskKey", default=None)
 
     def __repr__(self):
         return self.hostname
 
     def __str__(self):
         return self.hostname
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/intent.py` & `ipfabric-6.3.2b0/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/models/intent_check.py` & `ipfabric-6.3.2b0/ipfabric/models/intent_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
     nan: Union[int, str, dict] = Field(alias="-1", default=None)
 
 
 class Description(BaseModel):
     """model for description of intent check"""
 
-    general: Union[None, str]
+    general: Union[None, str] = None
     checks: Checks = Field(default_factory=Checks)
 
 
 class Result(BaseModel):
     """model for results of intent check"""
 
-    count: Union[int, None]
+    count: Union[int, None] = None
     checks: Checks = Field(default_factory=Checks)
 
     def compare(self, other: "Result") -> dict:
         """
 
         Args:
             other: intent check
@@ -87,11 +87,11 @@
     column: str
     custom: bool
     descriptions: Description
     name: str
     status: int
     result: Result
     api_endpoint: str = Field(alias="apiEndpoint")
-    default_color: Union[None, int] = Field(alias="defaultColor")
+    default_color: Optional[int] = Field(alias="defaultColor", default=None)
     web_endpoint: str = Field(alias="webEndpoint")
     intent_id: str = Field(alias="id")
     result_data: Optional[CheckResults] = Field(default_factory=CheckResults)
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/inventory.py` & `ipfabric-6.3.2b0/ipfabric/models/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 IGNORE_COLUMNS = {"id"}
 
 
 class Inventory(BaseModel):
     """model for inventories"""
 
-    client: Any
+    client: Any = None
 
     @property
     def sites(self):
         return Table(client=self.client, endpoint="tables/inventory/sites")
 
     @property
     def vendors(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/jobs.py` & `ipfabric-6.3.2b0/ipfabric/models/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .table import BaseTable
 
 logger = logging.getLogger("ipfabric")
 
 
 class Jobs(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def all_jobs(self):
         return BaseTable(client=self.client, endpoint="tables/jobs")
 
     @property
     def columns(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/snapshot.py` & `ipfabric-6.3.2b0/ipfabric/models/snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,42 +58,42 @@
 class Error(BaseModel):
     error_type: str = Field(alias="errorType")
     count: int
 
 
 class Snapshot(BaseModel):
     snapshot_id: str = Field(alias="id")
-    name: Optional[str]
-    note: Optional[str]
-    creator_username: Optional[str] = Field(alias="creatorUsername")
+    name: Optional[str] = None
+    note: Optional[str] = None
+    creator_username: Optional[str] = Field(alias="creatorUsername", default=None)
     total_dev_count: int = Field(alias="totalDevCount")
-    licensed_dev_count: Optional[int] = Field(alias="licensedDevCount")
+    licensed_dev_count: Optional[int] = Field(alias="licensedDevCount", default=None)
     user_count: int = Field(alias="userCount")
     interface_active_count: int = Field(alias="interfaceActiveCount")
     interface_count: int = Field(alias="interfaceCount")
     interface_edge_count: int = Field(alias="interfaceEdgeCount")
     device_added_count: int = Field(alias="deviceAddedCount")
     device_removed_count: int = Field(alias="deviceRemovedCount")
     status: str
     finish_status: str = Field(alias="finishStatus")
     loading: bool
     locked: bool
     from_archive: bool = Field(alias="fromArchive")
     start: datetime = Field(alias="tsStart")
-    end: Optional[datetime] = Field(alias="tsEnd")
-    change: Optional[datetime] = Field(alias="tsChange")
+    end: Optional[datetime] = Field(alias="tsEnd", default=None)
+    change: Optional[datetime] = Field(alias="tsChange", default=None)
     version: Optional[str] = None
-    initial_version: Optional[str] = Field(alias="initialVersion")
+    initial_version: Optional[str] = Field(alias="initialVersion", default=None)
     sites: List[str]
-    errors: Optional[List[Error]]
+    errors: Optional[List[Error]] = None
     loaded_size: int = Field(alias="loadedSize")
     unloaded_size: int = Field(alias="unloadedSize")
-    disabled_graph_cache: Optional[bool]
-    disabled_historical_data: Optional[bool]
-    disabled_intent_verification: Optional[bool]
+    disabled_graph_cache: Optional[bool] = None
+    disabled_historical_data: Optional[bool] = None
+    disabled_intent_verification: Optional[bool] = None
 
     def lock(self, ipf: IPFClient):
         if not self.locked and self.loaded:
             res = ipf.post(f"snapshots/{self.snapshot_id}/lock")
             res.raise_for_status()
             self.locked = True
         elif not self.loaded:
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/table.py` & `ipfabric-6.3.2b0/ipfabric/models/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 IGNORE_COLUMNS = {"id"}
 
 
 class BaseTable(BaseModel):
     """model for table data"""
 
     endpoint: str
-    client: Any
+    client: Any = None
 
     @property
     def name(self):
         return self.endpoint.split("/")[-1]
 
     @property
     def abs_endpoint(self):
@@ -245,15 +245,15 @@
             for col in table_columns:
                 # check if the data returned has nested columns
                 if isinstance(one_row_of_data[0][col], list):
                     logger.debug(f"Column: {col}, one row of data: {one_row_of_data}")
                     check_len_of_data = len(one_row_of_data[0][col])
                     if check_len_of_data >= 0:
                         logger.warning(
-                            "Nested Column was Detected, but no data was present to determine if there are any nested columns, skipping"
+                            "Nested Column was detected, but no data was present to verify nested columns, skipping."
                         )
                         continue
                     # get all the nested column names
                     nested_cols = set(one_row_of_data[0][col][0].keys())
                     # create a set of nested column names requested by the user
                     nested_cols_for_return = {col for col in nested_cols if col in nested_keys}
 
@@ -537,15 +537,15 @@
 
         return joined_data
 
 
 class DeviceTable(Table):
     """model for Device Table data"""
 
-    endpoint = "tables/inventory/devices"
+    endpoint: str = "tables/inventory/devices"
 
     def _as_model(self, devices, as_model):
         if not as_model:
             return devices
         try:
             attributes = Attributes(client=self.client, snapshot_id=self.client.snapshot_id).all()
         except HTTPStatusError:
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/__init__.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .security import Security
 from .stp import Stp
 from .vlans import Vlans
 from .wireless import Wireless
 
 
 class Technology(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def platforms(self):
         return Platforms(client=self.client)
 
     @property
     def interfaces(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/addressing.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/addressing.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Addressing(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def arp_table(self):
         return models.Table(client=self.client, endpoint="tables/addressing/arp")
 
     @property
     def mac_table(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/dhcp.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/dhcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Dhcp(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def relay_interfaces(self):
         return models.Table(client=self.client, endpoint="tables/dhcp/relay/interfaces")
 
     @property
     def relay_interfaces_stats_received(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/fhrp.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/fhrp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Fhrp(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def group_state(self):
         return models.Table(client=self.client, endpoint="tables/fhrp/group-state")
 
     @property
     def group_members(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/interfaces.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Interfaces(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def current_rates_data_inbound(self):
         return models.Table(client=self.client, endpoint="tables/interfaces/load/inbound")
 
     @property
     def current_rates_data_outbound(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/load_balancing.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class LoadBalancing(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def virtual_servers(self):
         return models.Table(client=self.client, endpoint="tables/load-balancing/virtual-servers")
 
     @property
     def virtual_servers_pools(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/management.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/management.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Management(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def aaa_servers(self):
         return models.Table(client=self.client, endpoint="tables/security/aaa/servers")
 
     @property
     def aaa_lines(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/mpls.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/mpls.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Mpls(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def ldp_neighbors(self):
         return models.Table(client=self.client, endpoint="tables/mpls/ldp/neighbors")
 
     @property
     def ldp_interfaces(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/multicast.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/multicast.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Multicast(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def pim_neighbors(self):
         return models.Table(client=self.client, endpoint="tables/multicast/pim/neighbors")
 
     @property
     def pim_interfaces(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/neighbors.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/neighbors.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Neighbors(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def neighbors_all(self):
         return models.Table(client=self.client, endpoint="tables/neighbors/all")
 
     @property
     def neighbors_unmanaged(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/oam.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/oam.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Oam(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def unidirectional_link_detection_neighbors(self):
         return models.Table(
             client=self.client, endpoint="tables/management/oam/unidirectional-link-detection/neighbors"
         )
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/platforms.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/platforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Platforms(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def environment_power_supplies(self):
         return models.Table(client=self.client, endpoint="tables/inventory/power-supplies")
 
     @property
     def environment_power_supplies_fans(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/port_channels.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/port_channels.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class PortChannels(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def inbound_balancing_table(self):
         return models.Table(client=self.client, endpoint="tables/interfaces/port-channel/balance/inbound")
 
     @property
     def outbound_balancing_table(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/qos.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/qos.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Qos(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def policy_maps(self):
         return models.Table(client=self.client, endpoint="tables/qos/policy-maps")
 
     @property
     def shaping(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/routing.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Routing(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def summary_protocols(self):
         return models.Table(client=self.client, endpoint="tables/networks/summary/protocols")
 
     @property
     def summary_protocols_bgp(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/sdn.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/sdn.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Sdn(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def aci_endpoints(self):
         return models.Table(client=self.client, endpoint="tables/aci/endpoints")
 
     @property
     def aci_vlan(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/security.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Security(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def acl(self):
         return models.Table(client=self.client, endpoint="tables/security/acl")
 
     @property
     def acl_interface(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/stp.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/stp.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Stp(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def bridges(self):
         return models.Table(client=self.client, endpoint="tables/spanning-tree/bridges")
 
     @property
     def instances(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/vlans.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/vlans.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Vlans(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def device_summary(self):
         return models.Table(client=self.client, endpoint="tables/vlan/device-summary")
 
     @property
     def device_detail(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/wireless.py` & `ipfabric-6.3.2b0/ipfabric/models/technology/wireless.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Wireless(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def controllers(self):
         return models.Table(client=self.client, endpoint="tables/wireless/controllers")
 
     @property
     def access_points(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/__init__.py` & `ipfabric-6.3.2b0/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/api_tokens.py` & `ipfabric-6.3.2b0/ipfabric/settings/api_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     username: str
     expires: Optional[int] = None
     token: Optional[str] = None
     user_id: str = Field(alias="userId")
     user_role_ids: Optional[List[str]] = Field(alias="userRoleIds", default=None)
     token_id: str = Field(alias="id")
     is_expired: bool = Field(alias="isExpired")
-    last_used: Optional[str] = Field(alias="lastUsed")
+    last_used: Optional[str] = Field(alias="lastUsed", default=None)
     role_ids: List[str] = Field(alias="roleIds")
     role_names: Optional[List[str]] = Field(alias="roleNames", default=None)
 
 
 class APIToken:
     def __init__(self, client):
         self.client: Any = client
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/attributes.py` & `ipfabric-6.3.2b0/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/authentication.py` & `ipfabric-6.3.2b0/ipfabric/settings/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 from pydantic.dataclasses import dataclass
 
 logger = logging.getLogger("ipfabric")
 
 
 class Expiration(BaseModel):
     enabled: bool
-    value: Optional[datetime]
+    value: Optional[datetime] = None
 
 
 class Credential(BaseModel):
     network: list
     excluded: list = Field(alias="excludeNetworks")
     expiration: Expiration = Field(alias="expirationDate")
     credential_id: str = Field(alias="id")
     encrypt_password: str = Field(alias="password")
-    priority: Optional[int]
+    priority: Optional[int] = None
     username: str
     config_mgmt: bool = Field(alias="syslog")
-    notes: Optional[str]
+    notes: Optional[str] = None
 
 
 class Privilege(BaseModel):
     network: list = Field(alias="includeNetworks")
     excluded: list = Field(alias="excludeNetworks")
     expiration: Expiration = Field(alias="expirationDate")
     privilege_id: str = Field(alias="id")
     encrypt_password: str = Field(alias="password")
-    priority: Optional[int]
+    priority: Optional[int] = None
     username: str
-    notes: Optional[str]
+    notes: Optional[str] = None
 
 
 @dataclass
 class Authentication:
     client: Any
     credentials: dict = Field(default=dict())
     enables: dict = Field(default=dict())
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/discovery.py` & `ipfabric-6.3.2b0/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/seeds.py` & `ipfabric-6.3.2b0/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/site_separation.py` & `ipfabric-6.3.2b0/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/user_mgmt.py` & `ipfabric-6.3.2b0/ipfabric/settings/user_mgmt.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,31 @@
 from pydantic import Field, BaseModel
 
 logger = logging.getLogger("ipfabric")
 
 
 class Token(BaseModel):
     token_id: str = Field(alias="id")
-    description: Optional[str]
+    description: Optional[str] = None
     role_ids: list = Field(alias="roleIds")
 
 
 class User(BaseModel):
     username: str
     user_id: str = Field(alias="id")
-    local: Optional[bool] = Field(alias="isLocal")
-    sso_provider: Optional[Any] = Field(alias="ssoProvider")
-    domains: Optional[Any] = Field(alias="domainSuffixes")
+    local: Optional[bool] = Field(alias="isLocal", default=None)
+    sso_provider: Optional[Any] = Field(alias="ssoProvider", default=None)
+    domains: Optional[Any] = Field(alias="domainSuffixes", default=None)
     role_names: Optional[list] = Field(alias="roleNames", default_factory=list)
     role_ids: list = Field(alias="roleIds")
-    ldap_id: Optional[Any] = Field(alias="ldapId")
-    timezone: Optional[str]
-    token: Optional[Token]
+    ldap_id: Optional[Any] = Field(alias="ldapId", default=None)
+    timezone: Optional[str] = None
+    token: Optional[Token] = None
     _get_snapshots_settings: Optional[bool] = None
 
-    class Config:
-        underscore_attrs_are_private = True
-
     @property
     def is_admin(self):
         return (
             True
             if (self.token and "admin" in self.token.role_ids) or (not self.token and "admin" in self.role_ids)
             else False
         )
@@ -54,15 +51,15 @@
             msg += f'Token "{self.token.description}" '
         return msg
 
 
 class Role(BaseModel):
     role_id: str = Field(alias="id")
     name: str
-    description: Optional[str]
+    description: Optional[str] = None
     role_type: str = Field(alias="type")
     admin: bool = Field(alias="isAdmin")
     system: bool = Field(alias="isSystem")
 
 
 class UserMgmt:
     def __init__(self, client):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/vendor_api.py` & `ipfabric-6.3.2b0/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.3.2b0/ipfabric/settings/vendor_api_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from typing import Optional, List, Union
+from typing import Literal, Optional, List, Union
 
-from pydantic import BaseModel, Field, validator, AnyHttpUrl
+from pydantic import field_validator, BaseModel, Field, AnyHttpUrl
 
 AWS_REGIONS = [
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -42,15 +42,16 @@
     base Vendor API config
     """
 
     slug: str
     comment: str = ""
     isEnabled: bool = True
 
-    @validator("slug")
+    @field_validator("slug")
+    @classmethod
     def check_slug(cls, slug):
         if not re.match(SLUG, slug):
             raise ValueError(f"{slug} is not a valid slug and must match regex {SLUG}")
         return slug
 
 
 class SystemProxy(BaseModel):
@@ -88,24 +89,26 @@
     AWS vendor api support
     """
 
     apiKey: str
     apiSecret: str
     regions: list
     assumeRoles: Optional[List[Union[str, dict, AssumeRole]]] = Field(default=None)
-    type: str = Field(default="aws-ec2", const=True)
+    type: Literal["aws-ec2"] = "aws-ec2"
 
-    @validator("regions")
+    @field_validator("regions")
+    @classmethod
     def check_region(cls, regions):
         for r in regions:
             if r.lower() not in AWS_REGIONS:
                 raise ValueError(f"{r} is not a valid AWS Region")
         return [r.lower() for r in regions]
 
-    @validator("assumeRoles")
+    @field_validator("assumeRoles")
+    @classmethod
     def check_roles(cls, roles):
         validated_roles = list()
         for role in roles:
             if isinstance(role, str):
                 validated_roles.append(AssumeRole(role=role))
             elif isinstance(role, dict):
                 if "role" in role:
@@ -122,136 +125,137 @@
     Azure vendor api support
     """
 
     clientId: str
     clientSecret: str
     subscriptionId: str
     tenantId: str
-    type: str = Field(default="azure", const=True)
+    type: Literal["azure"] = "azure"
 
 
 class CheckPointApiKey(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Checkpoint vendor api support
     """
 
     apiKey: str
     baseUrl: AnyHttpUrl
     domains: Optional[List[str]] = Field(default_factory=list)
-    type: str = Field(default="checkpoint-mgmt-api", const=True)
+    type: Literal["checkpoint-mgmt-api"] = "checkpoint-mgmt-api"
 
 
 class CheckPointUserAuth(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     checkpoint authentication vendor api support
     """
 
     domains: Optional[List[str]] = Field(default_factory=list)
-    type: str = Field(default="checkpoint-mgmt-api", const=True)
+    type: Literal["checkpoint-mgmt-api"] = "checkpoint-mgmt-api"
 
 
 class CiscoAPIC(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Cisco APIC vendor api support
     """
 
-    type: str = Field(default="ciscoapic", const=True)
+    type: Literal["ciscoapic"] = "ciscoapic"
 
 
 class CiscoFMC(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Cisco FMC vendor api support
     """
 
-    type: str = Field(default="ciscofmc", const=True)
+    type: Literal["ciscofmc"] = "ciscofmc"
 
 
 class ForcePoint(VendorAPI, RejectUnauthorized, BaseModel):
     """
     ForcePoint vendor api support
     """
 
     authenticationKey: str
     baseUrl: AnyHttpUrl
-    type: str = Field(default="forcepoint", const=True)
+    type: Literal["forcepoint"] = "forcepoint"
 
 
 class JuniperMist(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Juniper Mist vendor api support
     """
 
     apiToken: str
-    apiVer: str = Field(default="v1", const=True)
-    type: str = Field(default="juniper-mist", const=True)
+    apiVer: Literal["v1"] = "v1"
+    type: Literal["juniper-mist"] = "juniper-mist"
     baseUrl: AnyHttpUrl = "https://api.mist.com"
 
 
 class Merakiv1(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Meraki v1 vendor api support
     """
 
     apiKey: str
     baseUrl: AnyHttpUrl
     organizations: Optional[List[str]] = Field(default_factory=list)
-    apiVer: str = Field(default="v1", const=True)
-    type: str = Field(default="meraki-v0", const=True)
+    apiVer: Literal["v1"] = "v1"
+    type: Literal["meraki-v0"] = "meraki-v0"
 
 
 class NSXT(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     NSXT vendor api support
     """
 
-    type: str = Field(default="nsxT", const=True)
+    type: Literal["nsxT"] = "nsxT"
 
 
 class Prisma(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Prisma vendor api support
     """
 
     username: str
     password: str
     tsgid: str
-    type: str = Field(default="prisma", const=True)
+    type: Literal["prisma"] = "prisma"
 
 
 class RuckusVirtualSmartZone(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Ruckus Virtual SmartZone vendor api support
     """
 
-    apiVer: str = Field(default="v9_1", const=True)
-    type: str = Field(default="ruckus-vsz", const=True)
+    apiVer: Literal["v9_1"] = "v9_1"
+    type: Literal["ruckus-vsz"] = "ruckus-vsz"
 
 
 class SilverPeak(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     SilverPeak vendor api support
     """
 
     loginType: str = "Local"
-    type: str = Field(default="nsxT", const=True)
+    type: Literal["nsxT"] = "nsxT"
 
-    @validator("loginType")
+    @field_validator("loginType")
+    @classmethod
     def check_region(cls, login_type):
         if login_type not in ["Local", "RADIUS", "TACACS+"]:
             raise ValueError(f"{login_type} is not a valid login type must be in ['Local', 'RADIUS', 'TACACS+']")
         return login_type
 
 
 class Versa(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Versa vendor api support
     """
 
-    type: str = Field(default="versa", const=True)
+    type: Literal["versa"] = "versa"
 
 
 class Viptela(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Viptela vendor api support
     """
 
-    type: str = Field(default="viptela", const=True)
+    type: Literal["viptela"] = "viptela"
```

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/configuration.py` & `ipfabric-6.3.2b0/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/discovery_history.py` & `ipfabric-6.3.2b0/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/dashboard.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/groups.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/intents.json` & `ipfabric-6.3.2b0/ipfabric/tools/factory_defaults/v6/3/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/nist.py` & `ipfabric-6.3.2b0/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/restore_intents.py` & `ipfabric-6.3.2b0/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/shared.py` & `ipfabric-6.3.2b0/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.3.2b0/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.3.2b0/ipfabric/tools/vulnerabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from pydantic import BaseModel
 
 from ipfabric.tools.nist import NIST, CVEs
 
 
 class Version(BaseModel):
     vendor: str
-    family: Optional[str]
+    family: Optional[str] = None
     version: str
     cves: CVEs
-    hostname: Optional[str]
-    site: Optional[str]
+    hostname: Optional[str] = None
+    site: Optional[str] = None
 
 
 class Vulnerabilities:
     def __init__(self, ipf, nvd_api_key: str, timeout: int = 30):
         self.ipf = ipf
         self.nist = NIST(nvd_api_key=nvd_api_key, timeout=timeout)
```

### Comparing `ipfabric-6.3.1b2/LICENSE` & `ipfabric-6.3.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/pyproject.toml` & `ipfabric-6.3.2b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.3.1b2"
+version = "v6.3.2b0"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
@@ -17,25 +17,26 @@
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/python-ipfabric/-/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.1"
 python-dateutil = "^2.8.2"
-pydantic = "^1.10.4"
+pydantic = "^2.0.3"
 pytz = "^2023.3"
 python-dotenv = "^1.0"
 pandas = {version = "^2.0", optional = true}
 openpyxl = {version = "^3.0.9", optional = true}
 tabulate = {version = ">=0.8.9,<0.10.0",  optional = true}
 python-json-logger = {version = "^2.0.4",  optional = true}
 macaddress = "~2.0.2"
 pyyaml = {version = "^6.0", optional = true}
 deepdiff = "^6.3.1"
 case-insensitive-dictionary = "^0.2.1"
+pydantic-settings = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 flake8 = "^5.0"
 black = "^22.12"
```

### Comparing `ipfabric-6.3.1b2/README.md` & `ipfabric-6.3.2b0/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/setup.py` & `ipfabric-6.3.2b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 {'': ['*']}
 
 install_requires = \
 ['case-insensitive-dictionary>=0.2.1,<0.3.0',
  'deepdiff>=6.3.1,<7.0.0',
  'httpx>=0.24.1,<0.25.0',
  'macaddress>=2.0.2,<2.1.0',
- 'pydantic>=1.10.4,<2.0.0',
+ 'pydantic-settings>=2.0.2,<3.0.0',
+ 'pydantic>=2.0.3,<3.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-dotenv>=1.0,<2.0',
  'pytz>=2023.3,<2024.0']
 
 extras_require = \
 {'examples': ['pandas>=2.0,<3.0',
               'openpyxl>=3.0.9,<4.0.0',
               'tabulate>=0.8.9,<0.10.0',
               'python-json-logger>=2.0.4,<3.0.0',
               'pyyaml>=6.0,<7.0']}
 
 setup_kwargs = {
     'name': 'ipfabric',
-    'version': '6.3.1b2',
+    'version': '6.3.2b0',
     'description': 'Python package for interacting with IP Fabric',
     'long_description': '# IP Fabric \n\nIPFabric is a Python module for connecting to and communicating against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation. \n\n## v6.3.1 Deprecation Notices\n\nIn `ipfabric>=v6.3.1` Python 3.7 support was removed.  This was originally \nplanned for `v7.0.0` however to add new functionality of Pandas Dataframe we \nare required to move this forward.\n\n**Python 3.7 is now End of Life as of June 27th 2023**\n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- The use of `token=\'<TOKEN>\'` or `username=\'<USER>\', password=\'<PASS>\'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth=\'TOKEN\')`\n  - User/Pass: `IPFClient(auth=(\'USER\', \'PASS\'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API\'s are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK\'s match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric\n```\n\n## Introduction\n\nPlease take a look at [API Programmability - Part 1: The Basics](https://ipfabric.io/blog/api-programmability-part-1/)\nfor instructions on creating an API token.\n\nMost of the methods and features can be located in [Examples](examples) to show how to use this package. \nAnother great introduction to this package can be found at [API Programmability - Part 2: Python](https://ipfabric.io/blog/api-programmability-python/)\n\n## Diagrams\n\nDiagramming in IP Fabric version v4.3 and above has been moved to it\'s own package.\n\nDiagramming will move back to this project in v7.0\n\n```\npip install ipfabric-diagrams\n```\n\n## Authentication\n### Username/Password\nSupply in client:\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=(\'user\', \'pass\'))\n```\n\n### Token\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=\'token\')\n```\n\n### Environment \nThe easiest way to use this package is with a `.env` file.  You can copy the sample and edit it with your environment variables. \n\n```commandline\ncp sample.env .env\n```\n\nThis contains the following variables which can also be set as environment variables instead of a .env file.\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_TOKEN=TOKEN\nIPF_VERIFY=true\n```\n\nOr if using Username/Password:\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_USERNAME=USER\nIPF_PASSWORD=PASS\n```\n\n## Development\n\n### Poetry Installation\n\nIPFabric uses [Poetry](https://pypi.org/project/poetry/) to make setting up a virtual environment with all dependencies\ninstalled quick and easy.\n\nInstall poetry globally:\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo run examples, install extras:\n```\npoetry install ipfabric -E examples\n```\n\n### Test and Build\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric\npoetry update\n```\n',
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric',
```

### Comparing `ipfabric-6.3.1b2/PKG-INFO` & `ipfabric-6.3.2b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.3.1b2
+Version: 6.3.2b0
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,16 @@
 Provides-Extra: examples
 Requires-Dist: case-insensitive-dictionary (>=0.2.1,<0.3.0)
 Requires-Dist: deepdiff (>=6.3.1,<7.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: macaddress (>=2.0.2,<2.1.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0) ; extra == "examples"
 Requires-Dist: pandas (>=2.0,<3.0) ; extra == "examples"
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0) ; extra == "examples"
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "examples"
 Requires-Dist: tabulate (>=0.8.9,<0.10.0) ; extra == "examples"
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/python-ipfabric/-/blob/develop/CHANGELOG.md
```

