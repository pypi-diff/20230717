# Comparing `tmp/easyconfig-0.2.8.tar.gz` & `tmp/easyconfig-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyconfig-0.2.8.tar", last modified: Wed Feb  8 12:52:22 2023, max compression
+gzip compressed data, was "easyconfig-0.3.0.tar", last modified: Mon Jul 17 13:55:55 2023, max compression
```

## Comparing `easyconfig-0.2.8.tar` & `easyconfig-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 12:52:11.000000 easyconfig-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-08 12:52:11.000000 easyconfig-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-02-08 12:52:22.954873 easyconfig-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-08 12:52:11.000000 easyconfig-0.2.8/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 12:52:22.954873 easyconfig-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-02-08 12:52:11.000000 easyconfig-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.950873 easyconfig-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/src/easyconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/__const__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/src/easyconfig/config_objs/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/config_objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/config_objs/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/config_objs/object_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/config_objs/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/create_app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/src/easyconfig/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/errors/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/errors/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/src/easyconfig/models/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/models/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/models/convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/src/easyconfig/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/yaml/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/yaml/from_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-08 12:52:11.000000 easyconfig-0.2.8/src/easyconfig/yaml/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/src/easyconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-02-08 12:52:22.000000 easyconfig-0.2.8/src/easyconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-08 12:52:22.000000 easyconfig-0.2.8/src/easyconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 12:52:22.000000 easyconfig-0.2.8/src/easyconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-08 12:52:22.000000 easyconfig-0.2.8/src/easyconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-08 12:52:22.000000 easyconfig-0.2.8/src/easyconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 12:52:22.954873 easyconfig-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-08 12:52:11.000000 easyconfig-0.2.8/tests/test_app_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.718987 easyconfig-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 13:55:39.000000 easyconfig-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 13:55:39.000000 easyconfig-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-17 13:55:55.718987 easyconfig-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 13:55:39.000000 easyconfig-0.3.0/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:55:55.718987 easyconfig-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-17 13:55:39.000000 easyconfig-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.710986 easyconfig-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.714987 easyconfig-0.3.0/src/easyconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/__const__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.714987 easyconfig-0.3.0/src/easyconfig/config_objs/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/config_objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/config_objs/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/config_objs/object_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/config_objs/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/create_app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.714987 easyconfig-0.3.0/src/easyconfig/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/errors/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/errors/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.714987 easyconfig-0.3.0/src/easyconfig/expansion/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/expansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/expansion/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/expansion/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/expansion/load_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/expansion/location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.718987 easyconfig-0.3.0/src/easyconfig/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/models/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.718987 easyconfig-0.3.0/src/easyconfig/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/yaml/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/yaml/from_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-17 13:55:39.000000 easyconfig-0.3.0/src/easyconfig/yaml/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.714987 easyconfig-0.3.0/src/easyconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-17 13:55:55.000000 easyconfig-0.3.0/src/easyconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-17 13:55:55.000000 easyconfig-0.3.0/src/easyconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:55:55.000000 easyconfig-0.3.0/src/easyconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 13:55:55.000000 easyconfig-0.3.0/src/easyconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 13:55:55.000000 easyconfig-0.3.0/src/easyconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:55.718987 easyconfig-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-17 13:55:39.000000 easyconfig-0.3.0/tests/test_app_creation.py
```

### Comparing `easyconfig-0.2.8/LICENSE` & `easyconfig-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyconfig-0.2.8/setup.py` & `easyconfig-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `easyconfig-0.2.8/src/easyconfig/config_objs/object_config.py` & `easyconfig-0.3.0/src/easyconfig/config_objs/object_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from inspect import getmembers, isfunction
-from typing import Any, Callable, Dict, List, Tuple, Type, TYPE_CHECKING, TypeVar, Union
+from typing import Any, Callable, Dict, Final, List, Tuple, Type, TYPE_CHECKING, TypeVar, Union
 
 from pydantic import BaseModel
-from pydantic.fields import ModelField
-from typing_extensions import Final
+from pydantic.fields import FieldInfo
 
 from easyconfig import AppConfigMixin
 from easyconfig.__const__ import MISSING, MISSING_TYPE
 from easyconfig.config_objs import ConfigObjSubscription, SubscriptionParent
 from easyconfig.errors import DuplicateSubscriptionError, FunctionCallNotAllowedError
 
 if TYPE_CHECKING:
@@ -26,15 +25,15 @@
                  path: Tuple[str, ...] = ('__root__', ),
                  parent: Union[MISSING_TYPE, HINT_CONFIG_OBJ] = MISSING):
 
         self._obj_parent: Final = parent
         self._obj_path: Final = path
 
         self._obj_model_class: Final = model.__class__
-        self._obj_model_fields: Dict[str, ModelField] = model.__fields__
+        self._obj_model_fields: Dict[str, FieldInfo] = model.model_fields
         self._obj_model_private_attrs: List[str] = list(model.__private_attributes__.keys())
 
         self._obj_keys: Tuple[str, ...] = ()
         self._obj_values: Dict[str, Any] = {}
         self._obj_children: Dict[str, Union[HINT_CONFIG_OBJ, Tuple[HINT_CONFIG_OBJ, ...]]] = {}
 
         self._obj_subscriptions: List[SubscriptionParent] = []
@@ -149,24 +148,33 @@
     #     return getattr(self._last_model, item)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Match class signature with the Mixin Classes
     # ------------------------------------------------------------------------------------------------------------------
     def subscribe_for_changes(self, func: Callable[[], Any], propagate: bool = False, on_next_load: bool = True) \
             -> 'easyconfig.config_objs.ConfigObjSubscription':
+        """When a value in this container changes the passed function will be called.
+
+        :param func: function which will be called
+        :param propagate: Propagate the change event to the parent object
+        :param on_next_load: Call the function the next time when values get loaded even if there is no value change
+        :return: object which can be used to cancel the subscription
+        """
 
         target = f'{func.__name__} @ {self._full_obj_path}'
         for sub in self._obj_subscriptions:
             if sub.func is func:
                 raise DuplicateSubscriptionError(f'{target} is already subscribed!')
 
         sub = SubscriptionParent(func, self, propagate=propagate, on_next=on_next_load)
         self._obj_subscriptions.append(sub)
         return ConfigObjSubscription(sub, target)
 
+
+
     @classmethod
     def parse_obj(cls, *args, **kwargs):
         raise FunctionCallNotAllowedError()
 
     @classmethod
     def parse_raw(cls, *args, **kwargs):
         raise FunctionCallNotAllowedError()
```

