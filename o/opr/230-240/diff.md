# Comparing `tmp/opr-230.tar.gz` & `tmp/opr-240.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-230.tar", last modified: Thu Jul  6 00:56:23 2023, max compression
+gzip compressed data, was "opr-240.tar", last modified: Mon Jul 17 05:58:43 2023, max compression
```

## Comparing `opr-230.tar` & `opr-240.tar`

### file list

```diff
@@ -1,36 +1,55 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.530040 opr-230/
--rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-06 00:56:23.530040 opr-230/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1923 2023-07-04 14:13:27.000000 opr-230/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.526040 opr-230/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     6288 2023-07-05 21:49:59.000000 opr-230/bin/opr
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.526040 opr-230/opr/
--rw-r--r--   0 bart      (1000) bart      (1000)     1914 2023-07-04 11:49:32.000000 opr-230/opr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)    10722 2023-07-06 00:51:15.000000 opr-230/opr/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      535 2023-07-03 12:35:01.000000 opr-230/opr/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.530040 opr-230/opr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      361 2023-07-04 13:24:11.000000 opr-230/opr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      937 2023-07-03 11:41:20.000000 opr-230/opr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20964 2023-07-05 19:45:40.000000 opr-230/opr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-07-03 00:19:09.000000 opr-230/opr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4225 2023-07-03 11:59:03.000000 opr-230/opr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17831 2023-07-05 10:51:26.000000 opr-230/opr/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2354 2023-07-01 05:55:02.000000 opr-230/opr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     8151 2023-07-05 10:51:10.000000 opr-230/opr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1039 2023-07-03 00:19:36.000000 opr-230/opr/modules/shp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1065 2023-07-03 00:20:30.000000 opr-230/opr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2934 2023-07-03 11:58:30.000000 opr-230/opr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5691 2023-07-01 05:55:02.000000 opr-230/opr/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7012 2023-07-04 11:52:44.000000 opr-230/opr/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5121 2023-07-03 14:25:17.000000 opr-230/opr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1429 2023-07-03 12:41:32.000000 opr-230/opr/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2372 2023-07-03 12:33:25.000000 opr-230/opr/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1978 2023-07-03 12:42:29.000000 opr-230/opr/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.530040 opr-230/opr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      530 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     1025 2023-07-06 00:55:50.000000 opr-230/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-06 00:56:23.530040 opr-230/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-01 10:59:30.000000 opr-230/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2593 2023-07-17 05:58:43.156785 opr-240/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     2029 2023-07-15 21:11:27.000000 opr-240/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.152785 opr-240/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1990 2023-07-17 04:56:56.000000 opr-240/bin/opr
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.152785 opr-240/opr/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1725 2023-07-17 04:55:54.000000 opr-240/opr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1021 2023-07-17 04:55:54.000000 opr-240/opr/brokers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1952 2023-07-17 04:55:54.000000 opr-240/opr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      284 2023-07-17 04:55:54.000000 opr-240/opr/configs.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      938 2023-07-17 04:55:54.000000 opr-240/opr/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1558 2023-07-17 04:55:54.000000 opr-240/opr/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1248 2023-07-17 04:55:54.000000 opr-240/opr/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1158 2023-07-17 04:55:54.000000 opr-240/opr/evented.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      353 2023-07-17 04:55:54.000000 opr-240/opr/locking.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      802 2023-07-17 04:55:54.000000 opr-240/opr/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/opr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-07-17 04:56:00.000000 opr-240/opr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3528 2023-07-17 04:56:00.000000 opr-240/opr/modules/bsc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    19192 2023-07-17 04:56:00.000000 opr-240/opr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      829 2023-07-17 04:56:00.000000 opr-240/opr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4057 2023-07-17 04:56:00.000000 opr-240/opr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17641 2023-07-17 04:56:00.000000 opr-240/opr/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2401 2023-07-17 04:56:00.000000 opr-240/opr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7441 2023-07-17 04:56:00.000000 opr-240/opr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1036 2023-07-17 04:56:00.000000 opr-240/opr/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      998 2023-07-17 04:56:00.000000 opr-240/opr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2664 2023-07-17 04:56:00.000000 opr-240/opr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5754 2023-07-17 04:56:00.000000 opr-240/opr/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1009 2023-07-17 04:56:00.000000 opr-240/opr/modules/wsh.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5069 2023-07-17 04:55:54.000000 opr-240/opr/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1297 2023-07-17 04:55:54.000000 opr-240/opr/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4332 2023-07-17 04:55:54.000000 opr-240/opr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2174 2023-07-17 04:55:54.000000 opr-240/opr/reactor.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-07-17 04:55:54.000000 opr-240/opr/recurse.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1246 2023-07-17 04:55:54.000000 opr-240/opr/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1873 2023-07-17 04:55:54.000000 opr-240/opr/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2153 2023-07-17 04:55:54.000000 opr-240/opr/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/opr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2593 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      848 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     1131 2023-07-15 21:11:01.000000 opr-240/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-17 05:58:43.156785 opr-240/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      206 2023-07-15 21:11:56.000000 opr-240/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/test/
+-rw-r--r--   0 bart      (1000) bart      (1000)      748 2023-07-15 21:13:01.000000 opr-240/test/test_composite.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      504 2023-07-15 21:13:12.000000 opr-240/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      463 2023-07-15 21:13:25.000000 opr-240/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1009 2023-07-15 21:13:43.000000 opr-240/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4414 2023-07-15 21:14:03.000000 opr-240/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      427 2023-07-15 21:14:15.000000 opr-240/test/test_parse.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      670 2023-07-15 21:14:39.000000 opr-240/test/test_recursive.py
```

### Comparing `opr-230/PKG-INFO` & `opr-240/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 230
+Version: 240
 Summary: Object Programming Runtime
 Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
+# This file is placed in the Public Domain.
+#
+# __author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 NAME
 
 ::
 
    OPR - Object Programming Runtime
```

### Comparing `opr-230/README.rst` & `opr-240/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is placed in the Public Domain.
+#
+# __author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 NAME
 
 ::
 
    OPR - Object Programming Runtime
```

### Comparing `opr-230/bin/opr` & `opr-240/opr/modules/rss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,279 +1,305 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=E0001
+# pylint: disable=C,I,R,W0401
 
 
-"object programming runtime"
+"rich site syndicte"
 
 
-# IMPORTS
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
-import io
-import os
-import readline
-import sys
-import termios
+import html.parser
+import re
 import threading
 import time
