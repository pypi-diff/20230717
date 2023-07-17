# Comparing `tmp/newmod-1.0.tar.gz` & `tmp/newmod-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newmod-1.0.tar", last modified: Mon Jul 17 15:57:00 2023, max compression
+gzip compressed data, was "newmod-2.0.tar", last modified: Mon Jul 17 16:08:10 2023, max compression
```

## Comparing `newmod-1.0.tar` & `newmod-2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 15:56:35.000000 newmod-1.0/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 15:56:35.000000 newmod-1.0/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      732 2023-07-17 15:56:35.000000 newmod-1.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3076 2023-07-17 15:57:00.670308 newmod-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2556 2023-07-17 15:56:35.000000 newmod-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/newmod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3076 2023-07-17 15:57:00.000000 newmod-1.0/newmod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-07-17 15:57:00.000000 newmod-1.0/newmod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:57:00.000000 newmod-1.0/newmod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 15:57:00.000000 newmod-1.0/newmod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 15:57:00.000000 newmod-1.0/newmod.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/pyromod/
--rw-r--r--   0 root         (0) root         (0)      762 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/pyromod/filters/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/filters/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/pyromod/helpers/
--rw-r--r--   0 root         (0) root         (0)      812 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/pyromod/listen/
--rw-r--r--   0 root         (0) root         (0)      816 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4392 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/listen/listen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:57:00.670308 newmod-1.0/pyromod/utils/
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-07-17 15:56:35.000000 newmod-1.0/pyromod/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:57:00.670308 newmod-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      909 2023-07-17 15:56:35.000000 newmod-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.611559 newmod-2.0/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:07:46.000000 newmod-2.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:07:46.000000 newmod-2.0/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:07:46.000000 newmod-2.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-07-17 16:08:10.611559 newmod-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:07:46.000000 newmod-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 16:07:46.000000 newmod-2.0/newmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/filters/
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:07:46.000000 newmod-2.0/newmod/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:07:46.000000 newmod-2.0/newmod/filters/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/helpers/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:07:46.000000 newmod-2.0/newmod/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:07:46.000000 newmod-2.0/newmod/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/listen/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:07:46.000000 newmod-2.0/newmod/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:07:46.000000 newmod-2.0/newmod/listen/listen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/utils/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:07:46.000000 newmod-2.0/newmod/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:07:46.000000 newmod-2.0/newmod/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:08:10.611559 newmod-2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      907 2023-07-17 16:07:46.000000 newmod-2.0/setup.py
```

### Comparing `newmod-1.0/COPYING` & `newmod-2.0/COPYING`

 * *Files identical despite different names*

### Comparing `newmod-1.0/COPYING.lesser` & `newmod-2.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `newmod-1.0/NOTICE` & `newmod-2.0/newmod/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-pyromod - A monkeypatcher add-on for Newgram
-Copyright (C) 2020 Cezar H. <https://github.com/usernein>
-
-This file is part of pyromod.
-
-pyromod is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pyromod is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
+"""
+newmod - A monkeypatcher add-on for Newgram
+Copyright (C) 2020 Cezar H. <https://github.com/usernein>
+
+This file is part of newmod.
+
+newmod is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+newmod is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from .utils import patch, patchable
```

### Comparing `newmod-1.0/PKG-INFO` & `newmod-2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 1.0
+Version: 2.0
 Summary: A monkeypatcher add-on for newgram
-Home-page: https://github.com/jokokendi/pyromod
+Home-page: https://github.com/jokokendi/newmod
 Author: Cezar H.
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
-# pyromod
+# newmod
 A monkeypatcher add-on for Newgram
 
 ## Introduction
-pyromod is a compilation of utils i developed for extend my personal use of Newgram. Then i started to use it and more bots and now i published it to make it easier to be installed in new projects.
+newmod is a compilation of utils i developed for extend my personal use of Newgram. Then i started to use it and more bots and now i published it to make it easier to be installed in new projects.
 It works *together* with newgram, this is *not* a fork nor modded version. It does monkey patching to add features to Newgram classes.
 
 IMPORTANT: you should have installed asyncio newgram.
 
 ## Usage
