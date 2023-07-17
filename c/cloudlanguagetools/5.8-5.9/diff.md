# Comparing `tmp/cloudlanguagetools-5.8.tar.gz` & `tmp/cloudlanguagetools-5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-5.8.tar", last modified: Sun Jul 16 13:29:56 2023, max compression
+gzip compressed data, was "cloudlanguagetools-5.9.tar", last modified: Sun Jul 16 13:57:33 2023, max compression
```

## Comparing `cloudlanguagetools-5.8.tar` & `cloudlanguagetools-5.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17939 2023-07-16 13:29:35.000000 cloudlanguagetools-5.8/cloudlanguagetools/chatapi.py
--rw-r--r--   0 luc       (1000) luc       (1000)    11935 2023-07-16 13:29:35.000000 cloudlanguagetools-5.8/cloudlanguagetools/chatmodel.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-5.8/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/elevenlabs.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1462 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-07-16 13:29:53.000000 cloudlanguagetools-5.8/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:57:33.318749 cloudlanguagetools-5.9/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-16 13:57:33.318749 cloudlanguagetools-5.9/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:57:33.318749 cloudlanguagetools-5.9/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17939 2023-07-16 13:29:35.000000 cloudlanguagetools-5.9/cloudlanguagetools/chatapi.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    11935 2023-07-16 13:29:35.000000 cloudlanguagetools-5.9/cloudlanguagetools/chatmodel.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-5.9/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-5.9/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.9/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:57:33.318749 cloudlanguagetools-5.9/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-16 13:57:33.000000 cloudlanguagetools-5.9/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1462 2023-07-16 13:57:33.000000 cloudlanguagetools-5.9/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-16 13:57:33.000000 cloudlanguagetools-5.9/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-16 13:57:33.000000 cloudlanguagetools-5.9/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-16 13:57:33.000000 cloudlanguagetools-5.9/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-16 13:57:33.318749 cloudlanguagetools-5.9/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      931 2023-07-16 13:57:30.000000 cloudlanguagetools-5.9/setup.py
```

### Comparing `cloudlanguagetools-5.8/LICENSE` & `cloudlanguagetools-5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/PKG-INFO` & `cloudlanguagetools-5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.8
+Version: 5.9
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/amazon.py` & `cloudlanguagetools-5.9/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-5.9/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/azure.py` & `cloudlanguagetools-5.9/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-5.9/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/chatapi.py` & `cloudlanguagetools-5.9/cloudlanguagetools/chatapi.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/chatmodel.py` & `cloudlanguagetools-5.9/cloudlanguagetools/chatmodel.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/constants.py` & `cloudlanguagetools-5.9/cloudlanguagetools/constants.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/deepl.py` & `cloudlanguagetools-5.9/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-5.9/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-5.9/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/elevenlabs.py` & `cloudlanguagetools-5.9/cloudlanguagetools/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/encryption.py` & `cloudlanguagetools-5.9/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/epitran.py` & `cloudlanguagetools-5.9/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/forvo.py` & `cloudlanguagetools-5.9/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/fptai.py` & `cloudlanguagetools-5.9/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/google.py` & `cloudlanguagetools-5.9/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/keys.py` & `cloudlanguagetools-5.9/cloudlanguagetools/keys.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/languages.py` & `cloudlanguagetools-5.9/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-5.9/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-5.9/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/naver.py` & `cloudlanguagetools-5.9/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/openai.py` & `cloudlanguagetools-5.9/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-5.9/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-5.9/cloudlanguagetools/servicemanager.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/spacy.py` & `cloudlanguagetools-5.9/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/test_services.py` & `cloudlanguagetools-5.9/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-5.9/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-5.9/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-5.9/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-5.9/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-5.9/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/voicen.py` & `cloudlanguagetools-5.9/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/watson.py` & `cloudlanguagetools-5.9/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-5.9/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-5.9/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.8
+Version: 5.9
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.8/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-5.9/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.8/setup.py` & `cloudlanguagetools-5.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='5.8',
+      version='5.9',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
       ],      
       license='GPL',
       packages=['cloudlanguagetools'],
       install_requires=[
           'clt_wenlin>=1.0',
-          'clt_requirements>=0.9',
+          'clt_requirements>=1.0',
           'pinyin_jyutping>=0.9',
       ],
-      )
+      )
```

