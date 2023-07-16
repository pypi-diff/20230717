# Comparing `tmp/application_properties-0.7.0.tar.gz` & `tmp/application_properties-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "application_properties-0.7.0.tar", last modified: Sun Apr 23 21:02:14 2023, max compression
+gzip compressed data, was "application_properties-0.8.0.tar", last modified: Sun Jul 16 21:53:09 2023, max compression
```

## Comparing `application_properties-0.7.0.tar` & `application_properties-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.370810 application_properties-0.7.0/
--rw-rw-rw-   0        0        0     1066 2022-08-24 23:33:16.000000 application_properties-0.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0       75 2022-08-24 23:33:16.000000 application_properties-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5862 2023-04-23 21:02:14.371812 application_properties-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    12928 2022-08-24 23:33:16.000000 application_properties-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.352810 application_properties-0.7.0/application_properties/
--rw-rw-rw-   0        0        0      893 2023-04-23 16:36:58.000000 application_properties-0.7.0/application_properties/__init__.py
--rw-rw-rw-   0        0        0    17006 2023-04-23 03:07:39.000000 application_properties-0.7.0/application_properties/application_properties.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 13:51:18.000000 application_properties-0.7.0/application_properties/application_properties_config_loader.py
--rw-rw-rw-   0        0        0     4911 2022-08-24 23:33:16.000000 application_properties-0.7.0/application_properties/application_properties_facade.py
--rw-rw-rw-   0        0        0     3048 2023-04-23 03:27:58.000000 application_properties-0.7.0/application_properties/application_properties_json_loader.py
--rw-rw-rw-   0        0        0      955 2023-04-23 03:26:29.000000 application_properties-0.7.0/application_properties/application_properties_loader_helper.py
--rw-rw-rw-   0        0        0     3566 2023-04-23 03:27:58.000000 application_properties-0.7.0/application_properties/application_properties_toml_loader.py
--rw-rw-rw-   0        0        0       13 2022-08-24 23:33:16.000000 application_properties-0.7.0/application_properties/py.typed
--rw-rw-rw-   0        0        0       65 2023-04-23 02:12:55.000000 application_properties-0.7.0/application_properties/version.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.357810 application_properties-0.7.0/application_properties.egg-info/
--rw-rw-rw-   0        0        0     5862 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 13:44:16.000000 application_properties-0.7.0/install-requirements.txt
--rw-rw-rw-   0        0        0      696 2023-04-23 21:02:14.372813 application_properties-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     2691 2022-08-24 23:33:16.000000 application_properties-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.370810 application_properties-0.7.0/test/
--rw-rw-rw-   0        0        0    13948 2023-04-09 23:30:24.000000 application_properties-0.7.0/test/test_application_properties.py
--rw-rw-rw-   0        0        0    23261 2023-04-23 14:22:47.000000 application_properties-0.7.0/test/test_application_properties_config_loader.py
--rw-rw-rw-   0        0        0     8524 2022-08-24 23:33:16.000000 application_properties-0.7.0/test/test_application_properties_facade.py
--rw-rw-rw-   0        0        0    14040 2023-04-23 14:22:30.000000 application_properties-0.7.0/test/test_application_properties_json_loader.py
--rw-rw-rw-   0        0        0    22990 2023-04-23 14:22:38.000000 application_properties-0.7.0/test/test_application_properties_toml_loader.py
--rw-rw-rw-   0        0        0     3837 2022-08-24 23:33:16.000000 application_properties-0.7.0/test/test_get_boolean.py
--rw-rw-rw-   0        0        0     3821 2022-08-24 23:33:16.000000 application_properties-0.7.0/test/test_get_integer.py
--rw-rw-rw-   0        0        0     6155 2023-04-10 00:07:55.000000 application_properties-0.7.0/test/test_get_string.py
--rw-rw-rw-   0        0        0     1437 2023-04-23 14:24:39.000000 application_properties-0.7.0/test/test_helpers.py
--rw-rw-rw-   0        0        0    24230 2023-04-21 02:48:51.000000 application_properties-0.7.0/test/test_set_manual_property.py
--rw-rw-rw-   0        0        0      510 2021-06-05 04:57:29.000000 application_properties-0.7.0/test/test_version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.716650 application_properties-0.8.0/
+-rw-rw-rw-   0        0        0     1066 2023-05-14 22:38:18.000000 application_properties-0.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2023-07-16 16:33:32.000000 application_properties-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5862 2023-07-16 21:53:09.716650 application_properties-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8311 2023-07-15 23:41:15.000000 application_properties-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.698560 application_properties-0.8.0/application_properties/
+-rw-rw-rw-   0        0        0       13 2023-05-14 22:38:18.000000 application_properties-0.8.0/application_properties/.external-package
+-rw-rw-rw-   0        0        0     1339 2023-07-16 21:17:57.000000 application_properties-0.8.0/application_properties/__init__.py
+-rw-rw-rw-   0        0        0    17605 2023-07-16 03:47:33.000000 application_properties-0.8.0/application_properties/application_properties.py
+-rw-rw-rw-   0        0        0     8126 2023-04-28 01:01:24.000000 application_properties-0.8.0/application_properties/application_properties_config_loader.py
+-rw-rw-rw-   0        0        0     4911 2022-08-24 23:33:16.000000 application_properties-0.8.0/application_properties/application_properties_facade.py
+-rw-rw-rw-   0        0        0     3048 2023-04-23 03:27:58.000000 application_properties-0.8.0/application_properties/application_properties_json_loader.py
+-rw-rw-rw-   0        0        0      955 2023-04-23 03:26:29.000000 application_properties-0.8.0/application_properties/application_properties_loader_helper.py
+-rw-rw-rw-   0        0        0     3566 2023-04-23 03:27:58.000000 application_properties-0.8.0/application_properties/application_properties_toml_loader.py
+-rw-rw-rw-   0        0        0     4117 2023-07-16 21:41:04.000000 application_properties-0.8.0/application_properties/application_properties_utilities.py
+-rw-rw-rw-   0        0        0     4555 2023-07-16 04:02:08.000000 application_properties-0.8.0/application_properties/application_properties_yaml_loader.py
+-rw-rw-rw-   0        0        0       13 2023-05-14 22:38:18.000000 application_properties-0.8.0/application_properties/py.typed
+-rw-rw-rw-   0        0        0      212 2023-07-16 21:40:50.000000 application_properties-0.8.0/application_properties/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.703559 application_properties-0.8.0/application_properties.egg-info/
+-rw-rw-rw-   0        0        0     5862 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1368 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       40 2023-07-15 15:07:10.000000 application_properties-0.8.0/install-requirements.txt
+-rw-rw-rw-   0        0        0      798 2023-07-16 21:53:09.717650 application_properties-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     3084 2023-07-16 17:47:15.000000 application_properties-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.715774 application_properties-0.8.0/test/
+-rw-rw-rw-   0        0        0    14171 2023-07-16 21:41:52.000000 application_properties-0.8.0/test/test_application_properties.py
+-rw-rw-rw-   0        0        0    23586 2023-06-25 21:12:27.000000 application_properties-0.8.0/test/test_application_properties_config_loader.py
+-rw-rw-rw-   0        0        0     8820 2023-06-25 20:38:43.000000 application_properties-0.8.0/test/test_application_properties_facade.py
+-rw-rw-rw-   0        0        0    14361 2023-07-16 03:30:16.000000 application_properties-0.8.0/test/test_application_properties_json_loader.py
+-rw-rw-rw-   0        0        0    23303 2023-06-25 21:14:32.000000 application_properties-0.8.0/test/test_application_properties_toml_loader.py
+-rw-rw-rw-   0        0        0    20569 2023-07-15 19:12:59.000000 application_properties-0.8.0/test/test_application_properties_utilities.py
+-rw-rw-rw-   0        0        0    24775 2023-07-16 03:36:04.000000 application_properties-0.8.0/test/test_application_properties_yaml_loader.py
+-rw-rw-rw-   0        0        0     3917 2023-06-25 20:34:07.000000 application_properties-0.8.0/test/test_get_boolean.py
+-rw-rw-rw-   0        0        0     3885 2023-06-25 20:34:32.000000 application_properties-0.8.0/test/test_get_integer.py
+-rw-rw-rw-   0        0        0     6299 2023-06-25 20:58:42.000000 application_properties-0.8.0/test/test_get_string.py
+-rw-rw-rw-   0        0        0    24741 2023-07-16 03:26:31.000000 application_properties-0.8.0/test/test_set_manual_property.py
+-rw-rw-rw-   0        0        0      518 2023-06-25 19:04:56.000000 application_properties-0.8.0/test/test_version.py
```

### Comparing `application_properties-0.7.0/LICENSE.txt` & `application_properties-0.8.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2020-2022 Jack De Winter
+Copyright 2019-2023 Jack De Winter
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `application_properties-0.7.0/PKG-INFO` & `application_properties-0.8.0/application_properties.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: application_properties
-Version: 0.7.0
+Name: application-properties
+Version: 0.8.0
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
```

### Comparing `application_properties-0.7.0/application_properties/__init__.py` & `application_properties-0.8.0/application_properties/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 """
 Module to provide for easy access to various property file formats.
+
+https://stackoverflow.com/questions/44834/what-does-all-mean-in-python#When%20Avoiding%20__all__%20Makes%20Sense
 """
 from application_properties.application_properties import (  # noqa F401
     ApplicationProperties,
 )
+from application_properties.application_properties_config_loader import (  # noqa F401
+    ApplicationPropertiesConfigLoader,
+)
 from application_properties.application_properties_facade import (  # noqa F401
     ApplicationPropertiesFacade,
 )
 from application_properties.application_properties_json_loader import (  # noqa F401
     ApplicationPropertiesJsonLoader,
 )
 from application_properties.application_properties_toml_loader import (  # noqa F401
     ApplicationPropertiesTomlLoader,
 )
-from application_properties.application_properties_config_loader import (  # noqa F401
-    ApplicationPropertiesConfigLoader,
+from application_properties.application_properties_utilities import (  # noqa F401
+    ApplicationPropertiesUtilities,
+)
+from application_properties.application_properties_yaml_loader import (  # noqa F401
+    ApplicationPropertiesYamlLoader,
 )
 
 __all__ = [
     "ApplicationProperties",
+    "ApplicationPropertiesUtilities",
     "ApplicationPropertiesFacade",
     "ApplicationPropertiesJsonLoader",
     "ApplicationPropertiesTomlLoader",
+    "ApplicationPropertiesYamlLoader",
     "ApplicationPropertiesConfigLoader",
 ]
```

### Comparing `application_properties-0.7.0/application_properties/application_properties.py` & `application_properties-0.8.0/application_properties/application_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,18 +115,20 @@
         """
 
         if (
             " " in property_key
             or "\t" in property_key
             or "\n" in property_key
             or ApplicationProperties.__assignment_operator in property_key
+            or ApplicationProperties.__separator in property_key
         ):
             raise ValueError(
-                "Each part of the property key must not contain a "
-                + f"whitespace character or the '{ApplicationProperties.__separator}' character."
+                "Each part of the property key cannot contain a whitespace character, "
+                + f"a '{ApplicationProperties.__assignment_operator}' character, or "
+                + f"a '{ApplicationProperties.__separator}' character."
             )
         if not property_key:
             raise ValueError(
                 "Each part of the property key must contain at least one character."
             )
         return property_key
 
