# Comparing `tmp/alphatools_jv-2.2.0.tar.gz` & `tmp/alphatools_jv-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphatools_jv-2.2.0.tar", last modified: Sun Mar 12 06:19:33 2023, max compression
+gzip compressed data, was "alphatools_jv-3.0.0.tar", last modified: Mon Jul 17 01:44:17 2023, max compression
```

## Comparing `alphatools_jv-2.2.0.tar` & `alphatools_jv-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-03-12 06:19:33.071165 alphatools_jv-2.2.0/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2008 2023-03-12 06:19:33.071308 alphatools_jv-2.2.0/PKG-INFO
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1651 2023-01-19 03:58:04.000000 alphatools_jv-2.2.0/README.md
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-03-12 06:19:32.972262 alphatools_jv-2.2.0/alphatools/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-01-09 23:12:54.000000 alphatools_jv-2.2.0/alphatools/__init__.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     6588 2023-02-18 01:28:42.000000 alphatools_jv-2.2.0/alphatools/backtesting_app.py
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-03-12 06:19:33.052551 alphatools_jv-2.2.0/alphatools/utils/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-01-20 03:48:36.000000 alphatools_jv-2.2.0/alphatools/utils/__init__.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1131 2023-03-12 06:17:24.000000 alphatools_jv-2.2.0/alphatools/utils/cache.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1170 2023-02-05 18:12:52.000000 alphatools_jv-2.2.0/alphatools/utils/instrument_pnl_calculator.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1012 2023-02-05 18:12:52.000000 alphatools_jv-2.2.0/alphatools/utils/pnl_calculator.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1973 2023-03-12 06:17:24.000000 alphatools_jv-2.2.0/alphatools/utils/smartapi_helper.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2969 2023-02-17 01:48:30.000000 alphatools_jv-2.2.0/alphatools/utils/token_manager.py
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-03-12 06:19:33.068137 alphatools_jv-2.2.0/alphatools_jv.egg-info/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2008 2023-03-12 06:19:32.000000 alphatools_jv-2.2.0/alphatools_jv.egg-info/PKG-INFO
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      481 2023-03-12 06:19:32.000000 alphatools_jv-2.2.0/alphatools_jv.egg-info/SOURCES.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        1 2023-03-12 06:19:32.000000 alphatools_jv-2.2.0/alphatools_jv.egg-info/dependency_links.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)       16 2023-03-12 06:19:32.000000 alphatools_jv-2.2.0/alphatools_jv.egg-info/top_level.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      135 2023-03-12 06:19:33.072568 alphatools_jv-2.2.0/setup.cfg
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      616 2023-03-12 06:17:36.000000 alphatools_jv-2.2.0/setup.py
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-03-12 06:19:33.070395 alphatools_jv-2.2.0/test/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-01-09 05:13:21.000000 alphatools_jv-2.2.0/test/__init__.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3317 2023-02-05 18:43:11.000000 alphatools_jv-2.2.0/test/test_backtesting_app.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.198527 alphatools_jv-3.0.0/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2055 2023-07-17 01:44:17.197622 alphatools_jv-3.0.0/PKG-INFO
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1651 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/README.md
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.093088 alphatools_jv-3.0.0/alphatools/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/__init__.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     7134 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/backtesting_app.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.097609 alphatools_jv-3.0.0/alphatools/utils/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/utils/__init__.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      335 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/alphatools_prompt.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1376 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/cache.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1170 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/utils/instrument_pnl_calculator.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3397 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/instruments.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1012 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/utils/pnl_calculator.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2603 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/smartapi_helper.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2969 2023-07-16 04:53:16.000000 alphatools_jv-3.0.0/alphatools/utils/token_manager.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.193507 alphatools_jv-3.0.0/alphatools_jv.egg-info/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2055 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/PKG-INFO
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      620 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/SOURCES.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        1 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/dependency_links.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      134 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/requires.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)       16 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/top_level.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)       91 2023-07-17 01:29:34.000000 alphatools_jv-3.0.0/pyproject.toml
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)       38 2023-07-17 01:44:17.198595 alphatools_jv-3.0.0/setup.cfg
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      868 2023-07-17 01:18:54.000000 alphatools_jv-3.0.0/setup.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.196955 alphatools_jv-3.0.0/test/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/test/__init__.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3009 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/test/test_backtesting_app.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/test/test_pnl_calculator.py
```

### Comparing `alphatools_jv-2.2.0/PKG-INFO` & `alphatools_jv-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphatools_jv
-Version: 2.2.0
-Summary: A small example package
+Version: 3.0.0
+Summary: Wrapper over angel broking smartapi to read cached options market data
 Home-page: https://github.com/jaskirat1208/backtest-platform
 Author: Jaskirat Singh
 Author-email: jaskiratsingh1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `alphatools_jv-2.2.0/README.md` & `alphatools_jv-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alphatools_jv-2.2.0/alphatools/backtesting_app.py` & `alphatools_jv-3.0.0/alphatools/backtesting_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.candle_info_df = None
         cfg_parser = configparser.ConfigParser()
         cfg_parser.read(config_file)
         self.api_key = cfg_parser.get('SMARTAPI_LOGIN', 'API_KEY')
         self.client_code = cfg_parser.get('SMARTAPI_LOGIN', 'CLIENT_CODE')
         self.password = cfg_parser.get('SMARTAPI_LOGIN', 'PASSWORD')
         self.totp_key = cfg_parser.get('SMARTAPI_LOGIN', 'TOTP_KEY')
+        self.instruments_list = []
 
     @staticmethod
     def _get_time(time):
         return datetime.strptime(time, '%Y-%m-%dT%H:%M:%S%z')
 
     def _on_md(self, data_row):
         token = data_row["Token"]
@@ -102,31 +103,42 @@
             "symboltoken": token,
             "interval": self.data_interval,
             "fromdate": datetime.strftime(_date, '%Y-%m-%d 00:00'),
             "todate": datetime.strftime(_date, '%Y-%m-%d 23:59')
         }
         self.logger.info("Sending candle request for {}".format(candle_info_params))
         api_helper = SmartApiHelper(self.api_key, self.client_code, self.password, self.totp_key)
-        return api_helper.get_candle_info(candle_info_params)['data']
+        result =  api_helper.get_candle_info(candle_info_params)
+        try:
+            return result['data']
+        except Exception as e:
+            self.logger.error(result)
+            return []
 
     def load_data(self):
         """
         Based on the instrument info requested, sends get Request to AB smart API server
 
         :return: None
         """
+        self.logger.info("Loading data")
         self.candle_info_df = pd.DataFrame.from_records([],
                                                         columns=['Timestamp', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'VOLUME'])
 
         for _date in pd.date_range(self.start_date, self.end_date):
+            self.logger.info("Loading data for {} instruments, date: {}".format(len(self.instruments_list), _date))
+            count = 0
             for token, exchange in self.instruments_list:
+                count += 1
+                self.logger.info("{}/{}: Loading data for date: {}, {}, {}".format(count, len(self.instruments_list), _date, token, exchange))
+                results = None
                 results = self._get_candle_info_results(_date, token, exchange)
                 if not results:
                     self.logger.warning("No data available for Date: {}, "
-                                      "Token: {}, Exchange: {}".format(_date, token, exchange))
+                                    "Token: {}, Exchange: {}".format(_date, token, exchange))
                     continue
                 df = pd.DataFrame.from_records(results,
                                                columns=['Timestamp', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'VOLUME'])
                 df['Token'] = token
                 df['Timestamp'] = df['Timestamp'].apply(lambda x: self._get_time(x))
                 self.candle_info_df = pd.concat([self.candle_info_df, df])
                 sleep(0.35)
```

