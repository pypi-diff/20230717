# Comparing `tmp/fyers_apiv2-2.0.6.tar.gz` & `tmp/fyers_apiv2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fyers_apiv2-2.0.6.tar", last modified: Fri May  5 06:41:09 2023, max compression
+gzip compressed data, was "fyers_apiv2-2.0.7.tar", last modified: Mon Jul 17 12:50:38 2023, max compression
```

## Comparing `fyers_apiv2-2.0.6.tar` & `fyers_apiv2-2.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)      837 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/setup.py
--rw-rw-r--   0 ajack     (1000) ajack     (1000)       38 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/setup.cfg
-drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_api/
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)     1563 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/accessToken.py
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)    10320 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersModel.py
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)       18 2023-05-05 06:39:02.000000 fyers_apiv2-2.0.6/fyers_api/__init__.py
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)      747 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/config.py
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)     6338 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersService.py
-drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/
--rw-rw-r--   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/__init__.py
--rw-rw-r--   0 ajack     (1000) ajack     (1000)    11486 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/ws.py
--rw-rw-r--   0 ajack     (1000) ajack     (1000)      988 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/constants.py
--rw-rw-r--   0 ajack     (1000) ajack     (1000)    10517 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/tesapi.py
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)     1010 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersFormation.py
--rw-rw-r--   0 ajack     (1000) ajack     (1000)      989 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersLog.py
--rw-rw-r--   0 ajack     (1000) ajack     (1000)      797 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/PKG-INFO
-drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/
--rw-rw-r--   0 ajack     (1000) ajack     (1000)        1 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/dependency_links.txt
--rw-rw-r--   0 ajack     (1000) ajack     (1000)       10 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/top_level.txt
--rw-rw-r--   0 ajack     (1000) ajack     (1000)       85 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/requires.txt
--rw-rw-r--   0 ajack     (1000) ajack     (1000)      470 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/SOURCES.txt
--rw-rw-r--   0 ajack     (1000) ajack     (1000)      797 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/PKG-INFO
--rwxrwxr-x   0 ajack     (1000) ajack     (1000)      256 2023-05-05 06:39:02.000000 fyers_apiv2-2.0.6/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 12:50:38.695516 fyers_apiv2-2.0.7/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-17 12:09:13.000000 fyers_apiv2-2.0.7/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      647 2023-07-17 12:50:38.695516 fyers_apiv2-2.0.7/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      248 2023-07-17 12:45:28.000000 fyers_apiv2-2.0.7/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 12:50:38.671516 fyers_apiv2-2.0.7/fyers_api/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 12:50:38.675516 fyers_apiv2-2.0.7/fyers_api/Websocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-17 12:09:33.000000 fyers_apiv2-2.0.7/fyers_api/Websocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      988 2023-07-17 12:09:33.000000 fyers_apiv2-2.0.7/fyers_api/Websocket/constants.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    11486 2023-07-17 12:09:33.000000 fyers_apiv2-2.0.7/fyers_api/Websocket/ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-17 12:46:37.000000 fyers_apiv2-2.0.7/fyers_api/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1563 2023-07-17 12:09:33.000000 fyers_apiv2-2.0.7/fyers_api/accessToken.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      746 2023-07-17 12:09:56.000000 fyers_apiv2-2.0.7/fyers_api/config.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1010 2023-07-17 12:09:33.000000 fyers_apiv2-2.0.7/fyers_api/fyersFormation.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      989 2023-07-17 12:09:33.000000 fyers_apiv2-2.0.7/fyers_api/fyersLog.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10337 2023-07-17 12:11:18.000000 fyers_apiv2-2.0.7/fyers_api/fyersModel.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     6283 2023-07-17 12:40:13.000000 fyers_apiv2-2.0.7/fyers_api/fyersService.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10610 2023-07-17 12:42:18.000000 fyers_apiv2-2.0.7/fyers_api/tesapi.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 12:50:38.695516 fyers_apiv2-2.0.7/fyers_apiv2.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      647 2023-07-17 12:50:38.000000 fyers_apiv2-2.0.7/fyers_apiv2.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      482 2023-07-17 12:50:38.000000 fyers_apiv2-2.0.7/fyers_apiv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-17 12:50:38.000000 fyers_apiv2-2.0.7/fyers_apiv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       85 2023-07-17 12:50:38.000000 fyers_apiv2-2.0.7/fyers_apiv2.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-17 12:50:38.000000 fyers_apiv2-2.0.7/fyers_apiv2.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-17 12:50:38.695516 fyers_apiv2-2.0.7/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      837 2023-07-17 12:09:43.000000 fyers_apiv2-2.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fyers_apiv2-2.0.6/setup.py` & `fyers_apiv2-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_apiv2',  
-     version='2.0.6',
+     version='2.0.7',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

