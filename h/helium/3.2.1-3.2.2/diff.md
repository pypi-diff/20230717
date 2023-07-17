# Comparing `tmp/helium-3.2.1.tar.gz` & `tmp/helium-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helium-3.2.1.tar", last modified: Wed Jul  5 14:26:45 2023, max compression
+gzip compressed data, was "helium-3.2.2.tar", last modified: Mon Jul 17 12:39:13 2023, max compression
```

## Comparing `helium-3.2.1.tar` & `helium-3.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.659989 helium-3.2.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1125 2023-07-05 14:26:45.659989 helium-3.2.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     6181 2023-07-05 14:17:27.000000 helium-3.2.1/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.651989 helium-3.2.1/helium/
--rw-r--r--   0 michael   (1000) michael   (1000)    36009 2023-07-05 14:11:03.000000 helium-3.2.1/helium/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.651989 helium-3.2.1/helium/_impl/
--rw-r--r--   0 michael   (1000) michael   (1000)    44520 2023-07-05 13:53:44.000000 helium-3.2.1/helium/_impl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1235 2023-07-05 14:25:03.000000 helium-3.2.1/helium/_impl/chromedriver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1140 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/match_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5411 2023-07-03 06:19:15.000000 helium-3.2.1/helium/_impl/selenium_wrappers.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.651989 helium-3.2.1/helium/_impl/util/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/dictionary.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6355 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/geom.py
--rw-r--r--   0 michael   (1000) michael   (1000)      979 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/html.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1210 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/inspect_.py
--rw-r--r--   0 michael   (1000) michael   (1000)      570 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/lang.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/os_.py
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/path.py
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/system.py
--rw-r--r--   0 michael   (1000) michael   (1000)      466 2021-03-16 06:48:50.000000 helium-3.2.1/helium/_impl/util/xpath.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.651989 helium-3.2.1/helium/_impl/webdrivers/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.651989 helium-3.2.1/helium/_impl/webdrivers/linux/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  7008696 2023-06-12 05:45:47.000000 helium-3.2.1/helium/_impl/webdrivers/linux/geckodriver
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.655989 helium-3.2.1/helium/_impl/webdrivers/mac/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  5259056 2023-06-12 05:45:47.000000 helium-3.2.1/helium/_impl/webdrivers/mac/geckodriver
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.659989 helium-3.2.1/helium/_impl/webdrivers/windows/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  3566280 2023-06-12 05:45:47.000000 helium-3.2.1/helium/_impl/webdrivers/windows/geckodriver.exe
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 14:26:45.651989 helium-3.2.1/helium.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1125 2023-07-05 14:26:45.000000 helium-3.2.1/helium.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      736 2023-07-05 14:26:45.000000 helium-3.2.1/helium.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-07-05 14:26:45.000000 helium-3.2.1/helium.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2021-03-16 06:50:17.000000 helium-3.2.1/helium.egg-info/not-zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-07-05 14:26:45.000000 helium-3.2.1/helium.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-07-05 14:26:45.000000 helium-3.2.1/helium.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-05 14:26:45.659989 helium-3.2.1/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     1465 2023-07-05 14:26:33.000000 helium-3.2.1/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.161753 helium-3.2.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1125 2023-07-17 12:39:13.161753 helium-3.2.2/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     6181 2023-07-05 14:17:27.000000 helium-3.2.2/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.145752 helium-3.2.2/helium/
+-rw-r--r--   0 michael   (1000) michael   (1000)    36009 2023-07-05 14:11:03.000000 helium-3.2.2/helium/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.145752 helium-3.2.2/helium/_impl/
+-rw-r--r--   0 michael   (1000) michael   (1000)    44901 2023-07-17 12:37:25.000000 helium-3.2.2/helium/_impl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1235 2023-07-05 14:25:03.000000 helium-3.2.2/helium/_impl/chromedriver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1140 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/match_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5411 2023-07-03 06:19:15.000000 helium-3.2.2/helium/_impl/selenium_wrappers.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.145752 helium-3.2.2/helium/_impl/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/dictionary.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6355 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/geom.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      979 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/html.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1210 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/inspect_.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      570 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/lang.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/os_.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      466 2021-03-16 06:48:50.000000 helium-3.2.2/helium/_impl/util/xpath.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.145752 helium-3.2.2/helium/_impl/webdrivers/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.145752 helium-3.2.2/helium/_impl/webdrivers/linux/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  7008696 2023-06-12 05:45:47.000000 helium-3.2.2/helium/_impl/webdrivers/linux/geckodriver
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.153753 helium-3.2.2/helium/_impl/webdrivers/mac/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  5259056 2023-06-12 05:45:47.000000 helium-3.2.2/helium/_impl/webdrivers/mac/geckodriver
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.153753 helium-3.2.2/helium/_impl/webdrivers/windows/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  3566280 2023-06-12 05:45:47.000000 helium-3.2.2/helium/_impl/webdrivers/windows/geckodriver.exe
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-17 12:39:13.145752 helium-3.2.2/helium.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1125 2023-07-17 12:39:13.000000 helium-3.2.2/helium.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      736 2023-07-17 12:39:13.000000 helium-3.2.2/helium.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-07-17 12:39:13.000000 helium-3.2.2/helium.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2021-03-16 06:50:17.000000 helium-3.2.2/helium.egg-info/not-zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-07-17 12:39:13.000000 helium-3.2.2/helium.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-07-17 12:39:13.000000 helium-3.2.2/helium.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-17 12:39:13.161753 helium-3.2.2/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     1465 2023-07-17 12:38:32.000000 helium-3.2.2/setup.py
```

### Comparing `helium-3.2.1/PKG-INFO` & `helium-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: helium
-Version: 3.2.1
+Version: 3.2.2
 Summary: Lighter browser automation based on Selenium.
 Home-page: https://github.com/mherrmann/selenium-python-helium
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: helium selenium browser automation
```

### Comparing `helium-3.2.1/README.md` & `helium-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/__init__.py` & `helium-3.2.2/helium/__init__.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/__init__.py` & `helium-3.2.2/helium/_impl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -718,21 +718,29 @@
 		return Point(self.x, self.y)
 	@property
 	def web_element(self):
 		return self.first_occurrence.unwrap()
 	def find_all_occurrences(self):
 		self._handle_closed_window()
 		self._driver.switch_to.default_content()
