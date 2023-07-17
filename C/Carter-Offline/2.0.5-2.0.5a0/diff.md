# Comparing `tmp/Carter-Offline-2.0.5.tar.gz` & `tmp/Carter-Offline-2.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.5.tar", last modified: Mon Jul 17 14:22:43 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.5a0.tar", last modified: Mon Jul 17 14:36:01 2023, max compression
```

## Comparing `Carter-Offline-2.0.5.tar` & `Carter-Offline-2.0.5a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:22:43.945911 Carter-Offline-2.0.5/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:22:43.924547 Carter-Offline-2.0.5/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:22:43.925063 Carter-Offline-2.0.5/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.5/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.5/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)     9834 2023-07-17 14:21:06.000000 Carter-Offline-2.0.5/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.5/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.5/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:22:43.945508 Carter-Offline-2.0.5/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     2092 2023-07-17 14:22:43.000000 Carter-Offline-2.0.5/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 14:22:43.000000 Carter-Offline-2.0.5/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:22:43.000000 Carter-Offline-2.0.5/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 14:22:43.000000 Carter-Offline-2.0.5/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 14:22:43.000000 Carter-Offline-2.0.5/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.5/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     2092 2023-07-17 14:22:43.945769 Carter-Offline-2.0.5/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.5/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:22:43.945950 Carter-Offline-2.0.5/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-17 14:22:18.000000 Carter-Offline-2.0.5/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:36:01.671384 Carter-Offline-2.0.5a0/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:36:01.666937 Carter-Offline-2.0.5a0/CarterOffline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:36:01.667423 Carter-Offline-2.0.5a0/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.5a0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.5a0/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)    10366 2023-07-17 14:32:40.000000 Carter-Offline-2.0.5a0/CarterOffline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.5a0/CarterOffline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.5a0/CarterOffline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:36:01.671049 Carter-Offline-2.0.5a0/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:36:01.000000 Carter-Offline-2.0.5a0/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 14:36:01.000000 Carter-Offline-2.0.5a0/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:36:01.000000 Carter-Offline-2.0.5a0/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 14:36:01.000000 Carter-Offline-2.0.5a0/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 14:36:01.000000 Carter-Offline-2.0.5a0/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.5a0/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:36:01.671254 Carter-Offline-2.0.5a0/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.5a0/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:36:01.671423 Carter-Offline-2.0.5a0/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1323 2023-07-17 14:35:56.000000 Carter-Offline-2.0.5a0/setup.py
```

### Comparing `Carter-Offline-2.0.5/CarterOffline/__init__.py` & `Carter-Offline-2.0.5a0/CarterOffline/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -286,20 +286,34 @@
                 intent.setdefault("patterns", []).append(input_string)
                 intent.setdefault("responses", []).append(ResponseOutput.output_text)
                 with open(self.intents_file_path, 'w') as json_file:
                     json.dump(intents, json_file, indent=4, separators=(',', ': '))
 
                 break
 
-            if Done == 0:
+        if Done == 0:
+            for intent in intents['intents']:
+                if User == intent.get("tag"):
+                    intent.setdefault("patterns", []).append(input_string)
+                    intent.setdefault("responses", []).append(ResponseOutput.output_text)
+                    with open(self.intents_file_path, 'w') as json_file:
+                        json.dump(intents, json_file, indent=4, separators=(',', ': '))
+                    Done = 1
+                    break
+
+        if Done == 0:
+
                 new_class = {
-                "tag": User,
-                "patterns": [input_string],
-                "responses": [ResponseOutput.output_text]
+                    "tag": User,
+                    "patterns": [input_string],
+                    "responses": [ResponseOutput.output_text]
                 }
+
                 intents['intents'].append(new_class)
                 with open(self.intents_file_path, 'w') as json_file:
                     json.dump(intents, json_file, indent=4, separators=(',', ': '))
 
+                Done = 1
+
                 break
 
         return ResponseOutput.output_text
```

### Comparing `Carter-Offline-2.0.5/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.5a0/Carter_Offline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.5
+Version: 2.0.5a0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.5/LICENSE` & `Carter-Offline-2.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.5/PKG-INFO` & `Carter-Offline-2.0.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.5
+Version: 2.0.5a0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.5/README.md` & `Carter-Offline-2.0.5a0/README.md`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.5/setup.py` & `Carter-Offline-2.0.5a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.5",
+    version="2.0.5a",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

