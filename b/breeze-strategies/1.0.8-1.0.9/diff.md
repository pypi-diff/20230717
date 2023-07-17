# Comparing `tmp/breeze_strategies-1.0.8.tar.gz` & `tmp/breeze_strategies-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-1.0.8.tar", last modified: Fri Jul 14 08:42:16 2023, max compression
+gzip compressed data, was "breeze_strategies-1.0.9.tar", last modified: Fri Jul 14 09:27:05 2023, max compression
```

## Comparing `breeze_strategies-1.0.8.tar` & `breeze_strategies-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 08:42:16.824458 breeze_strategies-1.0.8/
--rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1727 2023-07-14 08:42:16.823459 breeze_strategies-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2023-07-14 08:42:11.000000 breeze_strategies-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 08:42:16.768874 breeze_strategies-1.0.8/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.8/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    28425 2023-07-14 08:41:54.000000 breeze_strategies-1.0.8/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:42:16.821449 breeze_strategies-1.0.8/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1727 2023-07-14 08:42:16.000000 breeze_strategies-1.0.8/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-14 08:42:16.000000 breeze_strategies-1.0.8/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 08:42:16.000000 breeze_strategies-1.0.8/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-14 08:42:16.000000 breeze_strategies-1.0.8/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-14 08:42:16.000000 breeze_strategies-1.0.8/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 08:42:16.824458 breeze_strategies-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-07-14 08:41:50.000000 breeze_strategies-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:27:05.033542 breeze_strategies-1.0.9/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1894 2023-07-14 09:27:05.031254 breeze_strategies-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2023-07-14 09:26:55.000000 breeze_strategies-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 09:27:05.000470 breeze_strategies-1.0.9/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.9/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    28433 2023-07-14 09:22:21.000000 breeze_strategies-1.0.9/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:27:05.029254 breeze_strategies-1.0.9/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1894 2023-07-14 09:27:04.000000 breeze_strategies-1.0.9/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-14 09:27:04.000000 breeze_strategies-1.0.9/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:27:04.000000 breeze_strategies-1.0.9/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-14 09:27:04.000000 breeze_strategies-1.0.9/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-14 09:27:04.000000 breeze_strategies-1.0.9/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 09:27:05.033542 breeze_strategies-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-14 09:26:32.000000 breeze_strategies-1.0.9/setup.py
```

### Comparing `breeze_strategies-1.0.8/LICENSE` & `breeze_strategies-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.8/PKG-INFO` & `breeze_strategies-1.0.9/breeze_strategies.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze_strategies
-Version: 1.0.8
+Name: breeze-strategies
+Version: 1.0.9
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.8
+pip install breeze_strategies==1.0.9
 
 ```
 
 ## Updating Library
 
 ```python
 
@@ -54,17 +54,20 @@
              quantity = "50",
              expiry_date = "2023-06-29T06:00:00.000Z")
 
 #Execute Single Leg
 obj.single_leg(right = "Call", strategy_type = "short",stock_code = "NIFTY", strike_price = "18700", quantity = "50", expiry_date = "2023-06-29T06:00:00.000Z")
 
 
-#SquareOff existing positions and exit the strategy
+#SquareOff existing positions and exit the strategy for straddle
 obj.stop() 
 
+#SquareOff existing positions and exit the strategy In case of single_leg pass single_leg flag as True as mentioned below
+obj.stop(single_leg = True)
+
 
 #Generate Profit & Loss report
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-1.0.8/README.md` & `breeze_strategies-1.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.8
+pip install breeze_strategies==1.0.9
 
 ```
 
 ## Updating Library
 
 ```python
 
@@ -38,16 +38,19 @@
              quantity = "50",
              expiry_date = "2023-06-29T06:00:00.000Z")
 
 #Execute Single Leg
 obj.single_leg(right = "Call", strategy_type = "short",stock_code = "NIFTY", strike_price = "18700", quantity = "50", expiry_date = "2023-06-29T06:00:00.000Z")
 
 
-#SquareOff existing positions and exit the strategy
+#SquareOff existing positions and exit the strategy for straddle
 obj.stop() 
 
+#SquareOff existing positions and exit the strategy In case of single_leg pass single_leg flag as True as mentioned below
+obj.stop(single_leg = True)
+
 
 #Generate Profit & Loss report
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-1.0.8/breeze_strategies/breeze_strategies.py` & `breeze_strategies-1.0.9/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
                 self.profit_and_loss(product_type, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price,call_execution,put_execution)
             
     
     
     
-    def stop(self,single_leg):
+    def stop(self,single_leg = False):
         if(self.socket == 1):
             self.client.ws_disconnect()
         self.socket = 0
         time.sleep(1)
         print("\n")
         print("Squaring off the  contracts and exiting strategy...")
         print("----------------------------------------")
```

### Comparing `breeze_strategies-1.0.8/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze-strategies
-Version: 1.0.8
+Name: breeze_strategies
+Version: 1.0.9
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.8
+pip install breeze_strategies==1.0.9
 
 ```
 
 ## Updating Library
 
 ```python
 
@@ -54,17 +54,20 @@
              quantity = "50",
              expiry_date = "2023-06-29T06:00:00.000Z")
 
 #Execute Single Leg
 obj.single_leg(right = "Call", strategy_type = "short",stock_code = "NIFTY", strike_price = "18700", quantity = "50", expiry_date = "2023-06-29T06:00:00.000Z")
 
 
-#SquareOff existing positions and exit the strategy
+#SquareOff existing positions and exit the strategy for straddle
 obj.stop() 
 
+#SquareOff existing positions and exit the strategy In case of single_leg pass single_leg flag as True as mentioned below
+obj.stop(single_leg = True)
+
 
 #Generate Profit & Loss report
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-1.0.8/setup.py` & `breeze_strategies-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="1.0.8",
+    version="1.0.9",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

