# Comparing `tmp/unitauto-0.9.3.tar.gz` & `tmp/unitauto-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-kvrcup18/unitauto-0.9.3.tar", last modified: Sat Jun 24 17:24:48 2023, max compression
+gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-rnhs14bd/unitauto-1.0.0.tar", last modified: Mon Jul 17 13:53:55 2023, max compression
```

## Comparing `unitauto-0.9.3.tar` & `unitauto-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 17:24:27.000000 unitauto-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 17:24:48.000000 unitauto-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-24 17:24:27.000000 unitauto-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 17:24:27.000000 unitauto-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 17:24:48.000000 unitauto-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21771 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/methodutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 13:53:37.000000 unitauto-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 13:53:55.000000 unitauto-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 13:53:37.000000 unitauto-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 13:53:37.000000 unitauto-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 13:53:55.000000 unitauto-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29657 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/methodutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 13:53:37.000000 unitauto-1.0.0/unitauto/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 13:53:55.000000 unitauto-1.0.0/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-0.9.3/LICENSE` & `unitauto-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.3/PKG-INFO` & `unitauto-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.9.3
+Version: 1.0.0
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unitauto-0.9.3/README.md` & `unitauto-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.3/setup.cfg` & `unitauto-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 0.9.3
+version = 1.0.0
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-0.9.3/unitauto/methodutil.py` & `unitauto-1.0.0/unitauto/methodutil.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
+import asyncio
+import builtins
 import json
+import re
 import time
 import inspect
 from typing import Type
 
 null = None
 false = False
 true = True
@@ -46,19 +48,21 @@
 KEY_UI = "ui"
 KEY_TIME = "time"
 KEY_TIMEOUT = "timeout"
 KEY_PACKAGE = "package"
 KEY_THIS = "this"
 KEY_CLASS = "class"
 KEY_CONSTRUCTOR = "constructor"
+KEY_KEY = 'key'
 KEY_TYPE = "type"
 KEY_AT_TYPE = "@type"
 KEY_VALUE = "value"
 KEY_WARN = "warn"
 KEY_STATIC = "static"
+KEY_ASYNC = "async"
 KEY_NAME = "name"
 KEY_METHOD = "method"
 KEY_MOCK = "mock"
 KEY_QUERY = "query"
 KEY_RETURN = "return"
 KEY_TIME_DETAIL = "time:start|duration|end"
 KEY_CLASS_ARGS = "classArgs"
@@ -71,14 +75,20 @@
 KEY_PACKAGE_TOTAL = "packageTotal"
 KEY_CLASS_TOTAL = "classTotal"
 KEY_METHOD_TOTAL = "methodTotal"
 KEY_PACKAGE_LIST = "packageList"
 KEY_CLASS_LIST = "classList"
 KEY_METHOD_LIST = "methodList"
 
+MILLIS_TIME = 1000000
+
+PATTERN_ALPHABET = re.compile('^[A-Za-z]+$')
+PATTERN_NUMBER = re.compile('^[0-9]+$')
+PATTERN_NAME = re.compile('^[A-Za-z0-9_]+$')
+
 PRIMITIVE_CLASS_MAP = {
     None: any,
     'None': any,
     'any': any,
     'bool': bool,
     'False': bool,
     'True': bool,
@@ -124,25 +134,50 @@
     'staticmethod': staticmethod,
     'super': super,
     'type': type,
     'zip': zip,
 })
 
 
+class InterfaceProxy:
+    pass
+
+
+def get_instance(self, typ: Type, value: any, class_args: list = null, reuse: bool = false):
+    return
+
+
+def on_complete(data: any, method: callable, proxy: InterfaceProxy, *extras: any):
+    pass
+
+
+def on_callback(data: any, method: callable, proxy: InterfaceProxy, *extras: any):
+    pass
+
+
+class Listener:
+    complete: callable = on_complete
+    callback: callable = on_callback
+    getinstance: callable = get_instance
+
+
+listener = Listener()
+
+
 def list_method(req) -> dict:
     start_time = time.time_ns()
     try:
         if is_str(req):
             req = parse_json(req)
 
         mock = req.get(KEY_MOCK)
-        assert mock in [null, true, false], KEY_MOCK + ' must must in [true, false]!'
+        assert mock in [null, true, false], KEY_MOCK + ' must be in [true, false]!'
 
         query = req.get(KEY_QUERY)
