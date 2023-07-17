# Comparing `tmp/dataclasses-json-0.5.8.tar.gz` & `tmp/dataclasses-json-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses-json-0.5.8.tar", last modified: Sun Jun 11 18:43:06 2023, max compression
+gzip compressed data, was "dataclasses-json-0.5.9.tar", last modified: Fri Jun 30 20:11:49 2023, max compression
```

## Comparing `dataclasses-json-0.5.8.tar` & `dataclasses-json-0.5.9.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.793468 dataclasses-json-0.5.8/
--rw-r--r--   0 charlie    (501) staff       (20)     1084 2019-06-16 15:23:27.000000 dataclasses-json-0.5.8/LICENSE
--rw-r--r--   0 charlie    (501) staff       (20)       16 2021-08-26 01:55:32.000000 dataclasses-json-0.5.8/MANIFEST.in
--rw-r--r--   0 charlie    (501) staff       (20)    27356 2023-06-11 18:43:06.793309 dataclasses-json-0.5.8/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)    21727 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/README.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.788593 dataclasses-json-0.5.8/dataclasses_json/
--rw-r--r--   0 charlie    (501) staff       (20)      441 2022-03-21 14:47:36.000000 dataclasses-json-0.5.8/dataclasses_json/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     5113 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/dataclasses_json/api.py
--rw-r--r--   0 charlie    (501) staff       (20)     3365 2022-03-21 14:47:36.000000 dataclasses-json-0.5.8/dataclasses_json/cfg.py
--rw-r--r--   0 charlie    (501) staff       (20)    14748 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/dataclasses_json/core.py
--rw-r--r--   0 charlie    (501) staff       (20)    13904 2021-08-26 01:55:32.000000 dataclasses-json-0.5.8/dataclasses_json/mm.py
--rw-r--r--   0 charlie    (501) staff       (20)        0 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/dataclasses_json/py.typed
--rw-r--r--   0 charlie    (501) staff       (20)     3307 2021-08-26 02:01:26.000000 dataclasses-json-0.5.8/dataclasses_json/stringcase.py
--rw-r--r--   0 charlie    (501) staff       (20)    10110 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/dataclasses_json/undefined.py
--rw-r--r--   0 charlie    (501) staff       (20)     5464 2022-08-14 20:35:15.000000 dataclasses-json-0.5.8/dataclasses_json/utils.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.789352 dataclasses-json-0.5.8/dataclasses_json.egg-info/
--rw-r--r--   0 charlie    (501) staff       (20)    27356 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)      931 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/SOURCES.txt
--rw-r--r--   0 charlie    (501) staff       (20)        1 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/dependency_links.txt
--rw-r--r--   0 charlie    (501) staff       (20)      246 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/requires.txt
--rw-r--r--   0 charlie    (501) staff       (20)       17 2023-06-11 18:43:06.000000 dataclasses-json-0.5.8/dataclasses_json.egg-info/top_level.txt
--rw-r--r--   0 charlie    (501) staff       (20)      645 2023-06-11 02:35:27.000000 dataclasses-json-0.5.8/publish.py
--rw-r--r--   0 charlie    (501) staff       (20)       46 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/pyproject.toml
--rw-r--r--   0 charlie    (501) staff       (20)       38 2023-06-11 18:43:06.793519 dataclasses-json-0.5.8/setup.cfg
--rw-r--r--   0 charlie    (501) staff       (20)     1159 2023-06-11 18:38:05.000000 dataclasses-json-0.5.8/setup.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-06-11 18:43:06.792880 dataclasses-json-0.5.8/tests/
--rw-r--r--   0 charlie    (501) staff       (20)     3960 2023-03-18 13:15:21.000000 dataclasses-json-0.5.8/tests/test_annotations.py
--rw-r--r--   0 charlie    (501) staff       (20)     9918 2022-03-21 14:47:44.000000 dataclasses-json-0.5.8/tests/test_api.py
--rw-r--r--   0 charlie    (501) staff       (20)     9681 2022-08-14 20:35:15.000000 dataclasses-json-0.5.8/tests/test_collections.py
--rw-r--r--   0 charlie    (501) staff       (20)     2989 2020-02-23 14:06:56.000000 dataclasses-json-0.5.8/tests/test_dict.py
--rw-r--r--   0 charlie    (501) staff       (20)     6420 2023-06-11 01:41:14.000000 dataclasses-json-0.5.8/tests/test_enum.py
--rw-r--r--   0 charlie    (501) staff       (20)     1448 2019-07-08 15:52:19.000000 dataclasses-json-0.5.8/tests/test_examples.py
--rw-r--r--   0 charlie    (501) staff       (20)     1451 2020-05-29 19:49:41.000000 dataclasses-json-0.5.8/tests/test_exclude.py
--rw-r--r--   0 charlie    (501) staff       (20)      896 2020-02-23 14:12:41.000000 dataclasses-json-0.5.8/tests/test_global_config.py
--rw-r--r--   0 charlie    (501) staff       (20)     1241 2019-08-12 00:04:35.000000 dataclasses-json-0.5.8/tests/test_invariants.py
--rw-r--r--   0 charlie    (501) staff       (20)     3081 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/tests/test_letter_case.py
--rw-r--r--   0 charlie    (501) staff       (20)     1141 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/tests/test_metadata.py
--rw-r--r--   0 charlie    (501) staff       (20)     1207 2021-06-05 01:16:21.000000 dataclasses-json-0.5.8/tests/test_nested.py
--rw-r--r--   0 charlie    (501) staff       (20)     1744 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/tests/test_recursive.py
--rw-r--r--   0 charlie    (501) staff       (20)     1618 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/tests/test_schema.py
--rw-r--r--   0 charlie    (501) staff       (20)     3790 2020-04-21 23:35:26.000000 dataclasses-json-0.5.8/tests/test_time.py
--rw-r--r--   0 charlie    (501) staff       (20)    12269 2021-06-03 10:39:20.000000 dataclasses-json-0.5.8/tests/test_undefined_parameters.py
--rw-r--r--   0 charlie    (501) staff       (20)     3904 2020-02-23 14:06:06.000000 dataclasses-json-0.5.8/tests/test_union.py
--rw-r--r--   0 charlie    (501) staff       (20)     1414 2022-08-14 20:35:15.000000 dataclasses-json-0.5.8/tests/test_unsupported_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:49.686619 dataclasses-json-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-06-30 20:11:49.686619 dataclasses-json-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21727 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:49.686619 dataclasses-json-0.5.9/dataclasses_json/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/mm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/stringcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/dataclasses_json/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:49.686619 dataclasses-json-0.5.9/dataclasses_json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-06-30 20:11:49.000000 dataclasses-json-0.5.9/dataclasses_json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-30 20:11:49.000000 dataclasses-json-0.5.9/dataclasses_json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:11:49.000000 dataclasses-json-0.5.9/dataclasses_json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 20:11:49.000000 dataclasses-json-0.5.9/dataclasses_json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 20:11:49.000000 dataclasses-json-0.5.9/dataclasses_json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:11:49.686619 dataclasses-json-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:49.686619 dataclasses-json-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_global_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_letter_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_str_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_undefined_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-30 20:11:40.000000 dataclasses-json-0.5.9/tests/test_unsupported_generics.py
```

### Comparing `dataclasses-json-0.5.8/LICENSE` & `dataclasses-json-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/PKG-INFO` & `dataclasses-json-0.5.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,670 +1,670 @@
 Metadata-Version: 2.1
 Name: dataclasses-json
-Version: 0.5.8
+Version: 0.5.9
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/lidatong/dataclasses-json
 Author: lidatong
 Author-email: charles.dt.li@gmail.com
 License: MIT