-import traceback
+import urllib
+import _thread
 
 
-sys.path.insert(0, os.getcwd())
-
-
-from opr.handler import Bus, Cfg, Commands, Errors, Event, Handler
-from opr.handler import command, parse_cli, scanstr, waiter
-from opr.loggers import Logging
-from opr.objects import Default, Object, keys, kind, prt, update
-from opr.persist import Persist
-from opr.threads import launch, name
-from opr.utility import elapsed, spl
-
-
-import opr.modules
-
-
-# DEFINES
-
-
-DATE = time.ctime(time.time()).replace("  ", " ")
-NAME = sys.argv[0].split(os.sep)[-1]
-STARTTIME = time.time()
-
-
-Persist.workdir = os.path.expanduser(f"~/.{NAME}")
-
-
-# CLASSES
-
-
-class CLI(Handler):
-
-    "command line interface"
-
-    def announce(self, txt):
-        "annouce text"
-
-    def raw(self, txt):
-        "print text"
-        print(txt)
-
-
-class Console(CLI):
-
-    "cli in a loop"
-
-    def handle(self, evt):
-        "wait for events"
-        CLI.handle(self, evt)
-        evt.wait()
-
-    def poll(self):
-        "echo prompt"
-        return self.event(input("> "))
-
-
-# UTILITY
-
-
-def banner():
-    "print banner"
-    print(f"{NAME.upper()} started {DATE}")
-    sys.stdout.flush()
-
-
-def daemon():
-    "fork to the background"
-    pid = os.fork()
-    print(f"forking {pid}")
-    if pid:
-        os._exit(0)
-    #os.setsid()
-    os.umask(0)
-    with open('/dev/null', 'r', encoding="utf-8") as sis:
-        os.dup2(sis.fileno(), sys.stdin.fileno())
-    with open('/dev/null', 'a+', encoding="utf-8") as sos:
-        os.dup2(sos.fileno(), sys.stdout.fileno())
-    with open('/dev/null', 'a+', encoding="utf-8") as ses:
-        os.dup2(ses.fileno(), sys.stderr.fileno())
-
-
-def wrap(func):
-    "wrap function"
-    fds = sys.stdin.fileno()
-    gotterm = True
+from urllib.error import HTTPError, URLError
+from urllib.parse import quote_plus, urlencode
+from urllib.request import Request, urlopen
+
+
+from .. import Broker, Cfg, Object, Repeater
+from .. import find, fntime, laps, prt, update, write
+from .. import launch, last, spl
+
+
+def start():
+    time.sleep(15.0)
+    fetcher = Fetcher()
+    fetcher.start()
+    return fetcher
+
+
+fetchlock = _thread.allocate_lock()
+
+
+class Feed(Object):
+
+    def len(self):
+        return len(self.__dict__)
+
+    def size(self):
+        return len(self.__dict__)
+
+
+class Rss(Object):
+
+    def __init__(self):
+        super().__init__()
+        self.display_list = 'title,link,author'
+        self.name = ''
+        self.rss = ''
+
+    def len(self):
+        return len(self.__dict__)
+
+    def size(self):
+        return len(self.__dict__)
+
+
+class Seen(Object):
+
+    def __init__(self):
+        super().__init__()
+        self.urls = []
+
+    def len(self):
+        return len(self.__dict__)
+
+    def size(self):
+        return len(self.__dict__)
+
+
+class Fetcher(Object):
+
+    dosave = False
+    seen = Seen()
+
+    def __init__(self):
+        super().__init__()
+        self.connected = threading.Event()
+
+    @staticmethod
+    def display(obj):
+        result = ''
+        displaylist = []
+        try:
+            displaylist = obj.display_list or 'title,link'
+        except AttributeError:
+            displaylist = 'title,link,author'
+        for key in spl(displaylist):
+            if not key:
+                continue
+            data = getattr(obj, key, None)
+            if not data:
+                continue
+            data = data.replace('\n', ' ')
+            data = striphtml(data.rstrip())
+            data = unescape(data)
+            result += data.rstrip()
+            result += ' - '
+        return result[:-2].rstrip()
+
+    def fetch(self, feed):
+        with fetchlock:
+            counter = 0
+            objs = []
+            for obj in reversed(list(getfeed(feed.rss, feed.display_list))):
+                fed = Feed()
+                update(fed, obj)
+                update(fed, feed)
+                if 'link' in fed:
+                    url = urllib.parse.urlparse(fed.link)
+                    if url.path and not url.path == '/':
+                        uurl = f'{url.scheme}://{url.netloc}/{url.path}'
+                    else:
+                        uurl = fed.link
+                    if uurl in Fetcher.seen.urls:
+                        continue
+                    Fetcher.seen.urls.append(uurl)
+                counter += 1
+                if self.dosave:
+                    write(fed)
+                objs.append(fed)
+        if objs:
+            write(Fetcher.seen)
+        txt = ''
+        feedname = getattr(feed, 'name')
+        if feedname:
+            txt = f'[{feedname}] '
+        for obj in objs:
+            txt2 = txt + self.display(obj)
+            Broker.announce(txt2.rstrip())
+        return counter
+
+    def run(self):
+        thrs = []
+        for feed in find('rss'):
+            thrs.append(launch(self.fetch, feed))
+        return thrs
+
+    def start(self, repeat=True):
+        last(Fetcher.seen)
+        if repeat:
+            repeater = Repeater(300.0, self.run)
+            repeater.start()
+
+
+class Parser(Object):
+
+    @staticmethod
+    def getitem(line, item):
+        lne = ''
+        try:
+            index1 = line.index(f'<{item}>') + len(item) + 2
+            index2 = line.index(f'</{item}>')
+            lne = line[index1:index2]
+            if 'CDATA' in lne:
+                lne = lne.replace('![CDATA[', '')
+                lne = lne.replace(']]', '')
+                lne = lne[1:-1]
+        except ValueError:
+            lne = None
+        return lne
+
+    @staticmethod
+    def parse(txt, item='title,link'):
+        res = []
+        for line in txt.split('<item>'):
+            line = line.strip()
+            obj = Object()
+            for itm in spl(item):
+                setattr(obj, itm, Parser.getitem(line, itm))
+            res.append(obj)
+        return res
+
+
+def getfeed(url, item):
+    if Cfg.debug:
+        return [Object(), Object()]
     try:
