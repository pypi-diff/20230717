# Comparing `tmp/gvol-0.5.9.tar.gz` & `tmp/gvol-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvol-0.5.9.tar", max compression
+gzip compressed data, was "gvol-0.6.0.tar", max compression
```

## Comparing `gvol-0.5.9.tar` & `gvol-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1132 2023-07-13 09:24:07.767249 gvol-0.5.9/README.md
--rw-r--r--   0        0        0       86 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/__init__.py
--rw-r--r--   0        0        0    55510 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/client.py
--rw-r--r--   0        0        0    36973 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/queries.py
--rw-r--r--   0        0        0     1766 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/types.py
--rw-r--r--   0        0        0     1411 2023-07-13 09:24:07.767249 gvol-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gvol-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-07-17 12:46:30.185339 gvol-0.6.0/README.md
+-rw-r--r--   0        0        0       86 2023-07-17 12:46:30.185339 gvol-0.6.0/gvol/__init__.py
+-rw-r--r--   0        0        0    55510 2023-07-17 12:46:30.185339 gvol-0.6.0/gvol/client.py
+-rw-r--r--   0        0        0    36971 2023-07-17 12:46:30.185339 gvol-0.6.0/gvol/queries.py
+-rw-r--r--   0        0        0     1766 2023-07-17 12:46:30.185339 gvol-0.6.0/gvol/types.py
+-rw-r--r--   0        0        0     1411 2023-07-17 12:46:30.185339 gvol-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gvol-0.6.0/PKG-INFO
```

### Comparing `gvol-0.5.9/README.md` & `gvol-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gvol-0.5.9/gvol/client.py` & `gvol-0.6.0/gvol/client.py`

 * *Files identical despite different names*

### Comparing `gvol-0.5.9/gvol/queries.py` & `gvol-0.6.0/gvol/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1378,17 +1378,17 @@
       oiNotional
       oiPcRatio
     }
   }
 """
 
 options_cumulative_net_volumes = """
-query NetVolumeGvolDirection($tradeType: TradeTypeEnum, $days: Float, $symbol: SymbolEnumType, $exchange: ExchangeEnumType, $showActiveExpirations: Boolean)
- {genericNetVolumeGvolDirection(symbol: $symbol, tradeType: $tradeType, days: $days, exchange: $exchange, showActiveExpirations: $showActiveExpirations) 
- {date strike cumulative indexPrice}}
+query NetVolumeGvolDirection($tradeType: TradeEnumType, $days: Float, $symbol: SymbolEnumType, $exchange: ExchangeEnumType, $showActiveExpirations: Boolean)
+{genericNetVolumeGvolDirection(symbol: $symbol, tradeType: $tradeType, days: $days, exchange: $exchange, showActiveExpirations: $showActiveExpirations) 
+{date strike cumulative indexPrice}}
 """
 
 options_cumulative_net_volumes_hist = """
 query HistoricalNetVolumeApi($symbol: SymbolEnumType, $dateStart: String, $dateEnd: String $exchange: ExchangeEnumType, $tradeType: TradeEnumType, $showActiveExpirations: Boolean)
 { HistoricalNetVolumeApi(symbol: $symbol, dateStart: $dateStart, dateEnd: $dateEnd exchange: $exchange, tradeType: $tradeType, showActiveExpirations: $showActiveExpirations)
 {date strike cumulative cumulativeGamma cumulativeVega cumulativeDelta indexPrice } }
 """
```

### Comparing `gvol-0.5.9/gvol/types.py` & `gvol-0.6.0/gvol/types.py`

 * *Files identical despite different names*

### Comparing `gvol-0.5.9/pyproject.toml` & `gvol-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gvol"
-version = "0.5.9"
+version = "0.6.0"
 description = "GVol is a Python library to access the GVol API"
 authors = ["Denys Halenok <denys.halenok@gmail.com>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/genesis-volatility/gvol-py"
 repository = "https://github.com/genesis-volatility/gvol-py"
```

### Comparing `gvol-0.5.9/PKG-INFO` & `gvol-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvol
-Version: 0.5.9
+Version: 0.6.0
 Summary: GVol is a Python library to access the GVol API
 Home-page: https://github.com/genesis-volatility/gvol-py
 Author: Denys Halenok
 Author-email: denys.halenok@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