### Comparing `fyers_apiv2-2.0.6/fyers_api/accessToken.py` & `fyers_apiv2-2.0.7/fyers_api/accessToken.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.6/fyers_api/fyersModel.py` & `fyers_apiv2-2.0.7/fyers_api/fyersModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 		except Exception as e:
 			self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "minquantity", self.header, "response", "ERROR  : {}".format(e))
 			return
 
 	def market_status(self):
 		try:
 			timestamp = self.create_timestamp()
-			response = self.service.getCall(Config.marketStatus, self.header)
+			response = self.service.getCall(Config.marketStatus, self.header , data_flag=True)
 			self.logObj.logEntryFunc(timestamp, "market_status", "", response)
 			return response
 		except Exception as e:
 			self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "market_status", "", "response", "ERROR  : {}".format(e))
 			return
 
 	def exit_positions(self,data=None):
```

### Comparing `fyers_apiv2-2.0.6/fyers_api/config.py` & `fyers_apiv2-2.0.7/fyers_api/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     positions = '/positions'
     holdings = '/holdings'
     convertPosition = '/positions'
     funds = '/funds'
     orders = '/orders'
     minquantity = '/minquantity'
     orderStatus = '/order-status'
-    marketStatus = '/market-status'
+    marketStatus = '/marketStatus'
     auth = '/generate-authcode'
     generateAccessToken = '/validate-authcode'
     exitPositions = '/positions'
     generateDataToken = '/data-token'
 
     dataVendorTD = "truedata-ws"
```

### Comparing `fyers_apiv2-2.0.6/fyers_api/fyersService.py` & `fyers_apiv2-2.0.7/fyers_api/fyersService.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,20 @@
     def __init__(self,logObj= None):
         self.logObj = logObj
         self.content = 'application/json'
 
     def postCall(self, api, header, data=None):
         try:
             response = requests.post(Config.Api + api, headers={"Authorization": header, 'Content-Type':self.content}, json=data)
+            return response.json()
         except Exception as e:
             response = formService.exceptionRaised(e)
             if self.logObj is not None:
                 self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "getCall", "","", e)
-        if type(response)==dict:
             return response
-        return response.json()
 
     def getCall(self, api, header, data=None,data_flag=False):
         try:
             if data_flag:
                 if api == "/history":
                     url = Config.historyDataUrl + api
                 else:
@@ -43,41 +42,40 @@
             if data is not None:
                 try:
                     url_params = urllib.urlencode(data)
                 except Exception as e:
                     url_params = urllib.parse.urlencode(data)
                 url = url + "?" + url_params
             response = requests.get(url=url, headers={"Authorization": header, 'Content-Type': self.content})
+            return response.json()
         except Exception as e:
             response = formService.exceptionRaised(e)
             if self.logObj is not None:
                 self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "getCall", "", "",e)
-        return response.json()
+            return response
 
     def deleteCall(self, api, header, data):
         try:
             response = requests.delete(url=Config.Api + api,headers={"Authorization": header, 'Content-Type': self.content}, json=data)