-        old = termios.tcgetattr(fds)
-    except termios.error:
-        gotterm = False
-    try:
-        func()
-    except (EOFError, KeyboardInterrupt):
-        print("")
-    finally:
-        if gotterm:
-            termios.tcsetattr(fds, termios.TCSADRAIN, old)
-        waiter()
-
-
-# COMMANDS
-
-
-def cmd(event):
-    "show list of commands"
-    event.reply(','.join(sorted(keys(Commands.cmds))))
-
-
-def err(event):
-    "show errors"
-    nmr = 0
-    for exc in Errors.errors:
-        stream = io.StringIO(
-                             traceback.print_exception(
-                                                       type(exc),
-                                                       exc,
-                                                       exc.__traceback__
-                                                      )
-                            )
-        for line in stream.readlines():
-            event.reply(line)
-            nmr += 1
-    if not nmr:
-        event.reply("no error")
+        result = geturl(url)
+    except (ValueError, HTTPError, URLError):
+        return [Object(), Object()]
+    if not result:
+        return [Object(), Object()]
+    return Parser.parse(str(result.data, 'utf-8'), item)
+
+
+def gettinyurl(url):
+    postarray = [
+        ('submit', 'submit'),
+        ('url', url),
+    ]
+    postdata = urlencode(postarray, quote_via=quote_plus)
+    req = Request('http://tinyurl.com/create.php',
+                  data=bytes(postdata, 'UTF-8'))
+    req.add_header('User-agent', useragent(url))
+    with urlopen(req) as htm:
+        for txt in htm.readlines():
+            line = txt.decode('UTF-8').strip()
+            i = re.search('data-clipboard-text="(.*?)"', line, re.M)
+            if i:
+                return i.groups()
+    return []
+
+
+def geturl(url):
+    url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
+    req = urllib.request.Request(url)
+    req.add_header('User-agent', useragent("rss fetcher"))
+    with urllib.request.urlopen(req) as response:
+        response.data = response.read()
+        return response
+
+
+def striphtml(text):
+    clean = re.compile('<.*?>')
+    return re.sub(clean, '', text)
+
+
+def unescape(text):
+    txt = re.sub(r'\s+', ' ', text)
+    return html.unescape(txt)
+
+
+def useragent(txt):
+    return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
+
+
+def dpl(event):
+    if len(event.args) < 2:
+        event.reply('dpl <stringinurl> <item1,item2>')
+        return
+    setter = {'display_list': event.args[1]}
+    for feed in find('rss', {'rss': event.args[0]}):
+        if feed:
+            update(feed, setter)
+            write(feed)
+    event.reply('ok')
 
 
-def flt(event):
-    "show listeners"
-    try:
-        index = int(event.args[0])
-        event.reply(prt(Bus.objs[index]))
-        return
-    except (KeyError, TypeError, IndexError, ValueError):
-        pass
-    event.reply(' | '.join([name(obj) for obj in Bus.objs]))
-
-
-def mod(event):
-    "show list of available modules"
-    path = opr.modules.__path__[0]
-    modlist = [x[:-3] for x in os.listdir(path) if x.endswith(".py") and x != "__init__.py"]
-    mods = ",".join(sorted(modlist))
-    event.reply(mods)
-
-
-def rld(event):
-    "reload"
-    if not event.args:
-        event.reply("rld <modname>")
-        return
-    modnames = event.args[0]
-    for modname in spl(modnames):
-        mods = getattr(opr.modules, modname)
-        if not mods:
-            event.reply(f"{modname} is not available")
-            continue
-        Commands.scan(mods)
-        if "start" in dir(mods):
-            thr = launch(mods.start)
-        event.reply(f"reloaded {modname}")
-
-
-def sts(event):
-    "print status"
-    nmr = 0
-    for bot in Bus.objs:
-        if 'state' in dir(bot):
-            event.reply(prt(bot.state, skip='lastline'))
-            nmr += 1
-    if not nmr:
-        event.reply("no status")
-
-
-def thr(event):
-    "show list of running threads"
-    result = []
-    for thread in sorted(threading.enumerate(), key=lambda x: x.name):
-        if str(thread).startswith('<_'):
-            continue
-        obj = Object()
-        update(obj, vars(thread))
-        if getattr(obj, 'sleep', None):
-            uptime = obj.sleep - int(time.time() - obj.state.latest)
-        elif getattr(obj, 'starttime', None):
-            uptime = int(time.time() - obj.starttime)
-        else:
-            uptime = int(time.time() - STARTTIME)
-        result.append((uptime, thread.name))
+def ftc(event):
     res = []
-    for uptime, txt in sorted(result, key=lambda x: x[1]):
-        lap = elapsed(uptime)
-        res.append(f'{txt}/{lap}')
+    thrs = []
+    fetcher = Fetcher()
+    fetcher.start(False)
+    thrs = fetcher.run()
+    for thr in thrs:
+        res.append(thr.join())
     if res:
-        event.reply(' '.join(res))
-    else:
-        event.reply('no threads')
+        event.reply(','.join([str(x) for x in res if x]))
+        return
 
 
-def unl(event):
-    "unload"
-    if not event.args:
-        event.reply("unl <modname>")
+def nme(event):
+    if len(event.args) != 2:
+        event.reply('name <stringinurl> <name>')
         return
-    modnames = event.args[0]
-    for modname in spl(modnames):
-        mods = getattr(opr.modules, modname)
-        if mods:
-            Commands.remove(mods)
-            if "stop" in dir(mods):
-                mods.stop()
-        event.reply(f"unloaded {modname}")
-
-
-def upt(event):
-    "show uptime"
-    event.reply(elapsed(time.time()-STARTTIME))
-
-
-# RUNTIME
-
-
-def main():
-    "main program function"
-    parse_cli(' '.join(sys.argv[1:]))
-    Commands.add(cmd)
-    Commands.add(err)
-    Commands.add(flt)
-    Commands.add(mod)
-    Commands.add(rld)
-    Commands.add(sts)
-    Commands.add(thr)
-    Commands.add(unl)
-    Commands.add(upt)
-    if "v" in Cfg.opts and "d" not in Cfg.opts:
-        Logging.verbose = True
-        Logging.raw = print
-    dowait = False
-    scanstr(opr.modules, Cfg.mod)
-    if Cfg.txt:
-        cli = CLI()
-        command(cli, Cfg.otxt)
-    elif 'd' in Cfg.opts:
-        daemon()
-        dowait = True
-    if "c" in Cfg.opts:
-        dowait = True
-    if dowait:
-        banner()
-        if 'c' in Cfg.opts and "d" not in Cfg.opts:
-            csl = Console()
-            csl.start()
-        scanstr(opr.modules, Cfg.mod, True, wait=False)
-        while 1:
-            time.sleep(1.0)
-            waiter()
+    selector = {'rss': event.args[0]}
+    for feed in find('rss', selector):
+        if feed:
+            feed.name = event.args[1]
+            write(feed)
+    event.reply('ok')
 
 
-if __name__ == "__main__":
-    wrap(main)
+def rem(event):
+    if len(event.args) != 1:
+        event.reply('rem <stringinurl>')
+        return
+    selector = {'rss': event.args[0]}
+    for feed in find('rss', selector):
+        if feed:
+            feed.__deleted__ = True
+            write(feed)
+    event.reply('ok')
+
+
+def rss(event):
+    if not event.rest:
+        nrs = 0
+        for feed in find('rss'):
+            elp = laps(time.time()-fntime(feed.__oid__))
+            txt = prt(feed)
+            event.reply(f'{nrs} {txt} {elp}')
+            nrs += 1
+        if not nrs:
+            event.reply('no rss feed found.')
+        return
+    url = event.args[0]
+    if 'http' not in url:
+        event.reply('i need an url')
+        return
+    for res in find('rss', {'rss': url}):
+        if res:
+            event.reply(f'already got {url}')
+            return
+    feed = Rss()
+    feed.rss = event.args[0]
+    write(feed)
+    event.reply('ok')
```

### Comparing `opr-230/opr/__init__.py` & `opr-240/opr.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,73 @@
+Metadata-Version: 2.1
+Name: opr
+Version: 240
+Summary: Object Programming Runtime
+Author-email: Bart Thate <programmingobject@gmail.com>
+License: Public Domain
+Project-URL: home, https://pypi.org/project/opr
+Project-URL: bugs, https://github.com/bthate/opr/issues
+Project-URL: source, https://github.com/bthate/opr
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: Public Domain
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+
 # This file is placed in the Public Domain.
