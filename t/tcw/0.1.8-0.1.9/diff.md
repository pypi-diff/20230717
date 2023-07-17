# Comparing `tmp/tcw-0.1.8.tar.gz` & `tmp/tcw-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcw-0.1.8.tar", last modified: Mon Jul 17 11:04:41 2023, max compression
+gzip compressed data, was "tcw-0.1.9.tar", last modified: Mon Jul 17 12:54:44 2023, max compression
```

## Comparing `tcw-0.1.8.tar` & `tcw-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.650390 tcw-0.1.8/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.8/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-07-17 11:04:41.650390 tcw-0.1.8/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.8/README.md
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-07-17 11:04:41.650390 tcw-0.1.8/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      596 2023-07-17 11:02:01.000000 tcw-0.1.8/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.642390 tcw-0.1.8/tcw/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.8/tcw/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.642390 tcw-0.1.8/tcw/apps/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.646390 tcw-0.1.8/tcw/apps/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1208 2023-05-25 14:21:10.000000 tcw-0.1.8/tcw/apps/contest/forms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3853 2023-05-25 15:11:54.000000 tcw-0.1.8/tcw/apps/contest/models.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.646390 tcw-0.1.8/tcw/apps/contest/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/contest/templates/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.650390 tcw-0.1.8/tcw/apps/contest/templates/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1547 2023-04-04 23:59:46.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/about.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5820 2023-04-13 13:07:38.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/animation.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2078 2023-04-05 05:32:34.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/form.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      303 2023-04-06 18:51:38.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/index.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2222 2023-04-07 12:49:55.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/privacy.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2302 2023-05-12 04:16:15.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/signup.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1735 2023-04-13 13:03:09.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/slide1.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      562 2023-04-13 13:03:16.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/slide2.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      219 2023-04-13 13:03:04.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/slide3.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/sorry.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2569 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/success.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      408 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/apps/contest/templates/contest/thanks.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3533 2023-05-25 14:59:11.000000 tcw-0.1.8/tcw/apps/contest/views.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1245 2023-05-25 14:53:59.000000 tcw-0.1.8/tcw/config.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1067 2023-05-25 15:47:01.000000 tcw-0.1.8/tcw/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-05-25 14:48:34.000000 tcw-0.1.8/tcw/exc.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      159 2023-05-25 14:57:02.000000 tcw-0.1.8/tcw/run.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.650390 tcw-0.1.8/tcw/static/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/static/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.650390 tcw-0.1.8/tcw/static/images/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/static/images/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.650390 tcw-0.1.8/tcw/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1971 2023-04-04 18:51:43.000000 tcw-0.1.8/tcw/templates/404.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1960 2023-04-05 14:13:22.000000 tcw-0.1.8/tcw/templates/410.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.8/tcw/templates/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2315 2023-07-17 11:01:32.000000 tcw-0.1.8/tcw/templates/base.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1606 2023-05-25 14:39:49.000000 tcw-0.1.8/tcw/utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-05-25 14:27:27.000000 tcw-0.1.8/tcw/wsgi.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 11:04:41.642390 tcw-0.1.8/tcw.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-07-17 11:04:41.000000 tcw-0.1.8/tcw.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-07-17 11:04:41.000000 tcw-0.1.8/tcw.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-07-17 11:04:41.000000 tcw-0.1.8/tcw.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-07-17 11:04:41.000000 tcw-0.1.8/tcw.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-07-17 11:04:41.000000 tcw-0.1.8/tcw.egg-info/top_level.txt
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:44.002301 tcw-0.1.9/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.9/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-07-17 12:54:44.002301 tcw-0.1.9/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.9/README.md
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-07-17 12:54:44.002301 tcw-0.1.9/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      596 2023-07-17 12:53:31.000000 tcw-0.1.9/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:43.994301 tcw-0.1.9/tcw/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.9/tcw/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:43.994301 tcw-0.1.9/tcw/apps/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:43.998301 tcw-0.1.9/tcw/apps/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1208 2023-05-25 14:21:10.000000 tcw-0.1.9/tcw/apps/contest/forms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3853 2023-05-25 15:11:54.000000 tcw-0.1.9/tcw/apps/contest/models.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:43.998301 tcw-0.1.9/tcw/apps/contest/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/contest/templates/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:44.002301 tcw-0.1.9/tcw/apps/contest/templates/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1547 2023-04-04 23:59:46.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/about.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5820 2023-04-13 13:07:38.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/animation.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2078 2023-04-05 05:32:34.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/form.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      303 2023-04-06 18:51:38.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/index.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2222 2023-04-07 12:49:55.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/privacy.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2302 2023-05-12 04:16:15.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/signup.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1735 2023-04-13 13:03:09.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/slide1.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      562 2023-04-13 13:03:16.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/slide2.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      219 2023-04-13 13:03:04.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/slide3.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/sorry.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2569 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/success.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      408 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/apps/contest/templates/contest/thanks.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3533 2023-05-25 14:59:11.000000 tcw-0.1.9/tcw/apps/contest/views.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1245 2023-05-25 14:53:59.000000 tcw-0.1.9/tcw/config.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1067 2023-05-25 15:47:01.000000 tcw-0.1.9/tcw/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-05-25 14:48:34.000000 tcw-0.1.9/tcw/exc.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      159 2023-05-25 14:57:02.000000 tcw-0.1.9/tcw/run.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:44.002301 tcw-0.1.9/tcw/static/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/static/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:44.002301 tcw-0.1.9/tcw/static/images/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/static/images/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:44.002301 tcw-0.1.9/tcw/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1971 2023-04-04 18:51:43.000000 tcw-0.1.9/tcw/templates/404.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1960 2023-04-05 14:13:22.000000 tcw-0.1.9/tcw/templates/410.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.9/tcw/templates/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2154 2023-07-17 11:19:46.000000 tcw-0.1.9/tcw/templates/base.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1606 2023-05-25 14:39:49.000000 tcw-0.1.9/tcw/utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-05-25 14:27:27.000000 tcw-0.1.9/tcw/wsgi.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-17 12:54:43.994301 tcw-0.1.9/tcw.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-07-17 12:54:43.000000 tcw-0.1.9/tcw.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-07-17 12:54:43.000000 tcw-0.1.9/tcw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-07-17 12:54:43.000000 tcw-0.1.9/tcw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-07-17 12:54:43.000000 tcw-0.1.9/tcw.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-07-17 12:54:43.000000 tcw-0.1.9/tcw.egg-info/top_level.txt
```

### Comparing `tcw-0.1.8/LICENSE` & `tcw-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/PKG-INFO` & `tcw-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.8
+Version: 0.1.9
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.8/README.md` & `tcw-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/setup.py` & `tcw-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tcw',
-    version='0.1.8',
+    version='0.1.9',
     author='J Leary',
     author_email='tinycontestwinners@gmail.com',
     description='tiny contest winners application',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(),
