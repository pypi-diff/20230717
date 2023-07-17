# Comparing `tmp/cpyvpn-1.6.tar.gz` & `tmp/cpyvpn-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpyvpn-1.6.tar", last modified: Fri Mar 24 10:29:06 2023, max compression
+gzip compressed data, was "cpyvpn-1.6.1.tar", last modified: Mon Jul 17 09:06:01 2023, max compression
```

## Comparing `cpyvpn-1.6.tar` & `cpyvpn-1.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-24 10:29:06.703666 cpyvpn-1.6/
--rw-r--r--   0 nick      (1000) nick      (1000)      400 2023-03-24 10:17:25.000000 cpyvpn-1.6/LICENSE
--rw-r--r--   0 nick      (1000) nick      (1000)    35147 2023-03-24 10:17:25.000000 cpyvpn-1.6/LICENSE-GPLv3
--rw-r--r--   0 nick      (1000) nick      (1000)       52 2023-03-24 10:17:25.000000 cpyvpn-1.6/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     8161 2023-03-24 10:29:06.703666 cpyvpn-1.6/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     7172 2023-03-24 10:17:25.000000 cpyvpn-1.6/README.md
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-24 10:29:06.700666 cpyvpn-1.6/cpyvpn/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      171 2023-03-24 10:29:06.000000 cpyvpn-1.6/cpyvpn/__version__.py
--rw-r--r--   0 nick      (1000) nick      (1000)    24527 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/appdirs.py
--rw-r--r--   0 nick      (1000) nick      (1000)    15377 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/auth.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4804 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/cfg.py
--rw-r--r--   0 nick      (1000) nick      (1000)    15137 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/client.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6742 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/crt.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3454 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/cui.py
--rw-r--r--   0 nick      (1000) nick      (1000)    23704 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/ma.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4037 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/rsa.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1029 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/snx.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-24 10:29:06.702666 cpyvpn-1.6/cpyvpn/srv/
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-24 10:29:06.703666 cpyvpn-1.6/cpyvpn/srv/data/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/cert.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/cl_cert.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/cl_key.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/key.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     7698 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/rr.js
--rw-r--r--   0 nick      (1000) nick      (1000)     1242 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/data/rsa.keys
--rw-r--r--   0 nick      (1000) nick      (1000)    28150 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/srv/server.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4384 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/ssl_ctx.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2724 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/trutils.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9553 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/utils.py
--rw-r--r--   0 nick      (1000) nick      (1000)    14065 2023-03-24 10:17:25.000000 cpyvpn-1.6/cpyvpn/vna.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-24 10:29:06.701666 cpyvpn-1.6/cpyvpn.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     8161 2023-03-24 10:29:06.000000 cpyvpn-1.6/cpyvpn.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      695 2023-03-24 10:29:06.000000 cpyvpn-1.6/cpyvpn.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-03-24 10:29:06.000000 cpyvpn-1.6/cpyvpn.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       71 2023-03-24 10:29:06.000000 cpyvpn-1.6/cpyvpn.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        7 2023-03-24 10:29:06.000000 cpyvpn-1.6/cpyvpn.egg-info/top_level.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-03-24 10:27:02.000000 cpyvpn-1.6/cpyvpn.egg-info/zip-safe
--rw-r--r--   0 nick      (1000) nick      (1000)      171 2023-03-24 10:17:25.000000 cpyvpn-1.6/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1104 2023-03-24 10:29:06.704666 cpyvpn-1.6/setup.cfg
--rw-r--r--   0 nick      (1000) nick      (1000)     1756 2023-03-24 10:17:25.000000 cpyvpn-1.6/setup.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.239914 cpyvpn-1.6.1/
+-rw-r--r--   0 nick      (1000) nick      (1000)      400 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)    35147 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/LICENSE-GPLv3
+-rw-r--r--   0 nick      (1000) nick      (1000)       52 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     8423 2023-07-17 09:06:01.239914 cpyvpn-1.6.1/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)     7432 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/README.md
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.236914 cpyvpn-1.6.1/cpyvpn/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      176 2023-07-17 09:06:00.000000 cpyvpn-1.6.1/cpyvpn/__version__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    24527 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/appdirs.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    15413 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/auth.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4804 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/cfg.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16821 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/client.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6742 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/crt.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3454 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/cui.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    23744 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/ma.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4037 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/rsa.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1029 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/snx.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.237914 cpyvpn-1.6.1/cpyvpn/srv/
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.239914 cpyvpn-1.6.1/cpyvpn/srv/data/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/cert.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/cl_cert.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/cl_key.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/key.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     7998 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/srv/data/rr.js
+-rw-r--r--   0 nick      (1000) nick      (1000)     1242 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/rsa.keys
+-rw-r--r--   0 nick      (1000) nick      (1000)    28150 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/server.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4615 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/ssl_ctx.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2724 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/trutils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9587 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/utils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    14263 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/vna.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.237914 cpyvpn-1.6.1/cpyvpn.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     8423 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)      695 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       71 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        7 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/top_level.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/zip-safe
+-rw-r--r--   0 nick      (1000) nick      (1000)      171 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1104 2023-07-17 09:06:01.240914 cpyvpn-1.6.1/setup.cfg
+-rw-r--r--   0 nick      (1000) nick      (1000)     1756 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/setup.py
```

### Comparing `cpyvpn-1.6/LICENSE-GPLv3` & `cpyvpn-1.6.1/LICENSE-GPLv3`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/PKG-INFO` & `cpyvpn-1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpyvpn
-Version: 1.6
+Version: 1.6.1
 Summary: Check Point VPN client written in Python.
 Home-page: https://gitlab.com/cpvpn/cpyvpn
 Author: Nikolay A. Krylov
 Author-email: krylovna@gmail.com
 License: GPL3
 Project-URL: PyPI, https://pypi.org/project/cpyvpn
 Project-URL: Source, https://gitlab.com/cpvpn/cpyvpn
@@ -108,14 +108,17 @@
 
     `cp_client -m l -u testuser vpn.example.org`
 
 * TRAC login with realm and predefined user name:
 
     `cp_client --realm vpn -u testuser vpn.example.org`
 
+* TRAC login with the predefined user name, run in the background after user authication, redirect output to cp.log and save background process pid to the cp.pid file:
+
+    `cp_client --daemon --logfile=./cp.log --pidfile=./cp.pid -u testuser vpn.example.org`
 * TRAC login with predefined user name and password from external program:
 
     `cp_client -u user --passwd-script 'kwallet-query kdewallet' vpn.example.org`
 
 * TRAC login with certificate as a first factor:
 
     `cp_client -c cert.pem vpn.example.org`
```

