# Comparing `tmp/yplib-2.5.5.tar.gz` & `tmp/yplib-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.5.5.tar", last modified: Mon Jul 17 00:21:59 2023, max compression
+gzip compressed data, was "dist\yplib-2.5.6.tar", last modified: Mon Jul 17 00:27:31 2023, max compression
```

## Comparing `yplib-2.5.5.tar` & `yplib-2.5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 00:21:59.837679 yplib-2.5.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-17 00:21:59.837351 yplib-2.5.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 00:21:59.837679 yplib-2.5.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-17 00:19:43.000000 yplib-2.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:21:59.833989 yplib-2.5.5/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.5/yplib/db.py
--rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.5/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    33707 2023-07-17 00:19:10.000000 yplib-2.5.5/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.5/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:21:59.836460 yplib-2.5.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 00:21:59.000000 yplib-2.5.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 00:27:31.638813 yplib-2.5.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-17 00:27:31.638813 yplib-2.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 00:27:31.638813 yplib-2.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-17 00:26:41.000000 yplib-2.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:27:31.636196 yplib-2.5.6/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.6/yplib/db.py
+-rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.6/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33939 2023-07-17 00:26:17.000000 yplib-2.5.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:27:31.638477 yplib-2.5.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-17 00:27:31.000000 yplib-2.5.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-17 00:27:31.000000 yplib-2.5.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:27:31.000000 yplib-2.5.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 00:27:31.000000 yplib-2.5.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.5.5/LICENSE` & `yplib-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/setup.py` & `yplib-2.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.5.5",
+  version="2.5.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.5.5/yplib/__init__.py` & `yplib-2.5.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/chart.py` & `yplib-2.5.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/chart_html.py` & `yplib-2.5.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/db.py` & `yplib-2.5.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/file.py` & `yplib-2.5.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/http_util.py` & `yplib-2.5.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/index.py` & `yplib-2.5.6/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,36 +44,36 @@
     return to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=False)
 
 
 # 将 log 数据, 写入到文件
 def to_print_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                   a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'print', True, '.txt')
+    to_txt(data_list=[lo], file_name=datetime.today().strftime('%Y-%m-%d'), file_path='print', fixed_name=True, suffix='.txt')
 
 
 # 将 log 数据, 写入到文件, 固定文件名称
 def to_print_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                  a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    to_txt([lo], file_name, 'print', True, '.txt')
+    to_txt(data_list=[lo], file_name=file_name, file_path='print', fixed_name=True, suffix='.txt')
 
 
 # 将 log 数据, 写入到文件
 def to_log_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=time_prefix)
-    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True, '.log')
+    to_txt(data_list=[lo], file_name=datetime.today().strftime('%Y-%m-%d'), file_path='log', fixed_name=True, suffix='.log')
 
 
 # 将 log 数据, 写入到固定文件中
 def to_log_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=time_prefix)
-    to_txt([lo], file_name, 'log', True, '.txt')
+    to_txt(data_list=[lo], file_name=file_name, file_path='log', fixed_name=True, suffix='.txt')
 
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
 def to_hump_one(s):
     if s is None or s == '':
@@ -369,15 +369,15 @@
     text_file.close()
     return file_name_path
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
 def to_txt_file(data_list, file_name=None):
     file_name = datetime.today().strftime('%Y%m%d_%H%M') if file_name is None else file_name
-    return to_txt(data_list, file_name, 'data', True)
+    return to_txt(data_list=data_list, file_name=file_name, file_path='txt', fixed_name=True)
 
 
 # 转化成字符串
 def to_str(data):
     if can_use_json(data):
         s = json.dumps(data)
     else:
```

### Comparing `yplib-2.5.5/yplib/mail.py` & `yplib-2.5.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/mail_html.py` & `yplib-2.5.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.5/yplib/markdown.py` & `yplib-2.5.6/yplib/markdown.py`

 * *Files identical despite different names*

