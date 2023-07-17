# Comparing `tmp/hubble_exchange-0.2.0.tar.gz` & `tmp/hubble_exchange-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.2.0.tar", last modified: Fri Jul 14 06:48:56 2023, max compression
+gzip compressed data, was "hubble_exchange-0.3.0.tar", last modified: Mon Jul 17 11:43:19 2023, max compression
```

## Comparing `hubble_exchange-0.2.0.tar` & `hubble_exchange-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.445812 hubble_exchange-0.2.0/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.2.0/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.2.0/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)     5428 2023-07-14 06:48:56.445633 hubble_exchange-0.2.0/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     3771 2023-07-14 06:35:59.000000 hubble_exchange-0.2.0/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.442436 hubble_exchange-0.2.0/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      351 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     5271 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/client.py
--rw-r--r--   0 shubham    (501) staff       (20)      202 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/constants.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.444964 hubble_exchange-0.2.0/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.2.0/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/eip712.py
--rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/errors.py
--rw-r--r--   0 shubham    (501) staff       (20)     5038 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/eth.py
--rw-r--r--   0 shubham    (501) staff       (20)     2389 2023-07-14 06:14:28.000000 hubble_exchange-0.2.0/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)     4407 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)      466 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.443193 hubble_exchange-0.2.0/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     5428 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      531 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)      112 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)     1035 2023-07-14 06:46:26.000000 hubble_exchange-0.2.0/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-07-14 06:48:56.445858 hubble_exchange-0.2.0/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.2.0/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.120891 hubble_exchange-0.3.0/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.3.0/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.3.0/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)     5648 2023-07-17 11:43:19.120759 hubble_exchange-0.3.0/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     3991 2023-07-17 10:52:10.000000 hubble_exchange-0.3.0/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.119423 hubble_exchange-0.3.0/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      351 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     6220 2023-07-17 10:10:11.000000 hubble_exchange-0.3.0/hubble_exchange/client.py
+-rw-r--r--   0 shubham    (501) staff       (20)      202 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.120292 hubble_exchange-0.3.0/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.3.0/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/errors.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5038 2023-07-17 09:02:27.000000 hubble_exchange-0.3.0/hubble_exchange/eth.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3152 2023-07-17 11:37:43.000000 hubble_exchange-0.3.0/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)     4407 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)      466 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.120101 hubble_exchange-0.3.0/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     5648 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      531 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       88 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-07-17 11:42:21.000000 hubble_exchange-0.3.0/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-07-17 11:43:19.120925 hubble_exchange-0.3.0/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.3.0/setup.py
```

### Comparing `hubble_exchange-0.2.0/LICENSE` & `hubble_exchange-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.2.0/PKG-INFO` & `hubble_exchange-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,62 +42,63 @@
 The simplest way is to install the package from PyPI:
 ```shell
 pip install hubble-exchange
 ```
 
 ## Example usage:
 
