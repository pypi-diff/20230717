# Comparing `tmp/IngeoDash-0.0.22.tar.gz` & `tmp/IngeoDash-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.0.22.tar", last modified: Mon Jul 17 13:44:11 2023, max compression
+gzip compressed data, was "IngeoDash-0.0.23.tar", last modified: Mon Jul 17 18:35:55 2023, max compression
```

## Comparing `IngeoDash-0.0.22.tar` & `IngeoDash-0.0.23.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.739664 IngeoDash-0.0.22/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:35:55.558448 IngeoDash-0.0.23/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:35:55.558448 IngeoDash-0.0.23/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:35:55.558448 IngeoDash-0.0.23/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:35:55.558448 IngeoDash-0.0.23/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 18:35:55.000000 IngeoDash-0.0.23/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 18:35:55.000000 IngeoDash-0.0.23/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:35:55.000000 IngeoDash-0.0.23/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 18:35:55.000000 IngeoDash-0.0.23/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 18:35:55.000000 IngeoDash-0.0.23/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 18:35:55.558448 IngeoDash-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:35:55.558448 IngeoDash-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-17 18:33:58.000000 IngeoDash-0.0.23/setup.py
```

### Comparing `IngeoDash-0.0.22/IngeoDash/__init__.py` & `IngeoDash-0.0.23/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.0.22'
+__version__ = '0.0.23'
```

### Comparing `IngeoDash-0.0.22/IngeoDash/__main__.py` & `IngeoDash-0.0.23/IngeoDash/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -75,30 +75,41 @@
 
 @callback(
     Output(CONFIG.store, 'data', allow_duplicate=True),
     Input(CONFIG.upload, 'contents'),
     State(CONFIG.lang, 'value'),
     State(CONFIG.text, 'value'),
     State(CONFIG.label_header, 'value'),
+    State(CONFIG.batch_size, 'value'),
     State(CONFIG.store, 'data'),
     prevent_initial_call=True
 )
-def upload_callback(content, lang, text, label, mem):
+def upload_callback(content, lang, 
+                    text, label, n_value,
+                    mem):
     mem = CONFIG(mem)
     return upload(mem, content, lang=lang,
-                  text=text, label=label)
+                  text=text, label=label,
+                  n_value=n_value)
 
 
-def run():
+def test_component(component):
+    app = Dash(external_stylesheets=[dbc.themes.BOOTSTRAP],
+               suppress_callback_exceptions=True)
+    app.layout = dbc.Container([dbc.Row(component)])
+    app.run_server(debug=True)
+
+
+def run(debug=True, **kwargs):
     app = Dash(external_stylesheets=[dbc.themes.BOOTSTRAP],
                suppress_callback_exceptions=True)
 
     app.layout = dbc.Container([dcc.Loading(children=dcc.Store(CONFIG.store),
                                             fullscreen=True),
                                 dbc.Row(table_component()),
                                 dbc.Row(download_component()),
                                 dbc.Row(upload_component())])
-    app.run_server(debug=True)
+    app.run_server(debug=debug)
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `IngeoDash-0.0.22/IngeoDash/annotate.py` & `IngeoDash-0.0.23/IngeoDash/annotate.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     index = (labels.index(label) + 1) % len(labels)
     data[k][mem.label_header] = labels[index]
     return data[k]
 
 
 def store(mem: Config):
     db = CONFIG.db[mem[mem.username]]
-    data = db.pop(mem.data)
+    data = db.pop(mem.data) if mem.data in db else []
     try:
         permanent = db[mem.permanent]
     except KeyError:
         permanent = []
     permanent.extend(data)        
     db[mem.permanent] = permanent
```

### Comparing `IngeoDash-0.0.22/IngeoDash/app.py` & `IngeoDash-0.0.23/IngeoDash/app.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.22/IngeoDash/config.py` & `IngeoDash-0.0.23/IngeoDash/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     n_jobs: int = 1
     denseBoW: dict = field(default_factory=dict)
     db: dict = field(default_factory=dict)
     username: str = 'username'
     text: str = 'text'
     mem: dict = field(default_factory=dict)
     prev: str='previous'
