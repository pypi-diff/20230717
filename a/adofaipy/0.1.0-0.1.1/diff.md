# Comparing `tmp/adofaipy-0.1.0.tar.gz` & `tmp/adofaipy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adofaipy-0.1.0.tar", last modified: Thu Jun 15 16:05:44 2023, max compression
+gzip compressed data, was "adofaipy-0.1.1.tar", last modified: Mon Jul 17 11:49:52 2023, max compression
```

## Comparing `adofaipy-0.1.0.tar` & `adofaipy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:05:44.939573 adofaipy-0.1.0/
--rw-rw-rw-   0        0        0      467 2023-06-15 16:04:14.000000 adofaipy-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2521 2023-06-15 16:05:44.937027 adofaipy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-06-14 14:48:56.000000 adofaipy-0.1.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 16:05:44.917405 adofaipy-0.1.0/adofaipy/
--rw-rw-rw-   0        0        0    21546 2023-06-15 16:01:11.000000 adofaipy-0.1.0/adofaipy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:05:44.934017 adofaipy-0.1.0/adofaipy.egg-info/
--rw-rw-rw-   0        0        0     2521 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:05:44.940573 adofaipy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-06-15 16:04:25.000000 adofaipy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:52.382155 adofaipy-0.1.1/
+-rw-rw-rw-   0        0        0      606 2023-07-17 11:32:59.000000 adofaipy-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2350 2023-07-17 11:49:52.380157 adofaipy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-06-14 14:48:56.000000 adofaipy-0.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:52.369628 adofaipy-0.1.1/adofaipy/
+-rw-rw-rw-   0        0        0    21596 2023-07-17 11:33:28.000000 adofaipy-0.1.1/adofaipy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:52.374630 adofaipy-0.1.1/adofaipy.egg-info/
+-rw-rw-rw-   0        0        0     2350 2023-07-17 11:49:52.000000 adofaipy-0.1.1/adofaipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-07-17 11:49:52.000000 adofaipy-0.1.1/adofaipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:49:52.000000 adofaipy-0.1.1/adofaipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 11:49:52.000000 adofaipy-0.1.1/adofaipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:49:52.382155 adofaipy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-07-17 11:33:20.000000 adofaipy-0.1.1/setup.py
```

### Comparing `adofaipy-0.1.0/LICENSE.txt` & `adofaipy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.1.0/PKG-INFO` & `adofaipy-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,66 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: adofaipy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
-Description: This is a library that makes automating events in ADOFAI levels more convenient.
-        
-        List of Functions:
-        
-        getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
-        
-        getAngles(filestring : str): takes a file string and returns the list of angles.
-        
-        setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
-        
-        There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
-        The arguments for these functions are the same as the fields that are present in the ingame editor.
-        Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
-        These functions return the event data as a string which can be added with addEvent().
-        
-        Note that addDecoration() works the same as other event functions. 
-        
-        addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
-        
-        writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
-        
-        
-        Change Log
-        ==========
-        
-        0.1.0 (2023/06/15)
-        ------------------
-        - Minor update
-        - Added dynamic pivot offset, parallax offset, masking and blending fields to addDecoration() and moveDecorations()
-        - Added angleOffset to setSpeed()
-        
-        0.0.3 (2023/06/14)
-        ------------------
-        - Minor bugfix: fixed filename __init__.py
-        
-        0.0.2 (2023/06/13)
-        ------------------
-        - Minor bugfix: 're' is no longer a dependency
-        
-        0.0.1 (2023/05/28)
-        ------------------
-        - First Release
 Keywords: adofai
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE.txt
+
+This is a library that makes automating events in ADOFAI levels more convenient.
+
+List of Functions:
+
+getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
+
+getAngles(filestring : str): takes a file string and returns the list of angles.
+
+setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
+
+There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
+The arguments for these functions are the same as the fields that are present in the ingame editor.
+Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
+These functions return the event data as a string which can be added with addEvent().
+
+Note that addDecoration() works the same as other event functions. 
+
+addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
+
+writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
+
+
+Change Log
+==========
+
+0.1.1 (2023/07/17)
+------------------
+- Minor bugfixes
+- Fixed encoding incompatibility
+- Fixed output string for moveDecorations()
+
+0.1.0 (2023/06/15)
+------------------
+- Minor update
+- Added dynamic pivot offset, parallax offset, masking and blending fields to addDecoration() and moveDecorations()
+- Added angleOffset to setSpeed()
+
+0.0.3 (2023/06/14)
+------------------
+- Minor bugfix: fixed filename __init__.py
+
+0.0.2 (2023/06/13)
+------------------
+- Minor bugfix: 're' is no longer a dependency
+
+0.0.1 (2023/05/28)
+------------------
+- First Release
+
```

### Comparing `adofaipy-0.1.0/README.txt` & `adofaipy-0.1.1/README.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.1.0/adofaipy/__init__.py` & `adofaipy-0.1.1/adofaipy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 def getFileString(filename : str) -> str:
-    with open(filename, "r") as f:
+    with open(filename, "r", encoding="utf-8-sig") as f:
         s = f.read()
         return s
 
 def getAngles(filestring : str) -> list:
 
     index= filestring.find( "\"angleData\": [")
     if index !=-1 :  
