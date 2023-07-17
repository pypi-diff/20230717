# Comparing `tmp/flet_translator-1.0.tar.gz` & `tmp/flet_translator-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_translator-1.0.tar", last modified: Mon Jul 17 19:28:07 2023, max compression
+gzip compressed data, was "flet_translator-1.1.tar", last modified: Mon Jul 17 20:05:57 2023, max compression
```

## Comparing `flet_translator-1.0.tar` & `flet_translator-1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 19:28:07.609001 flet_translator-1.0/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1060 2023-05-22 08:17:53.000000 flet_translator-1.0/LICENSE
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       24 2023-07-17 14:01:21.000000 flet_translator-1.0/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4006 2023-07-17 19:28:07.608854 flet_translator-1.0/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3572 2023-07-17 19:27:21.000000 flet_translator-1.0/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 19:28:07.605988 flet_translator-1.0/flet_translator/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      181 2023-07-17 18:25:35.000000 flet_translator-1.0/flet_translator/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 19:28:07.607671 flet_translator-1.0/flet_translator/tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 14:06:54.000000 flet_translator-1.0/flet_translator/tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2544 2023-07-17 18:20:54.000000 flet_translator-1.0/flet_translator/tools/translate_control_content.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3294 2023-07-17 18:56:34.000000 flet_translator-1.0/flet_translator/tools/translate_page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      594 2023-07-17 15:49:29.000000 flet_translator-1.0/flet_translator/tools/translate_using_google.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      550 2023-07-17 18:20:17.000000 flet_translator-1.0/flet_translator/tools/translate_using_opusMT.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 19:28:07.608607 flet_translator-1.0/flet_translator/utils/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 14:06:50.000000 flet_translator-1.0/flet_translator/utils/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       69 2023-07-17 18:17:38.000000 flet_translator-1.0/flet_translator/utils/allowed_props_to_translate.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3447 2023-07-17 14:41:56.000000 flet_translator-1.0/flet_translator/utils/google_supported_langaues.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      328 2023-07-17 18:01:36.000000 flet_translator-1.0/flet_translator/utils/is_rtl.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-07-17 18:17:21.000000 flet_translator-1.0/flet_translator/utils/opusMT_supported_languages.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-17 19:28:07.606967 flet_translator-1.0/flet_translator.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4006 2023-07-17 19:28:07.000000 flet_translator-1.0/flet_translator.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      717 2023-07-17 19:28:07.000000 flet_translator-1.0/flet_translator.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-07-17 19:28:07.000000 flet_translator-1.0/flet_translator.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       40 2023-07-17 19:28:07.000000 flet_translator-1.0/flet_translator.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-07-17 19:28:07.000000 flet_translator-1.0/flet_translator.egg-info/top_level.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-22 08:19:03.000000 flet_translator-1.0/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-07-17 19:28:07.609048 flet_translator-1.0/setup.cfg
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      714 2023-07-17 18:22:44.000000 flet_translator-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:57.188024 flet_translator-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 20:05:42.000000 flet_translator-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 20:05:42.000000 flet_translator-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-17 20:05:57.188024 flet_translator-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-17 20:05:42.000000 flet_translator-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:57.188024 flet_translator-1.1/flet_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:57.188024 flet_translator-1.1/flet_translator/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/tools/translate_control_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/tools/translate_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/tools/translate_using_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/tools/translate_using_opusMT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:57.188024 flet_translator-1.1/flet_translator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/utils/allowed_props_to_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/utils/google_supported_langaues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/utils/is_rtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-17 20:05:42.000000 flet_translator-1.1/flet_translator/utils/opusMT_supported_languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:05:57.188024 flet_translator-1.1/flet_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-17 20:05:57.000000 flet_translator-1.1/flet_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 20:05:57.000000 flet_translator-1.1/flet_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:05:57.000000 flet_translator-1.1/flet_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 20:05:57.000000 flet_translator-1.1/flet_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 20:05:57.000000 flet_translator-1.1/flet_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 20:05:42.000000 flet_translator-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:05:57.188024 flet_translator-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-17 20:05:42.000000 flet_translator-1.1/setup.py
```

### Comparing `flet_translator-1.0/LICENSE` & `flet_translator-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/PKG-INFO` & `flet_translator-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_translator
-Version: 1.0
+Version: 1.1
 Summary: A package that help flet developers to make their apps support multiple languages
 Home-page: https://github.com/SKbarbon/flet_translator
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_translator-1.0/README.md` & `flet_translator-1.1/README.md`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/flet_translator/tools/translate_control_content.py` & `flet_translator-1.1/flet_translator/tools/translate_control_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     It create an attr (last_translated_texts:dict) in the control that stores the last translated
     texts so it reduces unnecessary translation requests.
     """
     
     # Check if the control is skiped so not translate it.
     if control in TranslateFletPage_class.skiped_controls: return
+    if control == None: return
 
     # start translating the control
     for p in allowed_props_to_translate:
         if hasattr(control, str(p)):
             value = getattr(control, str(p))
             if use_internet and value != None:
                 r = translate_using_google(
@@ -34,28 +35,29 @@
                     from_language=TranslateFletPage_class.from_language.value,
                     into_language=TranslateFletPage_class.into_language.value
                 )
                 setattr(control, str(p), str(r))
 
 
 
-    sub_controls_names = ["controls", "tabs"]
+    sub_controls_names = ["controls", "tabs", "actions"]
     for i in sub_controls_names:
         if hasattr(control, i):
             for i in getattr(control, str(i)):
                 threading.Thread(target=translate_control_content, kwargs={
                     "TranslateFletPage_class" : TranslateFletPage_class,
                     "control" : i,
                     "use_internet" : use_internet
                 }, daemon=True).start()
                 # translate_control_content(TranslateFletPage_class, i, use_internet)
     
-
-    if hasattr(control, "content"):
-        threading.Thread(target=translate_control_content, kwargs={
-                    "TranslateFletPage_class" : TranslateFletPage_class,
-                    "control" : getattr(control, "content"),
-                    "use_internet" : use_internet
-                }, daemon=True).start()
+    sub_contents_names = ["content", "leading", "title"]
+    for ic in sub_contents_names:
+        if hasattr(control, ic):
+            threading.Thread(target=translate_control_content, kwargs={
+                        "TranslateFletPage_class" : TranslateFletPage_class,
+                        "control" : getattr(control, ic),
+                        "use_internet" : use_internet
+                    }, daemon=True).start()
 
     if control.page != None:
         control.update()
```