+#
+# __author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
+NAME
+
+::
+
+   OPR - Object Programming Runtime
 
 
-"""Object Programming Runtime
+DESCRIPTION
 
 
-OPR is a python3 runtime is intended to be programmable  in a
-static, only code, no popen, no user imports and no reading
-modules from a directory, way. 
+::
 
-OPR provides some functionality, it can connect to IRC, fetch
-and display RSS feeds, take todo notes, keep a shopping list and
-log text.
+    OPR is a python3 runtime is intended to be programmable  in a
+    static, only code, no popen, no user imports and no reading
+    modules from a directory, way. 
+
+    OPR provides some functionality, it can connect to IRC, fetch
+    and display RSS feeds, take todo notes, keep a shopping list and
+    log text.
 
 
 SYNOPSIS
 
+
+::
+
     opr <cmd> [key=val] 
     opr <cmd> [key==val]
     opr [-c] [-d] [-v]
 
 
 INSTALL
 
 
+::
+
     $ pipx install opr
 
 
 USAGE
 
 
+::
+
     list of commands
 
     $ opr cmd
     cmd,err,flt,sts,thr,upt
 
     start a console
 
@@ -65,14 +100,16 @@
     $ opr  mod=irc,rss -d
     $ 
 
 
 CONFIGURATION
 
 
+::
+
  irc
 
     $ opr cfg server=<server>
     $ opr cfg channel=<channel>
     $ opr cfg nick=<nick>
 
  sasl
@@ -87,14 +124,16 @@
     $ opr rem <url>
     $ opr nme <url< <name>
 
 
 COMMANDS
 
 
+::
+
     cmd - commands
     cfg - irc configuration
     dlt - remove a user
     dpl - sets display items
     ftc - runs a fetching batch
     fnd - find objects 
     flt - instances registered
@@ -107,22 +146,25 @@
     rss - add a feed
     slg - slogan
     thr - show the running threads
 
 
 FILES
 
+::
+
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
 
 
-COPYRIGHT
+AUTHOR
 
-    OPR is placed in the Public Domain.
+::
 
-"""
+    Bart Thate <bthate@dds.nl>
 
 
-__author__ = "Bart Thate <bthate@dds.nl>"
+COPYRIGHT
 
+::
 
-from opr.objects import *
+    OPR is placed in the Public Domain.
```

### Comparing `opr-230/opr/modules/irc.py` & `opr-240/opr/modules/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,75 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,W0401
 
 
 "internet relay chat"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
 import time
 import textwrap
 import threading
-import _thread
 
 
-from opr.handler import Bus, Commands, Errors, Event, Handler
-from opr.loggers import Logging
-from opr.objects import Default, Object, copy, edit, keys, prt, update
-from opr.persist import find, fntime, last, write
-from opr.threads import launch
-from opr.utility import elapsed
+from .. import Broker, Cfg, Command, Errors, Event, Logging, Object, Reactor
+from .. import edit, find, fntime, keys, laps, last, prt, write
+from .. import launch, parse, update
 
 
-NAME = "opr"
-VERSION = "221"
-
-saylock = _thread.allocate_lock()
+from ..locking import saylock
 
 
 def start():
-    "start a irc bot"
     irc = IRC()
-    irc.start()
+    launch(irc.start)
     irc.events.joined.wait()
     return irc
 
 
 def stop():
-    "stop irc bots"
-    for bot in Bus.objs:
-        print(type(bot))
+    for bot in Broker.objs:
         if "IRC" in str(type(bot)):
             bot.stop()
 
 
 class NoUser(Exception):
 
-    "user is not found"
-
+    pass
 
-class Config(Default):
 
-    "irc config"
+class Config(Object):
 
-    channel = f'#{NAME}'
+    channel = f'#{Cfg.name}'
     control = '!'
     edited = time.time()
-    nick = NAME
-    nocommands = True
+    nick = Cfg.name
+    nocommands = False
     password = ''
     port = 6667
-    realname = NAME
+    realname = Cfg.name
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = NAME
+    username = Cfg.name
     users = False
     verbose = False
-    version = VERSION
 
     def __init__(self):
-        Default.__init__(self)
+        Object.__init__(self)
         self.channel = Config.channel
         self.nick = Config.nick
         self.port = Config.port
         self.realname = Config.realname
         self.server = Config.server
         self.username = Config.username
 
