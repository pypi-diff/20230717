# Comparing `tmp/ex4nicegui-0.1.8.tar.gz` & `tmp/ex4nicegui-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.8.tar", last modified: Sun Jul 16 10:57:03 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.9.tar", last modified: Mon Jul 17 16:37:56 2023, max compression
```

## Comparing `ex4nicegui-0.1.8.tar` & `ex4nicegui-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.790430 ex4nicegui-0.1.8/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-16 10:57:03.789432 ex4nicegui-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.680226 ex4nicegui-0.1.8/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-16 10:56:47.000000 ex4nicegui-0.1.8/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.694085 ex4nicegui-0.1.8/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.708144 ex4nicegui-0.1.8/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0     1300 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.713221 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     2902 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.747468 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2559 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0    38721 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/officials.py
--rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/rxui.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.752437 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2142 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/usePagination.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.756441 ex4nicegui-0.1.8/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.8/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.787434 ex4nicegui-0.1.8/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.8/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.691351 ex4nicegui-0.1.8/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:57:03.790430 ex4nicegui-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.665471 ex4nicegui-0.1.9/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-17 16:37:56.664473 ex4nicegui-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.599861 ex4nicegui-0.1.9/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-17 16:36:37.000000 ex4nicegui-0.1.9/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.620914 ex4nicegui-0.1.9/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.636149 ex4nicegui-0.1.9/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.644816 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.js
+-rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.649806 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     4857 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     2888 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0     1303 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/drawer.py
+-rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    38806 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.654792 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.658458 ex4nicegui-0.1.9/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.9/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.9/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.663448 ex4nicegui-0.1.9/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.9/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.9/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.615924 ex4nicegui-0.1.9/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1101 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 16:37:56.666440 ex4nicegui-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/setup.py
```

### Comparing `ex4nicegui-0.1.8/LICENSE` & `ex4nicegui-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/README.md` & `ex4nicegui-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.9/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/__index.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     UploadBindableUi as upload,
     UploadResult,
 )
 from .q_pagination import QPagination as q_pagination
 from .local_file_picker import local_file_picker
 from ex4nicegui.utils.signals import ref_computed
 from signe import effect
-from .draggable.UseDraggable import use_draggable
+from .UseDraggable.UseDraggable import use_draggable
 from .useMouse.UseMouse import use_mouse
 from .drawer import drawer
 from .usePagination import PaginationRef as use_pagination
```

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -186,15 +186,15 @@
     },
     emits: ["update", "isDraggingUpdate"],
     setup(e, {
         emit: r
     }) {
         const t = e;
         return q(() => {
-            const o = document.getElementById(t.elementId),
+            const o = document.getElementById(`c${t.elementId}`),
                 {
                     x: a,
                     y: c,
                     style: g,
                     isDragging: _
                 } = le(o, t.options);
             h([a, c, g], ([l, f, i]) => {
```

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         ud.bind_style(element)
 
     return ud
 
 
 class UseDraggable(Element, component="UseDraggable.js"):
     def __init__(self, element: Element, init_x=0.0, init_y=0.0) -> None:
-        super().__init__("UseDraggable")
+        super().__init__()
         self._props["elementId"] = str(element.id)
         self._props["options"] = {"initialValue": {"x": init_x, "y": init_y}}
 
         self.__style_getter, self.__style_setter = createSignal("")
         self.__x_getter, self.__x_setter = createSignal(init_x)
         self.__y_getter, self.__y_setter = createSignal(init_y)
         self.__isDragging_getter, self.__isDragging_setter = createSignal(False)
```

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     dataType: Optional[str]
     value: Any
     color: str
 
 
 class echarts(Element, component="ECharts.js"):
     def __init__(self, options: dict) -> None:
-        super().__init__("ECharts")
+        super().__init__()
         self._props["options"] = options
 
     def update_options(self, options: dict, opts: Optional[dict] = None):
         """update chart options
 
         Args:
             options (dict): chart setting options dict
```

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/officials.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/officials.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from nicegui.elements.mixins.value_element import ValueElement
 from nicegui.elements.mixins.color_elements import (
     TextColorElement,
     QUASAR_COLORS,
     TAILWIND_COLORS,
 )
 from nicegui.page_layout import Drawer
-from ex4nicegui.reactive.echarts.ECharts import echarts
+from ex4nicegui.reactive.ECharts.ECharts import echarts
 
 T = TypeVar("T")
 
 TWidget = TypeVar("TWidget")
 
 
 class BindableUi(Generic[TWidget]):
@@ -572,15 +572,15 @@
         @effect
         def _():
             ele.value = self.value
 
         def onValueChanged():
             self._ref.value = ele.value
 