### Comparing `alphatools_jv-2.2.0/alphatools/utils/cache.py` & `alphatools_jv-3.0.0/alphatools/utils/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import json
 import logging
 
 logging.basicConfig(
-    format='[%(asctime)s] %(levelname)-8s {%(pathname)s:%(lineno)d} : %(message)s',
+    format='[%(asctime)s] %(levelname)-8s {%(filename)s:%(lineno)d} : %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S', level=logging.WARNING
 )
 
 def cache_to_file(dir_name, _hash):
     def decorator(original_func):
         logger = logging.getLogger(__name__)
 
-        def new_func(self, params):
+        def new_func(self, params, force_reload = False):
             hash_result = _hash(params)
             file_name = dir_name + "/{}.csv".format(hash_result)
+            logger.debug("Reading data from file: {}. Force reload set to {}".format(file_name, force_reload))
             try:
                 f = open(file_name, 'r')
                 cache = json.load(f)
                 f.close()
             except (IOError, ValueError):
                 cache = {}
 
-            if hash_result not in cache or not cache[hash_result]:
+            if hash_result not in cache or not cache[hash_result] or force_reload:
                 logger.debug("Could not find results in cache. Calling the function to get results")
                 cache[hash_result] = original_func(self, params)
+                logger.debug("Saving data to file: {}".format(file_name))
                 f = open(file_name, 'w')
                 json.dump(cache, f)
                 f.close()
