# Comparing `tmp/osaapi-0.4.4.tar.gz` & `tmp/osaapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osaapi-0.4.4.tar", last modified: Wed Aug 16 12:13:13 2017, max compression
+gzip compressed data, was "osaapi-1.0.0.tar", max compression
```

## Comparing `osaapi-0.4.4.tar` & `osaapi-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,5 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-08-16 12:13:13.000000 osaapi-0.4.4/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-08-16 12:13:13.000000 osaapi-0.4.4/osaapi/
--rw-r--r--   0 travis    (1000) travis    (1000)    55026 2017-08-16 12:13:02.000000 osaapi-0.4.4/osaapi/__init__.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-08-16 12:13:13.000000 osaapi-0.4.4/osaapi.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)    10226 2017-08-16 12:13:13.000000 osaapi-0.4.4/osaapi.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      169 2017-08-16 12:13:13.000000 osaapi-0.4.4/osaapi.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-08-16 12:13:13.000000 osaapi-0.4.4/osaapi.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        7 2017-08-16 12:13:13.000000 osaapi-0.4.4/osaapi.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       32 2017-08-16 12:13:02.000000 osaapi-0.4.4/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     7282 2017-08-16 12:13:02.000000 osaapi-0.4.4/README.md
--rw-r--r--   0 travis    (1000) travis    (1000)     1102 2017-08-16 12:13:02.000000 osaapi-0.4.4/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10226 2017-08-16 12:13:13.000000 osaapi-0.4.4/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       59 2017-08-16 12:13:13.000000 osaapi-0.4.4/setup.cfg
+-rw-r--r--   0        0        0    11320 2023-07-17 13:48:35.795511 osaapi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7286 2023-07-17 13:48:35.795511 osaapi-1.0.0/README.md
+-rw-r--r--   0        0        0    55239 2023-07-17 13:48:35.795511 osaapi-1.0.0/osaapi/__init__.py
+-rw-r--r--   0        0        0     1250 2023-07-17 13:48:58.787456 osaapi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 osaapi-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `osaapi-0.4.4/osaapi/__init__.py` & `osaapi-1.0.0/osaapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import random
 import string
 import sys
 import time
 import uuid
 
+
 if sys.version_info[0] < 3:
     import xmlrpclib as client
 else:
     from xmlrpc import client
 
 
 def rand_id(max_size=10, chars=string.ascii_uppercase + string.digits):
@@ -1407,14 +1408,20 @@
         def __init__(self, conn):
             self.__server__ = conn.__server__
             self.__server__._ServerProxy__verbose = conn.__server__._ServerProxy__verbose
 
         def rescheduleTask(self, **kwargs):
             return self.__server__.pem.tasks.rescheduleTask(kwargs)
 
+        def getTaskLog(self, **kwargs):
+            return self.__server__.pem.tasks.getTaskLog(kwargs)
+
+        def cancelJob(self, **kwargs):
+            return self.__server__.pem.tasks.cancelJob(kwargs)
+
     def create_account(self, first_name=None, last_name=None, account_type='C',
                        branded_domain=None, parent_account_id=None, **kwargs):
         """
         Possible values for the account_type:
             'C': Indicates that the Account is created for Customer. Default value.
             'R': Indicates that the Account is created for Reseller.
         If company param is present in call, this one is bypassed to openapi call, this one
@@ -1444,15 +1451,15 @@
             4, string.digits), 'phone_num': rand_id(10, string.digits), 'ext_num': ''}
 
         data = {
             'account_type': account_type,
             'person': person,
             'address': kwargs.get('address', address),
             'phone': kwargs.get('phone', phone),
-            'email': kwargs.get('email', '%s@%s.com' % (rand_id(10), rand_id(8)))
+            'email': kwargs.get('email', '%s@%s.com' % (rand_id(10), rand_id(8))),
         }
 
         if branded_domain:
             data['branded_domain'] = branded_domain
 
         if parent_account_id:
             data['parent_account_id'] = parent_account_id
@@ -1469,31 +1476,31 @@
         _user_id = random.randint(2 ** 20, 2 ** 31 - 1)
 
         address = {
             'street_name': rand_id(10),
             'zipcode': rand_id(10, string.digits),
             'city': rand_id(10),
             'country': 'ru',
-            'state': rand_id(10)
+            'state': rand_id(10),
         }
         phone = {
             'country_code': rand_id(3, string.digits),
             'area_code': rand_id(4, string.digits),
             'phone_num': rand_id(10, string.digits),
-            'ext_num': ''
+            'ext_num': '',
         }
 
         member = self.addAccountMember(
             account_id=account_id,
             user_id=_user_id,
             auth={'login': login, 'password': password},
             person={'first_name': first_name, 'last_name': last_name},
             address=kwargs.get('address', address),
             phone=kwargs.get('phone', phone),
-            email=email
+            email=email,
         )
 
         # !ATTENTION!
         # user_id returned from the pem.addAccountMember call is not actualy user_id, but member_id
         # and needs to be translated to the real user_id via pem.getMemberFullInfo call
         # !ATTENTION!
```

### Comparing `osaapi-0.4.4/README.md` & `osaapi-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 osaAPI
 =====
 ![pyversions](https://img.shields.io/pypi/pyversions/osaapi.svg) [![Build Status](https://img.shields.io/travis/ingrammicro/osaAPI/master.svg)](https://travis-ci.org/ingrammicro/osaAPI) [![PyPi Status](https://img.shields.io/pypi/v/osaapi.svg)](https://pypi.python.org/pypi/osaapi)
 
 
-A python binding for the Odin Service Automation (OSA) and billing APIs.
+A python binding for the CloudBlue Commerce APIs a.k.a. Odin Service Automation or OSA.
 
 Installation
 ------------
 
 Using pip:
 
     $ pip install osaAPI
@@ -56,15 +56,15 @@
 ``` {.sourceCode .python}
 from osaapi import OSA, PBA
 
 # connect to OSA 
 pem = OSA('mn.hostname.com', port=8888)
 ```
 
-Odin Service Automation (OSA) API
+CloudBlue Commerce API
 -----------------------------------------
 
 All but three of the OSA API calls start with 'pem', for this reason it
 is recommended you name your OSA connection object 'pem' so you can call
 functions exactly how they are documented in the OSA API as has been
 done in the examples in this Readme.
```

