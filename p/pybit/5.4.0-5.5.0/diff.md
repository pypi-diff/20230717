# Comparing `tmp/pybit-5.4.0.tar.gz` & `tmp/pybit-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybit-5.4.0.tar", last modified: Fri Jun 23 18:15:59 2023, max compression
+gzip compressed data, was "pybit-5.5.0.tar", last modified: Mon Jul 17 18:47:44 2023, max compression
```

## Comparing `pybit-5.4.0.tar` & `pybit-5.5.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-06-23 18:15:59.622222 pybit-5.4.0/
--rw-r--r--   0 uk09002ml   (502) staff       (20)    22081 2023-06-23 18:15:38.000000 pybit-5.4.0/CHANGELOG.md
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.4.0/LICENSE
--rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.4.0/MANIFEST.in
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-06-23 18:15:59.622679 pybit-5.4.0/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6585 2023-05-19 19:10:45.000000 pybit-5.4.0/README.md
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-06-23 18:15:59.575025 pybit-5.4.0/examples/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.4.0/examples/.DS_Store
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.4.0/examples/direct_session.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1605 2023-04-26 18:06:01.000000 pybit-5.4.0/examples/http_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-04-06 11:15:33.000000 pybit-5.4.0/examples/http_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.4.0/examples/websocket_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-04-18 18:56:31.000000 pybit-5.4.0/examples/websocket_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.4.0/examples/wrapper_class.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-06-23 18:15:59.605435 pybit-5.4.0/pybit/
--rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    13117 2023-05-19 19:00:49.000000 pybit-5.4.0/pybit/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7471 2023-04-26 18:06:01.000000 pybit-5.4.0/pybit/_v5_account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    14814 2023-04-26 18:06:01.000000 pybit-5.4.0/pybit/_v5_asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      530 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/_v5_broker.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8532 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/_v5_market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/_v5_misc.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/_v5_position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     4204 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/_v5_pre_upgrade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/_v5_spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6176 2023-04-18 16:12:52.000000 pybit-5.4.0/pybit/_v5_spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-26 18:06:01.000000 pybit-5.4.0/pybit/_v5_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6835 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/_v5_user.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    15265 2023-05-19 19:00:49.000000 pybit-5.4.0/pybit/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-26 18:06:01.000000 pybit-5.4.0/pybit/asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      160 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/broker.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1773 2023-05-19 19:00:49.000000 pybit-5.4.0/pybit/exceptions.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-06-23 18:15:59.621167 pybit-5.4.0/pybit/legacy/
--rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.4.0/pybit/legacy/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    32393 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/copy_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/exceptions.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/usdc_options.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/legacy/usdc_perpetual.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      856 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      153 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/misc.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      571 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/pre_upgrade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      932 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.4.0/pybit/trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     9049 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/unified_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      672 2023-06-23 18:15:38.000000 pybit-5.4.0/pybit/user.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-06-23 18:15:59.612891 pybit-5.4.0/pybit.egg-info/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-06-23 18:15:59.000000 pybit-5.4.0/pybit.egg-info/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1270 2023-06-23 18:15:59.000000 pybit-5.4.0/pybit.egg-info/SOURCES.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-06-23 18:15:59.000000 pybit-5.4.0/pybit.egg-info/dependency_links.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.4.0/pybit.egg-info/not-zip-safe
--rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2023-06-23 18:15:59.000000 pybit-5.4.0/pybit.egg-info/requires.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-06-23 18:15:59.000000 pybit-5.4.0/pybit.egg-info/top_level.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-06-23 18:15:59.624120 pybit-5.4.0/setup.cfg
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1085 2023-06-23 18:15:38.000000 pybit-5.4.0/setup.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-07-17 18:47:44.835940 pybit-5.5.0/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    22462 2023-07-17 18:47:13.000000 pybit-5.5.0/CHANGELOG.md
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.5.0/LICENSE
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.5.0/MANIFEST.in
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-07-17 18:47:44.837137 pybit-5.5.0/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6585 2023-05-19 19:10:45.000000 pybit-5.5.0/README.md
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-07-17 18:47:44.677653 pybit-5.5.0/examples/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.5.0/examples/.DS_Store
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.5.0/examples/direct_session.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1605 2023-04-26 18:06:01.000000 pybit-5.5.0/examples/http_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-04-06 11:15:33.000000 pybit-5.5.0/examples/http_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.5.0/examples/websocket_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-04-18 18:56:31.000000 pybit-5.5.0/examples/websocket_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.5.0/examples/wrapper_class.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-07-17 18:47:44.775781 pybit-5.5.0/pybit/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-07-17 18:45:37.000000 pybit-5.5.0/pybit/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    13117 2023-05-19 19:00:49.000000 pybit-5.5.0/pybit/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     7471 2023-04-26 18:06:01.000000 pybit-5.5.0/pybit/_v5_account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14814 2023-04-26 18:06:01.000000 pybit-5.5.0/pybit/_v5_asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      530 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/_v5_broker.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8532 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/_v5_market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-07-12 14:20:33.000000 pybit-5.5.0/pybit/_v5_misc.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/_v5_position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     4204 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/_v5_pre_upgrade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/_v5_spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6176 2023-04-18 16:12:52.000000 pybit-5.5.0/pybit/_v5_spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-26 18:06:01.000000 pybit-5.5.0/pybit/_v5_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6835 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/_v5_user.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    15265 2023-05-19 19:00:49.000000 pybit-5.5.0/pybit/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-26 18:06:01.000000 pybit-5.5.0/pybit/asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      160 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/broker.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1773 2023-05-19 19:00:49.000000 pybit-5.5.0/pybit/exceptions.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1331 2023-07-17 18:38:25.000000 pybit-5.5.0/pybit/helpers.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-07-17 18:47:44.829227 pybit-5.5.0/pybit/legacy/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.5.0/pybit/legacy/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    32393 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/copy_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/exceptions.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/usdc_options.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/legacy/usdc_perpetual.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      856 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      153 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/misc.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      571 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/pre_upgrade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      932 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.5.0/pybit/trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9049 2023-07-17 17:42:01.000000 pybit-5.5.0/pybit/unified_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      672 2023-06-23 18:15:38.000000 pybit-5.5.0/pybit/user.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-07-17 18:47:44.795242 pybit-5.5.0/pybit.egg-info/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-07-17 18:47:44.000000 pybit-5.5.0/pybit.egg-info/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1287 2023-07-17 18:47:44.000000 pybit-5.5.0/pybit.egg-info/SOURCES.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-07-17 18:47:44.000000 pybit-5.5.0/pybit.egg-info/dependency_links.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.5.0/pybit.egg-info/not-zip-safe
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2023-07-17 18:47:44.000000 pybit-5.5.0/pybit.egg-info/requires.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-07-17 18:47:44.000000 pybit-5.5.0/pybit.egg-info/top_level.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-07-17 18:47:44.842898 pybit-5.5.0/setup.cfg
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1085 2023-07-17 18:45:37.000000 pybit-5.5.0/setup.py
```

### Comparing `pybit-5.4.0/CHANGELOG.md` & `pybit-5.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [5.5.0] - 2023-07-17
+### Added
+- `helpers.py` which includes the `Helpers` class and the `close_position` method, which can be imported and employed like so:
+```python
+from pybit.helpers import Helpers
+my_helper = Helpers(session)  # your HTTP session object (eg, from pybit.unified_trading import HTTP)
+print(my_helper.close_position(category="linear", symbol="BTCUSDT"))
+```
+
 ## [5.4.0] - 2023-06-23
 ### Added
 - The following new endpoints to `unified_trading`:
   - `get_broker_earnings`
   - `get_announcement`
   - `get_pre_upgrade_order_history`
   - `get_pre_upgrade_trade_history`