-Requires HUBBLE_RPC_HOST and HUBBLE_BLOCKCHAIN_ID environment variable to be set
+All read/write functions are async
+<br>Requires HUBBLE_RPC_HOST and HUBBLE_BLOCKCHAIN_ID environment variable to be set
 ```shell
 export HUBBLE_RPC_HOST=candy-hubblenet-rpc.hubble.exchange
 export HUBBLE_BLOCKCHAIN_ID=iKMFgo49o4X3Pd3UWUkmPwjKom3xZz3Vo6Y1kkwL2Ce6DZaPm
 ```
 
 ```python
 import os
 from hubble_exchange import HubbleClient, OrderBookDepthResponse
 
 
-def main():
+async def main():
+
+    async def callback(response):
+        print(f"Received response: {response}")
+        return response
+
     client = HubbleClient(os.getenv("PRIVATE_KEY"))
     # place an order for market = 0, amount = 0.2, price = 1800, reduce_only = False
-    order = client.place_single_order(0, 0.2, 1800, False)
+    order = await client.place_single_order(0, 0.2, 1800, False, callback)
 
     # place multiple orders at once
     orders = []
     orders.append(Order.new(3, 1, 1.2, False)) # market = 3, qty = 1, price = 1.2, reduce_only = False
     orders.append(Order.new(0, 0.1, 1800, False)) # market = 0, qty = 0.1, price = 1800, reduce_only = False
     # placed_orders list will contain the order ids for the orders placed
-    placed_orders = client.place_orders(orders)
+    placed_orders = await client.place_orders(orders, callback)
 
     # get order status
-    order_status = client.get_order_status(order.Id)
+    order_status = await client.get_order_status(order.Id, callback)
     
     # cancel an order
-    client.cancel_orders([order])
+    await client.cancel_orders([order], callback)
 
     # order can also be cancelled by order id
-    client.cancel_order_by_id(order.id)
+    await client.cancel_order_by_id(order.id, callback)
 
     # get current order book for market = 1
-    order_book = client.get_order_book(1)
+    order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
-    positions = client.get_margin_and_positions()
+    positions = await client.get_margin_and_positions(callback)
 
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
-    # this is a blocking operation, so it needs to run in a separate thread
-    def callback(ws, message: OrderBookDepthResponse):
+    async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
-    client.subscribe_to_order_book_depth(0, callback=callback)
-
-
-if __name__ == "__main__":
-    main()
+    asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
 
 ## Custom transaction options
 
 The following options can be passed to the client to override the default
 
 ```python
@@ -112,15 +113,15 @@
 It can be used for `place_orders`, `place_single_order`, `cancel_orders`, `cancel_order_by_id` methods.
 Example:
 ```python
 
 from web3 import Web3
 
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
-placed_orders = client.place_orders(orders, {
+placed_orders = await client.place_orders(orders, callback, {
     "gas": 500_000,
     "maxFeePerGas": Web3.to_wei(80, 'gwei'),
     "maxPriorityFeePerGas": Web3.to_wei(20, 'gwei'),
 })
 ```
 
 ## Transaction modes
@@ -132,13 +133,13 @@
 - TransactionMode.wait_for_head: Wait for the transaction to be included in the canonical chain. At this time the block is preferred but not yet finalized. However, once the block in included in the canonical chain, the matching engine will start processing the order.
 - TransactionMode.wait_for_accept: Wait for the transaction to be finalised.
 
 Example:
 ```python
 from hubble_exchange import TransactionMode
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
-placed_orders = client.place_orders(orders, mode=TransactionMode.wait_for_accept)
+placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
-# or
+# or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
```

### Comparing `hubble_exchange-0.2.0/README.md` & `hubble_exchange-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,62 +9,63 @@
 The simplest way is to install the package from PyPI:
 ```shell
 pip install hubble-exchange
 ```
 
 ## Example usage:
 
