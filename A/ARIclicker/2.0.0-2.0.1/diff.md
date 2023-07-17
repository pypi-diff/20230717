# Comparing `tmp/ARIclicker-2.0.0.tar.gz` & `tmp/ARIclicker-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-2.0.0.tar", last modified: Mon Jul 17 03:17:48 2023, max compression
+gzip compressed data, was "ARIclicker-2.0.1.tar", last modified: Mon Jul 17 11:40:11 2023, max compression
```

## Comparing `ARIclicker-2.0.0.tar` & `ARIclicker-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:17:48.475144 ARIclicker-2.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-17 03:17:48.435144 ARIclicker-2.0.0/ARIclicker/
--rw-rw-rw-   0        0        0     1779 2023-07-16 11:37:39.000000 ARIclicker-2.0.0/ARIclicker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:17:48.465144 ARIclicker-2.0.0/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1021 2023-07-17 03:17:48.475144 ARIclicker-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-16 10:49:43.000000 ARIclicker-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 03:17:48.475144 ARIclicker-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      747 2023-07-17 03:17:17.000000 ARIclicker-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:40:11.592089 ARIclicker-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-17 11:40:11.513960 ARIclicker-2.0.1/ARIclicker/
+-rw-rw-rw-   0        0        0     1808 2023-07-17 03:30:48.000000 ARIclicker-2.0.1/ARIclicker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:40:11.576465 ARIclicker-2.0.1/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1626 2023-07-17 11:40:10.000000 ARIclicker-2.0.1/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-07-17 11:40:11.000000 ARIclicker-2.0.1/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:40:10.000000 ARIclicker-2.0.1/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 11:40:10.000000 ARIclicker-2.0.1/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1626 2023-07-17 11:40:11.592089 ARIclicker-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2023-07-17 11:38:36.000000 ARIclicker-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:40:11.607701 ARIclicker-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-07-17 11:39:51.000000 ARIclicker-2.0.1/setup.py
```

### Comparing `ARIclicker-2.0.0/ARIclicker/__init__.py` & `ARIclicker-2.0.1/ARIclicker/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,8 @@
         elif key == stop_key:
             click_thread.exit()
             listener.stop()
 
     with Listener(on_press=on_press) as listener:
         listener.join()
         start_listening_click = True
-
+autoclick("w","a","left",1,3)
```

### Comparing `ARIclicker-2.0.0/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-2.0.1/ARIclicker.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 2.0.0
+Version: 2.0.1
 Summary: The best autoclicker in minecraft!
 Home-page: UNKNOWN
 Author: LIN,Zhe
 Author-email: 2081812728@qq.com
 License: MIT
 Description:   # **--ARIclicker--** # 
         
@@ -22,14 +22,31 @@
         `
         
         ## Function ##
         * `def autoclick(start_stop_key_character, end_key_character, button,delay_min, delay_max) `
         
         
         
+        ## Attention ##
+        * This clicker can reduce the risk of banning to a certain extent, but it does not mean that it can guarantee that it will not be banned!
+        
+        * Please do not turn on the clicker for a long time! otherwise it may cause some impact on the hardware, in addition, it may increase the risk of banning!
+        
+        
+        
+        ### have fun ~ ###
+        <br><br>
+        
+        
+        ## Change log ##
+        
+        
+         ### **2.0.1**  (2023/7/17): ###
+         * Fixed several bugs
+         * Remove the "autopress" function
         
 Keywords: autoclicker,minecraft-auto
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ARIclicker-2.0.0/PKG-INFO` & `ARIclicker-2.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 2.0.0
+Version: 2.0.1
 Summary: The best autoclicker in minecraft!
 Home-page: UNKNOWN
 Author: LIN,Zhe
 Author-email: 2081812728@qq.com
 License: MIT
 Description:   # **--ARIclicker--** # 
         
@@ -22,14 +22,31 @@
         `
         
         ## Function ##
         * `def autoclick(start_stop_key_character, end_key_character, button,delay_min, delay_max) `
         
         
         
+        ## Attention ##
+        * This clicker can reduce the risk of banning to a certain extent, but it does not mean that it can guarantee that it will not be banned!
+        
+        * Please do not turn on the clicker for a long time! otherwise it may cause some impact on the hardware, in addition, it may increase the risk of banning!
+        
+        
+        
+        ### have fun ~ ###
+        <br><br>
+        
+        
+        ## Change log ##
+        
+        
+         ### **2.0.1**  (2023/7/17): ###
+         * Fixed several bugs
+         * Remove the "autopress" function
         
 Keywords: autoclicker,minecraft-auto
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ARIclicker-2.0.0/setup.py` & `ARIclicker-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='ARIclicker',
-    version='2.0.0',
+    version='2.0.1',
     description="The best autoclicker in minecraft!",
     long_description=open('README.md').read() ,
     long_description_content_type="text/markdown",
 
     author='LIN,Zhe',
     author_email='2081812728@qq.com',
     license='MIT',
```

