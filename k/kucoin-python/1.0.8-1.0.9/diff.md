# Comparing `tmp/kucoin-python-1.0.8.tar.gz` & `tmp/kucoin-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aaron/Workspace/public/kucoin-python-sdk/dist/tmp06za8o6m/kucoin-python-1.0.8.tar", last modified: Mon Jul 26 10:08:35 2021, max compression
+gzip compressed data, was "/Users/aaron/Workspace/public/kucoin-python-sdk/dist/tmpwqn_l_z4/kucoin-python-1.0.9.tar", last modified: Wed Aug 18 08:54:52 2021, max compression
```

## Comparing `kucoin-python-1.0.8.tar` & `kucoin-python-1.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.116585 kucoin-python-1.0.8/
--rw-r--r--   0 aaron      (501) staff       (20)     1063 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/LICENSE
--rw-r--r--   0 aaron      (501) staff       (20)      398 2021-07-26 10:08:35.115001 kucoin-python-1.0.8/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)     3307 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/README.rst
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.082419 kucoin-python-1.0.8/kucoin/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/__init__.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.085402 kucoin-python-1.0.8/kucoin/base_request/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/base_request/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)     4095 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/base_request/base_request.py
--rw-r--r--   0 aaron      (501) staff       (20)      390 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/client.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.089087 kucoin-python-1.0.8/kucoin/margin/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/margin/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    13183 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/margin/margin.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.092586 kucoin-python-1.0.8/kucoin/market/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/market/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    14559 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/market/market.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.095676 kucoin-python-1.0.8/kucoin/trade/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/trade/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    23936 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/trade/trade.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.098462 kucoin-python-1.0.8/kucoin/user/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/user/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    23860 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/user/user.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.101079 kucoin-python-1.0.8/kucoin/websocket/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/websocket/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)     4143 2021-07-26 08:24:42.000000 kucoin-python-1.0.8/kucoin/websocket/websocket.py
--rw-r--r--   0 aaron      (501) staff       (20)     1412 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/ws_client.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.103580 kucoin-python-1.0.8/kucoin/ws_token/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/ws_token/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)      451 2021-07-26 08:21:08.000000 kucoin-python-1.0.8/kucoin/ws_token/token.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-07-26 10:08:35.112975 kucoin-python-1.0.8/kucoin_python.egg-info/
--rw-r--r--   0 aaron      (501) staff       (20)      398 2021-07-26 10:08:35.000000 kucoin-python-1.0.8/kucoin_python.egg-info/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)      638 2021-07-26 10:08:35.000000 kucoin-python-1.0.8/kucoin_python.egg-info/SOURCES.txt
--rw-r--r--   0 aaron      (501) staff       (20)        1 2021-07-26 10:08:35.000000 kucoin-python-1.0.8/kucoin_python.egg-info/dependency_links.txt
--rw-r--r--   0 aaron      (501) staff       (20)       20 2021-07-26 10:08:35.000000 kucoin-python-1.0.8/kucoin_python.egg-info/requires.txt
--rw-r--r--   0 aaron      (501) staff       (20)      113 2021-07-26 10:08:35.000000 kucoin-python-1.0.8/kucoin_python.egg-info/top_level.txt
--rw-r--r--   0 aaron      (501) staff       (20)       38 2021-07-26 10:08:35.116786 kucoin-python-1.0.8/setup.cfg
--rw-r--r--   0 aaron      (501) staff       (20)      686 2021-07-26 08:48:39.000000 kucoin-python-1.0.8/setup.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.921877 kucoin-python-1.0.9/
+-rw-r--r--   0 aaron      (501) staff       (20)     1063 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/LICENSE
+-rw-r--r--   0 aaron      (501) staff       (20)      398 2021-08-18 08:54:52.920374 kucoin-python-1.0.9/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)     3307 2021-08-18 08:48:49.000000 kucoin-python-1.0.9/README.rst
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.869114 kucoin-python-1.0.9/kucoin/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/__init__.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.874467 kucoin-python-1.0.9/kucoin/base_request/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/base_request/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4095 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/base_request/base_request.py
+-rw-r--r--   0 aaron      (501) staff       (20)      390 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/client.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.881577 kucoin-python-1.0.9/kucoin/margin/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/margin/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    13183 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/margin/margin.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.885431 kucoin-python-1.0.9/kucoin/market/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/market/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    14559 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/market/market.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.894514 kucoin-python-1.0.9/kucoin/trade/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/trade/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    24825 2021-08-18 08:28:58.000000 kucoin-python-1.0.9/kucoin/trade/trade.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.897935 kucoin-python-1.0.9/kucoin/user/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/user/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    23860 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/user/user.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.903961 kucoin-python-1.0.9/kucoin/websocket/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/websocket/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4143 2021-07-26 08:24:42.000000 kucoin-python-1.0.9/kucoin/websocket/websocket.py
+-rw-r--r--   0 aaron      (501) staff       (20)     1412 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/ws_client.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.908636 kucoin-python-1.0.9/kucoin/ws_token/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/ws_token/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)      451 2021-07-26 08:21:08.000000 kucoin-python-1.0.9/kucoin/ws_token/token.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-08-18 08:54:52.918521 kucoin-python-1.0.9/kucoin_python.egg-info/
+-rw-r--r--   0 aaron      (501) staff       (20)      398 2021-08-18 08:54:52.000000 kucoin-python-1.0.9/kucoin_python.egg-info/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)      638 2021-08-18 08:54:52.000000 kucoin-python-1.0.9/kucoin_python.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron      (501) staff       (20)        1 2021-08-18 08:54:52.000000 kucoin-python-1.0.9/kucoin_python.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       20 2021-08-18 08:54:52.000000 kucoin-python-1.0.9/kucoin_python.egg-info/requires.txt
+-rw-r--r--   0 aaron      (501) staff       (20)      113 2021-08-18 08:54:52.000000 kucoin-python-1.0.9/kucoin_python.egg-info/top_level.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       38 2021-08-18 08:54:52.922135 kucoin-python-1.0.9/setup.cfg
+-rw-r--r--   0 aaron      (501) staff       (20)      686 2021-08-18 08:48:22.000000 kucoin-python-1.0.9/setup.py
```

### Comparing `kucoin-python-1.0.8/LICENSE` & `kucoin-python-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/README.rst` & `kucoin-python-1.0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - Implementation of REST endpoints
 - Simple handling of authentication
 - Response exception handling
 - Implement websockets (note only python3.6+)
 
 update
 ----------