-Description: # Dataclasses JSON
-        
-        ![](https://github.com/lidatong/dataclasses-json/workflows/dataclasses-json/badge.svg)
-        
-        This library provides a simple API for encoding and decoding [dataclasses](https://docs.python.org/3/library/dataclasses.html) to and from JSON.
-        
-        It's very easy to get started.
-        
-        [README / Documentation website](https://lidatong.github.io/dataclasses-json). Features a navigation bar and search functionality, and should mirror this README exactly -- take a look!
-        
-        ## Quickstart
-        
-        `pip install dataclasses-json`
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        
-        
-        person = Person(name='lidatong')
-        person.to_json()  # '{"name": "lidatong"}' <- this is a string
-        person.to_dict()  # {'name': 'lidatong'} <- this is a dict
-        Person.from_json('{"name": "lidatong"}')  # Person(1)
-        Person.from_dict({'name': 'lidatong'})  # Person(1)
-        
-        # You can also apply _schema validation_ using an alternative API
-        # This can be useful for "typed" Python code
-        
-        Person.from_json('{"name": 42}')  # This is ok. 42 is not a `str`, but
-                                          # dataclass creation does not validate types
-        Person.schema().loads('{"name": 42}')  # Error! Raises `ValidationError`
-        ```
-        
-        **What if you want to work with camelCase JSON?**
-        
-        ```python
-        # same imports as above, with the additional `LetterCase` import
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json, LetterCase
-        
-        @dataclass_json(letter_case=LetterCase.CAMEL)  # now all fields are encoded/decoded from camelCase
-        @dataclass
-        class ConfiguredSimpleExample:
-            int_field: int
-        
-        ConfiguredSimpleExample(1).to_json()  # {"intField": 1}
-        ConfiguredSimpleExample.from_json('{"intField": 1}')  # ConfiguredSimpleExample(1)
-        ```
-        
-        ## Supported types
-        
-        It's recursive (see caveats below), so you can easily work with nested dataclasses.
-        In addition to the supported types in the 
-        [py to JSON table](https://docs.python.org/3/library/json.html#py-to-json-table), this library supports the following:
-        
-        - any arbitrary [Collection](https://docs.python.org/3/library/collections.abc.html#collections.abc.Collection) type is supported.
-        [Mapping](https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping) types are encoded as JSON objects and `str` types as JSON strings. 
-        Any other Collection types are encoded into JSON arrays, but decoded into the original collection types.
-        
-        - [datetime](https://docs.python.org/3/library/datetime.html#available-types) 
-        objects. `datetime` objects are encoded to `float` (JSON number) using 
-        [timestamp](https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp).
-        As specified in the `datetime` docs, if your `datetime` object is naive, it will 
-        assume your system local timezone when calling `.timestamp()`. JSON numbers 
-        corresponding to a `datetime` field in your dataclass are decoded 
-        into a datetime-aware object, with `tzinfo` set to your system local timezone.
-        Thus, if you encode a datetime-naive object, you will decode into a 
-        datetime-aware object. This is important, because encoding and decoding won't 
-        strictly be inverses. See [this section](#Overriding) if you want to override this default
-        behavior (for example, if you want to use ISO).
-        
-        - [UUID](https://docs.python.org/3/library/uuid.html#uuid.UUID) objects. They 
-        are encoded as `str` (JSON string).
-        
-        - [Decimal](https://docs.python.org/3/library/decimal.html) objects. They are
-        also encoded as `str`.
-        
-        **The [latest release](https://github.com/lidatong/dataclasses-json/releases/latest) is compatible with both Python 3.7 and Python 3.6 (with the dataclasses backport).**
-        
-        ## Usage
-        
-        #### Approach 1: Class decorator
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        
-        lidatong = Person('lidatong')
-        
-        # Encoding to JSON
-        lidatong.to_json()  # '{"name": "lidatong"}'
-        
-        # Decoding from JSON
-        Person.from_json('{"name": "lidatong"}')  # Person(name='lidatong')
-        ```
-        
-        Note that the `@dataclass_json` decorator must be stacked above the `@dataclass`
-        decorator (order matters!)
-        
-        #### Approach 2: Inherit from a mixin
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import DataClassJsonMixin
-        
-        @dataclass
-        class Person(DataClassJsonMixin):
-            name: str
-        
-        lidatong = Person('lidatong')
-        
-        # A different example from Approach 1 above, but usage is the exact same
-        assert Person.from_json(lidatong.to_json()) == lidatong
-        ```
-        
-        Pick whichever approach suits your taste. Note that there is better support for
-         the mixin approach when using _static analysis_ tools (e.g. linting, typing),
-         but the differences in implementation will be invisible in _runtime_ usage.
-        
-        ## How do I...
-        
-        
-        
-        ### Use my dataclass with JSON arrays or objects?
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        ```
-        
-        **Encode into a JSON array containing instances of my Data Class**
-        
-        ```python
-        people_json = [Person('lidatong')]
-        Person.schema().dumps(people_json, many=True)  # '[{"name": "lidatong"}]'
-        ```
-        
-        **Decode a JSON array containing instances of my Data Class**
-        
-        ```python
-        people_json = '[{"name": "lidatong"}]'
-        Person.schema().loads(people_json, many=True)  # [Person(name='lidatong')]
-        ```
-        
-        **Encode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
-        request/response)**
-        
-        ```python
-        import json
-        
-        response_dict = {
-            'response': {
-                'person': Person('lidatong').to_dict()
-            }
-        }
-        
-        response_json = json.dumps(response_dict)
-        ```
-        
-        In this case, we do two steps. First, we encode the dataclass into a 
-        **python dictionary** rather than a JSON string, using `.to_dict`. 
-        
-        Second, we leverage the built-in `json.dumps` to serialize our `dataclass` into 
-        a JSON string.
-        
-        **Decode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
-        response)**
-        
-        ```python
-        import json
-        
-        response_dict = json.loads('{"response": {"person": {"name": "lidatong"}}}')
-        
-        person_dict = response_dict['response']
-        
-        person = Person.from_dict(person_dict)
-        ```
-        
-        In a similar vein to encoding above, we leverage the built-in `json` module.
-        
-        First, call `json.loads` to read the entire JSON object into a 
-        dictionary. We then access the key of the value containing the encoded dict of 
-        our `Person` that we want to decode (`response_dict['response']`).
-        
-        Second, we load in the dictionary using `Person.from_dict`.
-        
-        
-        ### Encode or decode into Python lists/dictionaries rather than JSON?
-        
-        This can be by calling `.schema()` and then using the corresponding 
-        encoder/decoder methods, ie. `.load(...)`/`.dump(...)`.
-        
-        **Encode into a single Python dictionary**
-        
-        ```python
-        person = Person('lidatong')
-        person.to_dict()  # {'name': 'lidatong'}
-        ```
-        
-        **Encode into a list of Python dictionaries**
-        
-        ```python
-        people = [Person('lidatong')]
-        Person.schema().dump(people, many=True)  # [{'name': 'lidatong'}]
-        ```
-        
-        **Decode a dictionary into a single dataclass instance**
-        
-        ```python
-        person_dict = {'name': 'lidatong'}
-        Person.from_dict(person_dict)  # Person(name='lidatong')
-        ```
-        
-        **Decode a list of dictionaries into a list of dataclass instances**
-        
-        ```python
-        people_dicts = [{"name": "lidatong"}]
-        Person.schema().load(people_dicts, many=True)  # [Person(name='lidatong')]
-        ```
-        
-        ### Encode or decode from camelCase (or kebab-case)?
-        
-        JSON letter case by convention is camelCase, in Python members are by convention snake_case.
-        
-        You can configure it to encode/decode from other casing schemes at both the class level and the field level.
-        
-        ```python
-        from dataclasses import dataclass, field
-        
-        from dataclasses_json import LetterCase, config, dataclass_json
-        
-        
-        # changing casing at the class level
-        @dataclass_json(letter_case=LetterCase.CAMEL)
-        @dataclass
-        class Person:
-            given_name: str
-            family_name: str
-            
-        Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
-        Person.from_json('{"givenName": "Alice", "familyName": "Liddell"}')  # Person('Alice', 'Liddell')
-        
-        # at the field level
-        @dataclass_json
-        @dataclass
-        class Person:
-            given_name: str = field(metadata=config(letter_case=LetterCase.CAMEL))
-            family_name: str
-            
-        Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
-        # notice how the `family_name` field is still snake_case, because it wasn't configured above
-        Person.from_json('{"givenName": "Alice", "family_name": "Liddell"}')  # Person('Alice', 'Liddell')
-        ```
-        
-        **This library assumes your field follows the Python convention of snake_case naming.**
-        If your field is not `snake_case` to begin with and you attempt to parameterize `LetterCase`, 
-        the behavior of encoding/decoding is undefined (most likely it will result in subtle bugs).
-        
-        ### Encode or decode using a different name
-        
-        ```python
-        from dataclasses import dataclass, field
-        
-        from dataclasses_json import config, dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            given_name: str = field(metadata=config(field_name="overriddenGivenName"))
-        
-        Person(given_name="Alice")  # Person('Alice')
-        Person.from_json('{"overriddenGivenName": "Alice"}')  # Person('Alice')
-        Person('Alice').to_json()  # {"overriddenGivenName": "Alice"}
-        ```
-        
-        ### Handle missing or optional field values when decoding?
-        
-        By default, any fields in your dataclass that use `default` or 
-        `default_factory` will have the values filled with the provided default, if the
-        corresponding field is missing from the JSON you're decoding.
-        
-        **Decode JSON with missing field**
-        
-        ```python
-        @dataclass_json
-        @dataclass
-        class Student:
-            id: int
-            name: str = 'student'
-        
-        Student.from_json('{"id": 1}')  # Student(id=1, name='student')
-        ```
-        
-        Notice `from_json` filled the field `name` with the specified default 'student'
-        when it was missing from the JSON.
-        
-        Sometimes you have fields that are typed as `Optional`, but you don't 
-        necessarily want to assign a default. In that case, you can use the 
-        `infer_missing` kwarg to make `from_json` infer the missing field value as `None`.
-        
-        **Decode optional field without default**
-        
-        ```python
-        @dataclass_json
-        @dataclass
-        class Tutor:
-            id: int
-            student: Optional[Student] = None
-        
-        Tutor.from_json('{"id": 1}')  # Tutor(id=1, student=None)
-        ```
-        
-        Personally I recommend you leverage dataclass defaults rather than using 
-        `infer_missing`, but if for some reason you need to decouple the behavior of 
-        JSON decoding from the field's default value, this will allow you to do so.
-        
-        
-        ### Handle unknown / extraneous fields in JSON?
-        
-        By default, it is up to the implementation what happens when a `json_dataclass` receives input parameters that are not defined.
-        (the `from_dict` method ignores them, when loading using `schema()` a ValidationError is raised.)
-        There are three ways to customize this behavior.
-        
-        Assume you want to instantiate a dataclass with the following dictionary:
-        ```python
-        dump_dict = {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}, "undefined_field_name": [1, 2, 3]}
-        ```
-        
-        1. You can enforce to always raise an error by setting the `undefined` keyword to `Undefined.RAISE`
-         (`'RAISE'` as a case-insensitive string works as well). Of course it works normally if you don't pass any undefined parameters.
-            
-        ```python
-        from dataclasses_json import Undefined
-        
-        @dataclass_json(undefined=Undefined.RAISE)
-        @dataclass()
-        class ExactAPIDump:
-            endpoint: str
-            data: Dict[str, Any]
-        
-        dump = ExactAPIDump.from_dict(dump_dict)  # raises UndefinedParameterError
-        ```
-        
-        2. You can simply ignore any undefined parameters by setting the `undefined` keyword to `Undefined.EXCLUDE`
-         (`'EXCLUDE'` as a case-insensitive string works as well). Note that you will not be able to retrieve them using `to_dict`:
-            
-        ```python
-        from dataclasses_json import Undefined
-        
-        @dataclass_json(undefined=Undefined.EXCLUDE)
-        @dataclass()
-        class DontCareAPIDump:
-            endpoint: str
-            data: Dict[str, Any]
-        
-        dump = DontCareAPIDump.from_dict(dump_dict)  # DontCareAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'})
-        dump.to_dict()  # {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}}
-        ```
-        
-        3. You can save them in a catch-all field and do whatever needs to be done later. Simply set the `undefined`
-        keyword to `Undefined.INCLUDE` (`'INCLUDE'` as a case-insensitive string works as well) and define a field
-        of type `CatchAll` where all unknown values will end up.
-         This simply represents a dictionary that can hold anything. 
-         If there are no undefined parameters, this will be an empty dictionary.
-            
-        ```python
-        from dataclasses_json import Undefined, CatchAll
-        
-        @dataclass_json(undefined=Undefined.INCLUDE)
-        @dataclass()
-        class UnknownAPIDump:
-            endpoint: str
-            data: Dict[str, Any]
-            unknown_things: CatchAll
-        
-        dump = UnknownAPIDump.from_dict(dump_dict)  # UnknownAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'}, unknown_things={'undefined_field_name': [1, 2, 3]})
-        dump.to_dict()  # {'endpoint': 'some_api_endpoint', 'data': {'foo': 1, 'bar': '2'}, 'undefined_field_name': [1, 2, 3]}
-        ```
-        
-        Notes:
-        - When using `Undefined.INCLUDE`, an `UndefinedParameterError` will be raised if you don't specify
-        exactly one field of type `CatchAll`.
-        - Note that `LetterCase` does not affect values written into the `CatchAll` field, they will be as they are given.
-        - When specifying a default (or a default factory) for the the `CatchAll`-field, e.g. `unknown_things: CatchAll = None`, the default value will be used instead of an empty dict if there are no undefined parameters.
-        - Calling __init__ with non-keyword arguments resolves the arguments to the defined fields and writes everything else into the catch-all field.
-        
-        4. All 3 options work as well using `schema().loads` and `schema().dumps`, as long as you don't overwrite it by specifying `schema(unknown=<a marshmallow value>)`.
-        marshmallow uses the same 3 keywords ['include', 'exclude', 'raise'](https://marshmallow.readthedocs.io/en/stable/quickstart.html#handling-unknown-fields).
-        
-        5. All 3 operations work as well using `__init__`, e.g. `UnknownAPIDump(**dump_dict)` will **not** raise a `TypeError`, but write all unknown values to the field tagged as `CatchAll`.
-           Classes tagged with `EXCLUDE` will also simply ignore unknown parameters. Note that classes tagged as `RAISE` still raise a `TypeError`, and **not** a `UndefinedParameterError` if supplied with unknown keywords.
-        
-        
-        ### Override the default encode / decode / marshmallow field of a specific field?
-        
-        See [Overriding](#Overriding)
-        
-        ### Handle recursive dataclasses?
-        Object hierarchies where fields are of the type that they are declared within require a small
-        type hinting trick to declare the forward reference.
-        ```python
-        from typing import Optional
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Tree():
-            value: str
-            left: Optional['Tree']
-            right: Optional['Tree']
-        ```
-        
-        Avoid using
-        ```python
-        from __future__ import annotations
-        ```
-        as it will cause problems with the way dataclasses_json accesses the type annotations.
-        
-        
-        ## Marshmallow interop
-        
-        Using the `dataclass_json` decorator or mixing in `DataClassJsonMixin` will
-        provide you with an additional method `.schema()`.
-        
-        `.schema()` generates a schema exactly equivalent to manually creating a
-        marshmallow schema for your dataclass. You can reference the [marshmallow API docs](https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
-        to learn other ways you can use the schema returned by `.schema()`.
-        
-        You can pass in the exact same arguments to `.schema()` that you would when
-        constructing a `PersonSchema` instance, e.g. `.schema(many=True)`, and they will
-        get passed through to the marshmallow schema.
-        
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        
-        # You don't need to do this - it's generated for you by `.schema()`!
-        from marshmallow import Schema, fields
-        
-        class PersonSchema(Schema):
-            name = fields.Str()
-        ```
-        
-        Briefly, on what's going on under the hood in the above examples: calling 
-        `.schema()` will have this library generate a
-        [marshmallow schema]('https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
-        for you. It also fills in the corresponding object hook, so that marshmallow
-        will create an instance of your Data Class on `load` (e.g.
-        `Person.schema().load` returns a `Person`) rather than a `dict`, which it does
-        by default in marshmallow.
-        
-        **Performance note**
-        
-        `.schema()` is not cached (it generates the schema on every call), so if you
-        have a nested Data Class you may want to save the result to a variable to 
-        avoid re-generation of the schema on every usage.
-        
-        ```python
-        person_schema = Person.schema()
-        person_schema.dump(people, many=True)
-        
-        # later in the code...
-        
-        person_schema.dump(person)
-        ```
-        
-        ## Overriding / Extending
-        
-        #### Overriding
-        
-        For example, you might want to encode/decode `datetime` objects using ISO format
-        rather than the default `timestamp`.
-        
-        ```python
-        from dataclasses import dataclass, field
-        from dataclasses_json import dataclass_json, config
-        from datetime import datetime
-        from marshmallow import fields
-        
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: datetime = field(
-                metadata=config(
-                    encoder=datetime.isoformat,
-                    decoder=datetime.fromisoformat,
-                    mm_field=fields.DateTime(format='iso')
-                )
-            )
-        ```
-        
-        #### Extending
-        
-        Similarly, you might want to extend `dataclasses_json` to encode `date` objects.
-        
-        ```python
-        from dataclasses import dataclass, field
-        from dataclasses_json import dataclass_json, config
-        from datetime import date
-        from marshmallow import fields
-        
-        dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
-        dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
-        
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: date
-            modified_at: date
-            accessed_at: date
-        ```
-        
-        As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
-        callable:
-        - `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
-        - `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
-        - `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
-        
-        Note that these hooks will be invoked regardless if you're using 
-        `.to_json`/`dump`/`dumps`
-        and `.from_json`/`load`/`loads`. So apply overrides / extensions judiciously, making sure to 
-        carefully consider whether the interaction of the encode/decode/mm_field is consistent with what you expect!
-        
-        
-        #### What if I have other dataclass field extensions that rely on `metadata`
-        
-        All the `dataclasses_json.config` does is return a mapping, namespaced under the key `'dataclasses_json'`.
-        
-        Say there's another module, `other_dataclass_package` that uses metadata. Here's how you solve your problem:
-        
-        ```python
-        metadata = {'other_dataclass_package': 'some metadata...'}  # pre-existing metadata for another dataclass package
-        dataclass_json_config = config(
-                    encoder=datetime.isoformat,
-                    decoder=datetime.fromisoformat,
-                    mm_field=fields.DateTime(format='iso')
-                )
-        metadata.update(dataclass_json_config)
-        
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: datetime = field(metadata=metadata)
-        ```
-        
-        You can also manually specify the dataclass_json configuration mapping.
-        
-        ```python
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: date = field(
-                metadata={'dataclasses_json': {
-                    'encoder': date.isoformat,
-                    'decoder': date.fromisoformat,
-                    'mm_field': fields.DateTime(format='iso')
-                }}
-            )
-        ```
-        
-        ## A larger example
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        from typing import List
-        
-        @dataclass_json
-        @dataclass(frozen=True)
-        class Minion:
-            name: str
-        
-        
-        @dataclass_json
-        @dataclass(frozen=True)
-        class Boss:
-            minions: List[Minion]
-        
-        boss = Boss([Minion('evil minion'), Minion('very evil minion')])
-        boss_json = """
-        {
-            "minions": [
-                {
-                    "name": "evil minion"
-                },
-                {
-                    "name": "very evil minion"
-                }
-            ]
-        }
-        """.strip()
-        
-        assert boss.to_json(indent=4) == boss_json
-        assert Boss.from_json(boss_json) == boss
-        ```
-        
-        ## Performance
-        
-        Take a look at [this issue](https://github.com/lidatong/dataclasses-json/issues/228)
-        
-        ## Versioning
-        
-        Note this library is still pre-1.0.0 (SEMVER).
-        
-        The current convention is:
-        - **PATCH** version upgrades for bug fixes and minor feature additions.
-        - **MINOR** version upgrades for big API features and breaking changes.
-        
-        Once this library is 1.0.0, it will follow standard SEMVER conventions.
-        
-        
-        ## Roadmap
-        
-        Currently the focus is on investigating and fixing bugs in this library, working
-        on performance, and finishing [this issue](https://github.com/lidatong/dataclasses-json/issues/31).
-        
-        That said, if you think there's a feature missing / something new needed in the
-        library, please see the contributing section below.
-        
-        
-        ## Contributing
-        
-        First of all, thank you for being interested in contributing to this library.
-        I really appreciate you taking the time to work on this project.
-        
-        - If you're just interested in getting into the code, a good place to start are 
-        issues tagged as bugs.
-        - If introducing a new feature, especially one that modifies the public API, 
-        consider submitting an issue for discussion before a PR. Please also take a look 
-        at existing issues / PRs to see what you're proposing has  already been covered 
-        before / exists.
-        - I like to follow the commit conventions documented [here](https://www.conventionalcommits.org/en/v1.0.0/#summary)
-        
 Keywords: dataclasses json
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Dataclasses JSON
+
+![](https://github.com/lidatong/dataclasses-json/workflows/dataclasses-json/badge.svg)
+
+This library provides a simple API for encoding and decoding [dataclasses](https://docs.python.org/3/library/dataclasses.html) to and from JSON.
+
+It's very easy to get started.
+
+[README / Documentation website](https://lidatong.github.io/dataclasses-json). Features a navigation bar and search functionality, and should mirror this README exactly -- take a look!
+
+## Quickstart
+
+`pip install dataclasses-json`
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+
+
+person = Person(name='lidatong')
+person.to_json()  # '{"name": "lidatong"}' <- this is a string
+person.to_dict()  # {'name': 'lidatong'} <- this is a dict
+Person.from_json('{"name": "lidatong"}')  # Person(1)
+Person.from_dict({'name': 'lidatong'})  # Person(1)
+
+# You can also apply _schema validation_ using an alternative API
+# This can be useful for "typed" Python code
+
+Person.from_json('{"name": 42}')  # This is ok. 42 is not a `str`, but
+                                  # dataclass creation does not validate types
+Person.schema().loads('{"name": 42}')  # Error! Raises `ValidationError`
+```
+
+**What if you want to work with camelCase JSON?**
+
+```python
+# same imports as above, with the additional `LetterCase` import
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json, LetterCase
+
+@dataclass_json(letter_case=LetterCase.CAMEL)  # now all fields are encoded/decoded from camelCase
+@dataclass
+class ConfiguredSimpleExample:
+    int_field: int
+
+ConfiguredSimpleExample(1).to_json()  # {"intField": 1}
+ConfiguredSimpleExample.from_json('{"intField": 1}')  # ConfiguredSimpleExample(1)
+```
+
+## Supported types
+
+It's recursive (see caveats below), so you can easily work with nested dataclasses.
+In addition to the supported types in the 
+[py to JSON table](https://docs.python.org/3/library/json.html#py-to-json-table), this library supports the following:
+
+- any arbitrary [Collection](https://docs.python.org/3/library/collections.abc.html#collections.abc.Collection) type is supported.
+[Mapping](https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping) types are encoded as JSON objects and `str` types as JSON strings. 
+Any other Collection types are encoded into JSON arrays, but decoded into the original collection types.
+
+- [datetime](https://docs.python.org/3/library/datetime.html#available-types) 
+objects. `datetime` objects are encoded to `float` (JSON number) using 
+[timestamp](https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp).
+As specified in the `datetime` docs, if your `datetime` object is naive, it will 
+assume your system local timezone when calling `.timestamp()`. JSON numbers 
+corresponding to a `datetime` field in your dataclass are decoded 
+into a datetime-aware object, with `tzinfo` set to your system local timezone.
+Thus, if you encode a datetime-naive object, you will decode into a 
+datetime-aware object. This is important, because encoding and decoding won't 
+strictly be inverses. See [this section](#Overriding) if you want to override this default
+behavior (for example, if you want to use ISO).
+
+- [UUID](https://docs.python.org/3/library/uuid.html#uuid.UUID) objects. They 
+are encoded as `str` (JSON string).
+
+- [Decimal](https://docs.python.org/3/library/decimal.html) objects. They are
+also encoded as `str`.
+
+**The [latest release](https://github.com/lidatong/dataclasses-json/releases/latest) is compatible with both Python 3.7 and Python 3.6 (with the dataclasses backport).**
+
+## Usage
+
+#### Approach 1: Class decorator
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+
+lidatong = Person('lidatong')
+
+# Encoding to JSON
+lidatong.to_json()  # '{"name": "lidatong"}'
+
+# Decoding from JSON
+Person.from_json('{"name": "lidatong"}')  # Person(name='lidatong')
+```
+
+Note that the `@dataclass_json` decorator must be stacked above the `@dataclass`
+decorator (order matters!)
+
+#### Approach 2: Inherit from a mixin
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import DataClassJsonMixin
+
+@dataclass
+class Person(DataClassJsonMixin):
+    name: str
+
+lidatong = Person('lidatong')
+
+# A different example from Approach 1 above, but usage is the exact same
+assert Person.from_json(lidatong.to_json()) == lidatong
+```
+
+Pick whichever approach suits your taste. Note that there is better support for
+ the mixin approach when using _static analysis_ tools (e.g. linting, typing),
+ but the differences in implementation will be invisible in _runtime_ usage.
+
+## How do I...
+
+
+
+### Use my dataclass with JSON arrays or objects?
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+```
+
+**Encode into a JSON array containing instances of my Data Class**
+
+```python
+people_json = [Person('lidatong')]
+Person.schema().dumps(people_json, many=True)  # '[{"name": "lidatong"}]'
+```
+
+**Decode a JSON array containing instances of my Data Class**
+
+```python
+people_json = '[{"name": "lidatong"}]'
+Person.schema().loads(people_json, many=True)  # [Person(name='lidatong')]
+```
+
+**Encode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
+request/response)**
+
+```python
+import json
+
+response_dict = {
+    'response': {
+        'person': Person('lidatong').to_dict()
+    }
+}
+
+response_json = json.dumps(response_dict)
+```
+
+In this case, we do two steps. First, we encode the dataclass into a 
+**python dictionary** rather than a JSON string, using `.to_dict`. 
+
+Second, we leverage the built-in `json.dumps` to serialize our `dataclass` into 
+a JSON string.
+
+**Decode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
+response)**
+
+```python
+import json
+
+response_dict = json.loads('{"response": {"person": {"name": "lidatong"}}}')
+
+person_dict = response_dict['response']
+
+person = Person.from_dict(person_dict)
+```
+
+In a similar vein to encoding above, we leverage the built-in `json` module.
+
+First, call `json.loads` to read the entire JSON object into a 
+dictionary. We then access the key of the value containing the encoded dict of 
+our `Person` that we want to decode (`response_dict['response']`).
+
+Second, we load in the dictionary using `Person.from_dict`.
+
+
+### Encode or decode into Python lists/dictionaries rather than JSON?
+
+This can be by calling `.schema()` and then using the corresponding 
+encoder/decoder methods, ie. `.load(...)`/`.dump(...)`.
+
+**Encode into a single Python dictionary**
+
+```python
+person = Person('lidatong')
+person.to_dict()  # {'name': 'lidatong'}
+```
+
+**Encode into a list of Python dictionaries**
+
+```python
+people = [Person('lidatong')]
+Person.schema().dump(people, many=True)  # [{'name': 'lidatong'}]
+```
+
+**Decode a dictionary into a single dataclass instance**
+
+```python
+person_dict = {'name': 'lidatong'}
+Person.from_dict(person_dict)  # Person(name='lidatong')
+```
+
+**Decode a list of dictionaries into a list of dataclass instances**
+
+```python
+people_dicts = [{"name": "lidatong"}]
+Person.schema().load(people_dicts, many=True)  # [Person(name='lidatong')]
+```
+
+### Encode or decode from camelCase (or kebab-case)?
+
+JSON letter case by convention is camelCase, in Python members are by convention snake_case.
+
+You can configure it to encode/decode from other casing schemes at both the class level and the field level.
+
+```python
+from dataclasses import dataclass, field
+
+from dataclasses_json import LetterCase, config, dataclass_json
+
+
+# changing casing at the class level
+@dataclass_json(letter_case=LetterCase.CAMEL)
+@dataclass
+class Person:
+    given_name: str
+    family_name: str
+    
+Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
+Person.from_json('{"givenName": "Alice", "familyName": "Liddell"}')  # Person('Alice', 'Liddell')
+
+# at the field level
+@dataclass_json
+@dataclass
+class Person:
+    given_name: str = field(metadata=config(letter_case=LetterCase.CAMEL))
+    family_name: str
+    
+Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
+# notice how the `family_name` field is still snake_case, because it wasn't configured above
+Person.from_json('{"givenName": "Alice", "family_name": "Liddell"}')  # Person('Alice', 'Liddell')
+```
+
+**This library assumes your field follows the Python convention of snake_case naming.**
+If your field is not `snake_case` to begin with and you attempt to parameterize `LetterCase`, 
+the behavior of encoding/decoding is undefined (most likely it will result in subtle bugs).
+
+### Encode or decode using a different name
+
+```python
+from dataclasses import dataclass, field
+
+from dataclasses_json import config, dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    given_name: str = field(metadata=config(field_name="overriddenGivenName"))
+
+Person(given_name="Alice")  # Person('Alice')
+Person.from_json('{"overriddenGivenName": "Alice"}')  # Person('Alice')
+Person('Alice').to_json()  # {"overriddenGivenName": "Alice"}
+```
+
+### Handle missing or optional field values when decoding?
+
+By default, any fields in your dataclass that use `default` or 
+`default_factory` will have the values filled with the provided default, if the
+corresponding field is missing from the JSON you're decoding.
+
+**Decode JSON with missing field**
+
+```python
+@dataclass_json
+@dataclass
+class Student:
+    id: int
+    name: str = 'student'
+
+Student.from_json('{"id": 1}')  # Student(id=1, name='student')
+```
+
+Notice `from_json` filled the field `name` with the specified default 'student'
+when it was missing from the JSON.
+
+Sometimes you have fields that are typed as `Optional`, but you don't 
+necessarily want to assign a default. In that case, you can use the 
+`infer_missing` kwarg to make `from_json` infer the missing field value as `None`.
+
+**Decode optional field without default**
+
+```python
+@dataclass_json
+@dataclass
+class Tutor:
+    id: int
+    student: Optional[Student] = None
+
+Tutor.from_json('{"id": 1}')  # Tutor(id=1, student=None)
+```
+
+Personally I recommend you leverage dataclass defaults rather than using 
+`infer_missing`, but if for some reason you need to decouple the behavior of 
+JSON decoding from the field's default value, this will allow you to do so.
+
+
+### Handle unknown / extraneous fields in JSON?
+
+By default, it is up to the implementation what happens when a `json_dataclass` receives input parameters that are not defined.
+(the `from_dict` method ignores them, when loading using `schema()` a ValidationError is raised.)
+There are three ways to customize this behavior.
+
+Assume you want to instantiate a dataclass with the following dictionary:
+```python
+dump_dict = {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}, "undefined_field_name": [1, 2, 3]}
+```
+
+1. You can enforce to always raise an error by setting the `undefined` keyword to `Undefined.RAISE`
+ (`'RAISE'` as a case-insensitive string works as well). Of course it works normally if you don't pass any undefined parameters.
+    
+```python
+from dataclasses_json import Undefined
+
+@dataclass_json(undefined=Undefined.RAISE)
+@dataclass()
+class ExactAPIDump:
+    endpoint: str
+    data: Dict[str, Any]
+
+dump = ExactAPIDump.from_dict(dump_dict)  # raises UndefinedParameterError
+```
+
+2. You can simply ignore any undefined parameters by setting the `undefined` keyword to `Undefined.EXCLUDE`
+ (`'EXCLUDE'` as a case-insensitive string works as well). Note that you will not be able to retrieve them using `to_dict`:
+    
+```python
+from dataclasses_json import Undefined
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclass()
+class DontCareAPIDump:
+    endpoint: str
+    data: Dict[str, Any]
+
+dump = DontCareAPIDump.from_dict(dump_dict)  # DontCareAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'})
+dump.to_dict()  # {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}}
+```
+
+3. You can save them in a catch-all field and do whatever needs to be done later. Simply set the `undefined`
+keyword to `Undefined.INCLUDE` (`'INCLUDE'` as a case-insensitive string works as well) and define a field
+of type `CatchAll` where all unknown values will end up.
+ This simply represents a dictionary that can hold anything. 
+ If there are no undefined parameters, this will be an empty dictionary.
+    
+```python
+from dataclasses_json import Undefined, CatchAll
+
+@dataclass_json(undefined=Undefined.INCLUDE)
+@dataclass()
+class UnknownAPIDump:
+    endpoint: str
+    data: Dict[str, Any]
+    unknown_things: CatchAll
+
+dump = UnknownAPIDump.from_dict(dump_dict)  # UnknownAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'}, unknown_things={'undefined_field_name': [1, 2, 3]})
+dump.to_dict()  # {'endpoint': 'some_api_endpoint', 'data': {'foo': 1, 'bar': '2'}, 'undefined_field_name': [1, 2, 3]}
+```
+
+Notes:
+- When using `Undefined.INCLUDE`, an `UndefinedParameterError` will be raised if you don't specify
+exactly one field of type `CatchAll`.
+- Note that `LetterCase` does not affect values written into the `CatchAll` field, they will be as they are given.
+- When specifying a default (or a default factory) for the the `CatchAll`-field, e.g. `unknown_things: CatchAll = None`, the default value will be used instead of an empty dict if there are no undefined parameters.
+- Calling __init__ with non-keyword arguments resolves the arguments to the defined fields and writes everything else into the catch-all field.
+
+4. All 3 options work as well using `schema().loads` and `schema().dumps`, as long as you don't overwrite it by specifying `schema(unknown=<a marshmallow value>)`.
+marshmallow uses the same 3 keywords ['include', 'exclude', 'raise'](https://marshmallow.readthedocs.io/en/stable/quickstart.html#handling-unknown-fields).
+
+5. All 3 operations work as well using `__init__`, e.g. `UnknownAPIDump(**dump_dict)` will **not** raise a `TypeError`, but write all unknown values to the field tagged as `CatchAll`.
+   Classes tagged with `EXCLUDE` will also simply ignore unknown parameters. Note that classes tagged as `RAISE` still raise a `TypeError`, and **not** a `UndefinedParameterError` if supplied with unknown keywords.
+
+
+### Override the default encode / decode / marshmallow field of a specific field?
+
+See [Overriding](#Overriding)
+
+### Handle recursive dataclasses?
+Object hierarchies where fields are of the type that they are declared within require a small
+type hinting trick to declare the forward reference.
+```python
+from typing import Optional
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Tree():
+    value: str
+    left: Optional['Tree']
+    right: Optional['Tree']
+```
+
+Avoid using
+```python
+from __future__ import annotations
+```
+as it will cause problems with the way dataclasses_json accesses the type annotations.
+
+
+## Marshmallow interop
+
+Using the `dataclass_json` decorator or mixing in `DataClassJsonMixin` will
+provide you with an additional method `.schema()`.
+
+`.schema()` generates a schema exactly equivalent to manually creating a
+marshmallow schema for your dataclass. You can reference the [marshmallow API docs](https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
+to learn other ways you can use the schema returned by `.schema()`.
+
+You can pass in the exact same arguments to `.schema()` that you would when
+constructing a `PersonSchema` instance, e.g. `.schema(many=True)`, and they will
+get passed through to the marshmallow schema.
+
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+
+# You don't need to do this - it's generated for you by `.schema()`!
+from marshmallow import Schema, fields
+
+class PersonSchema(Schema):
+    name = fields.Str()
+```
+
+Briefly, on what's going on under the hood in the above examples: calling 
+`.schema()` will have this library generate a
+[marshmallow schema]('https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
+for you. It also fills in the corresponding object hook, so that marshmallow
+will create an instance of your Data Class on `load` (e.g.
+`Person.schema().load` returns a `Person`) rather than a `dict`, which it does
+by default in marshmallow.
+
+**Performance note**
+
+`.schema()` is not cached (it generates the schema on every call), so if you
+have a nested Data Class you may want to save the result to a variable to 
+avoid re-generation of the schema on every usage.
+
+```python
+person_schema = Person.schema()
+person_schema.dump(people, many=True)
+
+# later in the code...
+
+person_schema.dump(person)
+```
+
+## Overriding / Extending
+
+#### Overriding
+
+For example, you might want to encode/decode `datetime` objects using ISO format
+rather than the default `timestamp`.
+
+```python
+from dataclasses import dataclass, field
+from dataclasses_json import dataclass_json, config
+from datetime import datetime
+from marshmallow import fields
+
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: datetime = field(
+        metadata=config(
+            encoder=datetime.isoformat,
+            decoder=datetime.fromisoformat,
+            mm_field=fields.DateTime(format='iso')
+        )
+    )
+```
+
+#### Extending
+
+Similarly, you might want to extend `dataclasses_json` to encode `date` objects.
+
+```python
+from dataclasses import dataclass, field
+from dataclasses_json import dataclass_json, config
+from datetime import date
+from marshmallow import fields
+
+dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
+dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
+
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: date
+    modified_at: date
+    accessed_at: date
+```
+
+As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
+callable:
+- `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
+- `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
+- `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
+
+Note that these hooks will be invoked regardless if you're using 
+`.to_json`/`dump`/`dumps`
+and `.from_json`/`load`/`loads`. So apply overrides / extensions judiciously, making sure to 
+carefully consider whether the interaction of the encode/decode/mm_field is consistent with what you expect!
+
+
+#### What if I have other dataclass field extensions that rely on `metadata`
+
+All the `dataclasses_json.config` does is return a mapping, namespaced under the key `'dataclasses_json'`.
+
+Say there's another module, `other_dataclass_package` that uses metadata. Here's how you solve your problem:
+
+```python
+metadata = {'other_dataclass_package': 'some metadata...'}  # pre-existing metadata for another dataclass package
+dataclass_json_config = config(
+            encoder=datetime.isoformat,
+            decoder=datetime.fromisoformat,
+            mm_field=fields.DateTime(format='iso')
+        )
+metadata.update(dataclass_json_config)
+
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: datetime = field(metadata=metadata)
+```
+
+You can also manually specify the dataclass_json configuration mapping.
+
+```python
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: date = field(
+        metadata={'dataclasses_json': {
+            'encoder': date.isoformat,
+            'decoder': date.fromisoformat,
+            'mm_field': fields.DateTime(format='iso')
+        }}
+    )
+```
+
+## A larger example
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+from typing import List
+
+@dataclass_json
+@dataclass(frozen=True)
+class Minion:
+    name: str
+
+
+@dataclass_json
+@dataclass(frozen=True)
+class Boss:
+    minions: List[Minion]
+
+boss = Boss([Minion('evil minion'), Minion('very evil minion')])
+boss_json = """
+{
+    "minions": [
+        {
+            "name": "evil minion"
+        },
+        {
+            "name": "very evil minion"
+        }
+    ]
+}
+""".strip()
+
+assert boss.to_json(indent=4) == boss_json
+assert Boss.from_json(boss_json) == boss
+```
+
+## Performance
+
+Take a look at [this issue](https://github.com/lidatong/dataclasses-json/issues/228)
+
+## Versioning
+
+Note this library is still pre-1.0.0 (SEMVER).
+
+The current convention is:
+- **PATCH** version upgrades for bug fixes and minor feature additions.
+- **MINOR** version upgrades for big API features and breaking changes.
+
+Once this library is 1.0.0, it will follow standard SEMVER conventions.
+
+
+## Roadmap
+
+Currently the focus is on investigating and fixing bugs in this library, working
+on performance, and finishing [this issue](https://github.com/lidatong/dataclasses-json/issues/31).
+
+That said, if you think there's a feature missing / something new needed in the
+library, please see the contributing section below.
+
+
+## Contributing
+
+First of all, thank you for being interested in contributing to this library.
+I really appreciate you taking the time to work on this project.
+
+- If you're just interested in getting into the code, a good place to start are 
+issues tagged as bugs.
+- If introducing a new feature, especially one that modifies the public API, 
+consider submitting an issue for discussion before a PR. Please also take a look 
+at existing issues / PRs to see what you're proposing has  already been covered 
+before / exists.
+- I like to follow the commit conventions documented [here](https://www.conventionalcommits.org/en/v1.0.0/#summary)
```

### Comparing `dataclasses-json-0.5.8/README.md` & `dataclasses-json-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/dataclasses_json/api.py` & `dataclasses-json-0.5.9/dataclasses_json/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                only=None,
                exclude=(),
                many: bool = False,
                context=None,
                load_only=(),
                dump_only=(),
                partial: bool = False,
-               unknown=None) -> SchemaType:
+               unknown=None) -> "SchemaType[A]":
         Schema = build_schema(cls, DataClassJsonMixin, infer_missing, partial)
 
         if unknown is None:
             undefined_parameter_action = _undefined_parameter_action_safe(cls)
             if undefined_parameter_action is not None:
                 # We can just make use of the same-named mm keywords
                 unknown = undefined_parameter_action.name.lower()
@@ -118,15 +118,15 @@
         return _process_class(cls, letter_case, undefined)
 
     if _cls is None:
         return wrap
     return wrap(_cls)
 
 
-def _process_class(cls, letter_case, undefined):
+def _process_class(cls, letter_case, undefined) -> Type[DataClassJsonMixin]:
     if letter_case is not None or undefined is not None:
         cls.dataclass_json_config = config(letter_case=letter_case,
                                            undefined=undefined)[
             'dataclasses_json']
 
     cls.to_json = DataClassJsonMixin.to_json
     # unwrap and rewrap classmethod to tag it to cls rather than the literal
```

### Comparing `dataclasses-json-0.5.8/dataclasses_json/cfg.py` & `dataclasses-json-0.5.9/dataclasses_json/cfg.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/dataclasses_json/core.py` & `dataclasses-json-0.5.9/dataclasses_json/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,25 +163,31 @@
         # The field should be skipped from being added
         # to init_kwargs as it's not intended as a constructor argument.
         if not field.init:
             continue
 
         field_value = kvs[field.name]
         field_type = types[field.name]
-        if field_value is None and not _is_optional(field_type):
-            warning = (f"value of non-optional type {field.name} detected "
-                       f"when decoding {cls.__name__}")
-            if infer_missing:
-                warnings.warn(
-                    f"Missing {warning} and was defaulted to None by "
-                    f"infer_missing=True. "
-                    f"Set infer_missing=False (the default) to prevent this "
-                    f"behavior.", RuntimeWarning)
-            else:
-                warnings.warn(f"`NoneType` object {warning}.", RuntimeWarning)
+        if field_value is None:
+            if not _is_optional(field_type):
+                warning = (
+                    f"value of non-optional type {field.name} detected "
+                    f"when decoding {cls.__name__}"
+                )
+                if infer_missing:
+                    warnings.warn(
+                        f"Missing {warning} and was defaulted to None by "
+                        f"infer_missing=True. "
+                        f"Set infer_missing=False (the default) to prevent "
+                        f"this behavior.", RuntimeWarning
+                    )
+                else:
+                    warnings.warn(
+                        f"`NoneType` object {warning}.", RuntimeWarning
+                    )
             init_kwargs[field.name] = field_value
             continue
 
         while True:
             if not _is_new_type(field_type):
                 break
 
@@ -231,14 +237,18 @@
         res = (field_value
                if isinstance(field_value, Decimal)
                else Decimal(field_value))
     elif _issubclass_safe(field_type, UUID):
         res = (field_value
                if isinstance(field_value, UUID)
                else UUID(field_value))
+    elif _issubclass_safe(field_type, (int, float, str, bool)):
+        res = (field_value
+               if isinstance(field_value, field_type)
+               else field_type(field_value))
     else:
         res = field_value
     return res
 
 
 def _is_supported_generic(type_):
     if type_ is _NO_ARGS:
```

### Comparing `dataclasses-json-0.5.8/dataclasses_json/mm.py` & `dataclasses-json-0.5.9/dataclasses_json/mm.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
 A = typing.TypeVar('A')
 JsonData = typing.Union[str, bytes, bytearray]
 TEncoded = typing.Dict[str, typing.Any]
 TOneOrMulti = typing.Union[typing.List[A], A]
 TOneOrMultiEncoded = typing.Union[typing.List[TEncoded], TEncoded]
 
-if sys.version_info >= (3, 7):
+if sys.version_info >= (3, 7) or typing.TYPE_CHECKING:
     class SchemaF(Schema, typing.Generic[A]):
         """Lift Schema into a type constructor"""
 
         def __init__(self, *args, **kwargs):
             """
             Raises exception because this class should not be inherited.
             This class is helper only.
@@ -299,15 +299,15 @@
                 options['allow_none'] = True
 
             if _is_optional(type_):
                 options.setdefault(missing_key, None)
                 options['allow_none'] = True
                 if len(type_.__args__) == 2:
                     # Union[str, int, None] is optional too, but it has more than 1 typed field.
-                    type_ = type_.__args__[0]
+                    type_ = [tp for tp in type_.__args__ if tp is not type(None)][0]
 
             if metadata.letter_case is not None:
                 options['data_key'] = metadata.letter_case(field.name)
 
             t = build_type(type_, options, mixin, field, cls)
             # if type(t) is not fields.Field:  # If we use `isinstance` we would return nothing.
             if field.type != typing.Optional[CatchAllVar]:
@@ -315,15 +315,15 @@
 
     return schema
 
 
 def build_schema(cls: typing.Type[A],
                  mixin,
                  infer_missing,
-                 partial) -> typing.Type[SchemaType]:
+                 partial) -> typing.Type["SchemaType[A]"]:
     Meta = type('Meta',
                 (),
                 {'fields': tuple(field.name for field in dc_fields(cls)
                                  if
                                  field.name != 'dataclass_json_config' and field.type !=
                                  typing.Optional[CatchAllVar]),
                  # TODO #180
@@ -355,15 +355,15 @@
                                                       usage="dump"))
         else:
             dumped.update(_handle_undefined_parameters_safe(cls=obj, kvs={},
                                                             usage="dump"))
         return dumped
 
     schema_ = schema(cls, mixin, infer_missing)
-    DataClassSchema: typing.Type[SchemaType] = type(
+    DataClassSchema: typing.Type["SchemaType[A]"] = type(
         f'{cls.__name__.capitalize()}Schema',
         (Schema,),
         {'Meta': Meta,
          f'make_{cls.__name__.lower()}': make_instance,
          'dumps': dumps,
          'dump': dump,
          **schema_})
```

### Comparing `dataclasses-json-0.5.8/dataclasses_json/stringcase.py` & `dataclasses-json-0.5.9/dataclasses_json/stringcase.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/dataclasses_json/undefined.py` & `dataclasses-json-0.5.9/dataclasses_json/undefined.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/dataclasses_json/utils.py` & `dataclasses-json-0.5.9/dataclasses_json/utils.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/dataclasses_json.egg-info/PKG-INFO` & `dataclasses-json-0.5.9/dataclasses_json.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,670 +1,670 @@
 Metadata-Version: 2.1
 Name: dataclasses-json
-Version: 0.5.8
+Version: 0.5.9
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/lidatong/dataclasses-json
 Author: lidatong
 Author-email: charles.dt.li@gmail.com
 License: MIT
-Description: # Dataclasses JSON
-        
-        ![](https://github.com/lidatong/dataclasses-json/workflows/dataclasses-json/badge.svg)
-        
-        This library provides a simple API for encoding and decoding [dataclasses](https://docs.python.org/3/library/dataclasses.html) to and from JSON.
-        
-        It's very easy to get started.
-        
-        [README / Documentation website](https://lidatong.github.io/dataclasses-json). Features a navigation bar and search functionality, and should mirror this README exactly -- take a look!
-        
-        ## Quickstart
-        
-        `pip install dataclasses-json`
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        
-        
-        person = Person(name='lidatong')
-        person.to_json()  # '{"name": "lidatong"}' <- this is a string
-        person.to_dict()  # {'name': 'lidatong'} <- this is a dict
-        Person.from_json('{"name": "lidatong"}')  # Person(1)
-        Person.from_dict({'name': 'lidatong'})  # Person(1)
-        
-        # You can also apply _schema validation_ using an alternative API
-        # This can be useful for "typed" Python code
-        
-        Person.from_json('{"name": 42}')  # This is ok. 42 is not a `str`, but
-                                          # dataclass creation does not validate types
-        Person.schema().loads('{"name": 42}')  # Error! Raises `ValidationError`
-        ```
-        
-        **What if you want to work with camelCase JSON?**
-        
-        ```python
-        # same imports as above, with the additional `LetterCase` import
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json, LetterCase
-        
-        @dataclass_json(letter_case=LetterCase.CAMEL)  # now all fields are encoded/decoded from camelCase
-        @dataclass
-        class ConfiguredSimpleExample:
-            int_field: int
-        
-        ConfiguredSimpleExample(1).to_json()  # {"intField": 1}
-        ConfiguredSimpleExample.from_json('{"intField": 1}')  # ConfiguredSimpleExample(1)
-        ```
-        
-        ## Supported types
-        
-        It's recursive (see caveats below), so you can easily work with nested dataclasses.
-        In addition to the supported types in the 
-        [py to JSON table](https://docs.python.org/3/library/json.html#py-to-json-table), this library supports the following:
-        
-        - any arbitrary [Collection](https://docs.python.org/3/library/collections.abc.html#collections.abc.Collection) type is supported.
-        [Mapping](https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping) types are encoded as JSON objects and `str` types as JSON strings. 
-        Any other Collection types are encoded into JSON arrays, but decoded into the original collection types.
-        
-        - [datetime](https://docs.python.org/3/library/datetime.html#available-types) 
-        objects. `datetime` objects are encoded to `float` (JSON number) using 
-        [timestamp](https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp).
-        As specified in the `datetime` docs, if your `datetime` object is naive, it will 
-        assume your system local timezone when calling `.timestamp()`. JSON numbers 
-        corresponding to a `datetime` field in your dataclass are decoded 
-        into a datetime-aware object, with `tzinfo` set to your system local timezone.
-        Thus, if you encode a datetime-naive object, you will decode into a 
-        datetime-aware object. This is important, because encoding and decoding won't 
-        strictly be inverses. See [this section](#Overriding) if you want to override this default
-        behavior (for example, if you want to use ISO).
-        
-        - [UUID](https://docs.python.org/3/library/uuid.html#uuid.UUID) objects. They 
-        are encoded as `str` (JSON string).
-        
-        - [Decimal](https://docs.python.org/3/library/decimal.html) objects. They are
-        also encoded as `str`.
-        
-        **The [latest release](https://github.com/lidatong/dataclasses-json/releases/latest) is compatible with both Python 3.7 and Python 3.6 (with the dataclasses backport).**
-        
-        ## Usage
-        
-        #### Approach 1: Class decorator
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        
-        lidatong = Person('lidatong')
-        
-        # Encoding to JSON
-        lidatong.to_json()  # '{"name": "lidatong"}'
-        
-        # Decoding from JSON
-        Person.from_json('{"name": "lidatong"}')  # Person(name='lidatong')
-        ```
-        
-        Note that the `@dataclass_json` decorator must be stacked above the `@dataclass`
-        decorator (order matters!)
-        
-        #### Approach 2: Inherit from a mixin
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import DataClassJsonMixin
-        
-        @dataclass
-        class Person(DataClassJsonMixin):
-            name: str
-        
-        lidatong = Person('lidatong')
-        
-        # A different example from Approach 1 above, but usage is the exact same
-        assert Person.from_json(lidatong.to_json()) == lidatong
-        ```
-        
-        Pick whichever approach suits your taste. Note that there is better support for
-         the mixin approach when using _static analysis_ tools (e.g. linting, typing),
-         but the differences in implementation will be invisible in _runtime_ usage.
-        
-        ## How do I...
-        
-        
-        
-        ### Use my dataclass with JSON arrays or objects?
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        ```
-        
-        **Encode into a JSON array containing instances of my Data Class**
-        
-        ```python
-        people_json = [Person('lidatong')]
-        Person.schema().dumps(people_json, many=True)  # '[{"name": "lidatong"}]'
-        ```
-        
-        **Decode a JSON array containing instances of my Data Class**
-        
-        ```python
-        people_json = '[{"name": "lidatong"}]'
-        Person.schema().loads(people_json, many=True)  # [Person(name='lidatong')]
-        ```
-        
-        **Encode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
-        request/response)**
-        
-        ```python
-        import json
-        
-        response_dict = {
-            'response': {
-                'person': Person('lidatong').to_dict()
-            }
-        }
-        
-        response_json = json.dumps(response_dict)
-        ```
-        
-        In this case, we do two steps. First, we encode the dataclass into a 
-        **python dictionary** rather than a JSON string, using `.to_dict`. 
-        
-        Second, we leverage the built-in `json.dumps` to serialize our `dataclass` into 
-        a JSON string.
-        
-        **Decode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
-        response)**
-        
-        ```python
-        import json
-        
-        response_dict = json.loads('{"response": {"person": {"name": "lidatong"}}}')
-        
-        person_dict = response_dict['response']
-        
-        person = Person.from_dict(person_dict)
-        ```
-        
-        In a similar vein to encoding above, we leverage the built-in `json` module.
-        
-        First, call `json.loads` to read the entire JSON object into a 
-        dictionary. We then access the key of the value containing the encoded dict of 
-        our `Person` that we want to decode (`response_dict['response']`).
-        
-        Second, we load in the dictionary using `Person.from_dict`.
-        
-        
-        ### Encode or decode into Python lists/dictionaries rather than JSON?
-        
-        This can be by calling `.schema()` and then using the corresponding 
-        encoder/decoder methods, ie. `.load(...)`/`.dump(...)`.
-        
-        **Encode into a single Python dictionary**
-        
-        ```python
-        person = Person('lidatong')
-        person.to_dict()  # {'name': 'lidatong'}
-        ```
-        
-        **Encode into a list of Python dictionaries**
-        
-        ```python
-        people = [Person('lidatong')]
-        Person.schema().dump(people, many=True)  # [{'name': 'lidatong'}]
-        ```
-        
-        **Decode a dictionary into a single dataclass instance**
-        
-        ```python
-        person_dict = {'name': 'lidatong'}
-        Person.from_dict(person_dict)  # Person(name='lidatong')
-        ```
-        
-        **Decode a list of dictionaries into a list of dataclass instances**
-        
-        ```python
-        people_dicts = [{"name": "lidatong"}]
-        Person.schema().load(people_dicts, many=True)  # [Person(name='lidatong')]
-        ```
-        
-        ### Encode or decode from camelCase (or kebab-case)?
-        
-        JSON letter case by convention is camelCase, in Python members are by convention snake_case.
-        
-        You can configure it to encode/decode from other casing schemes at both the class level and the field level.
-        
-        ```python
-        from dataclasses import dataclass, field
-        
-        from dataclasses_json import LetterCase, config, dataclass_json
-        
-        
-        # changing casing at the class level
-        @dataclass_json(letter_case=LetterCase.CAMEL)
-        @dataclass
-        class Person:
-            given_name: str
-            family_name: str
-            
-        Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
-        Person.from_json('{"givenName": "Alice", "familyName": "Liddell"}')  # Person('Alice', 'Liddell')
-        
-        # at the field level
-        @dataclass_json
-        @dataclass
-        class Person:
-            given_name: str = field(metadata=config(letter_case=LetterCase.CAMEL))
-            family_name: str
-            
-        Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
-        # notice how the `family_name` field is still snake_case, because it wasn't configured above
-        Person.from_json('{"givenName": "Alice", "family_name": "Liddell"}')  # Person('Alice', 'Liddell')
-        ```
-        
-        **This library assumes your field follows the Python convention of snake_case naming.**
-        If your field is not `snake_case` to begin with and you attempt to parameterize `LetterCase`, 
-        the behavior of encoding/decoding is undefined (most likely it will result in subtle bugs).
-        
-        ### Encode or decode using a different name
-        
-        ```python
-        from dataclasses import dataclass, field
-        
-        from dataclasses_json import config, dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            given_name: str = field(metadata=config(field_name="overriddenGivenName"))
-        
-        Person(given_name="Alice")  # Person('Alice')
-        Person.from_json('{"overriddenGivenName": "Alice"}')  # Person('Alice')
-        Person('Alice').to_json()  # {"overriddenGivenName": "Alice"}
-        ```
-        
-        ### Handle missing or optional field values when decoding?
-        
-        By default, any fields in your dataclass that use `default` or 
-        `default_factory` will have the values filled with the provided default, if the
-        corresponding field is missing from the JSON you're decoding.
-        
-        **Decode JSON with missing field**
-        
-        ```python
-        @dataclass_json
-        @dataclass
-        class Student:
-            id: int
-            name: str = 'student'
-        
-        Student.from_json('{"id": 1}')  # Student(id=1, name='student')
-        ```
-        
-        Notice `from_json` filled the field `name` with the specified default 'student'
-        when it was missing from the JSON.
-        
-        Sometimes you have fields that are typed as `Optional`, but you don't 
-        necessarily want to assign a default. In that case, you can use the 
-        `infer_missing` kwarg to make `from_json` infer the missing field value as `None`.
-        
-        **Decode optional field without default**
-        
-        ```python
-        @dataclass_json
-        @dataclass
-        class Tutor:
-            id: int
-            student: Optional[Student] = None
-        
-        Tutor.from_json('{"id": 1}')  # Tutor(id=1, student=None)
-        ```
-        
-        Personally I recommend you leverage dataclass defaults rather than using 
-        `infer_missing`, but if for some reason you need to decouple the behavior of 
-        JSON decoding from the field's default value, this will allow you to do so.
-        
-        
-        ### Handle unknown / extraneous fields in JSON?
-        
-        By default, it is up to the implementation what happens when a `json_dataclass` receives input parameters that are not defined.
-        (the `from_dict` method ignores them, when loading using `schema()` a ValidationError is raised.)
-        There are three ways to customize this behavior.
-        
-        Assume you want to instantiate a dataclass with the following dictionary:
-        ```python
-        dump_dict = {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}, "undefined_field_name": [1, 2, 3]}
-        ```
-        
-        1. You can enforce to always raise an error by setting the `undefined` keyword to `Undefined.RAISE`
-         (`'RAISE'` as a case-insensitive string works as well). Of course it works normally if you don't pass any undefined parameters.
-            
-        ```python
-        from dataclasses_json import Undefined
-        
-        @dataclass_json(undefined=Undefined.RAISE)
-        @dataclass()
-        class ExactAPIDump:
-            endpoint: str
-            data: Dict[str, Any]
-        
-        dump = ExactAPIDump.from_dict(dump_dict)  # raises UndefinedParameterError
-        ```
-        
-        2. You can simply ignore any undefined parameters by setting the `undefined` keyword to `Undefined.EXCLUDE`
-         (`'EXCLUDE'` as a case-insensitive string works as well). Note that you will not be able to retrieve them using `to_dict`:
-            
-        ```python
-        from dataclasses_json import Undefined
-        
-        @dataclass_json(undefined=Undefined.EXCLUDE)
-        @dataclass()
-        class DontCareAPIDump:
-            endpoint: str
-            data: Dict[str, Any]
-        
-        dump = DontCareAPIDump.from_dict(dump_dict)  # DontCareAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'})
-        dump.to_dict()  # {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}}
-        ```
-        
-        3. You can save them in a catch-all field and do whatever needs to be done later. Simply set the `undefined`
-        keyword to `Undefined.INCLUDE` (`'INCLUDE'` as a case-insensitive string works as well) and define a field
-        of type `CatchAll` where all unknown values will end up.
-         This simply represents a dictionary that can hold anything. 
-         If there are no undefined parameters, this will be an empty dictionary.
-            
-        ```python
-        from dataclasses_json import Undefined, CatchAll
-        
-        @dataclass_json(undefined=Undefined.INCLUDE)
-        @dataclass()
-        class UnknownAPIDump:
-            endpoint: str
-            data: Dict[str, Any]
-            unknown_things: CatchAll
-        
-        dump = UnknownAPIDump.from_dict(dump_dict)  # UnknownAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'}, unknown_things={'undefined_field_name': [1, 2, 3]})
-        dump.to_dict()  # {'endpoint': 'some_api_endpoint', 'data': {'foo': 1, 'bar': '2'}, 'undefined_field_name': [1, 2, 3]}
-        ```
-        
-        Notes:
-        - When using `Undefined.INCLUDE`, an `UndefinedParameterError` will be raised if you don't specify
-        exactly one field of type `CatchAll`.
-        - Note that `LetterCase` does not affect values written into the `CatchAll` field, they will be as they are given.
-        - When specifying a default (or a default factory) for the the `CatchAll`-field, e.g. `unknown_things: CatchAll = None`, the default value will be used instead of an empty dict if there are no undefined parameters.
-        - Calling __init__ with non-keyword arguments resolves the arguments to the defined fields and writes everything else into the catch-all field.
-        
-        4. All 3 options work as well using `schema().loads` and `schema().dumps`, as long as you don't overwrite it by specifying `schema(unknown=<a marshmallow value>)`.
-        marshmallow uses the same 3 keywords ['include', 'exclude', 'raise'](https://marshmallow.readthedocs.io/en/stable/quickstart.html#handling-unknown-fields).
-        
-        5. All 3 operations work as well using `__init__`, e.g. `UnknownAPIDump(**dump_dict)` will **not** raise a `TypeError`, but write all unknown values to the field tagged as `CatchAll`.
-           Classes tagged with `EXCLUDE` will also simply ignore unknown parameters. Note that classes tagged as `RAISE` still raise a `TypeError`, and **not** a `UndefinedParameterError` if supplied with unknown keywords.
-        
-        
-        ### Override the default encode / decode / marshmallow field of a specific field?
-        
-        See [Overriding](#Overriding)
-        
-        ### Handle recursive dataclasses?
-        Object hierarchies where fields are of the type that they are declared within require a small
-        type hinting trick to declare the forward reference.
-        ```python
-        from typing import Optional
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Tree():
-            value: str
-            left: Optional['Tree']
-            right: Optional['Tree']
-        ```
-        
-        Avoid using
-        ```python
-        from __future__ import annotations
-        ```
-        as it will cause problems with the way dataclasses_json accesses the type annotations.
-        
-        
-        ## Marshmallow interop
-        
-        Using the `dataclass_json` decorator or mixing in `DataClassJsonMixin` will
-        provide you with an additional method `.schema()`.
-        
-        `.schema()` generates a schema exactly equivalent to manually creating a
-        marshmallow schema for your dataclass. You can reference the [marshmallow API docs](https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
-        to learn other ways you can use the schema returned by `.schema()`.
-        
-        You can pass in the exact same arguments to `.schema()` that you would when
-        constructing a `PersonSchema` instance, e.g. `.schema(many=True)`, and they will
-        get passed through to the marshmallow schema.
-        
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        @dataclass_json
-        @dataclass
-        class Person:
-            name: str
-        
-        # You don't need to do this - it's generated for you by `.schema()`!
-        from marshmallow import Schema, fields
-        
-        class PersonSchema(Schema):
-            name = fields.Str()
-        ```
-        
-        Briefly, on what's going on under the hood in the above examples: calling 
-        `.schema()` will have this library generate a
-        [marshmallow schema]('https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
-        for you. It also fills in the corresponding object hook, so that marshmallow
-        will create an instance of your Data Class on `load` (e.g.
-        `Person.schema().load` returns a `Person`) rather than a `dict`, which it does
-        by default in marshmallow.
-        
-        **Performance note**
-        
-        `.schema()` is not cached (it generates the schema on every call), so if you
-        have a nested Data Class you may want to save the result to a variable to 
-        avoid re-generation of the schema on every usage.
-        
-        ```python
-        person_schema = Person.schema()
-        person_schema.dump(people, many=True)
-        
-        # later in the code...
-        
-        person_schema.dump(person)
-        ```
-        
-        ## Overriding / Extending
-        
-        #### Overriding
-        
-        For example, you might want to encode/decode `datetime` objects using ISO format
-        rather than the default `timestamp`.
-        
-        ```python
-        from dataclasses import dataclass, field
-        from dataclasses_json import dataclass_json, config
-        from datetime import datetime
-        from marshmallow import fields
-        
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: datetime = field(
-                metadata=config(
-                    encoder=datetime.isoformat,
-                    decoder=datetime.fromisoformat,
-                    mm_field=fields.DateTime(format='iso')
-                )
-            )
-        ```
-        
-        #### Extending
-        
-        Similarly, you might want to extend `dataclasses_json` to encode `date` objects.
-        
-        ```python
-        from dataclasses import dataclass, field
-        from dataclasses_json import dataclass_json, config
-        from datetime import date
-        from marshmallow import fields
-        
-        dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
-        dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
-        
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: date
-            modified_at: date
-            accessed_at: date
-        ```
-        
-        As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
-        callable:
-        - `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
-        - `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
-        - `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
-        
-        Note that these hooks will be invoked regardless if you're using 
-        `.to_json`/`dump`/`dumps`
-        and `.from_json`/`load`/`loads`. So apply overrides / extensions judiciously, making sure to 
-        carefully consider whether the interaction of the encode/decode/mm_field is consistent with what you expect!
-        
-        
-        #### What if I have other dataclass field extensions that rely on `metadata`
-        
-        All the `dataclasses_json.config` does is return a mapping, namespaced under the key `'dataclasses_json'`.
-        
-        Say there's another module, `other_dataclass_package` that uses metadata. Here's how you solve your problem:
-        
-        ```python
-        metadata = {'other_dataclass_package': 'some metadata...'}  # pre-existing metadata for another dataclass package
-        dataclass_json_config = config(
-                    encoder=datetime.isoformat,
-                    decoder=datetime.fromisoformat,
-                    mm_field=fields.DateTime(format='iso')
-                )
-        metadata.update(dataclass_json_config)
-        
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: datetime = field(metadata=metadata)
-        ```
-        
-        You can also manually specify the dataclass_json configuration mapping.
-        
-        ```python
-        @dataclass_json
-        @dataclass
-        class DataClassWithIsoDatetime:
-            created_at: date = field(
-                metadata={'dataclasses_json': {
-                    'encoder': date.isoformat,
-                    'decoder': date.fromisoformat,
-                    'mm_field': fields.DateTime(format='iso')
-                }}
-            )
-        ```
-        
-        ## A larger example
-        
-        ```python
-        from dataclasses import dataclass
-        from dataclasses_json import dataclass_json
-        
-        from typing import List
-        
-        @dataclass_json
-        @dataclass(frozen=True)
-        class Minion:
-            name: str
-        
-        
-        @dataclass_json
-        @dataclass(frozen=True)
-        class Boss:
-            minions: List[Minion]
-        
-        boss = Boss([Minion('evil minion'), Minion('very evil minion')])
-        boss_json = """
-        {
-            "minions": [
-                {
-                    "name": "evil minion"
-                },
-                {
-                    "name": "very evil minion"
-                }
-            ]
-        }
-        """.strip()
-        
-        assert boss.to_json(indent=4) == boss_json
-        assert Boss.from_json(boss_json) == boss
-        ```
-        
-        ## Performance
-        
-        Take a look at [this issue](https://github.com/lidatong/dataclasses-json/issues/228)
-        
-        ## Versioning
-        
-        Note this library is still pre-1.0.0 (SEMVER).
-        
-        The current convention is:
-        - **PATCH** version upgrades for bug fixes and minor feature additions.
-        - **MINOR** version upgrades for big API features and breaking changes.
-        
-        Once this library is 1.0.0, it will follow standard SEMVER conventions.
-        
-        
-        ## Roadmap
-        
-        Currently the focus is on investigating and fixing bugs in this library, working
-        on performance, and finishing [this issue](https://github.com/lidatong/dataclasses-json/issues/31).
-        
-        That said, if you think there's a feature missing / something new needed in the
-        library, please see the contributing section below.
-        
-        
-        ## Contributing
-        
-        First of all, thank you for being interested in contributing to this library.
-        I really appreciate you taking the time to work on this project.
-        
-        - If you're just interested in getting into the code, a good place to start are 
-        issues tagged as bugs.
-        - If introducing a new feature, especially one that modifies the public API, 
-        consider submitting an issue for discussion before a PR. Please also take a look 
-        at existing issues / PRs to see what you're proposing has  already been covered 
-        before / exists.
-        - I like to follow the commit conventions documented [here](https://www.conventionalcommits.org/en/v1.0.0/#summary)
-        
 Keywords: dataclasses json
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Dataclasses JSON
+
+![](https://github.com/lidatong/dataclasses-json/workflows/dataclasses-json/badge.svg)
+
+This library provides a simple API for encoding and decoding [dataclasses](https://docs.python.org/3/library/dataclasses.html) to and from JSON.
+
+It's very easy to get started.
+
+[README / Documentation website](https://lidatong.github.io/dataclasses-json). Features a navigation bar and search functionality, and should mirror this README exactly -- take a look!
+
+## Quickstart
+
+`pip install dataclasses-json`
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+
+
+person = Person(name='lidatong')
+person.to_json()  # '{"name": "lidatong"}' <- this is a string
+person.to_dict()  # {'name': 'lidatong'} <- this is a dict
+Person.from_json('{"name": "lidatong"}')  # Person(1)
+Person.from_dict({'name': 'lidatong'})  # Person(1)
+
+# You can also apply _schema validation_ using an alternative API
+# This can be useful for "typed" Python code
+
+Person.from_json('{"name": 42}')  # This is ok. 42 is not a `str`, but
+                                  # dataclass creation does not validate types
+Person.schema().loads('{"name": 42}')  # Error! Raises `ValidationError`
+```
+
+**What if you want to work with camelCase JSON?**
+
+```python
+# same imports as above, with the additional `LetterCase` import
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json, LetterCase
+
+@dataclass_json(letter_case=LetterCase.CAMEL)  # now all fields are encoded/decoded from camelCase
+@dataclass
+class ConfiguredSimpleExample:
+    int_field: int
+
+ConfiguredSimpleExample(1).to_json()  # {"intField": 1}
+ConfiguredSimpleExample.from_json('{"intField": 1}')  # ConfiguredSimpleExample(1)
+```
+
+## Supported types
+
+It's recursive (see caveats below), so you can easily work with nested dataclasses.
+In addition to the supported types in the 
+[py to JSON table](https://docs.python.org/3/library/json.html#py-to-json-table), this library supports the following:
+
+- any arbitrary [Collection](https://docs.python.org/3/library/collections.abc.html#collections.abc.Collection) type is supported.
+[Mapping](https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping) types are encoded as JSON objects and `str` types as JSON strings. 
+Any other Collection types are encoded into JSON arrays, but decoded into the original collection types.
+
+- [datetime](https://docs.python.org/3/library/datetime.html#available-types) 
+objects. `datetime` objects are encoded to `float` (JSON number) using 
+[timestamp](https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp).
+As specified in the `datetime` docs, if your `datetime` object is naive, it will 
+assume your system local timezone when calling `.timestamp()`. JSON numbers 
+corresponding to a `datetime` field in your dataclass are decoded 
+into a datetime-aware object, with `tzinfo` set to your system local timezone.
+Thus, if you encode a datetime-naive object, you will decode into a 
+datetime-aware object. This is important, because encoding and decoding won't 
+strictly be inverses. See [this section](#Overriding) if you want to override this default
+behavior (for example, if you want to use ISO).
+
+- [UUID](https://docs.python.org/3/library/uuid.html#uuid.UUID) objects. They 
+are encoded as `str` (JSON string).
+
+- [Decimal](https://docs.python.org/3/library/decimal.html) objects. They are
+also encoded as `str`.
+
+**The [latest release](https://github.com/lidatong/dataclasses-json/releases/latest) is compatible with both Python 3.7 and Python 3.6 (with the dataclasses backport).**
+
+## Usage
+
+#### Approach 1: Class decorator
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+
+lidatong = Person('lidatong')
+
+# Encoding to JSON
+lidatong.to_json()  # '{"name": "lidatong"}'
+
+# Decoding from JSON
+Person.from_json('{"name": "lidatong"}')  # Person(name='lidatong')
+```
+
+Note that the `@dataclass_json` decorator must be stacked above the `@dataclass`
+decorator (order matters!)
+
+#### Approach 2: Inherit from a mixin
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import DataClassJsonMixin
+
+@dataclass
+class Person(DataClassJsonMixin):
+    name: str
+
+lidatong = Person('lidatong')
+
+# A different example from Approach 1 above, but usage is the exact same
+assert Person.from_json(lidatong.to_json()) == lidatong
+```
+
+Pick whichever approach suits your taste. Note that there is better support for
+ the mixin approach when using _static analysis_ tools (e.g. linting, typing),
+ but the differences in implementation will be invisible in _runtime_ usage.
+
+## How do I...
+
+
+
+### Use my dataclass with JSON arrays or objects?
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+```
+
+**Encode into a JSON array containing instances of my Data Class**
+
+```python
+people_json = [Person('lidatong')]
+Person.schema().dumps(people_json, many=True)  # '[{"name": "lidatong"}]'
+```
+
+**Decode a JSON array containing instances of my Data Class**
+
+```python
+people_json = '[{"name": "lidatong"}]'
+Person.schema().loads(people_json, many=True)  # [Person(name='lidatong')]
+```
+
+**Encode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
+request/response)**
+
+```python
+import json
+
+response_dict = {
+    'response': {
+        'person': Person('lidatong').to_dict()
+    }
+}
+
+response_json = json.dumps(response_dict)
+```
+
+In this case, we do two steps. First, we encode the dataclass into a 
+**python dictionary** rather than a JSON string, using `.to_dict`. 
+
+Second, we leverage the built-in `json.dumps` to serialize our `dataclass` into 
+a JSON string.
+
+**Decode as part of a larger JSON object containing my Data Class (e.g. an HTTP 
+response)**
+
+```python
+import json
+
+response_dict = json.loads('{"response": {"person": {"name": "lidatong"}}}')
+
+person_dict = response_dict['response']
+
+person = Person.from_dict(person_dict)
+```
+
+In a similar vein to encoding above, we leverage the built-in `json` module.
+
+First, call `json.loads` to read the entire JSON object into a 
+dictionary. We then access the key of the value containing the encoded dict of 
+our `Person` that we want to decode (`response_dict['response']`).
+
+Second, we load in the dictionary using `Person.from_dict`.
+
+
+### Encode or decode into Python lists/dictionaries rather than JSON?
+
+This can be by calling `.schema()` and then using the corresponding 
+encoder/decoder methods, ie. `.load(...)`/`.dump(...)`.
+
+**Encode into a single Python dictionary**
+
+```python
+person = Person('lidatong')
+person.to_dict()  # {'name': 'lidatong'}
+```
+
+**Encode into a list of Python dictionaries**
+
+```python
+people = [Person('lidatong')]
+Person.schema().dump(people, many=True)  # [{'name': 'lidatong'}]
+```
+
+**Decode a dictionary into a single dataclass instance**
+
+```python
+person_dict = {'name': 'lidatong'}
+Person.from_dict(person_dict)  # Person(name='lidatong')
+```
+
+**Decode a list of dictionaries into a list of dataclass instances**
+
+```python
+people_dicts = [{"name": "lidatong"}]
+Person.schema().load(people_dicts, many=True)  # [Person(name='lidatong')]
+```
+
+### Encode or decode from camelCase (or kebab-case)?
+
+JSON letter case by convention is camelCase, in Python members are by convention snake_case.
+
+You can configure it to encode/decode from other casing schemes at both the class level and the field level.
+
+```python
+from dataclasses import dataclass, field
+
+from dataclasses_json import LetterCase, config, dataclass_json
+
+
+# changing casing at the class level
+@dataclass_json(letter_case=LetterCase.CAMEL)
+@dataclass
+class Person:
+    given_name: str
+    family_name: str
+    
+Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
+Person.from_json('{"givenName": "Alice", "familyName": "Liddell"}')  # Person('Alice', 'Liddell')
+
+# at the field level
+@dataclass_json
+@dataclass
+class Person:
+    given_name: str = field(metadata=config(letter_case=LetterCase.CAMEL))
+    family_name: str
+    
+Person('Alice', 'Liddell').to_json()  # '{"givenName": "Alice"}'
+# notice how the `family_name` field is still snake_case, because it wasn't configured above
+Person.from_json('{"givenName": "Alice", "family_name": "Liddell"}')  # Person('Alice', 'Liddell')
+```
+
+**This library assumes your field follows the Python convention of snake_case naming.**
+If your field is not `snake_case` to begin with and you attempt to parameterize `LetterCase`, 
+the behavior of encoding/decoding is undefined (most likely it will result in subtle bugs).
+
+### Encode or decode using a different name
+
+```python
+from dataclasses import dataclass, field
+
+from dataclasses_json import config, dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    given_name: str = field(metadata=config(field_name="overriddenGivenName"))
+
+Person(given_name="Alice")  # Person('Alice')
+Person.from_json('{"overriddenGivenName": "Alice"}')  # Person('Alice')
+Person('Alice').to_json()  # {"overriddenGivenName": "Alice"}
+```
+
+### Handle missing or optional field values when decoding?
+
+By default, any fields in your dataclass that use `default` or 
+`default_factory` will have the values filled with the provided default, if the
+corresponding field is missing from the JSON you're decoding.
+
+**Decode JSON with missing field**
+
+```python
+@dataclass_json
+@dataclass
+class Student:
+    id: int
+    name: str = 'student'
+
+Student.from_json('{"id": 1}')  # Student(id=1, name='student')
+```
+
+Notice `from_json` filled the field `name` with the specified default 'student'
+when it was missing from the JSON.
+
+Sometimes you have fields that are typed as `Optional`, but you don't 
+necessarily want to assign a default. In that case, you can use the 
+`infer_missing` kwarg to make `from_json` infer the missing field value as `None`.
+
+**Decode optional field without default**
+
+```python
+@dataclass_json
+@dataclass
+class Tutor:
+    id: int
+    student: Optional[Student] = None
+
+Tutor.from_json('{"id": 1}')  # Tutor(id=1, student=None)
+```
+
+Personally I recommend you leverage dataclass defaults rather than using 
+`infer_missing`, but if for some reason you need to decouple the behavior of 
+JSON decoding from the field's default value, this will allow you to do so.
+
+
+### Handle unknown / extraneous fields in JSON?
+
+By default, it is up to the implementation what happens when a `json_dataclass` receives input parameters that are not defined.
+(the `from_dict` method ignores them, when loading using `schema()` a ValidationError is raised.)
+There are three ways to customize this behavior.
+
+Assume you want to instantiate a dataclass with the following dictionary:
+```python
+dump_dict = {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}, "undefined_field_name": [1, 2, 3]}
+```
+
+1. You can enforce to always raise an error by setting the `undefined` keyword to `Undefined.RAISE`
+ (`'RAISE'` as a case-insensitive string works as well). Of course it works normally if you don't pass any undefined parameters.
+    
+```python
+from dataclasses_json import Undefined
+
+@dataclass_json(undefined=Undefined.RAISE)
+@dataclass()
+class ExactAPIDump:
+    endpoint: str
+    data: Dict[str, Any]
+
+dump = ExactAPIDump.from_dict(dump_dict)  # raises UndefinedParameterError
+```
+
+2. You can simply ignore any undefined parameters by setting the `undefined` keyword to `Undefined.EXCLUDE`
+ (`'EXCLUDE'` as a case-insensitive string works as well). Note that you will not be able to retrieve them using `to_dict`:
+    
+```python
+from dataclasses_json import Undefined
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclass()
+class DontCareAPIDump:
+    endpoint: str
+    data: Dict[str, Any]
+
+dump = DontCareAPIDump.from_dict(dump_dict)  # DontCareAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'})
+dump.to_dict()  # {"endpoint": "some_api_endpoint", "data": {"foo": 1, "bar": "2"}}
+```
+
+3. You can save them in a catch-all field and do whatever needs to be done later. Simply set the `undefined`
+keyword to `Undefined.INCLUDE` (`'INCLUDE'` as a case-insensitive string works as well) and define a field
+of type `CatchAll` where all unknown values will end up.
+ This simply represents a dictionary that can hold anything. 
+ If there are no undefined parameters, this will be an empty dictionary.
+    
+```python
+from dataclasses_json import Undefined, CatchAll
+
+@dataclass_json(undefined=Undefined.INCLUDE)
+@dataclass()
+class UnknownAPIDump:
+    endpoint: str
+    data: Dict[str, Any]
+    unknown_things: CatchAll
+
+dump = UnknownAPIDump.from_dict(dump_dict)  # UnknownAPIDump(endpoint='some_api_endpoint', data={'foo': 1, 'bar': '2'}, unknown_things={'undefined_field_name': [1, 2, 3]})
+dump.to_dict()  # {'endpoint': 'some_api_endpoint', 'data': {'foo': 1, 'bar': '2'}, 'undefined_field_name': [1, 2, 3]}
+```
+
+Notes:
+- When using `Undefined.INCLUDE`, an `UndefinedParameterError` will be raised if you don't specify
+exactly one field of type `CatchAll`.
+- Note that `LetterCase` does not affect values written into the `CatchAll` field, they will be as they are given.
+- When specifying a default (or a default factory) for the the `CatchAll`-field, e.g. `unknown_things: CatchAll = None`, the default value will be used instead of an empty dict if there are no undefined parameters.
+- Calling __init__ with non-keyword arguments resolves the arguments to the defined fields and writes everything else into the catch-all field.
+
+4. All 3 options work as well using `schema().loads` and `schema().dumps`, as long as you don't overwrite it by specifying `schema(unknown=<a marshmallow value>)`.
+marshmallow uses the same 3 keywords ['include', 'exclude', 'raise'](https://marshmallow.readthedocs.io/en/stable/quickstart.html#handling-unknown-fields).
+
+5. All 3 operations work as well using `__init__`, e.g. `UnknownAPIDump(**dump_dict)` will **not** raise a `TypeError`, but write all unknown values to the field tagged as `CatchAll`.
+   Classes tagged with `EXCLUDE` will also simply ignore unknown parameters. Note that classes tagged as `RAISE` still raise a `TypeError`, and **not** a `UndefinedParameterError` if supplied with unknown keywords.
+
+
+### Override the default encode / decode / marshmallow field of a specific field?
+
+See [Overriding](#Overriding)
+
+### Handle recursive dataclasses?
+Object hierarchies where fields are of the type that they are declared within require a small
+type hinting trick to declare the forward reference.
+```python
+from typing import Optional
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Tree():
+    value: str
+    left: Optional['Tree']
+    right: Optional['Tree']
+```
+
+Avoid using
+```python
+from __future__ import annotations
+```
+as it will cause problems with the way dataclasses_json accesses the type annotations.
+
+
+## Marshmallow interop
+
+Using the `dataclass_json` decorator or mixing in `DataClassJsonMixin` will
+provide you with an additional method `.schema()`.
+
+`.schema()` generates a schema exactly equivalent to manually creating a
+marshmallow schema for your dataclass. You can reference the [marshmallow API docs](https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
+to learn other ways you can use the schema returned by `.schema()`.
+
+You can pass in the exact same arguments to `.schema()` that you would when
+constructing a `PersonSchema` instance, e.g. `.schema(many=True)`, and they will
+get passed through to the marshmallow schema.
+
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+@dataclass_json
+@dataclass
+class Person:
+    name: str
+
+# You don't need to do this - it's generated for you by `.schema()`!
+from marshmallow import Schema, fields
+
+class PersonSchema(Schema):
+    name = fields.Str()
+```
+
+Briefly, on what's going on under the hood in the above examples: calling 
+`.schema()` will have this library generate a
+[marshmallow schema]('https://marshmallow.readthedocs.io/en/3.0/api_reference.html#schema)
+for you. It also fills in the corresponding object hook, so that marshmallow
+will create an instance of your Data Class on `load` (e.g.
+`Person.schema().load` returns a `Person`) rather than a `dict`, which it does
+by default in marshmallow.
+
+**Performance note**
+
+`.schema()` is not cached (it generates the schema on every call), so if you
+have a nested Data Class you may want to save the result to a variable to 
+avoid re-generation of the schema on every usage.
+
+```python
+person_schema = Person.schema()
+person_schema.dump(people, many=True)
+
+# later in the code...
+
+person_schema.dump(person)
+```
+
+## Overriding / Extending
+
+#### Overriding
+
+For example, you might want to encode/decode `datetime` objects using ISO format
+rather than the default `timestamp`.
+
+```python
+from dataclasses import dataclass, field
+from dataclasses_json import dataclass_json, config
+from datetime import datetime
+from marshmallow import fields
+
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: datetime = field(
+        metadata=config(
+            encoder=datetime.isoformat,
+            decoder=datetime.fromisoformat,
+            mm_field=fields.DateTime(format='iso')
+        )
+    )
+```
+
+#### Extending
+
+Similarly, you might want to extend `dataclasses_json` to encode `date` objects.
+
+```python
+from dataclasses import dataclass, field
+from dataclasses_json import dataclass_json, config
+from datetime import date
+from marshmallow import fields
+
+dataclasses_json.cfg.global_config.encoders[date] = date.isoformat
+dataclasses_json.cfg.global_config.decoders[date] = date.fromisoformat
+
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: date
+    modified_at: date
+    accessed_at: date
+```
+
+As you can see, you can **override** or **extend** the default codecs by providing a "hook" via a 
+callable:
+- `encoder`: a callable, which will be invoked to convert the field value when encoding to JSON
+- `decoder`: a callable, which will be invoked to convert the JSON value when decoding from JSON
+- `mm_field`: a marshmallow field, which will affect the behavior of any operations involving `.schema()`
+
+Note that these hooks will be invoked regardless if you're using 
+`.to_json`/`dump`/`dumps`
+and `.from_json`/`load`/`loads`. So apply overrides / extensions judiciously, making sure to 
+carefully consider whether the interaction of the encode/decode/mm_field is consistent with what you expect!
+
+
+#### What if I have other dataclass field extensions that rely on `metadata`
+
+All the `dataclasses_json.config` does is return a mapping, namespaced under the key `'dataclasses_json'`.
+
+Say there's another module, `other_dataclass_package` that uses metadata. Here's how you solve your problem:
+
+```python
+metadata = {'other_dataclass_package': 'some metadata...'}  # pre-existing metadata for another dataclass package
+dataclass_json_config = config(
+            encoder=datetime.isoformat,
+            decoder=datetime.fromisoformat,
+            mm_field=fields.DateTime(format='iso')
+        )
+metadata.update(dataclass_json_config)
+
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: datetime = field(metadata=metadata)
+```
+
+You can also manually specify the dataclass_json configuration mapping.
+
+```python
+@dataclass_json
+@dataclass
+class DataClassWithIsoDatetime:
+    created_at: date = field(
+        metadata={'dataclasses_json': {
+            'encoder': date.isoformat,
+            'decoder': date.fromisoformat,
+            'mm_field': fields.DateTime(format='iso')
+        }}
+    )
+```
+
+## A larger example
+
+```python
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
+
+from typing import List
+
+@dataclass_json
+@dataclass(frozen=True)
+class Minion:
+    name: str
+
+
+@dataclass_json
+@dataclass(frozen=True)
+class Boss:
+    minions: List[Minion]
+
+boss = Boss([Minion('evil minion'), Minion('very evil minion')])
+boss_json = """
+{
+    "minions": [
+        {
+            "name": "evil minion"
+        },
+        {
+            "name": "very evil minion"
+        }
+    ]
+}
+""".strip()
+
+assert boss.to_json(indent=4) == boss_json
+assert Boss.from_json(boss_json) == boss
+```
+
+## Performance
+
+Take a look at [this issue](https://github.com/lidatong/dataclasses-json/issues/228)
+
+## Versioning
+
+Note this library is still pre-1.0.0 (SEMVER).
+
+The current convention is:
+- **PATCH** version upgrades for bug fixes and minor feature additions.
+- **MINOR** version upgrades for big API features and breaking changes.
+
+Once this library is 1.0.0, it will follow standard SEMVER conventions.
+
+
+## Roadmap
+
+Currently the focus is on investigating and fixing bugs in this library, working
+on performance, and finishing [this issue](https://github.com/lidatong/dataclasses-json/issues/31).
+
+That said, if you think there's a feature missing / something new needed in the
+library, please see the contributing section below.
+
+
+## Contributing
+
+First of all, thank you for being interested in contributing to this library.
+I really appreciate you taking the time to work on this project.
+
+- If you're just interested in getting into the code, a good place to start are 
+issues tagged as bugs.
+- If introducing a new feature, especially one that modifies the public API, 
+consider submitting an issue for discussion before a PR. Please also take a look 
+at existing issues / PRs to see what you're proposing has  already been covered 
+before / exists.
+- I like to follow the commit conventions documented [here](https://www.conventionalcommits.org/en/v1.0.0/#summary)
```

### Comparing `dataclasses-json-0.5.8/dataclasses_json.egg-info/SOURCES.txt` & `dataclasses-json-0.5.9/dataclasses_json.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 dataclasses_json.egg-info/PKG-INFO
 dataclasses_json.egg-info/SOURCES.txt
 dataclasses_json.egg-info/dependency_links.txt
 dataclasses_json.egg-info/requires.txt
 dataclasses_json.egg-info/top_level.txt
 tests/test_annotations.py
 tests/test_api.py
+tests/test_builtins.py
 tests/test_collections.py
 tests/test_dict.py
 tests/test_enum.py
 tests/test_examples.py
 tests/test_exclude.py
 tests/test_global_config.py
 tests/test_invariants.py
 tests/test_letter_case.py
 tests/test_metadata.py
 tests/test_nested.py
 tests/test_recursive.py
 tests/test_schema.py
+tests/test_str_subclass.py
 tests/test_time.py
 tests/test_undefined_parameters.py
 tests/test_union.py
 tests/test_unsupported_generics.py
```

### Comparing `dataclasses-json-0.5.8/publish.py` & `dataclasses-json-0.5.9/publish.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/setup.py` & `dataclasses-json-0.5.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as f:
     readme = f.read()
 
 setup(
     name='dataclasses-json',
-    version='0.5.8',
+    version='0.5.9',
     packages=find_packages(exclude=('tests*',)),
     package_data={"dataclasses_json": ["py.typed"]},
     author='lidatong',
     author_email='charles.dt.li@gmail.com',
     description='Easily serialize dataclasses to and from JSON',
     long_description=readme,
     long_description_content_type='text/markdown',
@@ -28,14 +28,19 @@
             'pytest>=7.2.0',
             'ipython',
             'mypy>=0.710',
             'hypothesis',
             'portray',
             'flake8',
             'types-dataclasses;python_version=="3.6"',
-            'simplejson'
+            'simplejson',
+            'setuptools',
+            'wheel',
+            'twine'
         ]
     },
     include_package_data=True,
     scripts=['publish.py']
 )
 
+
+
```

### Comparing `dataclasses-json-0.5.8/tests/test_annotations.py` & `dataclasses-json-0.5.9/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_api.py` & `dataclasses-json-0.5.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_collections.py` & `dataclasses-json-0.5.9/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_dict.py` & `dataclasses-json-0.5.9/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_enum.py` & `dataclasses-json-0.5.9/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_examples.py` & `dataclasses-json-0.5.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_exclude.py` & `dataclasses-json-0.5.9/tests/test_exclude.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_global_config.py` & `dataclasses-json-0.5.9/tests/test_global_config.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_invariants.py` & `dataclasses-json-0.5.9/tests/test_invariants.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from tests.hypothesis2.strategies import deques, optionals
 
 dcconss_strategies_conss = [(DataClassWithList, lists, list),
                             (DataClassWithSet, sets, set),
                             (DataClassWithTuple, tuples, tuple),
                             (DataClassWithFrozenSet, frozensets, frozenset),
                             (DataClassWithDeque, deques, deque),
-                            (DataClassWithOptional, optionals, lambda x: x)]
+                            (DataClassWithOptional, optionals, lambda x: x[0])]
 example_input = [1]
 
 
 @given(one_of(*[strategy_fn(integers()).map(dccons)
                 for dccons, strategy_fn, _ in dcconss_strategies_conss]))
 @examples(*[dccons(cons(example_input))
             for dccons, _, cons in dcconss_strategies_conss])
```

### Comparing `dataclasses-json-0.5.8/tests/test_letter_case.py` & `dataclasses-json-0.5.9/tests/test_letter_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     given_name: str = field(metadata=config(field_name='givenName'))
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class CamelCasePersonWithOverride:
     given_name: str
-    years_on_earth: str = field(metadata=config(field_name='age'))
+    years_on_earth: int = field(metadata=config(field_name='age'))
 
 
 class TestLetterCase:
     def test_camel_encode(self):
         assert CamelCasePerson('Alice').to_json() == '{"givenName": "Alice"}'
 
     def test_camel_decode(self):
```

### Comparing `dataclasses-json-0.5.8/tests/test_metadata.py` & `dataclasses-json-0.5.9/tests/test_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 from dataclasses import dataclass, field
+from typing import Optional
 
 import pytest
 from marshmallow import fields, ValidationError
 
 from dataclasses_json import DataClassJsonMixin
 
 
@@ -19,23 +20,43 @@
 class StringDate(DataClassJsonMixin):
     string_date: datetime.datetime = field(
         metadata={'dataclasses_json': {
             'encoder': str,
             'decoder': str,
             'mm_field': fields.String(required=False)}
         })
+    
+@dataclass
+class OptionalStringDate(DataClassJsonMixin):
+    string_date: Optional[datetime.datetime] = field(
+        default=None,
+        metadata={'dataclasses_json': {
+            'encoder': str,
+            'decoder': str,
+            'mm_field': fields.String(required=False)}
+        })
 
 
 car_schema = Car.schema()
 string_date_schema = StringDate.schema()
+opt_string_date_schema = OptionalStringDate.schema()
 
 
 class TestMetadata:
     def test_validation_error_raises(self):
         with pytest.raises(ValidationError) as e:
             car_schema.load({'license_number': 123})
         assert e.value.messages == {'license_number': ['Not a valid string.']}
 
     def test_mm_field_takes_precedence_over_types(self):
         obj = string_date_schema.load({'string_date': 'yesterday'})
         assert isinstance(obj, StringDate)
         assert obj.string_date == 'yesterday'
+
+    def test_optional_field_only_decoded_when_present(self):
+        obj = opt_string_date_schema.load({})
+        assert isinstance(obj, OptionalStringDate)
+        assert obj.string_date == None
+        
+        another_obj = opt_string_date_schema.load({'string_date': 'today'})
+        assert isinstance(another_obj, OptionalStringDate)
+        assert another_obj.string_date == 'today'
```

### Comparing `dataclasses-json-0.5.8/tests/test_nested.py` & `dataclasses-json-0.5.9/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_recursive.py` & `dataclasses-json-0.5.9/tests/test_recursive.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_schema.py` & `dataclasses-json-0.5.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_time.py` & `dataclasses-json-0.5.9/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_undefined_parameters.py` & `dataclasses-json-0.5.9/tests/test_undefined_parameters.py`

 * *Files identical despite different names*

### Comparing `dataclasses-json-0.5.8/tests/test_union.py` & `dataclasses-json-0.5.9/tests/test_union.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,14 +69,55 @@
 
 @dataclass_json
 @dataclass
 class C9:
     f1: List[Union[Aux1, Aux2]]
 
 
+try:
+    @dataclass_json
+    @dataclass
+    class C10:
+        """
+         Use py3.10+ pipe notation for optionals
+         Check if passing None as the first type option doesn't break type resolution
+
+         Instantiate with None default so NoneType is returned for runtime field value type.
+        """
+        f1: None | str = None
+except TypeError:
+    @dataclass_json
+    @dataclass
+    class C10:
+        """
+         Replace test case on versions prior to 3.10
+        """
+        f1: Union[None, str] = None
+
+
+try:
+    @dataclass_json
+    @dataclass
+    class C11:
+        """
+         Use py3.10+ pipe notation for optionals
+         Check if passing None as the second type option doesn't break type resolution
+
+         Instantiate with None default so NoneType is returned for runtime field value type.
+        """
+        f1: str | None = None
+except TypeError:
+    @dataclass_json
+    @dataclass
+    class C11:
+        """
+         Replace test case on versions prior to 3.10
+        """
+        f1: Union[str, None] = None
+
 params = [
     (C1(f1=12), {"f1": 12}, '{"f1": 12}'),
     (C1(f1="str1"), {"f1": "str1"}, '{"f1": "str1"}'),
 
     (C2(f1=10), {"f1": 10}, '{"f1": 10}'),
     (C2(f1={"str1": 0.12}), {"f1": {"str1": 0.12}}, '{"f1": {"str1": 0.12}}'),
 
@@ -102,15 +143,20 @@
 
     (C8({"str1": Aux1(12), "str2": Aux2("str3")}),
      {"f1": {"str1": {"f1": 12, "__type": "Aux1"}, "str2": {"f1": "str3", "__type": "Aux2"}}},
      '{"f1": {"str1": {"f1": 12, "__type": "Aux1"}, "str2": {"f1": "str3", "__type": "Aux2"}}}'),
 
     (C9([Aux1(12), Aux2("str3")]),
      {"f1": [{"f1": 12, "__type": "Aux1"}, {"f1": "str3", "__type": "Aux2"}]},
-     '{"f1": [{"f1": 12, "__type": "Aux1"}, {"f1": "str3", "__type": "Aux2"}]}')
+     '{"f1": [{"f1": 12, "__type": "Aux1"}, {"f1": "str3", "__type": "Aux2"}]}'),
+
+    (C10(f1=None), {"f1": None}, '{"f1": null}'),
+    (C10(f1='str1'), {"f1": 'str1'}, '{"f1": "str1"}'),
+
+    (C11(f1=None), {"f1": None}, '{"f1": null}')
 ]
 
 
 @pytest.mark.parametrize('obj, expected, expected_json', params)
 def test_serialize(obj, expected, expected_json):
     s = obj.schema()
     assert s.dump(obj) == expected
```

### Comparing `dataclasses-json-0.5.8/tests/test_unsupported_generics.py` & `dataclasses-json-0.5.9/tests/test_unsupported_generics.py`

 * *Files identical despite different names*