### Comparing `easyconfig-0.2.8/src/easyconfig/config_objs/subscription.py` & `easyconfig-0.3.0/src/easyconfig/config_objs/subscription.py`

 * *Files identical despite different names*

### Comparing `easyconfig-0.2.8/src/easyconfig/create_app_config.py` & `easyconfig-0.3.0/src/easyconfig/create_app_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 from easyconfig.config_objs.app_config import AppConfig, yaml_rt
 from easyconfig.errors import ExtraKwArgsNotAllowedError
 
 TYPE_WRAPPED = TypeVar('TYPE_WRAPPED', bound=BaseModel)
 TYPE_DEFAULTS = Union[BaseModel, Dict[str, Any]]
 
 
+# noinspection PyProtectedMember
 def check_field_args(model: AppConfig, allowed: FrozenSet[str]):
     """Check extra args of pydantic fields"""
 
     # Model fields
     for name, field in model._obj_model_fields.items():
-        if not set(field.field_info.extra).issubset(allowed):
-            forbidden = sorted(set(field.field_info.extra) - allowed)
+        if (extras := field.json_schema_extra) is None:
+            continue
+        if not set(extras).issubset(allowed):
+            forbidden = sorted(set(extras) - allowed)
             raise ExtraKwArgsNotAllowedError(
                 f'Extra kwargs for field "{name}" of {model._last_model.__class__.__name__} are not allowed: '
                 f'{", ".join(forbidden)}'
             )
 
     # Submodels
     for sub_model in model._obj_children.values():
@@ -67,10 +70,10 @@
     if check_field_extra_args is not None:
         check_field_args(app_cfg, frozenset(check_field_extra_args))
 
     # validate the default file
     if file_values is not None and validate_file_values:
         _yaml = app_cfg.generate_default_yaml()
         _dict = yaml_rt.load(_yaml)
-        model.__class__.parse_obj(_dict)
+        model.__class__.model_validate(_dict)
 
     return app_cfg