### Comparing `cpyvpn-1.6/README.md` & `cpyvpn-1.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
     `cp_client -m l -u testuser vpn.example.org`
 
 * TRAC login with realm and predefined user name:
 
     `cp_client --realm vpn -u testuser vpn.example.org`
 
+* TRAC login with the predefined user name, run in the background after user authication, redirect output to cp.log and save background process pid to the cp.pid file:
+
+    `cp_client --daemon --logfile=./cp.log --pidfile=./cp.pid -u testuser vpn.example.org`
 * TRAC login with predefined user name and password from external program:
 
     `cp_client -u user --passwd-script 'kwallet-query kdewallet' vpn.example.org`
 
 * TRAC login with certificate as a first factor:
 
     `cp_client -c cert.pem vpn.example.org`
```

### Comparing `cpyvpn-1.6/cpyvpn/appdirs.py` & `cpyvpn-1.6.1/cpyvpn/appdirs.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/auth.py` & `cpyvpn-1.6.1/cpyvpn/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
               "RequestData":{
                   "client_type":self.ct,
                   "selectedLoginOption":self._logopt
                   }
               }
               }).serialize()[:-1]
         logger.info("Cert. login")
+        ssl_ctx.require_user_cert()
         return self._extract_ac(self.url + self.cert_path, body)
 
     def do_login(self):
 
         logger.info("Standard login")
         body = CPRR({"CCCclientRequest":
               {"RequestHeader":{
```

### Comparing `cpyvpn-1.6/cpyvpn/cfg.py` & `cpyvpn-1.6.1/cpyvpn/cfg.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/client.py` & `cpyvpn-1.6.1/cpyvpn/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # Created on 07.05.2021
 # Copyright © 2020-2021 Nick Krylov.
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import sys
+import stat
 import os.path as op
 import time
 import datetime
 
 import asyncio
 import logging
 import secrets
@@ -220,28 +221,45 @@
         else:
             logger.error("Exception occured in the event loop!\n{}".format("".join(traceback.format_exception(exc))))
         if self._ka_handle:
             self._ka_handle.cancel()
         self.evt.set()
 
 
+class PidFile:
+
+    def __init__(self, name):
+        self.name = name
+
+        try:
+            fd = os.open(name, os.O_WRONLY | os.O_CREAT | os.O_EXCL, stat.S_IRUSR | stat.S_IWUSR)
+            self.pidfile = os.fdopen(fd, 'w')
+            os.set_inheritable(fd, 1)
+        except Exception as e:
+            raise RuntimeError("Can't create pid file, error was {}".format(e))
+
+    def close(self):
+        self.pidfile.close()
+        os.unlink(self.name)
+
+    def __getattr__(self, name):
+        return getattr(self.pidfile, name)
+
+
 def vpn_main(options, vna_args):
-    loop = asyncio.new_event_loop()
+
     with contextlib.ExitStack() as es:
+        pidfile = es.enter_context(contextlib.closing(PidFile(options.pidfile)) if options.pidfile else contextlib.nullcontext())
         sna = es.enter_context(contextlib.closing(auth.SNXAuth(options, options.ui)))
         options.vna_obj = es.enter_context(vna.init_vna(vna_args))
 
         if options.mode == 'q':
             return
 
         sna.init()
-        kw = {}
-        if sys.version_info[:2] < (3, 10):
-            kw["loop"] = loop
-        evt = asyncio.Event(**kw)
 
         slim_ver = 1
         rl = []
         # Use slim protocol v2 if NOT MA
         if not options.force_v1 and not sna.use_ma and sna.gw_info.pv >= 100:
             slim_ver = 2
             rl = utils.get_ranges(sna.auth_obj.url, sna.auth_obj.sid)
@@ -253,14 +271,37 @@
         sd = sna.get_session_data()
         if options.printcookie:
             if sna.use_ma:
                 cookie_str = sna.auth_obj.ma_cookies
             else:
                 cookie_str = "{}:{}".format(sna.auth_obj.sid, sd.cookie)
             logger.info("COOKIE: {}".format(cookie_str))
+        if options.daemon:
+            for _ in range(2):
+                try:
+                    pid = os.fork()
+                    if pid != 0:
+                        es.pop_all()
+                        return
+                except OSError:
+                    quit(1)
+
+        if pidfile:
+            pidfile.write("{}".format(os.getpid()))
+            pidfile.flush()
+
+        if options.logfile:
+            logger.removeHandler(options.defhandler)
+            logger.addHandler(logging.FileHandler(options.logfile,mode='w'))
+
+        loop = asyncio.new_event_loop()
+        kw = {}
+        if sys.version_info[:2] < (3, 10):
+            kw["loop"] = loop
+        evt = asyncio.Event(**kw)
 
         async def evt_wait():
             await evt.wait()
 
         try:
             while True:
                 coro = loop.create_connection(lambda: SNXHandler(vna_obj, sd.cookie, slim_ver, rl, evt), \
@@ -405,14 +446,19 @@
     parser.add_argument("--ike", default=0, type=int, help="IKE mode switch. If not zero selects IKE version to use to setup vpn tunnel. Valid values are: 0(default),1,2. Implies -t esp.")
     parser.add_argument("--ct", default="TRAC", type=str, help="Client type: TRAC, SYMBIAN, etc.")
     parser.add_argument("-i", "--interface", type=str, help="Use given name for tunnel interface instead of default one.")
     group = parser.add_mutually_exclusive_group(required=utils.is_mac)
     group.add_argument("-S", "--script-tun", dest="script_tun", type=str, help="Pass traffic to 'script' program, instead of tun.")
     group.add_argument("-s", "--script", type=str, help="Shell command line for using a vpnc-compatible config script.")
 
+    parser.add_argument("--daemon", action='store_true', default=False, help="Run in the background after login.")
+    parser.add_argument("--pidfile", type=str, help="File to store main process id.")
+    parser.add_argument("--logfile", type=str, help="File to store output after user login. To be used with the --daemon option.")
+    parser.add_argument("--null_vna", action='store_true', default=False, help=argparse.SUPPRESS)
+
     # Certificate  enrollment support
     parser.add_argument("--enroll", action='store_true', default=False, help="Set enrollment key.")
     parser.add_argument("--rc", type=str, help="P12 certificate file to renew.")
 
     utils.add_common_args(parser)
     options = parser.parse_args()
     options.ui = cui.TUI()
@@ -421,18 +467,18 @@
         utils.setup_loglevel(options)
         manage_cert(options)
         return
 
     if options.user_cert:
         options.mode = 'c'
 
-    utils.client_setup(options)
+    options.defhandler = utils.client_setup(options)
 
     vna_args = {}
-    for k in ["interface", "script", "script_tun"]:
+    for k in ["interface", "script", "script_tun","null_vna"]:
         v = getattr(options, k)
         if v:
             vna_args[k] = v
 
     vpn_main(options, vna_args)
```

### Comparing `cpyvpn-1.6/cpyvpn/crt.py` & `cpyvpn-1.6.1/cpyvpn/crt.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/cui.py` & `cpyvpn-1.6.1/cpyvpn/cui.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/ma.py` & `cpyvpn-1.6.1/cpyvpn/ma.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,15 @@
         #  6 - Dynamic ID (delivered by SMS/Email)
 
         if amt == 8:
             raise RuntimeError("SAML mode not supported. Use regular browser-based login and pass browser cookies to client to init tunnel.")
 
         self.enc = enc = RSAEnc (self.modulus, self.exponent)
         if amt == 3:
+            ssl_ctx.require_user_cert()
             cert_path = self.args.filepref + "/Login/LoginWithCert?selectedRealm=" + selectedRealm
             self._do_request(cert_path)  # Full path here!
             self.nextfile = self.purl
             return
 
         if amt not in [1, 3] and not loginType:
             loginType = "Standard"
```

### Comparing `cpyvpn-1.6/cpyvpn/rsa.py` & `cpyvpn-1.6.1/cpyvpn/rsa.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/snx.py` & `cpyvpn-1.6.1/cpyvpn/snx.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/srv/data/cert.pem` & `cpyvpn-1.6.1/cpyvpn/srv/data/cert.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/srv/data/cl_cert.pem` & `cpyvpn-1.6.1/cpyvpn/srv/data/cl_cert.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/srv/data/cl_key.pem` & `cpyvpn-1.6.1/cpyvpn/srv/data/cl_key.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/srv/data/key.pem` & `cpyvpn-1.6.1/cpyvpn/srv/data/key.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/srv/data/rr.js` & `cpyvpn-1.6.1/cpyvpn/srv/data/rr.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -81,14 +81,27 @@
                                         "username": "\"Login\"",
                                         "password": "Password"
                                     }
                                 }
                             }
                         },
                         "2": {
+                            "id": "vpn_cert",
+                            "secondary_realm_hash": "00112233445566778899aabbccddeeff",
+                            "display_name": "Cert",
+                            "show_realm": 1,
+                            "factors": {
+                                "0": {
+                                    "factor_type": "certificate",
+                                    "securid_card_type": "",
+                                    "certificate_storage_type": ""
+                                }
+                            }
+                        },
+                        "3": {
                             "id": "vpn_2fa",
                             "secondary_realm_hash": "00112233445566778899aabbccddeeff",
                             "display_name": "SMS",
                             "show_realm": 1,
                             "factors": {
                                 "0": {
                                     "factor_type": "password",
```

### Comparing `cpyvpn-1.6/cpyvpn/srv/data/rsa.keys` & `cpyvpn-1.6.1/cpyvpn/srv/data/rsa.keys`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/srv/server.py` & `cpyvpn-1.6.1/cpyvpn/srv/server.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/ssl_ctx.py` & `cpyvpn-1.6.1/cpyvpn/ssl_ctx.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             pass
         try:
             with resources.path(pkg_data, 'cl_cert.pem') as certpem:
                 with resources.path(pkg_data, 'cl_key.pem') as keypem:
                         __ssl_cont__ .load_cert_chain(certpem, keypem)
         except:
             pass
+        __ssl_cont__.has_user_cert = False
 
     context = __ssl_cont__
     if __ssl_strict__:
         context.verify_mode = ssl.CERT_REQUIRED
     else:
         context.check_hostname = False
         context.verify_mode = ssl.CERT_NONE
@@ -148,7 +149,10 @@
                     _resolve_cert_chain((host, port))
                     _test_wrap(host, port)
                 else:
                     ssl_strict = False
         set_ssl_strict_mode(ssl_strict)
         logger.info("SSL mode is: {}.".format("strict" if ssl_strict else "permissive"))
 
+def require_user_cert():
+    if not get_ssl_context().has_user_cert:
+        raise RuntimeError("Certificate-based login mode selected, but user certificate is not set! Use '-c' option.")
```

### Comparing `cpyvpn-1.6/cpyvpn/trutils.py` & `cpyvpn-1.6.1/cpyvpn/trutils.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/cpyvpn/utils.py` & `cpyvpn-1.6.1/cpyvpn/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,15 @@
     def ask_cert_pwd():
         q = options.ui.ask_pwd("Certificate password")
         return options.ui.wait_input([q])[0]
 
     if options.user_cert:
         ctx = ssl_ctx.get_ssl_context()
         ctx.load_cert_chain(options.user_cert, password=ask_cert_pwd)
+        ctx.has_user_cert = True
 
     p = urlparse(add_slash(options.server))
     if p.scheme or p.path:
         options.server = p.netloc
     if p.path:
         options.path = p.path
         if hasattr(options, "mode"):
@@ -303,15 +304,15 @@
         options.pwd = options.ui.wait_input([q])[0]
     elif options.script_pwd:
         options.pwd = subprocess.check_output(shlex.split(options.script_pwd), text=True)
     return setup_loglevel(options, add_handler)
 
 
 def print_close_info():
-    logger.info("Press Ctrl-C or send SIGINT signal to stop this process (pid={}).".format(os.getpid()))
+    logger.info("Press Ctrl-C or send SIGINT signal to stop this process (pid: {}).".format(os.getpid()))
 
 
 __SIGLIST__ = (signal.SIGINT, signal.SIGTERM)
 
 try:
     #posix
     __SIGLIST__ += (signal.SIGQUIT,)
```

### Comparing `cpyvpn-1.6/cpyvpn/vna.py` & `cpyvpn-1.6.1/cpyvpn/vna.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,19 +484,23 @@
     def down(self):
         if self._sc_proc:
             os.killpg(self._sc_proc.pid, signal.SIGHUP)
         self.dev.close()
 
 
 def init_vna(args):
-    cls_list = [VNAProxy, VNAVPNC, VNANM, VNANull]
-    if args.get("null"):
+    cls_list = [VNAProxy, VNAVPNC, VNANM]
+
+    if args.get("null_vna"):
         cls_list = [VNANull]
+    inst = None
     for cls in cls_list:
         try:
             inst = cls(args)
             break
         except:
             pass
     if isinstance(inst, VNANull):
         logger.warning("Initializing null VNA for debugging. Network packet transfer won't be available.")
+    if inst is None:
+        raise RuntimeError("VNA initialisation failed! Check your -s/-S option, make sure Network Manager can handle TUN interfaces, use --null_vna hidden option.")
     return inst
```

### Comparing `cpyvpn-1.6/cpyvpn.egg-info/PKG-INFO` & `cpyvpn-1.6.1/cpyvpn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpyvpn
-Version: 1.6
+Version: 1.6.1
 Summary: Check Point VPN client written in Python.
 Home-page: https://gitlab.com/cpvpn/cpyvpn
 Author: Nikolay A. Krylov
 Author-email: krylovna@gmail.com
 License: GPL3
 Project-URL: PyPI, https://pypi.org/project/cpyvpn
 Project-URL: Source, https://gitlab.com/cpvpn/cpyvpn
@@ -108,14 +108,17 @@
 
     `cp_client -m l -u testuser vpn.example.org`
 
 * TRAC login with realm and predefined user name:
 
     `cp_client --realm vpn -u testuser vpn.example.org`
 
+* TRAC login with the predefined user name, run in the background after user authication, redirect output to cp.log and save background process pid to the cp.pid file:
+
+    `cp_client --daemon --logfile=./cp.log --pidfile=./cp.pid -u testuser vpn.example.org`
 * TRAC login with predefined user name and password from external program:
 
     `cp_client -u user --passwd-script 'kwallet-query kdewallet' vpn.example.org`
 
 * TRAC login with certificate as a first factor:
 
     `cp_client -c cert.pem vpn.example.org`
```

### Comparing `cpyvpn-1.6/cpyvpn.egg-info/SOURCES.txt` & `cpyvpn-1.6.1/cpyvpn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/setup.cfg` & `cpyvpn-1.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6/setup.py` & `cpyvpn-1.6.1/setup.py`

 * *Files identical despite different names*

