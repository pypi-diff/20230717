# Comparing `tmp/volstreet-1.0.3.tar.gz` & `tmp/volstreet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.3.tar", last modified: Mon Jul 17 06:23:35 2023, max compression
+gzip compressed data, was "volstreet-1.0.4.tar", last modified: Mon Jul 17 11:47:39 2023, max compression
```

## Comparing `volstreet-1.0.3.tar` & `volstreet-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:23:35.823495 volstreet-1.0.3/
--rw-rw-rw-   0        0        0      497 2023-07-17 06:23:35.823495 volstreet-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.3/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-17 06:23:35.824491 volstreet-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 06:23:35.817514 volstreet-1.0.3/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.3/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.3/volstreet/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.3/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.3/volstreet/constants.py
--rw-rw-rw-   0        0        0    42479 2023-07-16 12:56:47.000000 volstreet-1.0.3/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   192050 2023-07-17 05:57:04.000000 volstreet-1.0.3/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.3/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.3/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.3/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13257 2023-07-17 06:22:53.000000 volstreet-1.0.3/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:23:35.822498 volstreet-1.0.3/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 11:47:39.162629 volstreet-1.0.4/
+-rw-rw-rw-   0        0        0      497 2023-07-17 11:47:39.164013 volstreet-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.4/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-17 11:47:39.164013 volstreet-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 11:47:39.157669 volstreet-1.0.4/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.4/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.4/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.4/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.4/volstreet/constants.py
+-rw-rw-rw-   0        0        0    42479 2023-07-16 12:56:47.000000 volstreet-1.0.4/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   192075 2023-07-17 11:46:59.000000 volstreet-1.0.4/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.4/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.4/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.4/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13257 2023-07-17 06:22:53.000000 volstreet-1.0.4/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:47:39.162629 volstreet-1.0.4/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-17 11:47:39.000000 volstreet-1.0.4/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-17 11:47:39.000000 volstreet-1.0.4/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:47:39.000000 volstreet-1.0.4/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-17 11:47:39.000000 volstreet-1.0.4/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 11:47:39.000000 volstreet-1.0.4/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.3/setup.cfg` & `volstreet-1.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 330d 0a61  rsion = 1.0.3..a
+00000020: 7273 696f 6e20 3d20 312e 302e 340d 0a61  rsion = 1.0.4..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.3/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.4/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet/blackscholes.py` & `volstreet-1.0.4/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet/constants.py` & `volstreet-1.0.4/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet/datamodule.py` & `volstreet-1.0.4/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet/dealingroom.py` & `volstreet-1.0.4/volstreet/dealingroom.py`

 * *Files 0% similar despite different names*

```diff
@@ -2957,15 +2957,15 @@
         def process_stop_loss(info_dict, sl_type):
             if (
                 info_dict["call_sl"] and info_dict["put_sl"]
             ):  # Check to avoid double processing
                 return
 
             traded_strangle = info_dict["traded_strangle"]
-            other_side = "call" if sl_type == "put" else "put"
+            other_side: str = "call" if sl_type == "put" else "put"
 
             # Buying the stop loss option back if it is not already bought
             if info_dict[f"{sl_type}_stop_loss_order_ids"] is None:
                 option_to_buy = (
                     traded_strangle.call_option
                     if sl_type == "call"
                     else traded_strangle.put_option
@@ -3302,28 +3302,28 @@
                     self.webhook_url,
                     return_avg_price=True,
                 )
             shared_info_dict["call_exit_price"] = call_exit_avg_price
             shared_info_dict["put_exit_price"] = put_exit_avg_price
 
         elif (call_sl or put_sl) and not (call_sl and put_sl):  # Only one stop loss hit
-            exit_option = "put" if call_sl else "call"
+            exit_option_type: str = "put" if call_sl else "call"
             if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
-                non_sl_exit_price = shared_info_dict[f"{exit_option}_ltp"]
+                non_sl_exit_price = shared_info_dict[f"{exit_option_type}_ltp"]
             else:
                 exit_option = strangle.put_option if call_sl else strangle.call_option
                 non_sl_exit_price = place_option_order_and_notify(
                     exit_option,
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
                     self.webhook_url,
                 )
-            shared_info_dict[f"{exit_option}_exit_price"] = non_sl_exit_price
+            shared_info_dict[f"{exit_option_type}_exit_price"] = non_sl_exit_price
 
         else:  # Both stop losses hit
             pass
 
         # Calculate profit
         total_exit_price = (
             shared_info_dict["call_exit_price"] + shared_info_dict["put_exit_price"]
@@ -3393,16 +3393,16 @@
 
         # Price deque
         n_prices = max(int(minutes_to_avg / sleep_time), 1)
         price_deque = deque(maxlen=n_prices)
 
         notifier(
             f"{self.name} trender starting with {threshold_movement:0.2f} threshold movement\n"
-            f"Current Price: {open_price}\nUpper limit: {price_boundaries[1]:0.2f}\n"
-            f"Lower limit: {price_boundaries[0]:0.2f}.",
+            f"Current Price: {open_price}\nUpper limit: {price_boundaries[0]:0.2f}\n"
+            f"Lower limit: {price_boundaries[1]:0.2f}.",
             self.webhook_url,
         )
 
         entries = 0
         last_print_time = currenttime()
         movement = 0
         while entries < max_entries and currenttime().time() < exit_time:
```

### Comparing `volstreet-1.0.3/volstreet/discord_bot.py` & `volstreet-1.0.4/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet/nsefunctions.py` & `volstreet-1.0.4/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet/strategies.py` & `volstreet-1.0.4/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.3/volstreet.egg-info/requires.txt` & `volstreet-1.0.4/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