+    batch_size: str='n_value'
 
     def __getitem__(self, key):
         return self.mem[key]
     
     def __setitem__(self, key, value):
         self.mem[key] = value
```

### Comparing `IngeoDash-0.0.22/IngeoDash/download.py` & `IngeoDash-0.0.23/IngeoDash/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,13 @@
                            dbc.InputGroupText('Filename:'),
                            dbc.Input(placeholder='output.json',
                                      value='output.json',
                                      type='text',
                                      id=CONFIG.filename),
                            dbc.Button('Download',
                                       color='success',
-                                      id=CONFIG.save)])    
+                                      id=CONFIG.save)])
+
+
+if __name__ == '__main__':
+    from IngeoDash.__main__ import test_component
+    test_component(download_component())
```

### Comparing `IngeoDash-0.0.22/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.0.23/IngeoDash/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.22/IngeoDash/tests/test_app.py` & `IngeoDash-0.0.23/IngeoDash/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.22/IngeoDash/tests/test_config.py` & `IngeoDash-0.0.23/IngeoDash/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,16 @@
                    lang='lang',
                    n_jobs=1,
                    denseBoW={},
                    db={},
                    username='username',
                    text='text',
                    mem={},
-                   prev='previous')
+                   prev='previous',
+                   batch_size='n_value')
     for k, v in default.items():
         assert v == getattr(conf, k)
 
 
 def test_Config_mem():
     config = Config()
```

### Comparing `IngeoDash-0.0.22/IngeoDash/tests/test_download.py` & `IngeoDash-0.0.23/IngeoDash/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.22/IngeoDash/tests/test_upload.py` & `IngeoDash-0.0.23/IngeoDash/tests/test_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,23 +45,26 @@
 
 
 def test_upload_unique():
     mem = CONFIG({CONFIG.username: 'xxx'})
     D = list(tweet_iterator(TWEETS))
     for x in D:
         x['class'] = 1
-    CONFIG.db['xxx'] = {mem.data: D, mem.permanent: []}
+    CONFIG.db['xxx'] = {}
     _ = [json.dumps(x) for x in D[:15]]
     content_str = str(base64.b64encode(bytes('\n'.join(_),
                                        encoding='utf-8')),
                       encoding='utf-8')
     content = f'NA,{content_str}'
-    _ = upload(mem, content, lang='es', label='class')
+    _ = upload(mem, content, lang='es',
+               label='class', n_value=3)
     db = CONFIG.db['xxx']
     assert len(db[mem.permanent]) == 0
