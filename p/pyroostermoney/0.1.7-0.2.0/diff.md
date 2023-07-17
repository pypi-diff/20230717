# Comparing `tmp/pyroostermoney-0.1.7.tar.gz` & `tmp/pyroostermoney-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.7.tar", last modified: Sun Jul 16 21:53:27 2023, max compression
+gzip compressed data, was "pyroostermoney-0.2.0.tar", last modified: Mon Jul 17 19:19:00 2023, max compression
```

## Comparing `pyroostermoney-0.1.7.tar` & `pyroostermoney-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.865571 pyroostermoney-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 21:53:27.873571 pyroostermoney-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.935281 pyroostermoney-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.935281 pyroostermoney-0.2.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/child/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/child/standing_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/child/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-17 19:19:00.000000 pyroostermoney-0.2.0/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 19:19:00.000000 pyroostermoney-0.2.0/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:19:00.000000 pyroostermoney-0.2.0/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:19:00.000000 pyroostermoney-0.2.0/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 19:19:00.000000 pyroostermoney-0.2.0/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 19:19:00.939281 pyroostermoney-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-17 19:18:48.000000 pyroostermoney-0.2.0/setup.py
```

### Comparing `pyroostermoney-0.1.7/.github/scripts/release.py` & `pyroostermoney-0.2.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/.github/workflows/build.yml` & `pyroostermoney-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/.gitignore` & `pyroostermoney-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/LICENSE` & `pyroostermoney-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/PKG-INFO` & `pyroostermoney-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.7
+Version: 0.2.0
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.7/pyroostermoney/api.py` & `pyroostermoney-0.2.0/pyroostermoney/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,24 +34,40 @@
                                 auth=auth) as response:
             text = await response.text()
             return {
                 "status": response.status,
                 "response": json.loads(text)
             }
 
+async def _delete_request(url, body: dict, auth=None, headers=None):
+    if headers is None:
+        headers=HEADERS
+    async with aiohttp.ClientSession() as session:
+        async with session.delete(f"{BASE_URL}/{url}",
+                                json=body,
+                                headers=headers,
+                                auth=auth) as response:
+            text = await response.text()
+            return {
+                "status": response.status,
+                "response": json.loads(text)
+            }
+
 class RoosterSession:
     """The main Rooster Session."""
 
-    def __init__(self, username: str, password: str) -> None:
+    def __init__(self, username: str, password: str, update_interval: int=30, use_updater: bool=False) -> None:
         self._username = username
         self._password = password
         self._session = None
         self._headers = HEADERS
         self._logged_in = False
         self._logging_in = asyncio.Lock()
+        self.update_interval = update_interval
+        self.use_updater = use_updater
 
     async def async_login(self):
         """Logs into RoosterMoney and starts a new active session."""
         if self._logging_in.locked():
             _LOGGER.warning("Login already attempting. Only one execution allowed.")
             while self._logging_in.locked():
                 await asyncio.sleep(1)
@@ -136,26 +152,29 @@
         if add_security_token:
             headers["securitytoken"] = self._session["security_code"]
 
         if method == "GET":
             return await _fetch_request(url, headers=headers)
         elif method == "POST":
             return await _post_request(url, body=body, headers=headers)
+        elif method == "DELETE":
+            return await _delete_request(url, body=body, headers=headers)
         else:
             raise ValueError("Invalid type argument.")
 
     async def request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
                                         auth=None,
                                         method="GET",
                                         login_request=False,
                                         add_security_token=False):
         """Public calls for the private _internal_request_handler."""
+        _LOGGER.debug(f"Sending {method} HTTP request to {url}")
         try:
             return await self._internal_request_handler(
                 url=url,
                 body=body,
                 headers=headers,
                 auth=auth,
                 method=method,
@@ -170,7 +189,15 @@
                 headers=headers,
                 auth=auth,
                 method=method,
                 login_request=login_request
             )
         except NotLoggedIn as exc:
             raise NotLoggedIn() from exc
+        except aiohttp.ClientOSError as exc:
+            # silent exc handler
+            if exc.errno == 104: # connection reset by peer
+                _LOGGER.debug("Connection reset by peer - retrying request.")
+                asyncio.sleep(5)
+                await self.request_handler(**locals())
+            else:
+                raise aiohttp.ClientOSError from exc
```

### Comparing `pyroostermoney-0.1.7/pyroostermoney/child/card.py` & `pyroostermoney-0.2.0/pyroostermoney/child/card.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.2.0/pyroostermoney/child/money_pot.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/pyroostermoney/const.py` & `pyroostermoney-0.2.0/pyroostermoney/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.1.7"
+VERSION="0.2.0"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
@@ -23,26 +23,31 @@
     "get_account_info": "api/parent",
     "get_child": "api/parent/child/{user_id}",
     "get_child_allowance_periods": "api/parent/child/{user_id}/allowance-periods",
     "get_top_up_methods": "api/parent/acquirer/topup/methods?currency={currency}",
     "get_available_cards": "api/parent/acquirer/cards",
     "get_family_account": "api/parent/family/account",
     "get_child_pocket_money": "api/parent/child/{user_id}/pocketmoney",
-    "get_child_allowance_period_jobs": "api/parent/child/{user_id}/allowance-periods/{allowance_period_id}",
+    "get_child_allowance_period_jobs": "api/parent/child/{user_id}/allowance-periods/{allowance_period_id}/jobs",
     "get_master_jobs": "api/parent/master-jobs",
     "get_child_spend_history": "api/parent/child/{user_id}/spendHistory?count={count}",
     "create_payment": "api/parent/acquirer/create-payment",
     "get_child_card_details": "api/parent/child/{user_id}/card/details",
     "get_child_card_pin": "api/parent/child/{user_id}/cards/{card_id}/pin",
-    "get_family_account_cards": "api/parent/family/cards"
+    "get_family_account_cards": "api/parent/family/cards",
+    "get_child_standing_orders": "api/parent/child/{user_id}/standingorder",
+    "create_child_standing_order": "api/parent/child/{user_id}/standingorder/",
+    "delete_child_standing_order": "api/parent/child/{user_id}/standingorder/{delete_child_standing_order}",
+    "get_master_job_list": "api/parent/master-jobs"
 }
 
 HEADERS = {
     "content-type": "application/json",
-    "accept": "application/json"
+    "accept": "application/json",
+    "user-agent": f"Mozilla/5.0 Rooster Money {MOBILE_APP_VERSION}"
 }
 
 LOGIN_BODY={
     "countryOfResidence": COUNTRY,
     "cultureCode": LANGUAGE,
     "currency": CURRENCY,
     "dismissibleAlertSections": [],
```

### Comparing `pyroostermoney-0.1.7/pyroostermoney/exceptions.py` & `pyroostermoney-0.2.0/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.7/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.2.0/pyroostermoney.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.7
+Version: 0.2.0
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.7/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.2.0/pyroostermoney.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 pyroostermoney.egg-info/PKG-INFO
 pyroostermoney.egg-info/SOURCES.txt
 pyroostermoney.egg-info/dependency_links.txt
 pyroostermoney.egg-info/requires.txt
 pyroostermoney.egg-info/top_level.txt
 pyroostermoney/child/__init__.py
 pyroostermoney/child/card.py
-pyroostermoney/child/money_pot.py
+pyroostermoney/child/jobs.py
+pyroostermoney/child/money_pot.py
+pyroostermoney/child/standing_order.py
+pyroostermoney/child/transaction.py
```

