# Comparing `tmp/chartart-0.0.3.dev18.tar.gz` & `tmp/chartart-0.0.3.dev19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev18.tar", last modified: Tue Jun 20 13:44:15 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev19.tar", last modified: Mon Jul 17 14:57:18 2023, max compression
```

## Comparing `chartart-0.0.3.dev18.tar` & `chartart-0.0.3.dev19.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.572776 chartart-0.0.3.dev18/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2443 2023-06-20 13:44:15.573065 chartart-0.0.3.dev18/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     1921 2023-06-20 13:39:39.000000 chartart-0.0.3.dev18/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-06-20 13:44:15.574754 chartart-0.0.3.dev18/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.533692 chartart-0.0.3.dev18/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.562196 chartart-0.0.3.dev18/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    86312 2023-06-20 13:39:50.000000 chartart-0.0.3.dev18/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.569925 chartart-0.0.3.dev18/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.567939 chartart-0.0.3.dev18/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2443 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.571831 chartart-0.0.3.dev18/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-17 14:57:18.180307 chartart-0.0.3.dev19/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2575 2023-07-17 14:57:18.180600 chartart-0.0.3.dev19/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2053 2023-07-17 14:56:57.000000 chartart-0.0.3.dev19/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-07-17 14:57:18.182068 chartart-0.0.3.dev19/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-17 14:57:18.159842 chartart-0.0.3.dev19/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-17 14:57:18.170756 chartart-0.0.3.dev19/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    87281 2023-07-17 14:53:00.000000 chartart-0.0.3.dev19/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-17 14:57:18.177938 chartart-0.0.3.dev19/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-17 14:57:18.175457 chartart-0.0.3.dev19/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2575 2023-07-17 14:57:18.000000 chartart-0.0.3.dev19/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-07-17 14:57:18.000000 chartart-0.0.3.dev19/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-07-17 14:57:18.000000 chartart-0.0.3.dev19/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-07-17 14:57:18.000000 chartart-0.0.3.dev19/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-07-17 14:57:18.000000 chartart-0.0.3.dev19/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-17 14:57:18.179181 chartart-0.0.3.dev19/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev19/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev18/LICENSE` & `chartart-0.0.3.dev19/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev18/PKG-INFO` & `chartart-0.0.3.dev19/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev18
+Version: 0.0.3.dev19
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -73,7 +73,11 @@
 - Tree Map : c (color) param is optional
 - Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
 - Map : added support fo sub layers. 
 
 0.0.3.dev18
 - Added startAngle, endAngle, radius, groupTo in circular chart
 - Added number format on axis
+
+0.0.3.dev19
+- added support to specify axis type 
+- Made default bin interval is 0 . 0 means syncfusion will calculate internally.
```

### Comparing `chartart-0.0.3.dev18/README.md` & `chartart-0.0.3.dev19/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,8 +56,12 @@
 0.0.3.dev14 => 0.0.3.dev15
 - Tree Map : c (color) param is optional
 - Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
 - Map : added support fo sub layers. 
 
 0.0.3.dev18
 - Added startAngle, endAngle, radius, groupTo in circular chart
-- Added number format on axis
+- Added number format on axis
+
+0.0.3.dev19
+- added support to specify axis type 
+- Made default bin interval is 0 . 0 means syncfusion will calculate internally.
```

### Comparing `chartart-0.0.3.dev18/setup.cfg` & `chartart-0.0.3.dev19/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev18
+version = 0.0.3.dev19
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev18/src/chartart/__init__.py` & `chartart-0.0.3.dev19/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev18/src/chartart/conftest.py` & `chartart-0.0.3.dev19/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev18/src/chartart/helpers.py` & `chartart-0.0.3.dev19/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev18/src/chartart/plot.py` & `chartart-0.0.3.dev19/src/chartart/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,22 @@
          self.xAxisProperties['numberFormat'] = xAxisNumberFormat
 
     def set_xAxisRangePadding(self, xAxisRangePadding: str):
          self.xAxisProperties['rangePadding'] = xAxisRangePadding
 
     def set_xAxisPlotOffset(self, xAxisPlotOffset: float):
          self.xAxisProperties['plotOffset'] = xAxisPlotOffset
+    
+    def set_xAxisType(self, xAxisType: str):
+         """
+         Used to override axis type internally decided by library. Flow : create Figure create chart and then set axis type. 
+         Usefull in case of bar/column chart where seris is numeric but to look better in zoom we will make it catagorical.
+         :param xAxisType  numeric OR datetime OR category/categorical OR datetimeCategory OR logarithmic
+         """
+         self.xAxisProperties['xAxisType'] = xAxisType
 
     def set_yAxisMaximum(self, yAxisMaximum: Union[int, float, str]):
          self.yAxisProperties['maximum'] = yAxisMaximum
 
     def set_yAxisMinimum(self, yAxisMinimum: Union[int, float, str]):
          self.yAxisProperties['minimum'] = yAxisMinimum
 
@@ -374,14 +382,22 @@
 
     def set_yAxisRangePadding(self, yAxisRangePadding: str):
          self.yAxisProperties['rangePadding'] = yAxisRangePadding
 
     def set_yAxisPlotOffset(self, yAxisPlotOffset: float):
          self.yAxisProperties['plotOffset'] = yAxisPlotOffset
 
+    def set_yAxisType(self, yAxisType: str):
+         """
+         Used to override axis type internally decided by library. Flow : create Figure create chart and then set axis type. 
+         Usefull in case of bar/column chart where seris is numeric but to look better in zoom we will make it catagorical.
+         :param xAxisType  numeric OR datetime OR category/categorical OR datetimeCategory OR logarithmic
+         """
+         self.yAxisProperties['yAxisType'] = yAxisType
+
     def set_annotation(self, htmlText: str, x: Optional[Union[int, float, str]] = None, y: Optional[Union[int, float, str]] = None, radius: Optional[str] = None):
         """
         Use this method to add annotation on cartesian or circular chart
         Call this method multiple times to add multiple annotations
         :param htmlText: Annotation content in the form of html text
         :param x: x axis % or value in case of cartesian chart
         :param y: y axis % or value in case of cartesian chart
@@ -1015,15 +1031,15 @@
             formatted_x_data.append(xy_grp_id)
             formatted_y_data.append({'data': xy_grp_df['y'].tolist()})
 
         return formatted_x_data, formatted_y_data
 
     def hist(self, y: Union[str, list, np.ndarray, pd.Series],
              data: Optional[pd.DataFrame] = None, c: Optional[str] = None,
-             binwidth: int = 50, show_normal_curve: bool = False,
+             binwidth: int = 0, show_normal_curve: bool = False,
              labels: Optional[list] = None, animationDelay: Optional[float] = None, 
              animationDuration: Optional[float] = None, sortOrder: Optional[str]= None, sortOn: Optional[str]=None):
         """
         :param sortOrder: sort order or series. possible values asc/ascending , des/descending
         :param sortOn: sort on value of x or y. possible values are x/X , y/Y
         """
         if data is None:
```

### Comparing `chartart-0.0.3.dev18/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev19/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev18/src/chartart/test_plot.py` & `chartart-0.0.3.dev19/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev18/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev19/src/chartart.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev18
+Version: 0.0.3.dev19
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -73,7 +73,11 @@
 - Tree Map : c (color) param is optional
 - Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
 - Map : added support fo sub layers. 
 
 0.0.3.dev18
 - Added startAngle, endAngle, radius, groupTo in circular chart
 - Added number format on axis
+
+0.0.3.dev19
+- added support to specify axis type 
+- Made default bin interval is 0 . 0 means syncfusion will calculate internally.
```