@@ -33,15 +33,15 @@
         filestring = re.sub("\"decorations\":\n\t\[", "\"decorations\":\n\t[" + event, filestring)
     else:
         filestring = re.sub("\"actions\":\n\t\[", "\"actions\":\n\t[" + event, filestring)
     return filestring
 
 def writeToFile(filestring : str, filename : str):
     
-    with open(filename, "w") as f:
+    with open(filename, "w", encoding="utf-8-sig") as f:
         f.write(filestring)
 
 def setSpeed(floor : int, speedtype="Bpm", bpm=100, bpmmultiplier=1, angleoffset=0):
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"SetSpeed\", \"speedType\": \"" + str(speedtype) + "\", \"beatsPerMinute\": " + str(bpm) + ", \"bpmMultiplier\": " + str(bpmmultiplier) + ", \"angleOffset\": " + angleoffset + " }"
 
 def twirl(floor : int):
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"Twirl\" }"
@@ -172,15 +172,15 @@
     if maskingfrontdepth != None:
         maskingfrontdepthstring = ", \"maskingFrontDepth\": " + str(maskingfrontdepth)
 
     maskingbackdepthstring = ""
     if maskingbackdepth != None:
         maskingbackdepthstring = ", \"maskingBackDepth\": " + str(maskingbackdepth)
 
-    return "{ \"floor\": " + str(floor) + ", \"eventType\": \"MoveDecorations\", \"duration\": " + str(duration) + ", \"tag\": \"" + tag + "\"" + imgstring + ", \"positionOffset\": [" + str(posx) + ", " + str(posy) + "]" + ", \"pivotOffset\": [" + str(pivotx) + ", " + str(pivoty) + "]" + rotstring + scalexstring + scaleystring + colstring + opacitystring + depthstring + parallaxxstring + parallaxystring + ", \"parallaxOffset\": [" + str(parallaxoffsetx) + ", " + str(parallaxoffsety) + "]" + ", \"angleOffset\": " + str(angleoffset) + ", \"ease\": \"" + ease + "\", \"eventTag\": \"" + str(eventtag) + "\" " + maskingtypestring + usemaskingdepthstring + maskingfrontdepthstring + maskingbackdepthstring + " }"
+    return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"MoveDecorations\", \"duration\": " + str(duration) + ", \"tag\": \"" + tag + "\"" + imgstring + ", \"positionOffset\": [" + str(posx) + ", " + str(posy) + "]" + ", \"pivotOffset\": [" + str(pivotx) + ", " + str(pivoty) + "]" + rotstring + scalexstring + scaleystring + colstring + opacitystring + depthstring + parallaxxstring + parallaxystring + ", \"parallaxOffset\": [" + str(parallaxoffsetx) + ", " + str(parallaxoffsety) + "]" + ", \"angleOffset\": " + str(angleoffset) + ", \"ease\": \"" + ease + "\", \"eventTag\": \"" + str(eventtag) + "\" " + maskingtypestring + usemaskingdepthstring + maskingfrontdepthstring + maskingbackdepthstring + " }"
 
 def setText(floor : int, text="Text", tag="", angleoffset=0, eventtag=""):
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"SetText\", \"decText\": \"" + text + "\", \"tag\": \"" + tag + "\", \"angleOffset\": " + str(angleoffset) + ", \"eventTag\": \"" + eventtag + "\" }"
 
 
 def customBackground(floor : int, color="000000", bgimage="", imagecolor="ffffff", parallaxx=100, parallaxy=100, bgdisplaymode="FitToScreen", lockrot="Disabled", loopBG="Disabled", unscaledSize=100, angleoffset=0, eventtag=""):