```

### Comparing `easyconfig-0.2.8/src/easyconfig/models/config.py` & `easyconfig-0.3.0/src/easyconfig/models/config.py`

 * *Files identical despite different names*

### Comparing `easyconfig-0.2.8/src/easyconfig/yaml/align.py` & `easyconfig-0.3.0/src/easyconfig/yaml/align.py`

 * *Files identical despite different names*

### Comparing `easyconfig-0.2.8/src/easyconfig/yaml/from_model.py` & `easyconfig-0.3.0/src/easyconfig/yaml/from_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from __future__ import annotations
+
 from enum import Enum
 
 from pydantic import BaseModel
 
 from easyconfig.__const__ import ARG_NAME_IN_FILE, MISSING
 from easyconfig.yaml import CommentedMap, CommentedSeq
 
 NoneType = type(None)
 
 
-def _get_yaml_value(obj, parent_model: BaseModel, skip_none=True):
+def _get_yaml_value(obj, parent_model: BaseModel, *, skip_none=True, obj_name: str | None = None):
     if obj is None:
         return None
 
     # Sometimes enum is used with int/str
     if isinstance(obj, Enum):
         return _get_yaml_value(obj.value, parent_model=parent_model, skip_none=skip_none)
 
@@ -35,38 +37,37 @@
     if isinstance(obj, dict):
         ret = CommentedMap()
         for key, value in obj.items():
             yaml_key = _get_yaml_value(key, parent_model=parent_model, skip_none=skip_none)
             ret[yaml_key] = _get_yaml_value(value, parent_model=parent_model, skip_none=skip_none)
         return ret
 
-    # YAML can't serialize all data pydantic types natively, so we use the json serializer of the model
+    # YAML can't serialize all data pydantic types natively, so we use the serializer of the model
     # This works since a valid json is always a valid YAML. It's not nice but it's something!
-    model_cfg = parent_model.__config__
-    str_val = model_cfg.json_dumps(obj, default=parent_model.__json_encoder__)
-    return model_cfg.json_loads(str_val)
+    dump = parent_model.model_dump(mode='json', include={obj_name})
+    return dump[obj_name]
 
 
 def cmap_from_model(model: BaseModel, skip_none=True) -> CommentedMap:
     cmap = CommentedMap()
-    for obj_key, field in model.__fields__.items():
-        value = getattr(model, obj_key, MISSING)
+    for obj_name, field in model.model_fields.items():
+        value = getattr(model, obj_name, MISSING)
         if value is MISSING or (skip_none and value is None):
             continue
 
-        field_info = field.field_info
-
         yaml_key = field.alias
-        description = field_info.description
+        if yaml_key is None:
+            yaml_key = obj_name
+        description = field.description
 
-        if not field_info.extra.get(ARG_NAME_IN_FILE, True):
+        if (extra_kwargs := field.json_schema_extra) is not None and not extra_kwargs.get(ARG_NAME_IN_FILE, True):
             continue
 
         # get yaml representation
-        cmap[yaml_key] = _get_yaml_value(value, parent_model=model)
+        cmap[yaml_key] = _get_yaml_value(value, parent_model=model, obj_name=obj_name)
 
         if not description:
             continue
 
         # Don't overwrite comment
         if yaml_key not in cmap.ca.items:
             # Ensure that every line in the comment that has chars has a comment sign
```

### Comparing `easyconfig-0.2.8/src/easyconfig.egg-info/SOURCES.txt` & `easyconfig-0.3.0/src/easyconfig.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 src/easyconfig/config_objs/__init__.py
 src/easyconfig/config_objs/app_config.py
 src/easyconfig/config_objs/object_config.py
 src/easyconfig/config_objs/subscription.py
 src/easyconfig/errors/__init__.py
 src/easyconfig/errors/errors.py
 src/easyconfig/errors/handler.py
+src/easyconfig/expansion/__init__.py
+src/easyconfig/expansion/expand.py
+src/easyconfig/expansion/load_file.py
+src/easyconfig/expansion/load_var.py
+src/easyconfig/expansion/location.py
 src/easyconfig/models/__init__.py
 src/easyconfig/models/app.py
 src/easyconfig/models/config.py
 src/easyconfig/models/convenience.py
 src/easyconfig/yaml/__init__.py
 src/easyconfig/yaml/align.py
 src/easyconfig/yaml/from_model.py
```

### Comparing `easyconfig-0.2.8/tests/test_app_creation.py` & `easyconfig-0.3.0/tests/test_app_creation.py`

 * *Files identical despite different names*