-Import `pyromod` at least one time in your script, so you'll be able to use modified newgram in all files of the same proccess. Example:
+Import `newmod` at least one time in your script, so you'll be able to use modified newgram in all files of the same proccess. Example:
 ```python
 # config.py
-import pyromod.listen
+import newmod.listen
 from newgram import Client
 
 app = Client('my_session')
 ```
 ```python
 # any other .py
 from config import app
-# no need to import pyromod again, newgram is already monkeypatched globally (at the same proccess)
+# no need to import newmod again, newgram is already monkeypatched globally (at the same proccess)
 ```
 
-I separated the patches between packages to allow you to import only what you want. The `__init__.py` of each package does the monkeypatch automatically as soon as they are imported (except for `pyromod.helpers`, which provides classes and functions that should be explicitely imported).
+I separated the patches between packages to allow you to import only what you want. The `__init__.py` of each package does the monkeypatch automatically as soon as they are imported (except for `newmod.helpers`, which provides classes and functions that should be explicitely imported).
 
-### `pyromod.listen`
+### `newmod.listen`
 Just import it, it will automatically do the monkeypatch and you'll get these new methods:
 - `await newgram.Client.listen(chat_id, filters=None, timeout=30)`
 Awaits for a new message in the specified chat and returns it
 You can pass Update Filters to the filters parameter just like you do for the update handlers. e.g. `filters=filters.photo & filters.bot`
 
 - `await newgram.Client.ask(text, chat_id, filters=None, timeout=30)`
 Same of `.listen()` above, but sends a message before awaiting
 You can pass custom parameters to its send_message() call. Check the example below.
 
 - The bound methods `Chat.listen`, `User.listen`, `Chat.ask` and `User.ask`
 
 Example:
 ```python
-from pyromod import listen # or import pyromod.listen
+from newmod import listen # or import newmod.listen
 from newgram import Client
 client = Client(...)
 ...
     answer = await client.ask(chat_id, '*Send me your name:*', parse_mode='Markdown')
     await client.send_message(chat_id, f'Your name is: {answer.text}')    
 ```
 
-### `pyromod.filters`
+### `newmod.filters`
 Import it and the following Update Filters will be monkeypatched to `newgram.filters`:
 
 - `filters.dice`
 A dice message.
 
 ### Copyright & License
 This project may include snippets of Newgram code
```

### Comparing `newmod-1.0/README.md` & `newmod-2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# pyromod
+# newmod
 A monkeypatcher add-on for Newgram
 
 ## Introduction
-pyromod is a compilation of utils i developed for extend my personal use of Newgram. Then i started to use it and more bots and now i published it to make it easier to be installed in new projects.
+newmod is a compilation of utils i developed for extend my personal use of Newgram. Then i started to use it and more bots and now i published it to make it easier to be installed in new projects.
 It works *together* with newgram, this is *not* a fork nor modded version. It does monkey patching to add features to Newgram classes.
 
 IMPORTANT: you should have installed asyncio newgram.
 
 ## Usage
-Import `pyromod` at least one time in your script, so you'll be able to use modified newgram in all files of the same proccess. Example:
+Import `newmod` at least one time in your script, so you'll be able to use modified newgram in all files of the same proccess. Example:
 ```python
 # config.py
-import pyromod.listen
+import newmod.listen
 from newgram import Client
 
 app = Client('my_session')
 ```
 ```python
 # any other .py
 from config import app
-# no need to import pyromod again, newgram is already monkeypatched globally (at the same proccess)
+# no need to import newmod again, newgram is already monkeypatched globally (at the same proccess)
 ```
 
-I separated the patches between packages to allow you to import only what you want. The `__init__.py` of each package does the monkeypatch automatically as soon as they are imported (except for `pyromod.helpers`, which provides classes and functions that should be explicitely imported).
+I separated the patches between packages to allow you to import only what you want. The `__init__.py` of each package does the monkeypatch automatically as soon as they are imported (except for `newmod.helpers`, which provides classes and functions that should be explicitely imported).
 
