# Comparing `tmp/qtgql-0.129.0.tar.gz` & `tmp/qtgql-0.129.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.129.0.tar", max compression
+gzip compressed data, was "qtgql-0.129.1.tar", max compression
```

## Comparing `qtgql-0.129.0.tar` & `qtgql-0.129.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-07-16 14:43:36.502313 qtgql-0.129.0/LICENSE
--rw-r--r--   0        0        0     1055 2023-07-16 14:43:36.502313 qtgql-0.129.0/README.md
--rw-r--r--   0        0        0     4428 2023-07-16 14:43:56.890223 qtgql-0.129.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1939 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1685 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3302 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3877 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    16149 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0     4458 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/selections_injection.py
--rw-r--r--   0        0        0      864 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0     2195 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/utils.py
--rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4600 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3629 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2985 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1060 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4706 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4137 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5052 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5221 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18386 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1570 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.129.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-16 16:34:43.351374 qtgql-0.129.1/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-16 16:34:43.351374 qtgql-0.129.1/README.md
+-rw-r--r--   0        0        0     4428 2023-07-16 16:35:06.689226 qtgql-0.129.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1939 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1685 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3302 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16149 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4458 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2195 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4600 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3629 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2985 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1060 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4791 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4137 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5052 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5221 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18386 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1570 2023-07-16 16:34:43.363374 qtgql-0.129.1/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.129.1/PKG-INFO
```

### Comparing `qtgql-0.129.0/LICENSE` & `qtgql-0.129.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/README.md` & `qtgql-0.129.1/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/pyproject.toml` & `qtgql-0.129.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.129.0"
+version = "0.129.1"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.129.0/qtgqlcodegen/cli.py` & `qtgql-0.129.1/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/config.py` & `qtgql-0.129.1/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.129.1/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.129.1/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/core/template.py` & `qtgql-0.129.1/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/generator.py` & `qtgql-0.129.1/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.129.1/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.129.1/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/operation/selections_injection.py` & `qtgql-0.129.1/qtgqlcodegen/operation/selections_injection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/operation/template.py` & `qtgql-0.129.1/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/operation/utils.py` & `qtgql-0.129.1/qtgqlcodegen/operation/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.129.1/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.129.1/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/schema/template.py` & `qtgql-0.129.1/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,17 @@
 {% elif proxy_field.type.is_queried_interface or proxy_field.type.is_queried_union %}
 auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toObject();
 auto 👉f_concrete.name👈_typename  = 👉f_concrete.name👈_data.value("__typename").toString();
 {%set type_cond -%}👉f_concrete.name👈_typename{% endset -%}
 {% for choice in proxy_field.type.choices %}
 {% set do_on_meets -%}
 {% if choice.implements_node %}
-if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
-👉choice.updater_name👈(std::static_pointer_cast<👉choice.concrete.name👈>(👉current👈), 👉f_concrete.name👈_data,  👉operation_pointer👈);
+auto 👉f_concrete.name👈_casted = std::static_pointer_cast<👉choice.concrete.name👈>(👉current👈);
+if (👉current👈 && 👉f_concrete.name👈_casted->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
+👉choice.updater_name👈(👉f_concrete.name👈_casted, 👉f_concrete.name👈_data,  👉operation_pointer👈);
 }
 else{
 👉 setter_name 👈(👉choice.deserializer_name👈(👉proxy_field.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
 }
 {% else %}
 👉choice.updater_name👈(std::static_pointer_cast<👉choice.concrete.name👈>(👉current👈), 👉f_concrete.name👈_data,  👉operation_pointer👈);
 {% endif %}
```

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.129.1/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.129.1/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.129.1/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/types.py` & `qtgql-0.129.1/qtgqlcodegen/types.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/qtgqlcodegen/utils.py` & `qtgql-0.129.1/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.129.0/PKG-INFO` & `qtgql-0.129.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.129.0
+Version: 0.129.1
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

