# Comparing `tmp/anicli_api-0.4.3.tar.gz` & `tmp/anicli_api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.4.3.tar", max compression
+gzip compressed data, was "anicli_api-0.4.4.tar", max compression
```

## Comparing `anicli_api-0.4.3.tar` & `anicli_api-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.3/README.MD
--rw-r--r--   0        0        0     2940 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/_http.py
--rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.3/anicli_api/_logger.py
--rw-r--r--   0        0        0     3242 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/base.py
--rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.3/anicli_api/player/__init__.py
--rw-r--r--   0        0        0      921 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/__template__.py
--rw-r--r--   0        0        0     2147 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/aniboom.py
--rw-r--r--   0        0        0     1055 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/animejoy.py
--rw-r--r--   0        0        0     3434 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/base.py
--rw-r--r--   0        0        0     1198 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/csst.py
--rw-r--r--   0        0        0     1456 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/dzen.py
--rw-r--r--   0        0        0     3894 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/kodik.py
--rw-r--r--   0        0        0     1837 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/mailru.py
--rw-r--r--   0        0        0     1697 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/okru.py
--rw-r--r--   0        0        0     1106 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/sibnet.py
--rw-r--r--   0        0        0     1139 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/sovetromantica.py
--rw-r--r--   0        0        0     1527 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/player/vkcom.py
--rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.3/anicli_api/source/__init__.py
--rw-r--r--   0        0        0     2516 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/source/__template__.py
--rw-r--r--   0        0        0     6163 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/source/anilibria.py
--rw-r--r--   0        0        0    10586 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/source/animego.py
--rw-r--r--   0        0        0     8722 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/source/animejoy.py
--rw-r--r--   0        0        0     5543 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/source/animevost.py
--rw-r--r--   0        0        0     6462 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/source/sovetromantica.py
--rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.3/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.3/anicli_api/tools/random_useragent.py
--rw-r--r--   0        0        0      198 2023-07-14 17:47:29.562755 anicli_api-0.4.3/anicli_api/tools/utils.py
--rw-r--r--   0        0        0     2342 2023-07-16 08:51:49.664204 anicli_api-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.4/README.MD
+-rw-r--r--   0        0        0     2940 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/_http.py
+-rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.4/anicli_api/_logger.py
+-rw-r--r--   0        0        0     3242 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/base.py
+-rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.4/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     2147 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0     1055 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3434 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1198 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1456 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     4047 2023-07-17 10:02:25.493422 anicli_api-0.4.4/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1837 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1697 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1106 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0     1139 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/sovetromantica.py
+-rw-r--r--   0        0        0     1527 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.4/anicli_api/source/__init__.py
+-rw-r--r--   0        0        0     2516 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     6163 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0    10586 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     8722 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     5543 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0     6462 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/sovetromantica.py
+-rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.4/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.4/anicli_api/tools/random_useragent.py
+-rw-r--r--   0        0        0      198 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/tools/utils.py
+-rw-r--r--   0        0        0     2342 2023-07-17 10:02:43.744188 anicli_api-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.4/PKG-INFO
```

### Comparing `anicli_api-0.4.3/README.MD` & `anicli_api-0.4.4/README.MD`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/_http.py` & `anicli_api-0.4.4/anicli_api/_http.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/_logger.py` & `anicli_api-0.4.4/anicli_api/_logger.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/base.py` & `anicli_api-0.4.4/anicli_api/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/__init__.py` & `anicli_api-0.4.4/anicli_api/player/__init__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/__template__.py` & `anicli_api-0.4.4/anicli_api/player/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/aniboom.py` & `anicli_api-0.4.4/anicli_api/player/aniboom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/animejoy.py` & `anicli_api-0.4.4/anicli_api/player/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/base.py` & `anicli_api-0.4.4/anicli_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/csst.py` & `anicli_api-0.4.4/anicli_api/player/csst.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/dzen.py` & `anicli_api-0.4.4/anicli_api/player/dzen.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/kodik.py` & `anicli_api-0.4.4/anicli_api/player/kodik.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,20 @@
             return chr(
                 (ord(e.group(0)) + 13 - (65 if e.group(0) <= "Z" else 97)) % 26 + (65 if e.group(0) <= "Z" else 97)
             )
 
         base64_url = re.sub(r"[a-zA-Z]", char_wrapper, url_encoded)
         if not base64_url.endswith("=="):
             base64_url += "=="
-        return f"https:{b64decode(base64_url).decode()}"
+        decoded_url = b64decode(base64_url).decode()
+        return (
+            decoded_url
+            if decoded_url.startswith("https")
+            else f"https:{b64decode(base64_url).decode()}"
+        )
 
     @kodik_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
         response = self.http.get(url).text
         payload = _KodikPayload(response).dict()
         url_api = f"https://{urlsplit(url).netloc}/gvi"
         response_api = self.http.post(
```

### Comparing `anicli_api-0.4.3/anicli_api/player/mailru.py` & `anicli_api-0.4.4/anicli_api/player/mailru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/okru.py` & `anicli_api-0.4.4/anicli_api/player/okru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/sibnet.py` & `anicli_api-0.4.4/anicli_api/player/sibnet.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/sovetromantica.py` & `anicli_api-0.4.4/anicli_api/player/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/player/vkcom.py` & `anicli_api-0.4.4/anicli_api/player/vkcom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/source/__template__.py` & `anicli_api-0.4.4/anicli_api/source/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/source/anilibria.py` & `anicli_api-0.4.4/anicli_api/source/anilibria.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/source/animego.py` & `anicli_api-0.4.4/anicli_api/source/animego.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/source/animejoy.py` & `anicli_api-0.4.4/anicli_api/source/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/source/animevost.py` & `anicli_api-0.4.4/anicli_api/source/animevost.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/source/sovetromantica.py` & `anicli_api-0.4.4/anicli_api/source/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/anicli_api/tools/random_useragent.py` & `anicli_api-0.4.4/anicli_api/tools/random_useragent.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.3/pyproject.toml` & `anicli_api-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.4.3"
+version = "0.4.4"
 description = "Anime extractor api implementation"
 authors = ["Georgiy aka Vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/"]
 keywords = [
```

### Comparing `anicli_api-0.4.3/PKG-INFO` & `anicli_api-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: Anime extractor api implementation
 License: MIT
 Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
 Author: Georgiy aka Vypivshiy
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

