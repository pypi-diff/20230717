# Comparing `tmp/unitauto-1.0.0.tar.gz` & `tmp/unitauto-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-rnhs14bd/unitauto-1.0.0.tar", last modified: Mon Jul 17 13:53:55 2023, max compression
+gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-1rivqg0l/unitauto-1.0.1.tar", last modified: Mon Jul 17 15:31:39 2023, max compression
```

## Comparing `unitauto-1.0.0.tar` & `unitauto-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 13:53:37.000000 unitauto-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 13:53:55.000000 unitauto-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 13:53:37.000000 unitauto-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 13:53:37.000000 unitauto-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 13:53:55.000000 unitauto-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29657 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/methodutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 15:31:21.000000 unitauto-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 15:31:39.000000 unitauto-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 15:31:21.000000 unitauto-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 15:31:21.000000 unitauto-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 15:31:39.000000 unitauto-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/methodutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-1.0.0/LICENSE` & `unitauto-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.0/PKG-INFO` & `unitauto-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unitauto-1.0.0/README.md` & `unitauto-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.0/setup.cfg` & `unitauto-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 1.0.0
+version = 1.0.1
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-1.0.0/unitauto/methodutil.py` & `unitauto-1.0.1/unitauto/methodutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     getinstance: callable = get_instance
 
 
 listener = Listener()
 
 
 def list_method(req) -> dict:
-    start_time = time.time_ns()
+    start_time = cur_time_in_millis()
     try:
         if is_str(req):
             req = parse_json(req)
 
         mock = req.get(KEY_MOCK)
         assert mock in [null, true, false], KEY_MOCK + ' must be in [true, false]!'
 
@@ -466,14 +466,15 @@
         KEY_METHOD_ARGS: mas,
         KEY_TIME_DETAIL: time_detail
     }
 
 
 def invoke_method(req: any, callback: callable = null) -> dict:
     start_time = time.time_ns()
+    is_wait = false
     try:
         assert is_none(callback) or callable(callback)
 
         if is_str(req):
             req = parse_json(req)
 
         static = req.get(KEY_STATIC)
@@ -564,32 +565,37 @@
                 c_kwargs = {}
                 init_args(class_args, ca_keys, ca_types, ca_values, c_kwargs)
                 instance = cls(*ca_values, **c_kwargs) if constructor_func is None else constructor_func(*ca_values, **c_kwargs)
 
             func = getattr(instance, method)
 
         ksl = size(m_kwargs)
-        start_time = time.time_ns()
+        start_time = cur_time_in_millis()
 
+        # TODO 自动识别 async 关键词
         result = asyncio.run(func(*ma_values[:mal-ksl], **m_kwargs)) if is_async \
             else func(*ma_values[:mal-ksl], **m_kwargs)  # asyncio.run 只允许调 async 函数 is_async != false
 
         final_result[KEY_VALUE] = result
-        return wrap_result(func, method_args, ma_types, ma_values, result, start_time)
+        res = wrap_result(func, method_args, ma_types, ma_values, result, start_time)
     except Exception as e:
-        return {
+        res = {
             KEY_LANGUAGE: LANGUAGE,
             KEY_OK: false,
             KEY_CODE: CODE_SERVER_ERROR,
             KEY_MSG: str(e),
             KEY_TIME_DETAIL: get_time_detail(start_time),
             KEY_THROW: e.__class__.__name__,
             # KEY_TRACE: e.__traceback__.__str__()
         }
 
+    if (not is_wait) and callable(callback):
+        callback(res)
+    return res
+
 
 def init_args(
     method_args: list, ma_keys: list, ma_types: list, ma_values: list,
     ma_kwargs: dict, keep_kwargs_in_types_and_values: bool = false, callback: callable = null
 ):
     is_wait = false
     mal = size(method_args)
@@ -874,17 +880,17 @@
 
 def cur_time_in_millis() -> int:
     return round(time.time_ns()/MILLIS_TIME)
 
 
 def get_time_detail(start_time: int, end_time: int = 0):
     if end_time is None or end_time <= 0:
-        end_time = time.time_ns()
+        end_time = cur_time_in_millis()
     duration = end_time - start_time
-    return str(round(start_time/MILLIS_TIME)) + '|' + str(round(duration/MILLIS_TIME)) + '|' + str(round(end_time/MILLIS_TIME))
+    return str(round(start_time)) + '|' + str(round(duration)) + '|' + str(round(end_time))
 
 
 def parse_json(s: str):
     return json.loads(s)
 
 
 def to_json_str(obj, indent: int = 2) -> str:
```

### Comparing `unitauto-1.0.0/unitauto/server.py` & `unitauto-1.0.1/unitauto/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,54 +39,69 @@
 CONTENT_TYPE = 'application/json; charset=UTF-8'
 
 
 class Request(BaseHTTPRequestHandler):
     timeout = 5
     server_version = "Apache"
 
+    def send_headers(self, origin, method='POST'):
+        self.send_header(KEY_CONTENT_TYPE, CONTENT_TYPE)
+        self.send_header('Access-Control-Allow-Origin', origin)
+        self.send_header('Access-Control-Allow-Credentials', 'true')
+        self.send_header('Access-Control-Allow-Headers', 'Content-Type,content-type')
+        self.send_header('Access-Control-Allow-Methods', 'POST,GET,OPTIONS')
+        self.send_header('Access-Control-Request-Method', method)
+
+        self.end_headers()
+
     def do_OPTIONS(self):
         self.do_POST()
 
     def do_POST(self):
         method = self.command
         client_address = self.client_address
         host = 'http://' + client_address[0] + ':' + str(client_address[1])
         path = self.path
         print(method + ' ' + host + path)
         if path not in ['/method/list', '/method/invoke']:
             raise Exception('only support /method/list, /method/invoke')
 
         origin = self.headers.get('origin') or self.headers.get('Origin') or 'http://apijson.cn'
 
-        self.send_response(RESPONSE_CODE_SUCCESS)
-        self.send_header(KEY_CONTENT_TYPE, CONTENT_TYPE)
-        self.send_header('Access-Control-Allow-Origin', origin)
-        self.send_header('Access-Control-Allow-Credentials', 'true')
-        self.send_header('Access-Control-Allow-Headers', 'Content-Type,content-type')
-        self.send_header('Access-Control-Allow-Methods', 'POST,GET,OPTIONS')
-        self.send_header('Access-Control-Request-Method', method)
-
-        self.end_headers()
-
         if method == 'OPTIONS':
+            self.send_response(RESPONSE_CODE_SUCCESS)
+            self.send_headers(origin, method)
             # self.wfile.write('ok'.encode())
             return
 
         bs = self.rfile.read(int(self.headers[KEY_CONTENT_LENGTH]))
         req = bs.decode()  # bs.decode(CHARSET)
         # req = urllib.unquote(bs).decode(CHARSET, 'ignore')
 
-        def callback(rsp):
-            rsp_str = to_json_str(rsp)
-            self.wfile.write(rsp_str.encode())
+        done = [false]
+
+        def callback(res):
+            res_str = to_json_str(res)
+            res_byte = res_str.encode()
+            self.send_response(RESPONSE_CODE_SUCCESS)
+            self.send_headers(origin, method)
+            if done[0] or self.wfile.closed:
+                return
+            self.wfile.write(res_byte)
+            self.wfile.close()
+            done[0] = true
+
         if path == '/method/list':
             rsp = list_method(req)
             callback(rsp)
         else:
             invoke_method(req, callback)
+            while true:
+                if done[0]:
+                    break
 
 
 def start(host=HOST):
     server = HTTPServer(host, Request)
     print("Starting server, listen at: %s:%s" % host)
     server.serve_forever()
 
@@ -189,15 +204,15 @@
             {
                 # KEY_KEY: 'b',
                 KEY_TYPE: 'int',
                 KEY_VALUE: 5
             },
             {
                 KEY_KEY: 'callback',
-                KEY_TYPE: 'def(a,b,c)',
+                KEY_TYPE: 'def(a,b)',
                 KEY_VALUE: {
                     KEY_TYPE: 'int',
                     KEY_RETURN: 'a - b',
                     KEY_CALLBACK: true
                 }
             }
         ]
```

### Comparing `unitauto-1.0.0/unitauto/test/__init__.py` & `unitauto-1.0.1/unitauto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.0/unitauto/test/testutil.py` & `unitauto-1.0.1/unitauto/test/testutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 def compute_async(a, b, callback):
     print('start >>> ')
 
     def fun():
         time.sleep(3)
         print('callback >>> ')
-        ret = callback(a, b, a + b)
+        ret = callback(a, b)
         print('ret = ' + str(ret))
 
     thd = threading.Thread(target=fun)
     thd.start()
 
     print('return <<<')
     return True
```

### Comparing `unitauto-1.0.0/unitauto.egg-info/PKG-INFO` & `unitauto-1.0.1/unitauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