+            return response.json()
         except Exception as e:
             response = formService.exceptionRaised(e)
             if self.logObj is not None:
                 self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "getCall", "", "",e)
-        if type(response)==dict:
             return response
-        return response.json()
 
     def putCall(self, api, header, data):
         try:
             response = requests.put(url=Config.Api + api,headers={"Authorization": header, 'Content-Type': self.content}, json=data)
+            return response.json()
         except Exception as e:
             response = formService.exceptionRaised(e)
             if self.logObj is not None:
                 self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "getCall", "", "",e)
-        if type(response)==dict:
             return response
-        return response.json()
 
 
 class FyersAsyncService:
 
     def __init__(self,logObj=None):
         self.logObj = logObj
         self.content = 'application/json'
```

### Comparing `fyers_apiv2-2.0.6/fyers_api/Websocket/ws.py` & `fyers_apiv2-2.0.7/fyers_api/Websocket/ws.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.6/fyers_api/Websocket/constants.py` & `fyers_apiv2-2.0.7/fyers_api/Websocket/constants.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.6/fyers_api/tesapi.py` & `fyers_apiv2-2.0.7/fyers_api/tesapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import sys
-sys.path.insert(0, "/home/piyush/Documents/fyers_v2/Python_SDK/fyers-api-py/")
+sys.path.insert(0, "/home/vinay/Documents/apiv2-sdk-marketStatus/fyers-api-py")
 from fyers_api import fyersModel
 import webbrowser
 from fyers_api import accessToken
 from fyers_api.Websocket import ws
 import time
 # import asyncio
 
 def api_call(token,client_id):
 	# access_token = "your_access_token_from_generate_access_token_function" ## access_token from the rgenerate_access_token function
 	## If you want to make asynchronous API calls then assign the below variable as True and then pass it in the functions, by default its value is False
 	# is_async = True
 	access_token = token
 	# appId = client_id.split(":")[0]
 	# import ipdb;ipdb.set_trace()
-	fyers = fyersModel.FyersModel(token=access_token,is_async=True,client_id=client_id)
+	fyers = fyersModel.FyersModel(token=access_token,is_async=False,client_id=client_id, log_path="/home/vinay/Documents/apiv2-sdk-marketStatus/fyers-api-py")
 	fyers.token = access_token
 	#
 	# print(fyers.get_profile())
 	# data = {"symbol":"NSE:SBIN-EQ","resolution":"D","date_format":"0","range_from":"1622097600","range_to":"1622097685","cont_flag":"1"}
 	# print(fyers.history(data))
-	# start_time = time.time()
+	# # start_time = time.time()
 	# print(fyers.quotes({"symbols":"NSE:ONGC-EQ,NSE:SBIN-EQ"}))
 	# end_time = time.time()
-	# print(f"end_time:{end_time-start_time}")
+	# # print(f"end_time:{end_time-start_time}")
 	# print(fyers.depth({"symbol":"NSE:SBIN-EQ","ohlcv_flag":"0"}))
-	# print(fyers.ws.({"data_type":"symbolUpdate","symbol":"MCX:SILVERMIC21JUNFUT"}))
+	# # print(fyers.ws.({"data_type":"symbolUpdate","symbol":"MCX:SILVERMIC21JUNFUT"}))
 	# print(fyers.tradebook())
-	# print(fyers.tradebook_with_filter({"orderNumber":"808078094451"}))  #tradebook_with_filter
+	# # print(fyers.tradebook_with_filter({"orderNumber":"808078094451"}))  #tradebook_with_filter
 	# print(fyers.positions())
 	# print(fyers.holdings())
