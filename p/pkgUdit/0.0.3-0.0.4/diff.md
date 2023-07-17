# Comparing `tmp/pkgUdit-0.0.3-py3-none-any.whl.zip` & `tmp/pkgUdit-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2560 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      949 b- defN 23-Jul-17 06:25 pkgUdit/__init__.py
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-17 06:25 pkgUdit-0.0.3.dist-info/License.txt
--rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-17 06:25 pkgUdit-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 06:25 pkgUdit-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 06:25 pkgUdit-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      464 b- defN 23-Jul-17 06:25 pkgUdit-0.0.3.dist-info/RECORD
-6 files, 2956 bytes uncompressed, 1718 bytes compressed:  41.9%
+Zip file size: 2556 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      932 b- defN 23-Jul-17 07:45 pkgUdit/__init__.py
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-17 07:45 pkgUdit-0.0.4.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-17 07:45 pkgUdit-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 07:45 pkgUdit-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 07:45 pkgUdit-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      464 b- defN 23-Jul-17 07:45 pkgUdit-0.0.4.dist-info/RECORD
+6 files, 2939 bytes uncompressed, 1714 bytes compressed:  41.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pkgUdit/__init__.py
 Comment: 
 
-Filename: pkgUdit-0.0.3.dist-info/License.txt
+Filename: pkgUdit-0.0.4.dist-info/License.txt
 Comment: 
 
-Filename: pkgUdit-0.0.3.dist-info/METADATA
+Filename: pkgUdit-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pkgUdit-0.0.3.dist-info/WHEEL
+Filename: pkgUdit-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pkgUdit-0.0.3.dist-info/top_level.txt
+Filename: pkgUdit-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgUdit-0.0.3.dist-info/RECORD
+Filename: pkgUdit-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgUdit/__init__.py

```diff
@@ -1,38 +1,30 @@
 import random
-import array
-
-max_length = 12
 
 numerals = ['0','1','2','3','4','5','6','7','8','9']
 lowerCaps = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
 upperChars = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
 
-
-type(numerals)
 combinedChars = numerals + lowerCaps + upperChars
 
-# print(combinedChars)
-
-passLength = random.randint(6,12)
-# print(passLength)
+passLength = random.randint(6, 12)
 
 def custom_choice(combinedChars):
-    idx = random.randint(0,len(combinedChars)-1)
+    idx = random.randint(0, len(combinedChars)-1)
     return combinedChars[idx]
 
-
-def make_radom():
-    password = ""
-    for _ in range(passLength):
-        password += custom_choice(combinedChars)
-
-#print(password)
-
-    gen_password = list(password)
-    random.shuffle(gen_password)
-    return gen_password
+def make_random():
+    password = []
+    password.append(random.choice(numerals))  # Include one numeric value
+    
+    for _ in range(passLength - 1):
+        password.append(custom_choice(combinedChars))
+    
+    random.shuffle(password)
+    return password
 
 def generatePass():
-    created_pass=make_radom()
-    return (''.join(created_pass))
+    created_pass = make_random()
+    return ''.join(created_pass)
 
+# password = generatePass()
+# print(password)
```

## Comparing `pkgUdit-0.0.3.dist-info/License.txt` & `pkgUdit-0.0.4.dist-info/License.txt`

 * *Files identical despite different names*

