# Comparing `tmp/lightweight_charts-1.0.8.tar.gz` & `tmp/lightweight_charts-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.8.tar", last modified: Tue May 23 13:32:25 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.9.tar", last modified: Mon May 29 20:33:37 2023, max compression
```

## Comparing `lightweight_charts-1.0.8.tar` & `lightweight_charts-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-23 13:32:25.440313 lightweight_charts-1.0.8/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.8/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-23 13:32:25.440021 lightweight_charts-1.0.8/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     5856 2023-05-20 15:23:42.000000 lightweight_charts-1.0.8/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-23 13:32:25.437186 lightweight_charts-1.0.8/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.8/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     3110 2023-05-23 13:04:15.000000 lightweight_charts-1.0.8/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    28575 2023-05-23 13:10:38.000000 lightweight_charts-1.0.8/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   148472 2023-05-20 23:46:07.000000 lightweight_charts-1.0.8/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     2083 2023-05-21 12:37:38.000000 lightweight_charts-1.0.8/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)     1932 2023-05-20 19:56:58.000000 lightweight_charts-1.0.8/lightweight_charts/widgets.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-23 13:32:25.439527 lightweight_charts-1.0.8/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      402 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-23 13:32:25.440428 lightweight_charts-1.0.8/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-23 13:30:34.000000 lightweight_charts-1.0.8/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-29 20:33:37.966659 lightweight_charts-1.0.9/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.9/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     7769 2023-05-29 20:33:37.966105 lightweight_charts-1.0.9/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     7423 2023-05-29 19:43:54.000000 lightweight_charts-1.0.9/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-29 20:33:37.962608 lightweight_charts-1.0.9/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       82 2023-05-29 19:31:49.000000 lightweight_charts-1.0.9/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     2985 2023-05-29 19:31:32.000000 lightweight_charts-1.0.9/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)     9559 2023-05-29 19:31:32.000000 lightweight_charts-1.0.9/lightweight_charts/chartasync.py
+-rw-r--r--   0 louis      (501) staff       (20)    27637 2023-05-29 19:24:40.000000 lightweight_charts-1.0.9/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   148472 2023-05-20 23:46:07.000000 lightweight_charts-1.0.9/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     2083 2023-05-21 12:37:38.000000 lightweight_charts-1.0.9/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     4390 2023-05-29 19:16:13.000000 lightweight_charts-1.0.9/lightweight_charts/widgets.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-29 20:33:37.965397 lightweight_charts-1.0.9/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     7769 2023-05-29 20:33:37.000000 lightweight_charts-1.0.9/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      435 2023-05-29 20:33:37.000000 lightweight_charts-1.0.9/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-29 20:33:37.000000 lightweight_charts-1.0.9/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-29 20:33:37.000000 lightweight_charts-1.0.9/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-29 20:33:37.000000 lightweight_charts-1.0.9/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-29 20:33:37.966816 lightweight_charts-1.0.9/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-29 18:05:30.000000 lightweight_charts-1.0.9/setup.py
```

### Comparing `lightweight_charts-1.0.8/LICENSE` & `lightweight_charts-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.8/PKG-INFO` & `lightweight_charts-1.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1
-Name: lightweight_charts
-Version: 1.0.8
-Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
-Home-page: https://github.com/louisnw01/lightweight-charts-python
-Author: louisnw
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<div align="center">
 
