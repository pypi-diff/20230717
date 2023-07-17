# Comparing `tmp/q2gui-0.1.98.tar.gz` & `tmp/q2gui-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.98.tar", max compression
+gzip compressed data, was "q2gui-0.1.99.tar", max compression
```

## Comparing `q2gui-0.1.98.tar` & `q2gui-0.1.99.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.98/LICENSE
--rw-r--r--   0        0        0      576 2023-07-03 21:34:52.823611 q2gui-0.1.98/pyproject.toml
--rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.98/q2gui/__init__.py
--rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.98/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.98/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    23550 2023-07-03 21:07:47.237275 q2gui-0.1.98/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.98/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.98/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.98/q2gui/pyqt6/q2style.py
--rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.98/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4982 2023-07-03 11:10:22.540807 q2gui-0.1.98/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.98/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.98/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.98/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0    17484 2023-07-03 20:59:01.419271 q2gui-0.1.98/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.98/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.98/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.98/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.98/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.98/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.98/q2gui/pyqt6/widgets/q2image.py
--rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.98/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.98/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.98/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.98/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.98/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.98/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.98/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.98/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.98/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0     1118 2023-07-01 10:11:15.099025 q2gui-0.1.98/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.98/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     3934 2023-07-01 14:42:37.242752 q2gui-0.1.98/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.98/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.98/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.98/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    21339 2023-07-03 21:27:23.492605 q2gui-0.1.98/q2gui/q2app.py
--rw-r--r--   0        0        0    12944 2023-07-02 22:59:21.715306 q2gui-0.1.98/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    71919 2023-07-03 21:21:54.725101 q2gui-0.1.98/q2gui/q2form.py
--rw-r--r--   0        0        0    15855 2023-07-02 15:02:12.981402 q2gui-0.1.98/q2gui/q2model.py
--rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.98/q2gui/q2style.py
--rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.98/q2gui/q2utils.py
--rw-r--r--   0        0        0     6408 2023-07-03 13:46:38.975913 q2gui-0.1.98/q2gui/q2widget.py
--rw-r--r--   0        0        0     3847 2023-07-03 13:03:58.855238 q2gui-0.1.98/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2023-07-03 21:34:55.369573 q2gui-0.1.98/q2gui/version.py
--rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.98/README.md
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.99/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-04 21:58:22.819098 q2gui-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.99/q2gui/__init__.py
+-rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.99/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.99/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    23550 2023-07-04 21:49:21.087492 q2gui-0.1.99/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.99/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.99/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.99/q2gui/pyqt6/q2style.py
+-rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.99/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4982 2023-07-03 11:10:22.540807 q2gui-0.1.99/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.99/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.99/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.99/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0    17484 2023-07-03 20:59:01.419271 q2gui-0.1.99/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.99/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.99/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.99/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.99/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.99/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.99/q2gui/pyqt6/widgets/q2image.py
+-rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.99/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.99/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.99/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.99/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.99/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.99/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.99/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.99/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.99/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0     1118 2023-07-01 10:11:15.099025 q2gui-0.1.99/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.99/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     3934 2023-07-01 14:42:37.242752 q2gui-0.1.99/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.99/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.99/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.99/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    21418 2023-07-04 21:57:42.921137 q2gui-0.1.99/q2gui/q2app.py
+-rw-r--r--   0        0        0    12944 2023-07-02 22:59:21.715306 q2gui-0.1.99/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    71959 2023-07-04 21:58:07.101786 q2gui-0.1.99/q2gui/q2form.py
+-rw-r--r--   0        0        0    15855 2023-07-02 15:02:12.981402 q2gui-0.1.99/q2gui/q2model.py
+-rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.99/q2gui/q2style.py
+-rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.99/q2gui/q2utils.py
+-rw-r--r--   0        0        0     6408 2023-07-03 13:46:38.975913 q2gui-0.1.99/q2gui/q2widget.py
+-rw-r--r--   0        0        0     3847 2023-07-03 13:03:58.855238 q2gui-0.1.99/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2023-07-04 21:58:25.600297 q2gui-0.1.99/q2gui/version.py
+-rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.99/README.md
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.99/PKG-INFO
```

### Comparing `q2gui-0.1.98/LICENSE` & `q2gui-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/pyproject.toml` & `q2gui-0.1.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2gui"
-version = "0.1.98"
+version = "0.1.99"
 description = "Python GUI toolkit"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