-        assert query in [null, 0, 1, 2], KEY_QUERY + ' must must in [0, 1, 2]! 0-Data, 1-Total count, 2-Both above'
+        assert query in [null, 0, 1, 2], KEY_QUERY + ' must be in [0, 1, 2]! 0-Data, 1-Total count, 2-Both above'
 
         package = req.get(KEY_PACKAGE)
         assert is_str(package), KEY_PACKAGE + ' must be str!'
 
         clazz = req.get(KEY_CLASS)
         assert is_str(clazz), KEY_CLASS + ' must be str!'
 
@@ -378,23 +413,79 @@
         'parameterTypeList': types if static else types[1:],
         'genericParameterTypeList': types if static else types[1:],
         'parameterNameList': names if static else names[1:],
         'parameterDefaultValueList': null
     }
 
 
-def invoke_method(req: any) -> dict:
+def wrap_result(func, method_args, ma_types, ma_values, result, start_time):
+    time_detail = get_time_detail(start_time)
+
+    signature = inspect.signature(func)
+    return_annotation = null if signature is None else signature.return_annotation
+    rt = null
+    if return_annotation is not None:
+        try:
+            rt = return_annotation.__name__
+            if rt in ('_empty', 'POSITIONAL_OR_KEYWORD'):
+                rt = type(result).__name__
+        except Exception as e:
+            print(e)
+            rt = type(result).__name__  # str(return_annotation)
+
+    mal = size(method_args)
+    mas = [null] * mal
+    if mal > 0:  # bug 要及时发现 and size(ma_values) == mal:
+        i = -1
+        for v in ma_values:
+            i += 1
+
+            if callable(v):
+                mas[i] = method_args[i]
+                continue
+
+            t = ma_types[i]
+
+            try:
+                json.dumps(v)
+            except Exception as e:
+                print(e)
+                v = str(v)
+
+            mas[i] = {
+                KEY_TYPE: t.__name__ if t is not None else type(v),
+                KEY_VALUE: v
+            }
+
+    return {
+        KEY_LANGUAGE: LANGUAGE,
+        KEY_OK: true,
+        KEY_CODE: CODE_SUCCESS,
+        KEY_MSG: MSG_SUCCESS,
+        KEY_TYPE: rt,
+        KEY_RETURN: result,
+        KEY_METHOD_ARGS: mas,
+        KEY_TIME_DETAIL: time_detail
+    }
+
+
+def invoke_method(req: any, callback: callable = null) -> dict:
     start_time = time.time_ns()
     try:
+        assert is_none(callback) or callable(callback)
+
         if is_str(req):
             req = parse_json(req)
 
         static = req.get(KEY_STATIC)
         assert is_bool(static), (KEY_STATIC + ' must be bool!')
 
+        is_async = req.get(KEY_ASYNC)
+        assert is_bool(is_async), (KEY_ASYNC + ' must be bool!')
+
         package = req.get(KEY_PACKAGE)
         assert is_str(package), (KEY_PACKAGE + ' must be str!')
 
         clazz = req.get(KEY_CLASS)
         assert is_str(clazz), (KEY_CLASS + ' must be str!')
 
         method = req.get(KEY_METHOD)
@@ -415,27 +506,37 @@
 
         instance = None
         if this is not None:
             assert not static, KEY_STATIC + ' cannot appear together with ' + KEY_THIS + '!'
             assert class_args is None, KEY_THIS + ' cannot appear together with ' + KEY_CLASS_ARGS + '!'
             assert constructor is None, KEY_THIS + ' cannot appear together with ' + KEY_CONSTRUCTOR + '!'
 
+            this_keys = [null]
             this_types = [null]
             this_values = [null]
-            init_args([this], this_types, this_values)
+            this_kwargs = {}
+            init_args([this], this_keys, this_types, this_values, this_kwargs)
             instance = this_values[0]
 
         if class_args is not None:
             assert not static, KEY_CLASS_ARGS + ' cannot appear together with ' + KEY_STATIC + '!'
             assert this is None, KEY_CLASS_ARGS + ' cannot appear together with ' + KEY_THIS + '!'
 
         mal = size(method_args)
+        ma_keys = [null] * mal
         ma_types = [null] * mal
         ma_values = [null] * mal