-# lightweight_charts_python
+# lightweight-charts-python
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
-
+![async](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_async/async.png)
 ![cover](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
+</div>
 
 ## Installation
 ```
-pip install lightweight_charts
+pip install lightweight-charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
-4. Support for PyQt and wxPython.
-5. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
+4. Supports:
+   * PyQt
+   * wxPython
+   * Streamlit
+   * asyncio
+5. [Callbacks](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#chartasync) allowing for timeframe (1min, 5min, 30min etc.) selectors, searching, and more.
+6. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -188,42 +184,78 @@
 
     chart.show(block=True)
 
 ```
 ![styling image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/5_styling/styling.png)
 ___
 
-### 6. Callbacks:
+### 6. ChartAsync:
 
 ```python
+import asyncio
 import pandas as pd
-from lightweight_charts import Chart
 
+from lightweight_charts import ChartAsync
 
-def on_click(bar: dict):
-    print(f"Time: {bar['time']} | Close: {bar['close']}")
 
+def get_bar_data(symbol, timeframe):
+    return pd.read_csv(f'bar_data/{symbol}_{timeframe}.csv')
 
-if __name__ == '__main__':
-    
-    chart = Chart()
 
-    df = pd.read_csv('ohlcv.csv')
+class API:
+    def __init__(self):
+        self.chart = None  # Changes after each callback.
+        self.symbol = 'TSLA'
+        self.timeframe = '5min'
+
+    async def on_search(self, searched_string):  # Called when the user searches.
+        self.symbol = searched_string
+        new_data = await self.get_data()
+        if new_data.empty:
+            return
+        self.chart.set(new_data)
+        self.chart.corner_text(searched_string)
+
+    async def on_timeframe_selection(self, timeframe):  # Called when the user changes the timeframe.
+        self.timeframe = timeframe
+        new_data = await self.get_data()
+        if new_data.empty:
+            return
+        self.chart.set(new_data)
+
+    async def get_data(self):
+        if self.symbol not in ('AAPL', 'GOOGL', 'TSLA'):
+            print(f'No data for "{self.symbol}"')
+            return pd.DataFrame()
+        data = get_bar_data(self.symbol, self.timeframe)
+        return data
+
+
+async def main():
+    api = API()
+
+    chart = ChartAsync(api=api, debug=True)
+    chart.legend(True)
+
+    chart.create_switcher(api.on_timeframe_selection, '1min', '5min', '30min', default='5min')
+    chart.corner_text(api.symbol)
+
+    df = get_bar_data(api.symbol, api.timeframe)
     chart.set(df)
 
-    chart.subscribe_click(on_click)
+    await chart.show(block=True)
 
-    chart.show(block=True)
+
+if __name__ == '__main__':
+    asyncio.run(main())
 
 ```
-![callbacks gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_callbacks/callbacks.gif)
+![async gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_async/async.gif)
 ___
 
-[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
+<div align="center">
 
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
-
-
-
-
+</div>
```

### Comparing `lightweight_charts-1.0.8/README.md` & `lightweight_charts-1.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,51 @@
-# lightweight_charts_python
+Metadata-Version: 2.1
+Name: lightweight_charts
+Version: 1.0.9
+Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
+Home-page: https://github.com/louisnw01/lightweight-charts-python
+Author: louisnw
+License: MIT
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+# lightweight-charts-python
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
-
+![async](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_async/async.png)
 ![cover](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
+</div>
 
 ## Installation
 ```
-pip install lightweight_charts
+pip install lightweight-charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
-4. Support for PyQt and wxPython.
-5. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
+4. Supports:
+   * PyQt
+   * wxPython
+   * Streamlit
+   * asyncio
+5. [Callbacks](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#chartasync) allowing for timeframe (1min, 5min, 30min etc.) selectors, searching, and more.
+6. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -176,40 +196,80 @@
 
     chart.show(block=True)
 
 ```
 ![styling image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/5_styling/styling.png)
 ___
 
-### 6. Callbacks:
+### 6. ChartAsync:
 
 ```python
+import asyncio
 import pandas as pd
-from lightweight_charts import Chart
 
+from lightweight_charts import ChartAsync
 
-def on_click(bar: dict):
-    print(f"Time: {bar['time']} | Close: {bar['close']}")
 
+def get_bar_data(symbol, timeframe):
+    return pd.read_csv(f'bar_data/{symbol}_{timeframe}.csv')
 
-if __name__ == '__main__':
-    
-    chart = Chart()
 
-    df = pd.read_csv('ohlcv.csv')
+class API:
+    def __init__(self):
+        self.chart = None  # Changes after each callback.
+        self.symbol = 'TSLA'
+        self.timeframe = '5min'
+
+    async def on_search(self, searched_string):  # Called when the user searches.
+        self.symbol = searched_string
+        new_data = await self.get_data()
+        if new_data.empty:
+            return
+        self.chart.set(new_data)
+        self.chart.corner_text(searched_string)
+
+    async def on_timeframe_selection(self, timeframe):  # Called when the user changes the timeframe.
+        self.timeframe = timeframe
+        new_data = await self.get_data()
+        if new_data.empty:
+            return
+        self.chart.set(new_data)
+
+    async def get_data(self):
+        if self.symbol not in ('AAPL', 'GOOGL', 'TSLA'):
+            print(f'No data for "{self.symbol}"')
+            return pd.DataFrame()
+        data = get_bar_data(self.symbol, self.timeframe)
+        return data
+
+
+async def main():
+    api = API()
+
+    chart = ChartAsync(api=api, debug=True)
+    chart.legend(True)
+
+    chart.create_switcher(api.on_timeframe_selection, '1min', '5min', '30min', default='5min')
+    chart.corner_text(api.symbol)
+
+    df = get_bar_data(api.symbol, api.timeframe)
     chart.set(df)
 
-    chart.subscribe_click(on_click)
+    await chart.show(block=True)
 
-    chart.show(block=True)
+
+if __name__ == '__main__':
+    asyncio.run(main())
 
 ```
-![callbacks gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_callbacks/callbacks.gif)
+![async gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_async/async.gif)
 ___
 
-[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
+<div align="center">
 
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
+</div>
```

### Comparing `lightweight_charts-1.0.8/lightweight_charts/chart.py` & `lightweight_charts-1.0.9/lightweight_charts/chart.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import webview
 import multiprocessing as mp
 
 from lightweight_charts.js import LWC
 
 
+class CallbackAPI:
+    def __init__(self, emit): self.emit = emit
+
+    def callback(self, message: str):
+        messages = message.split('__')
+        name, chart_id = messages[:2]
+        args = messages[2:]
+        self.emit.put((name, chart_id, *args))
+
+
 class PyWV:
-    def __init__(self, q, exit, loaded, html, js_api, width, height, x, y, on_top, debug):
+    def __init__(self, q, exit, loaded, html, width, height, x, y, on_top, debug, emit=None):
         self.queue = q
         self.exit = exit
         self.loaded = loaded
         self.debug = debug
-        self.js_api = js_api
-        self.webview = webview.create_window('', html=html, on_top=on_top, js_api=js_api,
-                                             width=width, height=height, x=x, y=y, background_color='#000000')
+        js_api = CallbackAPI(emit) if emit else None
+        self.webview = webview.create_window('', html=html, on_top=on_top, js_api=js_api, width=width, height=height,
+                                             x=x, y=y, background_color='#000000')
         self.webview.events.loaded += self.on_js_load
         self.loop()
 
     def loop(self):
         while 1:
             arg = self.queue.get()
             if arg in ('start', 'show', 'hide', 'exit'):
                 webview.start(debug=self.debug) if arg == 'start' else getattr(self.webview, arg)()
                 self.exit.set() if arg in ('start', 'exit') else None
-            elif arg == 'subscribe':
-                func, c_id = (self.queue.get() for _ in range(2))
-                self.js_api.click_funcs[str(c_id)] = func
             else:
                 try:
                     self.webview.evaluate_js(arg)
                 except KeyError:
                     return
 
     def on_js_load(self):
@@ -36,20 +43,19 @@
 
 
 class Chart(LWC):
     def __init__(self, volume_enabled: bool = True, width: int = 800, height: int = 600, x: int = None, y: int = None,
                  on_top: bool = False, debug: bool = False,
                  inner_width: float = 1.0, inner_height: float = 1.0, dynamic_loading: bool = False):
         super().__init__(volume_enabled, inner_width, inner_height, dynamic_loading)
-        self._js_api_code = 'pywebview.api.onClick'
         self._q = mp.Queue()
         self._script_func = self._q.put
         self._exit = mp.Event()
         self._loaded = mp.Event()
-        self._process = mp.Process(target=PyWV, args=(self._q, self._exit, self._loaded, self._html, self._js_api,
+        self._process = mp.Process(target=PyWV, args=(self._q, self._exit, self._loaded, self._html,
                                                       width, height, x, y, on_top, debug,), daemon=True)
         self._process.start()
         self._create_chart()
 
     def show(self, block: bool = False):
         """
         Shows the chart window.\n
@@ -79,13 +85,7 @@
         Exits and destroys the chart window.\n
         """
         self._q.put('exit')
         self._exit.wait()
         self._process.terminate()
         del self
 
-    def subscribe_click(self, function: object):
-        self._q.put('subscribe')
-        self._q.put(function)
-        self._q.put(self.id)
-        super().subscribe_click(function)
-
```

### Comparing `lightweight_charts-1.0.8/lightweight_charts/js.py` & `lightweight_charts-1.0.9/lightweight_charts/js.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def _series_datetime_format(self, series):
         if 'date' in series.keys():
             series = series.rename({'date': 'time'})
         series['time'] = self._datetime_format(series['time'])
         return series
 
-    def _datetime_format(self, arg):
+    def _datetime_format(self, arg: Union[pd.Series, str]):
         arg = pd.to_datetime(arg)
         if self._interval != timedelta(days=1):
             arg = arg.astype('int64') // 10 ** 9 if isinstance(arg, pd.Series) else arg.timestamp()
             arg = self._interval.total_seconds() * (arg // self._interval.total_seconds())
         else:
             arg = arg.dt.strftime('%Y-%m-%d') if isinstance(arg, pd.Series) else arg.strftime('%Y-%m-%d')
         return arg
@@ -76,29 +76,17 @@
                }});''')
 
     def horizontal_line(self, price: Union[float, int], color: str = 'rgb(122, 146, 202)', width: int = 1,
                         style: LINE_STYLE = 'solid', text: str = '', axis_label_visible=True):
         """
         Creates a horizontal line at the given price.\n
         """
-        var = self._rand.generate()
         self.run_script(f"""
-           let priceLine{var} = {{
-               price: {price},
-               color: '{color}',
-               lineWidth: {width},
-               lineStyle: {_line_style(style)},
-               axisLabelVisible: {_js_bool(axis_label_visible)},
-               title: '{text}',
-           }};
-           let line{var} = {{
-               line: {self.id}.series.createPriceLine(priceLine{var}),
-               price: {price},
-           }};
-           {self.id}.horizontal_lines.push(line{var})""")
+        makeHorizontalLine({self.id}, {price}, '{color}', {width}, {_line_style(style)}, {_js_bool(axis_label_visible)}, '{text}')
+        """)
 
     def remove_horizontal_line(self, price: Union[float, int]):
         """
         Removes a horizontal line at the given price.
         """
         self.run_script(f'''
            {self.id}.horizontal_lines.forEach(function (line) {{
@@ -112,19 +100,19 @@
         self.run_script(f'{self.id}.series.applyOptions({{title: "{title}"}})')
 
 
 class Line(SeriesCommon):
     def __init__(self, parent, color, width):
         self._parent = parent
         self._rand = self._parent._rand
-        self.id = self._rand.generate()
+        self.id = f'window.{self._rand.generate()}'
         self.run_script = self._parent.run_script
 
         self._parent.run_script(f'''
-            var {self.id} = {{
+            {self.id} = {{
                 series: {self._parent.id}.chart.addLineSeries({{
                     color: '{color}',
                     lineWidth: {width},
                 }}),
                 markers: [],
                 horizontal_lines: [],
             }}
@@ -145,64 +133,46 @@
         :param series: labels: date/time, value
         """
         series = self._parent._series_datetime_format(series)
         self._last_bar = series
         self.run_script(f'{self.id}.series.update({series.to_dict()})')
 
 
-class API:
-    def __init__(self):
-        self.click_funcs = {}
-
-    def onClick(self, data):
-        click_func = self.click_funcs[data['id']]
-        if isinstance(data['time'], int):
-            data['time'] = datetime.fromtimestamp(data['time'])
-        else:
-            data['time'] = datetime.strptime(data['time'], '%Y-%m-%d')
-        click_func(data) if click_func else None
-
-
 class LWC(SeriesCommon):
     def __init__(self, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0, dynamic_loading: bool = False):
         self._volume_enabled = volume_enabled
         self._inner_width = inner_width
         self._inner_height = inner_height
         self._dynamic_loading = dynamic_loading
 
         self._rand = IDGen()
-        self.id = self._rand.generate()
+        self.id = f'window.{self._rand.generate()}'
         self._position = 'left'
         self.loaded = False
         self._html = HTML
-        self._append_js = f'document.body.append({self.id}.div)'
         self._scripts = []
         self._script_func = None
         self._last_bar = None
         self._interval = None
-        self._js_api = API()
-        self._js_api_code = None
 
         self._background_color = '#000000'
         self._volume_up_color = 'rgba(83,141,131,0.8)'
         self._volume_down_color = 'rgba(200,127,130,0.8)'
 
     def _on_js_load(self):
+        if self.loaded:
+            return
         self.loaded = True
-        for script in self._scripts:
-            self.run_script(script)
+        [self.run_script(script) for script in self._scripts]
 
-    def _create_chart(self):
+    def _create_chart(self, top_bar=False):
         self.run_script(f'''
-            {self.id} = makeChart({self._inner_width}, {self._inner_height})
-            {self.id}.div.style.float = "{self._position}"
-            {self._append_js}
-            window.addEventListener('resize', function() {{
-                {self.id}.chart.resize(window.innerWidth*{self.id}.scale.width, window.innerHeight*{self.id}.scale.height)
-                }});
+            {self.id} = makeChart({self._inner_width}, {self._inner_height}, topBar={_js_bool(top_bar)})
+            {self.id}.id = '{self.id}'
+            {self.id}.wrapper.style.float = "{self._position}"
             ''')
 
     def run_script(self, script):
         """
         For advanced users; evaluates JavaScript within the Webview.
         """
         self._script_func(script) if self.loaded else self._scripts.append(script)
@@ -494,67 +464,42 @@
             {f"{self.id}.legend.style.fontFamily = '{font_family}'" if font_family else ''}
             
             {self.id}.chart.subscribeCrosshairMove((param) => {{   
                 if (param.time){{
                     const data = param.seriesData.get({self.id}.series);
                     if (!data) {{return}}
                     let percentMove = ((data.close-data.open)/data.open)*100
-                    let ohlc = `open: ${{legendItemFormat(data.open)}} 
-                                | high: ${{legendItemFormat(data.high)}} 
-                                | low: ${{legendItemFormat(data.low)}}
-                                | close: ${{legendItemFormat(data.close)}} `
-                    let percent = `| daily: ${{percentMove >= 0 ? '+' : ''}}${{percentMove.toFixed(2)}} %`
+                    let ohlc = `O ${{legendItemFormat(data.open)}} 
+                                | H ${{legendItemFormat(data.high)}} 
+                                | L ${{legendItemFormat(data.low)}}
+                                | C ${{legendItemFormat(data.close)}} `
+                    let percent = `| ${{percentMove >= 0 ? '+' : ''}}${{percentMove.toFixed(2)}} %`
                     let finalString = ''
                     {'finalString += ohlc' if ohlc else ''}
                     {'finalString += percent' if percent else ''}
                     {self.id}.legend.innerHTML = finalString
                 }}
                 else {{
                     {self.id}.legend.innerHTML = ''
                 }}
             }});''')
 
-    def subscribe_click(self, function: object):
-        """
-        Subscribes the given function to a chart click event.
-        The event returns a dictionary containing the bar object at the time clicked, and the price at the crosshair.
-        """
-        self._js_api.click_funcs[self.id] = function
-        self.run_script(f'''
-            {self.id}.chart.subscribeClick((param) => {{
-                if (!param.point) {{return}}
-                let prices = param.seriesData.get({self.id}.series);
-                let data = {{
-                    time: param.time,
-                    open: prices.open,
-                    high: prices.high,
-                    low: prices.low,
-                    close: prices.close,
-                    hover: {self.id}.series.coordinateToPrice(param.point.y),
-                    id: '{self.id}'
-                    }}
-                {self._js_api_code}(data)
-                }})''')
-
     def create_subchart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
                          width: float = 0.5, height: float = 0.5, sync: Union[bool, str] = False):
         return SubChart(self, volume_enabled, position, width, height, sync)
 
 
 class SubChart(LWC):
     def __init__(self, parent, volume_enabled, position, width, height, sync):
         super().__init__(volume_enabled, width, height)
         self._chart = parent._chart if isinstance(parent, SubChart) else parent
         self._parent = parent
         self._position = position
         self._rand = self._chart._rand
         self.id = f'window.{self._rand.generate()}'
-        self._append_js = f'{self._parent.id}.div.parentNode.insertBefore({self.id}.div, {self._parent.id}.div.nextSibling)'
-        self._js_api = self._chart._js_api
-        self._js_api_code = self._chart._js_api_code
         self.run_script = self._chart.run_script
         self._create_chart()
         if not sync:
             return
         sync_parent_var = self._parent.id if isinstance(sync, bool) else sync
         self.run_script(f'''
             {sync_parent_var}.chart.timeScale().subscribeVisibleLogicalRangeChange((timeRange) => {{
@@ -565,30 +510,38 @@
 
 SCRIPT = """
 document.body.style.backgroundColor = '#000000'
 const up = 'rgba(39, 157, 130, 100)'
 const down = 'rgba(200, 97, 100, 100)'
 
 const wrapper = document.createElement('div')
+wrapper.className = 'wrapper'
 document.body.appendChild(wrapper)
 
-function makeChart(innerWidth, innerHeight) {
+function makeChart(innerWidth, innerHeight, topBar=false) {
     let chart = {
         markers: [],
         horizontal_lines: [],
         div: document.createElement('div'),
+        wrapper: document.createElement('div'),
         legend: document.createElement('div'),
         scale: {
             width: innerWidth,
             height: innerHeight
         },
     }
+    let topBarOffset = 0
+    if (topBar) {
+    makeTopBar(chart)
+    topBarOffset = chart.topBar.offsetHeight
+    }
+    
     chart.chart = LightweightCharts.createChart(chart.div, {
         width: window.innerWidth*innerWidth,
-        height: window.innerHeight*innerHeight,
+        height: (window.innerHeight*innerHeight)-topBarOffset,
         layout: {
             textColor: '#d1d4dc',
             background: {
                 color:'#000000',
                 type: LightweightCharts.ColorType.Solid,
                 },
             fontSize: 12
@@ -608,14 +561,20 @@
         },
         grid: {
             vertLines: {color: 'rgba(29, 30, 38, 5)'},
             horzLines: {color: 'rgba(29, 30, 58, 5)'},
         },
         handleScroll: {vertTouchDrag: true},
     })
+    window.addEventListener('resize', function() {
+        if (topBar) {
+        topBarOffset = chart.topBar.offsetHeight
+        }
+        chart.chart.resize(window.innerWidth*innerWidth, (window.innerHeight*innerHeight)-topBarOffset)
+        });
     chart.series = chart.chart.addCandlestickSeries({color: 'rgb(0, 120, 255)', upColor: up, borderUpColor: up, wickUpColor: up,
                                         downColor: down, borderDownColor: down, wickDownColor: down, lineWidth: 2,
                                         })
     chart.volumeSeries = chart.chart.addHistogramSeries({
                         color: '#26a69a',
                         priceFormat: {type: 'volume'},
                         priceScaleId: '',
@@ -627,17 +586,42 @@
     chart.legend.style.zIndex = 1000
     chart.legend.style.width = `${(chart.scale.width*100)-8}vw`
     chart.legend.style.top = '10px'
     chart.legend.style.left = '10px'
     chart.legend.style.fontFamily = 'Monaco'
     chart.legend.style.fontSize = '11px'
     chart.legend.style.color = 'rgb(191, 195, 203)'
+    
+    chart.wrapper.style.width = `${100*innerWidth}%`
+    chart.wrapper.style.height = `${100*innerHeight}%`
+    chart.div.style.position = 'relative'
+    chart.wrapper.style.display = 'flex'
+    chart.wrapper.style.flexDirection = 'column'
+    
     chart.div.appendChild(chart.legend)
+    chart.wrapper.appendChild(chart.div)
+    wrapper.append(chart.wrapper)
+    
     return chart
 }
+function makeHorizontalLine(chart, price, color, width, style, axisLabelVisible, text) {
+    let priceLine = {
+       price: price,
+       color: color,
+       lineWidth: width,
+       lineStyle: style,
+       axisLabelVisible: axisLabelVisible,
+       title: text,
+    };
+    let line = {
+       line: chart.series.createPriceLine(priceLine),
+       price: price,
+    };
+    chart.horizontal_lines.push(line)
+}
 function legendItemFormat(num) {
 return num.toFixed(2).toString().padStart(8, ' ')
 }
 """
 
 HTML = f"""
 <!DOCTYPE html>
```

### Comparing `lightweight_charts-1.0.8/lightweight_charts/pkg.py` & `lightweight_charts-1.0.9/lightweight_charts/pkg.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.8/lightweight_charts/util.py` & `lightweight_charts-1.0.9/lightweight_charts/util.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.8/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.9/lightweight_charts.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 Metadata-Version: 2.1
 Name: lightweight-charts
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# lightweight_charts_python
+<div align="center">
+
+# lightweight-charts-python
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
-
+![async](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_async/async.png)
 ![cover](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
+</div>
 
 ## Installation
 ```
-pip install lightweight_charts
+pip install lightweight-charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
-4. Support for PyQt and wxPython.
-5. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
+4. Supports:
+   * PyQt
+   * wxPython
+   * Streamlit
+   * asyncio
+5. [Callbacks](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#chartasync) allowing for timeframe (1min, 5min, 30min etc.) selectors, searching, and more.
+6. Multi-Pane Charts using the `SubChart` ([examples](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html#subchart)).
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -188,42 +196,80 @@
 
     chart.show(block=True)
 
 ```
 ![styling image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/5_styling/styling.png)
 ___
 
-### 6. Callbacks:
+### 6. ChartAsync:
 
 ```python
+import asyncio
 import pandas as pd
-from lightweight_charts import Chart
 
+from lightweight_charts import ChartAsync
 
-def on_click(bar: dict):
-    print(f"Time: {bar['time']} | Close: {bar['close']}")
 
+def get_bar_data(symbol, timeframe):
+    return pd.read_csv(f'bar_data/{symbol}_{timeframe}.csv')
 
-if __name__ == '__main__':
-    
-    chart = Chart()
 
-    df = pd.read_csv('ohlcv.csv')
+class API:
+    def __init__(self):
+        self.chart = None  # Changes after each callback.
+        self.symbol = 'TSLA'
+        self.timeframe = '5min'
+
+    async def on_search(self, searched_string):  # Called when the user searches.
+        self.symbol = searched_string
+        new_data = await self.get_data()
+        if new_data.empty:
+            return
+        self.chart.set(new_data)
+        self.chart.corner_text(searched_string)
+
+    async def on_timeframe_selection(self, timeframe):  # Called when the user changes the timeframe.
+        self.timeframe = timeframe
+        new_data = await self.get_data()
+        if new_data.empty:
+            return
+        self.chart.set(new_data)
+
+    async def get_data(self):
+        if self.symbol not in ('AAPL', 'GOOGL', 'TSLA'):
+            print(f'No data for "{self.symbol}"')
+            return pd.DataFrame()
+        data = get_bar_data(self.symbol, self.timeframe)
+        return data
+
+
+async def main():
+    api = API()
+
+    chart = ChartAsync(api=api, debug=True)
+    chart.legend(True)
+
+    chart.create_switcher(api.on_timeframe_selection, '1min', '5min', '30min', default='5min')
+    chart.corner_text(api.symbol)
+
+    df = get_bar_data(api.symbol, api.timeframe)
     chart.set(df)
 
-    chart.subscribe_click(on_click)
+    await chart.show(block=True)
 
-    chart.show(block=True)
+
+if __name__ == '__main__':
+    asyncio.run(main())
 
 ```
-![callbacks gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_callbacks/callbacks.gif)
+![async gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_async/async.gif)
 ___
 
-[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
+<div align="center">
 
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
-
-
+</div>
```

### Comparing `lightweight_charts-1.0.8/setup.py` & `lightweight_charts-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

