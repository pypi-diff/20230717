# Comparing `tmp/volstreet-1.0.2.tar.gz` & `tmp/volstreet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.2.tar", last modified: Mon Jul 17 06:14:21 2023, max compression
+gzip compressed data, was "volstreet-1.0.3.tar", last modified: Mon Jul 17 06:23:35 2023, max compression
```

## Comparing `volstreet-1.0.2.tar` & `volstreet-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:21.095025 volstreet-1.0.2/
--rw-rw-rw-   0        0        0      497 2023-07-17 06:14:21.095025 volstreet-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.2/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-17 06:14:21.096065 volstreet-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:21.089407 volstreet-1.0.2/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.2/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.2/volstreet/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.2/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.2/volstreet/constants.py
--rw-rw-rw-   0        0        0    42479 2023-07-16 12:56:47.000000 volstreet-1.0.2/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   192050 2023-07-17 05:57:04.000000 volstreet-1.0.2/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.2/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.2/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.2/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13244 2023-07-17 06:10:46.000000 volstreet-1.0.2/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:21.095025 volstreet-1.0.2/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-17 06:14:21.000000 volstreet-1.0.2/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-17 06:14:21.000000 volstreet-1.0.2/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:14:21.000000 volstreet-1.0.2/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-17 06:14:21.000000 volstreet-1.0.2/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-17 06:14:21.000000 volstreet-1.0.2/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 06:23:35.823495 volstreet-1.0.3/
+-rw-rw-rw-   0        0        0      497 2023-07-17 06:23:35.823495 volstreet-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.3/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-17 06:23:35.824491 volstreet-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 06:23:35.817514 volstreet-1.0.3/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.3/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.3/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.3/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.3/volstreet/constants.py
+-rw-rw-rw-   0        0        0    42479 2023-07-16 12:56:47.000000 volstreet-1.0.3/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   192050 2023-07-17 05:57:04.000000 volstreet-1.0.3/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.3/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.3/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.3/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13257 2023-07-17 06:22:53.000000 volstreet-1.0.3/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:23:35.822498 volstreet-1.0.3/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 06:23:35.000000 volstreet-1.0.3/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.2/setup.cfg` & `volstreet-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 320d 0a61  rsion = 1.0.2..a
+00000020: 7273 696f 6e20 3d20 312e 302e 330d 0a61  rsion = 1.0.3..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.2/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.3/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/blackscholes.py` & `volstreet-1.0.3/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/constants.py` & `volstreet-1.0.3/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/datamodule.py` & `volstreet-1.0.3/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/dealingroom.py` & `volstreet-1.0.3/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/discord_bot.py` & `volstreet-1.0.3/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/nsefunctions.py` & `volstreet-1.0.3/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.2/volstreet/strategies.py` & `volstreet-1.0.3/volstreet/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         webhook_url=discord_webhook_url,
     )
     nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
     bnf = vs.Index("BANKNIFTY", webhook_url=discord_webhook_url)
     fin = vs.Index("FINNIFTY", webhook_url=discord_webhook_url)
     midcap = vs.Index("MIDCPNIFTY", webhook_url=discord_webhook_url)
 
-    indices = vs.get_strangle_indices_to_trade(nifty, bnf, fin, midcap, safe_indices)
+    indices = vs.get_strangle_indices_to_trade(nifty, bnf, fin, midcap, safe_indices=safe_indices)
 
     parameters["quantity_in_lots"] = parameters["quantity_in_lots"] // len(indices)
 
     # Setting the shared data
     if shared_data:
         shared_data = vs.SharedData()
         update_data_thread = threading.Thread(target=shared_data.update_data)
```

### Comparing `volstreet-1.0.2/volstreet.egg-info/requires.txt` & `volstreet-1.0.3/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

