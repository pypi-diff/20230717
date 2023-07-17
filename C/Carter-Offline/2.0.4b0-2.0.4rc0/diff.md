# Comparing `tmp/Carter-Offline-2.0.4b0.tar.gz` & `tmp/Carter-Offline-2.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.4b0.tar", last modified: Mon Jul 17 14:14:21 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.4rc0.tar", last modified: Mon Jul 17 14:18:27 2023, max compression
```

## Comparing `Carter-Offline-2.0.4b0.tar` & `Carter-Offline-2.0.4rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.432474 Carter-Offline-2.0.4b0/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.425970 Carter-Offline-2.0.4b0/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.426538 Carter-Offline-2.0.4b0/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.4b0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.4b0/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)     9806 2023-07-17 14:13:28.000000 Carter-Offline-2.0.4b0/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.4b0/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.4b0/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.432163 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.4b0/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:14:21.432353 Carter-Offline-2.0.4b0/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.4b0/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:14:21.432506 Carter-Offline-2.0.4b0/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1327 2023-07-17 14:14:06.000000 Carter-Offline-2.0.4b0/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:18:27.388470 Carter-Offline-2.0.4rc0/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:18:27.381027 Carter-Offline-2.0.4rc0/CarterOffline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:18:27.381653 Carter-Offline-2.0.4rc0/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.4rc0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.4rc0/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)     9800 2023-07-17 14:16:40.000000 Carter-Offline-2.0.4rc0/CarterOffline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.4rc0/CarterOffline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.4rc0/CarterOffline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:18:27.387594 Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     2095 2023-07-17 14:18:27.000000 Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 14:18:27.000000 Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:18:27.000000 Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 14:18:27.000000 Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 14:18:27.000000 Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.4rc0/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     2095 2023-07-17 14:18:27.388325 Carter-Offline-2.0.4rc0/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.4rc0/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:18:27.388772 Carter-Offline-2.0.4rc0/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1324 2023-07-17 14:18:05.000000 Carter-Offline-2.0.4rc0/setup.py
```

### Comparing `Carter-Offline-2.0.4b0/CarterOffline/__init__.py` & `Carter-Offline-2.0.4rc0/CarterOffline/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -281,22 +281,21 @@
             intent_tag = intent.get("tag")
             if intent_tag == tag:
                 Done = 1
                 intent.setdefault("patterns", []).append(input_string)
                 intent.setdefault("responses", []).append(ResponseOutput.output_text)
                 with open(self.intents_file_path, 'w') as json_file:
                     json.dump(intents, json_file, indent=4, separators=(',', ': '))
-                break
+
+                return ResponseOutput.output_text
 
             if Done == 0:
                 new_class = {
                 "tag": User,
                 "patterns": [input_string],
                 "responses": [ResponseOutput.output_text]
                 }
                 intents['intents'].append(new_class)
                 with open(self.intents_file_path, 'w') as json_file:
                     json.dump(intents, json_file, indent=4, separators=(',', ': '))
-                    
-                break
 
-        return ResponseOutput.output_text
+                return ResponseOutput.output_text
```

### Comparing `Carter-Offline-2.0.4b0/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.4rc0/Carter_Offline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.4b0
+Version: 2.0.4rc0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.4b0/LICENSE` & `Carter-Offline-2.0.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.4b0/PKG-INFO` & `Carter-Offline-2.0.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.4b0
+Version: 2.0.4rc0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.4b0/README.md` & `Carter-Offline-2.0.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.4b0/setup.py` & `Carter-Offline-2.0.4rc0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.4.beta",
+    version="2.0.4.c",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

