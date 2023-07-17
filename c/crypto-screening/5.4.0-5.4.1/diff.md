# Comparing `tmp/crypto-screening-5.4.0.tar.gz` & `tmp/crypto-screening-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.4.0.tar", last modified: Sun Jul 16 14:37:11 2023, max compression
+gzip compressed data, was "crypto-screening-5.4.1.tar", last modified: Mon Jul 17 09:52:30 2023, max compression
```

## Comparing `crypto-screening-5.4.0.tar` & `crypto-screening-5.4.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.518366 crypto-screening-5.4.0/
--rw-rw-rw-   0        0        0       98 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-16 14:37:11.518366 crypto-screening-5.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.4.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.4.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.478190 crypto-screening-5.4.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.500100 crypto-screening-5.4.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.4.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.4.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.502632 crypto-screening-5.4.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.4.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19492 2023-07-16 14:27:18.000000 crypto-screening-5.4.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17311 2023-07-16 14:27:22.000000 crypto-screening-5.4.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12472 2023-07-16 14:27:27.000000 crypto-screening-5.4.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.506686 crypto-screening-5.4.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.4.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    21649 2023-07-16 13:58:33.000000 crypto-screening-5.4.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    12927 2023-07-16 14:36:33.000000 crypto-screening-5.4.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    20738 2023-07-16 13:59:10.000000 crypto-screening-5.4.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15035 2023-07-16 14:27:32.000000 crypto-screening-5.4.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.4.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.4.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.4.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.4.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.4.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.507190 crypto-screening-5.4.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.4.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.510226 crypto-screening-5.4.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.4.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.4.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.4.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.4.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.517361 crypto-screening-5.4.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-16 14:17:05.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36682 2023-07-16 13:04:17.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-16 14:16:54.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18061 2023-07-16 14:05:40.000000 crypto-screening-5.4.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.4.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.4.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.4.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.4.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:37:11.496574 crypto-screening-5.4.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1673 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-16 14:37:11.000000 crypto-screening-5.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 14:37:11.518366 crypto-screening-5.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-16 14:37:02.000000 crypto-screening-5.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.794229 crypto-screening-5.4.1/
+-rw-rw-rw-   0        0        0       98 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-17 09:52:30.793227 crypto-screening-5.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.4.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.4.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.666414 crypto-screening-5.4.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.697441 crypto-screening-5.4.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.4.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.4.1/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.705442 crypto-screening-5.4.1/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.4.1/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19456 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12436 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.708467 crypto-screening-5.4.1/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24779 2023-07-17 09:51:27.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    14885 2023-07-17 09:42:15.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21766 2023-07-17 09:50:45.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    14999 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16697 2023-07-17 09:46:37.000000 crypto-screening-5.4.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.4.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.4.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.4.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.4.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.719441 crypto-screening-5.4.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.4.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.739472 crypto-screening-5.4.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.792257 crypto-screening-5.4.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-16 14:17:05.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36682 2023-07-16 13:04:17.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-16 14:16:54.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18061 2023-07-16 14:05:40.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.4.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.4.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.4.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4233 2023-07-17 08:56:51.000000 crypto-screening-5.4.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.680874 crypto-screening-5.4.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.4.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:52:30.794229 crypto-screening-5.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-17 09:52:28.000000 crypto-screening-5.4.1/setup.py
```

### Comparing `crypto-screening-5.4.0/PKG-INFO` & `crypto-screening-5.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.4.0
+Version: 5.4.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.4.0/README.md` & `crypto-screening-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/build.py` & `crypto-screening-5.4.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/assets.py` & `crypto-screening-5.4.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/exchanges.py` & `crypto-screening-5.4.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, OHLCV_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
-    assets_to_symbol_market_prices, assets_market_state_data,
-    symbol_to_assets_market_prices, symbols_market_state_data,
+    assets_to_symbols_data, assets_market_state_data,
+    symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_ohlcv_market_state",
     "merge_assets_ohlcv_market_states",
     "merge_symbols_ohlcv_market_states",