+		already_yielded = set()
 		try:
 			for frame_index in FrameIterator(self._driver):
 				search_regions = self._get_search_regions_in_curr_frame()
 				for occurrence in self.find_all_in_curr_frame():
 					if self._should_yield(occurrence, search_regions):
+						if occurrence.target in already_yielded:
+							# We have seen this element before, but its frame
+							# had a different index. This means that the frames
+							# have changed. Prevent the element from appearing
+							# in results multiple times and abort:
+							raise FramesChangedWhileIterating()
 						occurrence.frame_index = frame_index
 						yield occurrence
+						already_yielded.add(occurrence.target)
 		except FramesChangedWhileIterating:
 			# Abort this search.
 			pass
 	def _handle_closed_window(self):
 		window_handles = self._driver.window_handles
 		try:
 			curr_window_handle = self._driver.current_window_handle
```

### Comparing `helium-3.2.1/helium/_impl/chromedriver.py` & `helium-3.2.2/helium/_impl/chromedriver.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/match_type.py` & `helium-3.2.2/helium/_impl/match_type.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/selenium_wrappers.py` & `helium-3.2.2/helium/_impl/selenium_wrappers.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/util/geom.py` & `helium-3.2.2/helium/_impl/util/geom.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/util/html.py` & `helium-3.2.2/helium/_impl/util/html.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/util/inspect_.py` & `helium-3.2.2/helium/_impl/util/inspect_.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/util/lang.py` & `helium-3.2.2/helium/_impl/util/lang.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/util/path.py` & `helium-3.2.2/helium/_impl/util/path.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/webdrivers/linux/geckodriver` & `helium-3.2.2/helium/_impl/webdrivers/linux/geckodriver`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/webdrivers/mac/geckodriver` & `helium-3.2.2/helium/_impl/webdrivers/mac/geckodriver`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium/_impl/webdrivers/windows/geckodriver.exe` & `helium-3.2.2/helium/_impl/webdrivers/windows/geckodriver.exe`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/helium.egg-info/PKG-INFO` & `helium-3.2.2/helium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: helium
-Version: 3.2.1
+Version: 3.2.2
 Summary: Lighter browser automation based on Selenium.
 Home-page: https://github.com/mherrmann/selenium-python-helium
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: helium selenium browser automation
```

### Comparing `helium-3.2.1/helium.egg-info/SOURCES.txt` & `helium-3.2.2/helium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helium-3.2.1/setup.py` & `helium-3.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'helium',
 	# Also update docs/conf.py when you change this:
-	version = '3.2.1',
+	version = '3.2.2',
 	author = 'Michael Herrmann',
 	author_email = 'michael+removethisifyouarehuman@herrmann.io',
 	description = 'Lighter browser automation based on Selenium.',
 	keywords = 'helium selenium browser automation',
 	url = 'https://github.com/mherrmann/selenium-python-helium',
 	python_requires='>=3',
 	packages = find_packages(exclude=['tests', 'tests.*']),
```

