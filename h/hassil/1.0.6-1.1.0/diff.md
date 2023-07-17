# Comparing `tmp/hassil-1.0.6.tar.gz` & `tmp/hassil-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassil-1.0.6.tar", last modified: Mon Feb 27 23:30:36 2023, max compression
+gzip compressed data, was "hassil-1.1.0.tar", last modified: Mon Jul 17 19:55:25 2023, max compression
```

## Comparing `hassil-1.0.6.tar` & `hassil-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-02-27 23:30:36.084252 hassil-1.0.6/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.0.6/HassILGrammar.g4
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.0.6/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.0.6/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4199 2023-02-27 23:30:36.084252 hassil-1.0.6/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3460 2023-02-01 04:31:35.000000 hassil-1.0.6/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-02-27 23:30:36.080252 hassil-1.0.6/hassil/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-02-22 19:10:08.000000 hassil-1.0.6/hassil/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.0.6/hassil/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.0.6/hassil/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.0.6/hassil/_resources.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2279 2023-02-10 20:55:51.000000 hassil-1.0.6/hassil/expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     9609 2023-02-23 16:53:06.000000 hassil-1.0.6/hassil/intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5388 2023-02-10 20:53:50.000000 hassil-1.0.6/hassil/parse_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7763 2023-02-01 04:31:35.000000 hassil-1.0.6/hassil/parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.0.6/hassil/py.typed
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    22976 2023-02-27 23:29:10.000000 hassil-1.0.6/hassil/recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.0.6/hassil/sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.0.6/hassil/sample_template.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.0.6/hassil/util.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-02-27 23:30:36.080252 hassil-1.0.6/hassil.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4199 2023-02-27 23:30:36.000000 hassil-1.0.6/hassil.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-02-27 23:30:36.000000 hassil-1.0.6/hassil.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-02-27 23:30:36.000000 hassil-1.0.6/hassil.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-02-27 23:30:36.000000 hassil-1.0.6/hassil.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-02-27 23:30:36.000000 hassil-1.0.6/hassil.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-02-27 23:30:36.000000 hassil-1.0.6/hassil.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.0.6/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-02-22 19:10:25.000000 hassil-1.0.6/requirements_dev.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-02-27 23:30:36.084252 hassil-1.0.6/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.0.6/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-02-27 23:30:36.084252 hassil-1.0.6/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.0.6/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2812 2023-02-01 04:31:35.000000 hassil-1.0.6/tests/test_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4469 2023-02-06 16:37:52.000000 hassil-1.0.6/tests/test_intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.0.6/tests/test_parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12466 2023-02-16 18:12:38.000000 hassil-1.0.6/tests/test_recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.0.6/tests/test_sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.0.6/tests/test_util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.1.0/HassILGrammar.g4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.1.0/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.1.0/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4389 2023-07-17 19:55:25.475653 hassil-1.1.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3650 2023-05-25 21:44:27.000000 hassil-1.1.0/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/hassil/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-17 19:54:35.000000 hassil-1.1.0/hassil/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.1.0/hassil/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.1.0/hassil/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.1.0/hassil/_resources.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2279 2023-02-10 20:55:51.000000 hassil-1.1.0/hassil/expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10085 2023-06-15 16:06:29.000000 hassil-1.1.0/hassil/intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5388 2023-02-10 20:53:50.000000 hassil-1.1.0/hassil/parse_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7763 2023-02-01 04:31:35.000000 hassil-1.1.0/hassil/parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.1.0/hassil/py.typed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23303 2023-06-15 16:06:29.000000 hassil-1.1.0/hassil/recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.1.0/hassil/sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.1.0/hassil/sample_template.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.1.0/hassil/util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/hassil.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4389 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.1.0/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.1.0/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-17 19:55:25.479653 hassil-1.1.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.1.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.1.0/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2812 2023-02-01 04:31:35.000000 hassil-1.1.0/tests/test_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4469 2023-02-06 16:37:52.000000 hassil-1.1.0/tests/test_intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.1.0/tests/test_parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13434 2023-06-15 16:06:29.000000 hassil-1.1.0/tests/test_recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.1.0/tests/test_sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.1.0/tests/test_util.py
```

### Comparing `hassil-1.0.6/HassILGrammar.g4` & `hassil-1.1.0/HassILGrammar.g4`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/LICENSE.md` & `hassil-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/PKG-INFO` & `hassil-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.0.6
+Version: 1.1.0
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
@@ -21,17 +21,15 @@
 # HassIL
 
 The Home Assistant Intent Language (HassIL) parser for [intents](https://github.com/home-assistant/intents).
 
 
 ## Dependencies
 
-* antlr4-python3-runtime
 * PyYAML
-* dataclasses-json
 
 
 ## Installation
 
 Run the `script/setup` script to automatically create a virtual environment and install the requirements.
 
 
@@ -92,15 +90,15 @@
   * `light[s]`
 * Slot Lists
   * `{list_name}`
   * `{list_name:slot_name}`
   * Refers to a pre-defined list of values in YAML (`lists`)
 * Expansion Rules
   * `<rule_name>`
-  * Refers to a pre-defined expansion rule in YAML (`expansion_rules`)
+  * Refers to a pre-defined expansion rule in YAML (`expansion_rules`), either global or local (particular to the intent to which the sentence refers)
 
 
 ## YAML Format
 
 ``` yaml
 language: "<language code>"
 intents:
@@ -116,14 +114,17 @@
           <name>: <value>
         requires_context:
           # Must be present in match context
           <name>: # Any provided value is good
         excludes_context:
           # Must NOT be present in match context
           <name>: <value or list>
+        expansion_rules:
+          # Expansion rules which only apply to the intent, referenced as <rule_name>
+          <rule_name>: <sentence template>
 
 # Optional lists of items that become alternatives in sentence templates
 lists:
   # Referenced as {list_name} or {list_name:slot_name}
   <list name>:
     values:
       - "items"
```

### Comparing `hassil-1.0.6/README.md` & `hassil-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # HassIL
 
 The Home Assistant Intent Language (HassIL) parser for [intents](https://github.com/home-assistant/intents).
 
 
 ## Dependencies
 
-* antlr4-python3-runtime
 * PyYAML
-* dataclasses-json
 
 
 ## Installation
 
 Run the `script/setup` script to automatically create a virtual environment and install the requirements.
 
 
@@ -72,15 +70,15 @@
   * `light[s]`
 * Slot Lists
   * `{list_name}`
   * `{list_name:slot_name}`
   * Refers to a pre-defined list of values in YAML (`lists`)
 * Expansion Rules
   * `<rule_name>`
-  * Refers to a pre-defined expansion rule in YAML (`expansion_rules`)
+  * Refers to a pre-defined expansion rule in YAML (`expansion_rules`), either global or local (particular to the intent to which the sentence refers)
 
 
 ## YAML Format
 
 ``` yaml
 language: "<language code>"
 intents:
@@ -96,14 +94,17 @@
           <name>: <value>
         requires_context:
           # Must be present in match context
           <name>: # Any provided value is good
         excludes_context:
           # Must NOT be present in match context
           <name>: <value or list>
+        expansion_rules:
+          # Expansion rules which only apply to the intent, referenced as <rule_name>
+          <rule_name>: <sentence template>
 
 # Optional lists of items that become alternatives in sentence templates
 lists:
   # Referenced as {list_name} or {list_name:slot_name}
   <list name>:
     values:
       - "items"
```

### Comparing `hassil-1.0.6/hassil/__main__.py` & `hassil-1.1.0/hassil/__main__.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil/expression.py` & `hassil-1.1.0/hassil/expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil/intents.py` & `hassil-1.1.0/hassil/intents.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
     requires_context: Dict[str, Any] = field(default_factory=dict)
     """Context items required before match is successful."""
 
     excludes_context: Dict[str, Any] = field(default_factory=dict)
     """Context items that must not be present for match to be successful."""
 
+    expansion_rules: Dict[str, Sentence] = field(default_factory=dict)
+    """Local expansion rules in the context of a single intent."""
+
     @cached_property
     def sentences(self) -> List[Sentence]:
         """Sentence templates that match this intent."""
         return [parse_sentence(text, keep_text=True) for text in self.sentence_texts]
 
 
 @dataclass
@@ -232,14 +235,20 @@
                     name=intent_name,
                     data=[
                         IntentData(
                             sentence_texts=data_dict["sentences"],
                             slots=data_dict.get("slots", {}),
                             requires_context=data_dict.get("requires_context", {}),
                             excludes_context=data_dict.get("excludes_context", {}),
+                            expansion_rules={
+                                rule_name: parse_sentence(rule_body, keep_text=True)
+                                for rule_name, rule_body in data_dict.get(
+                                    "expansion_rules", {}
+                                ).items()
+                            },
                             response=data_dict.get("response"),
                         )
                         for data_dict in intent_dict["data"]
                     ],
                 )
                 for intent_name, intent_dict in input_dict["intents"].items()
             },
```

### Comparing `hassil-1.0.6/hassil/parse_expression.py` & `hassil-1.1.0/hassil/parse_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil/parser.py` & `hassil-1.1.0/hassil/parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil/recognize.py` & `hassil-1.1.0/hassil/recognize.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,23 +241,32 @@
                         elif actual_value == excluded_value:
                             skip_data = True
                             break
 
                 if skip_data:
                     continue
 
