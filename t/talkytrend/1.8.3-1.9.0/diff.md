# Comparing `tmp/talkytrend-1.8.3.tar.gz` & `tmp/talkytrend-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.8.3.tar", max compression
+gzip compressed data, was "talkytrend-1.9.0.tar", max compression
```

## Comparing `talkytrend-1.8.3.tar` & `talkytrend-1.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-17 06:28:58.370004 talkytrend-1.8.3/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-17 06:28:58.370004 talkytrend-1.8.3/README.md
--rw-r--r--   0        0        0     2475 2023-07-17 06:28:59.142008 talkytrend-1.8.3/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-17 06:28:59.142008 talkytrend-1.8.3/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-17 06:28:58.370004 talkytrend-1.8.3/talkytrend/config.py
--rw-r--r--   0        0        0     2285 2023-07-17 06:28:58.370004 talkytrend-1.8.3/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7377 2023-07-17 06:28:58.370004 talkytrend-1.8.3/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-17 16:47:26.940350 talkytrend-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-17 16:47:26.940350 talkytrend-1.9.0/README.md
+-rw-r--r--   0        0        0     2651 2023-07-17 16:47:27.692346 talkytrend-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-17 16:47:27.692346 talkytrend-1.9.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-17 16:47:26.940350 talkytrend-1.9.0/talkytrend/config.py
+-rw-r--r--   0        0        0     2216 2023-07-17 16:47:26.940350 talkytrend-1.9.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6450 2023-07-17 16:47:26.940350 talkytrend-1.9.0/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.9.0/PKG-INFO
```

### Comparing `talkytrend-1.8.3/LICENSE` & `talkytrend-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.3/README.md` & `talkytrend-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.3/pyproject.toml` & `talkytrend-1.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.8.3"
+version = "1.9.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
@@ -27,36 +27,36 @@
 dynaconf = "^3.1.12"
 aiohttp = "^3.8.4"
 tradingview_ta = "^3.3.0"
 prettytable = "^3.8.0"
 alphavantage_api_client = "^2.2.2"
 xmltodict = "*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.0"
