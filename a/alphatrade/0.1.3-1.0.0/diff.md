# Comparing `tmp/alphatrade-0.1.3.tar.gz` & `tmp/alphatrade-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphatrade-0.1.3.tar", last modified: Fri Aug 27 21:19:33 2021, max compression
+gzip compressed data, was "alphatrade-1.0.0.tar", last modified: Mon Jul 17 19:19:03 2023, max compression
```

## Comparing `alphatrade-0.1.3.tar` & `alphatrade-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-08-27 21:19:33.170784 alphatrade-0.1.3/
--rw-rw-rw-   0        0        0     1086 2020-10-24 09:34:37.000000 alphatrade-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       45 2020-10-24 09:35:08.000000 alphatrade-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    32464 2021-08-27 21:19:33.171786 alphatrade-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    31172 2021-08-27 20:15:55.000000 alphatrade-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2021-08-27 21:19:33.085776 alphatrade-0.1.3/alphatrade/
--rw-rw-rw-   0        0        0      329 2020-10-24 09:34:37.000000 alphatrade-0.1.3/alphatrade/__init__.py
--rw-rw-rw-   0        0        0    51499 2021-08-27 20:43:26.000000 alphatrade-0.1.3/alphatrade/alphatrade.py
--rw-rw-rw-   0        0        0     2634 2020-10-24 09:34:37.000000 alphatrade-0.1.3/alphatrade/exceptions.py
-drwxrwxrwx   0        0        0        0 2021-08-27 21:19:33.162781 alphatrade-0.1.3/alphatrade.egg-info/
--rw-rw-rw-   0        0        0    32464 2021-08-27 21:19:32.000000 alphatrade-0.1.3/alphatrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2021-08-27 21:19:32.000000 alphatrade-0.1.3/alphatrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-27 21:19:32.000000 alphatrade-0.1.3/alphatrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2021-08-27 21:19:32.000000 alphatrade-0.1.3/alphatrade.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-08-27 21:19:32.000000 alphatrade-0.1.3/alphatrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2021-08-27 21:19:33.192785 alphatrade-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1555 2021-08-27 21:15:05.000000 alphatrade-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:03.421565 alphatrade-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 19:18:38.000000 alphatrade-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 19:18:38.000000 alphatrade-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33668 2023-07-17 19:19:03.421565 alphatrade-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32551 2023-07-17 19:18:38.000000 alphatrade-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:03.421565 alphatrade-1.0.0/alphatrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 19:18:38.000000 alphatrade-1.0.0/alphatrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51803 2023-07-17 19:18:38.000000 alphatrade-1.0.0/alphatrade/alphatrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-17 19:18:38.000000 alphatrade-1.0.0/alphatrade/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:03.421565 alphatrade-1.0.0/alphatrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33668 2023-07-17 19:19:03.000000 alphatrade-1.0.0/alphatrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-17 19:19:03.000000 alphatrade-1.0.0/alphatrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:19:03.000000 alphatrade-1.0.0/alphatrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 19:19:03.000000 alphatrade-1.0.0/alphatrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 19:19:03.000000 alphatrade-1.0.0/alphatrade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 19:19:03.421565 alphatrade-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-17 19:18:38.000000 alphatrade-1.0.0/setup.py
```

### Comparing `alphatrade-0.1.3/LICENSE` & `alphatrade-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 algo2win
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 algo2win
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `alphatrade-0.1.3/PKG-INFO` & `alphatrade-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,802 +1,851 @@
-Metadata-Version: 2.1
-Name: alphatrade
-Version: 0.1.3
-Summary: Python APIs for SAS Online Alpha Trade Web Platform
-Home-page: https://github.com/algo2t/alphatrade
-Author: Algo 2 Trade
-Author-email: help@algo2.trade
-License: UNKNOWN
-Keywords: alphatrade,alpha-trade,sasonline,python,sdk,trading,stock markets
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python APIs for SAS Online Alpha Trade Web Platform
-# NOTE:: This is Unofficial python module, don't ask SAS support team for help, use it AS-IS
-
-The Python APIs for communicating with the SAS Online Alpha Trade Web Platform.
-
-Alpha Trade Python library provides an easy to use python wrapper over the HTTPS APIs.
-
-The HTTP calls have been converted to methods and JSON responses are wrapped into Python-compatible objects.
-
-Websocket connections are handled automatically within the library.
-
-This work is completely based on Python SDK / APIs for [AliceBlueOnline](https://github.com/krishnavelu/alice_blue.git).  
-Thanks to [krishnavelu](https://github.com/krishnavelu/).  
-
-- **Author: [algo2t](https://github.com/algo2t/)**
-- **Github Repository: [alphatrade](https://github.com/algo2t/alphatrade.git)**
-
-## Installation
-
-This module is installed via pip:
-
-```
-pip install git+https://github.com/algo2t/alphatrade.git
-```
-
-It can also be installed from [pypi](https://pypi.org/project/alphatrade/0.1.2/)  
-
-```
-pip install alphatrade
-```
-
-To force upgrade existing installations:
-
-```
-pip uninstall alphatrade
-pip --no-cache-dir install --upgrade alphatrade
-```
-
-### Prerequisites
-
-Python 3.x
-
-Also, you need the following modules:
-
-- `protlib`
-- `websocket_client`
-- `requests`
-- `pandas`
-
-The modules can also be installed using `pip`
-
-## Examples - Start Here - Important 
-
-Please clone this repository and check the examples folder to get started.  
-Check [here](https://algo2t.github.io/alphatrade/#working-with-examples)
-
-## Getting started with API
-
-### Overview
-
-There is only one class in the whole library: `AlphaTrade`. When the `AlphaTrade` object is created an access token from the SAS Online alpha trade server is stored in text file `access_token.txt` in the same directory. An access token is valid for 24 hours. See the examples folder with `config.py` file to see how to store your credentials.
-With an access token, you can instantiate an AlphaTrade object again. Ideally you only need to create an access_token once every day.
-
-### REST Documentation
-
-The original REST API that this SDK is based on is available online.
-[Alice Blue API REST documentation](http://antplus.aliceblueonline.com/#introduction)
-
-## Using the API
-
-### Logging
-
-The whole library is equipped with pythonâ€˜s `logging` module for debugging. If more debug information is needed, enable logging using the following code.
-
-```python
-import logging
-logging.basicConfig(level=logging.DEBUG)
-```
-
-### Get an access token
-
-1. Import alphatrade
-
-```python
-from alphatrade import *
-```
-
-2. Create `config.py` file  
-Always keep credentials in a separate file
-```python
-login_id = "RR249"
-password = "SAS@249"
-twofa = "rr"
-
-try:
-    access_token = open('access_token.txt', 'r').read().rstrip()
-except Exception as e:
-    print('Exception occurred :: {}'.format(e))
-    access_token = None
-```
-
-3. Import the config
-```python
-import config
-```
-
-### Create AlphaTrade Object
-
-1. Create `AlphaTrade` object with your `login_id`, `password`, `2FA` and/or `access_token`.
-
-Use `config` object to get `login_id`, `password`, `twofa` and `access_token`.  
-
-```python
-from alphatrade import AlphaTrade
-import config
-sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.twofa, access_token=config.access_token)
-```
-
-2. You can run commands here to check your connectivity
-
-```python
-print(sas.get_balance()) # get balance / margin limits
-print(sas.get_profile()) # get profile
-print(sas.get_daywise_positions()) # get daywise positions
-print(sas.get_netwise_positions()) # get netwise positions
-print(sas.get_holding_positions()) # get holding positions
-```
-
-### Get master contracts
-
-Getting master contracts allow you to search for instruments by symbol name and place orders.
-Master contracts are stored as an OrderedDict by token number and by symbol name. Whenever you get a trade update, order update, or quote update, the library will check if master contracts are loaded. If they are, it will attach the instrument object directly to the update. By default all master contracts of all enabled exchanges in your personal profile will be downloaded. i.e. If your profile contains the following as enabled exchanges `['NSE', 'BSE', 'CDS', 'MCX', NFO']` all contract notes of all exchanges will be downloaded by default. If you feel it takes too much time to download all exchange, or if you donâ€˜t need all exchanges to be downloaded, you can specify which exchange to download contract notes while creating the AlphaTrade object.
-
-```python
-sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.twofa, access_token=config.access_token, master_contracts_to_download=['NSE', 'BSE'])
-```
-
-This will reduce a few milliseconds in object creation time of AlphaTrade object.
-
-### Get tradable instruments
-
-Symbols can be retrieved in multiple ways. Once you have the master contract loaded for an exchange, you can get an instrument in many ways.
-
-Get a single instrument by itâ€˜s name:
-
-```python
-tatasteel_nse_eq = sas.get_instrument_by_symbol('NSE', 'TATASTEEL')
-reliance_nse_eq = sas.get_instrument_by_symbol('NSE', 'RELIANCE')
-ongc_bse_eq = sas.get_instrument_by_symbol('BSE', 'ONGC')
-india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
-sensex_nse_index = sas.get_instrument_by_symbol('BSE', 'SENSEX')
-```
-
-Get a single instrument by itâ€˜s token number (generally useful only for BSE Equities):
-
-```python
-ongc_bse_eq = sas.get_instrument_by_token('BSE', 500312)
-reliance_bse_eq = sas.get_instrument_by_token('BSE', 500325)
-acc_nse_eq = sas.get_instrument_by_token('NSE', 22)
-```
-
-Get FNO instruments easily by mentioning expiry, strike & call or put.
-
-```python
-bn_fut = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=True, strike=None, is_call = False)
-bn_call = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = True)
-bn_put = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = False)
-```
-
-### Search for symbols
-
-Search for multiple instruments by matching the name. This works case insensitive and returns all instrument which has the name in its symbol.
-
-```python
-all_sensex_scrips = sas.search_instruments('BSE', 'sEnSeX')
-print(all_sensex_scrips)
-```
-
-The above code results multiple symbol which has â€˜sensexâ€™ in its symbol.
-
-```
-[Instrument(exchange='BSE', token=1, symbol='SENSEX', name='SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=540154, symbol='IDFSENSEXE B', name='IDFC Mutual Fund', expiry=None, lot_size=None), Instrument(exchange='BSE', token=532985, symbol='KTKSENSEX B', name='KOTAK MAHINDRA MUTUAL FUND', expiry=None, lot_size=None), Instrument(exchange='BSE', token=538683, symbol='NETFSENSEX B', name='NIPPON INDIA ETF SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=535276, symbol='SBISENSEX B', name='SBI MUTUAL FUND - SBI ETF SENS', expiry=None, lot_size=None)]
-```
-
-Search for multiple instruments by matching multiple names
-
-```python
-multiple_underlying = ['BANKNIFTY','NIFTY','INFY','BHEL']
-all_scripts = sas.search_instruments('NFO', multiple_underlying)
-```
-
-#### Instrument object
-
-Instruments are represented by instrument objects. These are named-tuples that are created while getting the master contracts. They are used when placing an order and searching for an instrument. The structure of an instrument tuple is as follows:
-
-```python
-Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
-                                      'name', 'expiry', 'lot_size'])
-```
-
-All instruments have the fields mentioned above. Wherever a field is not applicable for an instrument (for example, equity instruments donâ€˜t have strike prices), that value will be `None`
-
-### Quote update
-
-Once you have master contracts loaded, you can easily subscribe to quote updates.
-
-#### Four types of feed data are available
-
-You can subscribe any one type of quote update for a given scrip. Using the `LiveFeedType` enum, you can specify what type of live feed you need.
-
-- `LiveFeedType.MARKET_DATA`
-- `LiveFeedType.COMPACT`
-- `LiveFeedType.SNAPQUOTE`
-- `LiveFeedType.FULL_SNAPQUOTE`
-
-Please refer to the original documentation [here](http://antplus.aliceblueonline.com/#marketdata) for more details of different types of quote update.
-
-#### Subscribe to a live feed
-
-```python
-sas.subscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
-sas.subscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
-```
-
-Subscribe to multiple instruments in a single call. Give an array of instruments to be subscribed.
-
-```python
-sas.subscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
-```
-
-Note: There is a limit of 250 scrips that can be subscribed on total. Beyond this point the server may disconnect web-socket connection.
-
-Start getting live feed via socket
-
-```python
-socket_opened = False
-def event_handler_quote_update(message):
-    print(f"quote update {message}")
-
-def open_callback():
-    global socket_opened
-    socket_opened = True
-
-sas.start_websocket(subscribe_callback=event_handler_quote_update,
-                      socket_open_callback=open_callback,
-                      run_in_background=True)
-while(socket_opened==False):
-    pass
-sas.subscribe(sas.get_instrument_by_symbol('NSE', 'ONGC'), LiveFeedType.MARKET_DATA)
-sleep(10)
-```
-
-#### Unsubscribe to a live feed
-
-Unsubscribe to an existing live feed
-
-```python
-sas.unsubscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
-sas.unsubscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
-```
-
-Unsubscribe to multiple instruments in a single call. Give an array of instruments to be unsubscribed.
-
-```python
-sas.unsubscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
-```
-
-#### Get All Subscribed Symbols
-
-```python
-sas.get_all_subscriptions() # All
-```
-
-### Market Status messages & Exchange messages.
-
-Subscribe to market status messages
-
-```python
-sas.subscribe_market_status_messages()
-```
-
-Getting market status messages.
-
-```python
-print(sas.get_market_status_messages())
-```
-
-Example result of `get_market_status_messages()`
-
-```
-[{'exchange': 'NSE', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 31, 'status': b'The Closing Session has closed.'}, {'exchange': 'NFO', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'CDS', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'BSE', 'length_of_market_type': 13, 'market_type': b'OTHER SESSION', 'length_of_status': 0, 'status': b''}]
-```
-
-Note: As per `alice blue` [documentation](http://antplus.aliceblueonline.com/#market-status) all market status messages should be having a timestamp. But in actual the server doesnâ€˜t send timestamp, so the library is unable to get timestamp for now.
-
-Subscribe to exchange messages
-
-```python
-sas.subscribe_exchange_messages()
-```
-
-Getting market status messages.
-
-```python
-print(sas.get_exchange_messages())
-```
-
-Example result of `get_exchange_messages()`
-
-```
-[{'exchange': 'NSE', 'length': 32, 'message': b'DS : Bulk upload can be started.', 'exchange_time_stamp': 1590148595}, {'exchange': 'NFO', 'length': 200, 'message': b'MARKET WIDE LIMIT FOR VEDL IS 183919959. OPEN POSITIONS IN VEDL HAVE REACHED 84 PERCENT OF THE MARKET WIDE LIMIT.                                                                                       ', 'exchange_time_stamp': 1590146132}, {'exchange': 'CDS', 'length': 54, 'message': b'DS : Regular segment Bhav copy broadcast successfully.', 'exchange_time_stamp': 1590148932}, {'exchange': 'MCX', 'length': 7, 'message': b'.......', 'exchange_time_stamp': 1590196159}]
-```
-
-#### Market Status messages & Exchange messages through callbacks
-
-```python
-socket_opened = False
-def market_status_messages(message):
-    print(f"market status messages {message}")
-
-def exchange_messages(message):
-    print(f"exchange messages {message}")
-
-def open_callback():
-    global socket_opened
-    socket_opened = True
-
-sas.start_websocket(market_status_messages_callback=market_status_messages,
-					  exchange_messages_callback=exchange_messages,
-                      socket_open_callback=open_callback,
-                      run_in_background=True)
-while(socket_opened==False):
-    pass
-sas.subscribe_market_status_messages()
-sas.subscribe_exchange_messages()
-sleep(10)
-```
-
-### Place an order
-
-Place limit, market, SL, SL-M, AMO, BO, CO orders
-
-```python
-print (sas.get_profile())
-
-# TransactionType.Buy, OrderType.Market, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%1%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.Delivery,
-                     price = 0.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-   )
-
-# TransactionType.Buy, OrderType.Market, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%2%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.Intraday,
-                     price = 0.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-# TransactionType.Buy, OrderType.Market, ProductType.CoverOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%3%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.CoverOrder,
-                     price = 0.0,
-                     trigger_price = 7.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.Limit, ProductType.BracketOrder
-# OCO Order can't be of type market
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%4%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.BracketOrder,
-                     price = 8.0,
-                     trigger_price = None,
-                     stop_loss = 6.0,
-                     square_off = 10.0,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-# TransactionType.Buy, OrderType.Limit, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%5%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.Intraday,
-                     price = 8.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.Limit, ProductType.CoverOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%6%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.CoverOrder,
-                     price = 7.0,
-                     trigger_price = 6.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-###############################
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%7%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Delivery,
-                     price = 0.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%8%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Intraday,
-                     price = 0.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.CoverOrder
-# CO order is of type Limit and And Market Only
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.BO
-# BO order is of type Limit and And Market Only
-
-###################################
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%9%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Delivery,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%10%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossLimit,
-                     product_type = ProductType.Intraday,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.CoverOrder
-# CO order is of type Limit and And Market Only
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.BracketOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%11%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossLimit,
-                     product_type = ProductType.BracketOrder,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = 1.0,
-                     square_off = 1.0,
-                     trailing_sl = 20,
-                     is_amo = False)
-)
-```
-
-### Place basket order
-
-Basket order is used to buy or sell group of securities simultaneously.
-
-```python
-order1 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'INFY'),
-            "order_type"        : OrderType.Market,
-            "quantity"          : 1,
-            "transaction_type"  : TransactionType.Buy,
-            "product_type"      : ProductType.Delivery}
-order2 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'SBIN'),
-            "order_type"        : OrderType.Limit,
-            "quantity"          : 2,
-            "price"             : 280.0,
-            "transaction_type"  : TransactionType.Sell,
-            "product_type"      : ProductType.Intraday}
-order = [order1, order2]
-print(sas.place_basket_order(orders))
-```
-
-### Cancel an order
-
-```python
-sas.cancel_order('170713000075481') #Cancel an open order
-```
-
-### Getting order history and trade details
-
-#### Get order history of a particular order
-
-```python
-print(sas.get_order_history('170713000075481'))
-```
-
-#### Get order history of all orders.
-
-```python
-print(sas.get_order_history())
-```
-
-#### Get trade book
-
-```python
-print(sas.get_trade_book())
-```
-
-#### Get historical candles data
-
-This will provide historical data but **not for current day**.  
-This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
-
-```python
-from datetime import datetime
-print(sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', datetime(2020, 10, 19), datetime.now() ,interval=30))
-```
-
-Output 
-
-```console
-Instrument(exchange='MCX', token=224365, symbol='NATURALGAS NOV FUT', name='', expiry=datetime.date(2020, 11, 24), lot_size=None)
-                            open   high    low  close  volume
-date
-2020-10-19 09:00:00+05:30  238.9  239.2  238.4  239.0     373
-2020-10-19 09:30:00+05:30  239.0  239.0  238.4  238.6     210
-2020-10-19 10:00:00+05:30  238.7  238.7  238.1  238.1     213
-2020-10-19 10:30:00+05:30  238.0  238.4  238.0  238.1     116
-2020-10-19 11:00:00+05:30  238.1  238.2  238.0  238.0      69
-...                          ...    ...    ...    ...     ...
-2020-10-23 21:00:00+05:30  237.5  238.1  237.3  237.6     331
-2020-10-23 21:30:00+05:30  237.6  238.5  237.6  237.9     754
-2020-10-23 22:00:00+05:30  237.9  238.1  237.2  237.9     518
-2020-10-23 22:30:00+05:30  237.9  238.7  237.7  238.1     897
-2020-10-23 23:00:00+05:30  238.2  238.3  236.3  236.5    1906
-
-```
-
-Better way to get historical data, first get the latest version from github  
-
-`python -m pip install git+https://github.com/algo2t/alphatrade.git`
-
-```python
-from datetime import datetime
-india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
-print(sas.get_historical_candles(india_vix_nse_index.exchange, india_vix_nse_index.symbol, datetime(2020, 10, 19), datetime.now() ,interval=30))
-```
-
-
-#### Get intraday candles data
-
-This will give candles data for **current day only**.  
-This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
-
-```python
-print(sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', interval=15))
-```
-
-Better way to get intraday data, first get the latest version from github  
-
-`python -m pip install git+https://github.com/algo2t/alphatrade.git`
-
-```python
-from datetime import datetime
-nifty_bank_nse_index = sas.get_instrument_by_symbol('NSE', 'Nifty Bank')
-print(sas.get_intraday_candles(nifty_bank_nse_index.exchange, nifty_bank_nse_index.symbol, datetime(2020, 10, 19), datetime.now(), interval=10))
-```
-
-### Order properties as enums
-
-Order properties such as TransactionType, OrderType, and others have been safely classified as enums so you donâ€˜t have to write them out as strings
-
-#### TransactionType
-
-Transaction types indicate whether you want to buy or sell. Valid transaction types are of the following:
-
-- `TransactionType.Buy` - buy
-- `TransactionType.Sell` - sell
-
-#### OrderType
-
-Order type specifies the type of order you want to send. Valid order types include:
-
-- `OrderType.Market` - Place the order with a market price
-- `OrderType.Limit` - Place the order with a limit price (limit price parameter is mandatory)
-- `OrderType.StopLossLimit` - Place as a stop loss limit order
-- `OrderType.StopLossMarket` - Place as a stop loss market order
-
-#### ProductType
-
-Product types indicate the complexity of the order you want to place. Valid product types are:
-
-- `ProductType.Intraday` - Intraday order that will get squared off before market close
-- `ProductType.Delivery` - Delivery order that will be held with you after market close
-- `ProductType.CoverOrder` - Cover order
-- `ProductType.BracketOrder` - One cancels other order. Also known as bracket order
-
-## Working with examples
-
-[Here](https://github.com/algo2t/alphatrade/tree/main/examples), examples directory there are 3 files `sas_login_eg.py`, `streaming_data.py` and `stop.txt`
-
-### Steps
-
-- Clone the repository to your local machine `git clone https://github.com/algo2t/alphatrade.git`
-- Copy the examples directory to any location where you want to write your code
-- Install the `alphatrade` module using `pip` => `python -m pip install https://github.com/algo2t/alphatrade.git`
-- Open the examples directory in your favorite editor, in our case it is [VSCodium](https://vscodium.com/)
-- Open the `sas_login_eg.py` file in the editor
-- Now, create `config.py` file as per instructions given below and in the above file
-- Provide correct login credentials like login_id, password and twofa
-- twofa must be same for all questions under two factor authentication
-- This is generally set from the homepage of alpha web trading platform [here](https://alpha.sasonline.in/)
-- Click on `FORGET PASSWORD?` => Select `Reset 2FA` radio button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/forget_password.png)
-- Enter the CLIENT ID (LOGIN_ID), EMAIL ID and PAN NUMBER, click on `RESET` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/reset_two_fa.png)
-- Click on `BACK TO LOGIN` and enter `CLIENT ID` and `PASSWORD`, click on `SECURED SIGN-IN`
-- Set same answers for 5 questions and click on `SUBMIT` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/set_answers.png)
-
-`config.py`
-```python
-login_id = "RR249"
-password = "SAS@249"
-twofa = "rr"
-
-try:
-    access_token = open('access_token.txt', 'r').read().rstrip()
-except Exception as e:
-    print('Exception occurred :: {}'.format(e))
-    access_token = None
-
-```
-
-## Example strategy using alpha trade API
-
-[Here](https://github.com/algo2t/alphatrade/blob/main/examples/streaming_data.py) is an example moving average strategy using alpha trade web API.
-This strategy generates a buy signal when 5-EMA > 20-EMA (golden cross) or a sell signal when 5-EMA < 20-EMA (death cross).
-
-## Example for getting historical and intraday candles data
-
-[Here](https://github.com/algo2t/alphatrade/blob/main/examples/historical_data.py) is an example for getting historical data using alpha trade web API.
-
-For historical candles data `start_time` and `end_time` must be provided in format as shown below.
-It can also be provided as `timedelta`. Check the script `historical_data.py` in examples.
-
-```python
-from datetime import datetime, timedelta
-start_time = datetime(2020, 10, 19, 9, 15, 0)
-end_time = datetime(2020, 10, 21, 16, 59, 0)
-
-df = sas.get_historical_candles('MCX', 'NATURALGAS OCT FUT', start_time, end_time, 5)
-print(df)
-end_time = start_time + timedelta(days=5)
-df = sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', start_time, end_time, 15)
-print(df)
-```
-
-For intraday or todayâ€˜s / current dayâ€˜s candles data.  
-
-```python
-df = sas.get_intraday_candles('MCX', 'NATURALGAS OCT FUT')
-print(df)
-df = sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', 15)
-print(df)
-```
-
-
-## Read this before creating an issue
-
-Before creating an issue in this library, please follow the following steps.
-
-1. Search the problem you are facing is already asked by someone else. There might be some issues already there, either solved/unsolved related to your problem. Go to [issues](https://github.com/algo2t/alphatrade/issues) page, use `is:issue` as filter and search your problem. ![image](https://user-images.githubusercontent.com/38440742/85207058-376ee400-b2f4-11ea-91ad-c8fd8a682a12.png)
-2. If you feel your problem is not asked by anyone or no issues are related to your problem, then create a new issue.
-3. Describe your problem in detail while creating the issue. If you donâ€˜t have time to detail/describe the problem you are facing, assume that I also wonâ€˜t be having time to respond to your problem.
-4. Post a sample code of the problem you are facing. If I copy paste the code directly from issue, I should be able to reproduce the problem you are facing.
-5. Before posting the sample code, test your sample code yourself once. Only sample code should be tested, no other addition should be there while you are testing.
-6. Have some print() function calls to display the values of some variables related to your problem.
-7. Post the results of print() functions also in the issue.
-8. Use the insert code feature of github to inset code and print outputs, so that the code is displayed neat. ![image](https://user-images.githubusercontent.com/38440742/85207234-4dc96f80-b2f5-11ea-990c-df013dd69cf2.png)
-
-
+Metadata-Version: 2.1
+Name: alphatrade
+Version: 1.0.0
+Summary: Python APIs for SAS Online Alpha Trade Web Platform
+Home-page: https://github.com/algo2t/alphatrade
+Author: Algo 2 Trade
+Author-email: help@algo2.trade
+License: UNKNOWN
+Keywords: alphatrade,alpha-trade,sasonline,python,sdk,trading,stock markets
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python APIs for SAS Online Alpha Trade Web Platform
+
+# MAJOR CHANGES : NEW VERSION 1.0.0
+
+## API endpoints are changed to match the new ones, bugs expected
+
+1. Removed check for enabled exchanges, you can now download or search symbols from MCX as well if it is not enabled
+2. TOTP SECRET or TOTP both can be given as argument while creating AlphaTrade object (if it is 6 digits it will conside TOTP else TOTP SECRET)
+3. Added new search function to search scrips which will return json for found scrips, you need to process it further
+4. More functions to come.
+5. Check whether streaming websocket is working or not
+6. The `examples` folder is removed and examples are renamed and kept in root directory for ease of development
+
+# STEPS to work
+
+1. Clone the repo locally - `git clone https://github.com/algo2t/alphatrade.git` 
+2. Create a virtualenv - `python -m pip install virtualenv` and then `python -m virtualenv venv` and activate the `venv` environment.
+3. Install dev-requirement.txt - `python -m pip install -r dev-requirements.txt` - this is to ensure `setuptools==57.5.0` is installed. There is a bug with `protlib`, target is to get reed of `protlib` in future
+4. Install requirement.txt - `python -m pip install -r requirement.txt`
+5. Create the `config.py` file in root of cloned repo with `login_id`, `password` and `TOTP` SECRET, you can add the `access_token.txt` if you want to use existing `access_token`.
+6. Try the examples `python zlogin_example.py`, `python zexample_sas_login.py`, `python zhistorical_data.py` and `python zstreaming_data.py`
+7. Expecting issues with the streaming data !!! :P
+
+
+# NOTE:: This is Unofficial python module, don't ask SAS support team for help, use it AS-IS
+
+The Python APIs for communicating with the SAS Online Alpha Trade Web Platform.
+
+Alpha Trade Python library provides an easy to use python wrapper over the HTTPS APIs.
+
+The HTTP calls have been converted to methods and JSON responses are wrapped into Python-compatible objects.
+
+Websocket connections are handled automatically within the library.
+
+This work is completely based on Python SDK / APIs for [AliceBlueOnline](https://github.com/krishnavelu/alice_blue.git).  
+Thanks to [krishnavelu](https://github.com/krishnavelu/).  
+
+- **Author: [algo2t](https://github.com/algo2t/)**
+- **Github Repository: [alphatrade](https://github.com/algo2t/alphatrade.git)**
+
+## Installation
+
+This module is installed via pip:
+
+```
+pip install git+https://github.com/algo2t/alphatrade.git
+```
+
+It can also be installed from [pypi](https://pypi.org/project/alphatrade/0.1.2/)  
+
+```
+pip install alphatrade
+```
+
+To force upgrade existing installations:
+
+```
+pip uninstall alphatrade
+pip --no-cache-dir install --upgrade alphatrade
+```
+
+### Prerequisites
+
+Python 3.x
+
+Also, you need the following modules:
+
+- `protlib`
+- `websocket_client`
+- `requests`
+- `pandas`
+
+The modules can also be installed using `pip`
+
+## Examples - Start Here - Important 
+
+Please clone this repository and check the examples folder to get started.  
+Check [here](https://algo2t.github.io/alphatrade/#working-with-examples)
+
+## Getting started with API
+
+### Overview
+
+There is only one class in the whole library: `AlphaTrade`. When the `AlphaTrade` object is created an access token from the SAS Online alpha trade server is stored in text file `access_token.txt` in the same directory. An access token is valid for 24 hours. See the examples folder with `config.py` file to see how to store your credentials.
+With an access token, you can instantiate an AlphaTrade object again. Ideally you only need to create an access_token once every day.
+
+### REST Documentation
+
+The original REST API that this SDK is based on is available online.
+[Alice Blue API REST documentation](http://antplus.aliceblueonline.com/#introduction)
+
+## Using the API
+
+### Logging
+
+The whole library is equipped with python‘s `logging` module for debugging. If more debug information is needed, enable logging using the following code.
+
+```python
+import logging
+logging.basicConfig(level=logging.DEBUG)
+```
+
+### Get an access token
+
+1. Import alphatrade
+
+```python
+from alphatrade import *
+```
+
+2. Create `config.py` file  
+Always keep credentials in a separate file
+```python
+login_id = "XXXXX"
+password = "XXXXXXXX"
+Totp = 'XXXXXXXXXXXXXXXX'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print('Exception occurred :: {}'.format(e))
+    access_token = None
+```
+
+3. Import the config
+```python
+import config
+```
+
+### Create AlphaTrade Object
+
+1. Create `AlphaTrade` object with your `login_id`, `password`, `TOTP` / `TOTP_SECRET` and/or `access_token`.
+
+Use `config` object to get `login_id`, `password`, `TOTP` and `access_token`.  
+
+```python
+from alphatrade import AlphaTrade
+import config
+import pyotp
+Totp = config.Totp
+pin = pyotp.TOTP(Totp).now()
+totp = f"{int(pin):06d}" if len(pin) <=5 else pin   
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=totp, access_token=config.access_token)
+
+```
+
+```python
+## filename config.py
+
+login_id = "RR24XX"
+password = "SuperSecretPassword!!!"
+TOTP_SECRET = 'YOURTOTPSECRETEXTERNALAUTH'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print(f'Exception occurred :: {e}')
+    access_token = None
+
+```
+
+
+```python
+from alphatrade import AlphaTrade
+import config
+import pyotp
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.TOTP_SECRET, access_token=config.access_token)
+
+```
+
+
+2. You can run commands here to check your connectivity
+
+```python
+print(sas.get_balance()) # get balance / margin limits
+print(sas.get_profile()) # get profile
+print(sas.get_daywise_positions()) # get daywise positions
+print(sas.get_netwise_positions()) # get netwise positions
+print(sas.get_holding_positions()) # get holding positions
+```
+
+### Get master contracts
+
+Getting master contracts allow you to search for instruments by symbol name and place orders.
+Master contracts are stored as an OrderedDict by token number and by symbol name. Whenever you get a trade update, order update, or quote update, the library will check if master contracts are loaded. If they are, it will attach the instrument object directly to the update. By default all master contracts of all enabled exchanges in your personal profile will be downloaded. i.e. If your profile contains the following as enabled exchanges `['NSE', 'BSE', 'CDS', 'MCX', NFO']` all contract notes of all exchanges will be downloaded by default. If you feel it takes too much time to download all exchange, or if you don‘t need all exchanges to be downloaded, you can specify which exchange to download contract notes while creating the AlphaTrade object.
+
+```python
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=totp, access_token=config.access_token, master_contracts_to_download=['NSE', 'BSE'])
+```
+
+This will reduce a few milliseconds in object creation time of AlphaTrade object.
+
+### Get tradable instruments
+
+Symbols can be retrieved in multiple ways. Once you have the master contract loaded for an exchange, you can get an instrument in many ways.
+
+Get a single instrument by it‘s name:
+
+```python
+tatasteel_nse_eq = sas.get_instrument_by_symbol('NSE', 'TATASTEEL')
+reliance_nse_eq = sas.get_instrument_by_symbol('NSE', 'RELIANCE')
+ongc_bse_eq = sas.get_instrument_by_symbol('BSE', 'ONGC')
+india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
+sensex_nse_index = sas.get_instrument_by_symbol('BSE', 'SENSEX')
+```
+
+Get a single instrument by it‘s token number (generally useful only for BSE Equities):
+
+```python
+ongc_bse_eq = sas.get_instrument_by_token('BSE', 500312)
+reliance_bse_eq = sas.get_instrument_by_token('BSE', 500325)
+acc_nse_eq = sas.get_instrument_by_token('NSE', 22)
+```
+
+Get FNO instruments easily by mentioning expiry, strike & call or put.
+
+```python
+bn_fut = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=True, strike=None, is_call = False)
+bn_call = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = True)
+bn_put = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = False)
+```
+
+### Search for symbols
+
+Search for multiple instruments by matching the name. This works case insensitive and returns all instrument which has the name in its symbol.
+
+```python
+all_sensex_scrips = sas.search_instruments('BSE', 'sEnSeX')
+print(all_sensex_scrips)
+```
+
+The above code results multiple symbol which has ‘sensex’ in its symbol.
+
+```
+[Instrument(exchange='BSE', token=1, symbol='SENSEX', name='SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=540154, symbol='IDFSENSEXE B', name='IDFC Mutual Fund', expiry=None, lot_size=None), Instrument(exchange='BSE', token=532985, symbol='KTKSENSEX B', name='KOTAK MAHINDRA MUTUAL FUND', expiry=None, lot_size=None), Instrument(exchange='BSE', token=538683, symbol='NETFSENSEX B', name='NIPPON INDIA ETF SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=535276, symbol='SBISENSEX B', name='SBI MUTUAL FUND - SBI ETF SENS', expiry=None, lot_size=None)]
+```
+
+Search for multiple instruments by matching multiple names
+
+```python
+multiple_underlying = ['BANKNIFTY','NIFTY','INFY','BHEL']
+all_scripts = sas.search_instruments('NFO', multiple_underlying)
+```
+
+#### Instrument object
+
+Instruments are represented by instrument objects. These are named-tuples that are created while getting the master contracts. They are used when placing an order and searching for an instrument. The structure of an instrument tuple is as follows:
+
+```python
+Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
+                                      'name', 'expiry', 'lot_size'])
+```
+
+All instruments have the fields mentioned above. Wherever a field is not applicable for an instrument (for example, equity instruments don‘t have strike prices), that value will be `None`
+
+### Quote update
+
+Once you have master contracts loaded, you can easily subscribe to quote updates.
+
+#### Four types of feed data are available
+
+You can subscribe any one type of quote update for a given scrip. Using the `LiveFeedType` enum, you can specify what type of live feed you need.
+
+- `LiveFeedType.MARKET_DATA`
+- `LiveFeedType.COMPACT`
+- `LiveFeedType.SNAPQUOTE`
+- `LiveFeedType.FULL_SNAPQUOTE`
+
+Please refer to the original documentation [here](http://antplus.aliceblueonline.com/#marketdata) for more details of different types of quote update.
+
+#### Subscribe to a live feed
+
+```python
+sas.subscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
+sas.subscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
+```
+
+Subscribe to multiple instruments in a single call. Give an array of instruments to be subscribed.
+
+```python
+sas.subscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
+```
+
+Note: There is a limit of 250 scrips that can be subscribed on total. Beyond this point the server may disconnect web-socket connection.
+
+Start getting live feed via socket
+
+```python
+socket_opened = False
+def event_handler_quote_update(message):
+    print(f"quote update {message}")
+
+def open_callback():
+    global socket_opened
+    socket_opened = True
+
+sas.start_websocket(subscribe_callback=event_handler_quote_update,
+                      socket_open_callback=open_callback,
+                      run_in_background=True)
+while(socket_opened==False):
+    pass
+sas.subscribe(sas.get_instrument_by_symbol('NSE', 'ONGC'), LiveFeedType.MARKET_DATA)
+sleep(10)
+```
+
+#### Unsubscribe to a live feed
+
+Unsubscribe to an existing live feed
+
+```python
+sas.unsubscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
+sas.unsubscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
+```
+
+Unsubscribe to multiple instruments in a single call. Give an array of instruments to be unsubscribed.
+
+```python
+sas.unsubscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
+```
+
+#### Get All Subscribed Symbols
+
+```python
+sas.get_all_subscriptions() # All
+```
+
+### Market Status messages & Exchange messages.
+
+Subscribe to market status messages
+
+```python
+sas.subscribe_market_status_messages()
+```
+
+Getting market status messages.
+
+```python
+print(sas.get_market_status_messages())
+```
+
+Example result of `get_market_status_messages()`
+
+```
+[{'exchange': 'NSE', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 31, 'status': b'The Closing Session has closed.'}, {'exchange': 'NFO', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'CDS', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'BSE', 'length_of_market_type': 13, 'market_type': b'OTHER SESSION', 'length_of_status': 0, 'status': b''}]
+```
+
+Note: As per `alice blue` [documentation](http://antplus.aliceblueonline.com/#market-status) all market status messages should be having a timestamp. But in actual the server doesn‘t send timestamp, so the library is unable to get timestamp for now.
+
+Subscribe to exchange messages
+
+```python
+sas.subscribe_exchange_messages()
+```
+
+Getting market status messages.
+
+```python
+print(sas.get_exchange_messages())
+```
+
+Example result of `get_exchange_messages()`
+
+```
+[{'exchange': 'NSE', 'length': 32, 'message': b'DS : Bulk upload can be started.', 'exchange_time_stamp': 1590148595}, {'exchange': 'NFO', 'length': 200, 'message': b'MARKET WIDE LIMIT FOR VEDL IS 183919959. OPEN POSITIONS IN VEDL HAVE REACHED 84 PERCENT OF THE MARKET WIDE LIMIT.                                                                                       ', 'exchange_time_stamp': 1590146132}, {'exchange': 'CDS', 'length': 54, 'message': b'DS : Regular segment Bhav copy broadcast successfully.', 'exchange_time_stamp': 1590148932}, {'exchange': 'MCX', 'length': 7, 'message': b'.......', 'exchange_time_stamp': 1590196159}]
+```
+
+#### Market Status messages & Exchange messages through callbacks
+
+```python
+socket_opened = False
+def market_status_messages(message):
+    print(f"market status messages {message}")
+
+def exchange_messages(message):
+    print(f"exchange messages {message}")
+
+def open_callback():
+    global socket_opened
+    socket_opened = True
+
+sas.start_websocket(market_status_messages_callback=market_status_messages,
+					  exchange_messages_callback=exchange_messages,
+                      socket_open_callback=open_callback,
+                      run_in_background=True)
+while(socket_opened==False):
+    pass
+sas.subscribe_market_status_messages()
+sas.subscribe_exchange_messages()
+sleep(10)
+```
+
+### Place an order
+
+Place limit, market, SL, SL-M, AMO, BO, CO orders
+
+```python
+print (sas.get_profile())
+
+# TransactionType.Buy, OrderType.Market, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%1%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.Delivery,
+                     price = 0.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+   )
+
+# TransactionType.Buy, OrderType.Market, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%2%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.Intraday,
+                     price = 0.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+# TransactionType.Buy, OrderType.Market, ProductType.CoverOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%3%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.CoverOrder,
+                     price = 0.0,
+                     trigger_price = 7.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.Limit, ProductType.BracketOrder
+# OCO Order can't be of type market
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%4%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.BracketOrder,
+                     price = 8.0,
+                     trigger_price = None,
+                     stop_loss = 6.0,
+                     square_off = 10.0,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+# TransactionType.Buy, OrderType.Limit, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%5%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.Intraday,
+                     price = 8.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.Limit, ProductType.CoverOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%6%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.CoverOrder,
+                     price = 7.0,
+                     trigger_price = 6.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+###############################
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%7%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Delivery,
+                     price = 0.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%8%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Intraday,
+                     price = 0.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.CoverOrder
+# CO order is of type Limit and And Market Only
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.BO
+# BO order is of type Limit and And Market Only
+
+###################################
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%9%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Delivery,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%10%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossLimit,
+                     product_type = ProductType.Intraday,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.CoverOrder
+# CO order is of type Limit and And Market Only
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.BracketOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%11%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossLimit,
+                     product_type = ProductType.BracketOrder,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = 1.0,
+                     square_off = 1.0,
+                     trailing_sl = 20,
+                     is_amo = False)
+)
+```
+
+### Place basket order
+
+Basket order is used to buy or sell group of securities simultaneously.
+
+```python
+order1 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'INFY'),
+            "order_type"        : OrderType.Market,
+            "quantity"          : 1,
+            "transaction_type"  : TransactionType.Buy,
+            "product_type"      : ProductType.Delivery}
+order2 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'SBIN'),
+            "order_type"        : OrderType.Limit,
+            "quantity"          : 2,
+            "price"             : 280.0,
+            "transaction_type"  : TransactionType.Sell,
+            "product_type"      : ProductType.Intraday}
+order = [order1, order2]
+print(sas.place_basket_order(orders))
+```
+
+### Cancel an order
+
+```python
+sas.cancel_order('170713000075481') #Cancel an open order
+```
+
+### Getting order history and trade details
+
+#### Get order history of a particular order
+
+```python
+print(sas.get_order_history('170713000075481'))
+```
+
+#### Get order history of all orders.
+
+```python
+print(sas.get_order_history())
+```
+
+#### Get trade book
+
+```python
+print(sas.get_trade_book())
+```
+
+#### Get historical candles data
+
+This will provide historical data but **not for current day**.  
+This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
+
+```python
+from datetime import datetime
+print(sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', datetime(2020, 10, 19), datetime.now() ,interval=30))
+```
+
+Output 
+
+```console
+Instrument(exchange='MCX', token=224365, symbol='NATURALGAS NOV FUT', name='', expiry=datetime.date(2020, 11, 24), lot_size=None)
+                            open   high    low  close  volume
+date
+2020-10-19 09:00:00+05:30  238.9  239.2  238.4  239.0     373
+2020-10-19 09:30:00+05:30  239.0  239.0  238.4  238.6     210
+2020-10-19 10:00:00+05:30  238.7  238.7  238.1  238.1     213
+2020-10-19 10:30:00+05:30  238.0  238.4  238.0  238.1     116
+2020-10-19 11:00:00+05:30  238.1  238.2  238.0  238.0      69
+...                          ...    ...    ...    ...     ...
+2020-10-23 21:00:00+05:30  237.5  238.1  237.3  237.6     331
+2020-10-23 21:30:00+05:30  237.6  238.5  237.6  237.9     754
+2020-10-23 22:00:00+05:30  237.9  238.1  237.2  237.9     518
+2020-10-23 22:30:00+05:30  237.9  238.7  237.7  238.1     897
+2020-10-23 23:00:00+05:30  238.2  238.3  236.3  236.5    1906
+
+```
+
+Better way to get historical data, first get the latest version from github  
+
+`python -m pip install git+https://github.com/algo2t/alphatrade.git`
+
+```python
+from datetime import datetime
+india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
+print(sas.get_historical_candles(india_vix_nse_index.exchange, india_vix_nse_index.symbol, datetime(2020, 10, 19), datetime.now() ,interval=30))
+```
+
+
+#### Get intraday candles data
+
+This will give candles data for **current day only**.  
+This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
+
+```python
+print(sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', interval=15))
+```
+
+Better way to get intraday data, first get the latest version from github  
+
+`python -m pip install git+https://github.com/algo2t/alphatrade.git`
+
+```python
+from datetime import datetime
+nifty_bank_nse_index = sas.get_instrument_by_symbol('NSE', 'Nifty Bank')
+print(sas.get_intraday_candles(nifty_bank_nse_index.exchange, nifty_bank_nse_index.symbol, datetime(2020, 10, 19), datetime.now(), interval=10))
+```
+
+### Order properties as enums
+
+Order properties such as TransactionType, OrderType, and others have been safely classified as enums so you don‘t have to write them out as strings
+
+#### TransactionType
+
+Transaction types indicate whether you want to buy or sell. Valid transaction types are of the following:
+
+- `TransactionType.Buy` - buy
+- `TransactionType.Sell` - sell
+
+#### OrderType
+
+Order type specifies the type of order you want to send. Valid order types include:
+
+- `OrderType.Market` - Place the order with a market price
+- `OrderType.Limit` - Place the order with a limit price (limit price parameter is mandatory)
+- `OrderType.StopLossLimit` - Place as a stop loss limit order
+- `OrderType.StopLossMarket` - Place as a stop loss market order
+
+#### ProductType
+
+Product types indicate the complexity of the order you want to place. Valid product types are:
+
+- `ProductType.Intraday` - Intraday order that will get squared off before market close
+- `ProductType.Delivery` - Delivery order that will be held with you after market close
+- `ProductType.CoverOrder` - Cover order
+- `ProductType.BracketOrder` - One cancels other order. Also known as bracket order
+
+## Working with examples
+
+[Here](https://github.com/algo2t/alphatrade), examples directory there are 3 files `zlogin_example.py`, `zstreaming_data.py` and `stop.txt`
+
+### Steps
+
+- Clone the repository to your local machine `git clone https://github.com/algo2t/alphatrade.git`
+- Copy the examples directory to any location where you want to write your code
+- Install the `alphatrade` module using `pip` => `python -m pip install https://github.com/algo2t/alphatrade.git`
+- Open the examples directory in your favorite editor, in our case it is [VSCodium](https://vscodium.com/)
+- Open the `zlogin_example.py` file in the editor
+- Now, create `config.py` file as per instructions given below and in the above file
+- Provide correct login credentials like login_id, password and 16 digit totp code (find below qr code)
+- This is generally set from the homepage of alpha web trading platform [here](https://alpha.sasonline.in/)
+- Click on `FORGET PASSWORD?` => Select `Reset 2FA` radio button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/forget_password.png)
+- Enter the CLIENT ID (LOGIN_ID), EMAIL ID and PAN NUMBER, click on `RESET` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/reset_two_fa.png)
+- Click on `BACK TO LOGIN` and enter `CLIENT ID` and `PASSWORD`, click on `SECURED SIGN-IN`
+- Set same answers for 5 questions and click on `SUBMIT` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/set_answers.png)
+
+`config.py`
+```python
+login_id = "XXXXX"
+password = "XXXXXXXX"
+Totp = 'XXXXXXXXXXXXXXXX'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print('Exception occurred :: {}'.format(e))
+    access_token = None
+```
+
+## Example strategy using alpha trade API
+
+[Here](https://github.com/algo2t/alphatrade/blob/main/zstreaming_data.py) is an example moving average strategy using alpha trade web API.
+This strategy generates a buy signal when 5-EMA > 20-EMA (golden cross) or a sell signal when 5-EMA < 20-EMA (death cross).
+
+## Example for getting historical and intraday candles data
+
+[Here](https://github.com/algo2t/alphatrade/blob/main/zhistorical_data.py) is an example for getting historical data using alpha trade web API.
+
+For historical candles data `start_time` and `end_time` must be provided in format as shown below.
+It can also be provided as `timedelta`. Check the script `zhistorical_data.py` in examples.
+
+```python
+from datetime import datetime, timedelta
+start_time = datetime(2020, 10, 19, 9, 15, 0)
+end_time = datetime(2020, 10, 21, 16, 59, 0)
+
+df = sas.get_historical_candles('MCX', 'NATURALGAS OCT FUT', start_time, end_time, 5)
+print(df)
+end_time = start_time + timedelta(days=5)
+df = sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', start_time, end_time, 15)
+print(df)
+```
+
+For intraday or today‘s / current day‘s candles data.  
+
+```python
+df = sas.get_intraday_candles('MCX', 'NATURALGAS OCT FUT')
+print(df)
+df = sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', 15)
+print(df)
+```
+
+
+## Read this before creating an issue
+
+Before creating an issue in this library, please follow the following steps.
+
+1. Search the problem you are facing is already asked by someone else. There might be some issues already there, either solved/unsolved related to your problem. Go to [issues](https://github.com/algo2t/alphatrade/issues) page, use `is:issue` as filter and search your problem. ![image](https://user-images.githubusercontent.com/38440742/85207058-376ee400-b2f4-11ea-91ad-c8fd8a682a12.png)
+2. If you feel your problem is not asked by anyone or no issues are related to your problem, then create a new issue.
+3. Describe your problem in detail while creating the issue. If you don‘t have time to detail/describe the problem you are facing, assume that I also won‘t be having time to respond to your problem.
+4. Post a sample code of the problem you are facing. If I copy paste the code directly from issue, I should be able to reproduce the problem you are facing.
+5. Before posting the sample code, test your sample code yourself once. Only sample code should be tested, no other addition should be there while you are testing.
+6. Have some print() function calls to display the values of some variables related to your problem.
+7. Post the results of print() functions also in the issue.
+8. Use the insert code feature of github to inset code and print outputs, so that the code is displayed neat. ![image](https://user-images.githubusercontent.com/38440742/85207234-4dc96f80-b2f5-11ea-990c-df013dd69cf2.png)
+
+
```

### Comparing `alphatrade-0.1.3/README.md` & `alphatrade-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,771 +1,822 @@
-# Python APIs for SAS Online Alpha Trade Web Platform
-# NOTE:: This is Unofficial python module, don't ask SAS support team for help, use it AS-IS
-
-The Python APIs for communicating with the SAS Online Alpha Trade Web Platform.
-
-Alpha Trade Python library provides an easy to use python wrapper over the HTTPS APIs.
-
-The HTTP calls have been converted to methods and JSON responses are wrapped into Python-compatible objects.
-
-Websocket connections are handled automatically within the library.
-
-This work is completely based on Python SDK / APIs for [AliceBlueOnline](https://github.com/krishnavelu/alice_blue.git).  
-Thanks to [krishnavelu](https://github.com/krishnavelu/).  
-
-- **Author: [algo2t](https://github.com/algo2t/)**
-- **Github Repository: [alphatrade](https://github.com/algo2t/alphatrade.git)**
-
-## Installation
-
-This module is installed via pip:
-
-```
-pip install git+https://github.com/algo2t/alphatrade.git
-```
-
-It can also be installed from [pypi](https://pypi.org/project/alphatrade/0.1.2/)  
-
-```
-pip install alphatrade
-```
-
-To force upgrade existing installations:
-
-```
-pip uninstall alphatrade
-pip --no-cache-dir install --upgrade alphatrade
-```
-
-### Prerequisites
-
-Python 3.x
-
-Also, you need the following modules:
-
-- `protlib`
-- `websocket_client`
-- `requests`
-- `pandas`
-
-The modules can also be installed using `pip`
-
-## Examples - Start Here - Important 
-
-Please clone this repository and check the examples folder to get started.  
-Check [here](https://algo2t.github.io/alphatrade/#working-with-examples)
-
-## Getting started with API
-
-### Overview
-
-There is only one class in the whole library: `AlphaTrade`. When the `AlphaTrade` object is created an access token from the SAS Online alpha trade server is stored in text file `access_token.txt` in the same directory. An access token is valid for 24 hours. See the examples folder with `config.py` file to see how to store your credentials.
-With an access token, you can instantiate an AlphaTrade object again. Ideally you only need to create an access_token once every day.
-
-### REST Documentation
-
-The original REST API that this SDK is based on is available online.
-[Alice Blue API REST documentation](http://antplus.aliceblueonline.com/#introduction)
-
-## Using the API
-
-### Logging
-
-The whole library is equipped with python‘s `logging` module for debugging. If more debug information is needed, enable logging using the following code.
-
-```python
-import logging
-logging.basicConfig(level=logging.DEBUG)
-```
-
-### Get an access token
-
-1. Import alphatrade
-
-```python
-from alphatrade import *
-```
-
-2. Create `config.py` file  
-Always keep credentials in a separate file
-```python
-login_id = "RR249"
-password = "SAS@249"
-twofa = "rr"
-
-try:
-    access_token = open('access_token.txt', 'r').read().rstrip()
-except Exception as e:
-    print('Exception occurred :: {}'.format(e))
-    access_token = None
-```
-
-3. Import the config
-```python
-import config
-```
-
-### Create AlphaTrade Object
-
-1. Create `AlphaTrade` object with your `login_id`, `password`, `2FA` and/or `access_token`.
-
-Use `config` object to get `login_id`, `password`, `twofa` and `access_token`.  
-
-```python
-from alphatrade import AlphaTrade
-import config
-sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.twofa, access_token=config.access_token)
-```
-
-2. You can run commands here to check your connectivity
-
-```python
-print(sas.get_balance()) # get balance / margin limits
-print(sas.get_profile()) # get profile
-print(sas.get_daywise_positions()) # get daywise positions
-print(sas.get_netwise_positions()) # get netwise positions
-print(sas.get_holding_positions()) # get holding positions
-```
-
-### Get master contracts
-
-Getting master contracts allow you to search for instruments by symbol name and place orders.
-Master contracts are stored as an OrderedDict by token number and by symbol name. Whenever you get a trade update, order update, or quote update, the library will check if master contracts are loaded. If they are, it will attach the instrument object directly to the update. By default all master contracts of all enabled exchanges in your personal profile will be downloaded. i.e. If your profile contains the following as enabled exchanges `['NSE', 'BSE', 'CDS', 'MCX', NFO']` all contract notes of all exchanges will be downloaded by default. If you feel it takes too much time to download all exchange, or if you don‘t need all exchanges to be downloaded, you can specify which exchange to download contract notes while creating the AlphaTrade object.
-
-```python
-sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.twofa, access_token=config.access_token, master_contracts_to_download=['NSE', 'BSE'])
-```
-
-This will reduce a few milliseconds in object creation time of AlphaTrade object.
-
-### Get tradable instruments
-
-Symbols can be retrieved in multiple ways. Once you have the master contract loaded for an exchange, you can get an instrument in many ways.
-
-Get a single instrument by it‘s name:
-
-```python
-tatasteel_nse_eq = sas.get_instrument_by_symbol('NSE', 'TATASTEEL')
-reliance_nse_eq = sas.get_instrument_by_symbol('NSE', 'RELIANCE')
-ongc_bse_eq = sas.get_instrument_by_symbol('BSE', 'ONGC')
-india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
-sensex_nse_index = sas.get_instrument_by_symbol('BSE', 'SENSEX')
-```
-
-Get a single instrument by it‘s token number (generally useful only for BSE Equities):
-
-```python
-ongc_bse_eq = sas.get_instrument_by_token('BSE', 500312)
-reliance_bse_eq = sas.get_instrument_by_token('BSE', 500325)
-acc_nse_eq = sas.get_instrument_by_token('NSE', 22)
-```
-
-Get FNO instruments easily by mentioning expiry, strike & call or put.
-
-```python
-bn_fut = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=True, strike=None, is_call = False)
-bn_call = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = True)
-bn_put = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = False)
-```
-
-### Search for symbols
-
-Search for multiple instruments by matching the name. This works case insensitive and returns all instrument which has the name in its symbol.
-
-```python
-all_sensex_scrips = sas.search_instruments('BSE', 'sEnSeX')
-print(all_sensex_scrips)
-```
-
-The above code results multiple symbol which has ‘sensex’ in its symbol.
-
-```
-[Instrument(exchange='BSE', token=1, symbol='SENSEX', name='SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=540154, symbol='IDFSENSEXE B', name='IDFC Mutual Fund', expiry=None, lot_size=None), Instrument(exchange='BSE', token=532985, symbol='KTKSENSEX B', name='KOTAK MAHINDRA MUTUAL FUND', expiry=None, lot_size=None), Instrument(exchange='BSE', token=538683, symbol='NETFSENSEX B', name='NIPPON INDIA ETF SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=535276, symbol='SBISENSEX B', name='SBI MUTUAL FUND - SBI ETF SENS', expiry=None, lot_size=None)]
-```
-
-Search for multiple instruments by matching multiple names
-
-```python
-multiple_underlying = ['BANKNIFTY','NIFTY','INFY','BHEL']
-all_scripts = sas.search_instruments('NFO', multiple_underlying)
-```
-
-#### Instrument object
-
-Instruments are represented by instrument objects. These are named-tuples that are created while getting the master contracts. They are used when placing an order and searching for an instrument. The structure of an instrument tuple is as follows:
-
-```python
-Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
-                                      'name', 'expiry', 'lot_size'])
-```
-
-All instruments have the fields mentioned above. Wherever a field is not applicable for an instrument (for example, equity instruments don‘t have strike prices), that value will be `None`
-
-### Quote update
-
-Once you have master contracts loaded, you can easily subscribe to quote updates.
-
-#### Four types of feed data are available
-
-You can subscribe any one type of quote update for a given scrip. Using the `LiveFeedType` enum, you can specify what type of live feed you need.
-
-- `LiveFeedType.MARKET_DATA`
-- `LiveFeedType.COMPACT`
-- `LiveFeedType.SNAPQUOTE`
-- `LiveFeedType.FULL_SNAPQUOTE`
-
-Please refer to the original documentation [here](http://antplus.aliceblueonline.com/#marketdata) for more details of different types of quote update.
-
-#### Subscribe to a live feed
-
-```python
-sas.subscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
-sas.subscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
-```
-
-Subscribe to multiple instruments in a single call. Give an array of instruments to be subscribed.
-
-```python
-sas.subscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
-```
-
-Note: There is a limit of 250 scrips that can be subscribed on total. Beyond this point the server may disconnect web-socket connection.
-
-Start getting live feed via socket
-
-```python
-socket_opened = False
-def event_handler_quote_update(message):
-    print(f"quote update {message}")
-
-def open_callback():
-    global socket_opened
-    socket_opened = True
-
-sas.start_websocket(subscribe_callback=event_handler_quote_update,
-                      socket_open_callback=open_callback,
-                      run_in_background=True)
-while(socket_opened==False):
-    pass
-sas.subscribe(sas.get_instrument_by_symbol('NSE', 'ONGC'), LiveFeedType.MARKET_DATA)
-sleep(10)
-```
-
-#### Unsubscribe to a live feed
-
-Unsubscribe to an existing live feed
-
-```python
-sas.unsubscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
-sas.unsubscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
-```
-
-Unsubscribe to multiple instruments in a single call. Give an array of instruments to be unsubscribed.
-
-```python
-sas.unsubscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
-```
-
-#### Get All Subscribed Symbols
-
-```python
-sas.get_all_subscriptions() # All
-```
-
-### Market Status messages & Exchange messages.
-
-Subscribe to market status messages
-
-```python
-sas.subscribe_market_status_messages()
-```
-
-Getting market status messages.
-
-```python
-print(sas.get_market_status_messages())
-```
-
-Example result of `get_market_status_messages()`
-
-```
-[{'exchange': 'NSE', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 31, 'status': b'The Closing Session has closed.'}, {'exchange': 'NFO', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'CDS', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'BSE', 'length_of_market_type': 13, 'market_type': b'OTHER SESSION', 'length_of_status': 0, 'status': b''}]
-```
-
-Note: As per `alice blue` [documentation](http://antplus.aliceblueonline.com/#market-status) all market status messages should be having a timestamp. But in actual the server doesn‘t send timestamp, so the library is unable to get timestamp for now.
-
-Subscribe to exchange messages
-
-```python
-sas.subscribe_exchange_messages()
-```
-
-Getting market status messages.
-
-```python
-print(sas.get_exchange_messages())
-```
-
-Example result of `get_exchange_messages()`
-
-```
-[{'exchange': 'NSE', 'length': 32, 'message': b'DS : Bulk upload can be started.', 'exchange_time_stamp': 1590148595}, {'exchange': 'NFO', 'length': 200, 'message': b'MARKET WIDE LIMIT FOR VEDL IS 183919959. OPEN POSITIONS IN VEDL HAVE REACHED 84 PERCENT OF THE MARKET WIDE LIMIT.                                                                                       ', 'exchange_time_stamp': 1590146132}, {'exchange': 'CDS', 'length': 54, 'message': b'DS : Regular segment Bhav copy broadcast successfully.', 'exchange_time_stamp': 1590148932}, {'exchange': 'MCX', 'length': 7, 'message': b'.......', 'exchange_time_stamp': 1590196159}]
-```
-
-#### Market Status messages & Exchange messages through callbacks
-
-```python
-socket_opened = False
-def market_status_messages(message):
-    print(f"market status messages {message}")
-
-def exchange_messages(message):
-    print(f"exchange messages {message}")
-
-def open_callback():
-    global socket_opened
-    socket_opened = True
-
-sas.start_websocket(market_status_messages_callback=market_status_messages,
-					  exchange_messages_callback=exchange_messages,
-                      socket_open_callback=open_callback,
-                      run_in_background=True)
-while(socket_opened==False):
-    pass
-sas.subscribe_market_status_messages()
-sas.subscribe_exchange_messages()
-sleep(10)
-```
-
-### Place an order
-
-Place limit, market, SL, SL-M, AMO, BO, CO orders
-
-```python
-print (sas.get_profile())
-
-# TransactionType.Buy, OrderType.Market, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%1%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.Delivery,
-                     price = 0.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-   )
-
-# TransactionType.Buy, OrderType.Market, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%2%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.Intraday,
-                     price = 0.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-# TransactionType.Buy, OrderType.Market, ProductType.CoverOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%3%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.CoverOrder,
-                     price = 0.0,
-                     trigger_price = 7.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.Limit, ProductType.BracketOrder
-# OCO Order can't be of type market
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%4%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.BracketOrder,
-                     price = 8.0,
-                     trigger_price = None,
-                     stop_loss = 6.0,
-                     square_off = 10.0,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-# TransactionType.Buy, OrderType.Limit, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%5%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.Intraday,
-                     price = 8.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.Limit, ProductType.CoverOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%6%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.CoverOrder,
-                     price = 7.0,
-                     trigger_price = 6.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-###############################
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%7%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Delivery,
-                     price = 0.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%8%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Intraday,
-                     price = 0.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.CoverOrder
-# CO order is of type Limit and And Market Only
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.BO
-# BO order is of type Limit and And Market Only
-
-###################################
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%9%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Delivery,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%10%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossLimit,
-                     product_type = ProductType.Intraday,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.CoverOrder
-# CO order is of type Limit and And Market Only
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.BracketOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%11%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossLimit,
-                     product_type = ProductType.BracketOrder,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = 1.0,
-                     square_off = 1.0,
-                     trailing_sl = 20,
-                     is_amo = False)
-)
-```
-
-### Place basket order
-
-Basket order is used to buy or sell group of securities simultaneously.
-
-```python
-order1 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'INFY'),
-            "order_type"        : OrderType.Market,
-            "quantity"          : 1,
-            "transaction_type"  : TransactionType.Buy,
-            "product_type"      : ProductType.Delivery}
-order2 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'SBIN'),
-            "order_type"        : OrderType.Limit,
-            "quantity"          : 2,
-            "price"             : 280.0,
-            "transaction_type"  : TransactionType.Sell,
-            "product_type"      : ProductType.Intraday}
-order = [order1, order2]
-print(sas.place_basket_order(orders))
-```
-
-### Cancel an order
-
-```python
-sas.cancel_order('170713000075481') #Cancel an open order
-```
-
-### Getting order history and trade details
-
-#### Get order history of a particular order
-
-```python
-print(sas.get_order_history('170713000075481'))
-```
-
-#### Get order history of all orders.
-
-```python
-print(sas.get_order_history())
-```
-
-#### Get trade book
-
-```python
-print(sas.get_trade_book())
-```
-
-#### Get historical candles data
-
-This will provide historical data but **not for current day**.  
-This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
-
-```python
-from datetime import datetime
-print(sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', datetime(2020, 10, 19), datetime.now() ,interval=30))
-```
-
-Output 
-
-```console
-Instrument(exchange='MCX', token=224365, symbol='NATURALGAS NOV FUT', name='', expiry=datetime.date(2020, 11, 24), lot_size=None)
-                            open   high    low  close  volume
-date
-2020-10-19 09:00:00+05:30  238.9  239.2  238.4  239.0     373
-2020-10-19 09:30:00+05:30  239.0  239.0  238.4  238.6     210
-2020-10-19 10:00:00+05:30  238.7  238.7  238.1  238.1     213
-2020-10-19 10:30:00+05:30  238.0  238.4  238.0  238.1     116
-2020-10-19 11:00:00+05:30  238.1  238.2  238.0  238.0      69
-...                          ...    ...    ...    ...     ...
-2020-10-23 21:00:00+05:30  237.5  238.1  237.3  237.6     331
-2020-10-23 21:30:00+05:30  237.6  238.5  237.6  237.9     754
-2020-10-23 22:00:00+05:30  237.9  238.1  237.2  237.9     518
-2020-10-23 22:30:00+05:30  237.9  238.7  237.7  238.1     897
-2020-10-23 23:00:00+05:30  238.2  238.3  236.3  236.5    1906
-
-```
-
-Better way to get historical data, first get the latest version from github  
-
-`python -m pip install git+https://github.com/algo2t/alphatrade.git`
-
-```python
-from datetime import datetime
-india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
-print(sas.get_historical_candles(india_vix_nse_index.exchange, india_vix_nse_index.symbol, datetime(2020, 10, 19), datetime.now() ,interval=30))
-```
-
-
-#### Get intraday candles data
-
-This will give candles data for **current day only**.  
-This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
-
-```python
-print(sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', interval=15))
-```
-
-Better way to get intraday data, first get the latest version from github  
-
-`python -m pip install git+https://github.com/algo2t/alphatrade.git`
-
-```python
-from datetime import datetime
-nifty_bank_nse_index = sas.get_instrument_by_symbol('NSE', 'Nifty Bank')
-print(sas.get_intraday_candles(nifty_bank_nse_index.exchange, nifty_bank_nse_index.symbol, datetime(2020, 10, 19), datetime.now(), interval=10))
-```
-
-### Order properties as enums
-
-Order properties such as TransactionType, OrderType, and others have been safely classified as enums so you don‘t have to write them out as strings
-
-#### TransactionType
-
-Transaction types indicate whether you want to buy or sell. Valid transaction types are of the following:
-
-- `TransactionType.Buy` - buy
-- `TransactionType.Sell` - sell
-
-#### OrderType
-
-Order type specifies the type of order you want to send. Valid order types include:
-
-- `OrderType.Market` - Place the order with a market price
-- `OrderType.Limit` - Place the order with a limit price (limit price parameter is mandatory)
-- `OrderType.StopLossLimit` - Place as a stop loss limit order
-- `OrderType.StopLossMarket` - Place as a stop loss market order
-
-#### ProductType
-
-Product types indicate the complexity of the order you want to place. Valid product types are:
-
-- `ProductType.Intraday` - Intraday order that will get squared off before market close
-- `ProductType.Delivery` - Delivery order that will be held with you after market close
-- `ProductType.CoverOrder` - Cover order
-- `ProductType.BracketOrder` - One cancels other order. Also known as bracket order
-
-## Working with examples
-
-[Here](https://github.com/algo2t/alphatrade/tree/main/examples), examples directory there are 3 files `sas_login_eg.py`, `streaming_data.py` and `stop.txt`
-
-### Steps
-
-- Clone the repository to your local machine `git clone https://github.com/algo2t/alphatrade.git`
-- Copy the examples directory to any location where you want to write your code
-- Install the `alphatrade` module using `pip` => `python -m pip install https://github.com/algo2t/alphatrade.git`
-- Open the examples directory in your favorite editor, in our case it is [VSCodium](https://vscodium.com/)
-- Open the `sas_login_eg.py` file in the editor
-- Now, create `config.py` file as per instructions given below and in the above file
-- Provide correct login credentials like login_id, password and twofa
-- twofa must be same for all questions under two factor authentication
-- This is generally set from the homepage of alpha web trading platform [here](https://alpha.sasonline.in/)
-- Click on `FORGET PASSWORD?` => Select `Reset 2FA` radio button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/forget_password.png)
-- Enter the CLIENT ID (LOGIN_ID), EMAIL ID and PAN NUMBER, click on `RESET` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/reset_two_fa.png)
-- Click on `BACK TO LOGIN` and enter `CLIENT ID` and `PASSWORD`, click on `SECURED SIGN-IN`
-- Set same answers for 5 questions and click on `SUBMIT` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/set_answers.png)
-
-`config.py`
-```python
-login_id = "RR249"
-password = "SAS@249"
-twofa = "rr"
-
-try:
-    access_token = open('access_token.txt', 'r').read().rstrip()
-except Exception as e:
-    print('Exception occurred :: {}'.format(e))
-    access_token = None
-
-```
-
-## Example strategy using alpha trade API
-
-[Here](https://github.com/algo2t/alphatrade/blob/main/examples/streaming_data.py) is an example moving average strategy using alpha trade web API.
-This strategy generates a buy signal when 5-EMA > 20-EMA (golden cross) or a sell signal when 5-EMA < 20-EMA (death cross).
-
-## Example for getting historical and intraday candles data
-
-[Here](https://github.com/algo2t/alphatrade/blob/main/examples/historical_data.py) is an example for getting historical data using alpha trade web API.
-
-For historical candles data `start_time` and `end_time` must be provided in format as shown below.
-It can also be provided as `timedelta`. Check the script `historical_data.py` in examples.
-
-```python
-from datetime import datetime, timedelta
-start_time = datetime(2020, 10, 19, 9, 15, 0)
-end_time = datetime(2020, 10, 21, 16, 59, 0)
-
-df = sas.get_historical_candles('MCX', 'NATURALGAS OCT FUT', start_time, end_time, 5)
-print(df)
-end_time = start_time + timedelta(days=5)
-df = sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', start_time, end_time, 15)
-print(df)
-```
-
-For intraday or today‘s / current day‘s candles data.  
-
-```python
-df = sas.get_intraday_candles('MCX', 'NATURALGAS OCT FUT')
-print(df)
-df = sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', 15)
-print(df)
-```
-
-
-## Read this before creating an issue
-
-Before creating an issue in this library, please follow the following steps.
-
-1. Search the problem you are facing is already asked by someone else. There might be some issues already there, either solved/unsolved related to your problem. Go to [issues](https://github.com/algo2t/alphatrade/issues) page, use `is:issue` as filter and search your problem. ![image](https://user-images.githubusercontent.com/38440742/85207058-376ee400-b2f4-11ea-91ad-c8fd8a682a12.png)
-2. If you feel your problem is not asked by anyone or no issues are related to your problem, then create a new issue.
-3. Describe your problem in detail while creating the issue. If you don‘t have time to detail/describe the problem you are facing, assume that I also won‘t be having time to respond to your problem.
-4. Post a sample code of the problem you are facing. If I copy paste the code directly from issue, I should be able to reproduce the problem you are facing.
-5. Before posting the sample code, test your sample code yourself once. Only sample code should be tested, no other addition should be there while you are testing.
-6. Have some print() function calls to display the values of some variables related to your problem.
-7. Post the results of print() functions also in the issue.
-8. Use the insert code feature of github to inset code and print outputs, so that the code is displayed neat. ![image](https://user-images.githubusercontent.com/38440742/85207234-4dc96f80-b2f5-11ea-990c-df013dd69cf2.png)
+# Python APIs for SAS Online Alpha Trade Web Platform
+
+# MAJOR CHANGES : NEW VERSION 1.0.0
+
+## API endpoints are changed to match the new ones, bugs expected
+
+1. Removed check for enabled exchanges, you can now download or search symbols from MCX as well if it is not enabled
+2. TOTP SECRET or TOTP both can be given as argument while creating AlphaTrade object (if it is 6 digits it will conside TOTP else TOTP SECRET)
+3. Added new search function to search scrips which will return json for found scrips, you need to process it further
+4. More functions to come.
+5. Check whether streaming websocket is working or not
+6. The `examples` folder is removed and examples are renamed and kept in root directory for ease of development
+
+# STEPS to work
+
+1. Clone the repo locally - `git clone https://github.com/algo2t/alphatrade.git` 
+2. Create a virtualenv - `python -m pip install virtualenv` and then `python -m virtualenv venv` and activate the `venv` environment.
+3. Install dev-requirement.txt - `python -m pip install -r dev-requirements.txt` - this is to ensure `setuptools==57.5.0` is installed. There is a bug with `protlib`, target is to get reed of `protlib` in future
+4. Install requirement.txt - `python -m pip install -r requirement.txt`
+5. Create the `config.py` file in root of cloned repo with `login_id`, `password` and `TOTP` SECRET, you can add the `access_token.txt` if you want to use existing `access_token`.
+6. Try the examples `python zlogin_example.py`, `python zexample_sas_login.py`, `python zhistorical_data.py` and `python zstreaming_data.py`
+7. Expecting issues with the streaming data !!! :P
+
+
+# NOTE:: This is Unofficial python module, don't ask SAS support team for help, use it AS-IS
+
+The Python APIs for communicating with the SAS Online Alpha Trade Web Platform.
+
+Alpha Trade Python library provides an easy to use python wrapper over the HTTPS APIs.
+
+The HTTP calls have been converted to methods and JSON responses are wrapped into Python-compatible objects.
+
+Websocket connections are handled automatically within the library.
+
+This work is completely based on Python SDK / APIs for [AliceBlueOnline](https://github.com/krishnavelu/alice_blue.git).  
+Thanks to [krishnavelu](https://github.com/krishnavelu/).  
+
+- **Author: [algo2t](https://github.com/algo2t/)**
+- **Github Repository: [alphatrade](https://github.com/algo2t/alphatrade.git)**
+
+## Installation
+
+This module is installed via pip:
+
+```
+pip install git+https://github.com/algo2t/alphatrade.git
+```
+
+It can also be installed from [pypi](https://pypi.org/project/alphatrade/0.1.2/)  
+
+```
+pip install alphatrade
+```
+
+To force upgrade existing installations:
+
+```
+pip uninstall alphatrade
+pip --no-cache-dir install --upgrade alphatrade
+```
+
+### Prerequisites
+
+Python 3.x
+
+Also, you need the following modules:
+
+- `protlib`
+- `websocket_client`
+- `requests`
+- `pandas`
+
+The modules can also be installed using `pip`
+
+## Examples - Start Here - Important 
+
+Please clone this repository and check the examples folder to get started.  
+Check [here](https://algo2t.github.io/alphatrade/#working-with-examples)
+
+## Getting started with API
+
+### Overview
+
+There is only one class in the whole library: `AlphaTrade`. When the `AlphaTrade` object is created an access token from the SAS Online alpha trade server is stored in text file `access_token.txt` in the same directory. An access token is valid for 24 hours. See the examples folder with `config.py` file to see how to store your credentials.
+With an access token, you can instantiate an AlphaTrade object again. Ideally you only need to create an access_token once every day.
+
+### REST Documentation
+
+The original REST API that this SDK is based on is available online.
+[Alice Blue API REST documentation](http://antplus.aliceblueonline.com/#introduction)
+
+## Using the API
+
+### Logging
+
+The whole library is equipped with python‘s `logging` module for debugging. If more debug information is needed, enable logging using the following code.
+
+```python
+import logging
+logging.basicConfig(level=logging.DEBUG)
+```
+
+### Get an access token
+
+1. Import alphatrade
+
+```python
+from alphatrade import *
+```
+
+2. Create `config.py` file  
+Always keep credentials in a separate file
+```python
+login_id = "XXXXX"
+password = "XXXXXXXX"
+Totp = 'XXXXXXXXXXXXXXXX'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print('Exception occurred :: {}'.format(e))
+    access_token = None
+```
+
+3. Import the config
+```python
+import config
+```
+
+### Create AlphaTrade Object
+
+1. Create `AlphaTrade` object with your `login_id`, `password`, `TOTP` / `TOTP_SECRET` and/or `access_token`.
+
+Use `config` object to get `login_id`, `password`, `TOTP` and `access_token`.  
+
+```python
+from alphatrade import AlphaTrade
+import config
+import pyotp
+Totp = config.Totp
+pin = pyotp.TOTP(Totp).now()
+totp = f"{int(pin):06d}" if len(pin) <=5 else pin   
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=totp, access_token=config.access_token)
+
+```
+
+```python
+## filename config.py
+
+login_id = "RR24XX"
+password = "SuperSecretPassword!!!"
+TOTP_SECRET = 'YOURTOTPSECRETEXTERNALAUTH'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print(f'Exception occurred :: {e}')
+    access_token = None
+
+```
+
+
+```python
+from alphatrade import AlphaTrade
+import config
+import pyotp
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.TOTP_SECRET, access_token=config.access_token)
+
+```
+
+
+2. You can run commands here to check your connectivity
+
+```python
+print(sas.get_balance()) # get balance / margin limits
+print(sas.get_profile()) # get profile
+print(sas.get_daywise_positions()) # get daywise positions
+print(sas.get_netwise_positions()) # get netwise positions
+print(sas.get_holding_positions()) # get holding positions
+```
+
+### Get master contracts
+
+Getting master contracts allow you to search for instruments by symbol name and place orders.
+Master contracts are stored as an OrderedDict by token number and by symbol name. Whenever you get a trade update, order update, or quote update, the library will check if master contracts are loaded. If they are, it will attach the instrument object directly to the update. By default all master contracts of all enabled exchanges in your personal profile will be downloaded. i.e. If your profile contains the following as enabled exchanges `['NSE', 'BSE', 'CDS', 'MCX', NFO']` all contract notes of all exchanges will be downloaded by default. If you feel it takes too much time to download all exchange, or if you don‘t need all exchanges to be downloaded, you can specify which exchange to download contract notes while creating the AlphaTrade object.
+
+```python
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=totp, access_token=config.access_token, master_contracts_to_download=['NSE', 'BSE'])
+```
+
+This will reduce a few milliseconds in object creation time of AlphaTrade object.
+
+### Get tradable instruments
+
+Symbols can be retrieved in multiple ways. Once you have the master contract loaded for an exchange, you can get an instrument in many ways.
+
+Get a single instrument by it‘s name:
+
+```python
+tatasteel_nse_eq = sas.get_instrument_by_symbol('NSE', 'TATASTEEL')
+reliance_nse_eq = sas.get_instrument_by_symbol('NSE', 'RELIANCE')
+ongc_bse_eq = sas.get_instrument_by_symbol('BSE', 'ONGC')
+india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
+sensex_nse_index = sas.get_instrument_by_symbol('BSE', 'SENSEX')
+```
+
+Get a single instrument by it‘s token number (generally useful only for BSE Equities):
+
+```python
+ongc_bse_eq = sas.get_instrument_by_token('BSE', 500312)
+reliance_bse_eq = sas.get_instrument_by_token('BSE', 500325)
+acc_nse_eq = sas.get_instrument_by_token('NSE', 22)
+```
+
+Get FNO instruments easily by mentioning expiry, strike & call or put.
+
+```python
+bn_fut = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=True, strike=None, is_call = False)
+bn_call = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = True)
+bn_put = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = False)
+```
+
+### Search for symbols
+
+Search for multiple instruments by matching the name. This works case insensitive and returns all instrument which has the name in its symbol.
+
+```python
+all_sensex_scrips = sas.search_instruments('BSE', 'sEnSeX')
+print(all_sensex_scrips)
+```
+
+The above code results multiple symbol which has ‘sensex’ in its symbol.
+
+```
+[Instrument(exchange='BSE', token=1, symbol='SENSEX', name='SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=540154, symbol='IDFSENSEXE B', name='IDFC Mutual Fund', expiry=None, lot_size=None), Instrument(exchange='BSE', token=532985, symbol='KTKSENSEX B', name='KOTAK MAHINDRA MUTUAL FUND', expiry=None, lot_size=None), Instrument(exchange='BSE', token=538683, symbol='NETFSENSEX B', name='NIPPON INDIA ETF SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=535276, symbol='SBISENSEX B', name='SBI MUTUAL FUND - SBI ETF SENS', expiry=None, lot_size=None)]
+```
+
+Search for multiple instruments by matching multiple names
+
+```python
+multiple_underlying = ['BANKNIFTY','NIFTY','INFY','BHEL']
+all_scripts = sas.search_instruments('NFO', multiple_underlying)
+```
+
+#### Instrument object
+
+Instruments are represented by instrument objects. These are named-tuples that are created while getting the master contracts. They are used when placing an order and searching for an instrument. The structure of an instrument tuple is as follows:
+
+```python
+Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
+                                      'name', 'expiry', 'lot_size'])
+```
+
+All instruments have the fields mentioned above. Wherever a field is not applicable for an instrument (for example, equity instruments don‘t have strike prices), that value will be `None`
+
+### Quote update
+
+Once you have master contracts loaded, you can easily subscribe to quote updates.
+
+#### Four types of feed data are available
+
+You can subscribe any one type of quote update for a given scrip. Using the `LiveFeedType` enum, you can specify what type of live feed you need.
+
+- `LiveFeedType.MARKET_DATA`
+- `LiveFeedType.COMPACT`
+- `LiveFeedType.SNAPQUOTE`
+- `LiveFeedType.FULL_SNAPQUOTE`
+
+Please refer to the original documentation [here](http://antplus.aliceblueonline.com/#marketdata) for more details of different types of quote update.
+
+#### Subscribe to a live feed
+
+```python
+sas.subscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
+sas.subscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
+```
+
+Subscribe to multiple instruments in a single call. Give an array of instruments to be subscribed.
+
+```python
+sas.subscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
+```
+
+Note: There is a limit of 250 scrips that can be subscribed on total. Beyond this point the server may disconnect web-socket connection.
+
+Start getting live feed via socket
+
+```python
+socket_opened = False
+def event_handler_quote_update(message):
+    print(f"quote update {message}")
+
+def open_callback():
+    global socket_opened
+    socket_opened = True
+
+sas.start_websocket(subscribe_callback=event_handler_quote_update,
+                      socket_open_callback=open_callback,
+                      run_in_background=True)
+while(socket_opened==False):
+    pass
+sas.subscribe(sas.get_instrument_by_symbol('NSE', 'ONGC'), LiveFeedType.MARKET_DATA)
+sleep(10)
+```
+
+#### Unsubscribe to a live feed
+
+Unsubscribe to an existing live feed
+
+```python
+sas.unsubscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
+sas.unsubscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
+```
+
+Unsubscribe to multiple instruments in a single call. Give an array of instruments to be unsubscribed.
+
+```python
+sas.unsubscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
+```
+
+#### Get All Subscribed Symbols
+
+```python
+sas.get_all_subscriptions() # All
+```
+
+### Market Status messages & Exchange messages.
+
+Subscribe to market status messages
+
+```python
+sas.subscribe_market_status_messages()
+```
+
+Getting market status messages.
+
+```python
+print(sas.get_market_status_messages())
+```
+
+Example result of `get_market_status_messages()`
+
+```
+[{'exchange': 'NSE', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 31, 'status': b'The Closing Session has closed.'}, {'exchange': 'NFO', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'CDS', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'BSE', 'length_of_market_type': 13, 'market_type': b'OTHER SESSION', 'length_of_status': 0, 'status': b''}]
+```
+
+Note: As per `alice blue` [documentation](http://antplus.aliceblueonline.com/#market-status) all market status messages should be having a timestamp. But in actual the server doesn‘t send timestamp, so the library is unable to get timestamp for now.
+
+Subscribe to exchange messages
+
+```python
+sas.subscribe_exchange_messages()
+```
+
+Getting market status messages.
+
+```python
+print(sas.get_exchange_messages())
+```
+
+Example result of `get_exchange_messages()`
+
+```
+[{'exchange': 'NSE', 'length': 32, 'message': b'DS : Bulk upload can be started.', 'exchange_time_stamp': 1590148595}, {'exchange': 'NFO', 'length': 200, 'message': b'MARKET WIDE LIMIT FOR VEDL IS 183919959. OPEN POSITIONS IN VEDL HAVE REACHED 84 PERCENT OF THE MARKET WIDE LIMIT.                                                                                       ', 'exchange_time_stamp': 1590146132}, {'exchange': 'CDS', 'length': 54, 'message': b'DS : Regular segment Bhav copy broadcast successfully.', 'exchange_time_stamp': 1590148932}, {'exchange': 'MCX', 'length': 7, 'message': b'.......', 'exchange_time_stamp': 1590196159}]
+```
+
+#### Market Status messages & Exchange messages through callbacks
+
+```python
+socket_opened = False
+def market_status_messages(message):
+    print(f"market status messages {message}")
+
+def exchange_messages(message):
+    print(f"exchange messages {message}")
+
+def open_callback():
+    global socket_opened
+    socket_opened = True
+
+sas.start_websocket(market_status_messages_callback=market_status_messages,
+					  exchange_messages_callback=exchange_messages,
+                      socket_open_callback=open_callback,
+                      run_in_background=True)
+while(socket_opened==False):
+    pass
+sas.subscribe_market_status_messages()
+sas.subscribe_exchange_messages()
+sleep(10)
+```
+
+### Place an order
+
+Place limit, market, SL, SL-M, AMO, BO, CO orders
+
+```python
+print (sas.get_profile())
+
+# TransactionType.Buy, OrderType.Market, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%1%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.Delivery,
+                     price = 0.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+   )
+
+# TransactionType.Buy, OrderType.Market, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%2%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.Intraday,
+                     price = 0.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+# TransactionType.Buy, OrderType.Market, ProductType.CoverOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%3%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.CoverOrder,
+                     price = 0.0,
+                     trigger_price = 7.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.Limit, ProductType.BracketOrder
+# OCO Order can't be of type market
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%4%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.BracketOrder,
+                     price = 8.0,
+                     trigger_price = None,
+                     stop_loss = 6.0,
+                     square_off = 10.0,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+# TransactionType.Buy, OrderType.Limit, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%5%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.Intraday,
+                     price = 8.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.Limit, ProductType.CoverOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%6%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.CoverOrder,
+                     price = 7.0,
+                     trigger_price = 6.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+###############################
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%7%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Delivery,
+                     price = 0.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%8%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Intraday,
+                     price = 0.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.CoverOrder
+# CO order is of type Limit and And Market Only
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.BO
+# BO order is of type Limit and And Market Only
+
+###################################
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%9%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Delivery,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%10%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossLimit,
+                     product_type = ProductType.Intraday,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.CoverOrder
+# CO order is of type Limit and And Market Only
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.BracketOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%11%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossLimit,
+                     product_type = ProductType.BracketOrder,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = 1.0,
+                     square_off = 1.0,
+                     trailing_sl = 20,
+                     is_amo = False)
+)
+```
+
+### Place basket order
+
+Basket order is used to buy or sell group of securities simultaneously.
+
+```python
+order1 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'INFY'),
+            "order_type"        : OrderType.Market,
+            "quantity"          : 1,
+            "transaction_type"  : TransactionType.Buy,
+            "product_type"      : ProductType.Delivery}
+order2 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'SBIN'),
+            "order_type"        : OrderType.Limit,
+            "quantity"          : 2,
+            "price"             : 280.0,
+            "transaction_type"  : TransactionType.Sell,
+            "product_type"      : ProductType.Intraday}
+order = [order1, order2]
+print(sas.place_basket_order(orders))
+```
+
+### Cancel an order
+
+```python
+sas.cancel_order('170713000075481') #Cancel an open order
+```
+
+### Getting order history and trade details
+
+#### Get order history of a particular order
+
+```python
+print(sas.get_order_history('170713000075481'))
+```
+
+#### Get order history of all orders.
+
+```python
+print(sas.get_order_history())
+```
+
+#### Get trade book
+
+```python
+print(sas.get_trade_book())
+```
+
+#### Get historical candles data
+
+This will provide historical data but **not for current day**.  
+This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
+
+```python
+from datetime import datetime
+print(sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', datetime(2020, 10, 19), datetime.now() ,interval=30))
+```
+
+Output 
+
+```console
+Instrument(exchange='MCX', token=224365, symbol='NATURALGAS NOV FUT', name='', expiry=datetime.date(2020, 11, 24), lot_size=None)
+                            open   high    low  close  volume
+date
+2020-10-19 09:00:00+05:30  238.9  239.2  238.4  239.0     373
+2020-10-19 09:30:00+05:30  239.0  239.0  238.4  238.6     210
+2020-10-19 10:00:00+05:30  238.7  238.7  238.1  238.1     213
+2020-10-19 10:30:00+05:30  238.0  238.4  238.0  238.1     116
+2020-10-19 11:00:00+05:30  238.1  238.2  238.0  238.0      69
+...                          ...    ...    ...    ...     ...
+2020-10-23 21:00:00+05:30  237.5  238.1  237.3  237.6     331
+2020-10-23 21:30:00+05:30  237.6  238.5  237.6  237.9     754
+2020-10-23 22:00:00+05:30  237.9  238.1  237.2  237.9     518
+2020-10-23 22:30:00+05:30  237.9  238.7  237.7  238.1     897
+2020-10-23 23:00:00+05:30  238.2  238.3  236.3  236.5    1906
+
+```
+
+Better way to get historical data, first get the latest version from github  
+
+`python -m pip install git+https://github.com/algo2t/alphatrade.git`
+
+```python
+from datetime import datetime
+india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
+print(sas.get_historical_candles(india_vix_nse_index.exchange, india_vix_nse_index.symbol, datetime(2020, 10, 19), datetime.now() ,interval=30))
+```
+
+
+#### Get intraday candles data
+
+This will give candles data for **current day only**.  
+This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
+
+```python
+print(sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', interval=15))
+```
+
+Better way to get intraday data, first get the latest version from github  
+
+`python -m pip install git+https://github.com/algo2t/alphatrade.git`
+
+```python
+from datetime import datetime
+nifty_bank_nse_index = sas.get_instrument_by_symbol('NSE', 'Nifty Bank')
+print(sas.get_intraday_candles(nifty_bank_nse_index.exchange, nifty_bank_nse_index.symbol, datetime(2020, 10, 19), datetime.now(), interval=10))
+```
+
+### Order properties as enums
+
+Order properties such as TransactionType, OrderType, and others have been safely classified as enums so you don‘t have to write them out as strings
+
+#### TransactionType
+
+Transaction types indicate whether you want to buy or sell. Valid transaction types are of the following:
+
+- `TransactionType.Buy` - buy
+- `TransactionType.Sell` - sell
+
+#### OrderType
+
+Order type specifies the type of order you want to send. Valid order types include:
+
+- `OrderType.Market` - Place the order with a market price
+- `OrderType.Limit` - Place the order with a limit price (limit price parameter is mandatory)
+- `OrderType.StopLossLimit` - Place as a stop loss limit order
+- `OrderType.StopLossMarket` - Place as a stop loss market order
+
+#### ProductType
+
+Product types indicate the complexity of the order you want to place. Valid product types are:
+
+- `ProductType.Intraday` - Intraday order that will get squared off before market close
+- `ProductType.Delivery` - Delivery order that will be held with you after market close
+- `ProductType.CoverOrder` - Cover order
+- `ProductType.BracketOrder` - One cancels other order. Also known as bracket order
+
+## Working with examples
+
+[Here](https://github.com/algo2t/alphatrade), examples directory there are 3 files `zlogin_example.py`, `zstreaming_data.py` and `stop.txt`
+
+### Steps
+
+- Clone the repository to your local machine `git clone https://github.com/algo2t/alphatrade.git`
+- Copy the examples directory to any location where you want to write your code
+- Install the `alphatrade` module using `pip` => `python -m pip install https://github.com/algo2t/alphatrade.git`
+- Open the examples directory in your favorite editor, in our case it is [VSCodium](https://vscodium.com/)
+- Open the `zlogin_example.py` file in the editor
+- Now, create `config.py` file as per instructions given below and in the above file
+- Provide correct login credentials like login_id, password and 16 digit totp code (find below qr code)
+- This is generally set from the homepage of alpha web trading platform [here](https://alpha.sasonline.in/)
+- Click on `FORGET PASSWORD?` => Select `Reset 2FA` radio button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/forget_password.png)
+- Enter the CLIENT ID (LOGIN_ID), EMAIL ID and PAN NUMBER, click on `RESET` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/reset_two_fa.png)
+- Click on `BACK TO LOGIN` and enter `CLIENT ID` and `PASSWORD`, click on `SECURED SIGN-IN`
+- Set same answers for 5 questions and click on `SUBMIT` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/set_answers.png)
+
+`config.py`
+```python
+login_id = "XXXXX"
+password = "XXXXXXXX"
+Totp = 'XXXXXXXXXXXXXXXX'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print('Exception occurred :: {}'.format(e))
+    access_token = None
+```
+
+## Example strategy using alpha trade API
+
+[Here](https://github.com/algo2t/alphatrade/blob/main/zstreaming_data.py) is an example moving average strategy using alpha trade web API.
+This strategy generates a buy signal when 5-EMA > 20-EMA (golden cross) or a sell signal when 5-EMA < 20-EMA (death cross).
+
+## Example for getting historical and intraday candles data
+
+[Here](https://github.com/algo2t/alphatrade/blob/main/zhistorical_data.py) is an example for getting historical data using alpha trade web API.
+
+For historical candles data `start_time` and `end_time` must be provided in format as shown below.
+It can also be provided as `timedelta`. Check the script `zhistorical_data.py` in examples.
+
+```python
+from datetime import datetime, timedelta
+start_time = datetime(2020, 10, 19, 9, 15, 0)
+end_time = datetime(2020, 10, 21, 16, 59, 0)
+
+df = sas.get_historical_candles('MCX', 'NATURALGAS OCT FUT', start_time, end_time, 5)
+print(df)
+end_time = start_time + timedelta(days=5)
+df = sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', start_time, end_time, 15)
+print(df)
+```
+
+For intraday or today‘s / current day‘s candles data.  
+
+```python
+df = sas.get_intraday_candles('MCX', 'NATURALGAS OCT FUT')
+print(df)
+df = sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', 15)
+print(df)
+```
+
+
+## Read this before creating an issue
+
+Before creating an issue in this library, please follow the following steps.
+
+1. Search the problem you are facing is already asked by someone else. There might be some issues already there, either solved/unsolved related to your problem. Go to [issues](https://github.com/algo2t/alphatrade/issues) page, use `is:issue` as filter and search your problem. ![image](https://user-images.githubusercontent.com/38440742/85207058-376ee400-b2f4-11ea-91ad-c8fd8a682a12.png)
+2. If you feel your problem is not asked by anyone or no issues are related to your problem, then create a new issue.
+3. Describe your problem in detail while creating the issue. If you don‘t have time to detail/describe the problem you are facing, assume that I also won‘t be having time to respond to your problem.
+4. Post a sample code of the problem you are facing. If I copy paste the code directly from issue, I should be able to reproduce the problem you are facing.
+5. Before posting the sample code, test your sample code yourself once. Only sample code should be tested, no other addition should be there while you are testing.
+6. Have some print() function calls to display the values of some variables related to your problem.
+7. Post the results of print() functions also in the issue.
+8. Use the insert code feature of github to inset code and print outputs, so that the code is displayed neat. ![image](https://user-images.githubusercontent.com/38440742/85207234-4dc96f80-b2f5-11ea-990c-df013dd69cf2.png)
```

### Comparing `alphatrade-0.1.3/alphatrade/alphatrade.py` & `alphatrade-1.0.0/alphatrade/alphatrade.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1216 +1,1255 @@
-import json
-import requests
-import threading
-import websocket
-import logging
-import enum
-from datetime import datetime, timedelta, date
-from time import sleep
-from collections import OrderedDict
-from protlib import CUInt, CStruct, CULong, CUChar, CArray, CUShort, CString
-from collections import namedtuple
-import pandas as pd
-import pytz
-import alphatrade.exceptions as ex
-
-
-Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
-                                       'name', 'expiry', 'lot_size'])
-logger = logging.getLogger(__name__)
-
-
-class Requests(enum.Enum):
-    PUT = 1
-    DELETE = 2
-    GET = 3
-    POST = 4
-
-
-class TransactionType(enum.Enum):
-    Buy = 'BUY'
-    Sell = 'SELL'
-
-
-class OrderType(enum.Enum):
-    Market = 'MARKET'
-    Limit = 'LIMIT'
-    StopLossLimit = 'SL'
-    StopLossMarket = 'SL-M'
-
-
-class ProductType(enum.Enum):
-    Intraday = 'I'
-    Delivery = 'D'
-    CoverOrder = 'CO'
-    BracketOrder = 'BO'
-
-
-class LiveFeedType(enum.Enum):
-    MARKET_DATA = 1
-    COMPACT = 2
-    SNAPQUOTE = 3
-    FULL_SNAPQUOTE = 4
-
-
-class WsFrameMode(enum.IntEnum):
-    MARKETDATA = 1
-    COMPACT_MARKETDATA = 2
-    SNAPQUOTE = 3
-    FULL_SNAPQUOTE = 4
-    SPREADDATA = 5
-    SPREAD_SNAPQUOTE = 6
-    DPR = 7
-    OI = 8
-    MARKET_STATUS = 9
-    EXCHANGE_MESSAGES = 10
-
-
-class MarketData(CStruct):
-    exchange = CUChar()
-    token = CUInt()
-    ltp = CUInt()
-    ltt = CUInt()
-    ltq = CUInt()
-    volume = CUInt()
-    best_bid_price = CUInt()
-    best_bid_quantity = CUInt()
-    best_ask_price = CUInt()
-    best_ask_quantity = CUInt()
-    total_buy_quantity = CULong()
-    total_sell_quantity = CULong()
-    atp = CUInt()
-    exchange_time_stamp = CUInt()
-    open = CUInt()
-    high = CUInt()
-    low = CUInt()
-    close = CUInt()
-    yearly_high = CUInt()
-    yearly_low = CUInt()
-
-
-class CompactData(CStruct):
-    exchange = CUChar()
-    token = CUInt()
-    ltp = CUInt()
-    change = CUInt()
-    exchange_time_stamp = CUInt()
-    volume = CUInt()
-
-
-class SnapQuote(CStruct):
-    exchange = CUChar()
-    token = CUInt()
-    buyers = CArray(5, CUInt)
-    bid_prices = CArray(5, CUInt)
-    bid_quantities = CArray(5, CUInt)
-    sellers = CArray(5, CUInt)
-    ask_prices = CArray(5, CUInt)
-    ask_quantities = CArray(5, CUInt)
-    exchange_time_stamp = CUInt()
-
-
-class FullSnapQuote(CStruct):
-    exchange = CUChar()
-    token = CUInt()
-    buyers = CArray(5, CUInt)
-    bid_prices = CArray(5, CUInt)
-    bid_quantities = CArray(5, CUInt)
-    sellers = CArray(5, CUInt)
-    ask_prices = CArray(5, CUInt)
-    ask_quantities = CArray(5, CUInt)
-    atp = CUInt()
-    open = CUInt()
-    high = CUInt()
-    low = CUInt()
-    close = CUInt()
-    total_buy_quantity = CULong()
-    total_sell_quantity = CULong()
-    volume = CUInt()
-
-
-class DPR(CStruct):
-    exchange = CUChar()
-    token = CUInt()
-    exchange_time_stamp = CUInt()
-    high = CUInt()
-    low = CUInt()
-
-
-class OpenInterest(CStruct):
-    exchange = CUChar()
-    token = CUInt()
-    current_open_interest = CUChar()
-    initial_open_interest = CUChar()
-    exchange_time_stamp = CUInt()
-
-
-class ExchangeMessage(CStruct):
-    exchange = CUChar()
-    length = CUShort()
-    message = CString(length="length")
-    exchange_time_stamp = CUInt()
-
-
-class MarketStatus(CStruct):
-    exchange = CUChar()
-    length_of_market_type = CUShort()
-    market_type = CString(length="length_of_market_type")
-    length_of_status = CUShort()
-    status = CString(length="length_of_status")
-
-
-class AlphaTrade(object):
-    # dictionary object to hold settings
-    __service_config = {
-        'host': 'https://alpha.sasonline.in',
-        'routes': {
-            'login': '/api/v2/login',
-            'checktwofa': '/api/v2/checktwofa',
-            'profile': '/api/v2/profile',
-            'master_contract': '/api/v2/contracts.json?exchanges={exchange}',
-            'holdings': '/api/v2/holdings',
-            'balance': '/api/v2/cashposition',
-            'positions_daywise': '/api/v2/positions?type=daywise',
-            'positions_netwise': '/api/v2/positions?type=netwise',
-            'positions_holdings': '/api/v2/holdings',
-            'place_order': '/api/v2/order',
-            'place_amo': '/api/v2/amo',
-            'place_bracket_order': '/api/v2/bracketorder',
-            'place_basket_order': '/api/v2/basketorder',
-            'get_orders': '/api/v2/order',
-            'get_order_info': '/api/v2/order/{order_id}',
-            'modify_order': '/api/v2/order',
-            'cancel_order': '/api/v2/order?oms_order_id={order_id}&order_status=open',
-            'cancel_bo_order': '/api/v2/order?oms_order_id={order_id}&order_status=open&leg_order_indicator={leg_order_id}',
-            'cancel_co_order': '/api/v2/coverorder?oms_order_id={order_id}&order_status=open&leg_order_indicator={leg_order_id}',
-            'trade_book': '/api/v2/trade',
-            'scripinfo': '/api/v2/scripinfo?exchange={exchange}&instrument_token={token}',
-        },
-        'socket_endpoint': 'wss://alpha.sasonline.in/hydrasocket/v2/websocket?access_token={access_token}'
-    }
-
-    _candletype = {1: 1, 2: 1, 3: 1, 5: 1, 10: 1, 15: 1,
-                   30: 1, 45: 1, '1H': 2, '2H': 2, '3H': 2, '4H': 2, '1D': 3, 'D': 3, 'W': 3, 'M': 3}
-
-    _data_duration = {1: 1, 2: 2, 3: 3, 5: 5, 10: 10, 15: 15,
-                      30: 30, 45: 45, '1H': None, '2H': 2, '3H': 2, '4H': 2, '1D': None, 'D': None, 'W': None, 'M': None}
-
-    def __init__(self, login_id, password, twofa, access_token=None, master_contracts_to_download=None):
-        """ logs in and gets enabled exchanges and products for user """
-        self.__access_token = access_token
-        self.__login_id = login_id
-        self.__password = password
-        self.__twofa = twofa
-        self.__websocket = None
-        self.__websocket_connected = False
-        self.__ws_mutex = threading.Lock()
-        self.__on_error = None
-        self.__on_disconnect = None
-        self.__on_open = None
-        self.__subscribe_callback = None
-        self.__order_update_callback = None
-        self.__market_status_messages_callback = None
-        self.__exchange_messages_callback = None
-        self.__oi_callback = None
-        self.__dpr_callback = None
-        self.__subscribers = {}
-        self.__market_status_messages = []
-        self.__exchange_messages = []
-        self.__exchange_codes = {'NSE': 1,
-                                 'NFO': 2,
-                                 'CDS': 3,
-                                 'MCX': 4,
-                                 'BSE': 6,
-                                 'BFO': 7}
-        self.__exchange_price_multipliers = {1: 100,
-                                             2: 100,
-                                             3: 10000000,
-                                             4: 100,
-                                             6: 100,
-                                             7: 100}
-
-        self.__headers = {
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.102 Safari/537.36'
-        }
-
-        self.reqsession = requests.session()
-
-        if not self.__is_token_valid():
-            self.__get_question_ids()
-            self.__set_access_token()
-        else:
-            self.__headers['X-Authorization-Token'] = self.__access_token
-
-        try:
-            profile = self.get_profile()
-        except Exception as e:
-            raise ex.PermissionException(
-                f"Couldn't get profile info with credentials provided '{e}'")
-        if(profile['status'] == 'error'):
-            # Don't know why this error comes, but it safe to proceed further.
-            if(profile['message'] == 'Not able to retrieve AccountInfoService'):
-                logger.warning(
-                    "Couldn't get profile info - 'Not able to retrieve AccountInfoService'")
-            else:
-                raise ex.PermissionException(
-                    f"Couldn't get profile info '{profile['message']}'")
-        self.__master_contracts_by_token = {}
-        self.__master_contracts_by_symbol = {}
-        if(master_contracts_to_download == None):
-            for e in self.__enabled_exchanges:
-                self.__get_master_contract(e)
-        else:
-            for e in master_contracts_to_download:
-                self.__get_master_contract(e)
-        self.ws_thread = None
-
-    def __is_token_valid(self):
-        if self.__access_token is None:
-            try:
-                self.__access_token = open(
-                    'access_token.txt', 'r').read().rstrip()
-            except Exception as e:
-                print('Exception occurred :: {}'.format(e))
-                self.__access_token = None
-        self.__headers['X-Authorization-Token'] = self.__access_token
-        profile_url = 'https://alpha.sasonline.in/api/v2/profile'
-
-        resp = self.reqsession.get(profile_url, headers=self.__headers)
-        return resp.status_code == 200 and resp.json()['status'] == 'success'
-
-    def __get_question_ids(self):
-        login_body = {
-            "device": "web",
-            'login_id': self.__login_id,
-            'password': self.__password
-        }
-        response = self.reqsession.post(
-            'https://alpha.sasonline.in/api/v2/login', json=login_body)
-
-        if response.status_code != 200:
-            raise requests.HTTPError(response.text)
-        if 'error' in response.text:
-            raise requests.HTTPError(response.text)
-        question_ids = response.json()['data']['question_ids']
-
-        self.__question_ids = question_ids
-
-    def __set_access_token(self):
-        twofa_body = {
-            "device": "web",
-            "count": 2,
-            'answers': [self.__twofa, self.__twofa],
-            'login_id': self.__login_id,
-            'question_ids': self.__question_ids,
-        }
-        response = self.reqsession.post(
-            'https://alpha.sasonline.in/api/v2/checktwofa', json=twofa_body)
-        if response.status_code != 200:
-            raise requests.HTTPError(response.text)
-        if 'error' in response.text:
-            raise requests.HTTPError(response.text)
-        auth_token = response.json()['data']['auth_token']
-
-        with open('access_token.txt', 'w') as wr:
-            wr.write(auth_token)
-
-        self.__access_token = auth_token
-        self.__headers['X-Authorization-Token'] = self.__access_token
-
-    def __convert_prices(self, dictionary, multiplier):
-        keys = ['ltp',
-                'best_bid_price',
-                'best_ask_price',
-                'atp',
-                'open',
-                'high',
-                'low',
-                'close',
-                'yearly_high',
-                'yearly_low']
-        for key in keys:
-            if(key in dictionary):
-                dictionary[key] = dictionary[key]/multiplier
-        multiple_value_keys = ['bid_prices', 'ask_prices']
-        for key in multiple_value_keys:
-            if(key in dictionary):
-                new_values = []
-                for value in dictionary[key]:
-                    new_values.append(value/multiplier)
-                dictionary[key] = new_values
-        return dictionary
-
-    def __format_candles(self, data, divider=100):
-        records = data['data']
-        df = pd.DataFrame(records, columns=[
-            'date', 'open', 'high', 'low', 'close', 'volume'])  # , index=0)
-        df['date'] = df['date'].apply(
-            pd.Timestamp, unit='s', tzinfo=pytz.timezone('Asia/Kolkata'))
-        # df['datetime'] = df['datetime'].astype(str).str[:-6]
-        df[['open', 'high', 'low', 'close']] = df[[
-            'open', 'high', 'low', 'close']].astype(float).div(divider)
-        df['volume'] = df['volume'].astype(int)
-        df.set_index('date', inplace=True)
-        return df
-
-    def __convert_exchanges(self, dictionary):
-        if('exchange' in dictionary):
-            d = self.__exchange_codes
-            dictionary['exchange'] = list(d.keys())[list(
-                d.values()).index(dictionary['exchange'])]
-        return dictionary
-
-    def __convert_instrument(self, dictionary):
-        if('exchange' in dictionary) and ('token' in dictionary):
-            dictionary['instrument'] = self.get_instrument_by_token(
-                dictionary['exchange'], dictionary['token'])
-        return dictionary
-
-    def __modify_human_readable_values(self, dictionary):
-        dictionary = self.__convert_prices(
-            dictionary, self.__exchange_price_multipliers[dictionary['exchange']])
-        dictionary = self.__convert_exchanges(dictionary)
-        dictionary = self.__convert_instrument(dictionary)
-        return dictionary
-
-    def __on_data_callback(self, ws=None, message=None, data_type=None, continue_flag=None):
-        if(type(ws) is not websocket.WebSocketApp):  # This workaround is to solve the websocket_client's compatibility issue of older versions. ie.0.40.0 which is used in upstox. Now this will work in both 0.40.0 & newer version of websocket_client
-            message = ws
-        if(message[0] == WsFrameMode.MARKETDATA):
-            p = MarketData.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            if(self.__subscribe_callback is not None):
-                self.__subscribe_callback(res)
-        elif(message[0] == WsFrameMode.COMPACT_MARKETDATA):
-            p = CompactData.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            if(self.__subscribe_callback is not None):
-                self.__subscribe_callback(res)
-        elif(message[0] == WsFrameMode.SNAPQUOTE):
-            p = SnapQuote.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            if(self.__subscribe_callback is not None):
-                self.__subscribe_callback(res)
-        elif(message[0] == WsFrameMode.FULL_SNAPQUOTE):
-            p = FullSnapQuote.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            if(self.__subscribe_callback is not None):
-                self.__subscribe_callback(res)
-        elif(message[0] == WsFrameMode.DPR):
-            p = DPR.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            if(self.__dpr_callback is not None):
-                self.__dpr_callback(res)
-        elif(message[0] == WsFrameMode.OI):
-            p = OpenInterest.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            if(self.__oi_callback is not None):
-                self.__oi_callback(res)
-        elif(message[0] == WsFrameMode.MARKET_STATUS):
-            p = MarketStatus.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            self.__market_status_messages.append(res)
-            if(self.__market_status_messages_callback is not None):
-                self.__market_status_messages_callback(res)
-        elif(message[0] == WsFrameMode.EXCHANGE_MESSAGES):
-            p = ExchangeMessage.parse(message[1:]).__dict__
-            res = self.__modify_human_readable_values(p)
-            self.__exchange_messages.append(res)
-            if(self.__exchange_messages_callback is not None):
-                self.__exchange_messages_callback(res)
-
-    def __on_close_callback(self, ws=None):
-        self.__websocket_connected = False
-        if self.__on_disconnect:
-            self.__on_disconnect()
-
-    def __on_open_callback(self, ws=None):
-        self.__websocket_connected = True
-        self.__resubscribe()
-        if self.__on_open:
-            self.__on_open()
-
-    def __on_error_callback(self, ws=None, error=None):
-        if(type(ws) is not websocket.WebSocketApp):  # This workaround is to solve the websocket_client's compatibility issue of older versions. ie.0.40.0 which is used in upstox. Now this will work in both 0.40.0 & newer version of websocket_client
-            error = ws
-        if self.__on_error:
-            self.__on_error(error)
-
-    def __send_heartbeat(self):
-        heart_beat = {"a": "h", "v": [], "m": ""}
-        while True:
-            sleep(5)
-            self.__ws_send(json.dumps(heart_beat),
-                           opcode=websocket._abnf.ABNF.OPCODE_PING)
-
-    def __ws_run_forever(self):
-        while True:
-            try:
-                self.__websocket.run_forever()
-            except Exception as e:
-                logger.warning(
-                    f"websocket run forever ended in exception, {e}")
-            sleep(0.1)  # Sleep for 100ms between reconnection.
-
-    def __ws_send(self, *args, **kwargs):
-        while self.__websocket_connected == False:
-            # sleep for 50ms if websocket is not connected, wait for reconnection
-            sleep(0.05)
-        with self.__ws_mutex:
-            self.__websocket.send(*args, **kwargs)
-
-    def start_websocket(self, subscribe_callback=None,
-                        order_update_callback=None,
-                        socket_open_callback=None,
-                        socket_close_callback=None,
-                        socket_error_callback=None,
-                        run_in_background=False,
-                        market_status_messages_callback=None,
-                        exchange_messages_callback=None,
-                        oi_callback=None,
-                        dpr_callback=None):
-        """ Start a websocket connection for getting live data """
-        self.__on_open = socket_open_callback
-        self.__on_disconnect = socket_close_callback
-        self.__on_error = socket_error_callback
-        self.__subscribe_callback = subscribe_callback
-        self.__order_update_callback = order_update_callback
-        self.__market_status_messages_callback = market_status_messages_callback
-        self.__exchange_messages_callback = exchange_messages_callback
-        self.__oi_callback = oi_callback
-        self.__dpr_callback = dpr_callback
-
-        url = self.__service_config['socket_endpoint'].format(
-            access_token=self.__access_token)
-        self.__websocket = websocket.WebSocketApp(url,
-                                                  on_data=self.__on_data_callback,
-                                                  on_error=self.__on_error_callback,
-                                                  on_close=self.__on_close_callback,
-                                                  on_open=self.__on_open_callback)
-        th = threading.Thread(target=self.__send_heartbeat)
-        th.daemon = True
-        th.start()
-        if run_in_background is True:
-            self.__ws_thread = threading.Thread(target=self.__ws_run_forever)
-            self.__ws_thread.daemon = True
-            self.__ws_thread.start()
-        else:
-            self.__ws_run_forever()
-
-    def get_profile(self):
-        """ Get profile """
-        profile = self.__api_call_helper('profile', Requests.GET, None, None)
-        if(profile['status'] != 'error'):
-            self.__enabled_exchanges = profile['data']['exchanges']
-        return profile
-
-    def get_balance(self):
-        """ Get balance/margins """
-        return self.__api_call_helper('balance', Requests.GET, None, None)
-
-    def get_daywise_positions(self):
-        """ Get daywise positions """
-        return self.__api_call_helper('positions_daywise', Requests.GET, None, None)
-
-    def get_netwise_positions(self):
-        """ Get netwise positions """
-        return self.__api_call_helper('positions_netwise', Requests.GET, None, None)
-
-    def get_holding_positions(self):
-        """ Get holding positions """
-        return self.__api_call_helper('positions_holdings', Requests.GET, None, None)
-
-    def get_order_history(self, order_id=None):
-        """ leave order_id as None to get all entire order history """
-        if order_id is None:
-            return self.__api_call_helper('get_orders', Requests.GET, None, None)
-        else:
-            return self.__api_call_helper('get_order_info', Requests.GET, {'order_id': order_id}, None)
-
-    def get_scrip_info(self, instrument):
-        """ Get scrip information """
-        params = {'exchange': instrument.exchange, 'token': instrument.token}
-        return self.__api_call_helper('scripinfo', Requests.GET, params, None)
-
-    def get_trade_book(self):
-        """ get all trades """
-        return self.__api_call_helper('trade_book', Requests.GET, None, None)
-
-    def get_exchanges(self):
-        """ Get enabled exchanges """
-        return self.__enabled_exchanges
-
-    def __get_product_type_str(self, product_type, exchange):
-        prod_type = None
-        if (product_type == ProductType.Intraday):
-            prod_type = 'MIS'
-        elif product_type == ProductType.Delivery:
-            prod_type = 'NRML' if exchange in ['NFO', 'MCX', 'CDS'] else 'CNC'
-        elif(product_type == ProductType.CoverOrder):
-            prod_type = 'CO'
-        elif(product_type == ProductType.BracketOrder):
-            prod_type = None
-        return prod_type
-
-    def place_order(self, transaction_type, instrument, quantity, order_type,
-                    product_type, price=0.0, trigger_price=None,
-                    stop_loss=None, square_off=None, trailing_sl=None,
-                    is_amo=False,
-                    order_tag='python'):
-        """ placing an order, many fields are optional and are not required
-            for all order types
-        """
-        if transaction_type is None:
-            raise TypeError(
-                "Required parameter transaction_type not of type TransactionType")
-
-        if not isinstance(instrument, Instrument):
-            raise TypeError(
-                "Required parameter instrument not of type Instrument")
-
-        if not isinstance(quantity, int):
-            raise TypeError("Required parameter quantity not of type int")
-
-        if order_type is None:
-            raise TypeError(
-                "Required parameter order_type not of type OrderType")
-
-        if product_type is None:
-            raise TypeError(
-                "Required parameter product_type not of type ProductType")
-
-        if price is not None and not isinstance(price, float):
-            raise TypeError("Optional parameter price not of type float")
-
-        if trigger_price is not None and not isinstance(trigger_price, float):
-            raise TypeError(
-                "Optional parameter trigger_price not of type float")
-
-        prod_type = self.__get_product_type_str(
-            product_type, instrument.exchange)
-        # construct order object after all required parameters are met
-        order = {'exchange': instrument.exchange,
-                 'order_type': order_type.value,
-                 'instrument_token': instrument.token,
-                 'quantity': quantity,
-                 'disclosed_quantity': 0,
-                 'price': price,
-                 'transaction_type': transaction_type.value,
-                 'trigger_price': trigger_price,
-                 'validity': 'DAY',
-                 'product': prod_type,
-                 'source': 'web',
-                 'order_tag': order_tag}
-
-        if stop_loss is not None:
-            if isinstance(stop_loss, float):
-                order['stop_loss_value'] = stop_loss
-
-            else:
-                raise TypeError(
-                    "Optional parameter stop_loss not of type float")
-        if square_off is not None:
-            if isinstance(square_off, float):
-                order['square_off_value'] = square_off
-
-            else:
-                raise TypeError(
-                    "Optional parameter square_off not of type float")
-        if trailing_sl is not None:
-            if not isinstance(trailing_sl, int):
-                raise TypeError(
-                    "Optional parameter trailing_sl not of type int")
-            else:
-                order['trailing_stop_loss'] = trailing_sl
-
-        if product_type is ProductType.CoverOrder and not isinstance(
-            trigger_price, float
-        ):
-            raise TypeError(
-                "Required parameter trigger_price not of type float")
-
-        helper = 'place_amo' if (is_amo == True) else 'place_order'
-        if product_type is ProductType.BracketOrder:
-            helper = 'place_bracket_order'
-            del order['product']
-            if not isinstance(stop_loss, float):
-                raise TypeError(
-                    "Required parameter stop_loss not of type float")
-
-            if not isinstance(square_off, float):
-                raise TypeError(
-                    "Required parameter square_off not of type float")
-
-        return self.__api_call_helper(helper, Requests.POST, None, order)
-
-    def place_basket_order(self, orders):
-        """ placing a basket order, 
-            Argument orders should be a list of all orders that should be sent
-            each element in order should be a dictionary containing the following key.
-            "instrument", "order_type", "quantity", "price" (only if its a limit order), 
-            "transaction_type", "product_type"
-        """
-        keys = {"instrument": Instrument,
-                "order_type": OrderType,
-                "quantity": int,
-                "transaction_type": TransactionType,
-                "product_type": ProductType}
-        if not isinstance(orders, list):
-            raise TypeError("Required parameter orders is not of type list")
-
-        if len(orders) <= 0:
-            raise TypeError("Length of orders should be greater than 0")
-
-        for i in orders:
-            if not isinstance(i, dict):
-                raise TypeError(
-                    "Each element in orders should be of type dict")
-            for s, value in keys.items():
-                if s not in i:
-                    raise TypeError(
-                        f"Each element in orders should have key {s}")
-                if type(i[s]) is not value:
-                    raise TypeError(
-                        f"Element '{s}' in orders should be of type {keys[s]}")
-            if i['order_type'] == OrderType.Limit:
-                if "price" not in i:
-                    raise TypeError(
-                        "Each element in orders should have key 'price' if its a limit order ")
-                if not isinstance(i['price'], float):
-                    raise TypeError(
-                        "Element price in orders should be of type float")
-            else:
-                i['price'] = 0.0
-            if i['order_type'] in [
-                OrderType.StopLossLimit,
-                OrderType.StopLossMarket,
-            ]:
-                if 'trigger_price' not in i:
-                    raise TypeError(
-                        f"Each element in orders should have key 'trigger_price' if it is an {i['order_type']} order")
-                if not isinstance(i['trigger_price'], float):
-                    raise TypeError(
-                        "Element trigger_price in orders should be of type float")
-            else:
-                i['trigger_price'] = 0.0
-            if (i['product_type'] == ProductType.Intraday):
-                i['product_type'] = 'MIS'
-            elif i['product_type'] == ProductType.Delivery:
-                i['product_type'] = 'NRML' if (
-                    i['instrument'].exchange == 'NFO') else 'CNC'
-            elif i['product_type'] in [
-                ProductType.CoverOrder,
-                ProductType.BracketOrder,
-            ]:
-                raise TypeError(
-                    "Product Type BO or CO is not supported in basket order")
-            if i['quantity'] <= 0:
-                raise TypeError("Quantity should be greater than 0")
-
-        data = {'source': 'web',
-                'orders': []}
-        for i in orders:
-            # construct order object after all required parameters are met
-            data['orders'].append({'exchange': i['instrument'].exchange,
-                                   'order_type': i['order_type'].value,
-                                   'instrument_token': i['instrument'].token,
-                                   'quantity': i['quantity'],
-                                   'disclosed_quantity': 0,
-                                   'price': i['price'],
-                                   'transaction_type': i['transaction_type'].value,
-                                   'trigger_price': i['trigger_price'],
-                                   'validity': 'DAY',
-                                   'product': i['product_type']})
-
-        helper = 'place_basket_order'
-        return self.__api_call_helper(helper, Requests.POST, None, data)
-
-    def modify_order(self, transaction_type, instrument, product_type, order_id, order_type, quantity=None, price=0.0,
-                     trigger_price=0.0):
-        """ modify an order, transaction_type, instrument, product_type, order_id & order_type is required, 
-            rest are optional, use only when when you want to change that attribute.
-        """
-        if not isinstance(instrument, Instrument):
-            raise TypeError(
-                "Required parameter instrument not of type Instrument")
-
-        if not isinstance(order_id, str):
-            raise TypeError("Required parameter order_id not of type str")
-
-        if quantity is not None and not isinstance(quantity, int):
-            raise TypeError("Optional parameter quantity not of type int")
-
-        if type(order_type) is not OrderType:
-            raise TypeError(
-                "Optional parameter order_type not of type OrderType")
-
-        if ProductType is None:
-            raise TypeError(
-                "Required parameter product_type not of type ProductType")
-
-        if price is not None and not isinstance(price, float):
-            raise TypeError("Optional parameter price not of type float")
-
-        if trigger_price is not None and not isinstance(trigger_price, float):
-            raise TypeError(
-                "Optional parameter trigger_price not of type float")
-
-        if (product_type == ProductType.Intraday):
-            product_type = 'MIS'
-        elif product_type == ProductType.Delivery:
-            product_type = 'NRML' if (instrument.exchange == 'NFO') else 'CNC'
-        elif(product_type == ProductType.CoverOrder):
-            product_type = 'CO'
-        elif(product_type == ProductType.BracketOrder):
-            product_type = None
-        # construct order object with order id
-        order = {'oms_order_id': str(order_id),
-                 'instrument_token': int(instrument.token),
-                 'exchange': instrument.exchange,
-                 'transaction_type': transaction_type.value,
-                 'product': product_type,
-                 'validity': 'DAY',
-                 'order_type': order_type.value,
-                 'price': price,
-                 'trigger_price': trigger_price,
-                 'quantity': quantity,
-                 'disclosed_quantity': 0,
-                 'nest_request_id': '1'}
-        return self.__api_call_helper('modify_order', Requests.PUT, None, order)
-
-    def cancel_order(self, order_id, leg_order_id=None, is_co=False):
-        """ Cancel single order """
-        if (is_co == False):
-            if leg_order_id is None:
-                ret = self.__api_call_helper('cancel_order', Requests.DELETE, {
-                                             'order_id': order_id}, None)
-            else:
-                ret = self.__api_call_helper('cancel_bo_order', Requests.DELETE, {
-                                             'order_id': order_id, 'leg_order_id': leg_order_id}, None)
-        else:
-            ret = self.__api_call_helper('cancel_co_order', Requests.DELETE, {
-                                         'order_id': order_id, 'leg_order_id': leg_order_id}, None)
-        return ret
-
-    def cancel_all_orders(self):
-        """ Cancel all orders """
-        ret = []
-        orders = self.get_order_history()['data']
-        if not orders:
-            return
-        for c_order in orders['pending_orders']:
-            if(c_order['product'] == 'BO' and c_order['leg_order_indicator']):
-                r = self.cancel_order(
-                    c_order['leg_order_indicator'], leg_order_id=c_order['leg_order_indicator'])
-            elif(c_order['product'] == 'CO'):
-                r = self.cancel_order(
-                    c_order['oms_order_id'], leg_order_id=c_order['leg_order_indicator'], is_co=True)
-            else:
-                r = self.cancel_order(c_order['oms_order_id'])
-            ret.append(r)
-        return ret
-
-    def subscribe_market_status_messages(self):
-        """ Subscribe to market messages """
-        return self.__ws_send(json.dumps({"a": "subscribe", "v": [1, 2, 3, 4, 6], "m": "market_status"}))
-
-    def get_market_status_messages(self):
-        """ Get market messages """
-        return self.__market_status_messages
-
-    def subscribe_exchange_messages(self):
-        """ Subscribe to exchange messages """
-        return self.__ws_send(json.dumps({"a": "subscribe", "v": [1, 2, 3, 4, 6], "m": "exchange_messages"}))
-
-    def get_exchange_messages(self):
-        """ Get stored exchange messages """
-        return self.__exchange_messages
-
-    def subscribe(self, instrument, live_feed_type):
-        """ subscribe to the current feed of an instrument """
-        if(type(live_feed_type) is not LiveFeedType):
-            raise TypeError(
-                "Required parameter live_feed_type not of type LiveFeedType")
-        arr = []
-        if (isinstance(instrument, list)):
-            for _instrument in instrument:
-                if not isinstance(_instrument, Instrument):
-                    raise TypeError(
-                        "Required parameter instrument not of type Instrument")
-                exchange = self.__exchange_codes[_instrument.exchange]
-                arr.append([exchange, int(_instrument.token)])
-                self.__subscribers[_instrument] = live_feed_type
-        else:
-            if not isinstance(instrument, Instrument):
-                raise TypeError(
-                    "Required parameter instrument not of type Instrument")
-            exchange = self.__exchange_codes[instrument.exchange]
-            arr = [[exchange, int(instrument.token)]]
-            self.__subscribers[instrument] = live_feed_type
-        if(live_feed_type == LiveFeedType.MARKET_DATA):
-            mode = 'marketdata'
-        elif(live_feed_type == LiveFeedType.COMPACT):
-            mode = 'compact_marketdata'
-        elif(live_feed_type == LiveFeedType.SNAPQUOTE):
-            mode = 'snapquote'
-        elif(live_feed_type == LiveFeedType.FULL_SNAPQUOTE):
-            mode = 'full_snapquote'
-        data = json.dumps({'a': 'subscribe', 'v': arr, 'm': mode})
-        return self.__ws_send(data)
-
-    def unsubscribe(self, instrument, live_feed_type):
-        """ unsubscribe to the current feed of an instrument """
-        if(type(live_feed_type) is not LiveFeedType):
-            raise TypeError(
-                "Required parameter live_feed_type not of type LiveFeedType")
-        arr = []
-        if (isinstance(instrument, list)):
-            for _instrument in instrument:
-                if not isinstance(_instrument, Instrument):
-                    raise TypeError(
-                        "Required parameter instrument not of type Instrument")
-                exchange = self.__exchange_codes[_instrument.exchange]
-                arr.append([exchange, int(_instrument.token)])
-                if(_instrument in self.__subscribers):
-                    del self.__subscribers[_instrument]
-        else:
-            if not isinstance(instrument, Instrument):
-                raise TypeError(
-                    "Required parameter instrument not of type Instrument")
-            exchange = self.__exchange_codes[instrument.exchange]
-            arr = [[exchange, int(instrument.token)]]
-            if(instrument in self.__subscribers):
-                del self.__subscribers[instrument]
-        if(live_feed_type == LiveFeedType.MARKET_DATA):
-            mode = 'marketdata'
-        elif(live_feed_type == LiveFeedType.COMPACT):
-            mode = 'compact_marketdata'
-        elif(live_feed_type == LiveFeedType.SNAPQUOTE):
-            mode = 'snapquote'
-        elif(live_feed_type == LiveFeedType.FULL_SNAPQUOTE):
-            mode = 'full_snapquote'
-
-        data = json.dumps({'a': 'unsubscribe', 'v': arr, 'm': mode})
-        return self.__ws_send(data)
-
-    def get_all_subscriptions(self):
-        """ get the all subscribed instruments """
-        return self.__subscribers
-
-    def __resubscribe(self):
-        market = []
-        compact = []
-        snap = []
-        full = []
-        for key, value in self.get_all_subscriptions().items():
-            if(value == LiveFeedType.MARKET_DATA):
-                market.append(key)
-            elif(value == LiveFeedType.COMPACT):
-                compact.append(key)
-            elif(value == LiveFeedType.SNAPQUOTE):
-                snap.append(key)
-            elif(value == LiveFeedType.FULL_SNAPQUOTE):
-                full.append(key)
-        if market:
-            self.subscribe(market, LiveFeedType.MARKET_DATA)
-        if compact:
-            self.subscribe(compact, LiveFeedType.COMPACT)
-        if snap:
-            self.subscribe(snap, LiveFeedType.SNAPQUOTE)
-        if full:
-            self.subscribe(full, LiveFeedType.FULL_SNAPQUOTE)
-
-    def get_instrument_by_symbol(self, exchange, symbol):
-        """ get instrument by providing symbol """
-        # get instrument given exchange and symbol
-        exchange = exchange.upper()
-        # check if master contract exists
-        if exchange not in self.__master_contracts_by_symbol:
-            logger.warning(f"Cannot find exchange {exchange} in master contract. "
-                           "Please ensure if that exchange is enabled in your profile and downloaded the master contract for the same")
-            return None
-        master_contract = self.__master_contracts_by_symbol[exchange]
-        if symbol not in master_contract:
-            logger.warning(
-                f"Cannot find symbol {exchange} {symbol} in master contract")
-            return None
-        return master_contract[symbol]
-
-    def get_instrument_for_fno(self, symbol, expiry_date, is_fut=False, strike=None, is_call=False, exchange='NFO'):
-        """ get instrument for FNO """
-        res = self.search_instruments(exchange, symbol)
-        if(res == None):
-            return
-        matches = []
-        for i in res:
-            sp = i.symbol.split(' ')
-            if(sp[0] == symbol):
-                if(i.expiry == expiry_date):
-                    matches.append(i)
-        for i in matches:
-            if(is_fut == True):
-                if('FUT' in i.symbol):
-                    return i
-            else:
-                sp = i.symbol.split(' ')
-                if((sp[-1] == 'CE') or (sp[-1] == 'PE')):           # Only option scrips
-                    if(float(sp[-2]) == float(strike)):
-                        if(is_call == True):
-                            if(sp[-1] == 'CE'):
-                                return i
-                        else:
-                            if(sp[-1] == 'PE'):
-                                return i
-
-    def search_instruments(self, exchange, symbol):
-        """ Search instrument by symbol match """
-        # search instrument given exchange and symbol
-        exchange = exchange.upper()
-        matches = []
-        # check if master contract exists
-        if exchange not in self.__master_contracts_by_token:
-            logger.warning(f"Cannot find exchange {exchange} in master contract. "
-                           "Please ensure if that exchange is enabled in your profile and downloaded the master contract for the same")
-            return None
-        master_contract = self.__master_contracts_by_token[exchange]
-        for contract in master_contract:
-            if (isinstance(symbol, list)):
-                for sym in symbol:
-                    if sym.lower() in master_contract[contract].symbol.split(' ')[0].lower():
-                        matches.append(master_contract[contract])
-            else:
-                if symbol.lower() in master_contract[contract].symbol.split(' ')[0].lower():
-                    matches.append(master_contract[contract])
-        return matches
-
-    def get_instrument_by_token(self, exchange, token):
-        """ Get instrument by providing token """
-        # get instrument given exchange and token
-        exchange = exchange.upper()
-        token = int(token)
-        # check if master contract exists
-        if exchange not in self.__master_contracts_by_symbol:
-            logger.warning(f"Cannot find exchange {exchange} in master contract. "
-                           "Please ensure if that exchange is enabled in your profile and downloaded the master contract for the same")
-            return None
-        master_contract = self.__master_contracts_by_token[exchange]
-        if token not in master_contract:
-            logger.warning(
-                f"Cannot find symbol {exchange} {token} in master contract")
-            return None
-        return master_contract[token]
-
-    def get_master_contract(self, exchange):
-        """ Get master contract """
-        return self.__master_contracts_by_symbol[exchange]
-
-    def __get_master_contract(self, exchange):
-        """ returns all the tradable contracts of an exchange
-            placed in an OrderedDict and the key is the token
-        """
-        logger.info(f'Downloading master contracts for exchange: {exchange}')
-        body = self.__api_call_helper('master_contract', Requests.GET, {
-                                      'exchange': exchange}, None)
-        master_contract_by_token = OrderedDict()
-        master_contract_by_symbol = OrderedDict()
-        for sub in body:
-            for scrip in body[sub]:
-                # convert token
-                token = int(scrip['code'])
-
-                # convert symbol to upper
-                symbol = scrip['symbol']
-
-                # convert expiry to none if it's non-existent
-                if('expiry' in scrip):
-                    expiry = datetime.fromtimestamp(
-                        scrip['expiry']).date()
-                else:
-                    expiry = None
-
-                # convert lot size to int
-                lot_size = scrip['lotSize'] if ('lotSize' in scrip) else None
-                # Name & Exchange
-                name = scrip['company']
-                exch = scrip['exchange']
-
-                instrument = Instrument(
-                    exch, token, symbol, name, expiry, lot_size)
-                master_contract_by_token[token] = instrument
-                master_contract_by_symbol[symbol] = instrument
-        self.__master_contracts_by_token[exchange] = master_contract_by_token
-        self.__master_contracts_by_symbol[exchange] = master_contract_by_symbol
-
-    def __api_call_helper(self, name, http_method, params, data):
-        # helper formats the url and reads error codes nicely
-        config = self.__service_config
-        url = f"{config['host']}{config['routes'][name]}"
-        if params is not None:
-            url = url.format(**params)
-        response = self.__api_call(url, http_method, data)
-        if response.status_code != 200:
-            raise requests.HTTPError(response.text)
-        return json.loads(response.text)
-
-    def __api_call(self, url, http_method, data):
-        # logger.debug('url:: %s http_method:: %s data:: %s headers:: %s', url, http_method, data, headers)
-        headers = {"Content-Type": "application/json"}
-        if(len(self.__access_token) > 100):
-            headers['X-Authorization-Token'] = self.__access_token
-            headers['Connection'] = 'keep-alive'
-        else:
-            headers['client_id'] = self.__login_id
-            headers['authorization'] = f"Bearer {self.__access_token}"
-        r = None
-        if http_method is Requests.POST:
-            r = self.reqsession.post(
-                url, data=json.dumps(data), headers=headers)
-        elif http_method is Requests.DELETE:
-            r = self.reqsession.delete(url, headers=headers)
-        elif http_method is Requests.PUT:
-            r = self.reqsession.put(
-                url, data=json.dumps(data), headers=headers)
-        elif http_method is Requests.GET:
-            r = self.reqsession.get(url, headers=headers)
-        return r
-
-    def get_historical_candles(self, exchange, symbol, start_time, end_time, interval=5, is_index=False):
-        exchange = exchange.upper()
-        idx = '' if not is_index else '_INDICES'
-        divider = 100
-        if exchange == 'CDS':
-            divider = 1e7
-        # symbol = symbol.upper()
-        instrument = self.get_instrument_by_symbol(exchange, symbol)
-        print(instrument)
-        start_time = int(start_time.timestamp())
-        end_time = int(end_time.timestamp())
-
-        PARAMS = {
-            'candletype': 1,
-            'data_duration': interval,
-            'starttime': start_time,
-            'endtime': end_time,
-            'exchange': exchange + idx,
-            'type': 'historical',
-            'token': instrument.token
-        }
-
-        r = self.reqsession.get(
-            'https://alpha.sasonline.in/api/v1/charts', params=PARAMS, headers=self.__headers)
-        data = r.json()
-        return self.__format_candles(data, divider)
-
-    def get_intraday_candles(self, exchange, symbol, interval=5):
-        exchange = exchange.upper()
-        divider = 100
-        if exchange == 'CDS':
-            divider = 1e7
-        # symbol = symbol.upper()
-        today = datetime.today()
-        start_time = int(datetime(today.year, today.month,
-                                  today.day, hour=9, minute=00).timestamp())
-
-        previous_interval_minute = datetime.now().minute // interval * interval
-
-        end_time = int(datetime(today.year, today.month,
-                                today.day, hour=today.hour, minute=previous_interval_minute).timestamp())
-
-        instrument = self.get_instrument_by_symbol(exchange, symbol)
-
-        PARAMS = {
-            'candletype': 1,
-            'data_duration': interval,
-            'starttime': start_time,
-            'endtime': end_time,
-            'exchange': exchange,
-            'type': 'live',
-            'token': instrument.token
-        }
-
-        r = self.reqsession.get(
-            'https://alpha.sasonline.in/api/v1/charts', params=PARAMS, headers=self.__headers)
-        data = r.json()
-        return self.__format_candles(data, divider)
-
-    def buy_bo(self, instrument, qty, price, trigger_price, stop_loss_value, square_off_value):
-        data = self.place_order(TransactionType.Buy, instrument, qty,
-                                OrderType.StopLossLimit, ProductType.BracketOrder,
-                                price=price, trigger_price=trigger_price, stop_loss=stop_loss_value,
-                                square_off=square_off_value, order_tag='python-buy-bo')
-        if data['status'] == 'success':
-            return data['data']['oms_order_id']
-        return data.json()
-
-    def sell_bo(self, instrument, qty, price, trigger_price, stop_loss_value, square_off_value):
-        data = self.place_order(TransactionType.Sell, instrument, qty,
-                                OrderType.StopLossLimit, ProductType.BracketOrder,
-                                price=price, trigger_price=trigger_price, stop_loss=stop_loss_value,
-                                square_off=square_off_value, order_tag='python-sell-bo')
-        if data['status'] == 'success':
-            return data['data']['oms_order_id']
-        return data.json()
-
-    def get_total_m2m(self):
-        data = self.get_netwise_positions()
-        if data['status'] != 'success':
-            return None
-        else:
-            positions = pd.DataFrame(data['data']['positions'], index=None)
-            if positions.empty:
-                return 0
-            positions['m2m'] = positions['m2m'].str.replace(
-                ',', '').astype(float)
-            return float(positions['m2m'].sum())
-
-    def _format_candles(self, data, interval):
-        records = data['data']['candles']
-        df = pd.DataFrame(records, columns=[
-            'datetime', 'open', 'high', 'low', 'close', 'volume'])  # , index=0)
-        df['datetime'] = df['datetime'].apply(
-            pd.Timestamp, unit='s', tzinfo=pytz.timezone('Asia/Kolkata'))
-
-        df[['open', 'high', 'low', 'close']] = df[[
-            'open', 'high', 'low', 'close']].astype(float)
-        df['volume'] = df['volume'].astype(int)
-        df.set_index('datetime', inplace=True)
-        if interval in ['2H', '3H', '4H', 'W', 'M']:
-            if interval == 'W':
-                interval = 'W-Mon'
-            df = df.resample(interval, origin='start').agg({'open': 'first', 'high': 'max',
-                                                            'low': 'min', 'close': 'last', 'volume': 'sum'}).dropna()
-        df.index = df.index.astype(str).str[:-6]
-        return df
-
-    def history(self, instrument, start_time=datetime.today() - timedelta(days=2), end_time=datetime.now(), interval=1, is_index=False):
-        exchange = instrument.exchange
-        start_time = int(start_time.timestamp())
-        end_time = int(end_time.timestamp())
-        if is_index:
-            exchange = 'NSE_INDICES'
-
-        candle_type = self._candletype[interval]
-
-        data_duration = self._data_duration[interval]
-
-        PARAMS = {
-            'exchange': exchange,
-            'token': instrument.token,
-            'name': instrument.symbol,
-            'candletype': candle_type,
-            'starttime': start_time,
-            'endtime': end_time,
-            'type': 'all'
-        }
-        if data_duration is not None:
-            PARAMS['data_duration'] = data_duration
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Connection': 'Keep-Alive',
-            'Accept': 'application/json'
-        }
-        r = requests.get(
-            'https://ant.aliceblueonline.com/api/v1/charts/tdv', params=PARAMS, headers=headers)
-        data = r.json()
-        return self._format_candles(data, interval)
+from collections import namedtuple, OrderedDict
+from datetime import datetime, timedelta
+from protlib import CUInt, CStruct, CULong, CUChar, CArray, CUShort, CString
+
+import alphatrade.exceptions as ex
+import enum
+import logging
+import json
+import pandas as pd
+import pyotp
+import pytz
+from time import sleep
+import requests
+import threading
+import websocket
+
+Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
+                                       'name', 'expiry', 'lot_size'])
+logger = logging.getLogger(__name__)
+
+
+class Requests(enum.Enum):
+    """ Enum for all requests """
+    PUT = 1
+    DELETE = 2
+    GET = 3
+    POST = 4
+
+
+class TransactionType(enum.Enum):
+    Buy = 'BUY'
+    Sell = 'SELL'
+
+
+class OrderType(enum.Enum):
+    Market = 'MARKET'
+    Limit = 'LIMIT'
+    StopLossLimit = 'SL'
+    StopLossMarket = 'SL-M'
+
+
+class ProductType(enum.Enum):
+    Intraday = 'I'
+    Delivery = 'D'
+    CoverOrder = 'CO'
+    BracketOrder = 'BO'
+
+
+class LiveFeedType(enum.Enum):
+    MARKET_DATA = 1
+    COMPACT = 2
+    SNAPQUOTE = 3
+    FULL_SNAPQUOTE = 4
+
+
+class WsFrameMode(enum.IntEnum):
+    MARKETDATA = 1
+    COMPACT_MARKETDATA = 2
+    SNAPQUOTE = 3
+    FULL_SNAPQUOTE = 4
+    SPREADDATA = 5
+    SPREAD_SNAPQUOTE = 6
+    DPR = 7
+    OI = 8
+    MARKET_STATUS = 9
+    EXCHANGE_MESSAGES = 10
+
+
+class MarketData(CStruct):
+    exchange = CUChar()
+    token = CUInt()
+    ltp = CUInt()
+    ltt = CUInt()
+    ltq = CUInt()
+    volume = CUInt()
+    best_bid_price = CUInt()
+    best_bid_quantity = CUInt()
+    best_ask_price = CUInt()
+    best_ask_quantity = CUInt()
+    total_buy_quantity = CULong()
+    total_sell_quantity = CULong()
+    atp = CUInt()
+    exchange_time_stamp = CUInt()
+    open = CUInt()
+    high = CUInt()
+    low = CUInt()
+    close = CUInt()
+    yearly_high = CUInt()
+    yearly_low = CUInt()
+
+
+class CompactData(CStruct):
+    exchange = CUChar()
+    token = CUInt()
+    ltp = CUInt()
+    change = CUInt()
+    exchange_time_stamp = CUInt()
+    volume = CUInt()
+
+
+class SnapQuote(CStruct):
+    exchange = CUChar()
+    token = CUInt()
+    buyers = CArray(5, CUInt)
+    bid_prices = CArray(5, CUInt)
+    bid_quantities = CArray(5, CUInt)
+    sellers = CArray(5, CUInt)
+    ask_prices = CArray(5, CUInt)
+    ask_quantities = CArray(5, CUInt)
+    exchange_time_stamp = CUInt()
+
+
+class FullSnapQuote(CStruct):
+    exchange = CUChar()
+    token = CUInt()
+    buyers = CArray(5, CUInt)
+    bid_prices = CArray(5, CUInt)
+    bid_quantities = CArray(5, CUInt)
+    sellers = CArray(5, CUInt)
+    ask_prices = CArray(5, CUInt)
+    ask_quantities = CArray(5, CUInt)
+    atp = CUInt()
+    open = CUInt()
+    high = CUInt()
+    low = CUInt()
+    close = CUInt()
+    total_buy_quantity = CULong()
+    total_sell_quantity = CULong()
+    volume = CUInt()
+
+
+class DPR(CStruct):
+    exchange = CUChar()
+    token = CUInt()
+    exchange_time_stamp = CUInt()
+    high = CUInt()
+    low = CUInt()
+
+
+class OpenInterest(CStruct):
+    exchange = CUChar()
+    token = CUInt()
+    current_open_interest = CUChar()
+    initial_open_interest = CUChar()
+    exchange_time_stamp = CUInt()
+
+
+class ExchangeMessage(CStruct):
+    exchange = CUChar()
+    length = CUShort()
+    message = CString(length="length")
+    exchange_time_stamp = CUInt()
+
+
+class MarketStatus(CStruct):
+    exchange = CUChar()
+    length_of_market_type = CUShort()
+    market_type = CString(length="length_of_market_type")
+    length_of_status = CUShort()
+    status = CString(length="length_of_status")
+
+
+class AlphaTrade(object):
+    # dictionary object to hold settings
+    __service_config = {
+        'host': 'https://alpha.sasonline.in',
+        'routes': {
+            'login': '/api/v3/user/login',
+            'validatetotp': '/api/v3/user/validatetotp',
+            'profile': '/api/v1/user/profile',
+            'master_contract': '/api/v2/contracts.json?exchanges={exchange}',
+            'holdings': '/api/v1/holdings',
+            'balance': '/api/v1/funds/view?type=all',
+            'funds': '/api/v1/funds/view?type={fund_type}',
+            'positions_daywise': '/api/v1/positions?type=live',
+            'positions_netwise': '/api/v1/positions?type=historical',
+            'positions_holdings': '/api/v1/holdings',
+            'place_order': '/api/v1/orders',
+            'place_amo': '/api/v1/orders/amo',
+            'place_bracket_order': '/api/v1/orders/bracket',
+            'place_basket_order': '/api/v1/orders/basket',
+            'orders': '/api/v1/orders?type={order_type}',
+            'get_order_info': '/api/v1/order/{order_id}/history',
+            'modify_order': '/api/v1/orders',
+            'cancel_order': '/api/v1/order?oms_order_id={order_id}&order_status=open',
+            'cancel_bo_order': '/api/v1/order/bracket?oms_order_id={order_id}&order_status=open&leg_order_indicator={leg_order_id}',
+            'cancel_co_order': '/api/v1/order/cover?oms_order_id={order_id}&order_status=open&leg_order_indicator={leg_order_id}',
+            'trade_book': '/api/v1/trades',
+            'scripinfo': '/api/v1/contract/{exchange}?info=scrip&token={token}',
+            'contract': '/api/v1/contract/{exchange}',
+            'search': '/api/v1/search?key={symbol}',
+            'positions': '/api/v1/positions?type={position_type}',
+        },
+        # 'socket_endpoint': 'wss://alpha.sasonline.in/socket/websocket?token={access_token}&login_id={login_id}'
+        'socket_endpoint': 'wss://alpha.sasonline.in/hydrasocket/v2/websocket?access_token={access_token}'
+    }
+
+    _candle_type = {1: 1, 2: 1, 3: 1, 5: 1, 10: 1, 15: 1,
+                    30: 1, 45: 1, '1H': 2, '2H': 2, '3H': 2, '4H': 2, '1D': 3, 'D': 3, 'W': 3, 'M': 3}
+
+    _data_duration = {1: 1, 2: 2, 3: 3, 5: 5, 10: 10, 15: 15,
+                      30: 30, 45: 45, '1H': None, '2H': 2, '3H': 2, '4H': 2, '1D': None, 'D': None, 'W': None, 'M': None}
+
+    def __init__(self, login_id, password, twofa, access_token=None, master_contracts_to_download=None):
+        """ logs in and gets enabled exchanges and products for user """
+        if len(twofa) != 6:
+            pin = pyotp.TOTP(twofa).now()
+            twofa = f"{int(pin):06d}" if len(pin) <= 5 else pin
+
+        self.__access_token = access_token
+        self.__login_id = login_id
+        self.__password = password
+        self.__twofa = twofa
+        self.__websocket = None
+        self.__websocket_connected = False
+        self.__ws_mutex = threading.Lock()
+        self.__on_error = None
+        self.__on_disconnect = None
+        self.__on_open = None
+        self.__subscribe_callback = None
+        self.__order_update_callback = None
+        self.__market_status_messages_callback = None
+        self.__exchange_messages_callback = None
+        self.__oi_callback = None
+        self.__dpr_callback = None
+        self.__subscribers = {}
+        self.__market_status_messages = []
+        self.__exchange_messages = []
+        self.__exchange_codes = {'NSE': 1,
+                                 'NFO': 2,
+                                 'CDS': 3,
+                                 'MCX': 4,
+                                 'BSE': 6,
+                                 'BFO': 7}
+        self.__exchange_price_multipliers = {1: 100,
+                                             2: 100,
+                                             3: 10000000,
+                                             4: 100,
+                                             6: 100,
+                                             7: 100}
+
+        self.__headers = {
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.102 Safari/537.36'
+        }
+
+        self.session = requests.session()
+
+        if not self.__is_token_valid():
+            self.__get_question_ids()
+            self.__set_access_token()
+        else:
+            self.__headers['X-Authorization-Token'] = self.__access_token
+
+        try:
+            profile = self.get_profile()
+        except Exception as exp:
+            raise ex.PermissionException(
+                f"Couldn't get profile info with credentials provided :: {exp}")
+        if (profile['status'] == 'error'):
+            # Don't know why this error comes, but it safe to proceed further.
+            if (profile['message'] == 'Not able to retrieve AccountInfoService'):
+                logger.warning(
+                    "Couldn't get profile info - 'Not able to retrieve AccountInfoService'")
+            else:
+                raise ex.PermissionException(
+                    f"Couldn't get profile info '{profile['message']}'")
+        self.__master_contracts_by_token = {}
+        self.__master_contracts_by_symbol = {}
+        if (master_contracts_to_download is None):
+            # for e in self.__enabled_exchanges:
+            for e in ['NSE', 'NFO', 'CDS', 'BSE', 'BFO', 'MCX']:
+                self.__get_master_contract(e)
+        else:
+            for e in master_contracts_to_download:
+                self.__get_master_contract(e)
+        self.ws_thread = None
+
+    def __is_token_valid(self):
+        if self.__access_token is None:
+            try:
+                self.__access_token = open(
+                    'access_token.txt', 'r', encoding='utf-8').read().rstrip()
+            except FileNotFoundError:
+                print('File not found.')
+                self.__access_token = None
+                return False
+        self.__headers['X-Authorization-Token'] = self.__access_token
+        profile_url = 'https://alpha.sasonline.in/api/v1/user/profile'
+        resp = self.session.get(profile_url, headers=self.__headers)
+        return resp.status_code == 200 and resp.json()['status'] == 'success'
+
+    def __get_question_ids(self):
+        login_body = {
+            "device": "web",
+            'login_id': self.__login_id,
+            'password': self.__password
+        }
+        response = self.session.post(
+            'https://alpha.sasonline.in/api/v3/user/login', json=login_body)
+
+        if response.status_code != 200:
+            raise requests.HTTPError(response.text)
+        if 'error' in response.text:
+            raise requests.HTTPError(response.text)
+        twofa_token = response.json()['data']['twofa']['twofa_token']
+        self.__twofa_token = twofa_token
+
+    def __set_access_token(self):
+        twofa_body = {"login_id": self.__login_id,
+                      "twofa_token": self.__twofa_token,
+                      "totp": self.__twofa}
+        response = self.session.post(
+            'https://alpha.sasonline.in/api/v3/user/validatetotp', json=twofa_body)
+        if response.status_code != 200:
+            raise requests.HTTPError(response.text)
+        if 'error' in response.text:
+            raise requests.HTTPError(response.text)
+        auth_token = response.json()['data']['auth_token']
+
+        with open('access_token.txt', 'w', encoding='utf-8') as wr:
+            wr.write(auth_token)
+
+        self.__access_token = auth_token
+        self.__headers['X-Authorization-Token'] = self.__access_token
+
+    def __convert_prices(self, dictionary, multiplier):
+        keys = ['ltp',
+                'best_bid_price',
+                'best_ask_price',
+                'atp',
+                'open',
+                'high',
+                'low',
+                'close',
+                'yearly_high',
+                'yearly_low']
+        for key in keys:
+            if (key in dictionary):
+                dictionary[key] = dictionary[key]/multiplier
+        multiple_value_keys = ['bid_prices', 'ask_prices']
+        for key in multiple_value_keys:
+            if (key in dictionary):
+                new_values = []
+                for value in dictionary[key]:
+                    new_values.append(value/multiplier)
+                dictionary[key] = new_values
+        return dictionary
+
+    def __format_candles(self, data, divider=100):
+        records = data['data']
+        df = pd.DataFrame(records, columns=[
+            'date', 'open', 'high', 'low', 'close', 'volume'])  # , index=0)
+        df['date'] = df['date'].apply(
+            pd.Timestamp, unit='s', tzinfo=pytz.timezone('Asia/Kolkata'))
+        # df['datetime'] = df['datetime'].astype(str).str[:-6]
+        df[['open', 'high', 'low', 'close']] = df[[
+            'open', 'high', 'low', 'close']].astype(float).div(divider)
+        df['volume'] = df['volume'].astype(int)
+        df.set_index('date', inplace=True)
+        return df
+
+    def __convert_exchanges(self, dictionary):
+        if ('exchange' in dictionary):
+            d = self.__exchange_codes
+            dictionary['exchange'] = list(d.keys())[list(
+                d.values()).index(dictionary['exchange'])]
+        return dictionary
+
+    def __convert_instrument(self, dictionary):
+        if ('exchange' in dictionary) and ('token' in dictionary):
+            dictionary['instrument'] = self.get_instrument_by_token(
+                dictionary['exchange'], dictionary['token'])
+        return dictionary
+
+    def __modify_human_readable_values(self, dictionary):
+        dictionary = self.__convert_prices(
+            dictionary, self.__exchange_price_multipliers[dictionary['exchange']])
+        dictionary = self.__convert_exchanges(dictionary)
+        dictionary = self.__convert_instrument(dictionary)
+        return dictionary
+
+    def __on_data_callback(self, ws=None, message=None):
+        # This workaround is to solve the websocket_client's compatibility
+        # issue of older versions. ie.0.40.0 which is used in Upstox.
+        # Now this will work in both 0.40.0 & newer version of websocket_client
+        if not isinstance(ws, websocket.WebSocketApp):
+            message = ws
+        if (message[0] == WsFrameMode.MARKETDATA):
+            p = MarketData.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            if (self.__subscribe_callback is not None):
+                self.__subscribe_callback(res)
+        elif (message[0] == WsFrameMode.COMPACT_MARKETDATA):
+            p = CompactData.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            if (self.__subscribe_callback is not None):
+                self.__subscribe_callback(res)
+        elif (message[0] == WsFrameMode.SNAPQUOTE):
+            p = SnapQuote.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            if (self.__subscribe_callback is not None):
+                self.__subscribe_callback(res)
+        elif (message[0] == WsFrameMode.FULL_SNAPQUOTE):
+            p = FullSnapQuote.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            if (self.__subscribe_callback is not None):
+                self.__subscribe_callback(res)
+        elif (message[0] == WsFrameMode.DPR):
+            p = DPR.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            if (self.__dpr_callback is not None):
+                self.__dpr_callback(res)
+        elif (message[0] == WsFrameMode.OI):
+            p = OpenInterest.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            if (self.__oi_callback is not None):
+                self.__oi_callback(res)
+        elif (message[0] == WsFrameMode.MARKET_STATUS):
+            p = MarketStatus.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            self.__market_status_messages.append(res)
+            if (self.__market_status_messages_callback is not None):
+                self.__market_status_messages_callback(res)
+        elif (message[0] == WsFrameMode.EXCHANGE_MESSAGES):
+            p = ExchangeMessage.parse(message[1:]).__dict__
+            res = self.__modify_human_readable_values(p)
+            self.__exchange_messages.append(res)
+            if (self.__exchange_messages_callback is not None):
+                self.__exchange_messages_callback(res)
+
+    def __on_close_callback(self, ws=None):
+        self.__websocket_connected = False
+        if self.__on_disconnect:
+            self.__on_disconnect()
+
+    def __on_open_callback(self, ws=None):
+        self.__websocket_connected = True
+        self.__resubscribe()
+        if self.__on_open:
+            self.__on_open()
+
+    def __on_error_callback(self, ws=None, error=None):
+        # This workaround is to solve the websocket_client's compatibility issue of older versions. ie.0.40.0 which is used in upstox. Now this will work in both 0.40.0 & newer version of websocket_client
+        if (isinstance(ws, websocket.WebSocketApp) is not True):
+            error = ws
+        if self.__on_error:
+            self.__on_error(error)
+
+    def __send_heartbeat(self):
+        heart_beat = {"a": "h", "v": [], "m": ""}
+        while True:
+            sleep(5)
+            self.__ws_send(json.dumps(heart_beat),
+                           opcode=websocket._abnf.ABNF.OPCODE_PING)
+
+    def __ws_run_forever(self):
+        while True:
+            try:
+                self.__websocket.run_forever()
+            except Exception as exp:
+                logger.warning(
+                    f"websocket run forever ended in exception, {exp}")
+            sleep(0.1)  # Sleep for 100ms between reconnection.
+
+    def __ws_send(self, *args, **kwargs):
+        while self.__websocket_connected == False:
+            # sleep for 50ms if websocket is not connected, wait for reconnection
+            sleep(0.05)
+        with self.__ws_mutex:
+            self.__websocket.send(*args, **kwargs)
+
+    def start_websocket(self, subscribe_callback=None,
+                        order_update_callback=None,
+                        socket_open_callback=None,
+                        socket_close_callback=None,
+                        socket_error_callback=None,
+                        run_in_background=False,
+                        market_status_messages_callback=None,
+                        exchange_messages_callback=None,
+                        oi_callback=None,
+                        dpr_callback=None):
+        """ Start a websocket connection for getting live data """
+        self.__on_open = socket_open_callback
+        self.__on_disconnect = socket_close_callback
+        self.__on_error = socket_error_callback
+        self.__subscribe_callback = subscribe_callback
+        self.__order_update_callback = order_update_callback
+        self.__market_status_messages_callback = market_status_messages_callback
+        self.__exchange_messages_callback = exchange_messages_callback
+        self.__oi_callback = oi_callback
+        self.__dpr_callback = dpr_callback
+
+        url = self.__service_config['socket_endpoint'].format(
+            access_token=self.__access_token)
+        self.__websocket = websocket.WebSocketApp(url,
+                                                  on_data=self.__on_data_callback,
+                                                  on_error=self.__on_error_callback,
+                                                  on_close=self.__on_close_callback,
+                                                  on_open=self.__on_open_callback)
+        th = threading.Thread(target=self.__send_heartbeat)
+        th.daemon = True
+        th.start()
+        if run_in_background is True:
+            self.__ws_thread = threading.Thread(target=self.__ws_run_forever)
+            self.__ws_thread.daemon = True
+            self.__ws_thread.start()
+        else:
+            self.__ws_run_forever()
+
+    def get_profile(self):
+        """ Get profile """
+        profile = self.__api_call_helper('profile', Requests.GET, None, None)
+        if (profile['status'] != 'error'):
+            # self.__enabled_exchanges = profile['data']['exchanges_subscribed']
+            self.__enabled_exchanges = ['NSE', 'MCX', 'NFO', 'BSE', 'BFO', 'CDS']
+        return profile
+
+    def get_balance(self):
+        """ Get balance/margins """
+        return self.__api_call_helper('balance', Requests.GET, None, None)
+
+    def get_daywise_positions(self):
+        """ Get daywise positions """
+        return self.__api_call_helper('positions_daywise', Requests.GET, None, None)
+
+    def get_netwise_positions(self):
+        """ Get netwise positions """
+        return self.__api_call_helper('positions_netwise', Requests.GET, None, None)
+
+    def get_holding_positions(self):
+        """ Get holding positions """
+        return self.__api_call_helper('positions_holdings', Requests.GET, None, None)
+
+    def positions(self, position_type='live'):
+        """ get all positions """
+        params = {'position_type': position_type}
+        return self.__api_call_helper('positions', Requests.GET, params, None)
+
+    def orders(self, order_type='complete'):
+        """ get all orders """
+        params = {'order_type': order_type}
+        return self.__api_call_helper('orders', Requests.GET, params, None)
+
+    def funds(self, fund_type='all'):
+        """ get all funds """
+        params = {'fund_type': fund_type}
+        return self.__api_call_helper('funds', Requests.GET, params, None)
+
+    # def __to_instrument(self, scrip):
+    #     """ Convert scrip to instrument """
+    #     print(scrip)
+    #     instrument = Instrument(scrip['exchange'], int(scrip['token']), 
+    #                       scrip['trading_symbol'], 
+    #                       scrip['company'], None, 1)
+    #     print(isinstance(instrument, Instrument))
+    #     print(instrument)
+    #     return instrument
+        
+    
+    def search(self, symbol='Nifty Bank', exchange='NSE'):
+        """ search for scrips """
+        params = {'symbol': symbol}
+        data = self.__api_call_helper('search', Requests.GET, params, None)
+        return data['result']
+
+    def get_order_history(self, order_id=None):
+        """ leave order_id as None to get all entire order history """
+        if order_id is None:
+            return self.orders()
+        else:
+            return self.__api_call_helper('get_order_info', Requests.GET, {'order_id': order_id}, None)
+
+    def get_scrip_info(self, instrument):
+        """ Get scrip information """
+        params = {'exchange': instrument.exchange, 'token': instrument.token}
+        return self.__api_call_helper('scripinfo', Requests.GET, params, None)
+
+    def get_trade_book(self):
+        """ get all trades """
+        return self.__api_call_helper('trade_book', Requests.GET, None, None)
+
+    def get_exchanges(self):
+        """ Get enabled exchanges """
+        return self.__enabled_exchanges
+
+    def __get_product_type_str(self, product_type, exchange):
+        prod_type = None
+        if (product_type == ProductType.Intraday):
+            prod_type = 'MIS'
+        elif product_type == ProductType.Delivery:
+            prod_type = 'NRML' if exchange in ['NFO', 'MCX', 'CDS'] else 'CNC'
+        elif (product_type == ProductType.CoverOrder):
+            prod_type = 'CO'
+        elif (product_type == ProductType.BracketOrder):
+            prod_type = None
+        return prod_type
+
+    def place_order(self, transaction_type, instrument, quantity, order_type,
+                    product_type, price=0.0, trigger_price=None,
+                    stop_loss=None, square_off=None, trailing_sl=None,
+                    is_amo=False,
+                    order_tag='python'):
+        """ placing an order, many fields are optional and are not required
+            for all order types
+        """
+        if transaction_type is None:
+            raise TypeError(
+                "Required parameter transaction_type not of type TransactionType")
+
+        if not isinstance(instrument, Instrument):
+            raise TypeError(
+                "Required parameter instrument not of type Instrument")
+
+        if not isinstance(quantity, int):
+            raise TypeError("Required parameter quantity not of type int")
+
+        if order_type is None:
+            raise TypeError(
+                "Required parameter order_type not of type OrderType")
+
+        if product_type is None:
+            raise TypeError(
+                "Required parameter product_type not of type ProductType")
+
+        if price is not None and not isinstance(price, float):
+            raise TypeError("Optional parameter price not of type float")
+
+        if trigger_price is not None and not isinstance(trigger_price, float):
+            raise TypeError(
+                "Optional parameter trigger_price not of type float")
+
+        prod_type = self.__get_product_type_str(
+            product_type, instrument.exchange)
+        # construct order object after all required parameters are met
+        order = {'exchange': instrument.exchange,
+                 'order_type': order_type.value,
+                 'instrument_token': instrument.token,
+                 'quantity': quantity,
+                 'disclosed_quantity': 0,
+                 'price': price,
+                 'transaction_type': transaction_type.value,
+                 'trigger_price': trigger_price,
+                 'validity': 'DAY',
+                 'product': prod_type,
+                 'source': 'web',
+                 'order_tag': order_tag}
+
+        if stop_loss is not None:
+            if isinstance(stop_loss, float):
+                order['stop_loss_value'] = stop_loss
+
+            else:
+                raise TypeError(
+                    "Optional parameter stop_loss not of type float")
+        if square_off is not None:
+            if isinstance(square_off, float):
+                order['square_off_value'] = square_off
+
+            else:
+                raise TypeError(
+                    "Optional parameter square_off not of type float")
+        if trailing_sl is not None:
+            if not isinstance(trailing_sl, int):
+                raise TypeError(
+                    "Optional parameter trailing_sl not of type int")
+            else:
+                order['trailing_stop_loss'] = trailing_sl
+
+        if product_type is ProductType.CoverOrder and not isinstance(
+            trigger_price, float
+        ):
+            raise TypeError(
+                "Required parameter trigger_price not of type float")
+
+        helper = 'place_amo' if (is_amo == True) else 'place_order'
+        if product_type is ProductType.BracketOrder:
+            helper = 'place_bracket_order'
+            del order['product']
+            if not isinstance(stop_loss, float):
+                raise TypeError(
+                    "Required parameter stop_loss not of type float")
+
+            if not isinstance(square_off, float):
+                raise TypeError(
+                    "Required parameter square_off not of type float")
+
+        return self.__api_call_helper(helper, Requests.POST, None, order)
+
+    def place_basket_order(self, orders):
+        """ placing a basket order, 
+            Argument orders should be a list of all orders that should be sent
+            each element in order should be a dictionary containing the following key.
+            "instrument", "order_type", "quantity", "price" (only if its a limit order), 
+            "transaction_type", "product_type"
+        """
+        keys = {"instrument": Instrument,
+                "order_type": OrderType,
+                "quantity": int,
+                "transaction_type": TransactionType,
+                "product_type": ProductType}
+        if not isinstance(orders, list):
+            raise TypeError("Required parameter orders is not of type list")
+
+        if len(orders) <= 0:
+            raise TypeError("Length of orders should be greater than 0")
+
+        for i in orders:
+            if not isinstance(i, dict):
+                raise TypeError(
+                    "Each element in orders should be of type dict")
+            for s, value in keys.items():
+                if s not in i:
+                    raise TypeError(
+                        f"Each element in orders should have key {s}")
+                if type(i[s]) is not value:
+                    raise TypeError(
+                        f"Element '{s}' in orders should be of type {keys[s]}")
+            if i['order_type'] == OrderType.Limit:
+                if "price" not in i:
+                    raise TypeError(
+                        "Each element in orders should have key 'price' if its a limit order ")
+                if not isinstance(i['price'], float):
+                    raise TypeError(
+                        "Element price in orders should be of type float")
+            else:
+                i['price'] = 0.0
+            if i['order_type'] in [
+                OrderType.StopLossLimit,
+                OrderType.StopLossMarket,
+            ]:
+                if 'trigger_price' not in i:
+                    raise TypeError(
+                        f"Each element in orders should have key 'trigger_price' if it is an {i['order_type']} order")
+                if not isinstance(i['trigger_price'], float):
+                    raise TypeError(
+                        "Element trigger_price in orders should be of type float")
+            else:
+                i['trigger_price'] = 0.0
+            if (i['product_type'] == ProductType.Intraday):
+                i['product_type'] = 'MIS'
+            elif i['product_type'] == ProductType.Delivery:
+                i['product_type'] = 'NRML' if (
+                    i['instrument'].exchange == 'NFO') else 'CNC'
+            elif i['product_type'] in [
+                ProductType.CoverOrder,
+                ProductType.BracketOrder,
+            ]:
+                raise TypeError(
+                    "Product Type BO or CO is not supported in basket order")
+            if i['quantity'] <= 0:
+                raise TypeError("Quantity should be greater than 0")
+
+        data = {'source': 'web',
+                'orders': []}
+        for i in orders:
+            # construct order object after all required parameters are met
+            data['orders'].append({'exchange': i['instrument'].exchange,
+                                   'order_type': i['order_type'].value,
+                                   'instrument_token': i['instrument'].token,
+                                   'quantity': i['quantity'],
+                                   'disclosed_quantity': 0,
+                                   'price': i['price'],
+                                   'transaction_type': i['transaction_type'].value,
+                                   'trigger_price': i['trigger_price'],
+                                   'validity': 'DAY',
+                                   'product': i['product_type']})
+
+        helper = 'place_basket_order'
+        return self.__api_call_helper(helper, Requests.POST, None, data)
+
+    def modify_order(self, transaction_type, instrument, product_type, order_id, order_type, quantity=None, price=0.0,
+                     trigger_price=0.0):
+        """ modify an order, transaction_type, instrument, product_type, order_id & order_type is required, 
+            rest are optional, use only when when you want to change that attribute.
+        """
+        if not isinstance(instrument, Instrument):
+            raise TypeError(
+                "Required parameter instrument not of type Instrument")
+
+        if not isinstance(order_id, str):
+            raise TypeError("Required parameter order_id not of type str")
+
+        if quantity is not None and not isinstance(quantity, int):
+            raise TypeError("Optional parameter quantity not of type int")
+
+        if type(order_type) is not OrderType:
+            raise TypeError(
+                "Optional parameter order_type not of type OrderType")
+
+        if ProductType is None:
+            raise TypeError(
+                "Required parameter product_type not of type ProductType")
+
+        if price is not None and not isinstance(price, float):
+            raise TypeError("Optional parameter price not of type float")
+
+        if trigger_price is not None and not isinstance(trigger_price, float):
+            raise TypeError(
+                "Optional parameter trigger_price not of type float")
+
+        if (product_type == ProductType.Intraday):
+            product_type = 'MIS'
+        elif product_type == ProductType.Delivery:
+            product_type = 'NRML' if (instrument.exchange == 'NFO') else 'CNC'
+        elif (product_type == ProductType.CoverOrder):
+            product_type = 'CO'
+        elif (product_type == ProductType.BracketOrder):
+            product_type = None
+        # construct order object with order id
+        order = {'oms_order_id': str(order_id),
+                 'instrument_token': int(instrument.token),
+                 'exchange': instrument.exchange,
+                 'transaction_type': transaction_type.value,
+                 'product': product_type,
+                 'validity': 'DAY',
+                 'order_type': order_type.value,
+                 'price': price,
+                 'trigger_price': trigger_price,
+                 'quantity': quantity,
+                 'disclosed_quantity': 0,
+                 'nest_request_id': '1'}
+        return self.__api_call_helper('modify_order', Requests.PUT, None, order)
+
+    def cancel_order(self, order_id, leg_order_id=None, is_co=False):
+        """ Cancel single order """
+        if (is_co == False):
+            if leg_order_id is None:
+                ret = self.__api_call_helper('cancel_order', Requests.DELETE, {
+                                             'order_id': order_id}, None)
+            else:
+                ret = self.__api_call_helper('cancel_bo_order', Requests.DELETE, {
+                                             'order_id': order_id, 'leg_order_id': leg_order_id}, None)
+        else:
+            ret = self.__api_call_helper('cancel_co_order', Requests.DELETE, {
+                                         'order_id': order_id, 'leg_order_id': leg_order_id}, None)
+        return ret
+
+    def cancel_all_orders(self):
+        """ Cancel all orders """
+        ret = []
+        orders = self.get_order_history()['data']
+        if not orders:
+            return
+        for c_order in orders['pending_orders']:
+            if (c_order['product'] == 'BO' and c_order['leg_order_indicator']):
+                r = self.cancel_order(
+                    c_order['leg_order_indicator'], leg_order_id=c_order['leg_order_indicator'])
+            elif (c_order['product'] == 'CO'):
+                r = self.cancel_order(
+                    c_order['oms_order_id'], leg_order_id=c_order['leg_order_indicator'], is_co=True)
+            else:
+                r = self.cancel_order(c_order['oms_order_id'])
+            ret.append(r)
+        return ret
+
+    def subscribe_market_status_messages(self):
+        """ Subscribe to market messages """
+        return self.__ws_send(json.dumps({"a": "subscribe", "v": [1, 2, 3, 4, 6], "m": "market_status"}))
+
+    def get_market_status_messages(self):
+        """ Get market messages """
+        return self.__market_status_messages
+
+    def subscribe_exchange_messages(self):
+        """ Subscribe to exchange messages """
+        return self.__ws_send(json.dumps({"a": "subscribe", "v": [1, 2, 3, 4, 6], "m": "exchange_messages"}))
+
+    def get_exchange_messages(self):
+        """ Get stored exchange messages """
+        return self.__exchange_messages
+
+    def subscribe(self, instrument, live_feed_type):
+        """ subscribe to the current feed of an instrument """
+        if (type(live_feed_type) is not LiveFeedType):
+            raise TypeError(
+                "Required parameter live_feed_type not of type LiveFeedType")
+        arr = []
+        if (isinstance(instrument, list)):
+            for _instrument in instrument:
+                if not isinstance(_instrument, Instrument):
+                    raise TypeError(
+                        "Required parameter instrument not of type Instrument")
+                exchange = self.__exchange_codes[_instrument.exchange]
+                arr.append([exchange, int(_instrument.token)])
+                self.__subscribers[_instrument] = live_feed_type
+        else:
+            if not isinstance(instrument, Instrument):
+                raise TypeError(
+                    "Required parameter instrument not of type Instrument")
+            exchange = self.__exchange_codes[instrument.exchange]
+            arr = [[exchange, int(instrument.token)]]
+            self.__subscribers[instrument] = live_feed_type
+        if (live_feed_type == LiveFeedType.MARKET_DATA):
+            mode = 'marketdata'
+        elif (live_feed_type == LiveFeedType.COMPACT):
+            mode = 'compact_marketdata'
+        elif (live_feed_type == LiveFeedType.SNAPQUOTE):
+            mode = 'snapquote'
+        elif (live_feed_type == LiveFeedType.FULL_SNAPQUOTE):
+            mode = 'full_snapquote'
+        data = json.dumps({'a': 'subscribe', 'v': arr, 'm': mode})
+        return self.__ws_send(data)
+
+    def unsubscribe(self, instrument, live_feed_type):
+        """ unsubscribe to the current feed of an instrument """
+        if (type(live_feed_type) is not LiveFeedType):
+            raise TypeError(
+                "Required parameter live_feed_type not of type LiveFeedType")
+        arr = []
+        if (isinstance(instrument, list)):
+            for _instrument in instrument:
+                if not isinstance(_instrument, Instrument):
+                    raise TypeError(
+                        "Required parameter instrument not of type Instrument")
+                exchange = self.__exchange_codes[_instrument.exchange]
+                arr.append([exchange, int(_instrument.token)])
+                if (_instrument in self.__subscribers):
+                    del self.__subscribers[_instrument]
+        else:
+            if not isinstance(instrument, Instrument):
+                raise TypeError(
+                    "Required parameter instrument not of type Instrument")
+            exchange = self.__exchange_codes[instrument.exchange]
+            arr = [[exchange, int(instrument.token)]]
+            if (instrument in self.__subscribers):
+                del self.__subscribers[instrument]
+        if (live_feed_type == LiveFeedType.MARKET_DATA):
+            mode = 'marketdata'
+        elif (live_feed_type == LiveFeedType.COMPACT):
+            mode = 'compact_marketdata'
+        elif (live_feed_type == LiveFeedType.SNAPQUOTE):
+            mode = 'snapquote'
+        elif (live_feed_type == LiveFeedType.FULL_SNAPQUOTE):
+            mode = 'full_snapquote'
+
+        data = json.dumps({'a': 'unsubscribe', 'v': arr, 'm': mode})
+        return self.__ws_send(data)
+
+    def get_all_subscriptions(self):
+        """ get the all subscribed instruments """
+        return self.__subscribers
+
+    def __resubscribe(self):
+        market = []
+        compact = []
+        snap = []
+        full = []
+        for key, value in self.get_all_subscriptions().items():
+            if (value == LiveFeedType.MARKET_DATA):
+                market.append(key)
+            elif (value == LiveFeedType.COMPACT):
+                compact.append(key)
+            elif (value == LiveFeedType.SNAPQUOTE):
+                snap.append(key)
+            elif (value == LiveFeedType.FULL_SNAPQUOTE):
+                full.append(key)
+        if market:
+            self.subscribe(market, LiveFeedType.MARKET_DATA)
+        if compact:
+            self.subscribe(compact, LiveFeedType.COMPACT)
+        if snap:
+            self.subscribe(snap, LiveFeedType.SNAPQUOTE)
+        if full:
+            self.subscribe(full, LiveFeedType.FULL_SNAPQUOTE)
+
+    def get_instrument_by_symbol(self, exchange, symbol):
+        """ get instrument by providing symbol """
+        # get instrument given exchange and symbol
+        exchange = exchange.upper()
+        # check if master contract exists
+        if exchange not in self.__master_contracts_by_symbol:
+            logger.warning(f"Cannot find exchange {exchange} in master contract. "
+                           "Please ensure if that exchange is enabled in your profile and downloaded the master contract for the same")
+            return None
+        master_contract = self.__master_contracts_by_symbol[exchange]
+        if symbol not in master_contract:
+            logger.warning(
+                f"Cannot find symbol {exchange} {symbol} in master contract")
+            return None
+        return master_contract[symbol]
+
+    def get_instrument_for_fno(self, symbol, expiry_date, is_fut=False, strike=None, is_call=False, exchange='NFO'):
+        """ get instrument for FNO """
+        res = self.search_instruments(exchange, symbol)
+        if (res == None):
+            return
+        matches = []
+        for i in res:
+            sp = i.symbol.split(' ')
+            if (sp[0] == symbol):
+                if (i.expiry == expiry_date):
+                    matches.append(i)
+        for i in matches:
+            if (is_fut == True):
+                if ('FUT' in i.symbol):
+                    return i
+            else:
+                sp = i.symbol.split(' ')
+                if ((sp[-1] == 'CE') or (sp[-1] == 'PE')):           # Only option scrips
+                    if (float(sp[-2]) == float(strike)):
+                        if (is_call == True):
+                            if (sp[-1] == 'CE'):
+                                return i
+                        else:
+                            if (sp[-1] == 'PE'):
+                                return i
+
+    def search_instruments(self, exchange, symbol):
+        """ Search instrument by symbol match """
+        # search instrument given exchange and symbol
+        exchange = exchange.upper()
+        matches = []
+        # check if master contract exists
+        if exchange not in self.__master_contracts_by_token:
+            logger.warning(f"Cannot find exchange {exchange} in master contract. "
+                           "Please ensure if that exchange is enabled in your profile and downloaded the master contract for the same")
+            return None
+        master_contract = self.__master_contracts_by_token[exchange]
+        for contract in master_contract:
+            if (isinstance(symbol, list)):
+                for sym in symbol:
+                    if sym.lower() in master_contract[contract].symbol.split(' ')[0].lower():
+                        matches.append(master_contract[contract])
+            else:
+                if symbol.lower() in master_contract[contract].symbol.split(' ')[0].lower():
+                    matches.append(master_contract[contract])
+        return matches
+
+    def get_instrument_by_token(self, exchange, token):
+        """ Get instrument by providing token """
+        # get instrument given exchange and token
+        exchange = exchange.upper()
+        token = int(token)
+        
+
+    def get_master_contract(self, exchange):
+        """ Get master contract """
+        return self.__master_contracts_by_symbol[exchange]
+
+    def __get_master_contract(self, exchange):
+        """ returns all the tradable contracts of an exchange
+            placed in an OrderedDict and the key is the token
+        """
+        print(f'Downloading master contracts for exchange: {exchange}')
+        body = self.__api_call_helper(
+            'master_contract', Requests.GET, {'exchange': exchange}, None)
+        master_contract_by_token = OrderedDict()
+        master_contract_by_symbol = OrderedDict()
+        for sub in body:
+            for scrip in body[sub]:
+                # convert token
+                token = int(scrip['code'])
+
+                # convert symbol to upper
+                symbol = scrip['symbol']
+
+                # convert expiry to none if it's non-existent
+                if ('expiry' in scrip):
+                    expiry = datetime.fromtimestamp(
+                        scrip['expiry']).date()
+                else:
+                    expiry = None
+
+                # convert lot size to int
+                lot_size = scrip['lotSize'] if ('lotSize' in scrip) else None
+                # Name & Exchange
+                name = scrip['company']
+                exch = scrip['exchange']
+
+                instrument = Instrument(
+                    exch, token, symbol, name, expiry, lot_size)
+                master_contract_by_token[token] = instrument
+                master_contract_by_symbol[symbol] = instrument
+        self.__master_contracts_by_token[exchange] = master_contract_by_token
+        self.__master_contracts_by_symbol[exchange] = master_contract_by_symbol
+
+    def __api_call_helper(self, name, http_method, params, data):
+        # helper formats the url and reads error codes nicely
+        config = self.__service_config
+        url = f"{config['host']}{config['routes'][name]}"
+        if params is not None:
+            url = url.format(**params)
+
+        response = self.__api_call(url, http_method, data)
+        if response.status_code != 200:
+            raise requests.HTTPError(response.text)
+        return json.loads(response.text)
+
+    def __api_call(self, url, http_method, data):
+        # logger.debug('url:: %s http_method:: %s data:: %s headers:: %s', url, http_method, data, headers)
+        headers = {"Content-Type": "application/json"}
+        if (len(self.__access_token) > 100):
+            headers['X-Authorization-Token'] = self.__access_token
+            headers['Connection'] = 'keep-alive'
+        else:
+            headers['client_id'] = self.__login_id
+            headers['authorization'] = f"Bearer {self.__access_token}"
+        r = None
+        if http_method is Requests.POST:
+            r = self.session.post(
+                url, data=json.dumps(data), headers=headers)
+        elif http_method is Requests.DELETE:
+            r = self.session.delete(url, headers=headers)
+        elif http_method is Requests.PUT:
+            r = self.session.put(
+                url, data=json.dumps(data), headers=headers)
+        elif http_method is Requests.GET:
+            params = {'client_id': self.__login_id}
+            r = self.session.get(url, params=params, headers=headers)
+        return r
+
+    def get_historical_candles(self, exchange, symbol, start_time, end_time, interval=5, is_index=False):
+        exchange = exchange.upper()
+        idx = '' if not is_index else '_INDICES'
+        divider = 100
+        if exchange == 'CDS':
+            divider = 1e7
+        # symbol = symbol.upper()
+        instrument = self.get_instrument_by_symbol(exchange, symbol)
+        print(instrument)
+        start_time = int(start_time.timestamp())
+        end_time = int(end_time.timestamp())
+
+        PARAMS = {
+            'candletype': 1,
+            'data_duration': interval,
+            'starttime': start_time,
+            'endtime': end_time,
+            'exchange': exchange + idx,
+            'type': 'historical',
+            'token': instrument.token
+        }
+
+        r = self.session.get(
+            'https://alpha.sasonline.in/api/v1/charts', params=PARAMS, headers=self.__headers)
+        data = r.json()
+        return self.__format_candles(data, divider)
+
+    def get_intraday_candles(self, exchange, symbol, interval=5):
+        exchange = exchange.upper()
+        divider = 100
+        if exchange == 'CDS':
+            divider = 1e7
+        # symbol = symbol.upper()
+        today = datetime.today()
+        start_time = int(datetime(today.year, today.month,
+                                  today.day, hour=9, minute=00).timestamp())
+
+        previous_interval_minute = datetime.now().minute // interval * interval
+
+        end_time = int(datetime(today.year, today.month,
+                                today.day, hour=today.hour, minute=previous_interval_minute).timestamp())
+
+        instrument = self.get_instrument_by_symbol(exchange, symbol)
+
+        PARAMS = {
+            'candletype': 1,
+            'data_duration': interval,
+            'starttime': start_time,
+            'endtime': end_time,
+            'exchange': exchange,
+            'type': 'live',
+            'token': instrument.token
+        }
+
+        r = self.session.get(
+            'https://alpha.sasonline.in/api/v1/charts', params=PARAMS, headers=self.__headers)
+        data = r.json()
+        return self.__format_candles(data, divider)
+
+    def buy_bo(self, instrument, qty, price, trigger_price, stop_loss_value, square_off_value):
+        data = self.place_order(TransactionType.Buy, instrument, qty,
+                                OrderType.StopLossLimit, ProductType.BracketOrder,
+                                price=price, trigger_price=trigger_price, stop_loss=stop_loss_value,
+                                square_off=square_off_value, order_tag='python-buy-bo')
+        if data['status'] == 'success':
+            return data['data']['oms_order_id']
+        return data.json()
+
+    def sell_bo(self, instrument, qty, price, trigger_price, stop_loss_value, square_off_value):
+        data = self.place_order(TransactionType.Sell, instrument, qty,
+                                OrderType.StopLossLimit, ProductType.BracketOrder,
+                                price=price, trigger_price=trigger_price, stop_loss=stop_loss_value,
+                                square_off=square_off_value, order_tag='python-sell-bo')
+        if data['status'] == 'success':
+            return data['data']['oms_order_id']
+        return data.json()
+
+    def get_total_m2m(self):
+        """ Returns the total m2m of all positions.
+        Returns:
+            float: Total m2m of all positions.
+        """
+        data = self.positions(position_type='live')
+        if data['status'] != 'success':
+            return None
+        else:
+            positions = pd.DataFrame(data['data']['positions'], index=None)
+            if positions.empty:
+                return 0
+            positions['m2m'] = positions['m2m'].str.replace(
+                ',', '').astype(float)
+            return float(positions['m2m'].sum())
+
+    def _format_candles(self, data, interval):
+        records = data['data']['candles']
+        df = pd.DataFrame(records, columns=[
+            'datetime', 'open', 'high', 'low', 'close', 'volume'])  # , index=0)
+        df['datetime'] = df['datetime'].apply(
+            pd.Timestamp, unit='s', tzinfo=pytz.timezone('Asia/Kolkata'))
+
+        df[['open', 'high', 'low', 'close']] = df[[
+            'open', 'high', 'low', 'close']].astype(float)
+        df['volume'] = df['volume'].astype(int)
+        df.set_index('datetime', inplace=True)
+        if interval in ['2H', '3H', '4H', 'W', 'M']:
+            if interval == 'W':
+                interval = 'W-Mon'
+            df = df.resample(interval, origin='start').agg({'open': 'first', 'high': 'max',
+                                                            'low': 'min', 'close': 'last', 'volume': 'sum'}).dropna()
+        df.index = df.index.astype(str).str[:-6]
+        return df
+
+    def history(self, instrument, start_time=datetime.today() - timedelta(days=2), end_time=datetime.now(), interval=1, is_index=False):
+        exchange = instrument.exchange
+        start_time = int(start_time.timestamp())
+        end_time = int(end_time.timestamp())
+        if is_index:
+            exchange = 'NSE_INDICES'
+
+        candle_type = self._candle_type[interval]
+
+        data_duration = self._data_duration[interval]
+
+        PARAMS = {
+            'exchange': exchange,
+            'token': instrument.token,
+            'name': instrument.symbol,
+            'candletype': candle_type,
+            'starttime': start_time,
+            'endtime': end_time,
+            'type': 'all'
+        }
+        if data_duration is not None:
+            PARAMS['data_duration'] = data_duration
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Connection': 'Keep-Alive',
+            'Accept': 'application/json'
+        }
+        r = requests.get(
+            'https://alpha.sasonline.in/api/v1/charts/tdv', params=PARAMS, headers=headers)
+        data = r.json()
+        return self._format_candles(data, interval)
```

### Comparing `alphatrade-0.1.3/alphatrade/exceptions.py` & `alphatrade-1.0.0/alphatrade/exceptions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# -*- coding: utf-8 -*-
-"""
-    exceptions.py
-
-    Exceptions raised by the Alpha Trade client.
-
-    :license: see LICENSE for details.
-"""
-
-
-class AlphaException(Exception):
-    """
-    Base exception class representing a Alpha Trade client exception.
-
-    Every specific Alpha Trade client exception is a subclass of this
-    and  exposes two instance variables `.code` (HTTP error code)
-    and `.message` (error text).
-    """
-
-    def __init__(self, message, code=500):
-        """Initialize the exception."""
-        super(AlphaException, self).__init__(message)
-        self.code = code
-
-
-class GeneralException(AlphaException):
-    """An unclassified, general error. Default code is 500."""
-
-    def __init__(self, message, code=500):
-        """Initialize the exception."""
-        super(GeneralException, self).__init__(message, code)
-
-
-class TokenException(AlphaException):
-    """Represents all token and authentication related errors. Default code is 403."""
-
-    def __init__(self, message, code=403):
-        """Initialize the exception."""
-        super(TokenException, self).__init__(message, code)
-
-
-class PermissionException(AlphaException):
-    """Represents permission denied exceptions for certain calls. Default code is 403."""
-
-    def __init__(self, message, code=403):
-        """Initialize the exception."""
-        super(PermissionException, self).__init__(message, code)
-
-
-class OrderException(AlphaException):
-    """Represents all order placement and manipulation errors. Default code is 500."""
-
-    def __init__(self, message, code=500):
-        """Initialize the exception."""
-        super(OrderException, self).__init__(message, code)
-
-
-class InputException(AlphaException):
-    """Represents user input errors such as missing and invalid parameters. Default code is 400."""
-
-    def __init__(self, message, code=400):
-        """Initialize the exception."""
-        super(InputException, self).__init__(message, code)
-
-
-class DataException(AlphaException):
-    """Represents a bad response from the backend Order Management System (OMS). Default code is 502."""
-
-    def __init__(self, message, code=502):
-        """Initialize the exception."""
-        super(DataException, self).__init__(message, code)
-
-
-class NetworkException(AlphaException):
-    """Represents a network issue between Alpha Trade and the backend Order Management System (OMS). Default code is 503."""
-
-    def __init__(self, message, code=503):
-        """Initialize the exception."""
-        super(NetworkException, self).__init__(message, code)
+# -*- coding: utf-8 -*-
+"""
+    exceptions.py
+
+    Exceptions raised by the Alpha Trade client.
+
+    :license: see LICENSE for details.
+"""
+
+
+class AlphaException(Exception):
+    """
+    Base exception class representing a Alpha Trade client exception.
+
+    Every specific Alpha Trade client exception is a subclass of this
+    and  exposes two instance variables `.code` (HTTP error code)
+    and `.message` (error text).
+    """
+
+    def __init__(self, message, code=500):
+        """Initialize the exception."""
+        super(AlphaException, self).__init__(message)
+        self.code = code
+
+
+class GeneralException(AlphaException):
+    """An unclassified, general error. Default code is 500."""
+
+    def __init__(self, message, code=500):
+        """Initialize the exception."""
+        super(GeneralException, self).__init__(message, code)
+
+
+class TokenException(AlphaException):
+    """Represents all token and authentication related errors. Default code is 403."""
+
+    def __init__(self, message, code=403):
+        """Initialize the exception."""
+        super(TokenException, self).__init__(message, code)
+
+
+class PermissionException(AlphaException):
+    """Represents permission denied exceptions for certain calls. Default code is 403."""
+
+    def __init__(self, message, code=403):
+        """Initialize the exception."""
+        super(PermissionException, self).__init__(message, code)
+
+
+class OrderException(AlphaException):
+    """Represents all order placement and manipulation errors. Default code is 500."""
+
+    def __init__(self, message, code=500):
+        """Initialize the exception."""
+        super(OrderException, self).__init__(message, code)
+
+
+class InputException(AlphaException):
+    """Represents user input errors such as missing and invalid parameters. Default code is 400."""
+
+    def __init__(self, message, code=400):
+        """Initialize the exception."""
+        super(InputException, self).__init__(message, code)
+
+
+class DataException(AlphaException):
+    """Represents a bad response from the backend Order Management System (OMS). Default code is 502."""
+
+    def __init__(self, message, code=502):
+        """Initialize the exception."""
+        super(DataException, self).__init__(message, code)
+
+
+class NetworkException(AlphaException):
+    """Represents a network issue between Alpha Trade and the backend Order Management System (OMS). Default code is 503."""
+
+    def __init__(self, message, code=503):
+        """Initialize the exception."""
+        super(NetworkException, self).__init__(message, code)
```

### Comparing `alphatrade-0.1.3/alphatrade.egg-info/PKG-INFO` & `alphatrade-1.0.0/alphatrade.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,802 +1,851 @@
-Metadata-Version: 2.1
-Name: alphatrade
-Version: 0.1.3
-Summary: Python APIs for SAS Online Alpha Trade Web Platform
-Home-page: https://github.com/algo2t/alphatrade
-Author: Algo 2 Trade
-Author-email: help@algo2.trade
-License: UNKNOWN
-Keywords: alphatrade,alpha-trade,sasonline,python,sdk,trading,stock markets
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python APIs for SAS Online Alpha Trade Web Platform
-# NOTE:: This is Unofficial python module, don't ask SAS support team for help, use it AS-IS
-
-The Python APIs for communicating with the SAS Online Alpha Trade Web Platform.
-
-Alpha Trade Python library provides an easy to use python wrapper over the HTTPS APIs.
-
-The HTTP calls have been converted to methods and JSON responses are wrapped into Python-compatible objects.
-
-Websocket connections are handled automatically within the library.
-
-This work is completely based on Python SDK / APIs for [AliceBlueOnline](https://github.com/krishnavelu/alice_blue.git).  
-Thanks to [krishnavelu](https://github.com/krishnavelu/).  
-
-- **Author: [algo2t](https://github.com/algo2t/)**
-- **Github Repository: [alphatrade](https://github.com/algo2t/alphatrade.git)**
-
-## Installation
-
-This module is installed via pip:
-
-```
-pip install git+https://github.com/algo2t/alphatrade.git
-```
-
-It can also be installed from [pypi](https://pypi.org/project/alphatrade/0.1.2/)  
-
-```
-pip install alphatrade
-```
-
-To force upgrade existing installations:
-
-```
-pip uninstall alphatrade
-pip --no-cache-dir install --upgrade alphatrade
-```
-
-### Prerequisites
-
-Python 3.x
-
-Also, you need the following modules:
-
-- `protlib`
-- `websocket_client`
-- `requests`
-- `pandas`
-
-The modules can also be installed using `pip`
-
-## Examples - Start Here - Important 
-
-Please clone this repository and check the examples folder to get started.  
-Check [here](https://algo2t.github.io/alphatrade/#working-with-examples)
-
-## Getting started with API
-
-### Overview
-
-There is only one class in the whole library: `AlphaTrade`. When the `AlphaTrade` object is created an access token from the SAS Online alpha trade server is stored in text file `access_token.txt` in the same directory. An access token is valid for 24 hours. See the examples folder with `config.py` file to see how to store your credentials.
-With an access token, you can instantiate an AlphaTrade object again. Ideally you only need to create an access_token once every day.
-
-### REST Documentation
-
-The original REST API that this SDK is based on is available online.
-[Alice Blue API REST documentation](http://antplus.aliceblueonline.com/#introduction)
-
-## Using the API
-
-### Logging
-
-The whole library is equipped with pythonâ€˜s `logging` module for debugging. If more debug information is needed, enable logging using the following code.
-
-```python
-import logging
-logging.basicConfig(level=logging.DEBUG)
-```
-
-### Get an access token
-
-1. Import alphatrade
-
-```python
-from alphatrade import *
-```
-
-2. Create `config.py` file  
-Always keep credentials in a separate file
-```python
-login_id = "RR249"
-password = "SAS@249"
-twofa = "rr"
-
-try:
-    access_token = open('access_token.txt', 'r').read().rstrip()
-except Exception as e:
-    print('Exception occurred :: {}'.format(e))
-    access_token = None
-```
-
-3. Import the config
-```python
-import config
-```
-
-### Create AlphaTrade Object
-
-1. Create `AlphaTrade` object with your `login_id`, `password`, `2FA` and/or `access_token`.
-
-Use `config` object to get `login_id`, `password`, `twofa` and `access_token`.  
-
-```python
-from alphatrade import AlphaTrade
-import config
-sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.twofa, access_token=config.access_token)
-```
-
-2. You can run commands here to check your connectivity
-
-```python
-print(sas.get_balance()) # get balance / margin limits
-print(sas.get_profile()) # get profile
-print(sas.get_daywise_positions()) # get daywise positions
-print(sas.get_netwise_positions()) # get netwise positions
-print(sas.get_holding_positions()) # get holding positions
-```
-
-### Get master contracts
-
-Getting master contracts allow you to search for instruments by symbol name and place orders.
-Master contracts are stored as an OrderedDict by token number and by symbol name. Whenever you get a trade update, order update, or quote update, the library will check if master contracts are loaded. If they are, it will attach the instrument object directly to the update. By default all master contracts of all enabled exchanges in your personal profile will be downloaded. i.e. If your profile contains the following as enabled exchanges `['NSE', 'BSE', 'CDS', 'MCX', NFO']` all contract notes of all exchanges will be downloaded by default. If you feel it takes too much time to download all exchange, or if you donâ€˜t need all exchanges to be downloaded, you can specify which exchange to download contract notes while creating the AlphaTrade object.
-
-```python
-sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.twofa, access_token=config.access_token, master_contracts_to_download=['NSE', 'BSE'])
-```
-
-This will reduce a few milliseconds in object creation time of AlphaTrade object.
-
-### Get tradable instruments
-
-Symbols can be retrieved in multiple ways. Once you have the master contract loaded for an exchange, you can get an instrument in many ways.
-
-Get a single instrument by itâ€˜s name:
-
-```python
-tatasteel_nse_eq = sas.get_instrument_by_symbol('NSE', 'TATASTEEL')
-reliance_nse_eq = sas.get_instrument_by_symbol('NSE', 'RELIANCE')
-ongc_bse_eq = sas.get_instrument_by_symbol('BSE', 'ONGC')
-india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
-sensex_nse_index = sas.get_instrument_by_symbol('BSE', 'SENSEX')
-```
-
-Get a single instrument by itâ€˜s token number (generally useful only for BSE Equities):
-
-```python
-ongc_bse_eq = sas.get_instrument_by_token('BSE', 500312)
-reliance_bse_eq = sas.get_instrument_by_token('BSE', 500325)
-acc_nse_eq = sas.get_instrument_by_token('NSE', 22)
-```
-
-Get FNO instruments easily by mentioning expiry, strike & call or put.
-
-```python
-bn_fut = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=True, strike=None, is_call = False)
-bn_call = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = True)
-bn_put = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = False)
-```
-
-### Search for symbols
-
-Search for multiple instruments by matching the name. This works case insensitive and returns all instrument which has the name in its symbol.
-
-```python
-all_sensex_scrips = sas.search_instruments('BSE', 'sEnSeX')
-print(all_sensex_scrips)
-```
-
-The above code results multiple symbol which has â€˜sensexâ€™ in its symbol.
-
-```
-[Instrument(exchange='BSE', token=1, symbol='SENSEX', name='SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=540154, symbol='IDFSENSEXE B', name='IDFC Mutual Fund', expiry=None, lot_size=None), Instrument(exchange='BSE', token=532985, symbol='KTKSENSEX B', name='KOTAK MAHINDRA MUTUAL FUND', expiry=None, lot_size=None), Instrument(exchange='BSE', token=538683, symbol='NETFSENSEX B', name='NIPPON INDIA ETF SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=535276, symbol='SBISENSEX B', name='SBI MUTUAL FUND - SBI ETF SENS', expiry=None, lot_size=None)]
-```
-
-Search for multiple instruments by matching multiple names
-
-```python
-multiple_underlying = ['BANKNIFTY','NIFTY','INFY','BHEL']
-all_scripts = sas.search_instruments('NFO', multiple_underlying)
-```
-
-#### Instrument object
-
-Instruments are represented by instrument objects. These are named-tuples that are created while getting the master contracts. They are used when placing an order and searching for an instrument. The structure of an instrument tuple is as follows:
-
-```python
-Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
-                                      'name', 'expiry', 'lot_size'])
-```
-
-All instruments have the fields mentioned above. Wherever a field is not applicable for an instrument (for example, equity instruments donâ€˜t have strike prices), that value will be `None`
-
-### Quote update
-
-Once you have master contracts loaded, you can easily subscribe to quote updates.
-
-#### Four types of feed data are available
-
-You can subscribe any one type of quote update for a given scrip. Using the `LiveFeedType` enum, you can specify what type of live feed you need.
-
-- `LiveFeedType.MARKET_DATA`
-- `LiveFeedType.COMPACT`
-- `LiveFeedType.SNAPQUOTE`
-- `LiveFeedType.FULL_SNAPQUOTE`
-
-Please refer to the original documentation [here](http://antplus.aliceblueonline.com/#marketdata) for more details of different types of quote update.
-
-#### Subscribe to a live feed
-
-```python
-sas.subscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
-sas.subscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
-```
-
-Subscribe to multiple instruments in a single call. Give an array of instruments to be subscribed.
-
-```python
-sas.subscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
-```
-
-Note: There is a limit of 250 scrips that can be subscribed on total. Beyond this point the server may disconnect web-socket connection.
-
-Start getting live feed via socket
-
-```python
-socket_opened = False
-def event_handler_quote_update(message):
-    print(f"quote update {message}")
-
-def open_callback():
-    global socket_opened
-    socket_opened = True
-
-sas.start_websocket(subscribe_callback=event_handler_quote_update,
-                      socket_open_callback=open_callback,
-                      run_in_background=True)
-while(socket_opened==False):
-    pass
-sas.subscribe(sas.get_instrument_by_symbol('NSE', 'ONGC'), LiveFeedType.MARKET_DATA)
-sleep(10)
-```
-
-#### Unsubscribe to a live feed
-
-Unsubscribe to an existing live feed
-
-```python
-sas.unsubscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
-sas.unsubscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
-```
-
-Unsubscribe to multiple instruments in a single call. Give an array of instruments to be unsubscribed.
-
-```python
-sas.unsubscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
-```
-
-#### Get All Subscribed Symbols
-
-```python
-sas.get_all_subscriptions() # All
-```
-
-### Market Status messages & Exchange messages.
-
-Subscribe to market status messages
-
-```python
-sas.subscribe_market_status_messages()
-```
-
-Getting market status messages.
-
-```python
-print(sas.get_market_status_messages())
-```
-
-Example result of `get_market_status_messages()`
-
-```
-[{'exchange': 'NSE', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 31, 'status': b'The Closing Session has closed.'}, {'exchange': 'NFO', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'CDS', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'BSE', 'length_of_market_type': 13, 'market_type': b'OTHER SESSION', 'length_of_status': 0, 'status': b''}]
-```
-
-Note: As per `alice blue` [documentation](http://antplus.aliceblueonline.com/#market-status) all market status messages should be having a timestamp. But in actual the server doesnâ€˜t send timestamp, so the library is unable to get timestamp for now.
-
-Subscribe to exchange messages
-
-```python
-sas.subscribe_exchange_messages()
-```
-
-Getting market status messages.
-
-```python
-print(sas.get_exchange_messages())
-```
-
-Example result of `get_exchange_messages()`
-
-```
-[{'exchange': 'NSE', 'length': 32, 'message': b'DS : Bulk upload can be started.', 'exchange_time_stamp': 1590148595}, {'exchange': 'NFO', 'length': 200, 'message': b'MARKET WIDE LIMIT FOR VEDL IS 183919959. OPEN POSITIONS IN VEDL HAVE REACHED 84 PERCENT OF THE MARKET WIDE LIMIT.                                                                                       ', 'exchange_time_stamp': 1590146132}, {'exchange': 'CDS', 'length': 54, 'message': b'DS : Regular segment Bhav copy broadcast successfully.', 'exchange_time_stamp': 1590148932}, {'exchange': 'MCX', 'length': 7, 'message': b'.......', 'exchange_time_stamp': 1590196159}]
-```
-
-#### Market Status messages & Exchange messages through callbacks
-
-```python
-socket_opened = False
-def market_status_messages(message):
-    print(f"market status messages {message}")
-
-def exchange_messages(message):
-    print(f"exchange messages {message}")
-
-def open_callback():
-    global socket_opened
-    socket_opened = True
-
-sas.start_websocket(market_status_messages_callback=market_status_messages,
-					  exchange_messages_callback=exchange_messages,
-                      socket_open_callback=open_callback,
-                      run_in_background=True)
-while(socket_opened==False):
-    pass
-sas.subscribe_market_status_messages()
-sas.subscribe_exchange_messages()
-sleep(10)
-```
-
-### Place an order
-
-Place limit, market, SL, SL-M, AMO, BO, CO orders
-
-```python
-print (sas.get_profile())
-
-# TransactionType.Buy, OrderType.Market, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%1%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.Delivery,
-                     price = 0.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-   )
-
-# TransactionType.Buy, OrderType.Market, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%2%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.Intraday,
-                     price = 0.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-# TransactionType.Buy, OrderType.Market, ProductType.CoverOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%3%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Market,
-                     product_type = ProductType.CoverOrder,
-                     price = 0.0,
-                     trigger_price = 7.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.Limit, ProductType.BracketOrder
-# OCO Order can't be of type market
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%4%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.BracketOrder,
-                     price = 8.0,
-                     trigger_price = None,
-                     stop_loss = 6.0,
-                     square_off = 10.0,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-# TransactionType.Buy, OrderType.Limit, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%5%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.Intraday,
-                     price = 8.0,
-                     trigger_price = None,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.Limit, ProductType.CoverOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%6%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.Limit,
-                     product_type = ProductType.CoverOrder,
-                     price = 7.0,
-                     trigger_price = 6.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-###############################
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%7%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Delivery,
-                     price = 0.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%8%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Intraday,
-                     price = 0.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.CoverOrder
-# CO order is of type Limit and And Market Only
-
-# TransactionType.Buy, OrderType.StopLossMarket, ProductType.BO
-# BO order is of type Limit and And Market Only
-
-###################################
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Delivery
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%9%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossMarket,
-                     product_type = ProductType.Delivery,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Intraday
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%10%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossLimit,
-                     product_type = ProductType.Intraday,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = None,
-                     square_off = None,
-                     trailing_sl = None,
-                     is_amo = False)
-)
-
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.CoverOrder
-# CO order is of type Limit and And Market Only
-
-
-# TransactionType.Buy, OrderType.StopLossLimit, ProductType.BracketOrder
-
-print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%11%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-print(
-   sas.place_order(transaction_type = TransactionType.Buy,
-                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
-                     quantity = 1,
-                     order_type = OrderType.StopLossLimit,
-                     product_type = ProductType.BracketOrder,
-                     price = 8.0,
-                     trigger_price = 8.0,
-                     stop_loss = 1.0,
-                     square_off = 1.0,
-                     trailing_sl = 20,
-                     is_amo = False)
-)
-```
-
-### Place basket order
-
-Basket order is used to buy or sell group of securities simultaneously.
-
-```python
-order1 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'INFY'),
-            "order_type"        : OrderType.Market,
-            "quantity"          : 1,
-            "transaction_type"  : TransactionType.Buy,
-            "product_type"      : ProductType.Delivery}
-order2 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'SBIN'),
-            "order_type"        : OrderType.Limit,
-            "quantity"          : 2,
-            "price"             : 280.0,
-            "transaction_type"  : TransactionType.Sell,
-            "product_type"      : ProductType.Intraday}
-order = [order1, order2]
-print(sas.place_basket_order(orders))
-```
-
-### Cancel an order
-
-```python
-sas.cancel_order('170713000075481') #Cancel an open order
-```
-
-### Getting order history and trade details
-
-#### Get order history of a particular order
-
-```python
-print(sas.get_order_history('170713000075481'))
-```
-
-#### Get order history of all orders.
-
-```python
-print(sas.get_order_history())
-```
-
-#### Get trade book
-
-```python
-print(sas.get_trade_book())
-```
-
-#### Get historical candles data
-
-This will provide historical data but **not for current day**.  
-This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
-
-```python
-from datetime import datetime
-print(sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', datetime(2020, 10, 19), datetime.now() ,interval=30))
-```
-
-Output 
-
-```console
-Instrument(exchange='MCX', token=224365, symbol='NATURALGAS NOV FUT', name='', expiry=datetime.date(2020, 11, 24), lot_size=None)
-                            open   high    low  close  volume
-date
-2020-10-19 09:00:00+05:30  238.9  239.2  238.4  239.0     373
-2020-10-19 09:30:00+05:30  239.0  239.0  238.4  238.6     210
-2020-10-19 10:00:00+05:30  238.7  238.7  238.1  238.1     213
-2020-10-19 10:30:00+05:30  238.0  238.4  238.0  238.1     116
-2020-10-19 11:00:00+05:30  238.1  238.2  238.0  238.0      69
-...                          ...    ...    ...    ...     ...
-2020-10-23 21:00:00+05:30  237.5  238.1  237.3  237.6     331
-2020-10-23 21:30:00+05:30  237.6  238.5  237.6  237.9     754
-2020-10-23 22:00:00+05:30  237.9  238.1  237.2  237.9     518
-2020-10-23 22:30:00+05:30  237.9  238.7  237.7  238.1     897
-2020-10-23 23:00:00+05:30  238.2  238.3  236.3  236.5    1906
-
-```
-
-Better way to get historical data, first get the latest version from github  
-
-`python -m pip install git+https://github.com/algo2t/alphatrade.git`
-
-```python
-from datetime import datetime
-india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
-print(sas.get_historical_candles(india_vix_nse_index.exchange, india_vix_nse_index.symbol, datetime(2020, 10, 19), datetime.now() ,interval=30))
-```
-
-
-#### Get intraday candles data
-
-This will give candles data for **current day only**.  
-This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
-
-```python
-print(sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', interval=15))
-```
-
-Better way to get intraday data, first get the latest version from github  
-
-`python -m pip install git+https://github.com/algo2t/alphatrade.git`
-
-```python
-from datetime import datetime
-nifty_bank_nse_index = sas.get_instrument_by_symbol('NSE', 'Nifty Bank')
-print(sas.get_intraday_candles(nifty_bank_nse_index.exchange, nifty_bank_nse_index.symbol, datetime(2020, 10, 19), datetime.now(), interval=10))
-```
-
-### Order properties as enums
-
-Order properties such as TransactionType, OrderType, and others have been safely classified as enums so you donâ€˜t have to write them out as strings
-
-#### TransactionType
-
-Transaction types indicate whether you want to buy or sell. Valid transaction types are of the following:
-
-- `TransactionType.Buy` - buy
-- `TransactionType.Sell` - sell
-
-#### OrderType
-
-Order type specifies the type of order you want to send. Valid order types include:
-
-- `OrderType.Market` - Place the order with a market price
-- `OrderType.Limit` - Place the order with a limit price (limit price parameter is mandatory)
-- `OrderType.StopLossLimit` - Place as a stop loss limit order
-- `OrderType.StopLossMarket` - Place as a stop loss market order
-
-#### ProductType
-
-Product types indicate the complexity of the order you want to place. Valid product types are:
-
-- `ProductType.Intraday` - Intraday order that will get squared off before market close
-- `ProductType.Delivery` - Delivery order that will be held with you after market close
-- `ProductType.CoverOrder` - Cover order
-- `ProductType.BracketOrder` - One cancels other order. Also known as bracket order
-
-## Working with examples
-
-[Here](https://github.com/algo2t/alphatrade/tree/main/examples), examples directory there are 3 files `sas_login_eg.py`, `streaming_data.py` and `stop.txt`
-
-### Steps
-
-- Clone the repository to your local machine `git clone https://github.com/algo2t/alphatrade.git`
-- Copy the examples directory to any location where you want to write your code
-- Install the `alphatrade` module using `pip` => `python -m pip install https://github.com/algo2t/alphatrade.git`
-- Open the examples directory in your favorite editor, in our case it is [VSCodium](https://vscodium.com/)
-- Open the `sas_login_eg.py` file in the editor
-- Now, create `config.py` file as per instructions given below and in the above file
-- Provide correct login credentials like login_id, password and twofa
-- twofa must be same for all questions under two factor authentication
-- This is generally set from the homepage of alpha web trading platform [here](https://alpha.sasonline.in/)
-- Click on `FORGET PASSWORD?` => Select `Reset 2FA` radio button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/forget_password.png)
-- Enter the CLIENT ID (LOGIN_ID), EMAIL ID and PAN NUMBER, click on `RESET` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/reset_two_fa.png)
-- Click on `BACK TO LOGIN` and enter `CLIENT ID` and `PASSWORD`, click on `SECURED SIGN-IN`
-- Set same answers for 5 questions and click on `SUBMIT` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/set_answers.png)
-
-`config.py`
-```python
-login_id = "RR249"
-password = "SAS@249"
-twofa = "rr"
-
-try:
-    access_token = open('access_token.txt', 'r').read().rstrip()
-except Exception as e:
-    print('Exception occurred :: {}'.format(e))
-    access_token = None
-
-```
-
-## Example strategy using alpha trade API
-
-[Here](https://github.com/algo2t/alphatrade/blob/main/examples/streaming_data.py) is an example moving average strategy using alpha trade web API.
-This strategy generates a buy signal when 5-EMA > 20-EMA (golden cross) or a sell signal when 5-EMA < 20-EMA (death cross).
-
-## Example for getting historical and intraday candles data
-
-[Here](https://github.com/algo2t/alphatrade/blob/main/examples/historical_data.py) is an example for getting historical data using alpha trade web API.
-
-For historical candles data `start_time` and `end_time` must be provided in format as shown below.
-It can also be provided as `timedelta`. Check the script `historical_data.py` in examples.
-
-```python
-from datetime import datetime, timedelta
-start_time = datetime(2020, 10, 19, 9, 15, 0)
-end_time = datetime(2020, 10, 21, 16, 59, 0)
-
-df = sas.get_historical_candles('MCX', 'NATURALGAS OCT FUT', start_time, end_time, 5)
-print(df)
-end_time = start_time + timedelta(days=5)
-df = sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', start_time, end_time, 15)
-print(df)
-```
-
-For intraday or todayâ€˜s / current dayâ€˜s candles data.  
-
-```python
-df = sas.get_intraday_candles('MCX', 'NATURALGAS OCT FUT')
-print(df)
-df = sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', 15)
-print(df)
-```
-
-
-## Read this before creating an issue
-
-Before creating an issue in this library, please follow the following steps.
-
-1. Search the problem you are facing is already asked by someone else. There might be some issues already there, either solved/unsolved related to your problem. Go to [issues](https://github.com/algo2t/alphatrade/issues) page, use `is:issue` as filter and search your problem. ![image](https://user-images.githubusercontent.com/38440742/85207058-376ee400-b2f4-11ea-91ad-c8fd8a682a12.png)
-2. If you feel your problem is not asked by anyone or no issues are related to your problem, then create a new issue.
-3. Describe your problem in detail while creating the issue. If you donâ€˜t have time to detail/describe the problem you are facing, assume that I also wonâ€˜t be having time to respond to your problem.
-4. Post a sample code of the problem you are facing. If I copy paste the code directly from issue, I should be able to reproduce the problem you are facing.
-5. Before posting the sample code, test your sample code yourself once. Only sample code should be tested, no other addition should be there while you are testing.
-6. Have some print() function calls to display the values of some variables related to your problem.
-7. Post the results of print() functions also in the issue.
-8. Use the insert code feature of github to inset code and print outputs, so that the code is displayed neat. ![image](https://user-images.githubusercontent.com/38440742/85207234-4dc96f80-b2f5-11ea-990c-df013dd69cf2.png)
-
-
+Metadata-Version: 2.1
+Name: alphatrade
+Version: 1.0.0
+Summary: Python APIs for SAS Online Alpha Trade Web Platform
+Home-page: https://github.com/algo2t/alphatrade
+Author: Algo 2 Trade
+Author-email: help@algo2.trade
+License: UNKNOWN
+Keywords: alphatrade,alpha-trade,sasonline,python,sdk,trading,stock markets
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python APIs for SAS Online Alpha Trade Web Platform
+
+# MAJOR CHANGES : NEW VERSION 1.0.0
+
+## API endpoints are changed to match the new ones, bugs expected
+
+1. Removed check for enabled exchanges, you can now download or search symbols from MCX as well if it is not enabled
+2. TOTP SECRET or TOTP both can be given as argument while creating AlphaTrade object (if it is 6 digits it will conside TOTP else TOTP SECRET)
+3. Added new search function to search scrips which will return json for found scrips, you need to process it further
+4. More functions to come.
+5. Check whether streaming websocket is working or not
+6. The `examples` folder is removed and examples are renamed and kept in root directory for ease of development
+
+# STEPS to work
+
+1. Clone the repo locally - `git clone https://github.com/algo2t/alphatrade.git` 
+2. Create a virtualenv - `python -m pip install virtualenv` and then `python -m virtualenv venv` and activate the `venv` environment.
+3. Install dev-requirement.txt - `python -m pip install -r dev-requirements.txt` - this is to ensure `setuptools==57.5.0` is installed. There is a bug with `protlib`, target is to get reed of `protlib` in future
+4. Install requirement.txt - `python -m pip install -r requirement.txt`
+5. Create the `config.py` file in root of cloned repo with `login_id`, `password` and `TOTP` SECRET, you can add the `access_token.txt` if you want to use existing `access_token`.
+6. Try the examples `python zlogin_example.py`, `python zexample_sas_login.py`, `python zhistorical_data.py` and `python zstreaming_data.py`
+7. Expecting issues with the streaming data !!! :P
+
+
+# NOTE:: This is Unofficial python module, don't ask SAS support team for help, use it AS-IS
+
+The Python APIs for communicating with the SAS Online Alpha Trade Web Platform.
+
+Alpha Trade Python library provides an easy to use python wrapper over the HTTPS APIs.
+
+The HTTP calls have been converted to methods and JSON responses are wrapped into Python-compatible objects.
+
+Websocket connections are handled automatically within the library.
+
+This work is completely based on Python SDK / APIs for [AliceBlueOnline](https://github.com/krishnavelu/alice_blue.git).  
+Thanks to [krishnavelu](https://github.com/krishnavelu/).  
+
+- **Author: [algo2t](https://github.com/algo2t/)**
+- **Github Repository: [alphatrade](https://github.com/algo2t/alphatrade.git)**
+
+## Installation
+
+This module is installed via pip:
+
+```
+pip install git+https://github.com/algo2t/alphatrade.git
+```
+
+It can also be installed from [pypi](https://pypi.org/project/alphatrade/0.1.2/)  
+
+```
+pip install alphatrade
+```
+
+To force upgrade existing installations:
+
+```
+pip uninstall alphatrade
+pip --no-cache-dir install --upgrade alphatrade
+```
+
+### Prerequisites
+
+Python 3.x
+
+Also, you need the following modules:
+
+- `protlib`
+- `websocket_client`
+- `requests`
+- `pandas`
+
+The modules can also be installed using `pip`
+
+## Examples - Start Here - Important 
+
+Please clone this repository and check the examples folder to get started.  
+Check [here](https://algo2t.github.io/alphatrade/#working-with-examples)
+
+## Getting started with API
+
+### Overview
+
+There is only one class in the whole library: `AlphaTrade`. When the `AlphaTrade` object is created an access token from the SAS Online alpha trade server is stored in text file `access_token.txt` in the same directory. An access token is valid for 24 hours. See the examples folder with `config.py` file to see how to store your credentials.
+With an access token, you can instantiate an AlphaTrade object again. Ideally you only need to create an access_token once every day.
+
+### REST Documentation
+
+The original REST API that this SDK is based on is available online.
+[Alice Blue API REST documentation](http://antplus.aliceblueonline.com/#introduction)
+
+## Using the API
+
+### Logging
+
+The whole library is equipped with python‘s `logging` module for debugging. If more debug information is needed, enable logging using the following code.
+
+```python
+import logging
+logging.basicConfig(level=logging.DEBUG)
+```
+
+### Get an access token
+
+1. Import alphatrade
+
+```python
+from alphatrade import *
+```
+
+2. Create `config.py` file  
+Always keep credentials in a separate file
+```python
+login_id = "XXXXX"
+password = "XXXXXXXX"
+Totp = 'XXXXXXXXXXXXXXXX'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print('Exception occurred :: {}'.format(e))
+    access_token = None
+```
+
+3. Import the config
+```python
+import config
+```
+
+### Create AlphaTrade Object
+
+1. Create `AlphaTrade` object with your `login_id`, `password`, `TOTP` / `TOTP_SECRET` and/or `access_token`.
+
+Use `config` object to get `login_id`, `password`, `TOTP` and `access_token`.  
+
+```python
+from alphatrade import AlphaTrade
+import config
+import pyotp
+Totp = config.Totp
+pin = pyotp.TOTP(Totp).now()
+totp = f"{int(pin):06d}" if len(pin) <=5 else pin   
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=totp, access_token=config.access_token)
+
+```
+
+```python
+## filename config.py
+
+login_id = "RR24XX"
+password = "SuperSecretPassword!!!"
+TOTP_SECRET = 'YOURTOTPSECRETEXTERNALAUTH'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print(f'Exception occurred :: {e}')
+    access_token = None
+
+```
+
+
+```python
+from alphatrade import AlphaTrade
+import config
+import pyotp
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=config.TOTP_SECRET, access_token=config.access_token)
+
+```
+
+
+2. You can run commands here to check your connectivity
+
+```python
+print(sas.get_balance()) # get balance / margin limits
+print(sas.get_profile()) # get profile
+print(sas.get_daywise_positions()) # get daywise positions
+print(sas.get_netwise_positions()) # get netwise positions
+print(sas.get_holding_positions()) # get holding positions
+```
+
+### Get master contracts
+
+Getting master contracts allow you to search for instruments by symbol name and place orders.
+Master contracts are stored as an OrderedDict by token number and by symbol name. Whenever you get a trade update, order update, or quote update, the library will check if master contracts are loaded. If they are, it will attach the instrument object directly to the update. By default all master contracts of all enabled exchanges in your personal profile will be downloaded. i.e. If your profile contains the following as enabled exchanges `['NSE', 'BSE', 'CDS', 'MCX', NFO']` all contract notes of all exchanges will be downloaded by default. If you feel it takes too much time to download all exchange, or if you don‘t need all exchanges to be downloaded, you can specify which exchange to download contract notes while creating the AlphaTrade object.
+
+```python
+sas = AlphaTrade(login_id=config.login_id, password=config.password, twofa=totp, access_token=config.access_token, master_contracts_to_download=['NSE', 'BSE'])
+```
+
+This will reduce a few milliseconds in object creation time of AlphaTrade object.
+
+### Get tradable instruments
+
+Symbols can be retrieved in multiple ways. Once you have the master contract loaded for an exchange, you can get an instrument in many ways.
+
+Get a single instrument by it‘s name:
+
+```python
+tatasteel_nse_eq = sas.get_instrument_by_symbol('NSE', 'TATASTEEL')
+reliance_nse_eq = sas.get_instrument_by_symbol('NSE', 'RELIANCE')
+ongc_bse_eq = sas.get_instrument_by_symbol('BSE', 'ONGC')
+india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
+sensex_nse_index = sas.get_instrument_by_symbol('BSE', 'SENSEX')
+```
+
+Get a single instrument by it‘s token number (generally useful only for BSE Equities):
+
+```python
+ongc_bse_eq = sas.get_instrument_by_token('BSE', 500312)
+reliance_bse_eq = sas.get_instrument_by_token('BSE', 500325)
+acc_nse_eq = sas.get_instrument_by_token('NSE', 22)
+```
+
+Get FNO instruments easily by mentioning expiry, strike & call or put.
+
+```python
+bn_fut = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=True, strike=None, is_call = False)
+bn_call = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = True)
+bn_put = sas.get_instrument_for_fno(symbol = 'BANKNIFTY', expiry_date=datetime.date(2019, 6, 27), is_fut=False, strike=30000, is_call = False)
+```
+
+### Search for symbols
+
+Search for multiple instruments by matching the name. This works case insensitive and returns all instrument which has the name in its symbol.
+
+```python
+all_sensex_scrips = sas.search_instruments('BSE', 'sEnSeX')
+print(all_sensex_scrips)
+```
+
+The above code results multiple symbol which has ‘sensex’ in its symbol.
+
+```
+[Instrument(exchange='BSE', token=1, symbol='SENSEX', name='SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=540154, symbol='IDFSENSEXE B', name='IDFC Mutual Fund', expiry=None, lot_size=None), Instrument(exchange='BSE', token=532985, symbol='KTKSENSEX B', name='KOTAK MAHINDRA MUTUAL FUND', expiry=None, lot_size=None), Instrument(exchange='BSE', token=538683, symbol='NETFSENSEX B', name='NIPPON INDIA ETF SENSEX', expiry=None, lot_size=None), Instrument(exchange='BSE', token=535276, symbol='SBISENSEX B', name='SBI MUTUAL FUND - SBI ETF SENS', expiry=None, lot_size=None)]
+```
+
+Search for multiple instruments by matching multiple names
+
+```python
+multiple_underlying = ['BANKNIFTY','NIFTY','INFY','BHEL']
+all_scripts = sas.search_instruments('NFO', multiple_underlying)
+```
+
+#### Instrument object
+
+Instruments are represented by instrument objects. These are named-tuples that are created while getting the master contracts. They are used when placing an order and searching for an instrument. The structure of an instrument tuple is as follows:
+
+```python
+Instrument = namedtuple('Instrument', ['exchange', 'token', 'symbol',
+                                      'name', 'expiry', 'lot_size'])
+```
+
+All instruments have the fields mentioned above. Wherever a field is not applicable for an instrument (for example, equity instruments don‘t have strike prices), that value will be `None`
+
+### Quote update
+
+Once you have master contracts loaded, you can easily subscribe to quote updates.
+
+#### Four types of feed data are available
+
+You can subscribe any one type of quote update for a given scrip. Using the `LiveFeedType` enum, you can specify what type of live feed you need.
+
+- `LiveFeedType.MARKET_DATA`
+- `LiveFeedType.COMPACT`
+- `LiveFeedType.SNAPQUOTE`
+- `LiveFeedType.FULL_SNAPQUOTE`
+
+Please refer to the original documentation [here](http://antplus.aliceblueonline.com/#marketdata) for more details of different types of quote update.
+
+#### Subscribe to a live feed
+
+```python
+sas.subscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
+sas.subscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
+```
+
+Subscribe to multiple instruments in a single call. Give an array of instruments to be subscribed.
+
+```python
+sas.subscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
+```
+
+Note: There is a limit of 250 scrips that can be subscribed on total. Beyond this point the server may disconnect web-socket connection.
+
+Start getting live feed via socket
+
+```python
+socket_opened = False
+def event_handler_quote_update(message):
+    print(f"quote update {message}")
+
+def open_callback():
+    global socket_opened
+    socket_opened = True
+
+sas.start_websocket(subscribe_callback=event_handler_quote_update,
+                      socket_open_callback=open_callback,
+                      run_in_background=True)
+while(socket_opened==False):
+    pass
+sas.subscribe(sas.get_instrument_by_symbol('NSE', 'ONGC'), LiveFeedType.MARKET_DATA)
+sleep(10)
+```
+
+#### Unsubscribe to a live feed
+
+Unsubscribe to an existing live feed
+
+```python
+sas.unsubscribe(sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), LiveFeedType.MARKET_DATA)
+sas.unsubscribe(sas.get_instrument_by_symbol('BSE', 'RELIANCE'), LiveFeedType.COMPACT)
+```
+
+Unsubscribe to multiple instruments in a single call. Give an array of instruments to be unsubscribed.
+
+```python
+sas.unsubscribe([sas.get_instrument_by_symbol('NSE', 'TATASTEEL'), sas.get_instrument_by_symbol('NSE', 'ACC')], LiveFeedType.MARKET_DATA)
+```
+
+#### Get All Subscribed Symbols
+
+```python
+sas.get_all_subscriptions() # All
+```
+
+### Market Status messages & Exchange messages.
+
+Subscribe to market status messages
+
+```python
+sas.subscribe_market_status_messages()
+```
+
+Getting market status messages.
+
+```python
+print(sas.get_market_status_messages())
+```
+
+Example result of `get_market_status_messages()`
+
+```
+[{'exchange': 'NSE', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 31, 'status': b'The Closing Session has closed.'}, {'exchange': 'NFO', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'CDS', 'length_of_market_type': 6, 'market_type': b'NORMAL', 'length_of_status': 45, 'status': b'The Normal market has closed for 22 MAY 2020.'}, {'exchange': 'BSE', 'length_of_market_type': 13, 'market_type': b'OTHER SESSION', 'length_of_status': 0, 'status': b''}]
+```
+
+Note: As per `alice blue` [documentation](http://antplus.aliceblueonline.com/#market-status) all market status messages should be having a timestamp. But in actual the server doesn‘t send timestamp, so the library is unable to get timestamp for now.
+
+Subscribe to exchange messages
+
+```python
+sas.subscribe_exchange_messages()
+```
+
+Getting market status messages.
+
+```python
+print(sas.get_exchange_messages())
+```
+
+Example result of `get_exchange_messages()`
+
+```
+[{'exchange': 'NSE', 'length': 32, 'message': b'DS : Bulk upload can be started.', 'exchange_time_stamp': 1590148595}, {'exchange': 'NFO', 'length': 200, 'message': b'MARKET WIDE LIMIT FOR VEDL IS 183919959. OPEN POSITIONS IN VEDL HAVE REACHED 84 PERCENT OF THE MARKET WIDE LIMIT.                                                                                       ', 'exchange_time_stamp': 1590146132}, {'exchange': 'CDS', 'length': 54, 'message': b'DS : Regular segment Bhav copy broadcast successfully.', 'exchange_time_stamp': 1590148932}, {'exchange': 'MCX', 'length': 7, 'message': b'.......', 'exchange_time_stamp': 1590196159}]
+```
+
+#### Market Status messages & Exchange messages through callbacks
+
+```python
+socket_opened = False
+def market_status_messages(message):
+    print(f"market status messages {message}")
+
+def exchange_messages(message):
+    print(f"exchange messages {message}")
+
+def open_callback():
+    global socket_opened
+    socket_opened = True
+
+sas.start_websocket(market_status_messages_callback=market_status_messages,
+					  exchange_messages_callback=exchange_messages,
+                      socket_open_callback=open_callback,
+                      run_in_background=True)
+while(socket_opened==False):
+    pass
+sas.subscribe_market_status_messages()
+sas.subscribe_exchange_messages()
+sleep(10)
+```
+
+### Place an order
+
+Place limit, market, SL, SL-M, AMO, BO, CO orders
+
+```python
+print (sas.get_profile())
+
+# TransactionType.Buy, OrderType.Market, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%1%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.Delivery,
+                     price = 0.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+   )
+
+# TransactionType.Buy, OrderType.Market, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%2%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.Intraday,
+                     price = 0.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+# TransactionType.Buy, OrderType.Market, ProductType.CoverOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%3%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Market,
+                     product_type = ProductType.CoverOrder,
+                     price = 0.0,
+                     trigger_price = 7.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.Limit, ProductType.BracketOrder
+# OCO Order can't be of type market
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%4%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.BracketOrder,
+                     price = 8.0,
+                     trigger_price = None,
+                     stop_loss = 6.0,
+                     square_off = 10.0,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+# TransactionType.Buy, OrderType.Limit, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%5%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.Intraday,
+                     price = 8.0,
+                     trigger_price = None,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.Limit, ProductType.CoverOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%6%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.Limit,
+                     product_type = ProductType.CoverOrder,
+                     price = 7.0,
+                     trigger_price = 6.5, # trigger_price Here the trigger_price is taken as stop loss (provide stop loss in actual amount)
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+###############################
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%7%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Delivery,
+                     price = 0.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%8%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Intraday,
+                     price = 0.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.CoverOrder
+# CO order is of type Limit and And Market Only
+
+# TransactionType.Buy, OrderType.StopLossMarket, ProductType.BO
+# BO order is of type Limit and And Market Only
+
+###################################
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Delivery
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%9%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossMarket,
+                     product_type = ProductType.Delivery,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.Intraday
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%10%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossLimit,
+                     product_type = ProductType.Intraday,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = None,
+                     square_off = None,
+                     trailing_sl = None,
+                     is_amo = False)
+)
+
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.CoverOrder
+# CO order is of type Limit and And Market Only
+
+
+# TransactionType.Buy, OrderType.StopLossLimit, ProductType.BracketOrder
+
+print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%11%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+print(
+   sas.place_order(transaction_type = TransactionType.Buy,
+                     instrument = sas.get_instrument_by_symbol('NSE', 'INFY'),
+                     quantity = 1,
+                     order_type = OrderType.StopLossLimit,
+                     product_type = ProductType.BracketOrder,
+                     price = 8.0,
+                     trigger_price = 8.0,
+                     stop_loss = 1.0,
+                     square_off = 1.0,
+                     trailing_sl = 20,
+                     is_amo = False)
+)
+```
+
+### Place basket order
+
+Basket order is used to buy or sell group of securities simultaneously.
+
+```python
+order1 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'INFY'),
+            "order_type"        : OrderType.Market,
+            "quantity"          : 1,
+            "transaction_type"  : TransactionType.Buy,
+            "product_type"      : ProductType.Delivery}
+order2 = {  "instrument"        : sas.get_instrument_by_symbol('NSE', 'SBIN'),
+            "order_type"        : OrderType.Limit,
+            "quantity"          : 2,
+            "price"             : 280.0,
+            "transaction_type"  : TransactionType.Sell,
+            "product_type"      : ProductType.Intraday}
+order = [order1, order2]
+print(sas.place_basket_order(orders))
+```
+
+### Cancel an order
+
+```python
+sas.cancel_order('170713000075481') #Cancel an open order
+```
+
+### Getting order history and trade details
+
+#### Get order history of a particular order
+
+```python
+print(sas.get_order_history('170713000075481'))
+```
+
+#### Get order history of all orders.
+
+```python
+print(sas.get_order_history())
+```
+
+#### Get trade book
+
+```python
+print(sas.get_trade_book())
+```
+
+#### Get historical candles data
+
+This will provide historical data but **not for current day**.  
+This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
+
+```python
+from datetime import datetime
+print(sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', datetime(2020, 10, 19), datetime.now() ,interval=30))
+```
+
+Output 
+
+```console
+Instrument(exchange='MCX', token=224365, symbol='NATURALGAS NOV FUT', name='', expiry=datetime.date(2020, 11, 24), lot_size=None)
+                            open   high    low  close  volume
+date
+2020-10-19 09:00:00+05:30  238.9  239.2  238.4  239.0     373
+2020-10-19 09:30:00+05:30  239.0  239.0  238.4  238.6     210
+2020-10-19 10:00:00+05:30  238.7  238.7  238.1  238.1     213
+2020-10-19 10:30:00+05:30  238.0  238.4  238.0  238.1     116
+2020-10-19 11:00:00+05:30  238.1  238.2  238.0  238.0      69
+...                          ...    ...    ...    ...     ...
+2020-10-23 21:00:00+05:30  237.5  238.1  237.3  237.6     331
+2020-10-23 21:30:00+05:30  237.6  238.5  237.6  237.9     754
+2020-10-23 22:00:00+05:30  237.9  238.1  237.2  237.9     518
+2020-10-23 22:30:00+05:30  237.9  238.7  237.7  238.1     897
+2020-10-23 23:00:00+05:30  238.2  238.3  236.3  236.5    1906
+
+```
+
+Better way to get historical data, first get the latest version from github  
+
+`python -m pip install git+https://github.com/algo2t/alphatrade.git`
+
+```python
+from datetime import datetime
+india_vix_nse_index = sas.get_instrument_by_symbol('NSE', 'India VIX')
+print(sas.get_historical_candles(india_vix_nse_index.exchange, india_vix_nse_index.symbol, datetime(2020, 10, 19), datetime.now() ,interval=30))
+```
+
+
+#### Get intraday candles data
+
+This will give candles data for **current day only**.  
+This returns a `pandas` `DataFrame` object which be used with `pandas_ta` to get various indicators values.  
+
+```python
+print(sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', interval=15))
+```
+
+Better way to get intraday data, first get the latest version from github  
+
+`python -m pip install git+https://github.com/algo2t/alphatrade.git`
+
+```python
+from datetime import datetime
+nifty_bank_nse_index = sas.get_instrument_by_symbol('NSE', 'Nifty Bank')
+print(sas.get_intraday_candles(nifty_bank_nse_index.exchange, nifty_bank_nse_index.symbol, datetime(2020, 10, 19), datetime.now(), interval=10))
+```
+
+### Order properties as enums
+
+Order properties such as TransactionType, OrderType, and others have been safely classified as enums so you don‘t have to write them out as strings
+
+#### TransactionType
+
+Transaction types indicate whether you want to buy or sell. Valid transaction types are of the following:
+
+- `TransactionType.Buy` - buy
+- `TransactionType.Sell` - sell
+
+#### OrderType
+
+Order type specifies the type of order you want to send. Valid order types include:
+
+- `OrderType.Market` - Place the order with a market price
+- `OrderType.Limit` - Place the order with a limit price (limit price parameter is mandatory)
+- `OrderType.StopLossLimit` - Place as a stop loss limit order
+- `OrderType.StopLossMarket` - Place as a stop loss market order
+
+#### ProductType
+
+Product types indicate the complexity of the order you want to place. Valid product types are:
+
+- `ProductType.Intraday` - Intraday order that will get squared off before market close
+- `ProductType.Delivery` - Delivery order that will be held with you after market close
+- `ProductType.CoverOrder` - Cover order
+- `ProductType.BracketOrder` - One cancels other order. Also known as bracket order
+
+## Working with examples
+
+[Here](https://github.com/algo2t/alphatrade), examples directory there are 3 files `zlogin_example.py`, `zstreaming_data.py` and `stop.txt`
+
+### Steps
+
+- Clone the repository to your local machine `git clone https://github.com/algo2t/alphatrade.git`
+- Copy the examples directory to any location where you want to write your code
+- Install the `alphatrade` module using `pip` => `python -m pip install https://github.com/algo2t/alphatrade.git`
+- Open the examples directory in your favorite editor, in our case it is [VSCodium](https://vscodium.com/)
+- Open the `zlogin_example.py` file in the editor
+- Now, create `config.py` file as per instructions given below and in the above file
+- Provide correct login credentials like login_id, password and 16 digit totp code (find below qr code)
+- This is generally set from the homepage of alpha web trading platform [here](https://alpha.sasonline.in/)
+- Click on `FORGET PASSWORD?` => Select `Reset 2FA` radio button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/forget_password.png)
+- Enter the CLIENT ID (LOGIN_ID), EMAIL ID and PAN NUMBER, click on `RESET` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/reset_two_fa.png)
+- Click on `BACK TO LOGIN` and enter `CLIENT ID` and `PASSWORD`, click on `SECURED SIGN-IN`
+- Set same answers for 5 questions and click on `SUBMIT` button.  ![image](https://raw.githubusercontent.com/algo2t/alphatrade/main/snaps/set_answers.png)
+
+`config.py`
+```python
+login_id = "XXXXX"
+password = "XXXXXXXX"
+Totp = 'XXXXXXXXXXXXXXXX'
+
+try:
+    access_token = open('access_token.txt', 'r').read().rstrip()
+except Exception as e:
+    print('Exception occurred :: {}'.format(e))
+    access_token = None
+```
+
+## Example strategy using alpha trade API
+
+[Here](https://github.com/algo2t/alphatrade/blob/main/zstreaming_data.py) is an example moving average strategy using alpha trade web API.
+This strategy generates a buy signal when 5-EMA > 20-EMA (golden cross) or a sell signal when 5-EMA < 20-EMA (death cross).
+
+## Example for getting historical and intraday candles data
+
+[Here](https://github.com/algo2t/alphatrade/blob/main/zhistorical_data.py) is an example for getting historical data using alpha trade web API.
+
+For historical candles data `start_time` and `end_time` must be provided in format as shown below.
+It can also be provided as `timedelta`. Check the script `zhistorical_data.py` in examples.
+
+```python
+from datetime import datetime, timedelta
+start_time = datetime(2020, 10, 19, 9, 15, 0)
+end_time = datetime(2020, 10, 21, 16, 59, 0)
+
+df = sas.get_historical_candles('MCX', 'NATURALGAS OCT FUT', start_time, end_time, 5)
+print(df)
+end_time = start_time + timedelta(days=5)
+df = sas.get_historical_candles('MCX', 'NATURALGAS NOV FUT', start_time, end_time, 15)
+print(df)
+```
+
+For intraday or today‘s / current day‘s candles data.  
+
+```python
+df = sas.get_intraday_candles('MCX', 'NATURALGAS OCT FUT')
+print(df)
+df = sas.get_intraday_candles('MCX', 'NATURALGAS NOV FUT', 15)
+print(df)
+```
+
+
+## Read this before creating an issue
+
+Before creating an issue in this library, please follow the following steps.
+
+1. Search the problem you are facing is already asked by someone else. There might be some issues already there, either solved/unsolved related to your problem. Go to [issues](https://github.com/algo2t/alphatrade/issues) page, use `is:issue` as filter and search your problem. ![image](https://user-images.githubusercontent.com/38440742/85207058-376ee400-b2f4-11ea-91ad-c8fd8a682a12.png)
+2. If you feel your problem is not asked by anyone or no issues are related to your problem, then create a new issue.
+3. Describe your problem in detail while creating the issue. If you don‘t have time to detail/describe the problem you are facing, assume that I also won‘t be having time to respond to your problem.
+4. Post a sample code of the problem you are facing. If I copy paste the code directly from issue, I should be able to reproduce the problem you are facing.
+5. Before posting the sample code, test your sample code yourself once. Only sample code should be tested, no other addition should be there while you are testing.
+6. Have some print() function calls to display the values of some variables related to your problem.
+7. Post the results of print() functions also in the issue.
+8. Use the insert code feature of github to inset code and print outputs, so that the code is displayed neat. ![image](https://user-images.githubusercontent.com/38440742/85207234-4dc96f80-b2f5-11ea-990c-df013dd69cf2.png)
+
+
```