-### `pyromod.listen`
+### `newmod.listen`
 Just import it, it will automatically do the monkeypatch and you'll get these new methods:
 - `await newgram.Client.listen(chat_id, filters=None, timeout=30)`
 Awaits for a new message in the specified chat and returns it
 You can pass Update Filters to the filters parameter just like you do for the update handlers. e.g. `filters=filters.photo & filters.bot`
 
 - `await newgram.Client.ask(text, chat_id, filters=None, timeout=30)`
 Same of `.listen()` above, but sends a message before awaiting
 You can pass custom parameters to its send_message() call. Check the example below.
 
 - The bound methods `Chat.listen`, `User.listen`, `Chat.ask` and `User.ask`
 
 Example:
 ```python
-from pyromod import listen # or import pyromod.listen
+from newmod import listen # or import newmod.listen
 from newgram import Client
 client = Client(...)
 ...
     answer = await client.ask(chat_id, '*Send me your name:*', parse_mode='Markdown')
     await client.send_message(chat_id, f'Your name is: {answer.text}')    
 ```
 
-### `pyromod.filters`
+### `newmod.filters`
 Import it and the following Update Filters will be monkeypatched to `newgram.filters`:
 
 - `filters.dice`
 A dice message.
 
 ### Copyright & License
 This project may include snippets of Newgram code
```

### Comparing `newmod-1.0/newmod.egg-info/PKG-INFO` & `newmod-2.0/newmod.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 1.0
+Version: 2.0
 Summary: A monkeypatcher add-on for newgram
-Home-page: https://github.com/jokokendi/pyromod
+Home-page: https://github.com/jokokendi/newmod
 Author: Cezar H.
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
-# pyromod
+# newmod
 A monkeypatcher add-on for Newgram
 
 ## Introduction
-pyromod is a compilation of utils i developed for extend my personal use of Newgram. Then i started to use it and more bots and now i published it to make it easier to be installed in new projects.
+newmod is a compilation of utils i developed for extend my personal use of Newgram. Then i started to use it and more bots and now i published it to make it easier to be installed in new projects.
 It works *together* with newgram, this is *not* a fork nor modded version. It does monkey patching to add features to Newgram classes.
 
 IMPORTANT: you should have installed asyncio newgram.
 
 ## Usage
-Import `pyromod` at least one time in your script, so you'll be able to use modified newgram in all files of the same proccess. Example:
+Import `newmod` at least one time in your script, so you'll be able to use modified newgram in all files of the same proccess. Example:
 ```python
 # config.py
-import pyromod.listen
+import newmod.listen
 from newgram import Client
 
 app = Client('my_session')
 ```
 ```python
 # any other .py
 from config import app
-# no need to import pyromod again, newgram is already monkeypatched globally (at the same proccess)
+# no need to import newmod again, newgram is already monkeypatched globally (at the same proccess)
 ```
 
-I separated the patches between packages to allow you to import only what you want. The `__init__.py` of each package does the monkeypatch automatically as soon as they are imported (except for `pyromod.helpers`, which provides classes and functions that should be explicitely imported).
+I separated the patches between packages to allow you to import only what you want. The `__init__.py` of each package does the monkeypatch automatically as soon as they are imported (except for `newmod.helpers`, which provides classes and functions that should be explicitely imported).
 
-### `pyromod.listen`
+### `newmod.listen`
 Just import it, it will automatically do the monkeypatch and you'll get these new methods:
 - `await newgram.Client.listen(chat_id, filters=None, timeout=30)`
 Awaits for a new message in the specified chat and returns it
 You can pass Update Filters to the filters parameter just like you do for the update handlers. e.g. `filters=filters.photo & filters.bot`
 
 - `await newgram.Client.ask(text, chat_id, filters=None, timeout=30)`
 Same of `.listen()` above, but sends a message before awaiting
 You can pass custom parameters to its send_message() call. Check the example below.
 
 - The bound methods `Chat.listen`, `User.listen`, `Chat.ask` and `User.ask`
 
 Example:
 ```python
-from pyromod import listen # or import pyromod.listen
+from newmod import listen # or import newmod.listen
 from newgram import Client
 client = Client(...)
 ...
     answer = await client.ask(chat_id, '*Send me your name:*', parse_mode='Markdown')
     await client.send_message(chat_id, f'Your name is: {answer.text}')    
 ```
 
-### `pyromod.filters`
+### `newmod.filters`
 Import it and the following Update Filters will be monkeypatched to `newgram.filters`:
 
 - `filters.dice`
 A dice message.
 
 ### Copyright & License
 This project may include snippets of Newgram code