-- 2020 12/01
+- 2021 08/18
 
 Quick Start
 -----------
 
 Register an account with `KuCoin <https://www.kucoin.com/ucenter/signup>`_.
 
 To test on the Sandbox  with `KuCoin Sandbox <https://sandbox.kucoin.com/>`_.
```

### Comparing `kucoin-python-1.0.8/kucoin/base_request/base_request.py` & `kucoin-python-1.0.9/kucoin/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/kucoin/margin/margin.py` & `kucoin-python-1.0.9/kucoin/margin/margin.py`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/kucoin/market/market.py` & `kucoin-python-1.0.9/kucoin/market/market.py`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/kucoin/trade/trade.py` & `kucoin-python-1.0.9/kucoin/trade/trade.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,74 +159,77 @@
             clientOid = self.return_unique_id
         params['clientOid'] = clientOid
         if kwargs:
             params.update(kwargs)
 
         return self._request('POST', '/api/v1/orders', params=params)
 
-    def create_bulk_orders(self, side, symbol, price, size, clientOid='', **kwargs):
+    def create_bulk_orders(self, symbol, orderList):
         """
         https://docs.kucoin.com/#place-bulk-orders
-        :param side: place direction buy or sell (Mandatory)
+        :param symbol: a valid trading symbol code.
         :type: str
-        :param symbol: a valid trading symbol code (Mandatory)
-        :type: str
-        :param price: price per base currency (Mandatory)
-        :type: str
-        :param size: amount of base currency to buy or sell (Mandatory)
-        :type: str
-        :param clientOid: Unique order id created by users to identify their orders, e.g. UUID. (Mandatory)
-        :type: str
-        :param kwargs: Fill in parameters with reference documents
+        :param orderList: order list
+        :type: list
         :return:
         {
-            "success": true, // RESPONSE
-            "code": "200",
-            "msg": "success",
-            "retry": false,
-            "data": {
-              "data": [
-                  {
-                    "symbol": "BTC-USDT",
-                    "type": "limit",
-                    "side": "buy",
-                    "price": "9661",
-                    "size": "1",
-                    "funds": null,
-                    "stp": "",
-                    "stop": "",
-                    "stopPrice": "0",
-                    "timeInForce": "GTC",
-                    "cancelAfter": 0,
-                    "postOnly": false,
-                    "hidden": false,
-                    "iceberge": false,
-                    "iceberg": false,
-                    "visibleSize": "0",
-                    "channel": "API",
-                    "id": null,
-                    "status": "fail",
-                    "failMsg": "error.createOrder.accountBalanceInsufficient",
-                    "clientOid": "5e42743514832d53d255d921"
-                  }
-              ]
+          "data": [
+            {
+              "symbol": "KCS-USDT",
+              "type": "limit",
+              "side": "buy",
+              "price": "0.01",
+              "size": "0.01",
+              "funds": null,
+              "stp": "",
+              "stop": "",
+              "stopPrice": null,
+              "timeInForce": "GTC",
+              "cancelAfter": 0,
+              "postOnly": false,
+              "hidden": false,
+              "iceberge": false,
+              "iceberg": false,
+              "visibleSize": null,
+              "channel": "API",
+              "id": "611a6a309281bc000674d3c0",
+              "status": "success",
+              "failMsg": null,
+              "clientOid": "552a8a0b7cb04354be8266f0e202e7e9"
+            },
+            {
+              "symbol": "KCS-USDT",
+              "type": "limit",
+              "side": "buy",
+              "price": "0.01",
+              "size": "0.01",
+              "funds": null,
+              "stp": "",
+              "stop": "",
+              "stopPrice": null,
+              "timeInForce": "GTC",
+              "cancelAfter": 0,
+              "postOnly": false,
+              "hidden": false,
+              "iceberge": false,
+              "iceberg": false,
+              "visibleSize": null,
+              "channel": "API",
+              "id": "611a6a309281bc000674d3c1",
+              "status": "success",
+              "failMsg": null,
+              "clientOid": "bd1e95e705724f33b508ed270888a4a9"
             }
+          ]
         }
         """
         params = {
-            'side': side,
             'symbol': symbol,
-            'price': price,
-            'size': size
+            'orderList': orderList,
         }
