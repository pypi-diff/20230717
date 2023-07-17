# Comparing `tmp/yplib-2.5.4.tar.gz` & `tmp/yplib-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.5.4.tar", last modified: Mon Jul 17 00:17:18 2023, max compression
+gzip compressed data, was "dist\yplib-2.5.5.tar", last modified: Mon Jul 17 00:21:59 2023, max compression
```

## Comparing `yplib-2.5.4.tar` & `yplib-2.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 00:17:18.740931 yplib-2.5.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-17 00:17:18.740829 yplib-2.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 00:17:18.740931 yplib-2.5.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-17 00:16:48.000000 yplib-2.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:17:18.738373 yplib-2.5.4/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.4/yplib/db.py
--rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.4/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    33708 2023-07-17 00:16:13.000000 yplib-2.5.4/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.4/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.4/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.4/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.4/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:17:18.740342 yplib-2.5.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-17 00:17:18.000000 yplib-2.5.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-17 00:17:18.000000 yplib-2.5.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 00:17:18.000000 yplib-2.5.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 00:17:18.000000 yplib-2.5.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 00:21:59.837679 yplib-2.5.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-17 00:21:59.837351 yplib-2.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 00:21:59.837679 yplib-2.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-17 00:19:43.000000 yplib-2.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:21:59.833989 yplib-2.5.5/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.5/yplib/db.py
+-rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.5/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33707 2023-07-17 00:19:10.000000 yplib-2.5.5/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.5/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.5/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.5/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.5/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:21:59.836460 yplib-2.5.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.5.4/LICENSE` & `yplib-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/setup.py` & `yplib-2.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.5.4",
+  version="2.5.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.5.4/yplib/__init__.py` & `yplib-2.5.5/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/chart.py` & `yplib-2.5.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/chart_html.py` & `yplib-2.5.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/db.py` & `yplib-2.5.5/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/file.py` & `yplib-2.5.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/http_util.py` & `yplib-2.5.5/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/index.py` & `yplib-2.5.5/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
             else:
                 text_file.write(to_str(one) + '\n')
     text_file.close()
     return file_name_path
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
-def to_data_file(data_list, file_name=None):
+def to_txt_file(data_list, file_name=None):
     file_name = datetime.today().strftime('%Y%m%d_%H%M') if file_name is None else file_name
     return to_txt(data_list, file_name, 'data', True)
 
 
 # 转化成字符串
 def to_str(data):
     if can_use_json(data):
```

### Comparing `yplib-2.5.4/yplib/mail.py` & `yplib-2.5.5/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/mail_html.py` & `yplib-2.5.5/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.4/yplib/markdown.py` & `yplib-2.5.5/yplib/markdown.py`

 * *Files identical despite different names*

