# Comparing `tmp/epson_connect-0.2.2.tar.gz` & `tmp/epson_connect-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epson_connect-0.2.2.tar", max compression
+gzip compressed data, was "epson_connect-0.2.3.tar", max compression
```

## Comparing `epson_connect-0.2.2.tar` & `epson_connect-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.2/LICENSE
--rw-r--r--   0        0        0      763 2023-07-12 23:18:21.630580 epson_connect-0.2.2/README.md
--rw-r--r--   0        0        0     1339 2023-07-13 00:42:37.047774 epson_connect-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.2/src/epson_connect/__init__.py
--rw-r--r--   0        0        0     3661 2023-07-13 00:22:52.026520 epson_connect-0.2.2/src/epson_connect/authenticate.py
--rw-r--r--   0        0        0     1265 2023-07-12 23:49:14.792209 epson_connect-0.2.2/src/epson_connect/client.py
--rw-r--r--   0        0        0     4460 2023-07-12 23:51:36.755455 epson_connect-0.2.2/src/epson_connect/printer.py
--rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.2/src/epson_connect/printer_settings.py
--rw-r--r--   0        0        0     2450 2023-07-12 19:25:30.140848 epson_connect-0.2.2/src/epson_connect/scanner.py
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 epson_connect-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.3/LICENSE
+-rw-r--r--   0        0        0      763 2023-07-12 23:18:21.630580 epson_connect-0.2.3/README.md
+-rw-r--r--   0        0        0     1339 2023-07-16 22:43:30.432780 epson_connect-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.3/src/epson_connect/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-13 00:22:52.026520 epson_connect-0.2.3/src/epson_connect/authenticate.py
+-rw-r--r--   0        0        0     1265 2023-07-12 23:49:14.792209 epson_connect-0.2.3/src/epson_connect/client.py
+-rw-r--r--   0        0        0     4459 2023-07-16 22:42:48.040335 epson_connect-0.2.3/src/epson_connect/printer.py
+-rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.3/src/epson_connect/printer_settings.py
+-rw-r--r--   0        0        0     2450 2023-07-12 19:25:30.140848 epson_connect-0.2.3/src/epson_connect/scanner.py
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 epson_connect-0.2.3/PKG-INFO
```

### Comparing `epson_connect-0.2.2/LICENSE` & `epson_connect-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.2/README.md` & `epson_connect-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.2/pyproject.toml` & `epson_connect-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epson-connect"
-version = "0.2.2"
+version = "0.2.3"
 description = "Bindings for the Espon Connect API"
 license = "MIT"
 authors = ["Paul Logston <paul.logston@gmail.com>"]
 maintainers = ["Paul Logston <paul.logston@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/epson-connect/"
 repository = "https://github.com/logston/epson-connect"
```

### Comparing `epson_connect-0.2.2/src/epson_connect/authenticate.py` & `epson_connect-0.2.3/src/epson_connect/authenticate.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.2/src/epson_connect/client.py` & `epson_connect-0.2.3/src/epson_connect/client.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.2/src/epson_connect/printer.py` & `epson_connect-0.2.3/src/epson_connect/printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         return self._auth_ctx.send(method, path)
 
     def notification(self, callback_uri, enabled=True):
         """
         Set whether or not to notify of the print job status change.
         """
         method = 'POST'
-        path = f'/api/1/printing/printers/{self.device_id}/settings/notifications'
+        path = f'/api/1/printing/printers/{self.device_id}/settings/notification'
 
         data = {
             'notification': enabled,
             'callback_uri': callback_uri,
         }
 
         return self._auth_ctx.send(method, path, json=data)
```

### Comparing `epson_connect-0.2.2/src/epson_connect/printer_settings.py` & `epson_connect-0.2.3/src/epson_connect/printer_settings.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.2/src/epson_connect/scanner.py` & `epson_connect-0.2.3/src/epson_connect/scanner.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.2/PKG-INFO` & `epson_connect-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epson-connect
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bindings for the Espon Connect API
 Home-page: https://pypi.org/project/epson-connect/
 License: MIT
 Keywords: epson,connect,api
 Author: Paul Logston
 Author-email: paul.logston@gmail.com
 Maintainer: Paul Logston
```