```

### Comparing `q2gui-0.1.98/q2gui/__main__.py` & `q2gui-0.1.99/q2gui/__main__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/q2app.py` & `q2gui-0.1.99/q2gui/pyqt6/q2app.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/q2form.py` & `q2gui-0.1.99/q2gui/pyqt6/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/q2model.py` & `q2gui-0.1.99/q2gui/pyqt6/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/q2style.py` & `q2gui-0.1.99/q2gui/pyqt6/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.99/q2gui/pyqt6/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/q2window.py` & `q2gui-0.1.99/q2gui/pyqt6/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/__init__.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2button.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2button.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2check.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2code.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2code.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2combo.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2combo.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2date.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2date.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2doublespin.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2doublespin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2frame.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2grid.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2grid.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2image.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2image.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2label.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2line.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2list.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2list.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2progressbar.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2progressbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2radio.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2radio.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2relation.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2relation.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2scroller.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2scroller.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2sheet.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2sheet.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2space.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2space.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2spin.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2spin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2tab.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2tab.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2text.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2text.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2toolbar.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2toolbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.99/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/q2app.py` & `q2gui-0.1.99/q2gui/q2app.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,18 @@
 
     def __init__(self):
         self.c = self._C(self)
 
     def get(self, name):
         return self.c.__getattr__(name)
 
+    def delete(self, name):
+        c = self.get(name)
+        self.pop(self.index(c))
+
     def get_names(self):
         return [line["column"] for line in self]
 
     # def __getitem__(self, list_index):
     #     if isinstance(list_index, str):  # not index but name - return index for name
     #         for x in range(len(self)):
     #             if list_index == self[x].get("column"):
@@ -419,15 +423,15 @@
                     meta["datalen"] = 1
                 elif meta.get("control") in ("line"):
                     meta["datalen"] = 100
         return meta
 
 
 class Q2Settings:
-    def __init__(self, filename="", app_name=""):
+    def __init__(self, filename=""):
         self.filename = filename if filename else "q2gui.ini"
         self.config = ConfigParser()
         self.read()
 
     def read(self):
         if self.filename in ("none", "memory"):
             self.filename = io.StringIO("")
```

### Comparing `q2gui-0.1.98/q2gui/q2dialogs.py` & `q2gui-0.1.99/q2gui/q2dialogs.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/q2form.py` & `q2gui-0.1.99/q2gui/q2form.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,18 @@
 
     def set_model(self, model):
         self.model: Q2Model = model
         self.model.q2_form = self
         return self.model
 
     def refresh(self):
+        row = self.current_row
+        col = self.current_column
         self._q2dialogs.q2working(lambda: (self.model.refresh(), self.refresh_children()), _("Refreshing..."))
-        self.set_grid_index()
+        self.set_grid_index(row, col)
 
     def widget(self):
         if self.form_stack:
             return self.form_stack[-1]
 
     def widgets(self):
         if self.form_stack:
@@ -550,15 +552,14 @@
             label=q2app.CRUD_BUTTON_CANCEL_TEXT,
             control="button",
             mess=q2app.CRUD_BUTTON_CANCEL_MESSAGE,
             # valid=self.crud_close,
             valid=self.close,
         )
         buttons.add_control("/")
-        buttons.add_control("/s")
         self.system_controls = buttons
 
     def crud_view_to_edit(self):
         self.crud_form.set_title(f"{self.title}.[EDIT]")
         self.w._ok_button.set_enabled(True)
         self.w._prev_button.set_enabled(False)
         self.w._next_button.set_enabled(False)
```

### Comparing `q2gui-0.1.98/q2gui/q2model.py` & `q2gui-0.1.99/q2gui/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/q2style.py` & `q2gui-0.1.99/q2gui/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/q2utils.py` & `q2gui-0.1.99/q2gui/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/q2widget.py` & `q2gui-0.1.99/q2gui/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/q2gui/q2window.py` & `q2gui-0.1.99/q2gui/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/README.md` & `q2gui-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.98/PKG-INFO` & `q2gui-0.1.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.98
+Version: 0.1.99
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