-	# print(fyers.holdings_with_filter({"symbol":"NSE:JPASSOCIAT-"}))
+	# # print(fyers.holdings_with_filter({"symbol":"NSE:JPASSOCIAT-"}))
 	# print(fyers.convert_position({"symbol":"MCX:SILVERMIC20AUGFUT","positionSide":"1","convertQty":"1","convertFrom":"MARGIN","convertTo":"INTRADAY"}))
 	# print(fyers.funds())
-	# print(fyers.funds_with_filter({'id':"1"}))
-	# print(fyers.orderBook())
-	# print(fyers.orderBook_with_filter({'id':'808078094451'}))
-	# print(fyers.cancel_orders({'id':'8080582117761'}))
-	# print(fyers.place_orders({"symbol":"MCX:SILVERMIC20AUGFUT","qty":"1","type":"1","side":"1","productType":"INTRADAY","limitPrice":"76700","stopPrice":"0","disclosedQty":"0","validity":"DAY","offlineOrder":"False","stopLoss":"0","takeProfit":"0"}))
-	# print(fyers.modify_orders({"id":"808058117761", "qty":"0","type":"1","limitPrice":"71100","stopPrice":"0"})) #modify instead of update
-	# # print(fyers.minquantity())
+	# # print(fyers.funds_with_filter({'id':"1"}))
+	# print(fyers.orderbook())
+	# # print(fyers.orderBook_with_filter({'id':'808078094451'}))
+	# print(fyers.cancel_order({'id':'8080582117761'}))
+	# print(fyers.place_order({"symbol":"MCX:SILVERMIC20AUGFUT","qty":"1","type":"1","side":"1","productType":"INTRADAY","limitPrice":"76700","stopPrice":"0","disclosedQty":"0","validity":"DAY","offlineOrder":"False","stopLoss":"0","takeProfit":"0"}))
+	# print(fyers.modify_order({"id":"808058117761", "qty":"0","type":"1","limitPrice":"71100","stopPrice":"0"})) #modify instead of update
+	# print(fyers.minquantity())
 	# print(fyers.orderStatus_with_filter({'id':'808078094451'}))
-	# # print(fyers.market_status())
+	# print(fyers.market_status())
 	# print(fyers.exit_positions({"id":"MCX:SILVERMIC20AUGFUT-MARGIN"}))
-	# # print(fyers.generate_data_token({"vendorApp":"0KMS0EZVXI"}))
-	# # print(fyers.multiple_orders())
+	# print(fyers.generate_data_token({"vendorApp":"0KMS0EZVXI"}))
+	# print(fyers.multiple_orders())
 	# print(fyers.multiple_cancel_orders([{"id":"120080780536"},{"id":"120080777069"}]))
 	# print(fyers.multiple_place_orders([{"symbol":"NSE:SBIN-EQ","qty":"1","type":"1","side":"1","productType":"INTRADAY","limitPrice":"191","stopPrice":"0","disclosedQty":"0","validity":"DAY","offlineOrder":"False","stopLoss":"0","takeProfit":"0"},{"symbol":"NSE:SBIN-EQ","qty":"1","type":"1","side":"1","productType":"INTRADAY","limitPrice":"191","stopPrice":"0","disclosedQty":"0","validity":"DAY","offlineOrder":"False","stopLoss":"0","takeProfit":"0"}]))
-	#
+	
 	# print(fyers.multiple_modify_orders([{"id":"120080780536", "type":1, "limitPrice": 190, "stopPrice":0},{"id":"120080777069", "type":1, "limitPrice": 190}]))
 	
 	# p = threading.Thread(target=fyersSocket.subscribe)
 	# p.start()
 	# data = {"symbol":"NSE:SBIN-EQ","resolution":"D","date_format":"0","range_from":"1622097600","range_to":"1622097685","cont_flag":"1"}
 	# fyers.history(data)
 	# print(response)