```

### Comparing `newmod-1.0/pyromod/__init__.py` & `newmod-2.0/newmod/listen/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-pyromod - A monkeypatched add-on for Newgram
-Copyright (C) 2020 Cezar H. <https://github.com/usernein>
-
-This file is part of pyromod.
-
-pyromod is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pyromod is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-__version__ = "1.0"
+"""
+newmod - A monkeypatcher add-on for Newgram
+Copyright (C) 2020 Cezar H. <https://github.com/usernein>
+
+This file is part of newmod.
+
+newmod is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+newmod is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from .listen import Client, MessageHandler, Chat, User
```

### Comparing `newmod-1.0/pyromod/filters/__init__.py` & `newmod-2.0/newmod/filters/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-pyromod - A monkeypatcher add-on for Newgram
+newmod - A monkeypatcher add-on for Newgram
 Copyright (C) 2020 Cezar H. <https://github.com/usernein>
 
-This file is part of pyromod.
+This file is part of newmod.
 
-pyromod is free software: you can redistribute it and/or modify
+newmod is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-pyromod is distributed in the hope that it will be useful,
+newmod is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from .filters import dice
```

### Comparing `newmod-1.0/pyromod/filters/filters.py` & `newmod-2.0/newmod/filters/filters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-pyromod - A monkeypatcher add-on for Newgram
+newmod - A monkeypatcher add-on for Newgram
 Copyright (C) 2020 Cezar H. <https://github.com/usernein>
 
-This file is part of pyromod.
+This file is part of newmod.
 
-pyromod is free software: you can redistribute it and/or modify
+newmod is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-pyromod is distributed in the hope that it will be useful,
+newmod is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import newgram 
 
 def dice(ctx, message):
     return hasattr(message, 'dice') and message.dice
 newgram.filters.dice = dice
```

### Comparing `newmod-1.0/pyromod/helpers/__init__.py` & `newmod-2.0/newmod/helpers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-pyromod - A monkeypatcher add-on for Newgram
+newmod - A monkeypatcher add-on for Newgram
 Copyright (C) 2020 Cezar H. <https://github.com/usernein>
 
-This file is part of pyromod.
+This file is part of newmod.
 
-pyromod is free software: you can redistribute it and/or modify
+newmod is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-pyromod is distributed in the hope that it will be useful,
+newmod is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 from .helpers import ikb, btn, kb, kbtn, array_chunk
```

### Comparing `newmod-1.0/pyromod/helpers/helpers.py` & `newmod-2.0/newmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `newmod-1.0/pyromod/listen/__init__.py` & `newmod-2.0/NOTICE`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-"""
-pyromod - A monkeypatcher add-on for Newgram
-Copyright (C) 2020 Cezar H. <https://github.com/usernein>
-
-This file is part of pyromod.
-
-pyromod is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pyromod is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from .listen import Client, MessageHandler, Chat, User
+newmod - A monkeypatcher add-on for Newgram
+Copyright (C) 2020 Cezar H. <https://github.com/usernein>
+
+This file is part of newmod.
+
+newmod is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+newmod is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `newmod-1.0/pyromod/listen/listen.py` & `newmod-2.0/newmod/listen/listen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-pyromod - A monkeypatcher add-on for Newgram
+newmod - A monkeypatcher add-on for Newgram
 Copyright (C) 2020 Cezar H. <https://github.com/usernein>
 
-This file is part of pyromod.
+This file is part of newmod.
 
-pyromod is free software: you can redistribute it and/or modify
+newmod is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-pyromod is distributed in the hope that it will be useful,
+newmod is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with pyromod.  If not, see <https://www.gnu.org/licenses/>.
+along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import asyncio
 import functools
 import newgram
 
 from ..utils import patch, patchable
```

### Comparing `newmod-1.0/setup.py` & `newmod-2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
     
 with open('requirements.txt') as fp:
     requirements = [line.strip() for line in fp]
 
-with open('pyromod/__init__.py') as fp:
+with open('newmod/__init__.py') as fp:
     version = re.search('__version__ = "(.+?)"', fp.read())[1]
 
 
 setuptools.setup(
     name="newmod",
     version=version,
     author="Cezar H.",
     license="LGPLv3+",
     description="A monkeypatcher add-on for newgram",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/jokokendi/pyromod",
+    url="https://github.com/jokokendi/newmod",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