+    assert len(db[mem.data]) + len(db[mem.original]) == 15
+    assert len(db[mem.data]) == 3
 
 
 def test_upload_labels():
     mem = CONFIG({CONFIG.username: 'xxx'})
     D = list(tweet_iterator(TWEETS))
     _ = [json.dumps(x) for x in D]
     content_str = str(base64.b64encode(bytes('\n'.join(_),
@@ -77,8 +80,8 @@
     assert mem[mem.labels] == klasses.tolist()
 
 
 
 def test_upload_component():
     import dash_bootstrap_components as dbc
     component = upload_component()
-    assert isinstance(component, dbc.InputGroup)
+    assert isinstance(component, dbc.Col)
```

### Comparing `IngeoDash-0.0.22/IngeoDash/upload.py` & `IngeoDash-0.0.23/IngeoDash/upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,74 +8,93 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.config import CONFIG, Config
-from IngeoDash.app import user, label_column
+from IngeoDash.app import user, table_next
 from EvoMSA.utils import MODEL_LANG
-from dash import dcc
+from dash import dcc, html
 import numpy as np
 import dash_bootstrap_components as dbc
 import base64
 import io
 import json
 
 
 def read_json(mem: Config, data):
     _ = io.StringIO(data.decode('utf-8'))
     return [json.loads(x) for x in _]
 
 
 def upload(mem: Config, content, lang='es', 
-           type='json', text='text', label='klass',
-           call_next=label_column):
+           type='json', text='text', 
+           label='klass', n_value=CONFIG.n_value,
+           call_next=table_next):
     def _label(x):
         if mem.label_header in x:
             ele = x[mem.label_header]
             if ele is not None and len(f'{ele}'):
                 return True
         return False
-    mem.mem.update(dict(label_header=label, text=text))
+    mem.mem.update(dict(label_header=label, text=text, n_value=n_value))
     mem.label_header = label
     mem.text = text
+    mem.n_value = n_value
     content_type, content_string = content.split(',')
     decoded = base64.b64decode(content_string)
     data = globals()[f'read_{type}'](mem, decoded)
     username, db = user(mem)
     labels = np.unique([x[mem.label_header]
                         for x in data if _label(x)])
     permanent = db.get(mem.permanent, list())    
     if labels.shape[0] > 1:
         original = [x for x in data if not _label(x)]
         permanent.extend([x for x in data if _label(x)])
     else:
         original = data
-    db[mem.data] = original[:mem.n_value]
     db[mem.permanent] = permanent
-    db[mem.original] = original[mem.n_value:]
+    db[mem.original] = original
     mem.mem.update({mem.lang: lang,
                     mem.size: len(data),
                     mem.username: username})
     if call_next is not None:
         call_next(mem)
     return json.dumps(mem.mem)
 
 
 def upload_component():
-    lang = dbc.Select(id=CONFIG.lang, value='es',
-                      options=[dict(label=x, value=x) for x in MODEL_LANG])
-    upload = dbc.InputGroup([dbc.InputGroupText('Language:'),
-                             lang, 
-                             dbc.InputGroupText('Text Column:'),
-                             dcc.Input(id=CONFIG.text,
-                                       value='text',
-                                       type='text'),
-                             dbc.InputGroupText('Text Label:'),
-                             dcc.Input(id=CONFIG.label_header,
-                                       value='klass',
-                                       type='text'),
-                             dcc.Upload(id=CONFIG.upload, 
-                                        children=dbc.Button('Upload'))])
-    return upload
-
+    langs = {'ar': 'Arabic', 'ca': 'Catalan', 'de': 'German', 'en': 'English',
+             'es': 'Spanish', 'fr': 'French', 'hi': 'Hindi', 'in': 'Indonesian',
+             'it': 'Italian', 'ja': 'Japanese', 'ko': 'Korean', 'nl': 'Dutch',
+             'pl': 'Polish', 'pt': 'Portuguese', 'ru': 'Russian', 'tl': 'Tagalog',
+             'tr': 'Turkish', 'zh': 'Chinese'}
+    
+    lang_grp = dbc.InputGroup([dbc.InputGroupText('Language:'),
+                               dbc.Select(id=CONFIG.lang, value='es',
+                                          options=[dict(label=langs.get(x, x),
+                                                        value=x)
+                                                   for x in MODEL_LANG])])
+
+    data_grp = dbc.InputGroup([dbc.InputGroupText('Text Column:'),
+                               dcc.Input(id=CONFIG.text,
+                                         value='text',
+                                         type='text'),
+                               dbc.InputGroupText('Text Label:'),
+                               dcc.Input(id=CONFIG.label_header,
+                                         value='klass',
+                                         type='text'),
+                               dbc.InputGroupText('Batch Size:'),
+                               dcc.Input(id=CONFIG.batch_size,
+                                         value=10,
+                                         type='number')]) 
+                            #    dcc.Upload(id=CONFIG.upload,
+                            #               children=dbc.Button('Upload'))])
+    upload_button = dbc.Button(dcc.Upload(id=CONFIG.upload,
+                                          children=html.Div('Drop or Select File')))
+    return dbc.Col(dbc.Stack([lang_grp, data_grp, upload_button]))
+
+
+if __name__ == '__main__':
+    from IngeoDash.__main__ import test_component
+    test_component(upload_component())
```

### Comparing `IngeoDash-0.0.22/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.0.23/IngeoDash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.22
+Version: 0.0.23
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.0.22/LICENSE` & `IngeoDash-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.22/PKG-INFO` & `IngeoDash-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.22
+Version: 0.0.23
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.0.22/README.rst` & `IngeoDash-0.0.23/README.rst`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.22/setup.py` & `IngeoDash-0.0.23/setup.py`

 * *Files identical despite different names*

