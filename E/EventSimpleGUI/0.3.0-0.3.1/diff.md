# Comparing `tmp/EventSimpleGUI-0.3.0.tar.gz` & `tmp/EventSimpleGUI-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EventSimpleGUI-0.3.0.tar", last modified: Sun Feb 19 22:55:21 2023, max compression
+gzip compressed data, was "EventSimpleGUI-0.3.1.tar", last modified: Mon Jul 17 01:16:12 2023, max compression
```

## Comparing `EventSimpleGUI-0.3.0.tar` & `EventSimpleGUI-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 22:55:21.270555 EventSimpleGUI-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-02-19 22:55:21.265555 EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/
--rw-rw-rw-   0        0        0     3950 2023-02-19 22:55:21.000000 EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-02-19 22:55:21.000000 EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 22:55:21.000000 EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-19 22:55:21.000000 EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-19 22:55:21.000000 EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-01-20 17:34:03.000000 EventSimpleGUI-0.3.0/LICENCE
--rw-rw-rw-   0        0        0     3950 2023-02-19 22:55:21.269559 EventSimpleGUI-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-02-19 10:21:42.000000 EventSimpleGUI-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 22:55:21.268583 EventSimpleGUI-0.3.0/pysimpleevent/
--rw-rw-rw-   0        0        0       50 2023-02-19 06:18:44.000000 EventSimpleGUI-0.3.0/pysimpleevent/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-02-19 22:49:17.000000 EventSimpleGUI-0.3.0/pysimpleevent/fastevent.py
--rw-rw-rw-   0        0        0       42 2023-02-19 22:55:21.270555 EventSimpleGUI-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-02-19 22:55:14.000000 EventSimpleGUI-0.3.0/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 01:16:12.573209 EventSimpleGUI-0.3.1/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 01:16:12.573209 EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3822 2023-07-17 01:16:12.000000 EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      268 2023-07-17 01:16:12.000000 EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-17 01:16:12.000000 EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       12 2023-07-17 01:16:12.000000 EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       14 2023-07-17 01:16:12.000000 EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1072 2023-07-17 00:59:41.000000 EventSimpleGUI-0.3.1/LICENCE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3822 2023-07-17 01:16:12.573209 EventSimpleGUI-0.3.1/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3052 2023-07-17 00:59:41.000000 EventSimpleGUI-0.3.1/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 01:16:12.573209 EventSimpleGUI-0.3.1/pysimpleevent/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2023-07-17 00:59:41.000000 EventSimpleGUI-0.3.1/pysimpleevent/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3313 2023-07-17 01:03:41.000000 EventSimpleGUI-0.3.1/pysimpleevent/fastevent.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-17 01:16:12.573209 EventSimpleGUI-0.3.1/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1106 2023-07-17 01:14:36.000000 EventSimpleGUI-0.3.1/setup.py
```

### Comparing `EventSimpleGUI-0.3.0/EventSimpleGUI.egg-info/PKG-INFO` & `EventSimpleGUI-0.3.1/EventSimpleGUI.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-Metadata-Version: 2.1
-Name: EventSimpleGUI
-Version: 0.3.0
-Summary: A simple tool to create events to PySimpleGUI
-Home-page: https://github.com/MikalROn/EventSimpleGUI
-Author: Daniel Coêlho
-Author-email: heromon.9010@gmail.com
-License: MIT license
-Project-URL: Tests, https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/
-Project-URL: Source, https://github.com/MikalROn/EventSimpleGUI
-Project-URL: Demos, https://github.com/MikalROn/EventSimpleGUI/tree/main/demos
-Project-URL: Docs, https://mikalron.github.io/EventSimpleGUI/
-Keywords: eventsimplegui,EventSimpleGUI,simplegui,GUI,gui,events for simplegui,generate events,fast events,events
-Platform: UNKNOWN
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Events For SimpleGui
-
-> Status of project: in progress...
-
-
-<div align="center">
-
-![GitHub](https://img.shields.io/github/license/MikalROn/EventSimpleGUI?style=for-the-badge)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eventsimplegui?style=for-the-badge)
-<a href="https://github.com/MikalROn/EventSimpleGUI">
-<img alt="GitHub" src="https://img.shields.io/badge/Github-Open%20source-green?style=for-the-badge&amp;logo=github"/>
-</a>
-<a href="https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/">
-<img alt="Conv100%" src="https://img.shields.io/badge/coverage-100%25-green?style=for-the-badge">
-</a>
-</div>
-
-<em>This project has the intention to make easier, scalable and readable events on PySimpleGUI</em>
-
-## Download
-
-<p>Download from PyPi</p>
-
-````shell
-$pip install EventSimpleGUI
-````
-
-## Demonstration
-
-<h3> Creating an event function </h3>
-
-<p>Using the decorator event to run an event, you can pass the element key as an argument for decorator, when the event 
-is called, function is going to be called two</p>
-
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-@loop.event('_click')
-def when_btn_was_clicked(*ags):
-    print('Just a normal event')
-
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window)
-````
-Events can be passed as an argument of run window like in the exemple
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-
-def when_btn_was_clicked(*args):
-    event, _, _ = args
-    if event == '_click':
-        print('Just a normal event')
-
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window, when_btn_was_clicked)
-````
-And can also pass an event using add_event
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-
-def when_btn_was_clicked(*args):
-    event, _, _ = args
-    if event == '_click':
-        print('Just a normal event')
-
-loop.add_event(when_btn_was_clicked)
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window)
-````
-
-## Events
-
-<p> You can use a sting or list of keys to trigger your events </p>
-
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-
-loop = EventSimpleGUI()
-
-keys = ['_click', '_click1']
-@loop.event(keys)
-def when_btn_was_clicked(*args):
-    print('Just a normal event')
-
-
-layout = [
-    [sg.B(f'{"Just a button":54}', key='_click')],
-    [sg.B(f'{"Just another button":50}', key='_click1')]
-]
-window = sg.Window('Just a Window.', layout, scaling=1.5)
-if __name__ == '__main__':
-    loop.run_window(window, window_log=True)
-````
-<div>
-
-
-#### Change log 0.2.7
-
-- Tests are implemented 97% cov
-- Close event replaced to the end of loop
-
-####  Change log 0.2.5
-
-- Now events can return values on Values dict
-
-</div>
-
-
-
-
+Metadata-Version: 2.1
+Name: EventSimpleGUI
+Version: 0.3.1
+Summary: A simple tool to create events to PySimpleGUI
+Home-page: https://github.com/MikalROn/EventSimpleGUI
+Author: Daniel Coêlho
+Author-email: heromon.9010@gmail.com
+License: MIT license
+Project-URL: Tests, https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/
+Project-URL: Source, https://github.com/MikalROn/EventSimpleGUI
+Project-URL: Demos, https://github.com/MikalROn/EventSimpleGUI/tree/main/demos
+Project-URL: Docs, https://mikalron.github.io/EventSimpleGUI/
+Keywords: eventsimplegui,EventSimpleGUI,simplegui,GUI,gui,events for simplegui,event handler simple gui,generate events,fast events,events
+Platform: UNKNOWN
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Events For SimpleGui
+
+> Status of project: in progress...
+
+
+<div align="center">
+
+![GitHub](https://img.shields.io/github/license/MikalROn/EventSimpleGUI?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eventsimplegui?style=for-the-badge)
+<a href="https://github.com/MikalROn/EventSimpleGUI">
+<img alt="GitHub" src="https://img.shields.io/badge/Github-Open%20source-green?style=for-the-badge&amp;logo=github"/>
+</a>
+<a href="https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/">
+<img alt="Conv100%" src="https://img.shields.io/badge/coverage-100%25-green?style=for-the-badge">
+</a>
+</div>
+
+<em>This project has the intention to make easier, scalable and readable events on PySimpleGUI</em>
+
+## Download
+
+<p>Download from PyPi</p>
+
+````shell
+$pip install EventSimpleGUI
+````
+
+## Demonstration
+
+<h3> Creating an event function </h3>
+
+<p>Using the decorator event to run an event, you can pass the element key as an argument for decorator, when the event 
+is called, function is going to be called two</p>
+
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+@loop.event('_click')
+def when_btn_was_clicked(*ags):
+    print('Just a normal event')
+
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window)
+````
+Events can be passed as an argument of run window like in the exemple
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+
+def when_btn_was_clicked(*args):
+    event, _, _ = args
+    if event == '_click':
+        print('Just a normal event')
+
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window, when_btn_was_clicked)
+````
+And can also pass an event using add_event
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+
+def when_btn_was_clicked(*args):
+    event, _, _ = args
+    if event == '_click':
+        print('Just a normal event')
+
+loop.add_event(when_btn_was_clicked)
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window)
+````
+
+## Events
+
+<p> You can use a sting or list of keys to trigger your events </p>
+
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+
+loop = EventSimpleGUI()
+
+keys = ['_click', '_click1']
+@loop.event(keys)
+def when_btn_was_clicked(*args):
+    print('Just a normal event')
+
+
+layout = [
+    [sg.B(f'{"Just a button":54}', key='_click')],
+    [sg.B(f'{"Just another button":50}', key='_click1')]
+]
+window = sg.Window('Just a Window.', layout, scaling=1.5)
+if __name__ == '__main__':
+    loop.run_window(window, window_log=True)
+````
+<div>
+
+
+#### Change log 0.2.7
+
+- Tests are implemented 97% cov
+- Close event replaced to the end of loop
+
+####  Change log 0.2.5
+
+- Now events can return values on Values dict
+
+</div>
+
+
+
+
```

### Comparing `EventSimpleGUI-0.3.0/LICENCE` & `EventSimpleGUI-0.3.1/LICENCE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Daniel Mendonça
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Daniel Mendonça
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `EventSimpleGUI-0.3.0/PKG-INFO` & `EventSimpleGUI-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-Metadata-Version: 2.1
-Name: EventSimpleGUI
-Version: 0.3.0
-Summary: A simple tool to create events to PySimpleGUI
-Home-page: https://github.com/MikalROn/EventSimpleGUI
-Author: Daniel Coêlho
-Author-email: heromon.9010@gmail.com
-License: MIT license
-Project-URL: Tests, https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/
-Project-URL: Source, https://github.com/MikalROn/EventSimpleGUI
-Project-URL: Demos, https://github.com/MikalROn/EventSimpleGUI/tree/main/demos
-Project-URL: Docs, https://mikalron.github.io/EventSimpleGUI/
-Keywords: eventsimplegui,EventSimpleGUI,simplegui,GUI,gui,events for simplegui,generate events,fast events,events
-Platform: UNKNOWN
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Events For SimpleGui
-
-> Status of project: in progress...
-
-
-<div align="center">
-
-![GitHub](https://img.shields.io/github/license/MikalROn/EventSimpleGUI?style=for-the-badge)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eventsimplegui?style=for-the-badge)
-<a href="https://github.com/MikalROn/EventSimpleGUI">
-<img alt="GitHub" src="https://img.shields.io/badge/Github-Open%20source-green?style=for-the-badge&amp;logo=github"/>
-</a>
-<a href="https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/">
-<img alt="Conv100%" src="https://img.shields.io/badge/coverage-100%25-green?style=for-the-badge">
-</a>
-</div>
-
-<em>This project has the intention to make easier, scalable and readable events on PySimpleGUI</em>
-
-## Download
-
-<p>Download from PyPi</p>
-
-````shell
-$pip install EventSimpleGUI
-````
-
-## Demonstration
-
-<h3> Creating an event function </h3>
-
-<p>Using the decorator event to run an event, you can pass the element key as an argument for decorator, when the event 
-is called, function is going to be called two</p>
-
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-@loop.event('_click')
-def when_btn_was_clicked(*ags):
-    print('Just a normal event')
-
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window)
-````
-Events can be passed as an argument of run window like in the exemple
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-
-def when_btn_was_clicked(*args):
-    event, _, _ = args
-    if event == '_click':
-        print('Just a normal event')
-
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window, when_btn_was_clicked)
-````
-And can also pass an event using add_event
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-
-def when_btn_was_clicked(*args):
-    event, _, _ = args
-    if event == '_click':
-        print('Just a normal event')
-
-loop.add_event(when_btn_was_clicked)
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window)
-````
-
-## Events
-
-<p> You can use a sting or list of keys to trigger your events </p>
-
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-
-loop = EventSimpleGUI()
-
-keys = ['_click', '_click1']
-@loop.event(keys)
-def when_btn_was_clicked(*args):
-    print('Just a normal event')
-
-
-layout = [
-    [sg.B(f'{"Just a button":54}', key='_click')],
-    [sg.B(f'{"Just another button":50}', key='_click1')]
-]
-window = sg.Window('Just a Window.', layout, scaling=1.5)
-if __name__ == '__main__':
-    loop.run_window(window, window_log=True)
-````
-<div>
-
-
-#### Change log 0.2.7
-
-- Tests are implemented 97% cov
-- Close event replaced to the end of loop
-
-####  Change log 0.2.5
-
-- Now events can return values on Values dict
-
-</div>
-
-
-
-
+Metadata-Version: 2.1
+Name: EventSimpleGUI
+Version: 0.3.1
+Summary: A simple tool to create events to PySimpleGUI
+Home-page: https://github.com/MikalROn/EventSimpleGUI
+Author: Daniel Coêlho
+Author-email: heromon.9010@gmail.com
+License: MIT license
+Project-URL: Tests, https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/
+Project-URL: Source, https://github.com/MikalROn/EventSimpleGUI
+Project-URL: Demos, https://github.com/MikalROn/EventSimpleGUI/tree/main/demos
+Project-URL: Docs, https://mikalron.github.io/EventSimpleGUI/
+Keywords: eventsimplegui,EventSimpleGUI,simplegui,GUI,gui,events for simplegui,event handler simple gui,generate events,fast events,events
+Platform: UNKNOWN
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Events For SimpleGui
+
+> Status of project: in progress...
+
+
+<div align="center">
+
+![GitHub](https://img.shields.io/github/license/MikalROn/EventSimpleGUI?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eventsimplegui?style=for-the-badge)
+<a href="https://github.com/MikalROn/EventSimpleGUI">
+<img alt="GitHub" src="https://img.shields.io/badge/Github-Open%20source-green?style=for-the-badge&amp;logo=github"/>
+</a>
+<a href="https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/">
+<img alt="Conv100%" src="https://img.shields.io/badge/coverage-100%25-green?style=for-the-badge">
+</a>
+</div>
+
+<em>This project has the intention to make easier, scalable and readable events on PySimpleGUI</em>
+
+## Download
+
+<p>Download from PyPi</p>
+
+````shell
+$pip install EventSimpleGUI
+````
+
+## Demonstration
+
+<h3> Creating an event function </h3>
+
+<p>Using the decorator event to run an event, you can pass the element key as an argument for decorator, when the event 
+is called, function is going to be called two</p>
+
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+@loop.event('_click')
+def when_btn_was_clicked(*ags):
+    print('Just a normal event')
+
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window)
+````
+Events can be passed as an argument of run window like in the exemple
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+
+def when_btn_was_clicked(*args):
+    event, _, _ = args
+    if event == '_click':
+        print('Just a normal event')
+
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window, when_btn_was_clicked)
+````
+And can also pass an event using add_event
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+
+def when_btn_was_clicked(*args):
+    event, _, _ = args
+    if event == '_click':
+        print('Just a normal event')
+
+loop.add_event(when_btn_was_clicked)
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window)
+````
+
+## Events
+
+<p> You can use a sting or list of keys to trigger your events </p>
+
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+
+loop = EventSimpleGUI()
+
+keys = ['_click', '_click1']
+@loop.event(keys)
+def when_btn_was_clicked(*args):
+    print('Just a normal event')
+
+
+layout = [
+    [sg.B(f'{"Just a button":54}', key='_click')],
+    [sg.B(f'{"Just another button":50}', key='_click1')]
+]
+window = sg.Window('Just a Window.', layout, scaling=1.5)
+if __name__ == '__main__':
+    loop.run_window(window, window_log=True)
+````
+<div>
+
+
+#### Change log 0.2.7
+
+- Tests are implemented 97% cov
+- Close event replaced to the end of loop
+
+####  Change log 0.2.5
+
+- Now events can return values on Values dict
+
+</div>
+
+
+
+
```