@@ -65,16 +65,16 @@
 	# data_type = "orderUpdate"
 	# symbol =  ["MCX:SILVERMIC21NOVFUT","MCX:NATURALGAS21SEPFUT"]
 	symbol =["NSE:NIFTY50-INDEX","NSE:NIFTYBANK-INDEX","NSE:NIFTYAUTO-INDEX","NSE:NIFTYALPHA50-INDEX","BSE:150MIDCAP-INDEX"]
 	# symbol =["NSE:NIFTY50-INDEX"]
 	# symbol=["NSE:NIFTY2190917350CE","NSE:NIFTY2190917350PE"]
 	# symbol = ["NSE:SBIN-EQ","NSE:ONGC-EQ"]
 		# fs = ws.FyersSocket(access_token=access_token, data_type=data_type,run_background=True)
-	fs = ws.FyersSocket(access_token=access_token,run_background=False,log_path="/home/piyush/Downloads/")
-	fs.websocket_data = custom_message
+	# fs = ws.FyersSocket(access_token=access_token,run_background=False,log_path="/home/piyush/Downloads/")
+	# fs.websocket_data = custom_message
 	# fs.on_open = onopen
 	# fs.on_error = onerror
 	# fs.init_connection()
 	# time.sleep(5)
 	# import ipdb;ipdb.set_trace()
 	# fs.subscribe(symbol=symbol)
 	# def op_open(fs,fetch_symbol):
@@ -85,24 +85,24 @@
 	# 	message
 	# fs.on_open()
 	# fs.on_close()
 	# fs.on_message()
 	# fs.on_error()
 	# fs.init_connection()
 	# import ipdb;ipdb.set_trace()
-	fs.subscribe(symbol=symbol,data_type=data_type)
+	# fs.subscribe(symbol=symbol,data_type=data_type)
 	# # time.sleep(5)
 	# # fs.subscribe(symbol=["MCX:SILVER21SEPFUT"])
 	# print(fyers.get_profile())
 	# print(fyers.tradebook())
 	# print(fyers.positions())
 	# # print("unsubscribed symbol")
 	# # symbol = ["NSE:ONGC-EQ"]
 	# # fs.unsubscribe(symbol=symbol)
