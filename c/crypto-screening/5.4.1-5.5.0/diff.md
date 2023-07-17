# Comparing `tmp/crypto-screening-5.4.1.tar.gz` & `tmp/crypto-screening-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.4.1.tar", last modified: Mon Jul 17 09:52:30 2023, max compression
+gzip compressed data, was "crypto-screening-5.5.0.tar", last modified: Mon Jul 17 10:00:42 2023, max compression
```

## Comparing `crypto-screening-5.4.1.tar` & `crypto-screening-5.5.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.794229 crypto-screening-5.4.1/
--rw-rw-rw-   0        0        0       98 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-17 09:52:30.793227 crypto-screening-5.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.4.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.4.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.666414 crypto-screening-5.4.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.697441 crypto-screening-5.4.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.4.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.4.1/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.705442 crypto-screening-5.4.1/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.4.1/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19456 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12436 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.708467 crypto-screening-5.4.1/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24779 2023-07-17 09:51:27.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    14885 2023-07-17 09:42:15.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21766 2023-07-17 09:50:45.000000 crypto-screening-5.4.1/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    14999 2023-07-17 09:43:58.000000 crypto-screening-5.4.1/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16697 2023-07-17 09:46:37.000000 crypto-screening-5.4.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.4.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.4.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.4.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.4.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.719441 crypto-screening-5.4.1/crypto_screening/market/
--rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.4.1/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.739472 crypto-screening-5.4.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.4.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.792257 crypto-screening-5.4.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-16 14:17:05.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36682 2023-07-16 13:04:17.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-16 14:16:54.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18061 2023-07-16 14:05:40.000000 crypto-screening-5.4.1/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.4.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.4.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.4.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4233 2023-07-17 08:56:51.000000 crypto-screening-5.4.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:30.680874 crypto-screening-5.4.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1673 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-17 09:52:30.000000 crypto-screening-5.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.4.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 09:52:30.794229 crypto-screening-5.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-17 09:52:28.000000 crypto-screening-5.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:42.000748 crypto-screening-5.5.0/
+-rw-rw-rw-   0        0        0       98 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-17 10:00:42.000209 crypto-screening-5.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.5.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.5.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.965625 crypto-screening-5.5.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.982982 crypto-screening-5.5.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.5.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.5.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.986614 crypto-screening-5.5.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.5.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19456 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12436 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.988088 crypto-screening-5.5.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24779 2023-07-17 09:51:27.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    14887 2023-07-17 10:00:22.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21766 2023-07-17 09:50:45.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    14999 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16697 2023-07-17 09:46:37.000000 crypto-screening-5.5.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.5.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.5.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.5.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.5.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.990612 crypto-screening-5.5.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.5.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.993126 crypto-screening-5.5.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.998670 crypto-screening-5.5.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-16 14:17:05.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36682 2023-07-16 13:04:17.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-16 14:16:54.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18061 2023-07-16 14:05:40.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.5.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.5.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.5.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4233 2023-07-17 08:56:51.000000 crypto-screening-5.5.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.980462 crypto-screening-5.5.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.5.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:00:42.000748 crypto-screening-5.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-17 10:00:39.000000 crypto-screening-5.5.0/setup.py
```

### Comparing `crypto-screening-5.4.1/PKG-INFO` & `crypto-screening-5.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.4.1
+Version: 5.5.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.4.1/README.md` & `crypto-screening-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/build.py` & `crypto-screening-5.5.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/assets.py` & `crypto-screening-5.5.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/exchanges.py` & `crypto-screening-5.5.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/orderbook.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/orders.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/state/assets.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/state/base.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/state/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 }
 ORDERS_ATTRIBUTES = {
     "bids": BIDS,
     "asks": ASKS
 }
 TRADES_ATTRIBUTES = {
     "amounts": AMOUNT,
-    "data": PRICE,
+    "prices": PRICE,
     "sides": SIDE
 }
 
 SCREENER_ATTRIBUTES_MATCHES = {
     OrderbookScreener: ORDERBOOK_ATTRIBUTES,
     OHLCVScreener: OHLCV_ATTRIBUTES,
     OrdersScreener: ORDERS_ATTRIBUTES,
```

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/market/trades.py` & `crypto-screening-5.5.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/screeners.py` & `crypto-screening-5.5.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/collect/symbols.py` & `crypto-screening-5.5.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/dataset.py` & `crypto-screening-5.5.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/interval.py` & `crypto-screening-5.5.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/dynamic.py` & `crypto-screening-5.5.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/foundation/data.py` & `crypto-screening-5.5.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.5.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/foundation/state.py` & `crypto-screening-5.5.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.5.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/base.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/container.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.5.0/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/market/waiting.py` & `crypto-screening-5.5.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/process.py` & `crypto-screening-5.5.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/symbols.py` & `crypto-screening-5.5.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening/validate.py` & `crypto-screening-5.5.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.5.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.4.1
+Version: 5.5.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.4.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.5.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.4.1/pyproject.toml` & `crypto-screening-5.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.4.1'
+version = '5.5.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.4.1/setup.py` & `crypto-screening-5.5.0/setup.py`

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
-        version='5.4.1',
+        version='5.5.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