```

### Comparing `adofaipy-0.1.0/adofaipy.egg-info/PKG-INFO` & `adofaipy-0.1.1/adofaipy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,66 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: adofaipy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
-Description: This is a library that makes automating events in ADOFAI levels more convenient.
-        
-        List of Functions:
-        
-        getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
-        
-        getAngles(filestring : str): takes a file string and returns the list of angles.
-        
-        setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
-        
-        There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
-        The arguments for these functions are the same as the fields that are present in the ingame editor.
-        Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
-        These functions return the event data as a string which can be added with addEvent().
-        
-        Note that addDecoration() works the same as other event functions. 
-        
-        addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
-        
-        writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
-        
-        
-        Change Log
-        ==========
-        
-        0.1.0 (2023/06/15)
-        ------------------
-        - Minor update
-        - Added dynamic pivot offset, parallax offset, masking and blending fields to addDecoration() and moveDecorations()
-        - Added angleOffset to setSpeed()
-        
-        0.0.3 (2023/06/14)
-        ------------------
-        - Minor bugfix: fixed filename __init__.py
-        
-        0.0.2 (2023/06/13)
-        ------------------
-        - Minor bugfix: 're' is no longer a dependency
-        
-        0.0.1 (2023/05/28)
-        ------------------
-        - First Release
 Keywords: adofai
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE.txt
+
+This is a library that makes automating events in ADOFAI levels more convenient.
+
+List of Functions:
+
+getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
+
+getAngles(filestring : str): takes a file string and returns the list of angles.
+
+setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
+
+There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
+The arguments for these functions are the same as the fields that are present in the ingame editor.
+Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
+These functions return the event data as a string which can be added with addEvent().
+
+Note that addDecoration() works the same as other event functions. 
+
+addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
+
+writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
+
+
+Change Log
+==========
+
+0.1.1 (2023/07/17)
+------------------
+- Minor bugfixes
+- Fixed encoding incompatibility
+- Fixed output string for moveDecorations()
+
+0.1.0 (2023/06/15)
+------------------
+- Minor update
+- Added dynamic pivot offset, parallax offset, masking and blending fields to addDecoration() and moveDecorations()
+- Added angleOffset to setSpeed()
+
+0.0.3 (2023/06/14)
+------------------
+- Minor bugfix: fixed filename __init__.py
+
+0.0.2 (2023/06/13)
+------------------
+- Minor bugfix: 're' is no longer a dependency
+
+0.0.1 (2023/05/28)
+------------------
+- First Release
+
```

### Comparing `adofaipy-0.1.0/setup.py` & `adofaipy-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.11'
 ]
  
 setup(
   name='adofaipy',
-  version='0.1.0',
+  version='0.1.1',
   description='A library that makes automating events in ADOFAI levels more convenient.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='M1n3c4rt',
   author_email='vedicbits@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

