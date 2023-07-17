# Comparing `tmp/villa-0.7.0.tar.gz` & `tmp/villa-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.7.0.tar", max compression
+gzip compressed data, was "villa-0.7.1.tar", max compression
```

## Comparing `villa-0.7.0.tar` & `villa-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-07-17 10:09:09.644517 villa-0.7.0/LICENSE
--rw-r--r--   0        0        0     3747 2023-07-17 10:09:09.644517 villa-0.7.0/README.md
--rw-r--r--   0        0        0     2140 2023-07-17 10:09:09.644517 villa-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      277 2023-07-17 10:09:09.644517 villa-0.7.0/villa/__init__.py
--rw-r--r--   0        0        0    40806 2023-07-17 10:09:09.644517 villa-0.7.0/villa/bot.py
--rw-r--r--   0        0        0    12215 2023-07-17 10:09:09.644517 villa-0.7.0/villa/event.py
--rw-r--r--   0        0        0     1835 2023-07-17 10:09:09.644517 villa-0.7.0/villa/exception.py
--rw-r--r--   0        0        0     3337 2023-07-17 10:09:09.644517 villa-0.7.0/villa/handle.py
--rw-r--r--   0        0        0     1537 2023-07-17 10:09:09.644517 villa-0.7.0/villa/log.py
--rw-r--r--   0        0        0    21359 2023-07-17 10:09:09.644517 villa-0.7.0/villa/message.py
--rw-r--r--   0        0        0     9304 2023-07-17 10:09:09.644517 villa-0.7.0/villa/models.py
--rw-r--r--   0        0        0      935 2023-07-17 10:09:09.644517 villa-0.7.0/villa/store.py
--rw-r--r--   0        0        0      240 2023-07-17 10:09:09.644517 villa-0.7.0/villa/typing.py
--rw-r--r--   0        0        0      968 2023-07-17 10:09:09.644517 villa-0.7.0/villa/utils.py
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-17 10:49:59.663911 villa-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3747 2023-07-17 10:49:59.663911 villa-0.7.1/README.md
+-rw-r--r--   0        0        0     2140 2023-07-17 10:49:59.663911 villa-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-17 10:49:59.663911 villa-0.7.1/villa/__init__.py
+-rw-r--r--   0        0        0    40693 2023-07-17 10:49:59.663911 villa-0.7.1/villa/bot.py
+-rw-r--r--   0        0        0    12215 2023-07-17 10:49:59.663911 villa-0.7.1/villa/event.py
+-rw-r--r--   0        0        0     1835 2023-07-17 10:49:59.663911 villa-0.7.1/villa/exception.py
+-rw-r--r--   0        0        0     3337 2023-07-17 10:49:59.663911 villa-0.7.1/villa/handle.py
+-rw-r--r--   0        0        0     1537 2023-07-17 10:49:59.663911 villa-0.7.1/villa/log.py
+-rw-r--r--   0        0        0    21359 2023-07-17 10:49:59.663911 villa-0.7.1/villa/message.py
+-rw-r--r--   0        0        0     9304 2023-07-17 10:49:59.663911 villa-0.7.1/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-17 10:49:59.663911 villa-0.7.1/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-17 10:49:59.663911 villa-0.7.1/villa/typing.py
+-rw-r--r--   0        0        0      968 2023-07-17 10:49:59.663911 villa-0.7.1/villa/utils.py
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.1/PKG-INFO
```

### Comparing `villa-0.7.0/LICENSE` & `villa-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/README.md` & `villa-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/pyproject.toml` & `villa-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.7.0"
+version = "0.7.1"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.7.0/villa/bot.py` & `villa-0.7.1/villa/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -988,16 +988,15 @@
     ):
         sign = base64.b64decode(bot_sign)
         sign_data = urlencode(
             {"body": body.rstrip("\n"), "secret": self.bot_secret},
         ).encode()
         try:
             rsa.verify(sign_data, sign, self.pub_key)
-        except rsa.VerificationError as e:
-            logger.exception(e)
+        except rsa.VerificationError:
             return False
         return True
 
     async def _close_client(self) -> None:
         """关闭 HTTP Client"""
         await self._client.aclose()
 
@@ -1278,31 +1277,29 @@
     )
 
 
 async def handle_event(
     data: Dict[str, Any],
     request: Request,
     backgroud_tasks: BackgroundTasks,
-    # bot_sign: str = Header(..., alias="x-rpc-bot_sign"),
 ) -> JSONResponse:
     """处理事件"""
     if not (payload_data := data.get("event", None)):
         logger.warning(f"Received invalid data: {escape_tag(str(data))}")
         return JSONResponse(
             status_code=415,
             content={"retcode": 415, "msg": "Invalid data"},
         )
     try:
         event = parse_obj_as(event_classes, pre_handle_event(payload_data))
         if (bot := get_bot(event.bot_id)) is None:
             raise ValueError(f"Bot {event.bot_id} not found")
-        if (
-            bot.verify_event
-            and (bot_sign := request.headers.get("x-rpc-bot_sign")) is not None
-            and not bot._verify_signature((await request.body()).decode(), bot_sign)
+        if bot.verify_event and (
+            (bot_sign := request.headers.get("x-rpc-bot_sign")) is None
+            or not bot._verify_signature((await request.body()).decode(), bot_sign)
         ):
             logger.opt(colors=True).warning(
                 (
                     f"Bot <b><m>{bot.bot_id}</m></b> "
                     f"received invalid signature: <b><m>{bot_sign}</m></b>"
                 ),
             )
```

### Comparing `villa-0.7.0/villa/event.py` & `villa-0.7.1/villa/event.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/exception.py` & `villa-0.7.1/villa/exception.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/handle.py` & `villa-0.7.1/villa/handle.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/log.py` & `villa-0.7.1/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/message.py` & `villa-0.7.1/villa/message.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/models.py` & `villa-0.7.1/villa/models.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/store.py` & `villa-0.7.1/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/villa/utils.py` & `villa-0.7.1/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.0/PKG-INFO` & `villa-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.7.0
+Version: 0.7.1
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