-        if not clientOid:
-            clientOid = self.return_unique_id
-        params['clientOid'] = clientOid
-        if kwargs:
-            params.update(kwargs)
         return self._request('POST', '/api/v1/orders/multi', params=params)
 
     def cancel_client_order(self, clientId):
         """
         :param orderId: str  (Mandatory)
         :return:{"cancelledOrderId": "5f311183c9b6d539dc614db3","clientOid": "6d539dc614db3"}
         """
@@ -687,9 +690,45 @@
                 "type":"limit"
             }
         ]
         """
         return self._request('GET', '/api/v1/limit/fills')
 
     def get_client_order_details(self, clientOid):
-
-        return self._request('GET', f'/api/v1/orders/{clientOid}')
+        """
+        https://docs.kucoin.com/#recent-fills
+        :param clientOid: Unique order id created by users to identify their orders
+        :return:
+        {
+          "id": "61149d589281bc00064a9ee0",
+          "symbol": "KCS-USDT",
+          "opType": "DEAL",
+          "type": "limit",
+          "side": "buy",
+          "price": "0.001",
+          "size": "0.01",
+          "funds": "0",
+          "dealFunds": "0",
+          "dealSize": "0",
+          "fee": "0",
+          "feeCurrency": "USDT",
+          "stp": "",
+          "stop": "",
+          "stopTriggered": false,
+          "stopPrice": "0",
+          "timeInForce": "GTC",
+          "postOnly": false,
+          "hidden": false,
+          "iceberg": false,
+          "visibleSize": "0",
+          "cancelAfter": 0,
+          "channel": "API",
+          "clientOid": "03cd879961b64429b0e0149f311ce59f",
+          "remark": null,
+          "tags": null,
+          "isActive": false,
+          "cancelExist": true,
+          "createdAt": 1628740952556,
+          "tradeType": "MARGIN_TRADE"
+        }
+        """
+        return self._request('GET', f'/api/v1/order/client-order/{clientOid}')
```

### Comparing `kucoin-python-1.0.8/kucoin/user/user.py` & `kucoin-python-1.0.9/kucoin/user/user.py`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/kucoin/websocket/websocket.py` & `kucoin-python-1.0.9/kucoin/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/kucoin/ws_client.py` & `kucoin-python-1.0.9/kucoin/ws_client.py`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/kucoin_python.egg-info/SOURCES.txt` & `kucoin-python-1.0.9/kucoin_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kucoin-python-1.0.8/setup.py` & `kucoin-python-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 from setuptools import setup
 
 
 setup(
     name='kucoin-python',
-    version='v1.0.8',
+    version='v1.0.9',
     packages=['kucoin', 'kucoin/base_request', 'kucoin/margin', 'kucoin/market', 'kucoin/trade', 'kucoin/user',
               'kucoin/websocket', 'kucoin/ws_token'],
     license="MIT",
     author='Arthur',
     author_email="arthur.zhang@kucoin.com",
     url='https://github.com/Kucoin/kucoin-python-sdk',
     description="kucoin-api-sdk",
```