-        init_args(method_args, ma_types, ma_values)
+        m_kwargs = {}
+
+        final_result = {}
+        def final_callback(*args, **kwargs):
+            if not_none(callback):  # callable(callback):
+                callback(wrap_result(func, method_args, ma_types, ma_values, final_result.get(KEY_VALUE), start_time))
+
+        is_wait = init_args(method_args, ma_keys, ma_types, ma_values, m_kwargs, true, final_callback)
 
         fl = split(clazz, '$')
         l = size(fl)
 
         mn = package if l <= 0 else package + '.' + fl[0]
         module = __import__(mn, fromlist=['__init__'] if l <= 0 else fl[0])
 
@@ -453,115 +554,206 @@
         elif static:
             func = getattr(cls, method)
         else:
             constructor_func = None if constructor is None else getattr(module, constructor)
 
             if instance is None:
                 cal = size(class_args)
+                ca_keys = [null] * cal
                 ca_types = [null] * cal
                 ca_values = [null] * cal
-                init_args(class_args, ca_types, ca_values)
-                instance = cls(*ca_values) if constructor_func is None else constructor_func(*ca_values)
+                c_kwargs = {}
+                init_args(class_args, ca_keys, ca_types, ca_values, c_kwargs)
+                instance = cls(*ca_values, **c_kwargs) if constructor_func is None else constructor_func(*ca_values, **c_kwargs)
 
             func = getattr(instance, method)
 
+        ksl = size(m_kwargs)
         start_time = time.time_ns()
-        result = func(*ma_values)
-        time_detail = get_time_detail(start_time)
 
-        signature = inspect.signature(func)
-        return_annotation = null if signature is None else signature.return_annotation
-        rt = null
-        if return_annotation is not None:
-            try:
-                rt = return_annotation.__name__
-                if rt in ('_empty', 'POSITIONAL_OR_KEYWORD'):
-                    rt = type(result).__name__
-            except Exception as e:
-                print(e)
-                rt = type(result).__name__  # str(return_annotation)
+        result = asyncio.run(func(*ma_values[:mal-ksl], **m_kwargs)) if is_async \
+            else func(*ma_values[:mal-ksl], **m_kwargs)  # asyncio.run 只允许调 async 函数 is_async != false
 
-        mas = [null] * mal
-        if mal > 0:  # bug 要及时发现 and size(ma_values) == mal:
-            i = -1
-            for v in ma_values:
-                i += 1
-                t = ma_types[i]
-                mas[i] = {
-                    KEY_TYPE: t.__name__ if t is not None else type(v),
-                    KEY_VALUE: v
-                }
-
-        return {
-            KEY_LANGUAGE: LANGUAGE,
-            KEY_OK: true,
-            KEY_CODE: CODE_SUCCESS,
-            KEY_MSG: MSG_SUCCESS,
-            KEY_TYPE: rt,
-            KEY_RETURN: result,
-            KEY_METHOD_ARGS: mas,
-            KEY_TIME_DETAIL: time_detail
-        }
+        final_result[KEY_VALUE] = result
+        return wrap_result(func, method_args, ma_types, ma_values, result, start_time)
     except Exception as e:
         return {
             KEY_LANGUAGE: LANGUAGE,
             KEY_OK: false,
             KEY_CODE: CODE_SERVER_ERROR,
             KEY_MSG: str(e),
             KEY_TIME_DETAIL: get_time_detail(start_time),
             KEY_THROW: e.__class__.__name__,
             # KEY_TRACE: e.__traceback__.__str__()
         }
 
 
-def init_args(method_args, ma_types, ma_values):
+def init_args(
+    method_args: list, ma_keys: list, ma_types: list, ma_values: list,
+    ma_kwargs: dict, keep_kwargs_in_types_and_values: bool = false, callback: callable = null
+):
+    is_wait = false
     mal = size(method_args)
     if mal > 0:
         i = -1
         for arg in method_args:
             i += 1
             value = null
-            if is_str(arg) and arg.__contains__(':'):
-                ind = arg.index(':')
+            is_fun = false
+
+            if is_str(arg) and (arg.__contains__(':') or arg.__contains__('=')):
+                ind = index(arg, ':')
+                eq_ind = index(arg, '=')
+                key = (arg[:eq_ind] if ind < 0 else arg[ind+1:eq_ind]) if eq_ind >= 0 else null
                 typ = arg[:ind] if ind >= 0 else null
                 # ma_types.append(arg[:ind] if ind >= 0 else 'str')
