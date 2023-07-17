# Comparing `tmp/windeklar-0.2.5.tar.gz` & `tmp/windeklar-0.2.6.tar.gz`

## Comparing `windeklar-0.2.5.tar` & `windeklar-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.5/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.5/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/__init__.py
--rwxr-xr-x   0        0        0    16215 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    45955 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.5/LICENSE
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 windeklar-0.2.5/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 windeklar-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.6/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.6/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/__init__.py
+-rwxr-xr-x   0        0        0    16332 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    45955 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 windeklar-0.2.6/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 windeklar-0.2.6/PKG-INFO
```

### Comparing `windeklar-0.2.5/.github/workflows/python-publish.yml` & `windeklar-0.2.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.2.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/QTAux.py` & `windeklar-0.2.6/src/WinDeklar/QTAux.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         # bound is the object responsible to keep the value, must implement:
         #     get_control_value
         #     set_control_value
         self.name    = name
         self.ename   = title
         self.bounded = bound
         self.action  = action
+        self.label   = None
 
         # print('control:%s bound:%s, action:%s' % (name, bound, action))
 
         self.bounded_name = 'self.bounded.'
  
         is_widget, widget = self.get_widget()
         if is_widget and layout is not None:
@@ -127,14 +128,16 @@
         if widget is not None:
             widget.setFixedWidth(width)
 
     def set_visible(self, is_visible):
         valid, widget = self.get_widget()
         if valid:
             widget.setVisible(is_visible)
+            if self.label is not None:
+                self.label.setVisible(is_visible)
 
 
 class EnumCombo(ScreenControl):
     def __init__(self, name, title, bound, enum, action, layout, tooltip=None):
     
         self.enum  = enum
         self.combo = QtWidgets.QComboBox(None)
```

### Comparing `windeklar-0.2.5/src/WinDeklar/WindowForm.py` & `windeklar-0.2.6/src/WinDeklar/WindowForm.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/graph_aux.py` & `windeklar-0.2.6/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/points_box.py` & `windeklar-0.2.6/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/record.py` & `windeklar-0.2.6/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/signal_aux.py` & `windeklar-0.2.6/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/test_animation.py` & `windeklar-0.2.6/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/test_pyqt.py` & `windeklar-0.2.6/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/view_animation.py` & `windeklar-0.2.6/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/view_animation.yaml` & `windeklar-0.2.6/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/view_example.py` & `windeklar-0.2.6/src/WinDeklar/view_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,17 @@
 
     def initialize(self):
         """
         Code to run when initializing the form
         In this case it is shown how to set visible (or not) a control
         :return:
         """
+        # example of how to conditional show a control in the screen
         control = self.get_control_by_name('just_text')
-        control.set_visible(True)
+        control.set_visible(False)
 
     # actions
     def event_open_file(self):
         """
         Event defined in the yaml file to be called when File/Open is clicked
         :return:
         """
```

### Comparing `windeklar-0.2.5/src/WinDeklar/view_example.yaml` & `windeklar-0.2.6/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/view_simple_graph.py` & `windeklar-0.2.6/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/src/WinDeklar/yaml_functions.py` & `windeklar-0.2.6/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/LICENSE` & `windeklar-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/README.md` & `windeklar-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.5/pyproject.toml` & `windeklar-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.2.5/PKG-INFO` & `windeklar-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.2.5
+Version: 0.2.6
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