### Comparing `flet_translator-1.0/flet_translator/tools/translate_page.py` & `flet_translator-1.1/flet_translator/tools/translate_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,24 @@
             )
 
 
 
     def translate_child_controls (self):
         if self.page.appbar != None:
             translate_control_content(self, control=self.page.appbar, use_internet=self.__use_internet)
+
+        if self.page.dialog != None:
+            translate_control_content(self, control=self.page.dialog, use_internet=self.__use_internet)
+        
+        if self.page.banner != None:
+            translate_control_content(self, control=self.page.banner, use_internet=self.__use_internet)
+        
+        if self.page.snack_bar != None:
+            translate_control_content(self, control=self.page.snack_bar, use_internet=self.__use_internet)
+
         for con in self.page.controls:
             threading.Thread(
                 target=translate_control_content,
                 args=[self],
                 kwargs={
                     "control" : con,
                     "use_internet" : self.__use_internet
```

### Comparing `flet_translator-1.0/flet_translator/tools/translate_using_google.py` & `flet_translator-1.1/flet_translator/tools/translate_using_google.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/flet_translator/tools/translate_using_opusMT.py` & `flet_translator-1.1/flet_translator/tools/translate_using_opusMT.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/flet_translator/utils/google_supported_langaues.py` & `flet_translator-1.1/flet_translator/utils/google_supported_langaues.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/flet_translator/utils/opusMT_supported_languages.py` & `flet_translator-1.1/flet_translator/utils/opusMT_supported_languages.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/flet_translator.egg-info/PKG-INFO` & `flet_translator-1.1/flet_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-translator
-Version: 1.0
+Version: 1.1
 Summary: A package that help flet developers to make their apps support multiple languages
 Home-page: https://github.com/SKbarbon/flet_translator
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_translator-1.0/flet_translator.egg-info/SOURCES.txt` & `flet_translator-1.1/flet_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flet_translator-1.0/setup.py` & `flet_translator-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_translator',
-    version='1.0',
+    version='1.1',
     author='SKbarbon',
     description='A package that help flet developers to make their apps support multiple languages',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_translator',
     install_requires=["flet", "EasyNMT", "sacremoses", "deep-translator"],
     packages=find_packages(),
```

