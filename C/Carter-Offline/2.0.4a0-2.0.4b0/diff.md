# Comparing `tmp/Carter-Offline-2.0.4a0.tar.gz` & `tmp/Carter-Offline-2.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.4a0.tar", last modified: Mon Jul 17 11:39:52 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.4b0.tar", last modified: Mon Jul 17 14:14:21 2023, max compression
```

## Comparing `Carter-Offline-2.0.4a0.tar` & `Carter-Offline-2.0.4b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.750916 Carter-Offline-2.0.4a0/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.742247 Carter-Offline-2.0.4a0/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.742955 Carter-Offline-2.0.4a0/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.4a0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.4a0/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)     9763 2023-07-17 11:35:08.000000 Carter-Offline-2.0.4a0/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.4a0/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.4a0/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.750503 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     1893 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.4a0/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     1893 2023-07-17 11:39:52.750757 Carter-Offline-2.0.4a0/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1504 2023-07-14 15:34:56.000000 Carter-Offline-2.0.4a0/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 11:39:52.750960 Carter-Offline-2.0.4a0/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1328 2023-07-17 11:39:49.000000 Carter-Offline-2.0.4a0/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.432474 Carter-Offline-2.0.4b0/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.425970 Carter-Offline-2.0.4b0/CarterOffline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.426538 Carter-Offline-2.0.4b0/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.4b0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.4b0/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)     9806 2023-07-17 14:13:28.000000 Carter-Offline-2.0.4b0/CarterOffline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.4b0/CarterOffline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.4b0/CarterOffline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:14:21.432163 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 14:14:21.000000 Carter-Offline-2.0.4b0/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.4b0/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:14:21.432353 Carter-Offline-2.0.4b0/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.4b0/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:14:21.432506 Carter-Offline-2.0.4b0/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1327 2023-07-17 14:14:06.000000 Carter-Offline-2.0.4b0/setup.py
```

### Comparing `Carter-Offline-2.0.4a0/CarterOffline/__init__.py` & `Carter-Offline-2.0.4b0/CarterOffline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,9 +292,11 @@
                 "tag": User,
                 "patterns": [input_string],
                 "responses": [ResponseOutput.output_text]
                 }
                 intents['intents'].append(new_class)
                 with open(self.intents_file_path, 'w') as json_file:
                     json.dump(intents, json_file, indent=4, separators=(',', ': '))
+                    
+                break
 
         return ResponseOutput.output_text
```

### Comparing `Carter-Offline-2.0.4a0/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.4b0/Carter_Offline.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.4a0
+Version: 2.0.4b0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 
 # Carter Offline
 
 Carter Offline is an intent classifier which is based on a modified version of Janex, and utilises LazyLyrics' Carter-Py library.
 
 It compares the input you send to your carter agent with a list of patterns in your chosen intents file, and then remembers the class. Once your Carter agent creates a response, the program saves the response to your intents, recording the interaction and improving your intents dataset.
 
+This is based on an older version of Janex (release 0.0.5.beta, specifically), and so it may not include the latest features from there unless explicitly added in.
+
 See also:
 
 ```
 https://github.com/LazyLyrics/carter-py
 https://github.com/Cipher58/Janex
 ```
 
@@ -42,14 +44,16 @@
 <h4>Using Carter-Offline in your code</h4>
 
 <h5>Define Variables</h5>
 
 To use this program, you will need to define your API key, name and intent file path.
 
 ```
+intents_file_path = "intents.json"
+
 CarterAPI = "YOUR CARTER AGENT'S API"
 
 input_string = "Hello!" # for example
 
 User = "YOUR NAME"
 
 # Create an instance of the CarterOffline class
```

### Comparing `Carter-Offline-2.0.4a0/LICENSE` & `Carter-Offline-2.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.4a0/PKG-INFO` & `Carter-Offline-2.0.4b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.4a0
+Version: 2.0.4b0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 
 # Carter Offline
 
 Carter Offline is an intent classifier which is based on a modified version of Janex, and utilises LazyLyrics' Carter-Py library.
 
 It compares the input you send to your carter agent with a list of patterns in your chosen intents file, and then remembers the class. Once your Carter agent creates a response, the program saves the response to your intents, recording the interaction and improving your intents dataset.
 
+This is based on an older version of Janex (release 0.0.5.beta, specifically), and so it may not include the latest features from there unless explicitly added in.
+
 See also:
 
 ```
 https://github.com/LazyLyrics/carter-py
 https://github.com/Cipher58/Janex
 ```
 
@@ -42,14 +44,16 @@
 <h4>Using Carter-Offline in your code</h4>
 
 <h5>Define Variables</h5>
 
 To use this program, you will need to define your API key, name and intent file path.
 
 ```
+intents_file_path = "intents.json"
+
 CarterAPI = "YOUR CARTER AGENT'S API"
 
 input_string = "Hello!" # for example
 
 User = "YOUR NAME"
 
 # Create an instance of the CarterOffline class
```

### Comparing `Carter-Offline-2.0.4a0/README.md` & `Carter-Offline-2.0.4b0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Carter Offline
 
 Carter Offline is an intent classifier which is based on a modified version of Janex, and utilises LazyLyrics' Carter-Py library.
 
 It compares the input you send to your carter agent with a list of patterns in your chosen intents file, and then remembers the class. Once your Carter agent creates a response, the program saves the response to your intents, recording the interaction and improving your intents dataset.
 
+This is based on an older version of Janex (release 0.0.5.beta, specifically), and so it may not include the latest features from there unless explicitly added in.
+
 See also:
 
 ```
 https://github.com/LazyLyrics/carter-py
 https://github.com/Cipher58/Janex
 ```
 
@@ -29,14 +31,16 @@
 <h4>Using Carter-Offline in your code</h4>
 
 <h5>Define Variables</h5>
 
 To use this program, you will need to define your API key, name and intent file path.
 
 ```
+intents_file_path = "intents.json"
+
 CarterAPI = "YOUR CARTER AGENT'S API"
 
 input_string = "Hello!" # for example
 
 User = "YOUR NAME"
 
 # Create an instance of the CarterOffline class
```

### Comparing `Carter-Offline-2.0.4a0/setup.py` & `Carter-Offline-2.0.4b0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.4.alpha",
+    version="2.0.4.beta",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