+ruff = "^0.0.278"
+
+[tool.ruff]
+# select = [
+#   "E",  # pycodestyle
+#   "F",  # pyflakes
+#   "I",  # isort
+# ]
+exclude = [
+  ".github/*",
+  "docs/*",
+]
+ignore = ["E401"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.0"
-sphinx_bootstrap_theme = "^0.8.1"
-sphinx-autoapi = "^2.1.1"
-sphinx-copybutton= "^0.5.2"
-myst-parser = "^2.0.0"
-sphinx-notfound-page = "^0.8.3"
-sphinxext-remoteliteralinclude = "^0.4.0"
-sphinx-togglebutton = "*"
-
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
@@ -64,14 +64,27 @@
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0.0"
+sphinx_bootstrap_theme = "^0.8.1"
+sphinx-autoapi = "^2.1.1"
+sphinx-copybutton= "^0.5.2"
+myst-parser = "^2.0.0"
+sphinx-notfound-page = "^0.8.3"
+sphinxext-remoteliteralinclude = "^0.4.0"
+sphinx-togglebutton = "*"
+
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","talkytrend/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
```

### Comparing `talkytrend-1.8.3/talkytrend/config.py` & `talkytrend-1.9.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.3/talkytrend/default_settings.toml` & `talkytrend-1.9.0/talkytrend/default_settings.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,57 +8,52 @@
 # As an example, to change the port settings:
 # settings.toml
 # [default]
 # scanner_frequency = 3600
 # or via ENVVARS 
 # export TT_SCANNER_FREQUENCY=3600
 
-
 [default]
 VALUE = "On Default"
 talkytrend_enabled = true
-talkytrend_mode = "scanner"
-talkytrend_scanner = true
-talkytrend_scheduler = false
-scanner_frequency = 86400
+scanner_frequency = 7200
 enable_signals = true
 assets = [
-    { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
-    { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
-    # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
-    # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
-    # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
-    #use https://tvdb.brianthe.dev/ to get details
+    { id ="EURUSD", exchange='FX_IDC',screener="forex"},
+    { id ="BTCUSD", exchange='BINANCE',screener="crypto"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-09-20","2023-11-01","2023-12-13"]
+live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&max=2&apikey="
 news_api_key = ""
 enable_feed = true
-#news_feed="http://feeds.feedburner.com/zerohedge/feed"
-news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
-live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
-
+news_feed = "https://www.dailyfx.com/feeds/market-news"
 
 
 [testing]
 VALUE = "On Testing"
 talkytrend_enabled = true
-talkytrend_mode = "scanner"
-talkytrend_scanner = false
-talkytrend_scheduler = false
 scanner_frequency = 2
 enable_signals = true
 assets = [
-    { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
+    { id ="EURUSD", exchange='FX_IDC',screener="forex"},
+    { id ="BTCUSD",exchange="BINANCE",screener="crypto"},
+    # { id ="GOLD",exchange="TVC",screener="cfd"},
+    # { id ="USOIL",exchange="FX",screener="cfd"},
+    # { id ="ETHUSD",exchange="BINANCE",screener="crypto"},
+    # use https://tvdb.brianthe.dev/ to get details
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
+live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
 enable_feed = true
-news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
-live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
+news_feed = "http://feeds.feedburner.com/zerohedge/feed/"
+# news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
+# news_feed = "https://www.dailyfx.com/feeds/market-news"
+#news_feed="https://www.reutersagency.com/feed/?taxonomy=best-sectors&post_type=best"
```

### Comparing `talkytrend-1.8.3/talkytrend/main.py` & `talkytrend-1.9.0/talkytrend/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 
 class TalkyTrend:
     def __init__(self):
         self.logger = logging.getLogger("TalkyTrend")
         self.enabled = settings.talkytrend_enabled
         if not self.enabled:
             return
-        self.mode = settings.talkytrend_mode
         self.assets = settings.assets
         self.asset_signals = {}
         self.economic_calendar = settings.economic_calendar
         self.news_url = (
             f"{settings.news_url}{settings.news_api_key}"
             if settings.news_api_key
             else settings.news_url
         )
         self.live_tv = settings.live_tv_url
 
+    async def get_talkytrend_info(self):
+        return (f"ℹ️ {__class__.__name__} {__version__}\n")
 
     async def fetch_analysis(
         self,
         asset_id,
         exchange,
         screener,
         interval):
@@ -53,60 +54,38 @@
             elif analysis.summary["RECOMMENDATION"] == 'SELL':
                 return "🔽"
             elif analysis.summary["RECOMMENDATION"] == 'STRONG_SELL':
                 return "⏬"
             else:
                 return "▶️"
         except Exception as error:
-            self.logger.error("event %s", error)
-
-
-    async def get_talkytrend_info(self):
-        return (f"ℹ️ {__class__.__name__} {__version__}\n")
+            self.logger.warning("event %s", error)
 
-    async def check_signal(self):
+    async def check_signal(self, interval="4h"):
         signals = []
         table = PrettyTable()
-        table.field_names = ["Asset","4h"]
+        table.field_names = [" Trend ", interval]
+
         for asset in self.assets:
             current_signal = await self.fetch_analysis(
                 asset_id=asset["id"],
                 exchange=asset["exchange"],
                 screener=asset["screener"],
-                interval=asset["interval"]
+                interval=interval
             )
-            if self.is_new_signal(asset["id"], asset["interval"], current_signal):
+            if current_signal:
                 signal_item = {
                     "symbol": asset["id"],
-                    "interval": asset["interval"],
+                    "interval": interval,
                     "signal": current_signal
                 }
-                self.update_signal(asset["id"], asset["interval"], current_signal)
                 table.add_row([asset["id"], current_signal])
                 signals.append(signal_item)
-                return table.get_string()
 
-    def is_new_signal(self, asset_id, interval, current_signal):
-        if asset_id not in self.asset_signals:
-            self.asset_signals[asset_id] = {}
-        if interval not in self.asset_signals[asset_id]:
-            self.asset_signals[asset_id][interval] = current_signal
-            return True
-        elif current_signal != self.asset_signals[asset_id][interval]:
-            self.asset_signals[asset_id][interval] = current_signal
-            return True
-        return False
-
-    def update_signal(self, asset_id, interval, current_signal):
-        if asset_id not in self.asset_signals:
-            self.asset_signals[asset_id] = {}
-        self.asset_signals[asset_id][interval] = current_signal
-
-    def get_asset_signals(self):
-        return self.asset_signals
+        return table.get_string()
 
     async def fetch_key_events(self):
         def filter_events(data, today):
             return [event for event in data if event.get('date', '').startswith(today)]
 
         def is_usd_high_impact(event):
             return (
@@ -132,47 +111,47 @@
                 for event in events:
                     if is_usd_high_impact(event) or is_all_high_impact(event):
                         return format_event(event)
                     if is_opec_or_fomc(event):
                         return format_event(event)
         return None
 
-    async def fetch_key_news(self):
-        try:
-            async with aiohttp.ClientSession() as session:
-                async with session.get(self.news_url, timeout=10) as response:
-                    data = await response.json()
-                    articles = data.get('articles', [])
-                    key_news = [
-                        {'title': article['title'], 'url': article['url']}
-                        for article in articles
-                    ]
-                    last_item = key_news[-1]
-                    return f"📰 <a href='{last_item['url']}'>{last_item['title']}</a>"
-
-        except aiohttp.ClientError as error:
-            self.logger.error("news %s", error)
-            return None
-
     async def fetch_key_feed(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(settings.news_feed, timeout=10) as response:
                     data = (
                         xmltodict.parse(await response.text())
                         .get('rss')
                         .get('channel')['item'][0]
                     )
                     title = data['title']
                     link = data['link']
                     return f"📰 <a href='{link}'>{title}</a>"
         except Exception as error:
-            self.logger.error("event %s", error)
+            self.logger.warning("feed %s", error)
             return None
 
+    # async def fetch_key_news(self):
+    #     try:
+    #         async with aiohttp.ClientSession() as session:
+    #             async with session.get(self.news_url, timeout=10) as response:
+    #                 data = await response.json()
+    #                 articles = data.get('articles', [])
+    #                 key_news = [
+    #                     {'title': article['title'], 'url': article['url']}
+    #                     for article in articles
+    #                 ]
+    #                 last_item = key_news[-1]
+    #                 return f"📰 <a href='{last_item['url']}'>{last_item['title']}</a>"
+
+    #     except aiohttp.ClientError as error:
+    #         self.logger.warning("news %s", error)
+    #         return None
+
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
 
     async def get_tv(self):
         if self.live_tv:
@@ -182,19 +161,18 @@
         return bool(enable)
 
     async def scanner(self):
         while await self.allow_scanning():
             if settings.enable_events:
                 if await self.fetch_key_events() is not None:
                     yield await self.fetch_key_events()
-            if settings.enable_news:
-                if await self.fetch_key_news() is not None:
-                    yield await self.fetch_key_news()
+            # if settings.enable_news:
+            #     if await self.fetch_key_news() is not None:
+            #         yield await self.fetch_key_news()
             if settings.enable_feed:
                 if await self.fetch_key_feed() is not None:
                     yield await self.fetch_key_feed()
             if settings.enable_signals:
                 if await self.check_signal() is not None:
                     yield await self.check_signal()
 
             await asyncio.sleep(settings.scanner_frequency)
-
```

### Comparing `talkytrend-1.8.3/PKG-INFO` & `talkytrend-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.8.3
+Version: 1.9.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.8.3 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.9.0 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