-	fs.keep_running()
+	# fs.keep_running()
 	# fs.subscribe(run_background=False)
 	# with ThreadPoolExecutor(3) as executor:
 	# 	task = executor.submit(fs.subscribe())
 
 def getauthToken(client_id,redirect_uri,response_type,scope,state,nonce):
 	"""
 		The variable `generateTokenUrl` will have a url like
@@ -145,27 +145,27 @@
 
 def onerror(msg):
 	print(msg)	
 
 def main():
 
 	redirect_uri= "https://beta-rest.tradingview.com/trading/oauth-redirect/fyers/"
-	client_id = "L9NY34Z6BW-100"
+	client_id = "XC4EOD67IM-100"
 	# client_id = "TWQFQCS0Q4-101"
 	secret_key = "WGKBQ43W2G"
 	grant_type = "authorization_code"
 	response_type = "code"
 	state = "sample"
 	nonce = "baka"
 	scope = "openid"
 	# getauthToken(client_id, redirect_uri,response_type,scope,state,nonce)
 	auth_code = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkubG9naW4uZnllcnMuaW4iLCJpYXQiOjE2MjM3NDEwMzAsImV4cCI6MTYyMzc0MTMzMCwibmJmIjoxNjIzNzQxMDMwLCJhdWQiOiJbXCJ4OjJcIiwgXCJ4OjFcIiwgXCJ4OjBcIiwgXCJkOjFcIiwgXCJkOjJcIl0iLCJzdWIiOiJhdXRoX2NvZGUiLCJkaXNwbGF5X25hbWUiOiJEUDAwNDA0Iiwibm9uY2UiOiJiYWthIiwiYXBwX2lkIjoiR01FN0lBTFNZSiIsInV1aWQiOiJmMTJlMTEyZmQ5ODA0MWE2OWI0OGRiMDI5ZTIzOTdmNyIsImlwQWRkciI6IjY1LjEuMjU0LjI1MSIsInNjb3BlIjoib3BlbmlkIn0.0p_4K_D4CnNO3WCK49ZWq11Ho3mR1vYnPaX9u--AbAE"
 
 	# print(generate_access_token(auth_code, client_id, redirect_uri,secret_key,grant_type))
 
-	access_token ="eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2MzM1ODE3MzEsImV4cCI6MTYzMzY1MzAxMSwibmJmIjoxNjMzNTgxNzMxLCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCaFhucWpFNjhncHMtNjRzZGxjc0lMNFl0UmktQWRNeGdhcjByREs2RVlTbXVxQ0puVm0zWjN4Vk1hLXBsbV9GQzl1c0lwT3liUHVySGI4eURTUGZwTWdRNkVXNzZmNzFxS1JmWTcyUkZrWXZLX3AzZz0iLCJkaXNwbGF5X25hbWUiOiJQSVlVU0ggUkFKRU5EUkEgS0FQU0UiLCJmeV9pZCI6IkRQMDA0MDQiLCJhcHBUeXBlIjoxMDAsInBvYV9mbGFnIjoiTiJ9.U3qRPL3kJrE9gZq6DvPX14pHK3yikd826q25hhwOWpg"
+	access_token ="eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODk1NjU0NjUsImV4cCI6MTY4OTY0MDIyNSwibmJmIjoxNjg5NTY1NDY1LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa3RMa1pRdkdGOVE4Y3ZFQzdTNm8tdjdhSUZpWG1MSjlDSFpVRkYwRU04NDBuV1VrSVNOQTZvUW1yVDlieUJEU2dUWEJXMHhjOERKRFRsYkNQa3dNZW1EXzdsbDBzR1hXTkc3Yml6bTNUUUVxMkRLRT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.WPwPeJvZALvtxoiQUGLZJj9zehxuU8KyNlqb-NfLBa0"
 
 	api_call(access_token , client_id)
 
 if __name__ == '__main__':
 	main()
```

### Comparing `fyers_apiv2-2.0.6/fyers_api/fyersFormation.py` & `fyers_apiv2-2.0.7/fyers_api/fyersFormation.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.6/fyers_api/fyersLog.py` & `fyers_apiv2-2.0.7/fyers_api/fyersLog.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.6/PKG-INFO` & `fyers_apiv2-2.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fyers_apiv2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
-License: UNKNOWN
-Description: README
-        ========
-        
-        This module is installed via pip:
-        
-        ```
-        pip install fyers-api
-        ```
-        
-        Packages Required
-         - json
-         - requests
-         - tornado 
-        
-        For an overview of Fyers-api please refer to the documentation at [fyers-api-docs](http://apidashboard.fyers.in/api-docs)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+README
+========
+
+This module is installed via pip:
+
+```
+pip install fyers-apiv2
+```
+
+Packages Required
+ - json
+ - requests
+ - tornado 
+
+For an overview of Fyers-api please refer to the documentation at [fyers-api-docs](https://myapi.fyers.in/docs)
```

### Comparing `fyers_apiv2-2.0.6/fyers_apiv2.egg-info/PKG-INFO` & `fyers_apiv2-2.0.7/fyers_apiv2.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fyers-apiv2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
-License: UNKNOWN
-Description: README
-        ========
-        
-        This module is installed via pip:
-        
-        ```
-        pip install fyers-api
-        ```
-        
-        Packages Required
-         - json
-         - requests
-         - tornado 
-        
-        For an overview of Fyers-api please refer to the documentation at [fyers-api-docs](http://apidashboard.fyers.in/api-docs)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+README
+========
+
+This module is installed via pip:
+
+```
+pip install fyers-apiv2
+```
+
+Packages Required
+ - json
+ - requests
+ - tornado 
+
+For an overview of Fyers-api please refer to the documentation at [fyers-api-docs](https://myapi.fyers.in/docs)
```

