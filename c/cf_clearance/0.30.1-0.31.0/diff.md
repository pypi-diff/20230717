# Comparing `tmp/cf_clearance-0.30.1.tar.gz` & `tmp/cf_clearance-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_clearance-0.30.1.tar", last modified: Thu Jul 13 04:03:26 2023, max compression
+gzip compressed data, was "cf_clearance-0.31.0.tar", last modified: Mon Jul 17 04:16:18 2023, max compression
```

## Comparing `cf_clearance-0.30.1.tar` & `cf_clearance-0.31.0.tar`

### file list

```diff
@@ -1,21 +1,16 @@
--rw-r--r--   0        0        0    11343 2023-06-16 09:27:03.281672 cf_clearance-0.30.1/LICENSE
--rw-r--r--   0        0        0     6117 2023-07-13 03:42:57.357841 cf_clearance-0.30.1/README.md
--rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.30.1/cf_clearance/.DS_Store
--rw-r--r--   0        0        0      336 2023-07-13 03:41:27.148526 cf_clearance-0.30.1/cf_clearance/__init__.py
--rw-r--r--   0        0        0      118 2023-06-07 07:53:29.052052 cf_clearance-0.30.1/cf_clearance/errors.py
--rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.30.1/cf_clearance/js/canvas.fingerprinting.js
--rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.30.1/cf_clearance/js/chrome.global.js
--rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.30.1/cf_clearance/js/chrome.plugin.js
--rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.30.1/cf_clearance/js/chrome.runtime.js
--rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.30.1/cf_clearance/js/emulate.touch.js
--rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.30.1/cf_clearance/js/navigator.permissions.js
--rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.30.1/cf_clearance/js/navigator.webdriver.js
--rw-r--r--   0        0        0     2285 2023-07-13 04:01:31.970692 cf_clearance-0.30.1/cf_clearance/retry.py
--rw-r--r--   0        0        0     3677 2023-07-13 02:29:58.161925 cf_clearance-0.30.1/cf_clearance/stealth.py
--rw-r--r--   0        0        0     1006 2023-07-13 04:03:26.339413 cf_clearance-0.30.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.30.1/tests/__init__.py
--rw-r--r--   0        0        0     1816 2023-07-13 03:27:14.859270 cf_clearance-0.30.1/tests/test_async_cf.py
--rw-r--r--   0        0        0      715 2023-06-07 07:53:29.055195 cf_clearance-0.30.1/tests/test_common.py
--rw-r--r--   0        0        0     1020 2023-07-13 04:01:41.773088 cf_clearance-0.30.1/tests/test_cron_challenge.py
--rw-r--r--   0        0        0     1671 2023-07-13 03:27:14.859795 cf_clearance-0.30.1/tests/test_sync_cf.py
--rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 cf_clearance-0.30.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-16 09:27:03.281672 cf_clearance-0.31.0/LICENSE
+-rw-r--r--   0        0        0     3542 2023-07-17 03:47:23.266678 cf_clearance-0.31.0/README.md
+-rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.31.0/cf_clearance/.DS_Store
+-rw-r--r--   0        0        0      336 2023-07-13 03:41:27.148526 cf_clearance-0.31.0/cf_clearance/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 09:22:52.890643 cf_clearance-0.31.0/cf_clearance/js/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.31.0/cf_clearance/js/canvas.fingerprinting.js
+-rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.31.0/cf_clearance/js/chrome.global.js
+-rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.31.0/cf_clearance/js/chrome.plugin.js
+-rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.31.0/cf_clearance/js/chrome.runtime.js
+-rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.31.0/cf_clearance/js/emulate.touch.js
+-rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.31.0/cf_clearance/js/navigator.permissions.js
+-rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.31.0/cf_clearance/js/navigator.webdriver.js
+-rw-r--r--   0        0        0     2558 2023-07-15 09:35:58.051956 cf_clearance-0.31.0/cf_clearance/retry.py
+-rw-r--r--   0        0        0     3650 2023-07-15 09:22:52.891139 cf_clearance-0.31.0/cf_clearance/stealth.py
+-rw-r--r--   0        0        0     1330 2023-07-17 04:16:18.438424 cf_clearance-0.31.0/pyproject.toml
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 cf_clearance-0.31.0/PKG-INFO
```

### Comparing `cf_clearance-0.30.1/LICENSE` & `cf_clearance-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/.DS_Store` & `cf_clearance-0.31.0/cf_clearance/.DS_Store`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/js/canvas.fingerprinting.js` & `cf_clearance-0.31.0/cf_clearance/js/canvas.fingerprinting.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/js/chrome.global.js` & `cf_clearance-0.31.0/cf_clearance/js/chrome.global.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/js/chrome.plugin.js` & `cf_clearance-0.31.0/cf_clearance/js/chrome.plugin.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/js/chrome.runtime.js` & `cf_clearance-0.31.0/cf_clearance/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/js/navigator.permissions.js` & `cf_clearance-0.31.0/cf_clearance/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.1/cf_clearance/retry.py` & `cf_clearance-0.31.0/cf_clearance/retry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import logging
 from typing import Tuple
 
 from playwright.async_api import Error
 from playwright.async_api import Page as AsyncPage
 from playwright.sync_api import Page as SyncPage
 
 
@@ -12,27 +13,28 @@
     user_tries = tries
     while tries > 0:
         await page.wait_for_timeout(1500)
         try:
             success = False if await page.query_selector("#challenge-form") else True
             if success:
                 break
-            simple_challenge = await page.query_selector(
-                "#challenge-stage > div > input[type='button']"
-            )
-            if simple_challenge:
-                await simple_challenge.click()
             for target_frame in page.main_frame.child_frames:
                 if "challenge" in target_frame.url and "turnstile" in target_frame.url:
-                    click = await target_frame.query_selector(
-                        "xpath=//input[@type='checkbox']"
-                    )
-                    if click:
-                        await click.click()
+                    try:
+                        click = await target_frame.query_selector(
+                            "xpath=//input[@type='checkbox']"
+                        )
+                    except Error:
+                        # frame is refreshed, so playwright._impl._api_types.Error: Target closed
+                        logging.debug("Playwright Error:", exc_info=True)
+                    else:
+                        if click:
+                            await click.click()
         except Error:
+            logging.debug("Playwright Error:", exc_info=True)
             success = False
         tries -= 1
     if tries == user_tries:
         cf = False
     return success, cf
 
 
@@ -42,25 +44,26 @@
     user_tries = tries
     while tries > 0:
         page.wait_for_timeout(1500)
         try:
             success = False if page.query_selector("#challenge-form") else True
             if success:
                 break
-            simple_challenge = page.query_selector(
-                "#challenge-stage > div > input[type='button']"
-            )
-            if simple_challenge:
-                simple_challenge.click()
             for target_frame in page.main_frame.child_frames:
                 if "challenge" in target_frame.url and "turnstile" in target_frame.url:
-                    click = target_frame.query_selector(
-                        "xpath=//input[@type='checkbox']"
-                    )
-                    if click:
-                        click.click()
+                    try:
+                        click = target_frame.query_selector(
+                            "xpath=//input[@type='checkbox']"
+                        )
+                    except Error:
+                        # frame is refreshed, so playwright._impl._api_types.Error: Target closed
+                        logging.debug("Playwright Error:", exc_info=True)
+                    else:
+                        if click:
+                            click.click()
         except Error:
+            logging.debug("Playwright Error:", exc_info=True)
             success = False
         tries -= 1
     if tries == user_tries:
         cf = False
     return success, cf
```