-                value = arg[ind+1:] if ind >= 0 else arg
+                value = arg[eq_ind+1:] if eq_ind >= 0 else (arg[ind+1:] if ind >= 0 else arg)
                 # ma_values.append(arg[ind + 1:] if ind >= 0 else arg)
             else:
                 id = is_dict(arg)
+                key = arg.get(KEY_KEY) if id else null
                 typ = arg.get(KEY_TYPE) if id else null
                 # ma_types.append(arg.get(KEY_TYPE) if id else type(arg))
                 value = arg.get(KEY_VALUE) if id else arg
                 # ma_values.append(arg.get(KEY_VALUE) if id else arg)
 
-            clazz = get_class(typ, value)
+                start = index(typ, '(')
+                end = last_index(typ, ')')
+                if start >= 0 and end > start:  # 命名函数 或 lambda 匿名函数
+                    assert is_dict(value, true), '{"type": "def(arg0,arg1...)", "value": value} 中 value 类型错误，' \
+                        '必须为 dict！且格式必须为 {"type": returnType, "return": returnValue, "callback": bool}'
+                    cb = value.get(KEY_CALLBACK)
+                    assert is_bool(cb, false), '{"type": "def(arg0,arg1...)", "value": {"callback": bool}} 中' \
+                        ' value/callback 类型错误，必须为 true 或 false ！'
+
+                    is_fun = true
+                    is_wait = is_wait or cb
+
+                    fun = typ[:start] if start > 0 else null
+                    # assert is_none(fun) or is_name(fun), '{"type": "fun(arg0,arg1...)"} 必须是函数名，或者关键词 def '
+                    assert fun == 'def', '{"type": "fun(arg0,arg1...)"} 必须是函数名，或者关键词 def '
+
+                    aks = split(typ[start+1:end])
+                    akl = size(aks)
+                    fa_types = [null] * akl
+                    fa_keys = [null] * akl
+                    for j in range(akl):
+                        ak = aks[j]
+                        ak_ind = index(ak, ':')
+                        fa_types[j] = null if ak_ind < 0 else ak[:ak_ind]
+                        fa_keys[j] = ak if ak_ind < 0 else ak[ak_ind+1:]
+
+                    rtn_type = value.get(KEY_TYPE)
+                    rtn_val = value.get(KEY_RETURN)
+
+                    raw_val: dict = value
+                    def cb_fun(*args, **kwargs):
+                        mas: list = []
+                        if not_empty(args):
+                            for arg in args:
+                                mas.append({
+                                    KEY_TYPE: type(arg).__name__,
+                                    KEY_VALUE: arg
+                                })
+
+                        if not_empty(kwargs):
+                            for k in kwargs:
+                                v = kwargs[k]
+                                mas.append({
+                                    KEY_KEY: k,
+                                    KEY_TYPE: type(v).__name__,
+                                    KEY_VALUE: v
+                                })
+
+                        call_list: list = raw_val.get(KEY_CALL_LIST) or []
+                        call_list.append({
+                            KEY_TIME: cur_time_in_millis(),
+                            KEY_METHOD_ARGS: mas
+                        })
+                        raw_val[KEY_CALL_LIST] = call_list
+
+                        if cb:
+                            callback(*args, **kwargs)
+
+                        rv = rtn_val
+                        if is_str(rv, true):
+                            try:
+                                fn = '__unitauto_return_' + str(i) + '__'
+                                to_eval = 'def ' + fn + '('
+                                k = 0
+                                first = true
+                                for ak in fa_keys:
+                                    if ak in kwargs:
+                                        arg = kwargs.get(ak)
+                                    else:
+                                        arg = args[k]
+                                        k += 1
+                                    to_eval += ('' if first else ', ') + ak + '=' + str(arg)
+                                    first = false
+                                    # to_eval += ak + ' = ' + str(arg) + ';'
+                                    # exec(ak + ' = ' + str(arg))
+                                to_eval += '):\n    return ' + rv
+                                exec(to_eval)
+                                # to_eval += rv
+                                nrv = eval(fn + '()')  # eval(rv)  # eval(to_eval)  # exec(to_eval)
+                                return cast(nrv, get_class(rtn_type, nrv))
+                            except Exception as e:
+                                print(e)
+
+                        return cast(rv, get_class(rtn_type, rv))
+
+                    value = cb_fun  # eval('lambda ' + ', '.join(fa_keys) + ': ' + str(rtn_val))
+
+            clazz = type(value) if is_fun else get_class(typ, value)
+            value = cast(value, clazz) if not is_fun else value
+
+            ma_keys[i] = key
+            if is_none(key):
+                if is_empty(ma_kwargs):
+                    ma_types[i] = clazz
+                    ma_values[i] = value
+                    continue
+                raise Exception('所有已经有 key 的参数，必须后面也跟着有 key，对应调用 fun(key=value, key2=value2...) ！')
 
