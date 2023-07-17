# Comparing `tmp/mizdb-tomselect-0.4.0.tar.gz` & `tmp/mizdb-tomselect-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb-tomselect-0.4.0.tar", last modified: Tue Jul 11 07:58:35 2023, max compression
+gzip compressed data, was "mizdb-tomselect-0.5.0.tar", last modified: Mon Jul 17 09:26:54 2023, max compression
```

## Comparing `mizdb-tomselect-0.4.0.tar` & `mizdb-tomselect-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.865120 mizdb-tomselect-0.4.0/
--rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.4.0/LICENSE
--rw-r--r--   0 philip    (1000) philip    (1000)    11359 2023-07-11 07:58:35.865120 mizdb-tomselect-0.4.0/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)    10957 2023-07-11 06:57:55.000000 mizdb-tomselect-0.4.0/README.md
--rw-r--r--   0 philip    (1000) philip    (1000)     1601 2023-07-11 07:57:19.000000 mizdb-tomselect-0.4.0/pyproject.toml
--rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-07-11 07:58:35.865120 mizdb-tomselect-0.4.0/setup.cfg
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.860120 mizdb-tomselect-0.4.0/src/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.862120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/
--rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/__init__.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.863120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/css/
--rw-r--r--   0 philip    (1000) philip    (1000)      647 2023-07-11 07:06:00.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.863120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/js/
--rw-r--r--   0 philip    (1000) philip    (1000)   148177 2023-07-11 07:58:33.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.864120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/
--rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-r--r--   0 philip    (1000) philip    (1000)     4366 2023-07-04 08:10:45.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     6645 2023-07-04 09:47:30.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/widgets.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.863120 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/
--rw-r--r--   0 philip    (1000) philip    (1000)    11359 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)      654 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/SOURCES.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/dependency_links.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/requires.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/top_level.txt
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.864120 mizdb-tomselect-0.4.0/tests/
--rw-r--r--   0 philip    (1000) philip    (1000)    16516 2023-07-11 06:57:55.000000 mizdb-tomselect-0.4.0/tests/test_views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     5647 2023-07-11 06:57:55.000000 mizdb-tomselect-0.4.0/tests/test_widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.650929 mizdb-tomselect-0.5.0/
+-rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.5.0/LICENSE
+-rw-r--r--   0 philip    (1000) philip    (1000)    12851 2023-07-17 09:26:54.650929 mizdb-tomselect-0.5.0/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)    12449 2023-07-17 07:25:25.000000 mizdb-tomselect-0.5.0/README.md
+-rw-r--r--   0 philip    (1000) philip    (1000)     1601 2023-07-17 09:26:34.000000 mizdb-tomselect-0.5.0/pyproject.toml
+-rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-07-17 09:26:54.650929 mizdb-tomselect-0.5.0/setup.cfg
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.594928 mizdb-tomselect-0.5.0/src/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.596928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/
+-rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/__init__.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.595928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.595928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.597928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)      647 2023-07-14 08:07:53.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.598928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/js/
+-rw-r--r--   0 philip    (1000) philip    (1000)   148094 2023-07-17 09:26:51.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.595928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.595928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/tom-select/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.598928 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/tom-select/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-r--r--   0 philip    (1000) philip    (1000)     4366 2023-07-04 08:10:45.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     7567 2023-07-16 09:40:03.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect/widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.597928 mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/
+-rw-r--r--   0 philip    (1000) philip    (1000)    12851 2023-07-17 09:26:54.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)      654 2023-07-17 09:26:54.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/SOURCES.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-17 09:26:54.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/dependency_links.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-07-17 09:26:54.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/requires.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-07-17 09:26:54.000000 mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/top_level.txt
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-17 09:26:54.649929 mizdb-tomselect-0.5.0/tests/
+-rw-r--r--   0 philip    (1000) philip    (1000)    16516 2023-07-11 06:57:55.000000 mizdb-tomselect-0.5.0/tests/test_views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     9433 2023-07-14 08:57:42.000000 mizdb-tomselect-0.5.0/tests/test_widgets.py
```

### Comparing `mizdb-tomselect-0.4.0/LICENSE` & `mizdb-tomselect-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.4.0/PKG-INFO` & `mizdb-tomselect-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.4.0
+Version: 0.5.0
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TomSelect for Django (MIZDB)
 
 Django autocomplete widgets and views using [TomSelect](https://tom-select.js.org/).
 
+![Example of the MIZSelect widget](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/mizselect.png "MIZSelect preview")
+
 Note that this was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
+
 <!-- TOC -->
 * [TomSelect for Django (MIZDB)](#tomselect-for-django-mizdb)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
+      * [Adding more columns](#adding-more-columns)
+    * [MIZSelectMultiple & MIZSelectTabularMultiple](#mizselectmultiple--mizselecttabularmultiple)
   * [Function & Features](#function--features)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
     * [Inline edit link](#inline-edit-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
+
 ----
 
 ## Installation
 
 Install:
 ```bash
 pip install -U mizdb-tomselect
@@ -133,54 +139,78 @@
 |----------------|----------------------------------------|------------------------------------------------------------------------------------------------|
 | model          | **required**                           | the model class that provides the choices                                                      |
 | url            | `"autocomplete"`                       | URL pattern name of the autocomplete view                                                      |
 | value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
 | label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
 | search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
 | create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False                                  | if True, allow selecting multiple options                                                      |
 | changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
 | add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
 | edit_url       |                                        | URL name of the edit view for this model([see below](#inline-edit-link))                       |
 | filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
-
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
-![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
+![Tabular select preview](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/tabular_default.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
 | Argument           | Default value                   | Description                         |
 |--------------------|---------------------------------|-------------------------------------|
 | extra_columns      |                                 | a mapping for additional columns    |
 | value_field_label  | `f"{value_field.title()}"`      | table header for the value column   |
 | label_field_label  | `f"{model._meta.verbose_name}"` | table header for the label column   |
 
-#### Adding more columns 
+#### Adding more columns
 
 To add more columns, pass a `result attribute name: column label` mapping to the widget
-argument `extra_columns`.
+argument `extra_columns`. For example: 
+```python
+# models.py
+class Person(models.Model):
+    name = models.CharField(max_length=100, blank=True)
+    dob = models.DateField(blank=True, null=True)
+    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
 
-The column label is the table header label for a given column.  
 
-The attribute name tells TomSelect what value to look up on a result for the column.
+# forms.py 
+class TabularForm(forms.Form):
+    person = forms.ModelChoiceField(
+            Person.objects.all(),
+            widget=MIZSelectTabular(
+                Person,
+                extra_columns={"dob": "Date of Birth", "city__name": "City"},
+                label_field_label="Name",
+            ),
+            required=False,
+        )
+```
+
+The column label is the table header label for a given column (here: `Date of Birth` and `City`).  
+
+The attribute name tells TomSelect what value to look up on a result for the column (here: model field `dob` and lookup expression `city__name` on the relation field `city`).
+
+![Tabular select with more columns](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/tabular.png "Tabular select with more columns")
 
 **Important**: that means that the result visible to TomSelect must have an attribute
 or property with that name or the column will remain empty. 
 The results for TomSelect are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
+### MIZSelectMultiple & MIZSelectTabularMultiple
+
+Variants of the above widgets that allow selecting multiple options.
+
 ----
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
@@ -258,52 +288,57 @@
     path('city/edit/<path:object_id>/', CityChangeView.as_view(), name='city_change'),
 ]
 
 # forms.py
 widget = MIZSelect(City, edit_url='city_change')
 ```
 
+![Preview of the edit button](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/edit2.png "Edit button preview")
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
+
 ```python
 # models.py
 class Person(models.Model):
     name = models.CharField(max_length=50)
-    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
+    pob = models.ForeignKey("Place of Birth", on_delete=models.SET_NULL, blank=True, null=True)
     
 class City(models.Model):
     name = models.CharField(max_length=50)
-    is_capitol = models.BooleanField(default=False)
 
 # forms.py
-class PersonsFromCapitolsForm(forms.Form):
-    capitol = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
+class PersonCityForm(forms.Form):
+    city = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
     person = forms.ModelChoiceField(
         queryset=Person.objects.all(),
         widget=MIZSelect(
             Person,
-            filter_by=("capitol", "city_id")
+            filter_by=("city", "pob_id")
         )
     )
 ```
 This will result in the Person result queryset to be filtered against 
-`city_id` with the current value of the `capitol` formfield.  
+`pob_id` with the current value of the `city` formfield.
+
+![Example for the filter_by argument](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/filterby.png "Filtering example")
+
 NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
 ----
 
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
 
-Then see the demo for a preview: `python demo/manage.py runserver`
+See the demo for a preview: run `make init-demo` and then start the demo server `python demo/manage.py runserver`.
 
 Run tests with `make test` or `make tox`. To install required browsers for playwright: `playwright install`.
 See the makefile for other commands.
```

### Comparing `mizdb-tomselect-0.4.0/README.md` & `mizdb-tomselect-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # TomSelect for Django (MIZDB)
 
 Django autocomplete widgets and views using [TomSelect](https://tom-select.js.org/).
 
+![Example of the MIZSelect widget](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/mizselect.png "MIZSelect preview")
+
 Note that this was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
+
 <!-- TOC -->
 * [TomSelect for Django (MIZDB)](#tomselect-for-django-mizdb)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
+      * [Adding more columns](#adding-more-columns)
+    * [MIZSelectMultiple & MIZSelectTabularMultiple](#mizselectmultiple--mizselecttabularmultiple)
   * [Function & Features](#function--features)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
     * [Inline edit link](#inline-edit-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
+
 ----
 
 ## Installation
 
 Install:
 ```bash
 pip install -U mizdb-tomselect
@@ -121,54 +127,78 @@
 |----------------|----------------------------------------|------------------------------------------------------------------------------------------------|
 | model          | **required**                           | the model class that provides the choices                                                      |
 | url            | `"autocomplete"`                       | URL pattern name of the autocomplete view                                                      |
 | value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
 | label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
 | search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
 | create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False                                  | if True, allow selecting multiple options                                                      |
 | changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
 | add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
 | edit_url       |                                        | URL name of the edit view for this model([see below](#inline-edit-link))                       |
 | filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
-
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
-![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
+![Tabular select preview](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/tabular_default.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
 | Argument           | Default value                   | Description                         |
 |--------------------|---------------------------------|-------------------------------------|
 | extra_columns      |                                 | a mapping for additional columns    |
 | value_field_label  | `f"{value_field.title()}"`      | table header for the value column   |
 | label_field_label  | `f"{model._meta.verbose_name}"` | table header for the label column   |
 
-#### Adding more columns 
+#### Adding more columns
 
 To add more columns, pass a `result attribute name: column label` mapping to the widget
-argument `extra_columns`.
+argument `extra_columns`. For example: 
+```python
+# models.py
+class Person(models.Model):
+    name = models.CharField(max_length=100, blank=True)
+    dob = models.DateField(blank=True, null=True)
+    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
 
-The column label is the table header label for a given column.  
 
-The attribute name tells TomSelect what value to look up on a result for the column.
+# forms.py 
+class TabularForm(forms.Form):
+    person = forms.ModelChoiceField(
+            Person.objects.all(),
+            widget=MIZSelectTabular(
+                Person,
+                extra_columns={"dob": "Date of Birth", "city__name": "City"},
+                label_field_label="Name",
+            ),
+            required=False,
+        )
+```
+
+The column label is the table header label for a given column (here: `Date of Birth` and `City`).  
+
+The attribute name tells TomSelect what value to look up on a result for the column (here: model field `dob` and lookup expression `city__name` on the relation field `city`).
+
+![Tabular select with more columns](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/tabular.png "Tabular select with more columns")
 
 **Important**: that means that the result visible to TomSelect must have an attribute
 or property with that name or the column will remain empty. 
 The results for TomSelect are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
+### MIZSelectMultiple & MIZSelectTabularMultiple
+
+Variants of the above widgets that allow selecting multiple options.
+
 ----
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
@@ -246,52 +276,57 @@
     path('city/edit/<path:object_id>/', CityChangeView.as_view(), name='city_change'),
 ]
 
 # forms.py
 widget = MIZSelect(City, edit_url='city_change')
 ```
 
+![Preview of the edit button](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/edit2.png "Edit button preview")
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
+
 ```python
 # models.py
 class Person(models.Model):
     name = models.CharField(max_length=50)
-    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
+    pob = models.ForeignKey("Place of Birth", on_delete=models.SET_NULL, blank=True, null=True)
     
 class City(models.Model):
     name = models.CharField(max_length=50)
-    is_capitol = models.BooleanField(default=False)
 
 # forms.py
-class PersonsFromCapitolsForm(forms.Form):
-    capitol = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
+class PersonCityForm(forms.Form):
+    city = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
     person = forms.ModelChoiceField(
         queryset=Person.objects.all(),
         widget=MIZSelect(
             Person,
-            filter_by=("capitol", "city_id")
+            filter_by=("city", "pob_id")
         )
     )
 ```
 This will result in the Person result queryset to be filtered against 
-`city_id` with the current value of the `capitol` formfield.  
+`pob_id` with the current value of the `city` formfield.
+
+![Example for the filter_by argument](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/filterby.png "Filtering example")
+
 NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
 ----
 
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
 
-Then see the demo for a preview: `python demo/manage.py runserver`
+See the demo for a preview: run `make init-demo` and then start the demo server `python demo/manage.py runserver`.
 
 Run tests with `make test` or `make tox`. To install required browsers for playwright: `playwright install`.
 See the makefile for other commands.
```

### Comparing `mizdb-tomselect-0.4.0/pyproject.toml` & `mizdb-tomselect-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mizdb-tomselect"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using TomSelect"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4314,22 +4314,18 @@
             return;
         const html = `<a class="${options.className}" title="${options.title}" target="_blank">${options.label}</a>`;
         this.hook("after", "setupTemplates", () => {
             const orig = this.settings.render.item;
             this.settings.render.item = (data, escape) => {
                 const item = getDom2(orig.call(this, data, escape));
                 const editButton = getDom2(html);
+                editButton.href = options.getEditUrl(options, item, data[this.settings.valueField]);
                 editButton.addEventListener("click", (e) => {
                     e.stopPropagation();
                 });
-                this.on("item_add", (value, _item) => {
-                    if (item === _item) {
-                        editButton.href = options.getEditUrl(options, item, value);
-                    }
-                });
                 item.appendChild(editButton);
                 return item;
             };
         });
     }
 
     // client/mizselect.js
```

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect/views.py` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect/views.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect/widgets.py` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect/widgets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import json
 from urllib.parse import unquote
 
 from django import forms
 from django.urls import reverse
 
 
@@ -17,15 +18,14 @@
         self,
         model,
         url="autocomplete",
         value_field="",
         label_field="",
         search_lookup="",
         create_field="",
-        multiple=False,
         changelist_url="",
         add_url="",
         edit_url="",
         filter_by=(),
         **kwargs,
     ):
         """
@@ -42,15 +42,14 @@
               human-readable value of an option (f.ex. 'name'). Defaults to the
               value of the model's `name_field` attribute. If the model has no
               `name_field` attribute, it defaults to 'name'.
             search_lookup: a Django field lookup to use with the given search
               term to filter the results
             create_field: the name of the model field used to create new
               model objects with
-            multiple: if True, allow selecting multiple options
             changelist_url: URL name of the 'changelist' view for this model
             add_url: URL name of the 'add' view for this model
             edit_url: URL name of the 'change' view for this model
             filter_by: a 2-tuple (form_field_name, field_lookup) to filter the
               results against the value of the form field using the given
               Django field lookup. For example:
                ('foo', 'bar__id') => results.filter(bar__id=data['foo'])
@@ -58,23 +57,30 @@
         """
         self.model = model
         self.url = url
         self.value_field = value_field or self.model._meta.pk.name
         self.label_field = label_field or getattr(self.model, "name_field", "name")
         self.search_lookup = search_lookup or f"{self.label_field}__icontains"
         self.create_field = create_field
-        self.multiple = multiple
         self.changelist_url = changelist_url
         self.add_url = add_url
         self.edit_url = edit_url
         self.filter_by = filter_by
         super().__init__(**kwargs)
 
     def optgroups(self, name, value, attrs=None):
-        return []  # Never provide any options; let the view serve the options.
+        """Only query for selected model objects."""
+        # inspired by dal.widgets.WidgetMixin from django-autocomplete-light
+        selected_choices = [str(c) for c in value if c]
+        all_choices = copy.copy(self.choices)
+        # TODO: empty values in selected_choices will be filtered out twice
+        self.choices.queryset = self.choices.queryset.filter(pk__in=[c for c in selected_choices if c])
+        results = super().optgroups(name, value, attrs)
+        self.choices = all_choices
+        return results
 
     def get_url(self):
         """Hook to specify the autocomplete URL."""
         return reverse(self.url)
 
     def get_add_url(self):
         """Hook to specify the URL to the model's 'add' page."""
@@ -94,15 +100,14 @@
     def build_attrs(self, base_attrs, extra_attrs=None):
         """Build HTML attributes for the widget."""
         attrs = super().build_attrs(base_attrs, extra_attrs)
         opts = self.model._meta
         attrs.update(
             {
                 "is-tomselect": True,
-                "is-multiple": self.multiple,
                 "data-autocomplete-url": self.get_url(),
                 "data-model": f"{opts.app_label}.{opts.model_name}",
                 "data-search-lookup": self.search_lookup,
                 "data-value-field": self.value_field,
                 "data-label-field": self.label_field,
                 "data-create-field": self.create_field,
                 "data-changelist-url": self.get_changelist_url() or "",
@@ -153,7 +158,25 @@
                 "data-value-field-label": self.value_field_label,
                 "data-label-field-label": self.label_field_label,
                 "data-extra-headers": json.dumps(list(self.extra_columns.values())),
                 "data-extra-columns": json.dumps(list(self.extra_columns.keys())),
             }
         )
         return attrs
+
+
+class MultipleSelectionMixin:
+    """Enable multiple selection with TomSelect."""
+
+    def build_attrs(self, base_attrs, extra_attrs=None):
+        """Build HTML attributes for the widget."""
+        attrs = super().build_attrs(base_attrs, extra_attrs)  # noqa
+        attrs["is-multiple"] = True
+        return attrs
+
+
+class MIZSelectMultiple(MultipleSelectionMixin, MIZSelect, forms.SelectMultiple):
+    """A MIZSelect widget that allows multiple selection."""
+
+
+class MIZSelectTabularMultiple(MultipleSelectionMixin, MIZSelectTabular, forms.SelectMultiple):
+    """A MIZSelectTabular widget that allows multiple selection."""
```

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/PKG-INFO` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.4.0
+Version: 0.5.0
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TomSelect for Django (MIZDB)
 
 Django autocomplete widgets and views using [TomSelect](https://tom-select.js.org/).
 
+![Example of the MIZSelect widget](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/mizselect.png "MIZSelect preview")
+
 Note that this was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
+
 <!-- TOC -->
 * [TomSelect for Django (MIZDB)](#tomselect-for-django-mizdb)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
+      * [Adding more columns](#adding-more-columns)
+    * [MIZSelectMultiple & MIZSelectTabularMultiple](#mizselectmultiple--mizselecttabularmultiple)
   * [Function & Features](#function--features)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
     * [Inline edit link](#inline-edit-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
+
 ----
 
 ## Installation
 
 Install:
 ```bash
 pip install -U mizdb-tomselect
@@ -133,54 +139,78 @@
 |----------------|----------------------------------------|------------------------------------------------------------------------------------------------|
 | model          | **required**                           | the model class that provides the choices                                                      |
 | url            | `"autocomplete"`                       | URL pattern name of the autocomplete view                                                      |
 | value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
 | label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
 | search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
 | create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False                                  | if True, allow selecting multiple options                                                      |
 | changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
 | add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
 | edit_url       |                                        | URL name of the edit view for this model([see below](#inline-edit-link))                       |
 | filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
-
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
-![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
+![Tabular select preview](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/tabular_default.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
 | Argument           | Default value                   | Description                         |
 |--------------------|---------------------------------|-------------------------------------|
 | extra_columns      |                                 | a mapping for additional columns    |
 | value_field_label  | `f"{value_field.title()}"`      | table header for the value column   |
 | label_field_label  | `f"{model._meta.verbose_name}"` | table header for the label column   |
 
-#### Adding more columns 
+#### Adding more columns
 
 To add more columns, pass a `result attribute name: column label` mapping to the widget
-argument `extra_columns`.
+argument `extra_columns`. For example: 
+```python
+# models.py
+class Person(models.Model):
+    name = models.CharField(max_length=100, blank=True)
+    dob = models.DateField(blank=True, null=True)
+    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
 
-The column label is the table header label for a given column.  
 
-The attribute name tells TomSelect what value to look up on a result for the column.
+# forms.py 
+class TabularForm(forms.Form):
+    person = forms.ModelChoiceField(
+            Person.objects.all(),
+            widget=MIZSelectTabular(
+                Person,
+                extra_columns={"dob": "Date of Birth", "city__name": "City"},
+                label_field_label="Name",
+            ),
+            required=False,
+        )
+```
+
+The column label is the table header label for a given column (here: `Date of Birth` and `City`).  
+
+The attribute name tells TomSelect what value to look up on a result for the column (here: model field `dob` and lookup expression `city__name` on the relation field `city`).
+
+![Tabular select with more columns](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/tabular.png "Tabular select with more columns")
 
 **Important**: that means that the result visible to TomSelect must have an attribute
 or property with that name or the column will remain empty. 
 The results for TomSelect are created by the view calling `values()` on the 
 result queryset, so you must make sure that the attribute name is available
 on the view's root queryset as either a model field or as an annotation.
 
+### MIZSelectMultiple & MIZSelectTabularMultiple
+
+Variants of the above widgets that allow selecting multiple options.
+
 ----
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
@@ -258,52 +288,57 @@
     path('city/edit/<path:object_id>/', CityChangeView.as_view(), name='city_change'),
 ]
 
 # forms.py
 widget = MIZSelect(City, edit_url='city_change')
 ```
 
+![Preview of the edit button](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/edit2.png "Edit button preview")
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
+
 ```python
 # models.py
 class Person(models.Model):
     name = models.CharField(max_length=50)
-    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
+    pob = models.ForeignKey("Place of Birth", on_delete=models.SET_NULL, blank=True, null=True)
     
 class City(models.Model):
     name = models.CharField(max_length=50)
-    is_capitol = models.BooleanField(default=False)
 
 # forms.py
-class PersonsFromCapitolsForm(forms.Form):
-    capitol = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
+class PersonCityForm(forms.Form):
+    city = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
     person = forms.ModelChoiceField(
         queryset=Person.objects.all(),
         widget=MIZSelect(
             Person,
-            filter_by=("capitol", "city_id")
+            filter_by=("city", "pob_id")
         )
     )
 ```
 This will result in the Person result queryset to be filtered against 
-`city_id` with the current value of the `capitol` formfield.  
+`pob_id` with the current value of the `city` formfield.
+
+![Example for the filter_by argument](https://raw.githubusercontent.com/Actionb/mizdb-tomselect/main/demo/images/filterby.png "Filtering example")
+
 NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
 ----
 
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 make init
 ```
 
-Then see the demo for a preview: `python demo/manage.py runserver`
+See the demo for a preview: run `make init-demo` and then start the demo server `python demo/manage.py runserver`.
 
 Run tests with `make test` or `make tox`. To install required browsers for playwright: `playwright install`.
 See the makefile for other commands.
```

### Comparing `mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/SOURCES.txt` & `mizdb-tomselect-0.5.0/src/mizdb_tomselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.4.0/tests/test_views.py` & `mizdb-tomselect-0.5.0/tests/test_views.py`

 * *Files identical despite different names*