### Comparing `cf_clearance-0.30.1/cf_clearance/stealth.py` & `cf_clearance-0.31.0/cf_clearance/stealth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 import re
 from dataclasses import dataclass
+from importlib.resources import read_text
 from typing import Dict, Union
 
-import pkg_resources
 from playwright.async_api import BrowserContext as AsyncContext
 from playwright.async_api import Page as AsyncPage
 from playwright.sync_api import BrowserContext as SyncContext
 from playwright.sync_api import Page as SyncPage
 
 
 def from_file(name):
     """Read script from ./js directory"""
-    return pkg_resources.resource_string("cf_clearance", f"js/{name}").decode()
+
+    return read_text("cf_clearance.js", f"{name}")
 
 
 SCRIPTS: Dict[str, str] = {
     "chrome_fp": from_file("canvas.fingerprinting.js"),
     "chrome_global": from_file("chrome.global.js"),
     "chrome_touch": from_file("emulate.touch.js"),
     "navigator_permissions": from_file("navigator.permissions.js"),
@@ -70,36 +71,36 @@
             yield SCRIPTS["chrome_plugin"]
         if self.chrome_runtime:
             yield SCRIPTS["chrome_runtime"]
 
 
 def sync_stealth(
     page_or_context: Union[SyncContext, SyncPage],
-    config: StealthConfig = None,
+    config: StealthConfig = StealthConfig(),
     pure: bool = True,
 ):
     """teaches synchronous playwright Page to be stealthy like a ninja!"""
-    for script in (config or StealthConfig()).enabled_scripts:
+    for script in config.enabled_scripts:
         page_or_context.add_init_script(script)
     if pure:
         page_or_context.route(
             re.compile(
                 r"(.*\.png(\?.*|$))|(.*\.jpg(\?.*|$))|(.*\.jpeg(\?.*|$))|(.*\.css(\?.*|$))"
             ),
             lambda route: route.abort("blockedbyclient"),
         )
 
 
 async def async_stealth(
     page_or_context: Union[AsyncContext, AsyncPage],
-    config: StealthConfig = None,
+    config: StealthConfig = StealthConfig(),
     pure: bool = True,
 ):
     """teaches asynchronous playwright Page to be stealthy like a ninja!"""
-    for script in (config or StealthConfig()).enabled_scripts:
+    for script in config.enabled_scripts:
         await page_or_context.add_init_script(script)
     if pure:
         await page_or_context.route(
             re.compile(
                 r"(.*\.png(\?.*|$))|(.*\.jpg(\?.*|$))|(.*\.jpeg(\?.*|$))|(.*\.css(\?.*|$))"
             ),
             lambda route: route.abort("blockedbyclient"),
```

