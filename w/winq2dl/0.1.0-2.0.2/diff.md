# Comparing `tmp/winq2dl-0.1.0.tar.gz` & `tmp/winq2dl-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winq2dl-0.1.0.tar", last modified: Mon Jul 17 07:12:27 2023, max compression
+gzip compressed data, was "winq2dl-2.0.2.tar", last modified: Mon Jul 17 07:15:38 2023, max compression
```

## Comparing `winq2dl-0.1.0.tar` & `winq2dl-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:12:27.891313 winq2dl-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 07:12:27.891313 winq2dl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-17 07:11:55.000000 winq2dl-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 07:11:55.000000 winq2dl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:12:27.891313 winq2dl-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 07:11:55.000000 winq2dl-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:12:27.891313 winq2dl-0.1.0/winq2dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 07:12:27.000000 winq2dl-0.1.0/winq2dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 07:12:27.000000 winq2dl-0.1.0/winq2dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:12:27.000000 winq2dl-0.1.0/winq2dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 07:12:27.000000 winq2dl-0.1.0/winq2dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 07:12:27.000000 winq2dl-0.1.0/winq2dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-17 07:11:55.000000 winq2dl-0.1.0/winq2dl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:15:38.790126 winq2dl-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 07:15:38.790126 winq2dl-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-17 07:15:28.000000 winq2dl-2.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 07:15:28.000000 winq2dl-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:15:38.790126 winq2dl-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 07:15:28.000000 winq2dl-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:15:38.790126 winq2dl-2.0.2/winq2dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-17 07:15:28.000000 winq2dl-2.0.2/winq2dl.py
```

### Comparing `winq2dl-0.1.0/setup.py` & `winq2dl-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `winq2dl-0.1.0/winq2dl.py` & `winq2dl-2.0.2/winq2dl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import ctypes
 import win32gui
 from ctypes import wintypes
 
-__version__ = "0.1.0"
+__version__ = "2.0.2"
 
 # Windows API Types
 CS_HREDRAW = 0x0002
 CS_VREDRAW = 0x0001
 LRESULT = ctypes.c_long
 CW_USEDEFAULT = -2147483648
 
@@ -63,17 +63,14 @@
         ctypes.windll.user32.EndPaint(hwnd, ctypes.byref(ps))
         return 0
     
     elif msg == 0x0010:  # WM_DESTROY
         ctypes.windll.user32.PostQuitMessage(0)
         return 0
     
-    elif msg == WM_MOUSEMOVE:
-        return 0  # Ignore the WM_MOUSEMOVE message
-    
     else:
         return ctypes.windll.user32.DefWindowProcW(hwnd, msg, wParam, lParam)
 
 class WNDCLASS(ctypes.Structure):
     _fields_ = [("style", wintypes.UINT),
                 ("lpfnWndProc", WNDPROC),
                 ("cbClsExtra", wintypes.INT),
```