@@ -86,66 +78,57 @@
 
     def __size__(self):
         return len(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
-    "text wrapper"
-
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = True
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
         self.width = 450
 
 
 class Output(Object):
 
-    "output cache"
-
     cache = Object()
 
     def __init__(self):
         Object.__init__(self)
         self.oqueue = queue.Queue()
         self.dostop = threading.Event()
 
     def dosay(self, channel, txt):
-        "echo text to channel"
         raise NotImplementedError
 
     def extend(self, channel, txtlist):
-        "add to channel cache"
         if channel not in self.cache:
             setattr(self.cache, channel, [])
         cache = getattr(self.cache, channel, None)
         cache.extend(txtlist)
 
     def gettxt(self, channel):
-        "return text from chanel cache"
         txt = None
         try:
             cache = getattr(self.cache, channel, None)
             txt = cache.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
-        "send channel/txt to queue"
         if channel not in self.cache:
             setattr(self.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def output(self):
-        "output loop"
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             wrapper = TextWrap()
@@ -163,69 +146,62 @@
                 continue
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     def size(self, chan):
-        "show size of channel cache"
         if chan in self.cache:
             return len(getattr(self.cache, chan, []))
         return 0
 
     def start(self):
-        "start output loop"
         self.dostop.clear()
         launch(self.output)
         return self
 
     def stop(self):
-        "stop output loop"
         self.dostop.set()
         self.oqueue.put_nowait((None, None))
 
 
-class IRC(Handler, Output):
-
-    "internet relay chat"
+class IRC(Reactor, Output):
 
     def __init__(self):
-        Handler.__init__(self)
+        Reactor.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
-        self.events = Default()
+        self.events = Object()
         self.events.authed = threading.Event()
         self.events.connected = threading.Event()
         self.events.joined = threading.Event()
         self.channels = []
         self.sock = None
-        self.state = Default()
+        self.state = Object()
         self.state.keeprunning = False
         self.state.nrconnect = 0
         self.state.nrsend = 0
         self.zelf = ''
         self.register('903', cb_h903)
         self.register('904', cb_h903)
         self.register('AUTHENTICATE', cb_auth)
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
-        self.register("command", cb_command)
+        Broker.add(self)
 
     def announce(self, txt):
-        "annouce text on channels"
         for channel in self.channels:
             self.say(channel, txt)
 
     def command(self, cmd, *args):
-        "send command to server"
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -234,15 +210,14 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
-        "connect to server"
         self.state.nrconnect += 1
         self.events.connected.clear()
         Logging.debug(f"connecting to {server}:{port}")
         if self.cfg.password:
             Logging.debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
@@ -262,33 +237,29 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
-        "send direct text"
         time.sleep(1.0)
         Logging.debug(txt)
         self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
-        "disconnect from server"
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as ex:
             Errors.errors.append(ex)
 
-
     def doconnect(self, server, nck, port=6667):
-        "connect loop"
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
@@ -297,22 +268,20 @@
                 self.state.errors = str(ex)
                 Logging.debug(str(ex))
             Logging.debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def dosay(self, channel, txt):
-        "called from output cache"
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.command('PRIVMSG', channel, txt)
 
     def event(self, txt):
-        "return a event"
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
@@ -330,20 +299,18 @@
         elif cmd == '433':
             self.state.errors = txt
             nck = self.cfg.nick + '_' + str(random.randint(1, 10))
             self.command('NICK', nck)
         return evt
 
     def joinall(self):
-        "join all channels"
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
-        "keep alive loop"
         while 1:
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
@@ -353,25 +320,22 @@
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 start()
                 break
 
     def logon(self, server, nck):
-        "logon to server"
         self.events.connected.wait()
         self.events.authed.wait()
         nck = self.cfg.username
         self.command(f'NICK {nck}')
         self.command(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
-        # pylint: disable=R0912,R0915
-        "parse text"
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         Logging.debug(txt)
         obj = Event()
         obj.rawstr = rawstr
         obj.command = ''
@@ -422,15 +386,14 @@
             obj.args = spl[1:]
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        "poll input buffer for event"
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -449,15 +412,14 @@
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
-        "send raw text"
         txt = txt.rstrip()
         Logging.debug(txt)
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
@@ -474,236 +436,208 @@
                 Errors.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        "reconnect to server"
         Logging.debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def say(self, channel, txt):
-        "sat text of channel"
         self.oput(channel, txt)
 
     def some(self):
-        "check input cache"
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        "start irc loop"
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
-        launch(Handler.start, self)
+        launch(Reactor.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        "stop irc loop"
-        Bus.remove(self)
-        Handler.stop(self)
+        Broker.remove(self)
+        Reactor.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
 def cb_auth(evt):
-    "authenticate to server"
     bot = evt.bot()
     assert evt
     assert bot.cfg.password
     bot.direct(f'AUTHENTICATE {bot.cfg.password}')
 
+
 def cb_cap(evt):
-    "ask capabilities from server"
     bot = evt.bot()
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
 def cb_command(evt):
-    "execute an command"
-    Commands.handle(evt)
+    Command.handle(evt)
 
 
 def cb_error(evt):
-    "handle error"
     bot = evt.bot()
     bot.state.nrerror += 1
     bot.state.errors.append(evt.txt)
     Logging.debug(evt.txt)
 
 
 def cb_h903(evt):
-    "capabilities end"
     assert evt
     bot = evt.bot()
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(evt):
-    "capabilities end"
     assert evt
     bot = evt.bot()
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(evt):
-    "got killed"
+    pass
 
 
 def cb_log(evt):
-    "log event"
+    pass
 
 
 def cb_notice(evt):
-    "handle notice"
     bot = evt.bot()
     if evt.txt.startswith('VERSION'):
-        txt = f'\001VERSION {NAME} {bot.cfg.version} - {bot.cfg.username}\001'
+        txt = f'\001VERSION {Cfg.name.upper()} 140 - {bot.cfg.username}\001'
         bot.command('NOTICE', evt.channel, txt)
 
 
 def cb_privmsg(evt):
-    "handle privmsg"
     bot = evt.bot()
     if bot.cfg.nocommands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if bot.cfg.users and not Users.allowed(evt.origin, 'USER'):
             return
         Logging.debug(f"command from {evt.origin}: {evt.txt}")
-        msg = Event()
-        copy(msg, evt)
-        msg.type = 'command'
-        msg.parse(evt.txt)
-        bot.handle(msg)
+        parse(evt, evt.txt)
+        Command.handle(evt)
 
 
 def cb_quit(evt):
-    "handle quit"
     bot = evt.bot()
     Logging.debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
 class User(Object):
 
-    "an irc user"
-
     def __init__(self, val=None):
         Object.__init__(self)
         self.user = ''
         self.perms = []
         if val:
             update(self, val)
 
     def isok(self):
-        "verify user"
         return True
 
     def isthere(self):
-        "verify presence"
         return True
 
 
 class Users(Object):
 
-    "manages all irc users"
-
     @staticmethod
     def allowed(origin, perm):
-        "check whether user has permissions"
         perm = perm.upper()
         user = Users.get_user(origin)
         val = False
         if user and perm in user.perms:
             val = True
         return val
 
     @staticmethod
     def delete(origin, perm):
-        "delete an user"
         res = False
         for user in Users.get_users(origin):
             try:
                 user.perms.remove(perm)
                 write(user)
                 res = True
             except ValueError:
                 pass
         return res
 
     @staticmethod
     def get_users(origin=''):
-        "find all users"
         selector = {'user': origin}
         return find('user', selector)
 
     @staticmethod
     def get_user(origin):
-        "select specific user"
         users = list(Users.get_users(origin))
         res = None
         if len(users) > 0:
             res = users[-1]
         return res
 
     @staticmethod
     def perm(origin, permission):
-        "set permission of an user"
         user = Users.get_user(origin)
         if not user:
             raise NoUser(origin)
         if permission.upper() not in user.perms:
             user.perms.append(permission.upper())
             write(user)
         return user
 
 
 def cfg(event):
-    "edit irc config"
     config = Config()
     last(config)
     if not event.sets:
         event.reply(
                     prt(
                         config,
                         keys(config),
@@ -713,46 +647,43 @@
     else:
         edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
 def dlt(event):
-    "delete an user"
     if not event.args:
         event.reply('dlt <username>')
         return
     selector = {'user': event.args[0]}
     for obj in find('user', selector):
         obj.__deleted__ = True
         write(obj)
         event.reply('ok')
         break
 
 
 def met(event):
-    "add an user"
     if not event.args:
         nmr = 0
         for obj in find('user'):
-            lap = elapsed(time.time() - fntime(obj.__fnm__))
+            lap = laps(time.time() - fntime(obj.__fnm__))
             event.reply(f'{nmr} {obj.user} {obj.perms} {lap}s')
             nmr += 1
         if not nmr:
             event.reply('no user')
         return
     user = User()
     user.user = event.rest
     user.perms = ['USER']
     write(user)
     event.reply('ok')
 
 
 def mre(event):
-    "pull from output cache"
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
@@ -762,16 +693,16 @@
     for _x in range(3):
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
     event.reply(f'{size} more in cache')
 
+
 def pwd(event):
-    "create pasword from nickserv user/pass pair"
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
```

### Comparing `opr-230/opr/modules/log.py` & `opr-240/opr/modules/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R
 
 
 "log text"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import time
 
 
-from opr.objects import Object
-from opr.persist import find, fntime, write
-from opr.utility import elapsed
+from .. import Object
+from .. import find, fntime, laps, write
 
 
 class Log(Object):
 
-    "log objects"
-
     def __init__(self):
         super().__init__()
         self.createtime = time.time()
         self.txt = ''
 
     def __size__(self):
         return len(self.txt)
 
     def __since__(self):
         return self.createtime
 
 
 def log(event):
-    "log text"
     if not event.rest:
         nmr = 0
         for obj in find('log'):
-            lap = elapsed(time.time() - fntime(obj.__oid__))
+            lap = laps(time.time() - fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
```

### Comparing `opr-230/opr/modules/mbx.py` & `opr-240/opr/modules/mbx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,W0212,W0401
 
 
 "mailbox"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import mailbox
 import os
 import time
 
 
-from opr.objects import Object, prt, update
-from opr.persist import find, fntime, write
-from opr.utility import elapsed
+from .. import Object
+from .. import find, fntime, laps, prt, update, write
 
 
 bdmonths = [
             'Bo',
             'Jan',
             'Feb',
             'Mar',
@@ -26,15 +30,14 @@
             'Aug',
             'Sep',
             'Oct',
             'Nov',
             'Dec'
            ]
 
-
 monthint = {
             'Jan': 1,
             'Feb': 2,
             'Mar': 3,
             'Apr': 4,
             'May': 5,
             'Jun': 6,
@@ -45,32 +48,26 @@
             'Nov': 11,
             'Dec': 12
            }
 
 
 class Email(Object):
 
-    "email object"
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.text = ""
 
     def len(self):
-        "length"
         return len(self.__dict__)
 
     def size(self):
-        "size"
         return len(self.__dict__)
 
 
 def to_date(date):
-    # pylint: disable=C0209
-    "parse date out of string"
     date = date.replace("_", ":")
     res = date.split()
     ddd = ""
     try:
         if "+" in res[3]:
             raise ValueError
         if "-" in res[3]:
@@ -99,48 +96,44 @@
                             ddd = "{:4}".format(res[2])
                         except (IndexError, KeyError):
                             ddd = ""
     return ddd
 
 
 def cor(event):
-    "trace correspondence"
     if not event.args:
         event.reply("cor <email>")
         return
     nrs = -1
     for email in find("email", {"From": event.args[0]}):
         nrs += 1
         txt = ""
         if len(event.args) > 1:
             txt = ",".join(event.args[1:])
         else:
             txt = "From,Subject"
-        lsp = elapsed(time.time() - fntime(email.__oid__))
+        lsp = laps(time.time() - fntime(email.__oid__))
         txt = prt(email, txt, plain=True)
         event.reply(f"{nrs} {txt} {lsp}")
 
 
 def eml(event):
-    "search emails"
     if not event.args:
         event.reply("eml <searchtxtinemail>")
         return
     nrs = -1
     for email in find("email"):
         if event.rest in email.text:
             nrs += 1
             txt = prt(email, "From,Subject")
-            lsp = elapsed(time.time() - fntime(email.__oid__))
+            lsp = laps(time.time() - fntime(email.__oid__))
             event.reply(f"{nrs} {txt} {lsp}")
 
 
 def mbx(event):
-    # pylint: disable=W0212
-    "scan mailbox/maildir"
     if not event.args:
         return
     path = os.path.expanduser(event.args[0])
     event.reply("reading from {path}")
     nrs = 0
     if os.path.isdir(path):
         thing = mailbox.Maildir(path, create=False)
```

### Comparing `opr-230/opr/modules/mdl.py` & `opr-240/opr/modules/mdl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,I,R,,W0613,E1101,E0402
+# pylint: disable=C,I,R,W0613,E1101,E0402,W0401
 # pylama: ignore=E225,E501
 
 
-"genocide model for here in the netherlands"
+"genocide model of the netherlands"
 
 
-import datetime
-import time
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
-from opr.handler import Bus, Event
-from opr.objects import Object, copy, keys
-from opr.repeats import Repeater
-from opr.threads import launch
-from opr.utility import elapsed
+import datetime
+import time
 
 
-def __dir__():
-    return (
-        'mdl',
-        'now',
-        'start'
-    )
+from .. import Broker, Event, Object, Repeater
+from .. import laps, launch, keys
 
 
 def start():
     time.sleep(60.0)
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
@@ -42,15 +34,14 @@
 
 DAY=24*60*60
 YEAR = 365*DAY
 SOURCE = "https://github.com/bthate/genocide"
 STARTDATE = "2020-01-01 00:00:00"
 STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
-
 oor = """"Totaal onderliggende doodsoorzaken (aantal)";
          "1 Infectieuze en parasitaire ziekten/Totaal infectieuze en parasitaire zktn (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.1 Tuberculose (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.2 Meningokokkeninfecties (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.3 Virale hepatitis (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.4 AIDS (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.5 Ov. infectieuze en parasitaire zktn (aantal)";
@@ -139,15 +130,14 @@
          "17 Uitwendige doodsoorzaken/17.3 Moord en doodslag (aantal)";
          "17 Uitwendige doodsoorzaken/17.4 Gebeurtenissen opzet onbekend (aantal)";
          "17 Uitwendige doodsoorzaken/17.5 Overige uitwendige doodsoorzaken (aantal)";
          "18 COVID-19 (Coronavirus ziekte 19)/18 Totaal COVID-19 (Coronavirus 19) (aantal)";
          "18 COVID-19 (Coronavirus ziekte 19)/18.1 Vastgestelde COVID-19 (aantal)";
          "18 COVID-19 (Coronavirus ziekte 19)/18.2 Vermoedelijke COVID-19 (aantal)""".split(";")
 
-
 aantal = """
           168678;
           2974;
           32;
           1;
           34;
           23;
@@ -238,19 +228,14 @@
           28;
           639;
           20173;
           17495;
           2678
          """.split(";")
 
-
-oorzaak = Object()
-copy(oorzaak, zip(oor,aantal))
-
-
 #oorzaak.Suicide = 1859
 
 
 aliases = {}
 aliases["Nieuwvormingen"] = "cancer"
 aliases["Hart en vaatstelsel"] = "hart disease"
 aliases["Psychische en gedragsstoornissen"] = "mental illness"
@@ -266,20 +251,14 @@
 aliases["Bloed, bloedvormende organen"] = "blood disease"
 aliases["Aangeboren afwijkingen"] = "birth defect"
 aliases["Huid en subcutis"] = "skin disease"
 aliases["Zwangerschap"] = "pregnancy"
 aliases["Suicide"] = "suicide"
 
 
-def getalias(txt):
-    for key, value in aliases.items():
-        if txt.lower() in key.lower():
-            return value
-
-
 demo = Object()
 demo.gehandicapten = 2000000
 demo.ggz = 800000
 demo.population = 17440000
 demo.part = 7000000000 / demo.population
 
 
@@ -287,14 +266,15 @@
 jaar["WvGGZ"] = 14206
 jaar["Pvp"] = 20088
 jaar["Wzd"] = 25000
 jaar["Wfz"] = 23820
 jaar["totaal"] = 168678
 
 
+oorzaak = Object(zip(oor, aantal))
 oorzaken = Object()
 
 
 def boot():
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
@@ -323,32 +303,38 @@
         nms = nms.strip()
         setattr(oorzaken, nms, aantal[_nr])
 
 
 def daily():
     time.sleep(10.0)
     while 1:
-        event = Event()
-        cbnow(event)
+        evt = Event()
+        cbnow(evt)
         time.sleep(24*60*60)
 
 
 def hourly():
     while 1:
         time.sleep(60*60)
-        event = Event()
-        cbnow(event)
+        evt = Event()
+        cbnow(evt)
 
 
 def seconds(nrs):
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
+def getalias(txt):
+    for key, value in aliases.items():
+        if txt.lower() in key.lower():
+            return value
+
+
 def getday():
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
@@ -363,50 +349,49 @@
         if word in k:
             return True
     return False
 
 
 def cbnow(evt):
     delta = time.time() - STARTTIME
-    txt = elapsed(delta) + " "
+    txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
         txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
-    Bus.announce(txt)
+    Broker.announce(txt)
 
 
 def cbstats(evt):
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
         nrday = int(DAY/needed)
         delta2 = time.time() - getday()
         thisday = int(delta2/needed)
-        #onday = (24*60*60/needed)
         txt = "patient #%s died from %s (%s/%s) every %s (%s/year)" % (
                                                                nrtimes,
                                                                getalias(name),
                                                                thisday,
                                                                nrday,
-                                                               elapsed(needed),
+                                                               laps(needed),
                                                                nryear,
                                                               )
-        Bus.announce(txt)
+        Broker.announce(txt)
 
 
 def now(event):
     delta = time.time() - STARTTIME
-    txt = elapsed(delta) + " "
+    txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
         txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
@@ -424,29 +409,29 @@
         thisday = int(DAY % needed)
         txt = "patient #%s died from %s (%s/%s/%s) every %s" % (
                                                                nrtimes,
                                                                getalias(name),
                                                                thisday,
                                                                nrday,
                                                                nryear,
-                                                               elapsed(needed)
+                                                               laps(needed)
                                                               )
         event.reply(txt)
 
 
 def tpc(event):
-    txt = "%ss " % elapsed(time.time() - STARTTIME)
+    txt = "%ss " % laps(time.time() - STARTTIME)
     for name in sorted(oorzaken, key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         if needed > 60*60:
             continue
         txt += "%s %s " % (getalias(name), nrtimes)
-    for bot in Bus.objs:
+    for bot in Broker.objs:
         try:
             for channel in bot.channels:
                 bot.topic(channel, txt)
         except AttributeError:
             pass
```

### Comparing `opr-230/opr/modules/req.py` & `opr-240/opr/modules/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
@@ -73,10 +75,12 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 def req(event):
-    "show request to the prosecutor"
     event.reply(__doc__)
```

### Comparing `opr-230/opr/modules/shp.py` & `opr-240/opr/modules/wsh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,W0401,W0614
 
 
-"shop"
+"wish list"
 
 
-import time
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
 
+import time
 
-from opr.objects import Object
-from opr.persist import find, fntime, write
-from opr.utility import elapsed
 
+from .. import Object
+from .. import find, fntime, laps, write
 
-class Shop(Object):
 
-    "shop item"
+class Wish(Object):
 
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
-    def sizeof(self):
-        "size"
-        return len(self.txt)
+    def gettxt(self):
+        return self.txt
 
-    def length(self):
-        "len"
-        return len(self.__dict__)
+    def settxt(self, txt):
+        self.txt = txt
 
 
-def got(event):
-    "got shop"
+def ful(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
-    for obj in find('shop', selector):
+    for obj in find('wish', selector):
         obj.__deleted__ = True
         write(obj)
-        event.reply('ok')
+        event.reply('done')
 
 
-def shp(event):
-    "add shop"
+def wsh(event):
     if not event.rest:
         nmr = 0
-        for obj in find('shop'):
-            lap = elapsed(time.time()-fntime(obj.__oid__))
+        for obj in find('wish'):
+            lap = laps(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
-            event.reply("no shops")
+            event.reply("no wishes")
         return
-    obj = Shop()
+    obj = Wish()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `opr-230/opr/modules/tdo.py` & `opr-240/opr/modules/tdo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R
 
 
-"todo"
+"todo list"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import time
 
 
-from opr.objects import Object
-from opr.persist import find, fntime, write
-from opr.utility import elapsed
+from .. import Object
+from .. import laps, find, fntime, write
 
 
 class Todo(Object):
 
-    "todo object"
-
     def __init__(self):
         super().__init__()
         self.txt = ''
 
     def len(self):
-        "length"
-        return len(self.__dict__)
+        return 0
 
     def size(self):
-        "size"
         return len(self.__dict__)
 
 
 def dne(event):
-    "flag todo as done"
     if not event.args:
         return
     selector = {'txt': event.args[0]}
     for obj in find('todo', selector):
         obj.__deleted__ = True
         write(obj)
         event.reply('ok')
         break
 
 
 def tdo(event):
-    "add a todo"
     if not event.rest:
         nmr = 0
         for obj in find('todo'):
-            lap = elapsed(time.time()-fntime(obj.__oid__))
+            lap = laps(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply("no todo")
         return
     obj = Todo()
     obj.txt = event.rest
```

### Comparing `opr-230/opr/modules/udp.py` & `opr-240/opr/modules/udp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,96 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R
 
 
 "udp to irc relay"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import select
 import socket
 import sys
 import time
 
 
-from opr.handler import Bus
-from opr.objects import Default, Object
-from opr.persist import last
-from opr.threads import launch
+from .. import Broker, Object
+from .. import last, launch
 
 
 def start():
-    "start udp server"
     udpd = UDP()
     udpd.start()
     return udpd
 
 
-class Cfg(Default):
-
-    "udp configuration"
+class Cfg(Object):
 
     def __init__(self):
         super().__init__()
         self.host = "localhost"
         self.port = 5500
 
     def len(self):
-        "length"
         return self.server
 
     def size(self):
-        "size"
         return self.port
 
-class UDP(Object):
 
-    "udp to irc relay"
+class UDP(Object):
 
     def __init__(self):
         super().__init__()
         self.stopped = False
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.cfg = Cfg()
         self.cfg.addr = ""
 
     def output(self, txt, addr=None):
-        "output text on listeners bus"
         if addr:
             self.cfg.addr = addr
-        Bus.announce(txt.replace("\00", ""))
+        Broker.announce(txt.replace("\00", ""))
 
     def server(self):
-        "listen on udp socket"
         try:
             self._sock.bind((self.cfg.host, self.cfg.port))
         except socket.gaierror:
             return
         while not self.stopped:
             (txt, addr) = self._sock.recvfrom(64000)
             if self.stopped:
                 break
             data = str(txt.rstrip(), "utf-8")
             if not data:
                 break
             self.output(data, addr)
 
     def exit(self):
-        "exit loop"
         self.stopped = True
         self._sock.settimeout(0.01)
         self._sock.sendto(bytes("exit", "utf-8"), (self.cfg.host, self.cfg.port))
 
     def start(self):
-        "start udp listening loop"
         last(self.cfg)
         launch(self.server)
 
 
 def toudp(host, port, txt):
-    "function to send udp text"
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
 def udp(event):
-    "command to send udp"
     cfg = Cfg()
     last(cfg)
     if len(sys.argv) > 2:
         txt = " ".join(sys.argv[2:])
         toudp(cfg.host, cfg.port, txt)
         return
     if not select.select([sys.stdin, ], [], [], 0.0)[0]:
```

### Comparing `opr-230/opr/modules/wsd.py` & `opr-240/opr/modules/wsd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R
 
 
 """| wijsheid, wijs !
 
 | OVERDRACHT
 | ==========
 
@@ -180,13 +182,15 @@
 | twee eieren (gemeente huis en buiging naar west)
 | vreedevernoeming
 | duiding
 | coding
 """
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import random
 
 
 def wsd(event):
-    "present wisdom"
     event.reply(random.choice(__doc__.split("\n")).strip()[2:])
```

### Comparing `opr-230/opr/persist.py` & `opr-240/opr/persist.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,97 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R
 
 
-"persist"
+"persistence"
 
 
-# IMPORTS
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import os
 import sys
 import time
-import _thread
 
-
-from opr.objects import Object, copy, ident, dump, items, kind, load, update
-from opr.utility import cdir, strip
-
-
-# DEFINES
+from .objects import kind
+from .decoder import load
+from .encoder import dump
+from .locking import disklock
+from .objects import Object, ident, items, update
+from .utility import cdir, strip
 
 
 def __dir__():
     return (
             'Persist',
-            'files',
             'find',
-            'fnclass',
-            'fns',
-            'fntime',
-            'hook',
             'last',
             'read',
-            'readrec',
             'search',
-            'write',
-            'writerec'
+            'write'
            )
 
 
-disklock = _thread.allocate_lock()
+__all__ = __dir__()
 
 
-# CLASSES
 
+class Persist:
 
-class Persist(Object):
-
-    "directory to persist to"
+    """directory to persist to"""
 
     workdir = ""
 
     @staticmethod
     def path(pth) -> str:
-        "return store path"
+        """return store path"""
         return os.path.join(Persist.workdir, 'store', pth)
 
     @staticmethod
     def storedir() -> str:
-        "return storage directory"
-        return os.path.join(Persist.workdir, "store")
-
-
-# UTILITY
+        """return storage directory"""
+        return os.path.join(Persist.workdir, "store", "")
 
 
 def files() -> []:
-    "show all files in store"
+    """show all files in store"""
     res = []
     path = Persist.storedir()
     if os.path.exists(path):
         res = os.listdir(path)
     return res
 
 
 def find(mtc, selector=None) -> []:
-    "locate specific objects"
+    """locate specific objects"""
     if selector is None:
         selector = {}
     for fnm in fns(mtc):
         obj = hook(fnm)
         if '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
         yield obj
 
 
 def fnclass(pth) -> str:
-    "return class from filename"
+    """return class from filename"""
     try:
         *_rest, mpth = pth.split("store")
         splitted = mpth.split(os.sep)
         return splitted[0]
     except ValueError:
         pass
     return None
 
 
 def fns(mtc) -> []:
-    "return matching filenames"
+    """return matching filenames"""
     dname = ''
     lst = mtc.lower().split(".")[-1]
     for rootdir, dirs, _files in os.walk(Persist.storedir(), topdown=False):
         if dirs:
             dname = sorted(dirs)[-1]
             if dname.count('-') == 2:
                 ddd = os.path.join(rootdir, dname)
@@ -111,15 +100,15 @@
                     path2 = os.path.join(ddd, fls[-1])
                     splitted = strip(path2).split(os.sep, maxsplit=1)[0]
                     if lst in splitted.lower().split(".")[-1]:
                         yield strip(path2)
 
 
 def fntime(daystr) -> float:
-    "return time from filename"
+    """return time from filename"""
     daystr = daystr.replace('_', ':')
     datestr = ' '.join(daystr.split(os.sep)[-2:])
     if '.' in datestr:
         datestr, rest = datestr.rsplit('.', 1)
     else:
         rest = ''
     tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
@@ -127,15 +116,15 @@
         tme += float('.' + rest)
     else:
         tme = 0
     return tme
 
 
 def hook(otp) -> type:
-    "return object from filename"
+    """return object from filename"""
     clz = fnclass(otp)
     splitted = clz.split(".")
     modname = ".".join(splitted[:1])
     clz = splitted[-1]
     mod = sys.modules.get(modname, None)
     if mod:
         cls = getattr(mod, clz, None)
@@ -144,91 +133,61 @@
         read(obj, otp)
         return obj
     obj = Object()
     read(obj, otp)
     return obj
 
 
-## METHODS
+# METHODS
 
 
 def last(obj, selector=None) -> None:
-    "update with last saved version"
+    """update with last saved version"""
     if selector is None:
         selector = {}
     result = sorted(
                     find(kind(obj), selector),
                     key=lambda x: fntime(x.__oid__)
                    )
     if result:
         inp = result[-1]
         update(obj, inp)
         obj.__oid__ = inp.__oid__
     return obj.__oid__
 
 
 def read(obj, pth) -> str:
-    "read object from path"
+    """read object from path"""
     pth = Persist.path(pth)
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
     return obj.__oid__
 
 
-def readrec(obj, pth=None) -> type:
-    "read object recursively"
-    ooo = type(obj)()
-    if pth:
-        read(ooo, pth)
-    else:
-        update(ooo, obj)
-    oooo = type(obj)()
-    for key, value in items(ooo):
-        if issubclass(type(value), Object):
-            setattr(oooo, key, readrec(value))
-            continue
-        setattr(oooo, key, value)
-    return oooo
-
-
-def search(obj, selector) -> bool:
-    "check whether values in selector dict match in the object"
+def search(self, selector) -> bool:
     res = False
-    select = Object()
-    copy(select, selector)
-    for key, value in items(select):
+    for key, value in items(selector):
         try:
-            val = getattr(obj, key)
-        except AttributeError:
+            val = self[key]
+            if str(value) in str(val):
+                res = True
+                break
+        except KeyError:
             continue
-        if str(value) in str(val):
-            res = True
-            break
     return res
 
 
 def write(obj) -> str:
-    "write object to disk"
+    """write object to disk"""
     try:
         pth = obj.__oid__
     except TypeError:
         pth = ident(obj)
     pth = Persist.path(pth)
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
-
-
-def writerec(obj):
-    "write object recursively"
-    ooo = type(obj)()
-    for key, value in items(obj):
-        if issubclass(type(value), Object):
-            setattr(ooo, key, writerec(value))
-        else:
-            setattr(ooo, key, str(value))
-    return write(ooo)
```

### Comparing `opr-230/opr/threads.py` & `opr-240/opr/threads.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,87 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,W0718
 
 
-"thread"
+"running threads"
 
 
-# IMPORTS
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import functools
 import queue
 import threading
 import time
-import types
 
 
-# DEFINES
-
-
-STARTTIME = time.time()
+from .errored import Errors
+from .utility import name
 
 
 def __dir__():
     return (
             'Thread',
             'launch',
             'name',
             'threaded'
            )
 
 
-# CLASSES
+__all__ = __dir__()
 
 
 class Thread(threading.Thread):
 
-    "seperate line of execution"
-
     def __init__(self, func, thrname, *args, daemon=True):
         super().__init__(None, self.run, thrname, (), {}, daemon=daemon)
         self._result = None
         self.name = thrname or name(func)
         self.queue = queue.Queue()
         self.queue.put_nowait((func, args))
         self.sleep = None
         self.starttime = time.time()
 
     def __iter__(self):
-        ""
         return self
 
     def __next__(self):
-        ""
         for k in dir(self):
             yield k
 
     def join(self, timeout=None):
-        "join this thread"
         super().join(timeout)
         return self._result
 
     def run(self):
-        "run workload"
         func, args = self.queue.get()
-        self._result = func(*args)
-
-
-# UTILITY
+        try:
+            self._result = func(*args)
+        except Exception as ex:
+            exc = ex.with_traceback(ex.__traceback__)
+            Errors.errors.append(exc)
+            if args:
+                try:
+                    args[0].ready()
+                except AttributeError:
+                    pass
 
 
 def launch(func, *args, **kwargs) -> Thread:
-    "start a function in a thread"
     thrname = kwargs.get('name', '')
     thread = Thread(func, thrname, *args)
     thread.start()
     return thread
 
 
-# METHODS
-
-
-def name(obj) -> str:
-    "return full qualified name of an object"
-    typ = type(obj)
-    if isinstance(typ, types.ModuleType):
-        return obj.__name__
-    if '__self__' in dir(obj):
-        clz = obj.__self__.__class__.__name__
-        nme = obj.__name__
-        return f'{clz}.{nme}'
-    if '__class__' in dir(obj) and '__name__' in dir(obj):
-        clz = obj.__class__.__name__
-        nme = obj.__name__
-        return f'{clz}.{nme}'
-    if '__class__' in dir(obj):
-        return obj.__class__.__name__
-    if '__name__' in dir(obj):
-        clz = obj.__class__.__name__
-        nme = obj.__name__
-        return f'{clz}.{nme}'
-    return None
-
-
 def threaded(func, *args, **kwargs) -> None:
 
-    "threaded decorator"
-
     @functools.wraps(func)
     def threadedfunc(*args, **kwargs):
-        "run function in a thread"
         thread = launch(func, *args, **kwargs)
         if args:
             args[0].thr = thread
         return thread
 
     threadedfunc.args = args
     threadedfunc.kwargs = kwargs
```

### Comparing `opr-230/pyproject.toml` & `opr-240/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+# This file is placed in the Public Domain.
+#
+# __author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [options]
 zip_safe = true
 include_package_data = true
 
 
 [project]
 name = "opr"
 description = "Object Programming Runtime"
-version = "230"
+version = "240"
 authors = [
     {name = "Bart Thate", email = "programmingobject@gmail.com" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers = [ 
                'Development Status :: 3 - Alpha',
```