-Requires HUBBLE_RPC_HOST and HUBBLE_BLOCKCHAIN_ID environment variable to be set
+All read/write functions are async
+<br>Requires HUBBLE_RPC_HOST and HUBBLE_BLOCKCHAIN_ID environment variable to be set
 ```shell
 export HUBBLE_RPC_HOST=candy-hubblenet-rpc.hubble.exchange
 export HUBBLE_BLOCKCHAIN_ID=iKMFgo49o4X3Pd3UWUkmPwjKom3xZz3Vo6Y1kkwL2Ce6DZaPm
 ```
 
 ```python
 import os
 from hubble_exchange import HubbleClient, OrderBookDepthResponse
 
 
-def main():
+async def main():
+
+    async def callback(response):
+        print(f"Received response: {response}")
+        return response
+
     client = HubbleClient(os.getenv("PRIVATE_KEY"))
     # place an order for market = 0, amount = 0.2, price = 1800, reduce_only = False
-    order = client.place_single_order(0, 0.2, 1800, False)
+    order = await client.place_single_order(0, 0.2, 1800, False, callback)
 
     # place multiple orders at once
     orders = []
     orders.append(Order.new(3, 1, 1.2, False)) # market = 3, qty = 1, price = 1.2, reduce_only = False
     orders.append(Order.new(0, 0.1, 1800, False)) # market = 0, qty = 0.1, price = 1800, reduce_only = False
     # placed_orders list will contain the order ids for the orders placed
-    placed_orders = client.place_orders(orders)
+    placed_orders = await client.place_orders(orders, callback)
 
     # get order status
-    order_status = client.get_order_status(order.Id)
+    order_status = await client.get_order_status(order.Id, callback)
     
     # cancel an order
-    client.cancel_orders([order])
+    await client.cancel_orders([order], callback)
 
     # order can also be cancelled by order id
-    client.cancel_order_by_id(order.id)
+    await client.cancel_order_by_id(order.id, callback)
 
     # get current order book for market = 1
-    order_book = client.get_order_book(1)
+    order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
-    positions = client.get_margin_and_positions()
+    positions = await client.get_margin_and_positions(callback)
 
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
-    # this is a blocking operation, so it needs to run in a separate thread
-    def callback(ws, message: OrderBookDepthResponse):
+    async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
-    client.subscribe_to_order_book_depth(0, callback=callback)
-
-
-if __name__ == "__main__":
-    main()
+    asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
 
 ## Custom transaction options
 
 The following options can be passed to the client to override the default
 
 ```python
@@ -79,15 +80,15 @@
 It can be used for `place_orders`, `place_single_order`, `cancel_orders`, `cancel_order_by_id` methods.
 Example:
 ```python
 
 from web3 import Web3
 
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
-placed_orders = client.place_orders(orders, {
+placed_orders = await client.place_orders(orders, callback, {
     "gas": 500_000,
     "maxFeePerGas": Web3.to_wei(80, 'gwei'),
     "maxPriorityFeePerGas": Web3.to_wei(20, 'gwei'),
 })
 ```
 
 ## Transaction modes
@@ -99,13 +100,13 @@
 - TransactionMode.wait_for_head: Wait for the transaction to be included in the canonical chain. At this time the block is preferred but not yet finalized. However, once the block in included in the canonical chain, the matching engine will start processing the order.
 - TransactionMode.wait_for_accept: Wait for the transaction to be finalised.
 
 Example:
 ```python
 from hubble_exchange import TransactionMode
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
-placed_orders = client.place_orders(orders, mode=TransactionMode.wait_for_accept)
+placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
-# or
+# or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
```

### Comparing `hubble_exchange-0.2.0/hubble_exchange/client.py` & `hubble_exchange-0.3.0/hubble_exchange/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import json
-from typing import Any, Callable, List
+from typing import List
 
-import websocket
+import websockets
 from hexbytes import HexBytes
 
