# Comparing `tmp/talkytrend-1.8.1.tar.gz` & `tmp/talkytrend-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.8.1.tar", max compression
+gzip compressed data, was "talkytrend-1.8.2.tar", max compression
```

## Comparing `talkytrend-1.8.1.tar` & `talkytrend-1.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-15 14:17:52.561806 talkytrend-1.8.1/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-15 14:17:52.561806 talkytrend-1.8.1/README.md
--rw-r--r--   0        0        0     2476 2023-07-15 14:17:53.489825 talkytrend-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-15 14:17:53.489825 talkytrend-1.8.1/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-15 14:17:52.561806 talkytrend-1.8.1/talkytrend/config.py
--rw-r--r--   0        0        0     2285 2023-07-15 14:17:52.561806 talkytrend-1.8.1/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7386 2023-07-15 14:17:52.561806 talkytrend-1.8.1/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-17 05:55:37.496523 talkytrend-1.8.2/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-17 05:55:37.496523 talkytrend-1.8.2/README.md
+-rw-r--r--   0        0        0     2476 2023-07-17 05:55:38.264550 talkytrend-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-17 05:55:38.264550 talkytrend-1.8.2/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-17 05:55:37.496523 talkytrend-1.8.2/talkytrend/config.py
+-rw-r--r--   0        0        0     2285 2023-07-17 05:55:37.496523 talkytrend-1.8.2/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7377 2023-07-17 05:55:37.496523 talkytrend-1.8.2/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.8.2/PKG-INFO
```

### Comparing `talkytrend-1.8.1/LICENSE` & `talkytrend-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.1/README.md` & `talkytrend-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.1/pyproject.toml` & `talkytrend-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.8.1"
+version = "1.8.2"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.8.1/talkytrend/config.py` & `talkytrend-1.8.2/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.1/talkytrend/default_settings.toml` & `talkytrend-1.8.2/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.1/talkytrend/main.py` & `talkytrend-1.8.2/talkytrend/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,16 @@
                         xmltodict.parse(await response.text())
                         .get('rss')
                         .get('channel')['item'][0]
                     )
                     title = data['title']
                     link = data['link']
                     return f"📰 <a href='{link}'>{title}</a>"
-        except aiohttp.ClientError as error:
-            self.logger.error("feed %s", error)
+        except Exception as error:
+            self.logger.error("event %s", error)
             return None
 
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
```

### Comparing `talkytrend-1.8.1/PKG-INFO` & `talkytrend-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.8.1
+Version: 1.8.2
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
-Metadata-Version: 2.1 Name: talkytrend Version: 1.8.1 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.8.2 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