```

### Comparing `pybit-5.4.0/LICENSE` & `pybit-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/PKG-INFO` & `pybit-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.4.0
+Version: 5.5.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
```

### Comparing `pybit-5.4.0/README.md` & `pybit-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/examples/.DS_Store` & `pybit-5.5.0/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/examples/direct_session.py` & `pybit-5.5.0/examples/direct_session.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/examples/http_example_explanatory.py` & `pybit-5.5.0/examples/http_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/examples/websocket_example_explanatory.py` & `pybit-5.5.0/examples/websocket_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/examples/wrapper_class.py` & `pybit-5.5.0/examples/wrapper_class.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_helpers.py` & `pybit-5.5.0/pybit/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_http_manager.py` & `pybit-5.5.0/pybit/_http_manager.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_account.py` & `pybit-5.5.0/pybit/_v5_account.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_asset.py` & `pybit-5.5.0/pybit/_v5_asset.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_broker.py` & `pybit-5.5.0/pybit/_v5_broker.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_market.py` & `pybit-5.5.0/pybit/_v5_market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_misc.py` & `pybit-5.5.0/pybit/_v5_misc.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_position.py` & `pybit-5.5.0/pybit/_v5_position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_pre_upgrade.py` & `pybit-5.5.0/pybit/_v5_pre_upgrade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_spot_leverage_token.py` & `pybit-5.5.0/pybit/_v5_spot_leverage_token.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_spot_margin_trade.py` & `pybit-5.5.0/pybit/_v5_spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_trade.py` & `pybit-5.5.0/pybit/_v5_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_v5_user.py` & `pybit-5.5.0/pybit/_v5_user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/_websocket_stream.py` & `pybit-5.5.0/pybit/_websocket_stream.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/account.py` & `pybit-5.5.0/pybit/account.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/asset.py` & `pybit-5.5.0/pybit/asset.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/exceptions.py` & `pybit-5.5.0/pybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/_helpers.py` & `pybit-5.5.0/pybit/legacy/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/_http_manager.py` & `pybit-5.5.0/pybit/legacy/_http_manager.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/_websocket_stream.py` & `pybit-5.5.0/pybit/legacy/_websocket_stream.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/copy_trading.py` & `pybit-5.5.0/pybit/legacy/copy_trading.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/exceptions.py` & `pybit-5.5.0/pybit/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/usdc_options.py` & `pybit-5.5.0/pybit/legacy/usdc_options.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/legacy/usdc_perpetual.py` & `pybit-5.5.0/pybit/legacy/usdc_perpetual.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/market.py` & `pybit-5.5.0/pybit/market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/position.py` & `pybit-5.5.0/pybit/position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/pre_upgrade.py` & `pybit-5.5.0/pybit/pre_upgrade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/spot_margin_trade.py` & `pybit-5.5.0/pybit/spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/trade.py` & `pybit-5.5.0/pybit/trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/unified_trading.py` & `pybit-5.5.0/pybit/unified_trading.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit/user.py` & `pybit-5.5.0/pybit/user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.4.0/pybit.egg-info/PKG-INFO` & `pybit-5.5.0/pybit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.4.0
+Version: 5.5.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
```

### Comparing `pybit-5.4.0/pybit.egg-info/SOURCES.txt` & `pybit-5.5.0/pybit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 pybit/_v5_trade.py
 pybit/_v5_user.py
 pybit/_websocket_stream.py
 pybit/account.py
 pybit/asset.py
 pybit/broker.py
 pybit/exceptions.py
+pybit/helpers.py
 pybit/market.py
 pybit/misc.py
 pybit/position.py
 pybit/pre_upgrade.py
 pybit/spot_leverage_token.py
 pybit/spot_margin_trade.py
 pybit/trade.py
```

### Comparing `pybit-5.4.0/setup.py` & `pybit-5.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pybit',
-    version='5.4.0',
+    version='5.5.0',
     description='Python3 Bybit HTTP/WebSocket API Connector', 
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bybit-exchange/pybit",
     license="MIT License",
     author="Dexter Dickinson",
     author_email="dexter.dickinson@bybit.com",
```