@@ -242,16 +244,14 @@
             composed_property_value = property_value[2:].lower() == "true"
         else:
             composed_property_value = property_value[1:]
         return composed_property_value
 
     # pylint: disable=unidiomatic-typecheck
     # pylint: disable=too-many-arguments
-    # pylint: disable=broad-except
-    # pylint: disable=raise-missing-from
     def get_property(
         self,
         property_name: str,
         property_type: type,
         default_value: Any = None,
         valid_value_fn: Optional[Callable[[Any], Any]] = None,
         is_required: bool = False,
@@ -290,14 +290,18 @@
             )
         elif is_required:
             raise ValueError(
                 f"A value for property '{property_name}' must be provided."
             )
         return property_value
 
+    # pylint: enable=unidiomatic-typecheck
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=unidiomatic-typecheck
     def __get_present_property_value(
         self, property_name: str, property_type: type
     ) -> Tuple[bool, Any]:
         found_value = self.__flat_property_map[property_name]
         is_eligible = type(found_value) == property_type
 
         covertable_property_name = f"{ApplicationProperties.__separator}{property_name}"
@@ -315,14 +319,17 @@
                 found_value = f"{ApplicationProperties.__manual_property_type_prefix}{ApplicationProperties.__manual_property_type_integer}{found_value}"
             with contextlib.suppress(ValueError):
                 found_value = self.__adjust_property_type(found_value)
                 is_eligible = True
             # print(f"::{covertable_property_name}::{found_value}::")
         return is_eligible, found_value
 