-            if value is not None and not isinstance(value, clazz):
-                s = ''
-                try:
-                    s = value if is_str(value) else json.dumps(value)
-                    if PRIMITIVE_CLASS_MAP.__contains__(clazz.__name__):
-                        value = eval(clazz.__name__ + '(' + s + ')')
-                    else:
-                        value = json.loads(s, cls=clazz)  # FIXME 目前仅支持继承 JSONDecoder 且重写了 decode 方法的类
-                except Exception as e:
-                    print(e)
-                    if is_str(value):
-                        value = json.loads(value)
+            assert key not in ma_kwargs, '调函数传参，所有 key 不允许重名！必须有唯一的不同名称！'
+            ma_kwargs[key] = value
+
+            if keep_kwargs_in_types_and_values:
+                ma_types[i] = clazz
+                ma_values[i] = value
+            else:
+                del ma_types[-1]
+                del ma_values[-1]
+
+    return is_wait
 
-                    if not isinstance(value, clazz):
-                        if is_list(value):
-                            value = clazz(*value)
-                        elif is_dict(value):
-                            value = clazz(**value)  # FIXME 目前仅支持继承 __init__ 传完整参数且顺序一致的类
-                        else:
-                            pass
 
-            ma_types[i] = clazz
-            ma_values[i] = value
+def cast(value, clazz):
+    if value is not None and not isinstance(value, clazz):
+        s = ''
+        try:
+            s = value if is_str(value) else json.dumps(value)
+            if PRIMITIVE_CLASS_MAP.__contains__(clazz.__name__):
+                value = eval(clazz.__name__ + '(' + s + ')')
+            else:
+                value = json.loads(s, cls=clazz)  # FIXME 目前仅支持继承 JSONDecoder 且重写了 decode 方法的类
+        except Exception as e:
+            print(e)
+            if is_str(value):
+                value = json.loads(value)
+
+            if not isinstance(value, clazz):
+                if is_list(value):
+                    value = clazz(*value)
+                elif is_dict(value):
+                    value = clazz(**value)  # FIXME 目前仅支持继承 __init__ 传完整参数且顺序一致的类
+                else:
+                    pass
+
+    return value
 
 
 def get_class(typ: str, value: any = None) -> Type:
     fl = split(typ, '$')
     if is_empty(fl):
         return type(value)
 
@@ -626,27 +818,40 @@
     return (not strict) if obj is None else isinstance(obj, list)
 
 
 def is_dict(obj, strict: bool = false) -> bool:
     return (not strict) if obj is None else isinstance(obj, dict)
 
 
+def not_none(obj):
+    return not is_none(obj)
+
+
+def is_none(obj):
+    return obj is None
+
+
 def not_empty(obj) -> bool:
     return not is_empty(obj)
 
 
 def is_empty(obj) -> bool:
     if obj is None:
         return true
     if is_int(obj) or is_float(obj):
         return obj <= 0
 
     return size(obj) <= 0
 
 
+def is_name(s: str) -> bool:
+    m = null if is_empty(s) else PATTERN_NUMBER.match(s[:1])
+    return is_none(m) and not_none(PATTERN_NAME.match(s))
+
+
 def size(obj) -> int:
     if obj is None:
         return 0
 
     if is_bool(obj) or is_int(obj) or is_float(obj):
         raise Exception('obj cannot be any one of [bool, int, float]!')
 
@@ -656,19 +861,30 @@
 def index(s: str, sub: str) -> int:
     try:
         return s.index(sub)
     except Exception:
         return -1
 
 