```

### Comparing `tcw-0.1.8/tcw/__init__.py` & `tcw-0.1.9/tcw/__init__.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/forms.py` & `tcw-0.1.9/tcw/apps/contest/forms.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/models.py` & `tcw-0.1.9/tcw/apps/contest/models.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/about.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/about.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/animation.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/animation.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/form.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/form.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/privacy.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/privacy.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/signup.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/signup.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/slide1.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/slide1.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/slide2.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/slide2.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/templates/contest/success.html` & `tcw-0.1.9/tcw/apps/contest/templates/contest/success.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/apps/contest/views.py` & `tcw-0.1.9/tcw/apps/contest/views.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/config.py` & `tcw-0.1.9/tcw/config.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/database.py` & `tcw-0.1.9/tcw/database.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/templates/404.html` & `tcw-0.1.9/tcw/templates/404.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/templates/410.html` & `tcw-0.1.9/tcw/templates/410.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw/templates/base.html` & `tcw-0.1.9/tcw/templates/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,14 @@
                 <span class="small">Create fun raffles and contests</span>
             </div>
         </nav>
         <div class="container-md mt-4" style="margin-bottom: 5.0rem;">
             {% block content %}
             {% endblock content %}
         </div>
-        <!-- Ezoic - mid_content - mid_content -->
-        <div id="ezoic-pub-ad-placeholder-102"> </div>
-        <!-- End Ezoic - mid_content - mid_content -->
         <footer class="footer fixed-bottom" style="background: #EEE;">
             <ul class="nav justify-content-center">
                 <li class=nav-item><a href="{{ url_for('contest.index') }}" class="nav-link px-2 text-muted">&copy; 2022 Tiny Contest Winners</a></li>
                 <li class="nav-item"><a href="{{ url_for('contest.privacy') }}" class="nav-link px-2 text-muted">Privacy</a></li>
                 <li class="nav-item"><a href="{{ url_for('contest.about') }}" class="nav-link px-2 text-muted">About</a></li>
             </ul>
         </footer>
```

#### html2text {}

```diff
@@ -2,11 +2,10 @@
 
 
 
 
 ;">
 Tiny_Contest_Winners! Create fun raffles and contests
 {% block content %} {% endblock content %}
-
     * ©_2022_Tiny_Contest_Winners
     * Privacy
     * About
```

### Comparing `tcw-0.1.8/tcw/utils.py` & `tcw-0.1.9/tcw/utils.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.8/tcw.egg-info/PKG-INFO` & `tcw-0.1.9/tcw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.8
+Version: 0.1.9
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.8/tcw.egg-info/SOURCES.txt` & `tcw-0.1.9/tcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