+            local_settings = MatchSettings(
+                slot_lists=settings.slot_lists,
+                expansion_rules={
+                    **settings.expansion_rules,
+                    **intent_data.expansion_rules,
+                },
+                ignore_whitespace=settings.ignore_whitespace,
+            )
+
             # Check each sentence template
             for intent_sentence in intent_data.sentences:
                 # Create initial context
                 match_context = MatchContext(
                     text=text,
                     intent_context=intent_context,
                 )
                 maybe_match_contexts = match_expression(
-                    settings, match_context, intent_sentence
+                    local_settings, match_context, intent_sentence
                 )
                 for maybe_match_context in maybe_match_contexts:
                     if not maybe_match_context.is_match:
                         # Incomplete match with text still left at the end
                         continue
 
                     skip_match = False
```

### Comparing `hassil-1.0.6/hassil/sample.py` & `hassil-1.1.0/hassil/sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil/sample_template.py` & `hassil-1.1.0/hassil/sample_template.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil/util.py` & `hassil-1.1.0/hassil/util.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/hassil.egg-info/PKG-INFO` & `hassil-1.1.0/hassil.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.0.6
+Version: 1.1.0
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
@@ -21,17 +21,15 @@
 # HassIL
 
 The Home Assistant Intent Language (HassIL) parser for [intents](https://github.com/home-assistant/intents).
 
 
 ## Dependencies
 
-* antlr4-python3-runtime
 * PyYAML
-* dataclasses-json
 
 
 ## Installation
 
 Run the `script/setup` script to automatically create a virtual environment and install the requirements.
 
 
@@ -92,15 +90,15 @@
   * `light[s]`
 * Slot Lists
   * `{list_name}`
   * `{list_name:slot_name}`
   * Refers to a pre-defined list of values in YAML (`lists`)
 * Expansion Rules
   * `<rule_name>`
-  * Refers to a pre-defined expansion rule in YAML (`expansion_rules`)
+  * Refers to a pre-defined expansion rule in YAML (`expansion_rules`), either global or local (particular to the intent to which the sentence refers)
 
 
 ## YAML Format
 
 ``` yaml
 language: "<language code>"
 intents:
@@ -116,14 +114,17 @@
           <name>: <value>
         requires_context:
           # Must be present in match context
           <name>: # Any provided value is good
         excludes_context:
           # Must NOT be present in match context
           <name>: <value or list>
+        expansion_rules:
+          # Expansion rules which only apply to the intent, referenced as <rule_name>
+          <rule_name>: <sentence template>
 
 # Optional lists of items that become alternatives in sentence templates
 lists:
   # Referenced as {list_name} or {list_name:slot_name}
   <list name>:
     values:
       - "items"
```

### Comparing `hassil-1.0.6/hassil.egg-info/SOURCES.txt` & `hassil-1.1.0/hassil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/setup.py` & `hassil-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/tests/test_expression.py` & `hassil-1.1.0/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/tests/test_intents.py` & `hassil-1.1.0/tests/test_intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/tests/test_parser.py` & `hassil-1.1.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/tests/test_recognize.py` & `hassil-1.1.0/tests/test_recognize.py`

 * *Files 3% similar despite different names*

```diff
@@ -474,7 +474,42 @@
     """
 
     with io.StringIO(yaml_text) as test_file:
         intents = Intents.from_yaml(test_file)
 
     result = recognize("abcd", intents)
     assert result is not None
+
+
+def test_local_expansion_rules() -> None:
+    """Test local expansion rules, defined at the intent level"""
+    yaml_text = """
+    language: "en"
+    intents:
+      GetSmokeState:
+        data:
+          - expansion_rules:
+              verb: "(are|is)"
+              subject: "[all] [the] light[s]"
+              state: "on"
+              location: "[in <area>]"
+            sentences:
+              - "<verb> <subject> <state> <location>"
+              - "<verb> <subject> <location> <state>"
+    expansion_rules:
+      area: "[the] {area}"
+    lists:
+      area:
+        values:
+          - kitchen
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    for sentence in (
+        "are the lights on in the kitchen",
+        "are the lights in the kitchen on",
+    ):
+        result = recognize(sentence, intents)
+        assert result is not None, sentence
+        assert result.intent.name == "GetSmokeState"
```

### Comparing `hassil-1.0.6/tests/test_sample.py` & `hassil-1.1.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.0.6/tests/test_util.py` & `hassil-1.1.0/tests/test_util.py`

 * *Files identical despite different names*