-from hubble_exchange.eth import (get_web3_client,
-                                 get_websocket_endpoint)
-from hubble_exchange.models import (GetPositionsResponse, Order,
-                                    OrderBookDepthResponse,
-                                    OrderBookDepthUpdateResponse,
+from hubble_exchange.eth import get_web3_client, get_websocket_endpoint
+from hubble_exchange.models import (AsyncOrderBookDepthCallback,
+                                    AsyncOrderStatusCallback,
+                                    AsyncPlaceOrdersCallback,
+                                    AsyncPositionCallback,
+                                    AsyncSubscribeToOrderBookDepthCallback,
+                                    Order, OrderBookDepthUpdateResponse,
                                     OrderStatusResponse, WebsocketResponse)
-from hubble_exchange.order_book import OrderBookClient
+from hubble_exchange.order_book import OrderBookClient, TransactionMode
 from hubble_exchange.utils import (float_to_scaled_int,
                                    get_address_from_private_key, get_new_salt)
 
 
 class HubbleClient:
     def __init__(self, private_key: str):
         if not private_key:
@@ -23,24 +25,30 @@
         if not self.trader_address:
             raise ValueError("Cannot determine trader address from private key")
 
         self.web3_client = get_web3_client()
         self.websocket_endpoint = get_websocket_endpoint()
         self.order_book_client = OrderBookClient(private_key)
 
-    def get_order_book(self, market: int) -> OrderBookDepthResponse:
-        return self.web3_client.eth.get_order_book_depth(market)
+    def set_transaction_mode(self, mode: TransactionMode):
+        self.order_book_client.set_transaction_mode(mode)
 
-    def get_margin_and_positions(self) -> GetPositionsResponse:
-        return self.web3_client.eth.get_margin_and_positions(self.trader_address)
+    async def get_order_book(self, market: int, callback: AsyncOrderBookDepthCallback):
+        order_book_depth = self.web3_client.eth.get_order_book_depth(market)
+        return await callback(order_book_depth)
+
+    async def get_margin_and_positions(self, callback: AsyncPositionCallback):
+        response = self.web3_client.eth.get_margin_and_positions(self.trader_address)
+        return await callback(response)
+
+    async def get_order_status(self, order_id: HexBytes, callback: AsyncOrderStatusCallback):
+        response = self.web3_client.eth.get_order_status(order_id.hex()) # type: ignore
+        return await callback(response)
 
-    def get_order_status(self, order_id: HexBytes) -> OrderStatusResponse:
-        return self.web3_client.eth.get_order_status(order_id.hex())
-
-    def place_orders(self, orders: List[Order], tx_options = None, mode=None) -> List[Order]:
+    async def place_orders(self, orders: List[Order], callback: AsyncPlaceOrdersCallback, tx_options = None, mode=None):
         if len(orders) > 75:
             raise ValueError("Cannot place more than 75 orders at once")
 
         for order in orders:
             if order.amm_index is None:
                 raise ValueError("Order AMM index is not set")
             if order.base_asset_quantity is None:
@@ -52,72 +60,75 @@
 
             # trader and salt can be set automatically
             if order.trader in [None, "0x", ""]:
                 order.trader = self.trader_address
             if order.salt in [None, 0]:
                 order.salt = get_new_salt()
 
-        return self.order_book_client.place_orders(orders, tx_options, mode)
+        response = self.order_book_client.place_orders(orders, tx_options, mode)
+        return await callback(response)
 
-    def place_single_order(
-        self, market: int, base_asset_quantity: float, price: float, reduce_only: bool, tx_options = None, mode=None
+    async def place_single_order(
+        self, market: int, base_asset_quantity: float, price: float, reduce_only: bool, callback, tx_options = None, mode=None
     ) -> Order:
         order = Order(
             id=None,
             amm_index=market,
             trader=self.trader_address,
             base_asset_quantity=float_to_scaled_int(base_asset_quantity, 18),
             price=float_to_scaled_int(price, 6),
             salt=get_new_salt(),
             reduce_only=reduce_only,
         )
         order_hash = self.order_book_client.place_order(order, tx_options, mode)
         order.id = order_hash
-        return order
+        return await callback(order)
 
-    def cancel_orders(self, orders: List[Order], tx_options = None, mode=None) -> None:
+    async def cancel_orders(self, orders: List[Order], callback, tx_options = None, mode=None):
         if len(orders) > 100:
             raise ValueError("Cannot cancel more than 100 orders at once")
 
         self.order_book_client.cancel_orders(orders, tx_options, mode)
+        return await callback()
 
-    def cancel_order_by_id(self, order_id: HexBytes, tx_options = None, mode=None) -> None:
-        order_status = self.get_order_status(order_id)
-        position_side_multiplier = 1 if order_status.positionSide == "LONG" else -1
-        order = Order(
-            id=order_id.hex(),
-            amm_index=order_status.symbol,
-            trader=self.trader_address,
-            base_asset_quantity=float_to_scaled_int(float(order_status.origQty) * position_side_multiplier, 18),
-            price=float_to_scaled_int(float(order_status.price), 6),
-            salt=int(order_status.salt),
-            reduce_only=order_status.reduceOnly,
-        )
-        self.cancel_orders([order], tx_options, mode)
+    async def cancel_order_by_id(self, order_id: HexBytes, callback, tx_options = None, mode=None):
+        async def order_status_callback(response: OrderStatusResponse) -> Order:
+            position_side_multiplier = 1 if response.positionSide == "LONG" else -1
+            return Order(
+                id=order_id,
+                amm_index=response.symbol,
+                trader=self.trader_address,
+                base_asset_quantity=float_to_scaled_int(float(response.origQty) * position_side_multiplier, 18),
+                price=float_to_scaled_int(float(response.price), 6),
+                salt=int(response.salt),
+                reduce_only=response.reduceOnly,
+            )
+        order = await self.get_order_status(order_id, order_status_callback)
+        response = await self.cancel_orders([order], callback, tx_options, mode)
+        return await callback(response)
 
-    def subscribe_to_order_book_depth(
-        self, market: int, callback: Callable[[websocket.WebSocketApp, OrderBookDepthUpdateResponse], Any]
+    async def subscribe_to_order_book_depth(
+        self, market: int, callback: AsyncSubscribeToOrderBookDepthCallback
     ) -> None:
-
-        def on_open(ws):
+        async with websockets.connect(self.websocket_endpoint) as ws:
             msg = {
                 "jsonrpc": "2.0",
                 "id": 1,
                 "method": "trading_subscribe",
                 "params": ["streamDepthUpdateForMarket", market]
             }
-            ws.send(json.dumps(msg))
-
-        def on_message(ws, message):
-            message_json = json.loads(message)
-            response = WebsocketResponse(**message_json)
-            if response.method and response.method == "trading_subscription":
-                response = OrderBookDepthUpdateResponse(
-                    T=response.params['result']['T'],
-                    symbol=response.params['result']['s'],
-                    bids=response.params['result']['b'],
-                    asks=response.params['result']['a'],
-                )
-                callback(ws, response)
+            await ws.send(json.dumps(msg))
 
-        ws = websocket.WebSocketApp(self.websocket_endpoint, on_open=on_open, on_message=on_message)
-        ws.run_forever()
+            async for message in ws:
+                message_json = json.loads(message)
+                if message_json.get('result'):
+                    # ignore because it's a subscription confirmation with subscription id
+                    continue
+                response = WebsocketResponse(**message_json)
+                if response.method and response.method == "trading_subscription":
+                    response = OrderBookDepthUpdateResponse(
+                        T=response.params['result']['T'],
+                        symbol=response.params['result']['s'],
+                        bids=response.params['result']['b'],
+                        asks=response.params['result']['a'],
+                    )
+                    await callback(ws, response)
```

### Comparing `hubble_exchange-0.2.0/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.3.0/hubble_exchange/contract_abis/OrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.2.0/hubble_exchange/eip712.py` & `hubble_exchange-0.3.0/hubble_exchange/eip712.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.2.0/hubble_exchange/eth.py` & `hubble_exchange-0.3.0/hubble_exchange/eth.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.2.0/hubble_exchange/order_book.py` & `hubble_exchange-0.3.0/hubble_exchange/order_book.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.2.0/hubble_exchange.egg-info/PKG-INFO` & `hubble_exchange-0.3.0/hubble_exchange.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble-exchange
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,62 +42,63 @@
 The simplest way is to install the package from PyPI:
 ```shell
 pip install hubble-exchange
 ```
 
 ## Example usage:
 
-Requires HUBBLE_RPC_HOST and HUBBLE_BLOCKCHAIN_ID environment variable to be set
+All read/write functions are async
+<br>Requires HUBBLE_RPC_HOST and HUBBLE_BLOCKCHAIN_ID environment variable to be set
 ```shell
 export HUBBLE_RPC_HOST=candy-hubblenet-rpc.hubble.exchange
 export HUBBLE_BLOCKCHAIN_ID=iKMFgo49o4X3Pd3UWUkmPwjKom3xZz3Vo6Y1kkwL2Ce6DZaPm
 ```
 
 ```python
 import os
 from hubble_exchange import HubbleClient, OrderBookDepthResponse
 
 
-def main():
+async def main():
+
+    async def callback(response):
+        print(f"Received response: {response}")
+        return response
+
     client = HubbleClient(os.getenv("PRIVATE_KEY"))
     # place an order for market = 0, amount = 0.2, price = 1800, reduce_only = False
-    order = client.place_single_order(0, 0.2, 1800, False)
+    order = await client.place_single_order(0, 0.2, 1800, False, callback)
 
     # place multiple orders at once
     orders = []
     orders.append(Order.new(3, 1, 1.2, False)) # market = 3, qty = 1, price = 1.2, reduce_only = False
     orders.append(Order.new(0, 0.1, 1800, False)) # market = 0, qty = 0.1, price = 1800, reduce_only = False
     # placed_orders list will contain the order ids for the orders placed
-    placed_orders = client.place_orders(orders)
+    placed_orders = await client.place_orders(orders, callback)
 
     # get order status
-    order_status = client.get_order_status(order.Id)
+    order_status = await client.get_order_status(order.Id, callback)
     
     # cancel an order
-    client.cancel_orders([order])
+    await client.cancel_orders([order], callback)
 
     # order can also be cancelled by order id
-    client.cancel_order_by_id(order.id)
+    await client.cancel_order_by_id(order.id, callback)
 
     # get current order book for market = 1
-    order_book = client.get_order_book(1)
+    order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
-    positions = client.get_margin_and_positions()
+    positions = await client.get_margin_and_positions(callback)
 
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
-    # this is a blocking operation, so it needs to run in a separate thread
-    def callback(ws, message: OrderBookDepthResponse):
+    async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
-    client.subscribe_to_order_book_depth(0, callback=callback)
-
-
-if __name__ == "__main__":
-    main()
+    asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
 
 ## Custom transaction options
 
 The following options can be passed to the client to override the default
 
 ```python
@@ -112,15 +113,15 @@
 It can be used for `place_orders`, `place_single_order`, `cancel_orders`, `cancel_order_by_id` methods.
 Example:
 ```python
 
 from web3 import Web3
 
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
-placed_orders = client.place_orders(orders, {
+placed_orders = await client.place_orders(orders, callback, {
     "gas": 500_000,
     "maxFeePerGas": Web3.to_wei(80, 'gwei'),
     "maxPriorityFeePerGas": Web3.to_wei(20, 'gwei'),
 })
 ```
 
 ## Transaction modes
@@ -132,13 +133,13 @@
 - TransactionMode.wait_for_head: Wait for the transaction to be included in the canonical chain. At this time the block is preferred but not yet finalized. However, once the block in included in the canonical chain, the matching engine will start processing the order.
 - TransactionMode.wait_for_accept: Wait for the transaction to be finalised.
 
 Example:
 ```python
 from hubble_exchange import TransactionMode
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
-placed_orders = client.place_orders(orders, mode=TransactionMode.wait_for_accept)
+placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
-# or
+# or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
```

### Comparing `hubble_exchange-0.2.0/hubble_exchange.egg-info/SOURCES.txt` & `hubble_exchange-0.3.0/hubble_exchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.2.0/pyproject.toml` & `hubble_exchange-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.2.0"
+version = "0.3.0"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
     "eth_account >= 0.8.0",
     "requests >= 2.31.0",
-    "websocket-client >= 1.6.0",
     "eip712-structs >= 1.1.0",
 ]
 readme = "README.md"
 keywords = ["hubble", "exchange", "orderbook", "perpetual", "futures", "dex", "sdk", "python", "avalanche", "ethereum", "web3", "crypto"]
 
 [tool.setuptools]
 packages = ["hubble_exchange", "hubble_exchange.contract_abis"]
```

