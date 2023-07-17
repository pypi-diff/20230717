# Comparing `tmp/flet_translator-1.2.tar.gz` & `tmp/flet_translator-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_translator-1.2.tar", last modified: Mon Jul 17 20:50:38 2023, max compression
+gzip compressed data, was "flet_translator-1.2.5.tar", last modified: Mon Jul 17 21:10:02 2023, max compression
```

## Comparing `flet_translator-1.2.tar` & `flet_translator-1.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:38.567697 flet_translator-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 20:50:26.000000 flet_translator-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 20:50:26.000000 flet_translator-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-17 20:50:38.567697 flet_translator-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-17 20:50:26.000000 flet_translator-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:38.567697 flet_translator-1.2/flet_translator/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:38.567697 flet_translator-1.2/flet_translator/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/tools/translate_control_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/tools/translate_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/tools/translate_using_google.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/tools/translate_using_opusMT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:38.567697 flet_translator-1.2/flet_translator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/utils/allowed_props_to_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/utils/google_supported_langaues.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/utils/is_rtl.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-17 20:50:26.000000 flet_translator-1.2/flet_translator/utils/opusMT_supported_languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:38.567697 flet_translator-1.2/flet_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-17 20:50:38.000000 flet_translator-1.2/flet_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 20:50:38.000000 flet_translator-1.2/flet_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:50:38.000000 flet_translator-1.2/flet_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 20:50:38.000000 flet_translator-1.2/flet_translator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 20:50:38.000000 flet_translator-1.2/flet_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 20:50:26.000000 flet_translator-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:50:38.567697 flet_translator-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-17 20:50:26.000000 flet_translator-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:10:02.411039 flet_translator-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 21:09:49.000000 flet_translator-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 21:09:49.000000 flet_translator-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-17 21:10:02.411039 flet_translator-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-17 21:09:49.000000 flet_translator-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:10:02.407039 flet_translator-1.2.5/flet_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:10:02.407039 flet_translator-1.2.5/flet_translator/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/tools/translate_control_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/tools/translate_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/tools/translate_using_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/tools/translate_using_opusMT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:10:02.411039 flet_translator-1.2.5/flet_translator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/utils/allowed_props_to_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/utils/google_supported_langaues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/utils/is_rtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-17 21:09:49.000000 flet_translator-1.2.5/flet_translator/utils/opusMT_supported_languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:10:02.407039 flet_translator-1.2.5/flet_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-17 21:10:02.000000 flet_translator-1.2.5/flet_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 21:10:02.000000 flet_translator-1.2.5/flet_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:10:02.000000 flet_translator-1.2.5/flet_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 21:10:02.000000 flet_translator-1.2.5/flet_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 21:10:02.000000 flet_translator-1.2.5/flet_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 21:09:49.000000 flet_translator-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:10:02.411039 flet_translator-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 21:09:49.000000 flet_translator-1.2.5/setup.py
```

### Comparing `flet_translator-1.2/LICENSE` & `flet_translator-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/PKG-INFO` & `flet_translator-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_translator
-Version: 1.2
+Version: 1.2.5
 Summary: A package that help flet developers to make their apps support multiple languages
 Home-page: https://github.com/SKbarbon/flet_translator
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_translator-1.2/README.md` & `flet_translator-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/flet_translator/tools/translate_control_content.py` & `flet_translator-1.2.5/flet_translator/tools/translate_control_content.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/flet_translator/tools/translate_page.py` & `flet_translator-1.2.5/flet_translator/tools/translate_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,18 @@
             self.skiped_controls = skiped_controls
         else:
             self.skiped_controls = []
 
         self.__use_internet = use_internet
 
         if use_internet == False:
-            from easynmt import EasyNMT
+            try:
+                from easynmt import EasyNMT
+            except:
+                raise ImportError("Please install the easynmt package:\npip install EasyNMT")
             # store ML models
             self.opusMT_model = EasyNMT('opus-mt')
 
             # Activate the model to be faster in the second request.
             self.opusMT_model.translate(
                 "Hi", 
                 target_lang="en", 
@@ -70,15 +73,18 @@
                     "control" : con,
                     "use_internet" : self.__use_internet
                 }
             ).start()
     
     def activate_local_ML_translation (self):
         """This will activate the local machine learning model to be used in future translation requests"""
-        from easynmt import EasyNMT
+        try:
+            from easynmt import EasyNMT
+        except:
+            raise ImportError("Please install the easynmt package:\npip install EasyNMT")
         self.__use_internet = False
         # store ML models
         self.opusMT_model = EasyNMT('opus-mt')
 
         # Activate the model to be faster in the second request.
         self.opusMT_model.translate(
             "Hi",
```

### Comparing `flet_translator-1.2/flet_translator/tools/translate_using_google.py` & `flet_translator-1.2.5/flet_translator/tools/translate_using_google.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/flet_translator/tools/translate_using_opusMT.py` & `flet_translator-1.2.5/flet_translator/tools/translate_using_opusMT.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 
 
 
 def translate_using_opusMT (Translatemodel, src:str, from_language, into_language):
-    from easynmt import EasyNMT
+    try:
+        from easynmt import EasyNMT
+    except:
+        raise ImportError("Please install the easynmt package:\npip install EasyNMT")
     if from_language == "auto":
         r = Translatemodel.translate(src, target_lang=into_language, 
                                     perform_sentence_splitting=True)
     else:
         r = Translatemodel.translate(src, target_lang=into_language, source_lang=from_language, 
                                  perform_sentence_splitting=True)
```

### Comparing `flet_translator-1.2/flet_translator/utils/google_supported_langaues.py` & `flet_translator-1.2.5/flet_translator/utils/google_supported_langaues.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/flet_translator/utils/opusMT_supported_languages.py` & `flet_translator-1.2.5/flet_translator/utils/opusMT_supported_languages.py`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/flet_translator.egg-info/PKG-INFO` & `flet_translator-1.2.5/flet_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-translator
-Version: 1.2
+Version: 1.2.5
 Summary: A package that help flet developers to make their apps support multiple languages
 Home-page: https://github.com/SKbarbon/flet_translator
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_translator-1.2/flet_translator.egg-info/SOURCES.txt` & `flet_translator-1.2.5/flet_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flet_translator-1.2/setup.py` & `flet_translator-1.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_translator',
-    version='1.2',
+    version='1.2.5',
     author='SKbarbon',
     description='A package that help flet developers to make their apps support multiple languages',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_translator',
-    install_requires=["flet", "EasyNMT", "sacremoses", "deep-translator"],
+    install_requires=["flet", "sacremoses", "deep-translator"],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
     ],
 )
```