### Comparing `EventSimpleGUI-0.3.0/README.md` & `EventSimpleGUI-0.3.1/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# Events For SimpleGui
-
-> Status of project: in progress...
-
-
-<div align="center">
-
-![GitHub](https://img.shields.io/github/license/MikalROn/EventSimpleGUI?style=for-the-badge)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eventsimplegui?style=for-the-badge)
-<a href="https://github.com/MikalROn/EventSimpleGUI">
-<img alt="GitHub" src="https://img.shields.io/badge/Github-Open%20source-green?style=for-the-badge&amp;logo=github"/>
-</a>
-<a href="https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/">
-<img alt="Conv100%" src="https://img.shields.io/badge/coverage-100%25-green?style=for-the-badge">
-</a>
-</div>
-
-<em>This project has the intention to make easier, scalable and readable events on PySimpleGUI</em>
-
-## Download
-
-<p>Download from PyPi</p>
-
-````shell
-$pip install EventSimpleGUI
-````
-
-## Demonstration
-
-<h3> Creating an event function </h3>
-
-<p>Using the decorator event to run an event, you can pass the element key as an argument for decorator, when the event 
-is called, function is going to be called two</p>
-
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-@loop.event('_click')
-def when_btn_was_clicked(*ags):
-    print('Just a normal event')
-
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window)
-````
-Events can be passed as an argument of run window like in the exemple
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-
-def when_btn_was_clicked(*args):
-    event, _, _ = args
-    if event == '_click':
-        print('Just a normal event')
-
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window, when_btn_was_clicked)
-````
-And can also pass an event using add_event
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-loop = EventSimpleGUI()
-
-
-
-def when_btn_was_clicked(*args):
-    event, _, _ = args
-    if event == '_click':
-        print('Just a normal event')
-
-loop.add_event(when_btn_was_clicked)
-layout = [[sg.B('Just a button', key='_click')]]
-window = sg.Window('Just a Window.', layout)
-
-if __name__ == '__main__':
-    loop.run_window(window)
-````
-
-## Events
-
-<p> You can use a sting or list of keys to trigger your events </p>
-
-````python
-from pysimpleevent import EventSimpleGUI
-import PySimpleGUI as sg
-
-
-loop = EventSimpleGUI()
-
-keys = ['_click', '_click1']
-@loop.event(keys)
-def when_btn_was_clicked(*args):
-    print('Just a normal event')
-
-
-layout = [
-    [sg.B(f'{"Just a button":54}', key='_click')],
-    [sg.B(f'{"Just another button":50}', key='_click1')]
-]
-window = sg.Window('Just a Window.', layout, scaling=1.5)
-if __name__ == '__main__':
-    loop.run_window(window, window_log=True)
-````
-<div>
-
-
-#### Change log 0.2.7
-
-- Tests are implemented 97% cov
-- Close event replaced to the end of loop
-
-####  Change log 0.2.5
-
-- Now events can return values on Values dict
-
-</div>
-
-
+# Events For SimpleGui
+
+> Status of project: in progress...
+
+
+<div align="center">
+
+![GitHub](https://img.shields.io/github/license/MikalROn/EventSimpleGUI?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eventsimplegui?style=for-the-badge)
+<a href="https://github.com/MikalROn/EventSimpleGUI">
+<img alt="GitHub" src="https://img.shields.io/badge/Github-Open%20source-green?style=for-the-badge&amp;logo=github"/>
+</a>
+<a href="https://smokeshow.helpmanual.io/474z2x1c0s2u3j101i26/">
+<img alt="Conv100%" src="https://img.shields.io/badge/coverage-100%25-green?style=for-the-badge">
+</a>
+</div>
+
+<em>This project has the intention to make easier, scalable and readable events on PySimpleGUI</em>
+
+## Download
+
+<p>Download from PyPi</p>
+
+````shell
+$pip install EventSimpleGUI
+````
+
+## Demonstration
+
+<h3> Creating an event function </h3>
+
+<p>Using the decorator event to run an event, you can pass the element key as an argument for decorator, when the event 
+is called, function is going to be called two</p>
+
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+@loop.event('_click')
+def when_btn_was_clicked(*ags):
+    print('Just a normal event')
+
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window)
+````
+Events can be passed as an argument of run window like in the exemple
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+
+def when_btn_was_clicked(*args):
+    event, _, _ = args
+    if event == '_click':
+        print('Just a normal event')
+
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window, when_btn_was_clicked)
+````
+And can also pass an event using add_event
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+loop = EventSimpleGUI()
+
+
+
+def when_btn_was_clicked(*args):
+    event, _, _ = args
+    if event == '_click':
+        print('Just a normal event')
+
+loop.add_event(when_btn_was_clicked)
+layout = [[sg.B('Just a button', key='_click')]]
+window = sg.Window('Just a Window.', layout)
+
+if __name__ == '__main__':
+    loop.run_window(window)
+````
+
+## Events
+
+<p> You can use a sting or list of keys to trigger your events </p>
+
+````python
+from pysimpleevent import EventSimpleGUI
+import PySimpleGUI as sg
+
+
+loop = EventSimpleGUI()
+
+keys = ['_click', '_click1']
+@loop.event(keys)
+def when_btn_was_clicked(*args):
+    print('Just a normal event')
+
+
+layout = [
+    [sg.B(f'{"Just a button":54}', key='_click')],
+    [sg.B(f'{"Just another button":50}', key='_click1')]
+]
+window = sg.Window('Just a Window.', layout, scaling=1.5)
+if __name__ == '__main__':
+    loop.run_window(window, window_log=True)
+````
+<div>
+
+
+#### Change log 0.2.7
+
+- Tests are implemented 97% cov
+- Close event replaced to the end of loop
+
+####  Change log 0.2.5
+
+- Now events can return values on Values dict
+
+</div>
+
+
```

### Comparing `EventSimpleGUI-0.3.0/pysimpleevent/fastevent.py` & `EventSimpleGUI-0.3.1/pysimpleevent/fastevent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,103 @@
-import PySimpleGUI as sg
-
-
-class EventSimpleGUI:
-
-    """ Use this class to start a window and create events  """
-
-    def __init__(self):
-        """ self._events holds all events """
-        self._events = []
-
-    @property
-    def get_events(self) -> list:
-        """ Use this property to get all events, from @event or add_event """
-        return self._events
-
-    def add_event(self, event):
-        """ You can use this method, but it's recomended to use @EventSimpleGUI.event """
-        self._events.append(event)
-
-    def run_window(
-            self, Window: sg.Window, *args, window_log=False, close_event=False, return_values=True, task=None
-    ) -> dict or None:
-        """ Use this method to run PySimpleGUI Windows
-        :param Window:         can be any PySimpleGUI Window
-        :type Window:          PySimpleGUI.Window
-        :arg args:             can be any function that recives (event: str , values: dict, window: PySimpleGUI.Window)
-        :type args:            function
-        :param window_log:     if True prints events and values on the console
-        :type window_log:      bool
-        :param return_values:  if True return values of window.read()
-        :type return_values:   bool
-        :param task:           can be any callable function
-        :param close_event:    a diferent key to close the window
-        """
-        while True:
-
-            event, values = Window.Read()
-
-            # Run task
-            if task:
-                task()
-
-            # Run decorator events
-            for func in self._events:
-                func(event, values, Window)
-
-            # Run args events or functions
-            for arg in args:
-                arg(event, values, Window)
-
-            # Enable log
-            if window_log:
-                print(f'{"Event ->":10}', event)
-                print(f'{"Values ->":10}', values)
-
-            # Close window
-            if event == sg.WIN_CLOSED or event == close_event:
-                break
-
-            # return window on the values
-            values['Window'] = Window
-
-        # Return values of window.read()
-        Window.close()
-
-        if return_values:
-            return values
-
-    def event(self, key: str or list[str]):
-        """ Use this decorator to create events.
-        ::param key:     element key or list of element keys
-        ::type key:      str or list[str]
-
-        Exemple of a simple event:
-
-        app = EventSimpleGUI()
-        @app.event('_CLICK_')
-        def print_when_click(event: str , values: dict, window: PySimpleGUI.Window):
-            print('click!')
-
-        * All events will recive (event: str , values: dict, window: PySimpleGUI.Window)
-        """
-        def decorador(func_event):
-            def empacotador(event: str, values: dict, window: sg.Window):
-                if type(key) == list:
-                    if event in key:
-                        values[func_event.__name__] = func_event(event, values, window)
-                        return values[func_event.__name__]
-
-                elif type(key) == str:
-                    if event == key:
-                        values[func_event.__name__] = func_event(event, values, window)
-                        return values[func_event.__name__]
-            self.add_event(empacotador)
-            return empacotador
-        return decorador
-
-
-
-
-
-
-
+import PySimpleGUI as sg
+
+
+class EventSimpleGUI:
+
+    """ Use this class to start a window and create events  """
+
+    def __init__(self):
+        """ self._events holds all events """
+        self._events = []
+
+    @property
+    def get_events(self) -> list:
+        """ Use this property to get all events, from @event or add_event """
+        return self._events
+
+    def add_event(self, event):
+        """ You can use this method, but it's recomended to use @EventSimpleGUI.event """
+        self._events.append(event)
+
+    def run_window(
+            self, Window: sg.Window, *args, window_log=False, close_event=False, return_values=True, task=None
+    ) -> dict or None:
+        """ Use this method to run PySimpleGUI Windows
+        :param Window:         can be any PySimpleGUI Window
+        :type Window:          PySimpleGUI.Window
+        :arg args:             can be any function that recives (event: str , values: dict, window: PySimpleGUI.Window)
+        :type args:            function
+        :param window_log:     if True prints events and values on the console
+        :type window_log:      bool
+        :param return_values:  if True return values of window.read()
+        :type return_values:   bool
+        :param task:           can be any callable function
+        :param close_event:    a diferent key to close the window
+        """
+        while True:
+
+            event, values = Window.Read()
+
+            # Run task
+            if task:
+                task()
+
+            # Run decorator events
+            for func in self._events:
+                func(event, values, Window)
+
+            # Run args events or functions
+            for arg in args:
+                arg(event, values, Window)
+
+            # Enable log
+            if window_log:
+                print(f'{"Event ->":10}', event)
+                print(f'{"Values ->":10}', values)
+
+            # Close window
+            if event == sg.WIN_CLOSED or event == close_event:
+                break
+
+            # return window on the values
+            values['Window'] = Window
+
+        # Return values of window.read()
+        Window.close()
+
+        if return_values:
+            return values
+
+    def event(self, key: str or list[str]):
+        """ Use this decorator to create events.
+        ::param key:     element key or list of element keys
+        ::type key:      str or list[str]
+
+        Exemple of a simple event:
+
+        app = EventSimpleGUI()
+        @app.event('_CLICK_')
+        def print_when_click(event: str , values: dict, window: PySimpleGUI.Window):
+            print('click!')
+
+        * All events will recive (event: str , values: dict, window: PySimpleGUI.Window)
+        """
+        def decorador(func_event):
+            def empacotador(event: str, values: dict, window: sg.Window):
+                if type(key) == list:
+                    if event in key:
+                        window.write_event_value(f'{func_event.__name__}', func_event(event, values, window))
+                        
+                elif type(key) == str:
+                    if event == key:
+                        window.write_event_value(f'{func_event.__name__}', func_event(event, values, window))
+
+            self.add_event(empacotador)
+            return empacotador
+        return decorador
+
+
+
+
+
+
+
```