+def last_index(s: str, sub: str) -> int:
+    ws = split(s, sub)
+    if size(ws) <= 1:
+        return -1
+    return size(s) - size(ws[-1]) - 1
+
+
+def cur_time_in_millis() -> int:
+    return round(time.time_ns()/MILLIS_TIME)
+
+
 def get_time_detail(start_time: int, end_time: int = 0):
     if end_time is None or end_time <= 0:
         end_time = time.time_ns()
     duration = end_time - start_time
-    return str(round(start_time/1000)) + '|' + str(round(duration/1000)) + '|' + str(round(end_time/1000))
+    return str(round(start_time/MILLIS_TIME)) + '|' + str(round(duration/MILLIS_TIME)) + '|' + str(round(end_time/MILLIS_TIME))
 
 
 def parse_json(s: str):
     return json.loads(s)
 
 
 def to_json_str(obj, indent: int = 2) -> str:
```

### Comparing `unitauto-0.9.3/unitauto/server.py` & `unitauto-1.0.0/unitauto/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import json
 from unitauto import methodutil
 from unitauto.methodutil import null, true, false, to_json_str, list_method, invoke_method, KEY_PACKAGE, KEY_CLASS, \
-    KEY_CONSTRUCTOR, KEY_CLASS_ARGS, KEY_THIS, KEY_METHOD, KEY_METHOD_ARGS, KEY_TYPE, KEY_VALUE
+    KEY_CONSTRUCTOR, KEY_CLASS_ARGS, KEY_THIS, KEY_METHOD, KEY_METHOD_ARGS, KEY_TYPE, KEY_VALUE, KEY_RETURN, KEY_KEY, \
+    KEY_ASYNC, KEY_CALLBACK
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 
 
 CHARSET = 'uft-8'
 HOST = ('localhost', 8083)
 
@@ -69,35 +70,37 @@
         if method == 'OPTIONS':
             # self.wfile.write('ok'.encode())
             return
 
         bs = self.rfile.read(int(self.headers[KEY_CONTENT_LENGTH]))
         req = bs.decode()  # bs.decode(CHARSET)
         # req = urllib.unquote(bs).decode(CHARSET, 'ignore')
+
+        def callback(rsp):
+            rsp_str = to_json_str(rsp)
+            self.wfile.write(rsp_str.encode())
         if path == '/method/list':
             rsp = list_method(req)
+            callback(rsp)
         else:
-            rsp = invoke_method(req)
-
-        rsp_str = to_json_str(rsp)
-        self.wfile.write(rsp_str.encode())
+            invoke_method(req, callback)
 
 
 def start(host=HOST):
     server = HTTPServer(host, Request)
     print("Starting server, listen at: %s:%s" % host)
     server.serve_forever()
 
 
 def test():
     rsp0 = invoke_method({
         KEY_PACKAGE: 'unitauto.test',
         KEY_METHOD: 'test'
     })
-    print('unitauto.test.test() = \n' + to_json_str(rsp0))
+    print('\nunitauto.test.test() = \n' + to_json_str(rsp0))
 
     rsp1 = invoke_method({
         KEY_PACKAGE: 'unitauto.test',
         KEY_CLASS: 'testutil',
         KEY_METHOD: 'minus',
         KEY_METHOD_ARGS: [
             {
@@ -106,54 +109,103 @@
             },
             {
                 KEY_TYPE: 'int',
                 KEY_VALUE: 3
             }
         ]
     })
-    print('unitauto.test.testutil.minus(2, 3) = \n' + to_json_str(rsp1))
+    print('\nunitauto.test.testutil.minus(2, 3) = \n' + to_json_str(rsp1))
 
     rsp2 = invoke_method({
         KEY_PACKAGE: 'unitauto.test',
         KEY_CLASS: 'testutil$Test',
         KEY_CLASS_ARGS: [
             1,
             0,
             'UnitAuto'
         ],
         KEY_METHOD: 'get_id'
     })