-        ele.on("change ", onValueChanged)
+        ele.on("change", onValueChanged)
 
 
 class TextareaBindableUi(SingleValueBindableUi[str, ui.textarea]):
     def __init__(
         self,
         label: Optional[TMaybeRef[str]] = None,
         *,
@@ -1342,30 +1342,32 @@
         def _():
             ele = self.element
             source = ref_ui.value
             ele.on_source_change(source)
 
 
 class UploadResult:
-    def __init__(self, content: bytes = bytes()):
+    def __init__(self, content: bytes = bytes(), name="", type=""):
         self.content = content
+        self.name = name
+        self.type = type
 
     def get_bytes(self):
         return self.content
 
     @property
     def ready(self):
         return len(self.content) > 0
 
 
 class UploadBindableUi(SingleValueBindableUi[UploadResult, ui.upload]):
     @staticmethod
     def _setup_(binder: "UploadBindableUi"):
         def on_upload(e: ng_events.UploadEventArguments):
-            binder._ref.value = UploadResult(e.content.read())
+            binder._ref.value = UploadResult(e.content.read(), e.name, e.type)
 
         binder._on_upload_callbacks.append(on_upload)
 
     def __init__(
         self,
         multiple: TMaybeRef[bool] = False,
         max_file_size: Optional[TMaybeRef[int]] = None,
```

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, cast
 from dataclasses import dataclass
 from nicegui.helpers import KWONLY_SLOTS
 from nicegui.events import handle_event, EventArguments
 from nicegui.element import Element
 from signe import createSignal, effect, batch
+from ex4nicegui.utils.signals import ref_from_signal
 
+# from nicegui.dependencies import register_library
+# from pathlib import Path
+
+
+# register_library(Path(__file__).parent / "index-6543384e.js")
 
 _Update_Args = [
     "x",
     "y",
     "sourceType",
 ]
 
@@ -18,43 +24,48 @@
     x: float
     y: float
     sourceType: str
 
 
 class UseMouse(Element, component="UseMouse.js"):
     def __init__(self, options: Optional[dict] = None) -> None:
-        super().__init__("UseMouse")
+        super().__init__()
 
         if options:
             self._props["options"] = options
 
         self.__x_getter, self.__x_setter = createSignal(0.0)
+        self.__x_readonly_ref = ref_from_signal(self.__x_getter)
+
         self.__y_getter, self.__y_setter = createSignal(0.0)
+        self.__y_readonly_ref = ref_from_signal(self.__y_getter)
+
         self.__sourceType_getter, self.__sourceType_setter = createSignal("sourceType")
+        self.__sourceType_readonly_ref = ref_from_signal(self.__sourceType_getter)
 
         def update(args: UseMouseUpdateEventArguments):
             @batch
             def _():
                 self.__x_setter(args.x)
                 self.__y_setter(args.y)
                 self.__sourceType_setter(args.sourceType)
 
         self.on_update(update)
 
     @property
     def x(self):
-        return self.__x_getter()
+        return self.__x_readonly_ref
 
     @property
     def y(self):
-        return self.__y_getter()
+        return self.__y_readonly_ref
 
     @property
     def sourceType(self):
-        return self.__sourceType_getter()
+        return self.__sourceType_readonly_ref
 
     def on_update(self, handler: Optional[Callable[..., Any]]):
         def inner_handler(e):
             args = e.args
             handle_event(
                 handler,
                 UseMouseUpdateEventArguments(
@@ -65,16 +76,16 @@
                     sourceType=args["sourceType"],
                 ),
             )
 
         self.on("update", inner_handler, args=_Update_Args)
 
 
-_Use_Mouse_Ins = UseMouse()
+_Use_Mouse_Ins = None
 
 
 def use_mouse(options: Optional[dict] = None):
     global _Use_Mouse_Ins
-    # if _Use_Mouse_Ins is None:
-    #     _Use_Mouse_Ins = UseMouse(options)
+    if _Use_Mouse_Ins is None:
+        _Use_Mouse_Ins = UseMouse(options)
 
-    return _Use_Mouse_Ins
+    return cast(UseMouse, _Use_Mouse_Ins)
```

### Comparing `ex4nicegui-0.1.8/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.1.9/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.9/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.9/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.8/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.9/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 ex4nicegui/reactive/__init__.py
 ex4nicegui/reactive/drawer.py
 ex4nicegui/reactive/local_file_picker.py
 ex4nicegui/reactive/officials.py
 ex4nicegui/reactive/q_pagination.py
 ex4nicegui/reactive/rxui.py
 ex4nicegui/reactive/usePagination.py
-ex4nicegui/reactive/draggable/UseDraggable.js
-ex4nicegui/reactive/draggable/UseDraggable.py
-ex4nicegui/reactive/draggable/__init__.py
-ex4nicegui/reactive/echarts/ECharts.js
-ex4nicegui/reactive/echarts/ECharts.py
-ex4nicegui/reactive/echarts/__init__.py
+ex4nicegui/reactive/ECharts/ECharts.js
+ex4nicegui/reactive/ECharts/ECharts.py
+ex4nicegui/reactive/ECharts/__init__.py
+ex4nicegui/reactive/UseDraggable/UseDraggable.js
+ex4nicegui/reactive/UseDraggable/UseDraggable.py
+ex4nicegui/reactive/UseDraggable/__init__.py
 ex4nicegui/reactive/useMouse/UseMouse.js
 ex4nicegui/reactive/useMouse/UseMouse.py
 ex4nicegui/reactive/useMouse/__init__.py
 ex4nicegui/tools/__init__.py
 ex4nicegui/tools/debug.py
 ex4nicegui/utils/__init__.py
 ex4nicegui/utils/common.py
```

### Comparing `ex4nicegui-0.1.8/setup.py` & `ex4nicegui-0.1.9/setup.py`

 * *Files identical despite different names*

