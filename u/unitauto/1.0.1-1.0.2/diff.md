# Comparing `tmp/unitauto-1.0.1.tar.gz` & `tmp/unitauto-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-1rivqg0l/unitauto-1.0.1.tar", last modified: Mon Jul 17 15:31:39 2023, max compression
+gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-sf2gyurg/unitauto-1.0.2.tar", last modified: Mon Jul 17 16:30:30 2023, max compression
```

## Comparing `unitauto-1.0.1.tar` & `unitauto-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 15:31:21.000000 unitauto-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 15:31:39.000000 unitauto-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 15:31:21.000000 unitauto-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 15:31:21.000000 unitauto-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 15:31:39.000000 unitauto-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/methodutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-17 15:31:21.000000 unitauto-1.0.1/unitauto/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 15:31:39.000000 unitauto-1.0.1/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:30:30.000000 unitauto-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 16:30:13.000000 unitauto-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-17 16:30:30.000000 unitauto-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-17 16:30:13.000000 unitauto-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 16:30:13.000000 unitauto-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 16:30:30.000000 unitauto-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 16:30:13.000000 unitauto-1.0.2/unitauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30829 2023-07-17 16:30:13.000000 unitauto-1.0.2/unitauto/methodutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-17 16:30:13.000000 unitauto-1.0.2/unitauto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 16:30:13.000000 unitauto-1.0.2/unitauto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-17 16:30:13.000000 unitauto-1.0.2/unitauto/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 16:30:30.000000 unitauto-1.0.2/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-1.0.1/LICENSE` & `unitauto-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.1/setup.cfg` & `unitauto-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 1.0.1
+version = 1.0.2
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-1.0.1/unitauto/methodutil.py` & `unitauto-1.0.2/unitauto/methodutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         'parameterTypeList': types if static else types[1:],
         'genericParameterTypeList': types if static else types[1:],
         'parameterNameList': names if static else names[1:],
         'parameterDefaultValueList': null
     }
 
 
-def wrap_result(func, method_args, ma_types, ma_values, result, start_time):
+def wrap_result(instance, func, method_args, ma_types, ma_values, result, start_time):
     time_detail = get_time_detail(start_time)
 
     signature = inspect.signature(func)
     return_annotation = null if signature is None else signature.return_annotation
     rt = null
     if return_annotation is not None:
         try:
@@ -452,22 +452,56 @@
                 v = str(v)
 
             mas[i] = {
                 KEY_TYPE: t.__name__ if t is not None else type(v),
                 KEY_VALUE: v
             }
 
+    if is_none(instance):
+        return {
+            KEY_LANGUAGE: LANGUAGE,
+            KEY_OK: true,
+            KEY_CODE: CODE_SUCCESS,
+            KEY_MSG: MSG_SUCCESS,
+            KEY_TYPE: rt,
+            KEY_RETURN: result,
+            KEY_METHOD_ARGS: mas,
+            KEY_TIME_DETAIL: time_detail
+        }
+
+    cls = type(instance)
+    this = {
+        KEY_TYPE: cls.__name__,
+    }
+
+    try:
+        json.dumps(instance)
+        this[KEY_VALUE] = instance
+    except Exception as e:
+        print(e)
+        try:
+            this[KEY_VALUE] = json.loads(json.dumps(instance, cls=cls))
+        except Exception as e2:
+            print(e2)
+            try:
+                this[KEY_VALUE] = json.loads(instance.encode(null))
+            except Exception as e3:
+                print(e3)  # FIXME instance.__dict__ , dir(instance)
+                this[KEY_VALUE] = str(instance)
+                this[KEY_WARN] = str(e)
+
     return {
         KEY_LANGUAGE: LANGUAGE,
         KEY_OK: true,
         KEY_CODE: CODE_SUCCESS,
         KEY_MSG: MSG_SUCCESS,
         KEY_TYPE: rt,
         KEY_RETURN: result,
         KEY_METHOD_ARGS: mas,
+        KEY_THIS: this,
         KEY_TIME_DETAIL: time_detail
     }
 
 
 def invoke_method(req: any, callback: callable = null) -> dict:
     start_time = time.time_ns()
     is_wait = false
@@ -527,15 +561,15 @@
         ma_types = [null] * mal
         ma_values = [null] * mal
         m_kwargs = {}
 
         final_result = {}
         def final_callback(*args, **kwargs):
             if not_none(callback):  # callable(callback):
-                callback(wrap_result(func, method_args, ma_types, ma_values, final_result.get(KEY_VALUE), start_time))
+                callback(wrap_result(final_result.get(KEY_THIS), func, method_args, ma_types, ma_values, final_result.get(KEY_VALUE), start_time))
 
         is_wait = init_args(method_args, ma_keys, ma_types, ma_values, m_kwargs, true, final_callback)
 
         fl = split(clazz, '$')
         l = size(fl)
 
         mn = package if l <= 0 else package + '.' + fl[0]
@@ -564,23 +598,24 @@
                 ca_values = [null] * cal
                 c_kwargs = {}
                 init_args(class_args, ca_keys, ca_types, ca_values, c_kwargs)
                 instance = cls(*ca_values, **c_kwargs) if constructor_func is None else constructor_func(*ca_values, **c_kwargs)
 
             func = getattr(instance, method)
 
+        final_result[KEY_THIS] = instance
         ksl = size(m_kwargs)
         start_time = cur_time_in_millis()
 
         # TODO 自动识别 async 关键词
         result = asyncio.run(func(*ma_values[:mal-ksl], **m_kwargs)) if is_async \
             else func(*ma_values[:mal-ksl], **m_kwargs)  # asyncio.run 只允许调 async 函数 is_async != false
 
         final_result[KEY_VALUE] = result
-        res = wrap_result(func, method_args, ma_types, ma_values, result, start_time)
+        res = wrap_result(instance, func, method_args, ma_types, ma_values, result, start_time)
     except Exception as e:
         res = {
             KEY_LANGUAGE: LANGUAGE,
             KEY_OK: false,
             KEY_CODE: CODE_SERVER_ERROR,
             KEY_MSG: str(e),
             KEY_TIME_DETAIL: get_time_detail(start_time),
```

### Comparing `unitauto-1.0.1/unitauto/server.py` & `unitauto-1.0.2/unitauto/server.py`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.1/unitauto/test/__init__.py` & `unitauto-1.0.2/unitauto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.1/unitauto/test/testutil.py` & `unitauto-1.0.2/unitauto/test/testutil.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import asyncio
 import json
 import threading
 import time
-from json import JSONDecoder
+from json import JSONDecoder, JSONEncoder
 from typing import Callable, Any
 
 
 def test():
     return 'UnitAuto@Python'
 
 
@@ -94,23 +94,39 @@
         self.sex = sex
         self.name = name
 
     def decode(self, s: str, _w: Callable[..., Any] = ...) -> Any:
         args = json.loads(s)
         return Test(**args)
 
+    def encode(self, o: Any) -> str:
+        return json.dumps({
+            'id': self.id,
+            'sex': self.sex,
+            'name': self.name
+        })
+
     def get_id(self) -> int:
         return self.id
 
+    def set_id(self, id: int):
+        self.id = id
+
     def get_sex(self) -> int:
         return self.sex
 
+    def set_sex(self, sex: int):
+        self.sex = sex
+
     def get_name(self) -> str:
         return self.name
 
+    def set_name(self, name: str):
+        self.name = name
+
     def is_male(self) -> bool:
         return self.sex is None or self.sex == 0
 
     def is_female(self) -> bool:
         return not self.is_male()
 
     def get_sex_str(self) -> str:
```