@@ -576,15 +576,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOHLCVMarketState(
         screeners=set(screeners),
         **merge_symbols_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in OHLCVMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_symbols_ohlcv_market_states
 
 def merge_assets_ohlcv_market_states(
@@ -604,15 +604,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOHLCVMarketState(
         screeners=set(screeners),
         **merge_assets_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in OHLCVMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_assets_ohlcv_market_states
 
 def assets_to_symbols_ohlcv_market_state(
@@ -626,15 +626,15 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return SymbolsOHLCVMarketState(
         **{
-            name: assets_to_symbol_market_prices(
+            name: assets_to_symbols_data(
                 data=getattr(state, name), separator=separator
             ) for name in OHLCVMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_ohlcv_market_state
 
 def symbols_to_assets_ohlcv_market_state(
@@ -648,13 +648,13 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return AssetsOHLCVMarketState(
         **{
-            name: symbol_to_assets_market_prices(
+            name: symbol_to_assets_data(
                 data=getattr(state, name), separator=separator
             ) for name in OHLCVMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_ohlcv_market_state
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/orderbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, ORDERBOOK_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
-    assets_to_symbol_market_prices, assets_market_state_data,
-    symbol_to_assets_market_prices, symbols_market_state_data,
+    assets_to_symbols_data, assets_market_state_data,
+    symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, SymbolsMarketState, AssetsMarketState
 )
 
 __all__ = [
     "symbols_orderbook_market_state",
     "merge_assets_orderbook_market_states",
     "merge_symbols_orderbook_market_states",
@@ -493,15 +493,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOrderbookMarketState(
         screeners=set(screeners),
         **merge_symbols_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in OrderbookMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_symbols_ohlcv_market_states
 
 def merge_assets_orderbook_market_states(
@@ -521,15 +521,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOrderbookMarketState(
         screeners=set(screeners),
         **merge_assets_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in OrderbookMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_assets_ohlcv_market_states
 
 def assets_to_symbols_orderbook_market_state(
@@ -543,15 +543,15 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return SymbolsOrderbookMarketState(
         **{
-            name: assets_to_symbol_market_prices(
+            name: assets_to_symbols_data(
                 data=getattr(state, name), separator=separator
             ) for name in OrderbookMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_ohlcv_market_state
 
 def symbols_to_assets_orderbook_market_state(
@@ -565,13 +565,13 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return AssetsOrderbookMarketState(
         **{
-            name: symbol_to_assets_market_prices(
+            name: symbol_to_assets_data(
                 data=getattr(state, name), separator=separator
             ) for name in OrderbookMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_ohlcv_market_state
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/orders.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, ORDERS_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
-    assets_to_symbol_market_prices, assets_market_state_data,
-    symbol_to_assets_market_prices, symbols_market_state_data,
+    assets_to_symbols_data, assets_market_state_data,
+    symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_orders_market_state",
     "merge_assets_orders_market_states",
     "merge_symbols_orders_market_states",
@@ -336,15 +336,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOrdersMarketState(
         screeners=set(screeners),
         **merge_symbols_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in OrdersMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_symbols_orders_market_states
 
 def merge_assets_orders_market_states(
@@ -364,15 +364,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOrdersMarketState(
         screeners=set(screeners),
         **merge_assets_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in OrdersMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_assets_orders_market_states
 
 def assets_to_symbols_orders_market_state(
@@ -386,15 +386,15 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return SymbolsOrdersMarketState(
         **{
-            name: assets_to_symbol_market_prices(
+            name: assets_to_symbols_data(
                 data=getattr(state, name), separator=separator
             ) for name in OrdersMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_orders_market_state
 
 def symbols_to_assets_orders_market_state(
@@ -408,13 +408,13 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return AssetsOrdersMarketState(
         **{
-            name: symbol_to_assets_market_prices(
+            name: symbol_to_assets_data(
                 data=getattr(state, name), separator=separator
             ) for name in OrdersMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_orders_market_state
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/state/assets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # assets.py
 
 from abc import ABCMeta
 import datetime as dt
 from typing import (
     Iterable, Dict, Optional, Union,
-    Any, List, Tuple, TypeVar
+    Any, List, Tuple, TypeVar, Type
 )
 
 from attrs import define
 
 from represent import represent
 
 import numpy as np
@@ -17,42 +17,46 @@
 from crypto_screening.dataset import create_market_dataframe
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.market.screeners.orders import OrdersScreener
 from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
-from crypto_screening.collect.screeners import screeners_to_assets_datasets
+from crypto_screening.collect.screeners import find_screeners
 from crypto_screening.collect.market.state.base import (
     is_exchange_in_market_data, get_last_value, MarketState,
-    dataset_to_data, add_data_to_screeners, adjusted_dataset_length,
+    dataset_to_data_rows, add_data_to_screeners, data_from_dataset,
     minimum_common_dataset_length, screener_dataset,
-    add_data_to_symbols_screeners, index_to_datetime
+    add_data_to_symbols_screeners, index_to_datetime,
+    adjusted_screener_dataset_length, sort_data, set_screener_dataset
 )
 
 __all__ = [
     "validate_assets_market_state_values_symbol",
     "assets_market_value",
     "is_symbol_in_assets_market_values",
     "assets_market_values",
-    "assets_to_symbol_market_prices",
+    "assets_to_symbols_data",
     "assets_to_symbols_market_datasets",
     "assets_screeners",
     "assets_to_symbols_market_data",
     "add_assets_market_data_to_screeners",
     "merge_assets_market_data",
     "assets_datasets_to_assets_data",
     "screeners_to_assets_data",
     "assets_market_data",
     "assets_market_state_data",
     "merge_assets_market_states_data",
     "assets_to_symbols_screeners",
     "AssetsMarketState",
     "add_data_to_screeners",
-    "sort_assets_market_data"
+    "sort_assets_market_data",
+    "assets_market_datasets",
+    "screeners_to_assets_datasets",
+    "assets_market_datasets_to_screeners"
 ]
 
 _V = TypeVar("_V")
 
 Data = List[Tuple[dt.datetime, _V]]
 AssetData = Data
 AssetsData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, _V]]]]]
@@ -111,33 +115,33 @@
     """
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
     if exchange not in data:
         raise ValueError(
             f"exchange '{exchange}' is not found inside the values of"
-            f"{f' of {provider}' if provider is not None else ''}. "
+            f"{f' of {repr(provider)}' if provider is not None else ''}. "
             f"Found exchanges for are: {', '.join(data.keys())}"
         )
     # end if
 
     if base not in data[exchange]:
         raise ValueError(
             f"base asset '{base}' is not found in '{exchange}' values of"
-            f"{f' of {provider}' if provider is not None else ''}. "
+            f"{f' of {repr(provider)}' if provider is not None else ''}. "
             f"Found base '{exchange}' assets are: "
             f"{', '.join(data[exchange].keys())}"
         )
     # end if
 
     if quote not in data[exchange][base]:
         raise ValueError(
             f"quote asset '{quote}' is not found in the quote "
             f"assets of the '{base}' base asset in the values"
-            f"{f' of {provider}' if provider is not None else ''}. "
+            f"{f' of {repr(provider)}' if provider is not None else ''}. "
             f"Found quote assets for the '{base}' base asset in "
             f"the values are: {', '.join(data[exchange][base].keys())}"
         )
     # end if
 # end validate_assets_market_state_prices_symbol
 
 def assets_market_values(
@@ -192,71 +196,15 @@
         symbol=symbol, data=data, exchange=exchange,
         separator=separator, provider=provider
     )
 
     return get_last_value(values)
 # end assets_market_price
 
-AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
-AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
-
-@define(repr=False)
-@represent
-class AssetsMarketState(MarketState, metaclass=ABCMeta):
-    """
-    A class to represent the current market state.
-
-    This object contains the state of the market, as Close,
-    bids and asks values of specific assets, gathered from the network.
-
-    attributes:
-
-    - screeners:
-        The screener objects to collect the values of the assets.
-    """
-
-    def data(self) -> AssetsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return assets_market_data(
-            columns=self.ATTRIBUTES,
-            prices={name: getattr(self, name) for name in self.ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> AssetsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: AssetsMarketDatasets = {}
-
-        for exchange, bases in self.data().items():
-            for base, quotes in bases.items():
-                for quote, rows in quotes.items():
-                    dataset = create_market_dataframe(
-                        columns=self.ATTRIBUTES.values()
-                    )
-
-                    for time, row in rows:
-                        dataset.loc[time] = row
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end assets_market_state_to_datasets
-# end AssetsMarketState
+AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, _V]]]]]]
 
 def assets_datasets_to_assets_data(
         datasets: Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 ) -> AssetsMarketData:
     """
     Converts the datasets structure to the structure of the data rows.
 
@@ -264,21 +212,49 @@
 
     :return: The new data.
     """
 
     return {
         exchange: {
             base: {
-                quote: dataset_to_data(dataset=dataset)
+                quote: dataset_to_data_rows(dataset=dataset)
                 for quote, dataset in quotes.items()
             } for base, quotes in bases.items()
         } for exchange, bases in datasets.items()
     }
 # end assets_datasets_to_assets_data
 
+def screeners_to_assets_datasets(
+        screeners: Iterable[BaseScreener],
+        separator: Optional[str] = None
+) -> Dict[str, Dict[str, Dict[str, pd.DataFrame]]]:
+    """
+    Converts the datasets structure to the structure of the data rows.
+
+    :param screeners: The screeners to process.
+    :param separator: The separator for the symbols.
+
+    :return: The new data.
+    """
+
+    results: Dict[str, Dict[str, Dict[str, pd.DataFrame]]] = {}
+
+    for screener in screeners:
+        base, quote = symbol_to_parts(screener.symbol, separator=separator)
+        (
+            results.
+            setdefault(screener.exchange, {}).
+            setdefault(base, {}).
+            setdefault(quote, screener.market)
+        )
+    # end for
+
+    return results
+# end screeners_to_assets_datasets
+
 def screeners_to_assets_data(
         screeners: Iterable[BaseScreener],
         separator: Optional[str] = None
 ) -> AssetsMarketData:
     """
     Converts the datasets structure to the structure of the data rows.
 
@@ -300,16 +276,16 @@
     Sorts the data of the market.
 
     :param data: The data to sort.
     """
 
     for exchange, bases in data.items():
         for base, quotes in bases.items():
-            for quote, prices in quotes.items():
-                prices.sort(key=lambda pair: pair[0])
+            for quote_data in quotes.values():
+                sort_data(data=quote_data)
             # end for
         # end for
     # end for
 # end sort_assets_market_data
 
 def merge_assets_market_data(
         *data: AssetsMarketData, sort: Optional[bool] = True
@@ -342,16 +318,16 @@
     if sort:
         sort_assets_market_data(data=new_data)
     # end if
 
     return new_data
 # end merge_assets_ohlcv_market_states
 
-SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
+AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 
 def assets_to_symbols_market_datasets(
         datasets: AssetsMarketDatasets, separator: Optional[str] = None
 ) -> SymbolsMarketDatasets:
     """
     Converts the datasets structure from assets to symbols.
 
@@ -377,47 +353,47 @@
 
     return symbols_datasets
 # end assets_to_symbols_market_datasets
 
 SymbolData = List[Tuple[dt.datetime, _V]]
 SymbolsData = Dict[str, Dict[str, SymbolData]]
 
-def assets_to_symbol_market_prices(
+def assets_to_symbols_data(
         data: AssetsData, separator: Optional[str] = None
 ) -> SymbolsData:
     """
     Converts an assets market values into a symbols market values.
 
     :param data: The source values.
     :param separator: The separator for the symbols.
 
     :return: The result values.
     """
 
-    symbols_prices: SymbolsData = {}
+    symbols_data: SymbolsData = {}
 
     for exchange, bases in data.items():
         for base, quotes in bases.items():
             for quote, quote_data in quotes.items():
-                for time, price in quote_data:
-                    symbol = parts_to_symbol(base, quote, separator=separator)
+                symbol = parts_to_symbol(base, quote, separator=separator)
 
-                    (
-                        symbols_prices.
-                        setdefault(exchange, {}).
-                        setdefault(symbol, []).
-                        append((time, price))
-                    )
-                # end for
+                (
+                    symbols_data.
+                    setdefault(exchange, {}).
+                    setdefault(symbol, []).
+                    extend(quote_data)
+                )
             # end for
         # end for
     # end for
 
-    return symbols_prices
-# end assets_to_symbol_market_prices
+    return symbols_data
+# end assets_to_symbols_data
+
+SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, _V]]]]]
 
 def assets_to_symbols_market_data(
         data: AssetsMarketData,
         separator: Optional[str] = None
 ) -> SymbolsMarketData:
     """
     Converts the structure of the market data from assets to symbols.
@@ -450,16 +426,71 @@
     "_S",
     BaseScreener,
     OrderbookScreener,
     OHLCVScreener,
     OrdersScreener,
     TradesScreener
 )
+
 AssetsScreeners = Dict[str, Dict[str, Dict[str, _S]]]
 
+def assets_market_datasets_to_screeners(
+        datasets: AssetsMarketDatasets,
+        adjust: Optional[bool] = True,
+        base: Optional[Type[_S]] = None,
+        screeners: Optional[Iterable[_S]] = None,
+        separator: Optional[str] = None
+) -> AssetsScreeners:
+    """
+    Builds the screeners from the assets market datasets structure.
+
+    :param datasets: The datasets for the screeners.
+    :param adjust: The value to adjust the data.
+    :param base: The base type for a screener.
+    :param screeners: screeners to insert datasets into.
+    :param separator: The symbols' separator.
+
+    :return: The screeners.
+    """
+
+    if screeners is None:
+        screeners = []
+    # end if
+
+    screener_base = base or BaseScreener
+
+    new_screeners: AssetsScreeners = {}
+
+    for exchange, bases in datasets.items():
+        for base, quotes in bases.items():
+            for quote, dataset in quotes.items():
+                symbol = parts_to_symbol(base, quote, separator=separator)
+
+                found_screeners = (
+                    find_screeners(screeners, exchange=exchange, symbol=symbol) or
+                    [screener_base(symbol=symbol, exchange=exchange)]
+                )
+
+                for screener in found_screeners:
+                    set_screener_dataset(
+                        screener=screener, dataset=dataset, adjust=adjust
+                    )
+
+                    (
+                        new_screeners.setdefault(exchange, {}).
+                        setdefault(base, {}).
+                        setdefault(quote, screener)
+                    )
+                # end for
+            # end for
+    # end for
+
+    return new_screeners
+# end symbols_market_datasets_to_symbols_screeners
+
 def assets_screeners(screeners: AssetsScreeners) -> List[Union[BaseScreener, _S]]:
     """
     Collects the screeners from the assets screeners structure.
 
     :param screeners: The screeners structure.
 
     :return: The screeners' collection.
@@ -542,167 +573,239 @@
             # end for
         # end for
     # end for
 # end add_assets_data_to_screeners
 
 def assets_market_data(
         columns: Dict[str, str],
-        prices: Optional[Dict[str, AssetsData]] = None
+        data: Optional[Dict[str, AssetsData]] = None,
+        sort: Optional[bool] = True
 ) -> AssetsMarketData:
     """
     Returns the structured data of the state.
 
-    :param prices: The values for the data collection.
+    :param data: The values for the data collection.
     :param columns: The columns for the data.
+    :param sort: The value to sort the data.
 
     :return: The data of the state.
     """
 
-    prices = prices or {name: {} for name in columns}
+    data = data or {name: {} for name in columns}
 
-    datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]]] = {}
+    datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, _V]]]]] = {}
 
-    for name in columns:
-        for exchange, bases in prices[name].items():
+    for name, column in columns.items():
+        for exchange, bases in data[name].items():
             for base, quotes in bases.items():
-                for quote, symbols_prices in quotes.items():
-                    for i, (index, price) in enumerate(symbols_prices):
-                        index = index_to_datetime(index)
-
+                for quote, quote_data in quotes.items():
+                    for index, value in quote_data:
                         (
                             datasets.
                             setdefault(exchange, {}).
                             setdefault(base, {}).
                             setdefault(quote, {}).
-                            setdefault(index, {})
-                        )[columns[name]] = price
+                            setdefault(index_to_datetime(index), {}).
+                            setdefault(column, value)
+                        )
                     # end for
             # end for
         # end for
     # end for
 
     new_datasets: AssetsMarketData = {}
 
     for exchange, bases in datasets.items():
         for base, quotes in bases.items():
-            for quote, symbols_prices in quotes.items():
+            for quote, quote_data in quotes.items():
+                quote_data = list(quote_data.items())
+
                 (
                     new_datasets.
                     setdefault(exchange, {}).
-                    setdefault(base, {})
-                )[quote] = sorted(
-                    list(symbols_prices.items()), key=lambda pair: pair[0]
+                    setdefault(base, {}).
+                    setdefault(quote, quote_data)
                 )
+
+                if sort:
+                    sort_data(data=quote_data)
+                # end if
             # end for
         # end for
     # end for
 
     return new_datasets
 # end assets_market_data
 
+def assets_market_datasets(
+        columns: Dict[str, str],
+        data: Optional[Dict[str, AssetsData]] = None,
+        sort: Optional[bool] = True
+) -> AssetsMarketDatasets:
+    """
+    Returns the structured data of the state.
+
+    :param data: The values for the data collection.
+    :param columns: The columns for the data.
+    :param sort: The value to sort the data.
+
+    :return: The data of the state.
+    """
+
+    datasets: AssetsMarketDatasets = {}
+
+    data = assets_market_data(columns=columns, data=data, sort=sort)
+
+    for exchange, bases in data.items():
+        for base, quotes in bases.items():
+            for quote, rows in quotes.items():
+                dataset = create_market_dataframe(columns=columns)
+
+                for index, row in rows:
+                    dataset.loc[index] = row
+                # end for
+            # end for
+        # end for
+    # end for
+
+    return datasets
+# end assets_market_datasets
+
 def assets_market_state_data(
         columns: Dict[str, str],
         screeners: Iterable[BaseScreener],
-        datas: Optional[Dict[str, AssetsData]] = None,
+        data: Optional[Dict[str, AssetsData]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> Dict[str, AssetsData]:
     """
     Fetches the values and relations between the assets.
 
-    :param datas: The values for the data collection.
+    :param data: The values for the data collection.
     :param columns: The columns for the data.
     :param screeners: The price screeners.
     :param separator: The separator of the assets.
     :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
-    datas = datas or {name: {} for name in columns}
+    data = data or {name: {} for name in columns}
 
     if (length is None) and (not adjust):
         length = minimum_common_dataset_length(
             columns=columns, screeners=screeners
         )
     # end if
 
     for screener in screeners:
         market = screener_dataset(columns=columns, screener=screener)
 
-        try:
-            length = adjusted_dataset_length(
-                dataset=market, adjust=adjust, length=length
-            )
-
-        except ValueError as e:
-            raise ValueError(
-                f"Data of '{screener.exchange}' "
-                f"symbol in '{screener.symbol}' exchange: {e}"
-            )
-        # end try
+        length = adjusted_screener_dataset_length(
+            screener=screener, dataset=market,
+            adjust=adjust, length=length
+        )
 
         base, quote = symbol_to_parts(
             symbol=screener.symbol, separator=separator
         )
 
-        for name in columns:
+        for name, column in columns.items():
+            attribute_data = data_from_dataset(
+                dataset=market, column=column,
+                adjust=adjust, length=length
+            )
+
             (
-                datas[name].
+                data[name].
                 setdefault(screener.exchange, {}).
                 setdefault(base, {}).
-                setdefault(
-                    quote,
-                    list(
-                        zip(
-                            list(market.index[-length:]),
-                            list(market[columns[name]][-length:])
-                        )
-                    )
-                )
+                setdefault(quote, attribute_data)
             )
     # end for
 
-    return datas
+    return data
 # end assets_market_state
 
 def merge_assets_market_states_data(
         *states: MarketState,
-        datas: Dict[str, AssetsData],
+        data: Dict[str, AssetsData],
         sort: Optional[bool] = True
 ) -> Dict[str, AssetsData]:
     """
     Concatenates the states of the market.
 
-    :param datas: The values for the data collection.
+    :param data: The values for the data collection.
     :param states: The states to concatenate.
     :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     for state in states:
-        for name in datas:
+        for name in data:
             for exchange, bases in getattr(state, name).items():
                 for base, quotes in bases.items():
                     for quote, quote_data in quotes.items():
                         (
-                            datas[name].setdefault(exchange, {}).
+                            data[name].setdefault(exchange, {}).
                             setdefault(base, {}).
                             setdefault(quote, []).
                             extend(quote_data)
                         )
                 # end for
             # end for
         # end for
     # end for
 
     if sort:
-        for data in datas.values():
-            sort_assets_market_data(data=data)
+        for attribute_data in data.values():
+            sort_assets_market_data(data=attribute_data)
         # end for
     # end if
 
-    return datas
-# end merge_assets_market_states
+    return data
+# end merge_assets_market_states
+
+@define(repr=False)
+@represent
+class AssetsMarketState(MarketState, metaclass=ABCMeta):
+    """
+    A class to represent the current market state.
+
+    This object contains the state of the market, as Close,
+    bids and asks values of specific assets, gathered from the network.
+
+    attributes:
+
+    - screeners:
+        The screener objects to collect the values of the assets.
+    """
+
+    def data(self) -> AssetsMarketData:
+        """
+        Returns the structured data of the state.
+
+        :return: The data of the state.
+        """
+
+        return assets_market_data(
+            columns=self.ATTRIBUTES,
+            data={name: getattr(self, name) for name in self.ATTRIBUTES}
+        )
+    # end data
+
+    def datasets(self) -> AssetsMarketDatasets:
+        """
+        Rebuilds the dataset from the market state.
+
+        :return: The dataset of the state data.
+        """
+
+        return assets_market_datasets(
+            columns=self.ATTRIBUTES,
+            data={name: getattr(self, name) for name in self.ATTRIBUTES}
+        )
+    # end assets_market_state_to_datasets
+# end AssetsMarketState
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/state/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from crypto_screening.market.screeners.orders import OrdersScreener
 from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.dataset import dataset_to_json
 from crypto_screening.collect.screeners import find_screeners
 
 __all__ = [
     "is_exchange_in_market_data",
-    "dataset_to_data",
+    "dataset_to_data_rows",
     "MarketState",
     "ORDERBOOK_ATTRIBUTES",
     "OHLCV_ATTRIBUTES",
     "ORDERS_ATTRIBUTES",
     "TRADES_ATTRIBUTES",
     "add_data_to_symbols_screeners",
     "add_data_to_screeners",
@@ -39,20 +39,53 @@
     "set_screener_dataset",
     "is_match",
     "screener_dataset",
     "get_last_value",
     "no_match_error",
     "is_ohlcv_orderbook_match",
     "minimum_common_dataset_length",
-    "index_to_datetime"
+    "index_to_datetime",
+    "data_from_dataset",
+    "adjusted_screener_dataset_length",
+    "sort_data"
 ]
 
 _V = TypeVar("_V")
 
 Data = List[Tuple[dt.datetime, _V]]
+
+def data_from_dataset(
+        dataset: pd.DataFrame,
+        column: str,
+        length: Optional[int] = None,
+        adjust: Optional[bool] = True
+) -> Data:
+    """
+    Gets the data of the column from the dataset.
+
+    :param dataset: The dataset to extract data from.
+    :param column: The name of the data column.
+    :param length: The length of data to extract.
+    :param adjust: The value to adjust the length of the data.
+
+    :return: The data of the column from the dataset in the right length.
+    """
+
+    length = adjusted_dataset_length(
+        dataset=dataset, adjust=adjust, length=length
+    )
+
+    return list(
+        zip(
+            list(dataset.index[-length:]),
+            list(dataset[column][-length:])
+        )
+    )
+# end data_from_dataset
+
 def is_exchange_in_market_data(exchange: str, values: Dict[str, Any]) -> None:
     """
     Checks if the exchange is in the values.
 
     :param exchange: The exchange name.
     :param values: The values.
 
@@ -109,27 +142,37 @@
         :return: The hash of the object.
         """
 
         return id(self)
     # end __hash__
 # end MarketState
 
-def dataset_to_data(dataset: pd.DataFrame) -> List[Tuple[dt.datetime, Dict[str, Any]]]:
+def sort_data(data: Data) -> None:
+    """
+    Sorts the data of the market.
+
+    :param data: The data to sort.
+    """
+
+    data.sort(key=lambda pair: pair[0])
+# end sort_data
+
+def dataset_to_data_rows(dataset: pd.DataFrame) -> List[Tuple[dt.datetime, Dict[str, Any]]]:
     """
     Converts the dataset into the data of the rows.
 
     :param dataset: The dataset.
 
     :return: The data structure.
     """
 
     data = dataset_to_json(dataset)
 
     return [
-        (index, value)
+        (index_to_datetime(index), value)
         for index, (_, value) in zip(dataset.index, data)
     ]
 # end dataset_to_data
 
 _S = TypeVar(
     "_S",
     BaseScreener,
@@ -154,15 +197,15 @@
 }
 ORDERS_ATTRIBUTES = {
     "bids": BIDS,
     "asks": ASKS
 }
 TRADES_ATTRIBUTES = {
     "amounts": AMOUNT,
-    "prices": PRICE,
+    "data": PRICE,
     "sides": SIDE
 }
 
 SCREENER_ATTRIBUTES_MATCHES = {
     OrderbookScreener: ORDERBOOK_ATTRIBUTES,
     OHLCVScreener: OHLCV_ATTRIBUTES,
     OrdersScreener: ORDERS_ATTRIBUTES,
@@ -210,15 +253,15 @@
     :param columns: The columns.
 
     :return: The matching boolean flag.
     """
 
     return ValueError(
         f"Unable to set dataset with columns: "
-        f"{set(columns)} to {type(screener)} object of "
+        f"{', '.join(set(columns))} to {type(screener)} object of "
         f"'{screener.exchange}' and symbol "
         f"'{screener.symbol}' to update its data. "
         f"Consider setting the 'adjust' parameter to {True}, ignore."
     )
 # end no_match_error
 
 def set_screener_dataset(
@@ -456,8 +499,38 @@
             f"Data is not long enough for the requested length: {length}. "
             f"Consider using the 'adjust' parameter as {True}, "
             f"to adjust to the actual length of the data."
         )
     # end if
 
     return length
-# end adjusted_dataset_length
+# end adjusted_dataset_length
+
+def adjusted_screener_dataset_length(
+        screener: BaseScreener,
+        dataset: pd.DataFrame,
+        length: Optional[int] = None,
+        adjust: Optional[bool] = True
+) -> int:
+    """
+    Finds the minimum common length of all datasets.
+
+    :param screener: The screener object.
+    :param dataset: The price dataset.
+    :param length: The base length.
+    :param adjust: The value to adjust the length.
+
+    :return: The minimum common length.
+    """
+
+    try:
+        return adjusted_dataset_length(
+            dataset=dataset, adjust=adjust, length=length
+        )
+
+    except ValueError as e:
+        raise ValueError(
+            f"Data of '{screener.exchange}' "
+            f"symbol in '{screener.symbol}' exchange: {e}"
+        )
+    # end try
+# end adjusted_screener_dataset_length
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/state/symbols.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,38 +17,37 @@
 from crypto_screening.dataset import create_market_dataframe
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.market.screeners.orders import OrdersScreener
 from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.symbols import symbol_to_parts
-from crypto_screening.collect.screeners import (
-    find_screeners, screeners_to_symbols_datasets
-)
+from crypto_screening.collect.screeners import find_screeners
 from crypto_screening.collect.market.state.base import (
     is_exchange_in_market_data, get_last_value, MarketState,
-    dataset_to_data, add_data_to_screeners, adjusted_dataset_length,
+    dataset_to_data_rows, add_data_to_screeners, adjusted_dataset_length,
     minimum_common_dataset_length, screener_dataset, set_screener_dataset,
-    add_data_to_symbols_screeners, index_to_datetime
+    add_data_to_symbols_screeners, index_to_datetime, data_from_dataset,
+    adjusted_screener_dataset_length, sort_data
 )
 
 __all__ = [
     "symbols_market_values",
     "symbols_market_value",
     "validate_symbols_market_state_values_symbol",
     "is_exchange_in_market_data",
     "is_symbol_in_symbols_market_values",
-    "symbol_to_assets_market_prices",
+    "symbol_to_assets_data",
     "symbols_to_assets_market_datasets",
     "symbols_screeners",
-    "symbols_market_datasets_to_symbols_screeners",
+    "symbols_market_datasets_to_screeners",
     "add_symbols_market_data_to_screeners",
     "symbols_to_assets_market_data",
     "merge_symbols_market_data",
-    "dataset_to_data",
+    "dataset_to_data_rows",
     "symbols_datasets_to_symbols_data",
     "screeners_to_symbols_data",
     "MarketState",
     "symbols_market_data",
     "symbols_market_state_data",
     "merge_symbols_market_states_data",
     "symbols_to_assets_screeners",
@@ -57,15 +56,17 @@
     "add_data_to_screeners",
     "adjusted_dataset_length",
     "sort_symbols_market_data",
     "set_screener_dataset",
     "screener_dataset",
     "get_last_value",
     "minimum_common_dataset_length",
-    "index_to_datetime"
+    "index_to_datetime",
+    "symbols_market_datasets",
+    "screeners_to_symbols_datasets"
 ]
 
 _V = TypeVar("_V")
 
 Data = List[Tuple[dt.datetime, _V]]
 SymbolData = Data
 SymbolsData = Dict[str, Dict[str, SymbolData]]
@@ -112,23 +113,23 @@
 
     :return: The validation value.
     """
 
     if exchange not in data:
         raise ValueError(
             f"exchange '{exchange}' is not found inside the values of"
-            f"{f' of {provider}' if provider is not None else ''}. "
+            f"{f' of {repr(provider)}' if provider is not None else ''}. "
             f"Found exchanges for are: {', '.join(data.keys())}"
         )
     # end if
 
     if symbol not in data[exchange]:
         raise ValueError(
             f"symbol '{symbol}' is not found in '{exchange}' values of"
-            f"{f' of {provider}' if provider is not None else ''}. "
+            f"{f' of {repr(provider)}' if provider is not None else ''}. "
             f"Found symbols for '{exchange}' values are: "
             f"{', '.join(data[exchange].keys())}"
         )
     # end if
 # end validate_symbols_market_state_prices_symbol
 
 def symbols_market_values(
@@ -177,89 +178,59 @@
         symbol=symbol, data=data,
         exchange=exchange, provider=provider
     )
 
     return get_last_value(values)
 # end symbols_market_price
 
-SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
-SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
-
-@define(repr=False)
-@represent
-class SymbolsMarketState(MarketState, metaclass=ABCMeta):
-    """
-    A class to represent the current market state.
-
-    This object contains the state of the market, as Close,
-    bids and asks values of specific assets, gathered from the network.
-
-    attributes:
-
-    - screeners:
-        The screener objects to collect the values of the assets.
-    """
-
-    def data(self) -> SymbolsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return symbols_market_data(
-            columns=self.ATTRIBUTES,
-            prices={name: getattr(self, name) for name in self.ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> SymbolsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: SymbolsMarketDatasets = {}
-
-        for exchange, symbols in self.data().items():
-            for symbol, rows in symbols.items():
-                dataset = create_market_dataframe(
-                    columns=self.ATTRIBUTES.values()
-                )
-
-                for time, row in rows:
-                    dataset.loc[time] = row
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end symbols_market_state_to_datasets
-# end SymbolsMarketState
+SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, _V]]]]]
 
 def symbols_datasets_to_symbols_data(
         datasets: Dict[str, Dict[str, pd.DataFrame]]
 ) -> SymbolsMarketData:
     """
     Converts the datasets structure to the structure of the data rows.
 
     :param datasets: The datasets to convert.
 
     :return: The new data.
     """
 
     return {
         exchange: {
-            symbol: dataset_to_data(dataset=dataset)
+            symbol: dataset_to_data_rows(dataset=dataset)
             for symbol, dataset in symbols.items()
         } for exchange, symbols in datasets.items()
     }
 # end symbols_datasets_to_symbols_data
 
+def screeners_to_symbols_datasets(
+        screeners: Iterable[BaseScreener]
+) -> Dict[str, Dict[str, pd.DataFrame]]:
+    """
+    Converts the datasets structure to the structure of the data rows.
+
+    :param screeners: The screeners to process.
+
+    :return: The new data.
+    """
+
+    results: Dict[str, Dict[str, pd.DataFrame]] = {}
+
+    for screener in screeners:
+        (
+            results.
+            setdefault(screener.exchange, {}).
+            setdefault(screener.symbol, screener.market)
+        )
+    # end for
+
+    return results
+# end screeners_to_symbols_datasets
+
 def screeners_to_symbols_data(screeners: Iterable[BaseScreener]) -> SymbolsMarketData:
     """
     Converts the datasets structure to the structure of the data rows.
 
     :param screeners: The screeners to process.
 
     :return: The new data.
@@ -274,16 +245,16 @@
     """
     Sorts the data of the market.
 
     :param data: The data to sort.
     """
 
     for exchange, symbols in data.items():
-        for symbol, prices in symbols.items():
-            prices.sort(key=lambda pair: pair[0])
+        for symbol_data in symbols.values():
+            sort_data(data=symbol_data)
         # end for
     # end for
 # end sort_symbols_market_data
 
 def merge_symbols_market_data(
         *data: SymbolsMarketData, sort: Optional[bool] = True
 ) -> SymbolsMarketData:
@@ -313,16 +284,16 @@
     if sort:
         sort_symbols_market_data(data=new_data)
     # end if
 
     return new_data
 # end merge_symbols_ohlcv_market_states
 
-AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
 AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
+SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 def symbols_to_assets_market_datasets(
         datasets: SymbolsMarketDatasets, separator: Optional[str] = None
 ) -> AssetsMarketDatasets:
     """
     Converts the datasets structure from symbols to assets.
 
@@ -348,15 +319,15 @@
 
     return assets_datasets
 # end symbols_to_assets_market_datasets
 
 AssetData = Data
 AssetsData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, _V]]]]]
 
-def symbol_to_assets_market_prices(
+def symbol_to_assets_data(
         data: SymbolsData, separator: Optional[str] = None
 ) -> AssetsData:
     """
     Converts a symbols market values into an assets market values.
 
     :param data: The source values.
     :param separator: The separator for the symbols.
@@ -366,28 +337,28 @@
 
     assets_prices: AssetsData = {}
 
     for exchange, symbols in data.items():
         for symbol, symbol_data in symbols.items():
             base, quote = symbol_to_parts(symbol, separator=separator)
 
-            for time, price in symbol_data:
-                (
-                    assets_prices.
-                    setdefault(exchange, {}).
-                    setdefault(base, {}).
-                    setdefault(quote, []).
-                    append((time, price))
-                )
-            # end for
+            (
+                assets_prices.
+                setdefault(exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, []).
+                extend(symbol_data)
+            )
         # end for
     # end for
 
     return assets_prices
-# end symbol_to_assets_market_prices
+# end symbol_to_assets_data
+
+AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, _V]]]]]]
 
 def symbols_to_assets_market_data(
         data: SymbolsMarketData,
         separator: Optional[str] = None
 ) -> AssetsMarketData:
     """
     Converts the structure of the market data from assets to symbols.
@@ -425,15 +396,15 @@
     OHLCVScreener,
     OrdersScreener,
     TradesScreener
 )
 
 SymbolsScreeners = Dict[str, Dict[str, _S]]
 
-def symbols_market_datasets_to_symbols_screeners(
+def symbols_market_datasets_to_screeners(
         datasets: SymbolsMarketDatasets,
         adjust: Optional[bool] = True,
         base: Optional[Type[_S]] = None,
         screeners: Optional[Iterable[_S]] = None
 ) -> SymbolsScreeners:
     """
     Builds the screeners from the assets market datasets structure.
@@ -554,150 +525,218 @@
             )
         # end for
     # end for
 # end add_symbols_market_data_to_screeners
 
 def symbols_market_data(
         columns: Dict[str, str],
-        prices: Optional[Dict[str, SymbolsData]] = None
+        data: Optional[Dict[str, SymbolsData]] = None,
+        sort: Optional[bool] = True
 ) -> SymbolsMarketData:
     """
     Returns the structured data of the state.
 
-    :param prices: The values for the data collection.
+    :param data: The values for the data collection.
     :param columns: The columns for the data.
+    :param sort: The value to sort the data.
 
     :return: The data of the state.
     """
 
-    datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
-
-    for name in columns:
-        for exchange, symbols in prices[name].items():
-            for symbol, symbols_prices in symbols.items():
-                for i, (index, price) in enumerate(symbols_prices):
-                    index = index_to_datetime(index)
+    datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, _V]]]] = {}
 
+    for name, column in columns.items():
+        for exchange, symbols in data[name].items():
+            for symbol, symbol_data in symbols.items():
+                for index, value in symbol_data:
                     (
                         datasets.
                         setdefault(exchange, {}).
                         setdefault(symbol, {}).
-                        setdefault(index, {})
-                    )[columns[name]] = price
+                        setdefault(index_to_datetime(index), {}).
+                        setdefault(column, value)
+                    )
                 # end for
             # end for
         # end for
     # end for
 
     new_datasets: SymbolsMarketData = {}
 
     for exchange, symbols in datasets.items():
-        for symbol, symbols_prices in symbols.copy().items():
-            new_datasets.setdefault(exchange, {})[symbol] = sorted(
-                list(symbols_prices.items()), key=lambda pair: pair[0]
-            )
+        for symbol, symbol_data in symbols.copy().items():
+            symbol_data = list(symbol_data.items())
+            new_datasets.setdefault(exchange, {})[symbol] = symbol_data
+
+            if sort:
+                sort_data(data=symbol_data)
+            # end if
         # end for
     # end for
 
     return new_datasets
 # end symbols_market_data
 
+def symbols_market_datasets(
+        columns: Dict[str, str],
+        data: Optional[Dict[str, SymbolsData]] = None,
+        sort: Optional[bool] = True
+) -> SymbolsMarketDatasets:
+    """
+    Returns the structured data of the state.
+
+    :param data: The values for the data collection.
+    :param columns: The columns for the data.
+    :param sort: The value to sort the data.
+
+    :return: The data of the state.
+    """
+
+    datasets: SymbolsMarketDatasets = {}
+
+    data = symbols_market_data(columns=columns, data=data, sort=sort)
+
+    for exchange, symbols in data.items():
+        for symbol, rows in symbols.items():
+            dataset = create_market_dataframe(columns=columns)
+
+            for index, row in rows:
+                dataset.loc[index] = row
+            # end for
+        # end for
+    # end for
+
+    return datasets
+# end symbols_market_datasets
+
 def symbols_market_state_data(
         columns: Dict[str, str],
-        datas: Optional[Dict[str, SymbolsData]] = None,
+        data: Optional[Dict[str, SymbolsData]] = None,
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> Dict[str, SymbolsData]:
     """
     Fetches the values and relations between the assets.
 
-    :param datas: The values for the data collection.
+    :param data: The values for the data collection.
     :param columns: The columns for the data.
     :param screeners: The price screeners.
     :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
-    datas = datas or {name: {} for name in columns}
+    data = data or {name: {} for name in columns}
 
     if (length is None) and (not adjust):
         length = minimum_common_dataset_length(
             columns=columns, screeners=screeners
         )
     # end if
 
     for screener in screeners:
         market = screener_dataset(columns=columns, screener=screener)
 
-        try:
-            length = adjusted_dataset_length(
-                dataset=market, adjust=adjust, length=length
-            )
+        length = adjusted_screener_dataset_length(
+            screener=screener, dataset=market,
+            adjust=adjust, length=length
+        )
 
-        except ValueError as e:
-            raise ValueError(
-                f"Data of '{screener.exchange}' "
-                f"symbol in '{screener.symbol}' exchange: {e}"
+        for name, column in columns.items():
+            attribute_data = data_from_dataset(
+                dataset=market, column=column,
+                adjust=adjust, length=length
             )
-        # end try
 
-        for name in columns:
             (
-                datas[name].
+                data[name].
                 setdefault(screener.exchange, {}).
-                setdefault(
-                    screener.symbol,
-                    list(
-                        zip(
-                            list(market.index[-length:]),
-                            list(market[columns[name]][-length:])
-                        )
-                    )
-                )
+                setdefault(screener.symbol, attribute_data)
             )
         # end for
     # end for
 
-    return datas
+    return data
 # end symbols_market_state
 
 def merge_symbols_market_states_data(
         *states: MarketState,
-        datas: Dict[str, SymbolsData],
+        data: Dict[str, SymbolsData],
         sort: Optional[bool] = True
 ) -> Dict[str, SymbolsData]:
     """
     Concatenates the states of the market.
 
-    :param datas: The values for the data collection.
+    :param data: The values for the data collection.
     :param states: The states to concatenate.
     :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     for state in states:
-        for name in datas:
+        for name in data:
             for exchange, symbols in getattr(state, name).items():
                 for symbol, symbol_data in symbols.items():
                     (
-                        datas[name].
+                        data[name].
                         setdefault(exchange, {}).
                         setdefault(symbol, []).
                         extend(symbol_data)
                     )
                 # end for
             # end for
         # end for
     # end for
 
     if sort:
-        for data in datas.values():
-            sort_symbols_market_data(data=data)
+        for attribute_data in data.values():
+            sort_symbols_market_data(data=attribute_data)
         # end for
     # end if
 
-    return datas
-# end merge_symbols_market_states
+    return data
+# end merge_symbols_market_states
+
+@define(repr=False)
+@represent
+class SymbolsMarketState(MarketState, metaclass=ABCMeta):
+    """
+    A class to represent the current market state.
+
+    This object contains the state of the market, as Close,
+    bids and asks values of specific assets, gathered from the network.
+
+    attributes:
+
+    - screeners:
+        The screener objects to collect the values of the assets.
+    """
+
+    def data(self) -> SymbolsMarketData:
+        """
+        Returns the structured data of the state.
+
+        :return: The data of the state.
+        """
+
+        return symbols_market_data(
+            columns=self.ATTRIBUTES,
+            data={name: getattr(self, name) for name in self.ATTRIBUTES}
+        )
+    # end data
+
+    def datasets(self) -> SymbolsMarketDatasets:
+        """
+        Rebuilds the dataset from the market state.
+
+        :return: The dataset of the state data.
+        """
+
+        return symbols_market_datasets(
+            columns=self.ATTRIBUTES,
+            data={name: getattr(self, name) for name in self.ATTRIBUTES}
+        )
+    # end symbols_market_state_to_datasets
+# end SymbolsMarketState
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/market/trades.py` & `crypto-screening-5.4.1/crypto_screening/collect/market/trades.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, TRADES_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
-    assets_to_symbol_market_prices, assets_market_state_data,
-    symbol_to_assets_market_prices, symbols_market_state_data,
+    assets_to_symbols_data, assets_market_state_data,
+    symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_trades_market_state",
     "merge_assets_trades_market_states",
     "merge_symbols_trades_market_states",
@@ -418,15 +418,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsTradesMarketState(
         screeners=set(screeners),
         **merge_symbols_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in TradesMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_symbols_orders_market_states
 
 def merge_assets_trades_market_states(
@@ -446,15 +446,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsTradesMarketState(
         screeners=set(screeners),
         **merge_assets_market_states_data(
-            *states, datas={
+            *states, data={
                 name: {} for name in TradesMarketState.ATTRIBUTES
             }, sort=sort
         )
     )
 # end merge_assets_orders_market_states
 
 def assets_to_symbols_trades_market_state(
@@ -468,15 +468,15 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return SymbolsTradesMarketState(
         **{
-            name: assets_to_symbol_market_prices(
+            name: assets_to_symbols_data(
                 data=getattr(state, name), separator=separator
             ) for name in TradesMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_orders_market_state
 
 def symbols_to_assets_trades_market_state(
@@ -490,13 +490,13 @@
     :param separator: The separator for the symbols.
 
     :return: The results state.
     """
 
     return AssetsTradesMarketState(
         **{
-            name: symbol_to_assets_market_prices(
+            name: symbol_to_assets_data(
                 data=getattr(state, name), separator=separator
             ) for name in TradesMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_orders_market_state
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/screeners.py` & `crypto-screening-5.4.1/crypto_screening/collect/screeners.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,15 @@
     "gather_screeners",
     "exchanges_symbols_screeners",
     "screeners_to_multiple_symbols_screeners",
     "screeners_to_assets_screeners",
     "screeners_to_symbols_screeners",
     "screeners_to_multiple_assets_screeners",
     "screeners_to_multiple_assets_datasets",
-    "screeners_to_multiple_symbols_datasets",
-    "screeners_to_assets_datasets",
-    "screeners_to_symbols_datasets"
+    "screeners_to_multiple_symbols_datasets"
 ]
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_screener_pair(
         screener1: BaseScreener,
         screener2: BaseScreener, /, *,
@@ -534,38 +532,14 @@
             append(screener.market)
         )
     # end for
 
     return results
 # end screeners_to_multiple_symbols_datasets
 
-def screeners_to_symbols_datasets(
-        screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, pd.DataFrame]]:
-    """
-    Converts the datasets structure to the structure of the data rows.
-
-    :param screeners: The screeners to process.
-
-    :return: The new data.
-    """
-
-    results: Dict[str, Dict[str, pd.DataFrame]] = {}
-
-    for screener in screeners:
-        (
-            results.
-            setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, screener.market)
-        )
-    # end for
-
-    return results
-# end screeners_to_symbols_datasets
-
 def screeners_to_multiple_assets_datasets(
         screeners: Iterable[BaseScreener],
         separator: Optional[str] = None
 ) -> Dict[str, Dict[str, Dict[str, List[pd.DataFrame]]]]:
     """
     Converts the datasets structure to the structure of the data rows.
 
@@ -585,36 +559,8 @@
             setdefault(base, {}).
             setdefault(quote, []).
             append(screener.market)
         )
     # end for
 
     return results
-# end screeners_to_multiple_assets_datasets
-
-def screeners_to_assets_datasets(
-        screeners: Iterable[BaseScreener],
-        separator: Optional[str] = None
-) -> Dict[str, Dict[str, Dict[str, pd.DataFrame]]]:
-    """
-    Converts the datasets structure to the structure of the data rows.
-
-    :param screeners: The screeners to process.
-    :param separator: The separator for the symbols.
-
-    :return: The new data.
-    """
-
-    results: Dict[str, Dict[str, Dict[str, pd.DataFrame]]] = {}
-
-    for screener in screeners:
-        base, quote = symbol_to_parts(screener.symbol, separator=separator)
-        (
-            results.
-            setdefault(screener.exchange, {}).
-            setdefault(base, {}).
-            setdefault(quote, screener.market)
-        )
-    # end for
-
-    return results
-# end screeners_to_assets_datasets
+# end screeners_to_multiple_assets_datasets
```

### Comparing `crypto-screening-5.4.0/crypto_screening/collect/symbols.py` & `crypto-screening-5.4.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/dataset.py` & `crypto-screening-5.4.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/interval.py` & `crypto-screening-5.4.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/dynamic.py` & `crypto-screening-5.4.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/foundation/data.py` & `crypto-screening-5.4.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.4.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/foundation/state.py` & `crypto-screening-5.4.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.4.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/base.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/container.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.4.1/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/market/waiting.py` & `crypto-screening-5.4.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/process.py` & `crypto-screening-5.4.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/symbols.py` & `crypto-screening-5.4.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/crypto_screening/validate.py` & `crypto-screening-5.4.1/crypto_screening/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     if not is_valid_symbol(
             exchange=exchange, symbol=symbol, symbols=symbols
     ):
         raise ValueError(
             f"'{symbol}' is not a valid "
             f"symbol for the '{exchange}' exchange. "
             f"Valid symbols: {', '.join(symbols or [])}"
-            f"{f' for {provider}.' if provider else ''}"
+            f"{f' for {repr(provider)}.' if provider else ''}"
         )
     # end if
 
     return symbol
 # end validate_symbol
 
 def validate_interval(interval: str) -> str:
@@ -147,13 +147,13 @@
         exchanges = EXCHANGE_NAMES
     # end if
 
     if not is_valid_exchange(exchange=exchange, exchanges=exchanges):
         raise ValueError(
             f"'{exchange}' is not a valid exchange name. "
             f"Valid exchanges: {', '.join(exchanges or [])}"
-            f"{f' for {provider}.' if provider else ''}"
+            f"{f' for {repr(provider)}.' if provider else ''}"
         )
     # end if
 
     return exchange
 # end validate_exchange
```

### Comparing `crypto-screening-5.4.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.4.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.4.0
+Version: 5.4.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.4.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.4.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.0/pyproject.toml` & `crypto-screening-5.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.4.0'
+version = '5.4.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.4.0/setup.py` & `crypto-screening-5.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.4.0',
+        version='5.4.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