-    print('unitauto.test.testutil.Test.get_id() = \n' + to_json_str(rsp2))
+    print('\nunitauto.test.testutil.Test.get_id() = \n' + to_json_str(rsp2))
 
     rsp3 = invoke_method({
         KEY_PACKAGE: 'unitauto.test',
         KEY_CLASS: 'testutil$Test',
         KEY_CONSTRUCTOR: 'get_test_instance',
         KEY_CLASS_ARGS: [
             2,
             1,
             'UnitAuto@Python'
         ],
         KEY_METHOD: 'get_name'
     })
-    print('unitauto.test.testutil.Test.get_name() = \n' + to_json_str(rsp3))
+    print('\nunitauto.test.testutil.Test.get_name() = \n' + to_json_str(rsp3))
 
     rsp4 = invoke_method({
         KEY_PACKAGE: 'unitauto.test',
         KEY_CLASS: 'testutil$Test',
         KEY_THIS: {
             KEY_TYPE: 'unitauto.test.testutil$Test',
             KEY_VALUE: {
                 'id': 3,
                 'sex': 1,
                 'name': 'UnitAuto'
             }
         },
         KEY_METHOD: 'get_sex_str'
     })
-    print('unitauto.test.testutil.Test.get_sex_str() = \n' + to_json_str(rsp4))
+    print('\nunitauto.test.testutil.Test.get_sex_str() = \n' + to_json_str(rsp4))
+
+    rsp5 = invoke_method({
+        KEY_ASYNC: true,
+        KEY_PACKAGE: 'unitauto.test',
+        KEY_CLASS: 'testutil',
+        KEY_METHOD: 'async_test',
+        KEY_METHOD_ARGS: [
+            {
+                KEY_TYPE: 'int',
+                KEY_VALUE: 2
+            },
+            {
+                KEY_TYPE: 'int',
+                KEY_VALUE: 5
+            }
+        ]
+    })
+    print('\nunitauto.test.testutil.async_test(2, 5) = \n' + to_json_str(rsp5))
+
+    def callback(rsp):
+        print('unitauto.test.testutil.compute_async(2, 5, callback) = \n' + to_json_str(rsp))
+
+    rsp6 = invoke_method({
+        KEY_PACKAGE: 'unitauto.test',
+        KEY_CLASS: 'testutil',
+        KEY_METHOD: 'compute_async',
+        KEY_METHOD_ARGS: [
+            {
+                # KEY_KEY: 'a',
+                KEY_TYPE: 'int',
+                KEY_VALUE: 2
+            },
+            {
+                # KEY_KEY: 'b',
+                KEY_TYPE: 'int',
+                KEY_VALUE: 5
+            },
+            {
+                KEY_KEY: 'callback',
+                KEY_TYPE: 'def(a,b,c)',
+                KEY_VALUE: {
+                    KEY_TYPE: 'int',
+                    KEY_RETURN: 'a - b',
+                    KEY_CALLBACK: true
+                }
+            }
+        ]
+    }, callback)
+    print('\nunitauto.test.testutil.compute_async(2, 5, callback) = \n' + to_json_str(rsp6))
 
 
 if __name__ == '__main__':
     test()
     start()
```

### Comparing `unitauto-0.9.3/unitauto/test/__init__.py` & `unitauto-1.0.0/unitauto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.3/unitauto/test/testutil.py` & `unitauto-1.0.0/unitauto/test/testutil.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import asyncio
 import json
+import threading
+import time
 from json import JSONDecoder
 from typing import Callable, Any
 
 
 def test():
     return 'UnitAuto@Python'
 
@@ -53,14 +56,37 @@
     return a * b
 
 
 def divide(a: float, b: float):
     return a / b
 
 
+async def async_test(a, b):
+    print('start >>> ')
+    await asyncio.sleep(3)
+    print('end <<<')
+    return a + b
+
+
+def compute_async(a, b, callback):
+    print('start >>> ')
+
+    def fun():
+        time.sleep(3)
+        print('callback >>> ')
+        ret = callback(a, b, a + b)
+        print('ret = ' + str(ret))
+
+    thd = threading.Thread(target=fun)
+    thd.start()
+
+    print('return <<<')
+    return True
+
+
 class Test(JSONDecoder):
     id: int
     sex: int
     name: str
 
     def __init__(self, id: int = 0, sex: int = 0, name: str = ''):
         super().__init__()
```

### Comparing `unitauto-0.9.3/unitauto.egg-info/PKG-INFO` & `unitauto-1.0.0/unitauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.9.3
+Version: 1.0.0
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