+    # pylint: enable=unidiomatic-typecheck
+
+    # pylint: disable=too-many-arguments, broad-exception-caught
     def __get_present_property(
         self,
         property_name: str,
         property_value: Any,
         property_type: type,
         strict_mode: bool,
         valid_value_fn: Optional[Callable[[Any], Any]],
@@ -343,18 +350,15 @@
                     raise ValueError(
                         f"The value for property '{property_name}' is not valid: {str(this_exception)}"
                     ) from this_exception
         if is_eligible:
             property_value = found_value
         return property_value
 
-    # pylint: enable=unidiomatic-typecheck
-    # pylint: enable=too-many-arguments
-    # pylint: enable=broad-except
-    # pylint: enable=raise-missing-from
+    # pylint: enable=too-many-arguments, broad-exception-caught
 
     def get_boolean_property(
         self,
         property_name: str,
         default_value: Optional[bool] = None,
         is_required: bool = False,
         strict_mode: Optional[bool] = None,
@@ -439,17 +443,25 @@
 
     def __scan_map(self, config_map: Dict[Any, Any], current_prefix: str) -> None:
         for next_key, next_value in config_map.items():
             if not isinstance(next_key, str):
                 raise ValueError(
                     "All keys in the main dictionary and nested dictionaries must be strings."
                 )
-            if self.__separator in next_key:
+            if (
+                " " in next_key
+                or "\t" in next_key
+                or "\n" in next_key
+                or ApplicationProperties.__assignment_operator in next_key
+                or ApplicationProperties.__separator in next_key
+            ):
                 raise ValueError(
-                    f"Keys strings cannot contain the separator character '{self.__separator}'."
+                    "Key strings cannot contain a whitespace character, "
+                    + f"a '{ApplicationProperties.__assignment_operator}' character, or "
+                    + f"a '{ApplicationProperties.__separator}' character."
                 )
 
             if isinstance(next_value, dict):
                 self.__scan_map(
                     next_value, f"{current_prefix}{next_key}{self.__separator}"
                 )
             else:
```

### Comparing `application_properties-0.7.0/application_properties/application_properties_config_loader.py` & `application_properties-0.8.0/application_properties/application_properties_config_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.7.0/application_properties/application_properties_facade.py` & `application_properties-0.8.0/application_properties/application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.7.0/application_properties/application_properties_json_loader.py` & `application_properties-0.8.0/application_properties/application_properties_json_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.7.0/application_properties/application_properties_loader_helper.py` & `application_properties-0.8.0/application_properties/application_properties_loader_helper.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.7.0/application_properties/application_properties_toml_loader.py` & `application_properties-0.8.0/application_properties/application_properties_toml_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.7.0/application_properties.egg-info/PKG-INFO` & `application_properties-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: application-properties
-Version: 0.7.0
+Name: application_properties
+Version: 0.8.0
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
```

### Comparing `application_properties-0.7.0/application_properties.egg-info/SOURCES.txt` & `application_properties-0.8.0/application_properties.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 install-requirements.txt
 setup.cfg
 setup.py
+application_properties/.external-package
 application_properties/__init__.py
 application_properties/application_properties.py
 application_properties/application_properties_config_loader.py
 application_properties/application_properties_facade.py
 application_properties/application_properties_json_loader.py
 application_properties/application_properties_loader_helper.py
 application_properties/application_properties_toml_loader.py
+application_properties/application_properties_utilities.py
+application_properties/application_properties_yaml_loader.py
 application_properties/py.typed
 application_properties/version.py
 application_properties.egg-info/PKG-INFO
 application_properties.egg-info/SOURCES.txt
 application_properties.egg-info/dependency_links.txt
 application_properties.egg-info/requires.txt
 application_properties.egg-info/top_level.txt
 test/test_application_properties.py
 test/test_application_properties_config_loader.py
 test/test_application_properties_facade.py
 test/test_application_properties_json_loader.py
 test/test_application_properties_toml_loader.py
+test/test_application_properties_utilities.py
+test/test_application_properties_yaml_loader.py
 test/test_get_boolean.py
 test/test_get_integer.py
 test/test_get_string.py
-test/test_helpers.py
 test/test_set_manual_property.py
 test/test_version.py
```

### Comparing `application_properties-0.7.0/setup.cfg` & `application_properties-0.8.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -13,32 +13,38 @@
 000000c0: 2d6c 696e 652d 6c65 6e67 7468 203d 2038  -line-length = 8
 000000d0: 380d 0a6d 6178 2d63 6f6d 706c 6578 6974  8..max-complexit
 000000e0: 7920 3d20 3138 0d0a 7365 6c65 6374 203d  y = 18..select =
 000000f0: 2042 2c43 2c45 2c46 2c57 2c54 340d 0a0d   B,C,E,F,W,T4...
 00000100: 0a5b 7079 6c69 6e74 5d0d 0a64 6973 6162  .[pylint]..disab
 00000110: 6c65 203d 2043 3033 3031 2c20 5730 3531  le = C0301, W051
 00000120: 312c 2064 7570 6c69 6361 7465 2d63 6f64  1, duplicate-cod
-00000130: 650d 0a65 7874 656e 7369 6f6e 2d70 6b67  e..extension-pkg
-00000140: 2d77 6869 7465 6c69 7374 203d 2077 696e  -whitelist = win
-00000150: 3332 6170 690d 0a0d 0a5b 746f 6f6c 3a70  32api....[tool:p
-00000160: 7974 6573 745d 0d0a 7465 7374 7061 7468  ytest]..testpath
-00000170: 7320 3d20 2e2f 7465 7374 0d0a 6361 6368  s = ./test..cach
-00000180: 655f 6469 7220 3d20 2e2f 6275 696c 642f  e_dir = ./build/
-00000190: 7465 7374 2f2e 7079 7465 7374 5f63 6163  test/.pytest_cac
-000001a0: 6865 0d0a 6a75 6e69 745f 6661 6d69 6c79  he..junit_family
-000001b0: 203d 2078 756e 6974 320d 0a61 6464 6f70   = xunit2..addop
-000001c0: 7473 203d 202d 2d74 696d 656f 7574 3d31  ts = --timeout=1
-000001d0: 3020 2d2d 6874 6d6c 3d72 6570 6f72 742f  0 --html=report/
-000001e0: 7265 706f 7274 2e68 746d 6c20 2d2d 636f  report.html --co
-000001f0: 7620 2d2d 636f 762d 6272 616e 6368 202d  v --cov-branch -
-00000200: 2d63 6f76 2d66 6169 6c2d 756e 6465 723d  -cov-fail-under=
-00000210: 3830 202d 2d73 7472 6963 742d 6d61 726b  80 --strict-mark
-00000220: 6572 7320 2d72 6120 2d2d 636f 762d 7265  ers -ra --cov-re
-00000230: 706f 7274 2078 6d6c 3a72 6570 6f72 742f  port xml:report/
-00000240: 636f 7665 7261 6765 2e78 6d6c 202d 2d63  coverage.xml --c
-00000250: 6f76 2d72 6570 6f72 7420 6874 6d6c 3a72  ov-report html:r
-00000260: 6570 6f72 742f 636f 7665 7261 6765 202d  eport/coverage -
-00000270: 2d6a 756e 6974 786d 6c3d 7265 706f 7274  -junitxml=report
-00000280: 2f74 6573 7473 2e78 6d6c 0d0a 0d0a 5b65  /tests.xml....[e
-00000290: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000002a0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000002b0: 203d 2030 0d0a 0d0a                       = 0....
+00000130: 652c 2063 7963 6c69 632d 696d 706f 7274  e, cyclic-import
+00000140: 0d0a 6578 7465 6e73 696f 6e2d 706b 672d  ..extension-pkg-
+00000150: 7768 6974 656c 6973 7420 3d20 7769 6e33  whitelist = win3
+00000160: 3261 7069 0d0a 0d0a 5b74 6f6f 6c3a 7079  2api....[tool:py
+00000170: 7465 7374 5d0d 0a74 6573 7470 6174 6873  test]..testpaths
+00000180: 203d 202e 2f74 6573 740d 0a63 6163 6865   = ./test..cache
+00000190: 5f64 6972 203d 202e 2f62 7569 6c64 2f74  _dir = ./build/t
+000001a0: 6573 742f 2e70 7974 6573 745f 6361 6368  est/.pytest_cach
+000001b0: 650d 0a6a 756e 6974 5f66 616d 696c 7920  e..junit_family 
+000001c0: 3d20 7875 6e69 7432 0d0a 7079 7468 6f6e  = xunit2..python
+000001d0: 5f63 6c61 7373 6573 203d 204e 6f54 6861  _classes = NoTha
+000001e0: 6e6b 730d 0a61 6464 6f70 7473 203d 202d  nks..addopts = -
+000001f0: 2d74 696d 656f 7574 3d31 3020 2d2d 6874  -timeout=10 --ht
+00000200: 6d6c 3d72 6570 6f72 742f 7265 706f 7274  ml=report/report
+00000210: 2e68 746d 6c20 2d2d 636f 7620 2d2d 636f  .html --cov --co
+00000220: 762d 6272 616e 6368 202d 2d63 6f76 2d66  v-branch --cov-f
+00000230: 6169 6c2d 756e 6465 723d 3530 202d 2d73  ail-under=50 --s
+00000240: 7472 6963 742d 6d61 726b 6572 7320 2d72  trict-markers -r
+00000250: 6120 2d2d 636f 762d 7265 706f 7274 2078  a --cov-report x
+00000260: 6d6c 3a72 6570 6f72 742f 636f 7665 7261  ml:report/covera
+00000270: 6765 2e78 6d6c 202d 2d63 6f76 2d72 6570  ge.xml --cov-rep
+00000280: 6f72 7420 6874 6d6c 3a72 6570 6f72 742f  ort html:report/
+00000290: 636f 7665 7261 6765 202d 2d6a 756e 6974  coverage --junit
+000002a0: 786d 6c3d 7265 706f 7274 2f74 6573 7473  xml=report/tests
+000002b0: 2e78 6d6c 0d0a 0d0a 5b74 6f6f 6c2e 6d79  .xml....[tool.my
+000002c0: 7079 5d0d 0a6d 7970 795f 7061 7468 203d  py]..mypy_path =
+000002d0: 2027 7374 7562 7327 0d0a 7761 726e 5f72   'stubs'..warn_r
+000002e0: 6574 7572 6e5f 616e 7920 3d20 7472 7565  eturn_any = true
+000002f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000300: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000310: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `application_properties-0.7.0/setup.py` & `application_properties-0.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,54 +3,71 @@
 """
 
 import os
 import runpy
 
 from setuptools import setup
 
+INSTALL_REQUIREMENT_FILE = "install-requirements.txt"
 PROJECT_README_FILE = "README.md"
 ALTERNATE_PYPI_README_FILE = "pypi.md"
-INSTALL_REQUIREMENT_FILE = "install-requirements.txt"
 
 
 def parse_requirements():
     with open(f"{INSTALL_REQUIREMENT_FILE}", "r", encoding="utf-8") as requirement_file:
         lineiter = [line.strip() for line in requirement_file]
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 def get_semantic_version():
     version_meta = runpy.run_path(f"./{PACKAGE_NAME}/version.py")
     return version_meta["__version__"]
 
 
+def get_project_name():
+    version_meta = runpy.run_path(f"./{PACKAGE_NAME}/version.py")
+    return version_meta["__project_name__"]
+
+
+def get_description():
+    version_meta = runpy.run_path(f"./{PACKAGE_NAME}/version.py")
+    return version_meta["__description__"]
+
+
 def load_readme_file():
     source_file = (
         ALTERNATE_PYPI_README_FILE
         if os.path.exists(ALTERNATE_PYPI_README_FILE)
         else PROJECT_README_FILE
     )
     with open(source_file, "r", encoding="utf-8") as readme_file:
         return readme_file.read()
 
 
+def get_package_modules():
+    return [
+        next_item[0][2:]
+        for next_item in os.walk(".")
+        if os.path.exists(os.path.join(next_item[0], ".external-package"))
+    ]
+
+
 AUTHOR = "Jack De Winter"
 AUTHOR_EMAIL = "jack.de.winter@outlook.com"
 PROJECT_URL = "https://github.com/jackdewinter/application_properties"
 PROJECT_URLS = {
     "Change Log": "https://github.com/jackdewinter/application_properties/blob/main/changelog.md",
 }
 
 PACKAGE_NAME = "application_properties"
+PROJECT_NAME = get_project_name()
 SEMANTIC_VERSION = get_semantic_version()
 MINIMUM_PYTHON_VERSION = "3.8.0"
 
-ONE_LINE_DESCRIPTION = (
-    "A simple, easy to use, unified manner of accessing program properties."
-)
+ONE_LINE_DESCRIPTION = get_description()
 LONG_DESCRIPTION = load_readme_file()
 LONG_DESCRIPTION_CONTENT_TYPE = "text/markdown"
 
 KEYWORDS = ["properties"]
 PROJECT_CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -59,18 +76,14 @@
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 
-PACKAGE_MODULES = [
-    "application_properties",
-]
-
 setup(
     name=PACKAGE_NAME,
     version=SEMANTIC_VERSION,
     python_requires=f">={MINIMUM_PYTHON_VERSION}",
     install_requires=parse_requirements(),
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
@@ -80,11 +93,11 @@
     description=ONE_LINE_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESCRIPTION_CONTENT_TYPE,
     keywords=KEYWORDS,
     classifiers=PROJECT_CLASSIFIERS,
     project_urls=PROJECT_URLS,
     entry_points={},
-    packages=PACKAGE_MODULES,
+    packages=get_package_modules(),
     include_package_data=True,
     package_data={"": ["*.typed"]},
 )
```

### Comparing `application_properties-0.7.0/test/test_application_properties.py` & `application_properties-0.8.0/test/test_application_properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Tests for the ApplicationProperties class
 """
-from application_properties import ApplicationProperties
+from typing import Any, Dict
 
-# pylint: disable=too-many-lines
+from application_properties import ApplicationProperties
 
 
-def test_property_name_separator():
+def test_property_name_separator() -> None:
     """
     Test to make sure that the property name separator is as expected.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     expected_separator = "."
@@ -18,15 +18,15 @@
     # Act
     actual_separator = application_properties.separator
 
     # Assert
     assert actual_separator == expected_separator
 
 
-def test_properties_with_object():
+def test_properties_with_object() -> None:
     """
     Test to make sure that a default application properties object has no properties.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     expected_property_count = 0
@@ -34,15 +34,15 @@
     # Act
     actual_property_count = application_properties.number_of_properties
 
     # Assert
     assert actual_property_count == expected_property_count
 
 
-def test_properties_with_single_property():
+def test_properties_with_single_property() -> None:
     """
     Test a configuration map with a single property, and how that property looks.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     config_map = {"enabled": True}
@@ -55,15 +55,15 @@
 
     # Assert
     assert actual_property_count == expected_property_count
     assert len(found_names) == expected_property_count
     assert "enabled" in found_names
 
 
-def test_properties_with_single_nested_property():
+def test_properties_with_single_nested_property() -> None:
     """
     Test a configuration map with a single nested property, and how that property looks.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     config_map = {"feature": {"enabled": True}}
@@ -76,15 +76,15 @@
 
     # Assert
     assert actual_property_count == expected_property_count
     assert len(found_names) == expected_property_count
     assert "feature.enabled" in found_names
 
 
-def test_properties_with_mixed_properties():
+def test_properties_with_mixed_properties() -> None:
     """
     Test a configuration map with properties at different levels, and how those properties look.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     config_map = {
@@ -102,21 +102,21 @@
     assert actual_property_count == expected_property_count
     assert len(found_names) == expected_property_count
     assert "feature.enabled" in found_names
     assert "other_feature.enabled" in found_names
     assert "other_feature.other" in found_names
 
 
-def test_get_properties_under_at_top_level_partial():
+def test_get_properties_under_at_top_level_partial() -> None:
     """
     Test calling the `property_names_under` function specifying only part of the top level.
     """
 
     # Arrange
-    config_map = {
+    config_map: Dict[str, Dict[str, Any]] = {
         "feature": {"enabled": True},
         "other_feature": {"enabled": False, "other": 1},
     }
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
@@ -124,36 +124,36 @@
 
     # Assert
     assert len(found_names) == len(config_map["other_feature"])
     assert "other_feature.enabled" in found_names
     assert "other_feature.other" in found_names
 
 
-def test_get_properties_under_at_top_level_none():
+def test_get_properties_under_at_top_level_none() -> None:
     """
     Test calling the `property_names_under` function specifying none of the top level.
     """
 
     # Arrange
-    config_map = {
+    config_map: Dict[str, Dict[str, Any]] = {
         "feature": {"enabled": True},
         "other_feature": {"enabled": False, "other": 1},
     }
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     found_names = application_properties.property_names_under("missing_feature")
 
     # Assert
     assert not found_names
     assert "missing_feature" not in config_map
 
 
-def test_get_properties_under_at_sub_level():
+def test_get_properties_under_at_sub_level() -> None:
     """
     Test calling the `property_names_under` function specifying none of the top level.
     """
 
     # Arrange
     config_map = {
         "new_top_level": {
@@ -164,43 +164,43 @@
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     found_names = application_properties.property_names_under("new_top_level.feature")
 
     # Assert
-    assert len(found_names) == len(config_map["new_top_level"]["feature"])
+    assert len(found_names) == 1
     assert "new_top_level.feature.enabled" in found_names
 
 
-def test_properties_load_from_non_dictionary():
+def test_properties_load_from_non_dictionary() -> None:
     """
     Test a loading a configuration map that is not a dictionary.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     config_map = [{"feature": True}]
 
     # Act
     raised_exception = None
     try:
-        application_properties.load_from_dict(config_map)
+        application_properties.load_from_dict(config_map)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception) == "Specified parameter was not a dictionary."
     ), "Expected message was not present in exception."
 
 
-def test_properties_load_with_non_string_key():
+def test_properties_load_with_non_string_key() -> None:
     """
     Test a loading a configuration map that contains a key that is not a string.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     config_map = {1: True}
@@ -217,15 +217,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "All keys in the main dictionary and nested dictionaries must be strings."
     ), "Expected message was not present in exception."
 
 
-def test_properties_load_with_key_containing_dot():
+def test_properties_load_with_key_containing_dot() -> None:
     """
     Test a loading a configuration map that contains a key with a '.' character.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     config_map = {"my.property": True}
@@ -238,46 +238,46 @@
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
-        == "Keys strings cannot contain the separator character '.'."
+        == "Key strings cannot contain a whitespace character, a '=' character, or a '.' character."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_generic_with_bad_type():
+def test_properties_get_generic_with_bad_type() -> None:
     """
     Test a fetching a configuration value where the generic function is
     used and the type and the default are confused.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_property("property", False)
+        application_properties.get_property("property", False)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "The property_type argument for 'property' must be a type."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_generic_with_required_and_found():
+def test_properties_get_generic_with_required_and_found() -> None:
     """
     Test a fetching a configuration value where the value is required and present.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
@@ -289,15 +289,15 @@
         "property", bool, is_required=True
     )
 
     # Assert
     assert actual_value == expected_value
 
 
-def test_properties_get_generic_with_required_and_not_found():
+def test_properties_get_generic_with_required_and_not_found() -> None:
     """
     Test a fetching a configuration value where the value is required and not present.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
@@ -315,15 +315,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "A value for property 'other_property' must be provided."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_generic_with_strict_mode_and_bad_type():
+def test_properties_get_generic_with_strict_mode_and_bad_type() -> None:
     """
     Test a fetching a configuration value where strict mode is on and the type is not correct.
     """
 
     # Arrange
     config_map = {"property": 1}
     application_properties = ApplicationProperties()
@@ -341,15 +341,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "The value for property 'property' must be of type 'str'."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_generic_with_global_strict_mode_and_bad_type():
+def test_properties_get_generic_with_global_strict_mode_and_bad_type() -> None:
     """
     Test a fetching a configuration value where strict mode is on and the type is not correct.
     """
 
     # Arrange
     config_map = {"property": 1}
     application_properties = ApplicationProperties(strict_mode=True)
@@ -368,15 +368,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "The value for property 'property' must be of type 'str'."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_generic_with_delayed_global_strict_mode_and_bad_type():
+def test_properties_get_generic_with_delayed_global_strict_mode_and_bad_type() -> None:
     """
     Test a fetching a configuration value where strict mode is on through the
     delayed mechanism and the type is not correct.
     """
 
     # Arrange
     config_map = {"property": 1}
@@ -397,23 +397,23 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "The value for property 'property' must be of type 'str'."
     ), "Expected message was not present in exception."
 
 
-def __sample_string_validation_function(property_value):
+def __sample_string_validation_function(property_value: str) -> None:
     """
     Simple string validation that throws an error if not "1" or "2".
     """
     if property_value not in ["1", "2"]:
-        raise ValueError(f"Value '{str(property_value)}' is not '1' or '2'")
+        raise ValueError(f"Value '{property_value}' is not '1' or '2'")
 
 
-def test_properties_get_generic_with_strict_mode_and_bad_validity():
+def test_properties_get_generic_with_strict_mode_and_bad_validity() -> None:
     """
     Test a fetching a configuration value where strict mode is on and the value is not valid.
     """
 
     # Arrange
     config_map = {"property": "3"}
     application_properties = ApplicationProperties()
```

### Comparing `application_properties-0.7.0/test/test_application_properties_config_loader.py` & `application_properties-0.8.0/test/test_application_properties_config_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Tests for the ApplicationProperties class
 """
 import io
 import os
 import sys
-from test.test_helpers import ErrorResults, TestHelpers
+from test.pytest_helpers import ErrorResults, TestHelpers
 
 from application_properties import ApplicationProperties
 from application_properties.application_properties_config_loader import (
     ApplicationPropertiesConfigLoader,
 )
 
 
-def test_config_loader_config_not_present_check_enabled():
+def test_config_loader_config_not_present_check_enabled() -> None:
     """
     Test to make sure that we do not try and load a configuration file that is not present.
     """
 
     # Arrange
     configuration_file = "does-not-exist"
     configuration_file = os.path.abspath(configuration_file)
@@ -37,15 +37,15 @@
 
     # Assert
     assert expected_value == actual_value
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
 
 
-def test_config_loader_config_not_present_check_disabled():
+def test_config_loader_config_not_present_check_disabled() -> None:
     """
     Test to make sure that we do not try and load a configuration file that is not present.
     """
 
     # Arrange
     configuration_file = "does-not-exist"
     configuration_file = os.path.abspath(configuration_file)
@@ -66,15 +66,15 @@
 
     # Assert
     assert expected_value == actual_value
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
 
 
-def test_config_loader_valid_config():
+def test_config_loader_valid_config() -> None:
     """
     Test to make sure that we can load a valid config file.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
 md999.test_value = 2
@@ -109,15 +109,15 @@
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_valid_config_but_wrong_get_property_type():
+def test_config_loader_valid_config_but_wrong_get_property_type() -> None:
     """
     Test to make sure that we can load a valid config file, even if the property
     we are looking for is of the wrong type.  The load should succeed, even
     if the get fails.
     """
 
     # Arrange
@@ -152,15 +152,15 @@
         assert captured_exception is not None
         assert str(captured_exception) == expected_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_not_present_with_check():
+def test_config_loader_config_file_not_present_with_check() -> None:
     """
     Test to make sure that we cannot load a config file that is not there,
     and explicitly have something in place to check for that.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
@@ -181,15 +181,15 @@
     )
 
     # Assert
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
 
 
-def test_config_loader_config_file_not_present_without_check():
+def test_config_loader_config_file_not_present_without_check() -> None:
     """
     Test to make sure that we cannot load a config file that is not there,
     and explicitly do not have something in place to check for that.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
@@ -221,24 +221,24 @@
     finally:
         sys.stdout = old_stdout
         sys.stderr = old_stderr
 
     # Assert
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
-    assert std_output is not None
     assert (
         std_output.getvalue()
         == f"Specified configuration file '{configuration_file}' does not exist.\n"
     )
-    assert std_error is not None
     assert std_error.getvalue() == ""
 
 
-def test_config_loader_config_file_not_present_without_check_and_error_function():
+def test_config_loader_config_file_not_present_without_check_and_error_function() -> (
+    None
+):
     """
     Test to make sure that we cannot load a config file that is not there,
     and explicitly do not have something in place to check for that, but have
     all errors getting captured.
     """
 
     # Arrange
@@ -271,15 +271,15 @@
     assert results.reported_error is not None
     assert (
         results.reported_error
         == f"Specified configuration file '{configuration_file}' does not exist."
     )
 
 
-def test_config_loader_config_file_not_valid():
+def test_config_loader_config_file_not_valid() -> None:
     """
     Test to make sure that we error loading an invalid config file.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
 md999.test_value
@@ -306,26 +306,25 @@
                 application_properties, configuration_file, None, None, True, False
             )
         finally:
             sys.stdout = old_stdout
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
-        assert std_output is not None
         assert std_output.getvalue() is not None
         configuration_file2 = configuration_file.replace("\\", "\\\\")
         assert std_output.getvalue() == (
             f"Specified configuration file '{configuration_file}' is not a valid config file: Source contains parsing errors: '{configuration_file2}'\n\t[line  2]: 'md999.test_value\\n'.\n"
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_valid_with_no_section_header():
+def test_config_loader_config_file_valid_with_no_section_header() -> None:
     """
     Test to make sure that not having a section header implies that everything in the
     file is part of the configuration.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
@@ -357,15 +356,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_valid_with_one_word_section_header():
+def test_config_loader_config_file_valid_with_one_word_section_header() -> None:
     """
     Test to make sure that having a having a one word section header that is
     present in the config file allows for anything under that entry to be
     processed as configuration.
     """
 
     # Arrange
@@ -412,15 +411,15 @@
         assert expected_value == actual_value
         assert other_expected_value == other_actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_valid_with_one_word_bad_section_header():
+def test_config_loader_config_file_valid_with_one_word_bad_section_header() -> None:
     """
     Test to make sure that having a one word section header that is not
     present in the config file effectively does not contribute to the
     configuration.
     """
 
     # Arrange
@@ -459,15 +458,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_valid_with_multi_word_valid_section_header():
+def test_config_loader_config_file_valid_with_multi_word_valid_section_header() -> None:
     """
     Test to make sure that having a having a multi word section header that points to
     an existing section is recognized.
     """
 
     # Arrange
     section_header = "tools.mytool"
@@ -505,15 +504,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_bad_config_format_with_repeated_section():
+def test_config_loader_config_file_bad_config_format_with_repeated_section() -> None:
     """
     Test to make sure that a repeated section, in different forms, causes errors.
     """
 
     # Arrange
     section_header = "plugins.tools.bar"
     supplied_configuration = """[plugins.tools]
@@ -545,24 +544,27 @@
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
         configuration_file2 = configuration_file.replace("\\", "\\\\")
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Specified configuration file '{configuration_file}' is not a valid config file: While reading from '{configuration_file2}' [line  4]: section 'plugins.tools' already exists."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_bad_config_format_with_header_with_leading_period():
+def test_config_loader_config_file_bad_config_format_with_header_with_leading_period() -> (
+    None
+):
     """
     Test to make sure that a header that starts with a period is an error.
     """
 
     # Arrange
     section_header = "plugins.tools.bar"
     supplied_configuration = """[.plugins]
@@ -590,24 +592,27 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Configuration section name '.plugins' in file '{configuration_file}' is not a valid section name: Configuration section name must not start or end with the '.' character."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_bad_config_format_with_item_with_leading_period():
+def test_config_loader_config_file_bad_config_format_with_item_with_leading_period() -> (
+    None
+):
     """
     Test to make sure that an item that starts with a period is an error.
     """
 
     # Arrange
     section_header = None
     supplied_configuration = """[plugins]
@@ -635,24 +640,27 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Configuration item name '.tools.bar' in file '{configuration_file}' is not a valid section name: Configuration item name must not start or end with the '.' character."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_bad_config_format_with_double_items_through_different_paths():
+def test_config_loader_config_file_bad_config_format_with_double_items_through_different_paths() -> (
+    None
+):
     """
     Test to make sure that an item name that is doubled, but through different paths, is caught.
     """
 
     # Arrange
     section_header = None
     supplied_configuration = """[plugins]
@@ -683,24 +691,25 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Full configuration item name 'plugins.tools.bar' in file '{configuration_file}' occurs multiple times using different formats."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_config_loader_config_file_bad_config_format_with_no_item_value():
+def test_config_loader_config_file_bad_config_format_with_no_item_value() -> None:
     """
     Test to make sure that an item name that is followed by a separator, but not value, is handled.
     """
 
     # Arrange
     section_header = None
     supplied_configuration = """[plugins]
@@ -730,14 +739,15 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Full configuration item name 'plugins.tools.bar' in file '{configuration_file}' does not have a value assigned to it."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
```

### Comparing `application_properties-0.7.0/test/test_application_properties_facade.py` & `application_properties-0.8.0/test/test_application_properties_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 """
 Tests for the ApplicationPropertiesFacade class
 """
+from typing import Any, Dict, List
+
 from application_properties import ApplicationProperties, ApplicationPropertiesFacade
 
 
-def test_properties_facade_base_not_properties_object():
+def test_properties_facade_base_not_properties_object() -> None:
     """
     Test setting up a facade with properties object that is not a properties object.
     """
 
     # Arrange
 
     # Act
     raised_exception = None
     try:
-        ApplicationPropertiesFacade(1, 1)
+        ApplicationPropertiesFacade(1, 1)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "The base_properties of the facade must be an ApplicationProperties instance."
     ), "Expected message was not present in exception."
 
 
-def test_properties_facade_prefix_not_string():
+def test_properties_facade_prefix_not_string() -> None:
     """
     Test setting up a facade with a prefix that is not a string.
     """
 
     # Arrange
     config_map = {"property": "2"}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        ApplicationPropertiesFacade(application_properties, 1)
+        ApplicationPropertiesFacade(application_properties, 1)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception) == "The property_prefix argument must be a string."
     ), "Expected message was not present in exception."
 
 
-def test_properties_facade_prefix_not_terminated_with_separator():
+def test_properties_facade_prefix_not_terminated_with_separator() -> None:
     """
     Test setting up a facade with a prefix that is not terminated with the separator.
     """
 
     # Arrange
     config_map = {"property": "2"}
     application_properties = ApplicationProperties()
@@ -74,15 +76,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "The property_prefix argument must end with the separator character '.'."
     ), "Expected message was not present in exception."
 
 
-def test_properties_facade_get_with_found_value():
+def test_properties_facade_get_with_found_value() -> None:
     """
     Test fetching through a configuration facade for a property that is present.
     """
 
     # Arrange
     config_map = {"upper": {"property": 1.2}}
     application_properties = ApplicationProperties()
@@ -93,15 +95,15 @@
     # Act
     actual_value = facade.get_property("property", float)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_facade_get_boolean_with_found_value():
+def test_properties_facade_get_boolean_with_found_value() -> None:
     """
     Test fetching through a configuration facade for a boolean property that is present.
     """
 
     # Arrange
     config_map = {"upper": {"property": True}}
     application_properties = ApplicationProperties()
@@ -112,15 +114,15 @@
     # Act
     actual_value = facade.get_boolean_property("property")
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_facade_get_integer_with_found_value():
+def test_properties_facade_get_integer_with_found_value() -> None:
     """
     Test fetching through a configuration facade for an integer property that is present.
     """
 
     # Arrange
     config_map = {"upper": {"property": 2}}
     application_properties = ApplicationProperties()
@@ -131,15 +133,15 @@
     # Act
     actual_value = facade.get_integer_property("property")
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_facade_get_string_with_found_value():
+def test_properties_facade_get_string_with_found_value() -> None:
     """
     Test fetching through a configuration facade for a string property that is present.
     """
 
     # Arrange
     config_map = {"upper": {"property": "2"}}
     application_properties = ApplicationProperties()
@@ -150,15 +152,15 @@
     # Act
     actual_value = facade.get_string_property("property")
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_facade_get_property_names_with_one_value():
+def test_properties_facade_get_property_names_with_one_value() -> None:
     """
     Test fetching through a configuration facade the property names for a single property value.
     """
 
     # Arrange
     config_map = {"upper": {"property": "2"}}
     application_properties = ApplicationProperties()
@@ -171,42 +173,42 @@
 
     # Assert
     print(type(expected_value))
     print(type(actual_value))
     assert expected_value == actual_value
 
 
-def test_properties_facade_get_property_names_with_no_values():
+def test_properties_facade_get_property_names_with_no_values() -> None:
     """
     Test fetching through a configuration facade the property names without a single property value.
     """
 
     # Arrange
-    config_map = {"upper": {"property": "2"}}
+    config_map: Dict[str, Dict[str, Any]] = {"upper": {"property": "2"}}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
     facade = ApplicationPropertiesFacade(application_properties, "uppers.")
-    expected_value = []
+    expected_value: List[str] = []
 
     # Act
     actual_value = facade.property_names
 
     # Assert
     print(type(expected_value))
     print(type(actual_value))
     assert expected_value == actual_value
 
 
-def test_properties_facade_get_properties_under_at_top_level_partial():
+def test_properties_facade_get_properties_under_at_top_level_partial() -> None:
     """
     Test calling the `property_names_under` function specifying only part of the top level.
     """
 
     # Arrange
-    config_map = {
+    config_map: Dict[str, Dict[str, Any]] = {
         "upper": {
             "feature": {"enabled": True},
             "other_feature": {"enabled": False, "other": 1},
         }
     }
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
@@ -217,21 +219,21 @@
 
     # Assert
     assert len(found_names) == len(config_map["upper"]["other_feature"])
     assert "other_feature.enabled" in found_names
     assert "other_feature.other" in found_names
 
 
-def test_properties_facade_get_properties_under_at_top_level_none():
+def test_properties_facade_get_properties_under_at_top_level_none() -> None:
     """
     Test calling the `property_names_under` function specifying none of the top level.
     """
 
     # Arrange
-    config_map = {
+    config_map: Dict[str, Dict[str, Any]] = {
         "upper": {
             "feature": {"enabled": True},
             "other_feature": {"enabled": False, "other": 1},
         }
     }
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
@@ -241,21 +243,21 @@
     found_names = facade.property_names_under("missing_feature")
 
     # Assert
     assert not found_names
     assert "missing_feature" not in config_map["upper"]
 
 
-def test_properties_facade_get_properties_under_at_sub_level():
+def test_properties_facade_get_properties_under_at_sub_level() -> None:
     """
     Test calling the `property_names_under` function specifying none of the top level.
     """
 
     # Arrange
-    config_map = {
+    config_map: Dict[str, Dict[str, Dict[str, Any]]] = {
         "upper": {
             "new_top_level": {
                 "feature": {"enabled": True},
                 "other_feature": {"enabled": False, "other": 1},
             }
         }
     }
```

### Comparing `application_properties-0.7.0/test/test_application_properties_json_loader.py` & `application_properties-0.8.0/test/test_application_properties_json_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Tests for the ApplicationProperties class
 """
 import io
 import json
 import os
 import sys
-from test.test_helpers import TestHelpers
+from test.pytest_helpers import TestHelpers
+from typing import Any, List, Optional
 
 from application_properties import (
     ApplicationProperties,
     ApplicationPropertiesJsonLoader,
 )
 
 
-def test_json_loader_config_not_present():
+def test_json_loader_config_not_present() -> None:
     """
     Test to make sure that we do not try and load a configuration file that is not present.
     """
 
     # Arrange
     configuration_file = "does-not-exist"
     configuration_file = os.path.abspath(configuration_file)
@@ -38,15 +39,15 @@
 
     # Assert
     assert expected_value == actual_value
     assert expected_did_error == actual_did_error
     assert expected_did_apply == actual_did_apply
 
 
-def test_json_loader_valid_json():
+def test_json_loader_valid_json() -> None:
     """
     Test to make sure that we can load a valid Json file.
     """
 
     # Arrange
     supplied_configuration = {"plugins": {"md999": {"test_value": 2}}}
     expected_value = 2
@@ -76,15 +77,15 @@
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_valid_json_but_wrong_get_property_type():
+def test_json_loader_valid_json_but_wrong_get_property_type() -> None:
     """
     Test to make sure that we can load a valid Json file, even if the property
     we are looking for is of the wrong type.  The load should succeed, even
     if the get fails.
     """
 
     # Arrange
@@ -124,15 +125,17 @@
         assert captured_exception is not None
         assert str(captured_exception) == expected_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_valid_json_but_wrong_get_property_type_with_untyped_conversion():
+def test_json_loader_valid_json_but_wrong_get_property_type_with_untyped_conversion() -> (
+    None
+):
     """
     Test to make sure that we can load a valid Json file, even if the property
     we are looking for is of the wrong type.  The load should succeed, even
     if the get fails.  The get should still fail as JSON is a typed source.
     """
 
     # Arrange
@@ -172,27 +175,27 @@
         assert captured_exception is not None
         assert str(captured_exception) == expected_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_invalid_json():
+def test_json_loader_invalid_json() -> None:
     """
     Test to make sure that we cannot load an invalid Json file.
     """
 
     # Arrange
     supplied_configuration = "this is not a json file"
     expected_did_apply = False
     expected_did_error = True
 
-    handled_error_parameters = []
+    handled_error_parameters: List[Any] = []
 
-    def inner_func(formatted_error, this_exception):
+    def inner_func(formatted_error: str, this_exception: Optional[Exception]) -> None:
         handled_error_parameters.append(formatted_error)
         handled_error_parameters.append(this_exception)
 
     configuration_file = None
     try:
         configuration_file = TestHelpers.write_temporary_configuration(
             supplied_configuration
@@ -218,25 +221,25 @@
         )
         assert isinstance(handled_error_parameters[1], json.decoder.JSONDecodeError)
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_missing_file():
+def test_json_loader_missing_file() -> None:
     """
     Test to make sure that we fail to load a file that isn't there.
     """
 
     # Arrange
     expected_did_apply = False
     expected_did_error = True
-    handled_error_parameters = []
+    handled_error_parameters: List[Any] = []
 
-    def inner_func(formatted_error, this_exception):
+    def inner_func(formatted_error: str, this_exception: Optional[Exception]) -> None:
         handled_error_parameters.append(formatted_error)
         handled_error_parameters.append(this_exception)
 
     configuration_file = "missing_file_name.other"
     assert not os.path.exists(configuration_file)
     application_properties = ApplicationProperties()
 
@@ -254,27 +257,27 @@
     assert handled_error_parameters
     assert handled_error_parameters[0].startswith(
         "Specified configuration file 'missing_file_name.other' was not loaded: "
     )
     assert isinstance(handled_error_parameters[1], FileNotFoundError)
 
 
-def test_json_loader_valid_json_but_invalid_key():
+def test_json_loader_valid_json_but_invalid_key() -> None:
     """
     Test to make sure that we can load a valid Json file, but fail when there is an invalid key.
     """
 
     # Arrange
     supplied_configuration = {"plugins": {"md999": {"test.value": 2}}}
     expected_did_apply = False
     expected_did_error = True
 
-    handled_error_parameters = []
+    handled_error_parameters: List[Any] = []
 
-    def inner_func(formatted_error, this_exception):
+    def inner_func(formatted_error: str, this_exception: Optional[Exception]) -> None:
         handled_error_parameters.append(formatted_error)
         handled_error_parameters.append(this_exception)
 
     configuration_file = None
     try:
         configuration_file = TestHelpers.write_temporary_configuration(
             supplied_configuration
@@ -291,24 +294,24 @@
 
         # Assert
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
         assert handled_error_parameters
         assert handled_error_parameters[0].startswith("Specified configuration file '")
         assert (
-            "' is not valid: Keys strings cannot contain the separator character '.'."
+            "' is not valid: Key strings cannot contain a whitespace character, a '=' character, or a '.' character."
             in handled_error_parameters[0]
         )
         assert isinstance(handled_error_parameters[1], ValueError)
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_valid_json_but_invalid_key_with_stdin_capture():
+def test_json_loader_valid_json_but_invalid_key_with_stdin_capture() -> None:
     """
     Test to make sure that we can load a valid Json file, but fail when there is an invalid key.
     """
 
     # Arrange
     supplied_configuration = {"plugins": {"md999": {"test.value": 2}}}
     expected_did_apply = False
@@ -341,24 +344,24 @@
             sys.stderr = saved_stderr
 
         # Assert
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
         assert new_stdout.getvalue().startswith("Specified configuration file '")
         assert (
-            "' is not valid: Keys strings cannot contain the separator character '.'."
+            "' is not valid: Key strings cannot contain a whitespace character, a '=' character, or a '.' character."
             in new_stdout.getvalue()
         )
         assert not new_stderr.getvalue()
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_pair_valid_json():
+def test_json_loader_pair_valid_json() -> None:
     """
     Test to make sure that we can load more than one configuration file and not have
     the configurations stomp on each other in an unpredictable manner.
     """
 
     # Arrange
     supplied_configuration_first = {
```

### Comparing `application_properties-0.7.0/test/test_application_properties_toml_loader.py` & `application_properties-0.8.0/test/test_application_properties_toml_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Tests for the ApplicationProperties class
 """
 import io
 import os
 import sys
-from test.test_helpers import ErrorResults, TestHelpers
+from test.pytest_helpers import ErrorResults, TestHelpers
 
 from application_properties import ApplicationProperties
 from application_properties.application_properties_toml_loader import (
     ApplicationPropertiesTomlLoader,
 )
 
 
-def test_toml_loader_config_not_present():
+def test_toml_loader_config_not_present() -> None:
     """
     Test to make sure that we do not try and load a configuration file that is not present.
     """
 
     # Arrange
     configuration_file = "does-not-exist"
     configuration_file = os.path.abspath(configuration_file)
@@ -37,15 +37,15 @@
 
     # Assert
     assert expected_value == actual_value
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
 
 
-def test_toml_loader_valid_toml():
+def test_toml_loader_valid_toml() -> None:
     """
     Test to make sure that we can load a valid toml file.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
 md999.test_value = 2
@@ -77,15 +77,15 @@
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_valid_toml_but_wrong_get_property_type():
+def test_toml_loader_valid_toml_but_wrong_get_property_type() -> None:
     """
     Test to make sure that we can load a valid toml file, even if the property
     we are looking for is of the wrong type.  The load should succeed, even
     if the get fails.
     """
 
     # Arrange
@@ -120,15 +120,17 @@
         assert captured_exception is not None
         assert str(captured_exception) == expected_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_valid_toml_but_wrong_get_property_type_with_untyped_conversion():
+def test_toml_loader_valid_toml_but_wrong_get_property_type_with_untyped_conversion() -> (
+    None
+):
     """
     Test to make sure that we can load a valid toml file, even if the property
     we are looking for is of the wrong type.  The load should succeed, even
     if the get fails.  The get should still fail as TOML is a typed source.
     """
 
     # Arrange
@@ -164,15 +166,15 @@
         assert captured_exception is not None
         assert str(captured_exception) == expected_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_not_present_with_check():
+def test_toml_loader_toml_file_not_present_with_check() -> None:
     """
     Test to make sure that we cannot load a toml file that is not there,
     and explicitly have something in place to check for that.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
@@ -193,15 +195,15 @@
     )
 
     # Assert
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
 
 
-def test_toml_loader_toml_file_not_present_without_check():
+def test_toml_loader_toml_file_not_present_without_check() -> None:
     """
     Test to make sure that we cannot load a toml file that is not there,
     and explicitly do not have something in place to check for that.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
@@ -229,22 +231,21 @@
         )
     finally:
         sys.stdout = old_stdout
 
     # Assert
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
-    assert std_output is not None
     assert std_output.getvalue() is not None
     assert std_output.getvalue().startswith(
         f"Specified configuration file '{configuration_file}' was not loaded: "
     )
 
 
-def test_toml_loader_toml_file_not_present_without_check_and_error_function():
+def test_toml_loader_toml_file_not_present_without_check_and_error_function() -> None:
     """
     Test to make sure that we cannot load a toml file that is not there,
     and explicitly do not have something in place to check for that, but have
     all errors getting captured.
     """
 
     # Arrange
@@ -271,20 +272,20 @@
         False,
     )
 
     # Assert
     assert expected_did_apply == actual_did_apply
     assert expected_did_error == actual_did_error
     assert results.reported_error is not None
-    assert results.reported_error.startswith(
+    assert str(results.reported_error).startswith(
         f"Specified configuration file '{configuration_file}' was not loaded: "
     )
 
 
-def test_toml_loader_toml_file_not_valid():
+def test_toml_loader_toml_file_not_valid() -> None:
     """
     Test to make sure that we error loading an invalid toml file.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
 md999.test_value
@@ -311,25 +312,24 @@
                 application_properties, configuration_file, None, None, True, False
             )
         finally:
             sys.stdout = old_stdout
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
-        assert std_output is not None
         assert std_output.getvalue() is not None
         assert std_output.getvalue().startswith(
             f"Specified configuration file '{configuration_file}' is not a valid TOML file: Expected '=' after a key in a key/value pair (at line 2, column 17).\n"
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_valid_with_no_section_header():
+def test_toml_loader_toml_file_valid_with_no_section_header() -> None:
     """
     Test to make sure that not having a section header implies that everything in the
     file is part of the configuration.
     """
 
     # Arrange
     supplied_configuration = """[plugins]
@@ -361,15 +361,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_valid_with_one_word_section_header():
+def test_toml_loader_toml_file_valid_with_one_word_section_header() -> None:
     """
     Test to make sure that having a having a one word section header that is
     present in the TOML file allows for anything under that entry to be
     processed as configuration.
     """
 
     # Arrange
@@ -408,15 +408,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_valid_with_one_word_bad_section_header():
+def test_toml_loader_toml_file_valid_with_one_word_bad_section_header() -> None:
     """
     Test to make sure that having a one word section header that is not
     present in the TOML file effectively does not contribute to the
     configuration.
     """
 
     # Arrange
@@ -455,15 +455,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_valid_with_multi_word_valid_section_header():
+def test_toml_loader_toml_file_valid_with_multi_word_valid_section_header() -> None:
     """
     Test to make sure that having a having a multi word section header that points to
     an existing section is recognized.
     """
 
     # Arrange
     section_header = "tools.mytool"
@@ -501,15 +501,17 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_valid_with_multi_word_section_header_that_points_to_a_value():
+def test_toml_loader_toml_file_valid_with_multi_word_section_header_that_points_to_a_value() -> (
+    None
+):
     """
     Test to make sure that having a having a multi word section header that points
     to a specific value instead of a section does not get applied.
     """
 
     # Arrange
     section_header = "plugins.tools.bar"
@@ -547,15 +549,15 @@
         assert expected_did_error == actual_did_error
         assert expected_value == actual_value
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_bad_toml_format_with_repeated_section():
+def test_toml_loader_toml_file_bad_toml_format_with_repeated_section() -> None:
     """
     Test to make sure that a repeated section, in different forms, causes errors.
     """
 
     # Arrange
     section_header = "plugins.tools.bar"
     supplied_configuration = """[plugins]
@@ -586,24 +588,27 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Specified configuration file '{configuration_file}' is not a valid TOML file: Cannot declare ('plugins', 'tools') twice (at line 4, column 15)."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_bad_toml_format_with_header_with_leading_period():
+def test_toml_loader_toml_file_bad_toml_format_with_header_with_leading_period() -> (
+    None
+):
     """
     Test to make sure that a header that starts with a period is an error.
     """
 
     # Arrange
     section_header = "plugins.tools.bar"
     supplied_configuration = """[.plugins]
@@ -631,24 +636,25 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Specified configuration file '{configuration_file}' is not a valid TOML file: Invalid initial character for a key part (at line 1, column 2)."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_bad_toml_format_with_item_with_leading_period():
+def test_toml_loader_toml_file_bad_toml_format_with_item_with_leading_period() -> None:
     """
     Test to make sure that an item that starts with a period is an error.
     """
 
     # Arrange
     section_header = "plugins.tools.bar"
     supplied_configuration = """[plugins]
@@ -676,24 +682,27 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Specified configuration file '{configuration_file}' is not a valid TOML file: Invalid statement (at line 2, column 1)."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_toml_loader_toml_file_bad_toml_format_with_double_items_through_different_paths():
+def test_toml_loader_toml_file_bad_toml_format_with_double_items_through_different_paths() -> (
+    None
+):
     """
     Test to make sure that an item name that is doubled, but through different paths, is caught.
     """
 
     # Arrange
     section_header = None
     supplied_configuration = """[plugins]
@@ -724,14 +733,15 @@
             results.keep_error,
             True,
             False,
         )
 
         assert expected_did_apply == actual_did_apply
         assert expected_did_error == actual_did_error
+        assert results.reported_error is not None
         assert (
             results.reported_error
             == f"Specified configuration file '{configuration_file}' is not a valid TOML file: Cannot declare ('plugins', 'tools') twice (at line 4, column 15)."
         )
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
```

### Comparing `application_properties-0.7.0/test/test_get_boolean.py` & `application_properties-0.8.0/test/test_get_integer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 """
-Tests for the get_boolean* functions of the ApplicationProperties class
+Tests for the get_integer* functions of the ApplicationProperties class
 """
 from application_properties import ApplicationProperties
 
 
-def test_properties_get_boolean_with_found_value():
+def test_properties_get_integer_with_found_value() -> None:
     """
-    Test fetching a configuration value that is present and boolean.
+    Test fetching a configuration value that is present and integer.
     """
 
     # Arrange
-    config_map = {"property": True}
+    config_map = {"property": 1}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
-    expected_value = True
+    expected_value = 1
 
     # Act
-    actual_value = application_properties.get_boolean_property("property", False)
+    actual_value = application_properties.get_integer_property("property", -1)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_boolean_with_found_value_but_wrong_type():
+def test_properties_get_integer_with_found_value_but_wrong_type() -> None:
     """
-    Test fetching a configuration value that is present and not boolean.
+    Test fetching a configuration value that is present and not integer.
     """
 
     # Arrange
-    config_map = {"property": 1}
+    config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
-    expected_value = True
+    expected_value = -1
 
     # Act
-    actual_value = application_properties.get_boolean_property("property", True)
+    actual_value = application_properties.get_integer_property("property", -1)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_boolean_with_not_found_value():
+def test_properties_get_integer_with_not_found_value() -> None:
     """
-    Test fetching a configuration value that is not present and boolean.
+    Test fetching a configuration value that is not present and integer.
     """
 
     # Arrange
-    config_map = {"property": True}
+    config_map = {"property": 2}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
-    expected_value = True
+    expected_value = 3
 
     # Act
-    actual_value = application_properties.get_boolean_property("other_property", True)
+    actual_value = application_properties.get_integer_property("other_property", 3)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_boolean_with_not_found_value_and_no_default_value():
+def test_properties_get_integer_with_not_found_value_and_no_default_value() -> None:
     """
-    Test fetching a configuration value that is not present, with no default, and boolean.
+    Test fetching a configuration value that is not present, with no default, and integer.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
-    actual_value = application_properties.get_boolean_property("other_property")
+    actual_value = application_properties.get_integer_property("other_property")
 
     # Assert
     assert actual_value is None
 
 
-def test_properties_get_boolean_with_a_bad_property_name():
+def test_properties_get_integer_with_a_bad_property_name() -> None:
     """
     Test fetching a configuration value with a bad property name.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_boolean_property(1, 1)
+        application_properties.get_integer_property(1, 1)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception) == "The propertyName argument must be a string."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_boolean_with_a_bad_default():
+def test_properties_get_integer_with_a_bad_default() -> None:
     """
-    Test fetching a configuration value with a default value that is not a boolean.
+    Test fetching a configuration value with a default value that is not an integer.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_boolean_property("property", 1)
+        application_properties.get_integer_property("property", True)
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
-        == "The default value for property 'property' must either be None or a 'bool' value."
+        == "The default value for property 'property' must either be None or a 'int' value."
     ), "Expected message was not present in exception."
```

### Comparing `application_properties-0.7.0/test/test_get_integer.py` & `application_properties-0.8.0/test/test_get_boolean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 """
-Tests for the get_integer* functions of the ApplicationProperties class
+Tests for the get_boolean* functions of the ApplicationProperties class
 """
 from application_properties import ApplicationProperties
 
 
-def test_properties_get_integer_with_found_value():
+def test_properties_get_boolean_with_found_value() -> None:
     """
-    Test fetching a configuration value that is present and integer.
+    Test fetching a configuration value that is present and boolean.
     """
 
     # Arrange
-    config_map = {"property": 1}
+    config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
-    expected_value = 1
+    expected_value = True
 
     # Act
-    actual_value = application_properties.get_integer_property("property", -1)
+    actual_value = application_properties.get_boolean_property("property", False)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_integer_with_found_value_but_wrong_type():
+def test_properties_get_boolean_with_found_value_but_wrong_type() -> None:
     """
-    Test fetching a configuration value that is present and not integer.
+    Test fetching a configuration value that is present and not boolean.
     """
 
     # Arrange
-    config_map = {"property": True}
+    config_map = {"property": 1}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
-    expected_value = -1
+    expected_value = True
 
     # Act
-    actual_value = application_properties.get_integer_property("property", -1)
+    actual_value = application_properties.get_boolean_property("property", True)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_integer_with_not_found_value():
+def test_properties_get_boolean_with_not_found_value() -> None:
     """
-    Test fetching a configuration value that is not present and integer.
+    Test fetching a configuration value that is not present and boolean.
     """
 
     # Arrange
-    config_map = {"property": 2}
+    config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
-    expected_value = 3
+    expected_value = True
 
     # Act
-    actual_value = application_properties.get_integer_property("other_property", 3)
+    actual_value = application_properties.get_boolean_property("other_property", True)
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_integer_with_not_found_value_and_no_default_value():
+def test_properties_get_boolean_with_not_found_value_and_no_default_value() -> None:
     """
-    Test fetching a configuration value that is not present, with no default, and integer.
+    Test fetching a configuration value that is not present, with no default, and boolean.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
-    actual_value = application_properties.get_integer_property("other_property")
+    actual_value = application_properties.get_boolean_property("other_property")
 
     # Assert
     assert actual_value is None
 
 
-def test_properties_get_integer_with_a_bad_property_name():
+def test_properties_get_boolean_with_a_bad_property_name() -> None:
     """
     Test fetching a configuration value with a bad property name.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_integer_property(1, 1)
+        application_properties.get_boolean_property(1, 1)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception) == "The propertyName argument must be a string."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_integer_with_a_bad_default():
+def test_properties_get_boolean_with_a_bad_default() -> None:
     """
-    Test fetching a configuration value with a default value that is not an integer.
+    Test fetching a configuration value with a default value that is not a boolean.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_integer_property("property", True)
+        application_properties.get_boolean_property("property", 1)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
-        == "The default value for property 'property' must either be None or a 'int' value."
+        == "The default value for property 'property' must either be None or a 'bool' value."
     ), "Expected message was not present in exception."
```

### Comparing `application_properties-0.7.0/test/test_get_string.py` & `application_properties-0.8.0/test/test_get_string.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Tests for the get_string* functions of the ApplicationProperties class
 """
+from typing import Any
+
 from application_properties import ApplicationProperties
 
 
-def test_properties_get_string_with_found_value():
+def test_properties_get_string_with_found_value() -> None:
     """
     Test fetching a configuration value that is present and string.
     """
 
     # Arrange
     config_map = {"property": "me"}
     application_properties = ApplicationProperties()
@@ -18,15 +20,15 @@
     # Act
     actual_value = application_properties.get_string_property("property", "")
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_string_with_found_value_but_wrong_type():
+def test_properties_get_string_with_found_value_but_wrong_type() -> None:
     """
     Test fetching a configuration value that is present and not string.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
@@ -36,15 +38,15 @@
     # Act
     actual_value = application_properties.get_string_property("property", "")
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_string_with_not_found_value():
+def test_properties_get_string_with_not_found_value() -> None:
     """
     Test fetching a configuration value that is not present and string.
     """
 
     # Arrange
     config_map = {"property": "2"}
     application_properties = ApplicationProperties()
@@ -54,15 +56,15 @@
     # Act
     actual_value = application_properties.get_string_property("other_property", "3")
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_string_with_not_found_value_and_no_default_value():
+def test_properties_get_string_with_not_found_value_and_no_default_value() -> None:
     """
     Test fetching a configuration value that is not present, with no default, and integer.
     """
 
     # Arrange
     config_map = {"property": "2"}
     application_properties = ApplicationProperties()
@@ -71,15 +73,15 @@
     # Act
     actual_value = application_properties.get_string_property("other_property")
 
     # Assert
     assert actual_value is None
 
 
-def test_properties_get_string_with_found_value_validated():
+def test_properties_get_string_with_found_value_validated() -> None:
     """
     Test fetching a configuration value that is present and adheres to the validation function.
     """
 
     # Arrange
     config_map = {"property": "2"}
     application_properties = ApplicationProperties()
@@ -91,23 +93,23 @@
         "property", "-", lambda property_value: property_value in ["1", "2"]
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def __sample_string_validation_function(property_value):
+def __sample_string_validation_function(property_value: str) -> Any:
     """
     Simple string validation that throws an error if not "1" or "2".
     """
     if property_value not in ["1", "2"]:
-        raise ValueError(f"Value '{str(property_value)}' is not '1' or '2'")
+        raise ValueError(f"Value '{property_value}' is not '1' or '2'")
 
 
-def test_properties_get_string_with_found_value_not_validated():
+def test_properties_get_string_with_found_value_not_validated() -> None:
     """
     Test fetching a configuration value that is present and does not adhere to the validation function.
     """
 
     # Arrange
     config_map = {"property": "3"}
     application_properties = ApplicationProperties()
@@ -120,26 +122,26 @@
     )
 
     # Assert
     assert expected_value == actual_value
 
 
 # pylint: disable=broad-exception-raised
-def bad_validation_function(property_value):
+def bad_validation_function(property_value: str) -> Any:
     """
     Test validation function that always throws an exception.
     """
     # sourcery skip: raise-specific-error
-    raise Exception(f"huh? {str(property_value)}")
+    raise Exception(f"huh? {property_value}")
 
 
 # pylint: enable=broad-exception-raised
 
 
-def test_properties_get_string_with_found_value_validation_raises_error():
+def test_properties_get_string_with_found_value_validation_raises_error() -> None:
     """
     Test fetching a configuration value that is present and the validation function raises an error.
     """
 
     # Arrange
     config_map = {"property": "1"}
     application_properties = ApplicationProperties()
@@ -151,53 +153,53 @@
         "property", "-", bad_validation_function
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_get_string_with_a_bad_property_name():
+def test_properties_get_string_with_a_bad_property_name() -> None:
     """
     Test fetching a configuration value with a bad property name.
     """
 
     # Arrange
     config_map = {"property": True}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_string_property(1, "3")
+        application_properties.get_string_property(1, "3")  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception) == "The propertyName argument must be a string."
     ), "Expected message was not present in exception."
 
 
-def test_properties_get_string_with_a_bad_default():
+def test_properties_get_string_with_a_bad_default() -> None:
     """
     Test fetching a configuration value with a default value that is not a string.
     """
 
     # Arrange
     config_map = {"property": "2"}
     application_properties = ApplicationProperties()
     application_properties.load_from_dict(config_map)
 
     # Act
     raised_exception = None
     try:
-        application_properties.get_string_property("property", True)
+        application_properties.get_string_property("property", True)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
```

### Comparing `application_properties-0.7.0/test/test_set_manual_property.py` & `application_properties-0.8.0/test/test_set_manual_property.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """
 Tests for the set_manual_property related functions of the ApplicationProperties class
 """
+from typing import List
+
 from application_properties import ApplicationProperties
 
 
-def test_properties_set_manual_property_with_non_string():
+def test_properties_set_manual_property_with_non_string() -> None:
     """
     Test to make sure that a manual property with a non-string is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_string = 1
 
     # Act
     raised_exception = None
     try:
-        application_properties.set_manual_property(full_string)
+        application_properties.set_manual_property(full_string)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Manual property form must either be a string or an iterable of strings."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_no_equals():
+def test_properties_set_manual_property_with_no_equals() -> None:
     """
     Test to make sure that a full key with no value part is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_string = "a_property"
@@ -50,15 +52,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Manual property key and value must be separated by the '=' character."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_single_part_string():
+def test_properties_set_manual_property_with_single_part_string() -> None:
     """
     Test to make sure that a full key specifying an string without any format is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
@@ -69,15 +71,15 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.get_string_property(full_property_key)
     assert property_value == actual_value
 
 
-def test_properties_set_manual_property_shows_up_in_property_names():
+def test_properties_set_manual_property_shows_up_in_property_names() -> None:
     """
     Test to make sure that a full key specifying an string without any format shows
     up properly in the properrt names list.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
@@ -89,15 +91,15 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.property_names
     assert property_value == actual_value
 
 
-def test_properties_set_manual_property_with_only_format_indicator():
+def test_properties_set_manual_property_with_only_format_indicator() -> None:
     """
     Test to make sure that a full key specifying an string format but with no
     format character following is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
@@ -109,15 +111,15 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.get_string_property(full_property_key)
     assert property_value[1:] == actual_value
 
 
-def test_properties_set_manual_property_with_string_indicator():
+def test_properties_set_manual_property_with_string_indicator() -> None:
     """
     Test to make sure that a full key specifying an string is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
@@ -128,15 +130,15 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.get_string_property(full_property_key)
     assert property_value[2:] == actual_value
 
 
-def test_properties_set_manual_property_with_integer_indicator():
+def test_properties_set_manual_property_with_integer_indicator() -> None:
     """
     Test to make sure that a full key specifying an integer is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
@@ -147,15 +149,17 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.get_integer_property(full_property_key)
     assert property_value == actual_value
 
 
-def test_properties_set_manual_property_with_integer_indicator_and_bad_integer():
+def test_properties_set_manual_property_with_integer_indicator_and_bad_integer() -> (
+    None
+):
     """
     Test to make sure that a full key specifying a bad integer is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
@@ -175,15 +179,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Manual property value '$#123a' cannot be translated into an integer."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_boolean_indicator():
+def test_properties_set_manual_property_with_boolean_indicator() -> None:
     """
     Test to make sure that a full key specifying a True boolean is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
@@ -194,15 +198,15 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.get_boolean_property(full_property_key)
     assert property_value == actual_value
 
 
-def test_properties_set_manual_property_with_uncased_boolean_indicator():
+def test_properties_set_manual_property_with_uncased_boolean_indicator() -> None:
     """
     Test to make sure that a full key specifying a True boolean in lower case is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
@@ -213,34 +217,35 @@
     application_properties.set_manual_property(full_string)
 
     # Assert
     actual_value = application_properties.get_boolean_property(full_property_key)
     assert property_value == actual_value
 
 
-def test_properties_set_manual_property_with_multiples():
+def test_properties_set_manual_property_with_multiples() -> None:
     """
     Test to make sure that a list of full keys is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a"
     property_value = True
     full_string = f"{full_property_key}=$!{property_value}"
+    full_string_in_array: List[str] = [full_string]
 
     # Act
-    application_properties.set_manual_property([full_string])
+    application_properties.set_manual_property(full_string_in_array)  # type: ignore
 
     # Assert
     actual_value = application_properties.get_boolean_property(full_property_key)
     assert property_value == actual_value
 
 
-def test_properties_set_manual_property_with_bad_key_start():
+def test_properties_set_manual_property_with_bad_key_start() -> None:
     """
     Test to make sure that a full key starting with the key separator character is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = ".a"
@@ -260,15 +265,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Full property key must not start or end with the '.' character."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_bad_key_end():
+def test_properties_set_manual_property_with_bad_key_end() -> None:
     """
     Test to make sure that a full key ending with the key separator character is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a."
@@ -288,15 +293,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Full property key must not start or end with the '.' character."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_empty_key_middle():
+def test_properties_set_manual_property_with_empty_key_middle() -> None:
     """
     Test to make sure that an empty key part for the full key is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a..a"
@@ -316,15 +321,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Full property key cannot contain multiples of the . without any text between them."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_empty_key():
+def test_properties_set_manual_property_with_empty_key() -> None:
     """
     Test to make sure that a key with an empty key part is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = ""
@@ -344,15 +349,15 @@
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
         == "Each part of the property key must contain at least one character."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_with_whitespace_key():
+def test_properties_set_manual_property_with_whitespace_key() -> None:
     """
     Test to make sure that a key with whitespace is handled properly.
     """
 
     # Arrange
     application_properties = ApplicationProperties()
     full_property_key = "a a"
@@ -368,43 +373,45 @@
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception)
-        == "Each part of the property key must not contain a whitespace character or the '.' character."
+        == "Each part of the property key cannot contain a whitespace character, a '=' character, or a '.' character."
     ), "Expected message was not present in exception."
 
 
-def test_properties_verify_manual_property_form_with_non_string():
+def test_properties_verify_manual_property_form_with_non_string() -> None:
     """
     Test to make sure that if we try and test the verification form function
     with a non-string, it fails predictably.
     """
 
     # Arrange
     full_string = 1
 
     # Act
     raised_exception = None
     try:
-        ApplicationProperties.verify_manual_property_form(full_string)
+        ApplicationProperties.verify_manual_property_form(full_string)  # type: ignore
         raise AssertionError("Should have raised an exception by now.")
     except ValueError as this_exception:
         raised_exception = this_exception
 
     # Assert
     assert raised_exception, "Expected exception was not raised."
     assert (
         str(raised_exception) == "Manual property form must be a string."
     ), "Expected message was not present in exception."
 
 
-def test_properties_set_manual_property_bool_wrong_type_convert_disabled_strict_enabled():
+def test_properties_set_manual_property_bool_wrong_type_convert_disabled_strict_enabled() -> (
+    None
+):
     """
     Test to make sure that asking for a boolean with only a string present, strict
     mode on and covert mode off results in an exception.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -427,15 +434,17 @@
         caught_exception = this_exception
 
     # Assert
     assert caught_exception is not None
     assert str(caught_exception) == expected_error
 
 
-def test_properties_set_manual_property_bool_wrong_type_convert_disabled_strict_disabled():
+def test_properties_set_manual_property_bool_wrong_type_convert_disabled_strict_disabled() -> (
+    None
+):
     """
     Test to make sure that asking for a boolean with only a string present, strict
     mode off and covert mode off results in an exception.  As strict mode is off, the
     default value takes precedence over reporting an error.
     """
 
     # Arrange
@@ -454,15 +463,17 @@
         full_property_key, default_value=False
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_enabled_with_valid():
+def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_enabled_with_valid() -> (
+    None
+):
     """
     Test to make sure that asking for a boolean with only a string present, strict
     mode on and covert mode on with a valid string that can be translated into a boolean.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -480,15 +491,17 @@
         full_property_key, default_value=False
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_enabled_with_invalid():
+def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_enabled_with_invalid() -> (
+    None
+):
     """
     Test to make sure that asking for a boolean with only a string present, strict
     mode on and covert mode off with an invalid (i.e. non-"true") boolean value. This happens
     because any string that is not "true" (case insensitive) is assumed to be False. As such,
     strict mode is never triggered as it always has a valid value.
     """
 
@@ -508,15 +521,17 @@
         full_property_key, default_value=False
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_disabled_with_valid():
+def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_disabled_with_valid() -> (
+    None
+):
     """
     Test to make sure that asking for a boolean with only a string present, strict
     mode off and covert mode on with a valid string that can be translated into a boolean.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -534,15 +549,17 @@
         full_property_key, default_value=False
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_disabled_with_invalid():
+def test_properties_set_manual_property_bool_wrong_type_convert_enabled_strict_disabled_with_invalid() -> (
+    None
+):
     """
     Test to make sure that asking for a boolean with only a string present, strict
     mode off and covert mode off with an invalid (i.e. non-"true") boolean value. This happens
     because any string that is not "true" (case insensitive) is assumed to be False. As such,
     strict mode is never triggered as it always has a valid value.
     """
 
@@ -562,15 +579,17 @@
         full_property_key, default_value=False
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_integer_wrong_type_convert_disabled_strict_enabled():
+def test_properties_set_manual_property_integer_wrong_type_convert_disabled_strict_enabled() -> (
+    None
+):
     """
     Test to make sure that asking for a integer with only a string present, strict
     mode on and covert mode off results in an exception.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -591,15 +610,17 @@
         caught_exception = this_exception
 
     # Assert
     assert caught_exception is not None
     assert str(caught_exception) == expected_error
 
 
-def test_properties_set_manual_property_integer_wrong_type_convert_disabled_strict_disabled():
+def test_properties_set_manual_property_integer_wrong_type_convert_disabled_strict_disabled() -> (
+    None
+):
     """
     Test to make sure that asking for a integer with only a string present, strict
     mode off and covert mode off results in an exception.  As strict mode is off, the
     default value takes precedence over reporting an error.
     """
 
     # Arrange
@@ -618,15 +639,17 @@
         full_property_key, default_value=-1
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_enabled_with_valid():
+def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_enabled_with_valid() -> (
+    None
+):
     """
     Test to make sure that asking for a integer with only a string present, strict
     mode on and covert mode on with a valid string that can be translated into an integer.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -644,15 +667,17 @@
         full_property_key, default_value=-1
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_enabled_with_invalid():
+def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_enabled_with_invalid() -> (
+    None
+):
     """
     Test to make sure that asking for a integer with only a string present, strict
     mode on and covert mode off with an invalid integer value.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -673,15 +698,17 @@
         caught_exception = this_exception
 
     # Assert
     assert caught_exception is not None
     assert str(caught_exception) == expected_error
 
 
-def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_disabled_with_valid():
+def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_disabled_with_valid() -> (
+    None
+):
     """
     Test to make sure that asking for a integer with only a string present, strict
     mode off and covert mode on with a valid string that can be translated into a integer.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
@@ -699,15 +726,17 @@
         full_property_key, default_value=-1
     )
 
     # Assert
     assert expected_value == actual_value
 
 
-def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_disabled_with_invalid():
+def test_properties_set_manual_property_integer_wrong_type_convert_enabled_strict_disabled_with_invalid() -> (
+    None
+):
     """
     Test to make sure that asking for a integer with only a string present, strict
     mode off and covert mode off with an invalid integer value.
     """
 
     # Arrange
     application_properties = ApplicationProperties(
```