-            logger.debug("Results already exist. Fetching from cache")
+            else:
+                logger.debug("Results already exist. Fetching from cache")
             return cache[hash_result]
 
         return new_func
 
     return decorator
```

### Comparing `alphatools_jv-2.2.0/alphatools/utils/instrument_pnl_calculator.py` & `alphatools_jv-3.0.0/alphatools/utils/instrument_pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-2.2.0/alphatools/utils/pnl_calculator.py` & `alphatools_jv-3.0.0/alphatools/utils/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-2.2.0/alphatools/utils/token_manager.py` & `alphatools_jv-3.0.0/alphatools/utils/token_manager.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-2.2.0/alphatools_jv.egg-info/PKG-INFO` & `alphatools_jv-3.0.0/alphatools_jv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphatools-jv
-Version: 2.2.0
-Summary: A small example package
+Version: 3.0.0
+Summary: Wrapper over angel broking smartapi to read cached options market data
 Home-page: https://github.com/jaskirat1208/backtest-platform
 Author: Jaskirat Singh
 Author-email: jaskiratsingh1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `alphatools_jv-2.2.0/test/test_backtesting_app.py` & `alphatools_jv-3.0.0/test/test_backtesting_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,38 +32,34 @@
 
     def post_simulation(self):
         self.logger.info("Total Pnl: {}".format(self.get_total_pnl()))
 
 
 class TestBackTestingApp(TestCase):
     logger = logging.getLogger(__name__)
+    def setUp(self) -> None:
+        self.app = BackTestingAppOnDummyData("/Users/jaskiratsingh/projects/smart-api-creds.ini")
+        self.app.add_instrument(53825, "NFO")
+        self.app.add_instrument(48756, "NFO")
+        self.app.set_start_date(datetime.strptime('2022-12-20 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
+        self.app.set_end_date(datetime.strptime('2022-12-20 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
+        self.app.set_interval('ONE_MINUTE')
 
     def test_run_backtesting_engine_basic(self):
-        app = BackTestingAppOnDummyData("/Users/jaskiratsingh/projects/smart-api-creds.ini")
-        app.set_start_date(datetime.strptime('2022-12-20 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
-        app.set_end_date(datetime.strptime('2022-12-20 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
-        app.set_interval('ONE_MINUTE')
-        app.add_instrument(53825, "NFO")
-        app.add_instrument(48756, "NFO")
-        app.load_data()                     # Loads the data into a dataframe
-        app.get_row_number(datetime.strptime('2022-12-23 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
-        df = app.get_candle_info_df()            # Returns the entire simulation dataframe
-        assert len(df) == 2 * len(app.dummy_feed)
+        self.app.load_data()                     # Loads the data into a dataframe
+        self.app.get_row_number(datetime.strptime('2022-12-23 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
+        df = self.app.get_candle_info_df()            # Returns the entire simulation dataframe
+
+        assert len(df) == 2 * len(self.app.dummy_feed)
 
     def test_run_backtesting_engine_advanced(self):
-        app = BackTestingAppOnDummyData("/Users/jaskiratsingh/projects/smart-api-creds.ini")
-        app.set_start_date(datetime.strptime('2022-12-20 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
-        app.set_end_date(datetime.strptime('2022-12-20 11:39:00+05:30', '%Y-%m-%d %H:%M:%S%z'))
-        app.set_interval('ONE_MINUTE')
-        app.add_instrument(53825, "NFO")
-        app.add_instrument(48756, "NFO")
-        app.load_data()                             # Loads the data into a dataframe
-        df1 = app.get_candle_info_df(-1)            # Returns entire candle info dataframe
-        df2 = app.get_candle_info_df(2)             # Returns first two rows of the dataframe
-        assert len(df1) == 2 * len(app.dummy_feed)
+        self.app.load_data()                             # Loads the data into a dataframe
+        df1 = self.app.get_candle_info_df(-1)            # Returns entire candle info dataframe
+        df2 = self.app.get_candle_info_df(2)             # Returns first two rows of the dataframe
+        assert len(df1) == 2 * len(self.app.dummy_feed)
         assert len(df2) == 2
 
     def test_run_token_manager(self):
         app = TokenManager()
         self.logger.info(app.get_instrument('BANKNIFTY23FEB23FUT'))
         self.logger.info(app.get_instrument(48756))
         self.logger.info(app.get_opt("NIFTY", "09FEB23", 16000, "PE"))
```

