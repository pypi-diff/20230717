# Comparing `tmp/shioaji_realtime_kbars-1.0.3.tar.gz` & `tmp/shioaji_realtime_kbars-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_realtime_kbars-1.0.3.tar", last modified: Thu Jun 29 16:01:52 2023, max compression
+gzip compressed data, was "shioaji_realtime_kbars-1.0.4.tar", last modified: Mon Jul 17 15:53:21 2023, max compression
```

## Comparing `shioaji_realtime_kbars-1.0.3.tar` & `shioaji_realtime_kbars-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.3/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4244 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3650 2023-06-29 16:01:34.000000 shioaji_realtime_kbars-1.0.3/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.3/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      757 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.015000 shioaji_realtime_kbars-1.0.3/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5152 2023-06-29 15:59:45.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4244 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:21.002124 shioaji_realtime_kbars-1.0.4/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.4/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4313 2023-07-17 15:53:21.002124 shioaji_realtime_kbars-1.0.4/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3719 2023-07-17 15:52:52.000000 shioaji_realtime_kbars-1.0.4/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.4/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      764 2023-07-17 15:53:21.006124 shioaji_realtime_kbars-1.0.4/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:20.994124 shioaji_realtime_kbars-1.0.4/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:20.998124 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5228 2023-07-17 15:51:45.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:21.002124 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4313 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       21 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/top_level.txt
```

### Comparing `shioaji_realtime_kbars-1.0.3/PKG-INFO` & `shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji_realtime_kbars
-Version: 1.0.3
+Name: shioaji-realtime-kbars
+Version: 1.0.4
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -115,14 +115,16 @@
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
 ## Version
+### v1.0.4 (2023/7/17)
+#### * Fix resamplind will have some NaN rows
 ### v1.0.3 (2023/6/30)
 ### v1.0.2 (2023/6/30)
 #### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
```

### Comparing `shioaji_realtime_kbars-1.0.3/README.md` & `shioaji_realtime_kbars-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
 ## Version
+### v1.0.4 (2023/7/17)
+#### * Fix resamplind will have some NaN rows
 ### v1.0.3 (2023/6/30)
 ### v1.0.2 (2023/6/30)
 #### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
```

### Comparing `shioaji_realtime_kbars-1.0.3/setup.cfg` & `shioaji_realtime_kbars-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_realtime_kbars
-version = 1.0.3
+version = 1.0.4
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you streaming with real-time data
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/Shioaji_Realtime_Kline
@@ -19,14 +19,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	pandas
 	shioaji
+	numpy
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py` & `shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     def getKlines(self, period):
         ts = [int(x) for x in self.ts]
         kbars_list = list(zip(ts, self.Open, self.High, self.Low, self.Close, self.Volume, self.Amount))
         kbars_df = pd.DataFrame(kbars_list, columns=["ts", "Open", "High", "Low", "Close", "Volume", "Amount"])
         kbars_df.ts = pd.to_datetime(kbars_df.ts)
         kbars_df = kbars_df.set_index(kbars_df.ts)
         kbars_df = kbars_df.resample(f'{period}', closed='right', label='right').apply({'Open': 'first', 'High': 'max', 'Low': 'min', 'Close': 'last', 'Volume': 'sum', 'Amount': 'sum'})
+        kbars_df = kbars_df.dropna(subset=['Open', 'High', 'Low', 'Close'])
         kbars = Kbars(ts = kbars_df.index.values.tolist(), 
                            Open = kbars_df["Open"].values.tolist(), 
                            High = kbars_df["High"].values.tolist(), 
                            Low = kbars_df["Low"].values.tolist(), 
                            Close = kbars_df["Close"].values.tolist(), 
                            Volume = kbars_df["Volume"].values.tolist(), 
                            Amount = kbars_df["Amount"].values.tolist())
```

### Comparing `shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/PKG-INFO` & `shioaji_realtime_kbars-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji-realtime-kbars
-Version: 1.0.3
+Name: shioaji_realtime_kbars
+Version: 1.0.4
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -115,14 +115,16 @@
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
 ## Version
+### v1.0.4 (2023/7/17)
+#### * Fix resamplind will have some NaN rows
 ### v1.0.3 (2023/6/30)
 ### v1.0.2 (2023/6/30)
 #### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
```

