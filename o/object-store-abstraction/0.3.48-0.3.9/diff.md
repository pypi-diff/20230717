# Comparing `tmp/object_store_abstraction-0.3.48.tar.gz` & `tmp/object_store_abstraction-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object_store_abstraction-0.3.48.tar", last modified: Mon Jul 17 16:00:37 2023, max compression
+gzip compressed data, was "dist/object_store_abstraction-0.3.9.tar", last modified: Wed Aug  7 14:28:40 2019, max compression
```

## Comparing `object_store_abstraction-0.3.48.tar` & `object_store_abstraction-0.3.9.tar`

### file list

```diff
@@ -1,41 +1,27 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       67 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)      323 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      895 2022-11-05 15:22:38.000000 object_store_abstraction-0.3.48/README.md
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/object_store_abstraction/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1478 2022-07-30 19:49:06.000000 object_store_abstraction-0.3.48/object_store_abstraction/MultiTenantObjectStore.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4754 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/RepositoryBaseClass.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1328 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/RepositoryCachingBaseClass.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2311 2023-07-17 15:57:11.000000 object_store_abstraction-0.3.48/object_store_abstraction/RepositoryObjBaseClass.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2752 2022-11-05 15:39:54.000000 object_store_abstraction-0.3.48/object_store_abstraction/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      498 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/object_store_abstraction/_version.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3321 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/makeDictJSONSerializable.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3363 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/
--rw-rw-r--   0 robert    (1000) robert    (1000)       56 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/__init__.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/caching/
--rw-rw-r--   0 robert    (1000) robert    (1000)     7062 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/caching/CachePolicy.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2576 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/caching/ConnectionContext.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      939 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/caching/CullQueues.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2048 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/caching/ObjectStore_Caching.py
--rw-rw-r--   0 robert    (1000) robert    (1000)       90 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStoresPackage/caching/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    16316 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_DynamoDB.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5864 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_Memory.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4418 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_Migrating.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    17730 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_SQLAlchemy.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    14825 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_SimpleFileStore.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4485 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_TenantAware.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    13443 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/objectStores_base.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3062 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/paginatedResult.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3128 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/object_store_abstraction/paginatedResultIterator.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)      323 2023-07-17 16:00:37.000000 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1581 2023-07-17 16:00:37.000000 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-17 16:00:37.000000 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-28 09:46:25.000000 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      121 2023-07-17 16:00:37.000000 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       25 2023-07-17 16:00:37.000000 object_store_abstraction-0.3.48/object_store_abstraction.egg-info/top_level.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)      280 2023-07-17 16:00:37.123912 object_store_abstraction-0.3.48/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)     1061 2023-03-23 13:18:52.000000 object_store_abstraction-0.3.48/setup.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-28 09:33:13.000000 object_store_abstraction-0.3.48/versioneer.py
+drwxr-xr-x   0 rjmetcal (506597328) domain users (287000513)        0 2019-08-07 14:28:40.000000 object_store_abstraction-0.3.9/
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      311 2019-08-07 14:28:40.000000 object_store_abstraction-0.3.9/PKG-INFO
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)       67 2019-06-15 15:16:21.000000 object_store_abstraction-0.3.9/MANIFEST.in
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      987 2019-07-17 13:24:47.000000 object_store_abstraction-0.3.9/setup.py
+drwxr-xr-x   0 rjmetcal (506597328) domain users (287000513)        0 2019-08-07 14:28:40.000000 object_store_abstraction-0.3.9/object_store_abstraction/
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     3158 2019-08-06 12:51:01.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)    10169 2019-07-24 11:15:29.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_base.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     4262 2019-08-07 13:55:30.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_TenantAware.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     4204 2019-07-24 11:33:52.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_Migrating.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     3433 2019-07-02 12:15:37.000000 object_store_abstraction-0.3.9/object_store_abstraction/paginatedResult.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     2517 2019-06-15 15:16:21.000000 object_store_abstraction-0.3.9/object_store_abstraction/makeDictJSONSerializable.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)    11874 2019-07-24 08:54:12.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_SimpleFileStore.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     4558 2019-07-24 08:53:34.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_Memory.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)    14963 2019-07-24 08:54:21.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_SQLAlchemy.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)    13299 2019-07-24 08:54:01.000000 object_store_abstraction-0.3.9/object_store_abstraction/objectStores_DynamoDB.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     1961 2019-08-06 12:51:47.000000 object_store_abstraction-0.3.9/object_store_abstraction/__init__.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      497 2019-08-07 14:28:40.000000 object_store_abstraction-0.3.9/object_store_abstraction/_version.py
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      280 2019-08-07 14:28:40.000000 object_store_abstraction-0.3.9/setup.cfg
+drwxr-xr-x   0 rjmetcal (506597328) domain users (287000513)        0 2019-08-07 14:28:40.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)        1 2019-08-07 14:28:38.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/dependency_links.txt
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      909 2019-08-07 14:28:38.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/SOURCES.txt
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      311 2019-08-07 14:28:38.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/PKG-INFO
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)      121 2019-08-07 14:28:38.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/requires.txt
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)        1 2019-08-07 14:22:02.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/not-zip-safe
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)       25 2019-08-07 14:28:38.000000 object_store_abstraction-0.3.9/object_store_abstraction.egg-info/top_level.txt
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)     1157 2019-07-01 14:43:57.000000 object_store_abstraction-0.3.9/README.md
+-rw-r--r--   0 rjmetcal (506597328) domain users (287000513)    68611 2019-06-15 15:16:21.000000 object_store_abstraction-0.3.9/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `object_store_abstraction-0.3.48/README.md` & `object_store_abstraction-0.3.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,25 @@
 
 
 Python library providing abstract object store
 
 
 # Release process
 
-use coderelease
+````
+git tag -l #find latest tag
+
+
+git tag 0.0.1
+sudo python3 setup.py sdist
+sudo python3 setup.py register sdist upload
+git push --tags
+````
+
+If you get an error message reporting "dirty" versions can't be uploaded to pypi it means that you have uncommitted changes.
 
 
 # installs to make a package:
 
 pip install nose
 pip install tox
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/__init__.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,62 @@
-# -*- coding: utf-8 -*-
-
-"""
-    object_store_abstraction
-    ~~~~~~~~
-    Object store abstraction
-    :copyright: (c) 2018 by Robert Metcalf.
-    :license: MIT, see LICENSE for more details.
-"""
-
-#Exception classes from base
-from .objectStores_base import WrongObjectVersionExceptionClass,  SuppliedObjectVersionWhenCreatingExceptionClass, ObjectStoreConfigError,  MissingTransactionContextExceptionClass, UnallowedMutationExceptionClass,  TriedToDeleteMissingObjectExceptionClass, TryingToCreateExistingObjectExceptionClass
-from .objectStores_base import ObjectStore, ObjectStoreConnectionContext
-
-#Exception instances from base
-from .objectStores_base import WrongObjectVersionException, SuppliedObjectVersionWhenCreatingException, MissingTransactionContextException, UnallowedMutationException, TriedToDeleteMissingObjectException, TryingToCreateExistingObjectException, SavingDateTimeTypeException
-#Helper fns from base
-from .objectStores_base import outputFnJustKeys, outputFnItems
-
-from .objectStores import createObjectStoreInstance, ObjectStoreConfigNotDictObjectExceptionClass, InvalidObjectStoreConfigUnknownTypeClass, InvalidObjectStoreConfigMissingTypeException, InvalidObjectStoreConfigUnknownTypeException, InvalidObjectStoreConfigMissingTypeClass
-
-from .makeDictJSONSerializable import getRJMJSONSerializableDICT, getNormalDICTFromRJMJSONSerializableDICT
-
-#TenantAware exceptions and instances
-from .objectStores_TenantAware import CallingNonTenantAwareVersion, CallingNonTenantAwareVersionException, UnsupportedTenantNameException, UnsupportedObjectTypeException
-
-#Allow direct testing of types
-from .objectStores_SQLAlchemy import ObjectStore_SQLAlchemy
+from .objectStores_TenantAware import ObjectStore_TenantAware
 from .objectStores_Memory import ObjectStore_Memory
+from .objectStores_SQLAlchemy import ObjectStore_SQLAlchemy
 from .objectStores_SimpleFileStore import ObjectStore_SimpleFileStore
 from .objectStores_DynamoDB import ObjectStore_DynamoDB
 from .objectStores_Migrating import ObjectStore_Migrating
-from .objectStores_TenantAware import ObjectStore_TenantAware
-from .objectStoresPackage import ObjectStore_Caching, UniqueQueue
 
-#Allowing reuse of iterator
-from .paginatedResult import sanatizePaginatedParamValues
-from .paginatedResult import getPaginatedResultUsingIterator
-from .paginatedResultIterator import PaginatedResultIteratorBaseClass
-from .paginatedResult import getPaginatedResultUsingPythonIterator
-
-#Repository
-from .RepositoryBaseClass import RepositoryBaseClass, RepositoryValidationException
-from .RepositoryCachingBaseClass import RepositoryCachingBaseClass
-from .RepositoryObjBaseClass import RepositoryObjBaseClass
-
-#MultiTenant OBject Store
-from .MultiTenantObjectStore import InvalidTenantNameException, MultiTenantObjectStore
-
-from ._version import get_versions
-__version__ = get_versions()['version']
-del get_versions
+class InvalidObjectStoreConfigMissingTypeClass(Exception):
+  pass
+InvalidObjectStoreConfigMissingTypeException = InvalidObjectStoreConfigMissingTypeClass('APIAPP_OBJECTSTORECONFIG value has no Type attribute')
+
+class InvalidObjectStoreConfigUnknownTypeClass(Exception):
+  pass
+InvalidObjectStoreConfigUnknownTypeException = InvalidObjectStoreConfigUnknownTypeClass('APIAPP_OBJECTSTORECONFIG Type value is not recognised')
+
+class ObjectStoreConfigNotDictObjectExceptionClass(Exception):
+  pass
+
+def _createObjectStoreInstanceTypeSpecified(type, configDICT, initFN, externalFns, detailLogging):
+  print("Using Object Store Type: " + type)
+  return initFN(configDICT, externalFns, detailLogging, type, createObjectStoreInstance)
+
+def _createTenantAwareObjectStoreInstanceTypeSpecified(type, configDICT, initFN, externalFns, detailLogging):
+  objectStore = _createObjectStoreInstanceTypeSpecified(type, configDICT, initFN, externalFns, detailLogging)
+  return ObjectStore_TenantAware(objectStore)
+
+#Based on applicaiton options create an instance of objectStore to be used
+def createObjectStoreInstance(
+  objectStoreConfigDict,
+  externalFns,
+  detailLogging=False,  #True or False
+  tenantAware=False
+):
+  if 'getCurDateTime' not in externalFns:
+    raise Exception("createObjectStoreInstance - Must supply getCurDateTime externalFunction")
+
+  if objectStoreConfigDict is None:
+    objectStoreConfigDict = {}
+    objectStoreConfigDict["Type"] = "Memory"
+
+  if not isinstance(objectStoreConfigDict, dict):
+    raise ObjectStoreConfigNotDictObjectExceptionClass('You must pass a dict as config to createObjectStoreInstance (or None)')
+
+  createFN = _createObjectStoreInstanceTypeSpecified
+  if tenantAware:
+    createFN = _createTenantAwareObjectStoreInstanceTypeSpecified
+
+  if "Type" not in objectStoreConfigDict:
+    raise InvalidObjectStoreConfigMissingTypeException
+  if objectStoreConfigDict["Type"] == "Memory":
+    return createFN("Memory", objectStoreConfigDict, ObjectStore_Memory, externalFns, detailLogging)
+  if objectStoreConfigDict["Type"] == "SQLAlchemy":
+    return createFN("SQLAlchemy", objectStoreConfigDict, ObjectStore_SQLAlchemy, externalFns, detailLogging)
+  if objectStoreConfigDict["Type"] == "SimpleFileStore":
+    return createFN("SimpleFileStore", objectStoreConfigDict, ObjectStore_SimpleFileStore, externalFns, detailLogging)
+  if objectStoreConfigDict["Type"] == "DynamoDB":
+    return createFN("DynamoDB", objectStoreConfigDict, ObjectStore_DynamoDB, externalFns, detailLogging)
+  if objectStoreConfigDict["Type"] == "Migrating":
+    return createFN("Migrating", objectStoreConfigDict, ObjectStore_Migrating, externalFns, detailLogging)
+
+  print("Trying to create object store type " + objectStoreConfigDict["Type"])
+  raise InvalidObjectStoreConfigUnknownTypeException
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/makeDictJSONSerializable.py` & `object_store_abstraction-0.3.9/object_store_abstraction/makeDictJSONSerializable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 #Some types of object are not JSON serialbizle
 # this class swaps them for RJM objects which are
 import json
-import decimal
 
 standardTypeTagString = "rj5mt3ypebdf3ase_TYPE"
 
 def getRJMJSONSerializableDICT(normalDICT):
   return _recursiveConvertFromNormalToRJM(normalDICT)
-
+  
 def getNormalDICTFromRJMJSONSerializableDICT(RJMDICT):
   return _recursiveConvertFromRJMToNormal(RJMDICT)
-
+  
 def getJSONtoPutInStore(origObj):
   #print("Putting in:", type(origObj), ":", origObj)
-  convertedDict = getRJMJSONSerializableDICT(origObj)
-  #print("Converted:", convertedDict)
-  #print("ORig:", origObj)
-  return json.dumps(convertedDict)
+  return json.dumps(getRJMJSONSerializableDICT(origObj))
 
 def getObjFromJSONThatWasPutInStore(jsonFromStore):
   jsonDict = json.loads(jsonFromStore)
   normalDict = getNormalDICTFromRJMJSONSerializableDICT(jsonDict)
   #print("Getting out:", type(normalDict), ":", jsonFromStore)
   return normalDict
 
 def _recursiveConvertFromNormalToRJM(anyObj):
   if isinstance(anyObj,dict):
-    output = {}
     for x in anyObj:
-      output[x] = _recursiveConvertFromNormalToRJM(anyObj[x])
-    return output
+      anyObj[x] = _recursiveConvertFromNormalToRJM(anyObj[x])
+    return anyObj
   if isinstance(anyObj,list):
-    output = []
     for i in range(len(anyObj)):
-      output.append(_recursiveConvertFromNormalToRJM(anyObj[i]))
-    return output
+      anyObj[i] = _recursiveConvertFromNormalToRJM(anyObj[i])
+    return anyObj
   if isinstance(anyObj,bytes):
     return getRJMTypeFromOrigObj(anyObj).toJSONableDICT()
-  if isinstance(anyObj,decimal.Decimal):
-    return getRJMTypeFromOrigObj(anyObj).toJSONableDICT()
-
-  #It was not a type that we recognise so return original
   return anyObj
 
 def _recursiveConvertFromRJMToNormal(anyObj):
   if isinstance(anyObj,dict):
     if standardTypeTagString in anyObj:
       return getRJMTypeFromRJMTypeJSONDict(anyObj).toOrig()
     for x in anyObj:
@@ -55,23 +45,19 @@
       anyObj[i] = _recursiveConvertFromRJMToNormal(anyObj[i])
   return anyObj
 
 
 def getRJMTypeFromOrigObj(obj):
   if isinstance(obj,bytes):
     return RJMTypeBytesClass(obj, None)
-  if isinstance(obj,decimal.Decimal):
-    return RJMTypeDecimalClass(obj, None)
   raise Exception("Unhandled specialType")
 
 def getRJMTypeFromRJMTypeJSONDict(dictObjThatIsJSONRepresenationOfRJMTypeClass):
   if dictObjThatIsJSONRepresenationOfRJMTypeClass[standardTypeTagString] == 'RJMTypeBytesClass':
     return RJMTypeBytesClass(None, dictObjThatIsJSONRepresenationOfRJMTypeClass)
-  if dictObjThatIsJSONRepresenationOfRJMTypeClass[standardTypeTagString] == 'RJMTypeDecimalClass':
-    return RJMTypeDecimalClass(None, dictObjThatIsJSONRepresenationOfRJMTypeClass)
   raise Exception("Unknown type " + dictObjThatIsJSONRepresenationOfRJMTypeClass[standardTypeTagString])
 
 class RJMTypeBaseClass:
   obj = None
   def __init__(self, obj, rjmTypeDict):
     if obj is None:
       self.obj = rjmTypeDict['data'].encode("utf-8")
@@ -82,16 +68,8 @@
 
 class RJMTypeBytesClass(RJMTypeBaseClass):
   def toJSONableDICT(self):
     return {
       standardTypeTagString: 'RJMTypeBytesClass',
       'data': self.obj.decode("utf-8")
     }
-
-class RJMTypeDecimalClass(RJMTypeBaseClass):
-  def toJSONableDICT(self):
-    return {
-      standardTypeTagString: 'RJMTypeDecimalClass',
-      'data': str(self.obj)
-    }
-  def toOrig(self):
-    return decimal.Decimal(self.obj.decode("utf-8"))
+
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_DynamoDB.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_DynamoDB.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item
 
-from .objectStores_base import readOptionalBooleanValueFromConfigDict, ObjectStore, ObjectStoreConnectionContext, StoringNoneObjectAfterUpdateOperationException, WrongObjectVersionException, TriedToDeleteMissingObjectException, TryingToCreateExistingObjectException, SuppliedObjectVersionWhenCreatingException, ObjectStoreConfigError
+from .objectStores_base import ObjectStore, ObjectStoreConnectionContext, StoringNoneObjectAfterUpdateOperationException, WrongObjectVersionException, TriedToDeleteMissingObjectException, TryingToCreateExistingObjectException, SuppliedObjectVersionWhenCreatingException, ObjectStoreConfigError
 from .paginatedResult import getPaginatedResult
-from .paginatedResultIterator import PaginatedResultIteratorBaseClass, sortListOfKeysToDictBySortString, PaginatedResultIteratorFromDictWithAttrubtesAsKeysClass
 
 from boto3 import Session as AWSSession
 from botocore.config import Config
 from botocore import exceptions as botocoreexceptions
 from boto3.dynamodb.conditions import Key, Attr
 
 import logging
@@ -27,39 +26,38 @@
   def _startTransaction(self):
     pass
   def _commitTransaction(self):
     pass
   def _rollbackTransaction(self):
     pass
 
-  def _saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion):
+  def _saveJSONObject(self, objectType, objectKey, JSONString, objectVersion):
     partition_key = make_partition_key(objectType, objectKey)
     (curObjectDICT, curObjectVersion, curCreationDate, curLastUpdateDate, curObjectKey) = self._getObjectJSON(objectType, objectKey)
-    curTime = self.objectStore.externalFns['getCurDateTime']()
-    curTimeValue = curTime.isoformat()
+    curTime = self.objectStore.externalFns['getCurDateTime']().isoformat()
 
     if curObjectDICT is None:
       if objectVersion is not None:
         raise SuppliedObjectVersionWhenCreatingException
       newObjectVersion = 1
 
       self.objectStore.savingNewObject(objectType)
       jsonToStore = getJSONtoPutInStore(JSONString)
       response = self.objectStore.getTable(objectType).put_item(
          Item={
               'partition_key': partition_key,
               'objectType': objectType,
               'objectKey': objectKey,
               'objectVersion': newObjectVersion,
-              'creationDate': curTimeValue,
-              'lastUpdateData': curTimeValue,
+              'creationDate': curTime,
+              'lastUpdateData': curTime,
               'objectDICT': jsonToStore
           }
       )
-      return (newObjectVersion, curTime, curTime)
+      return newObjectVersion
 
     if objectVersion is None:
       raise TryingToCreateExistingObjectException
     if str(curObjectVersion) != str(objectVersion):
       raise WrongObjectVersionException
     newObjectVersion = curObjectVersion + 1
 
@@ -67,30 +65,29 @@
     response = self.objectStore.getTable(objectType).update_item(
         Key={
             'partition_key': partition_key
         },
         UpdateExpression="set objectVersion = :ov, lastUpdateData=:lud, objectDICT=:od",
         ExpressionAttributeValues={
             ':ov': newObjectVersion,
-            ':lud': curTimeValue,
+            ':lud': curTime,
             ':od': jsonToStore
         },
         ReturnValues="UPDATED_NEW"
     )
+    return newObjectVersion
 
-    return (newObjectVersion, curCreationDate, curTime)
-
-  def getTupleFromItem(self, item):
+  def __getTupleFromItem(self, item):
     dt = parse(item['creationDate'])
     creationDate = dt.astimezone(pytz.utc)
     dt = parse(item['lastUpdateData'])
     lastUpdateDate = dt.astimezone(pytz.utc)
     convertedObjectDICT = getObjFromJSONThatWasPutInStore(item['objectDICT'])
 
-    return convertedObjectDICT, int(item['objectVersion']), creationDate, lastUpdateDate, item['objectKey']
+    return convertedObjectDICT, item['objectVersion'], creationDate, lastUpdateDate, item['objectKey']
 
   def _removeJSONObject(self, objectType, objectKey, objectVersion, ignoreMissingObject):
     #Object version error only raised when not ignoring missing
     #https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Expressions.ConditionExpressions.html#Expressions.ConditionExpressions.AdvancedComparisons
     partition_key = make_partition_key(objectType, objectKey)
     ConditionalExpression = None
     ExpressionAttributeValues = None
@@ -122,73 +119,70 @@
 
 
   #Return value is objectDICT, ObjectVersion, creationDate, lastUpdateDate
   #Return None, None, None, None if object isn't in store
   def _getObjectJSON(self, objectType, objectKey):
     partition_key = make_partition_key(objectType, objectKey)
 
-    table = self.objectStore.getTable(objectType)
-
-    response = None
-    try:
-      response = table.get_item(
-          Key={
-              'partition_key': partition_key
-          }
-      )
-    except botocoreexceptions.ResourceNotFoundException as e:
-      # if we get BEFORE any inserts the partition key will not exist
-      #  in this case the item isn't in the store
-      return None, None, None, None, None
-
+    response = self.objectStore.getTable(objectType).get_item(
+        Key={
+            'partition_key': partition_key
+        }
+    )
     if "Item" not in response:
       return None, None, None, None, None
 
-    return self.getTupleFromItem(response["Item"])
+    return self.__getTupleFromItem(response["Item"])
 
 
   def __getAllRowsForObjectType(self, objectType, offset, pagesize):
-    it = Iterator(None, None, None, self, objectType)
     srcData = {}
-    curItem=it.next()
-    while curItem is not None:
-      srcData[curItem[4]] = curItem
-      curItem=it.next()
+
+
+    response = {'LastEvaluatedKey': 'setToStartLoop'}
+    numFetched = 0
+    fetching = True
+    while ('LastEvaluatedKey' in response) and (fetching == True):
+      response = self.objectStore.getTable(objectType).scan(
+          FilterExpression=Key('partition_key').begins_with(objectType),
+      )
+      for curItem in response['Items']:
+        if fetching:
+          numFetched = numFetched + 1
+          srcData[curItem['objectKey']] = self.__getTupleFromItem(curItem)
+          if offset != None: # allows this to work in non-pagination mode
+            if numFetched > (offset + pagesize): #Total caculation will be off when we don't go thorough entire dataset
+                                # but invalid figure will be always be one over as we fetch one past in all cases
+              fetching = False
 
     return srcData
 
   def _getPaginatedResult(self, objectType, paginatedParamValues, outputFN):
     #https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html?highlight=delete_item#paginators
-    srcData = []
-    if paginatedParamValues['sort'] is None:
-      srcData = self.__getAllRowsForObjectType(objectType, paginatedParamValues['offset'], paginatedParamValues['pagesize'])
-    else:
-      # We are doing deep inspection sorting so we must get all the data
-      # TODO could improve this by getting DynamoDB to understand sort somehow
-      srcData = self.__getAllRowsForObjectType(objectType, None, None)
+    srcData = self.__getAllRowsForObjectType(objectType, paginatedParamValues['offset'], paginatedParamValues['pagesize'])
 
     #paginatedParamValues['query'],
     #paginatedParamValues['offset'],
     #paginatedParamValues['pagesize']
 
     return getPaginatedResult(
       list=srcData,
       outputFN=outputFN,
       offset=paginatedParamValues['offset'],
       pagesize=paginatedParamValues['pagesize'],
       query=paginatedParamValues['query'],
       sort=paginatedParamValues['sort'],
-      filterFN=self.filterFN_basicTextInclusion
+      filterFN=self._filterFN_basicTextInclusion
     )
 
   def _getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     superObj = self.__getAllRowsForObjectType(objectType, None, None)
     outputLis = []
     for curKey in superObj:
-      if self.filterFN_basicTextInclusion(superObj[curKey], whereClauseText):
+      if self._filterFN_basicTextInclusion(superObj[curKey], whereClauseText):
         if filterFN(superObj[curKey], whereClauseText):
           outputLis.append(superObj[curKey])
     return list(map(outputFN, outputLis))
 
   def _list_all_objectTypes_singleTableMode(self):
     results = []
     if not self.objectStore.singleTableModeObjectTypeCacheLoaded:
@@ -214,21 +208,14 @@
     return results
 
   def _list_all_objectTypes(self):
     if self.objectStore.singleTableMode:
       return self._list_all_objectTypes_singleTableMode()
     return self._list_all_objectTypes_multiTableMode()
 
-  def _getPaginatedResultIterator(self, query, sort, filterFN, getSortKeyValueFn, objectType):
-    if sort is None:
-      return Iterator(query, filterFN, getSortKeyValueFn, self, objectType)
-    else:
-      dict = self.__getAllRowsForObjectType(objectType, None, None)
-      return PaginatedResultIteratorFromDictWithAttrubtesAsKeysClass(dict, query, sort, filterFN, getSortKeyValueFn)
-
 # Class that will store objects
 class ObjectStore_DynamoDB(ObjectStore):
   awsSession = None
   awsDynamodbClient = None
   objectPrefix = None
   dynTables = None
   singleTableMode = None
@@ -274,15 +261,23 @@
     for x in requiredConfigItems:
       if x not in configJSON:
         raise ObjectStoreConfigError("APIAPP_OBJECTSTORECONFIG DynamoDB ERROR - config param " + x + " missing")
     endpointURL = configJSON["endpoint_url"]
     if endpointURL.strip().upper() == "NONE":
       endpointURL = None
 
-    self.singleTableMode=readOptionalBooleanValueFromConfigDict(key="single_table_mode",default=None,configDict=configJSON)
+    singleTableModeTT = configJSON["single_table_mode"].strip().upper()
+    if singleTableModeTT == "FALSE":
+      self.singleTableMode = False
+    else:
+      if singleTableModeTT.strip().upper() == "TRUE":
+        self.singleTableMode = True
+      else:
+        raise ObjectStoreConfigError("APIAPP_OBJECTSTORECONFIG DynamoDB ERROR - single_table_mode must be true or false")
+
 
     self.awsSession = AWSSession(
       aws_access_key_id=configJSON["aws_access_key_id"],
       aws_secret_access_key=configJSON["aws_secret_access_key"],
       aws_session_token=None,
       region_name=configJSON["region_name"],
       botocore_session=None,
@@ -346,70 +341,7 @@
       for objectType in self.dynTables:
         self.dynTables[objectType]['dyn'].delete()
       self.dynTables = {}
     self.executeInsideTransaction(someFn)
 
   def _getConnectionContext(self):
     return ConnectionContext(self)
-
-class Iterator(PaginatedResultIteratorBaseClass):
-  #https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GettingStarted.Python.04.html#GettingStarted.Python.04.Scan
-  dynamoDBStoreConnectionContext = None
-  objectType = None
-
-  curResponse = None
-  curResponseIdx = None
-
-  def __init__(self, query, filterFN, getSortKeyValueFn, dynamoDBStoreConnectionContext, objectType):
-    PaginatedResultIteratorBaseClass.__init__(self, query, filterFN)
-    self.dynamoDBStoreConnectionContext = dynamoDBStoreConnectionContext
-    self.objectType = objectType
-
-    # Get first page
-    self.curResponseIdx = 0
-    self.curResponse = self.dynamoDBStoreConnectionContext.objectStore.getTable(self.objectType).scan(
-        FilterExpression=Key('partition_key').begins_with(self.objectType + "_"),
-    )
-
-    #self.objectKeys = list(self.memoryStoreConnectionContext.objectStore._INT_getDictForObjectType(objectType).keys())
-
-  def _next(self):
-    if len(self.curResponse['Items']) == 0:
-      return None
-    if self.curResponseIdx < len(self.curResponse['Items']):
-      self.curResponseIdx = self.curResponseIdx + 1
-      return self.dynamoDBStoreConnectionContext.getTupleFromItem(
-        self.curResponse['Items'][self.curResponseIdx-1]
-      )
-
-    if 'LastEvaluatedKey' not in self.curResponse:
-      return None
-
-    # If we are here we have already output the last item in the current response
-    #  get next response
-    self.curResponseIdx = 0
-    self.curResponse = self.dynamoDBStoreConnectionContext.objectStore.getTable(self.objectType).scan(
-        FilterExpression=Key('partition_key').begins_with(self.objectType),
-        ExclusiveStartKey=self.curResponse['LastEvaluatedKey']
-    )
-
-    # We can call ourselves again which will result in the first row of the _next
-    # batch being returned
-    return self.next()
-
-'''
-    response = {'LastEvaluatedKey': 'setToStartLoop'}
-    numFetched = 0
-    fetching = True
-    while ('LastEvaluatedKey' in response) and (fetching == True):
-      response = self.objectStore.getTable(objectType).scan(
-          FilterExpression=Key('partition_key').begins_with(objectType),
-      )
-      for curItem in response['Items']:
-        if fetching:
-          numFetched = numFetched + 1
-          srcData[curItem['objectKey']] = self.getTupleFromItem(curItem)
-          if offset != None: # allows this to work in non-pagination mode
-            if numFetched > (offset + pagesize): #Total caculation will be off when we don't go thorough entire dataset
-                                # but invalid figure will be always be one over as we fetch one past in all cases
-              fetching = False
-'''
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_Memory.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_Memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .objectStores_base import ObjectStore, ObjectStoreConnectionContext, StoringNoneObjectAfterUpdateOperationException, WrongObjectVersionException, TriedToDeleteMissingObjectException, TryingToCreateExistingObjectException, SuppliedObjectVersionWhenCreatingException
 from .paginatedResult import getPaginatedResult
-from .paginatedResultIterator import PaginatedResultIteratorBaseClass, sortListOfKeysToDictBySortString
 
 class ConnectionContext(ObjectStoreConnectionContext):
   objectStore = None
   def __init__(self, objectStore):
     super(ConnectionContext, self).__init__()
     self.objectStore = objectStore
 
@@ -13,15 +12,15 @@
     pass
   def _commitTransaction(self):
     pass
   def _rollbackTransaction(self):
     pass
 
 
-  def _saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion):
+  def _saveJSONObject(self, objectType, objectKey, JSONString, objectVersion):
     dictForObjectType = self.objectStore._INT_getDictForObjectType(objectType)
     curTimeValue = self.objectStore.externalFns['getCurDateTime']()
     newObjectVersion = None
     if objectKey not in dictForObjectType:
       if objectVersion is not None:
         raise SuppliedObjectVersionWhenCreatingException
       newObjectVersion = 1
@@ -30,15 +29,15 @@
       #We have found an object in the DB
       if objectVersion is None:
         raise TryingToCreateExistingObjectException
       if str(objectVersion) != str(dictForObjectType[objectKey][1]):
         raise WrongObjectVersionException
       newObjectVersion = int(objectVersion) + 1
     dictForObjectType[objectKey] = (JSONString, newObjectVersion, dictForObjectType[objectKey][2], curTimeValue, objectKey)
-    return (newObjectVersion, dictForObjectType[objectKey][2], curTimeValue)
+    return newObjectVersion
 
   def _removeJSONObject(self, objectType, objectKey, objectVersion, ignoreMissingObject):
     dictForObjectType = self.objectStore._INT_getDictForObjectType(objectType)
     if objectVersion is not None:
       if objectKey not in dictForObjectType:
         if ignoreMissingObject:
           return None
@@ -76,28 +75,26 @@
     return getPaginatedResult(
       list=srcData,
       outputFN=outputFN,
       offset=paginatedParamValues['offset'],
       pagesize=paginatedParamValues['pagesize'],
       query=paginatedParamValues['query'],
       sort=paginatedParamValues['sort'],
-      filterFN=self.filterFN_basicTextInclusion
+      filterFN=self._filterFN_basicTextInclusion
     )
 
   def _getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     superObj = self.__getAllRowsForObjectType(objectType)
     outputLis = []
     for curKey in superObj:
-      if self.filterFN_basicTextInclusion(superObj[curKey], whereClauseText):
+      if self._filterFN_basicTextInclusion(superObj[curKey], whereClauseText):
         if filterFN(superObj[curKey], whereClauseText):
           outputLis.append(superObj[curKey])
     return list(map(outputFN, outputLis))
 
-  def _getPaginatedResultIterator(self, query, sort, filterFN, getSortKeyValueFn, objectType):
-    return Iterator(query, sort, filterFN, getSortKeyValueFn, self, objectType)
 
 # Class that will store objects in memory only
 class ObjectStore_Memory(ObjectStore):
   objectData = None
   def __init__(self, configJSON, externalFns, detailLogging, type, factoryFn):
     super(ObjectStore_Memory, self).__init__(externalFns, detailLogging, type)
     self.objectData = dict()
@@ -107,29 +104,7 @@
     if objectType not in self.objectData:
       #print("Creating dict for " + objectType)
       self.objectData[objectType] = dict()
     return self.objectData[objectType]
 
   def _getConnectionContext(self):
     return ConnectionContext(self)
-
-class Iterator(PaginatedResultIteratorBaseClass):
-  objectKeys = None
-  curIdx = None
-  memoryStoreConnectionContext = None
-  objectType = None
-
-  def __init__(self, query, sort, filterFN, getSortKeyValueFn, memoryStoreConnectionContext, objectType):
-    PaginatedResultIteratorBaseClass.__init__(self, query, filterFN)
-    self.memoryStoreConnectionContext = memoryStoreConnectionContext
-    self.objectType = objectType
-    self.curIdx = 0
-
-    self.objectKeys = list(self.memoryStoreConnectionContext.objectStore._INT_getDictForObjectType(objectType).keys())
-    if sort is not None:
-      sortListOfKeysToDictBySortString(self.objectKeys, self.memoryStoreConnectionContext.objectStore._INT_getDictForObjectType(objectType), sort, getSortKeyValueFn)
-
-  def _next(self):
-    self.curIdx = self.curIdx + 1
-    if self.curIdx > len(self.objectKeys):
-      return None
-    return self.memoryStoreConnectionContext._getObjectJSON(self.objectType, self.objectKeys[self.curIdx-1])
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_Migrating.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_Migrating.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,21 +30,21 @@
   def _commitTransaction(self):
     self.toContext._commitTransaction()
     return self.fromContext._commitTransaction()
   def _rollbackTransaction(self):
     self.toContext._rollbackTransaction()
     return self.fromContext._rollbackTransaction()
 
-  def _saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion):
+  def _saveJSONObject(self, objectType, objectKey, JSONString, objectVersion):
     to_objectDICT, to_ObjectVersion, to_creationDate, to_lastUpdateDate, to_objectKey = self.toContext._getObjectJSON(objectType, objectKey)
     if to_objectDICT is None:
-      self.toContext._saveJSONObjectV2(objectType, objectKey, JSONString, objectVersion=None)
+      self.toContext._saveJSONObject(objectType, objectKey, JSONString, objectVersion=None)
     else:
-      self.toContext._saveJSONObjectV2(objectType, objectKey, JSONString, objectVersion=to_ObjectVersion)
-    return self.fromContext._saveJSONObjectV2(objectType, objectKey, JSONString, objectVersion)
+      self.toContext._saveJSONObject(objectType, objectKey, JSONString, objectVersion=to_ObjectVersion)
+    return self.fromContext._saveJSONObject(objectType, objectKey, JSONString, objectVersion)
 
   def _removeJSONObject(self, objectType, objectKey, objectVersion, ignoreMissingObject):
     to_objectDICT = None
     to_objectDICT, to_ObjectVersion, to_creationDate, to_lastUpdateDate, to_objectKey = self.toContext._getObjectJSON(objectType, objectKey)
     if to_objectDICT is not None:
       #no need to remove from to stroe if it is not in tostore
       self.toContext._removeJSONObject(objectType, objectKey, to_ObjectVersion, ignoreMissingObject)
@@ -58,17 +58,14 @@
 
   def _getPaginatedResult(self, objectType, paginatedParamValues, outputFN):
     return self.fromContext._getPaginatedResult(objectType, paginatedParamValues, outputFN)
 
   def _getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     return self.fromContext._getAllRowsForObjectType(objectType, filterFN, outputFN, whereClauseText)
 
-  def _getPaginatedResultIterator(self, query, sort, filterFN, getSortKeyValueFn, objectType):
-    return self.fromContext._getPaginatedResultIterator(query, sort, filterFN, getSortKeyValueFn, objectType)
-
 # Class that will store objects in memory only
 class ObjectStore_Migrating(ObjectStore):
   fromStore = None
   toStore = None
   def __init__(self, configJSON, externalFns, detailLogging, type, factoryFn):
     super(ObjectStore_Migrating, self).__init__(externalFns, detailLogging, type)
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_SQLAlchemy.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_SQLAlchemy.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ##import datetime
 from dateutil.parser import parse
 import os
 import logging
 from .paginatedResult import getPaginatedResult
 
 from .makeDictJSONSerializable import getJSONtoPutInStore, getObjFromJSONThatWasPutInStore
-from .paginatedResultIterator import PaginatedResultIteratorBaseClass, sortListOfKeysToDictBySortString, PaginatedResultIteratorFromDictWithAttrubtesAsKeysClass
+
 
 ###---------- Code to get actual query being run
 '''
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.sql.sqltypes import String, DateTime, NullType
 
 PY3 = str is not bytes
@@ -88,15 +88,15 @@
     self.transaction = None
     return res
   def _rollbackTransaction(self):
     res = self.transaction.rollback()
     self.transaction = None
     return res
 
-  def _saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion):
+  def _saveJSONObject(self, objectType, objectKey, JSONString, objectVersion):
     #print("JSONString:", JSONString)
     query = self.objectStore.objDataTable.select(
       whereclause=(
         and_(
           self.objectStore.objDataTable.c.type==objectType,
           self.objectStore.objDataTable.c.key==objectKey
           )
@@ -123,15 +123,15 @@
         lastUpdateDate_iso8601=curTime.isoformat()
       )
       result = self._INT_execute(query)
       if len(result.inserted_primary_key) != 1:
         raise Exception('_saveJSONObject wrong number of rows inserted')
       #if result.inserted_primary_key[0] != objectKey:
       #  raise Exception('_saveJSONObject issue with primary key')
-      return (newObjectVersion, curTime, curTime)
+      return newObjectVersion
     if objectVersion is None:
       raise TryingToCreateExistingObjectException
     if str(firstRow.objectVersion) != str(objectVersion):
       raise WrongObjectVersionException
     newObjectVersion = firstRow.objectVersion + 1
     query = self.objectStore.objDataTable.update(whereclause=(
       and_(
@@ -142,19 +142,17 @@
       objectVersion=newObjectVersion,
       objectDICT=getJSONtoPutInStore(JSONString),
       lastUpdateDate=curTime,
       lastUpdateDate_iso8601=curTime.isoformat()
     )
     result = self._INT_execute(query)
     if result.rowcount != 1:
-      #print('Result count is ', result.rowcount)
+      print('Result count is ', result.rowcount)
       raise Exception('_saveJSONObject wrong number of rows updated')
-
-    #not returning creation date time as it is not present without an extra query
-    return (newObjectVersion, None, curTime)
+    return newObjectVersion
 
   def _removeJSONObject(self, objectType, objectKey, objectVersion, ignoreMissingObject):
     query = self.objectStore.objDataTable.delete(whereclause=(
       and_(
         self.objectStore.objDataTable.c.type==objectType,
         self.objectStore.objDataTable.c.key==objectKey
       )
@@ -207,52 +205,71 @@
         fetching = False
       else:
         results.append(row[0])
 
     return results
 
   def __getObjectTypeListFromDBUsingQuery(self, objectType, queryString, offset, pagesize):
-    # TODO refactor to use iterator
-    iterator = Iterator(queryString, None, None, self, objectType)
+    self.objectStore.detailLog('__getObjectTypeListFromDBUsingQuery')
+    self.objectStore.detailLog('   objectType:' + str(objectType))
+    self.objectStore.detailLog('  queryString:' + str(queryString))
+    whereclauseToUse = self.objectStore.objDataTable.c.type==objectType
+    if queryString is not None:
+      if queryString != '':
+        self.objectStore.detailLog('   **Adding where clause**')
+        whereclauseToUse = and_(
+          whereclauseToUse,
+          self.objectStore.objDataTable.c.objectDICT.ilike('%' + queryString + '%')
+        )
+    query = self.objectStore.objDataTable.select(
+      whereclause=whereclauseToUse,
+      order_by=self.objectStore.objDataTable.c.key
+    )
+    '''
+     SELECT "_objData".id, "_objData".type, "_objData".key, "_objData"."objectDICT", "_objData"."objectVersion", "_objData"."creationDate", "_objData"."lastUpdateDate", "_objData"."creationDate_iso8601", "_objData"."lastUpdateDate_iso8601"
+     FROM "_objData"
+     WHERE "_objData".type = 'Test1' AND lower("_objData"."objectDICT") LIKE lower('%''AA'': 3%') ORDER BY "_objData".key
+    '''
+
+    #print("\n---------\nwhereclauseToUse:", whereclauseToUse)
+    #print("query:", literalquery(query))
+    result =  self._INT_execute(query)
+
     srcData = {}
-    curItem=iterator.next()
-    while curItem is not None:
-      srcData[curItem[4]] = curItem
-      curItem=iterator.next()
+    fetching = True
+    numFetched = 0
+    while (fetching):
+      row = result.fetchone()
+      numFetched = numFetched + 1
+      if row is None:
+        fetching = False
+      else:
+        srcData[row['key']] = self._INT_getTupleFromRow(row)
+      if offset != None: # allows this to work in non-pagination mode
+        if numFetched > (offset + pagesize): #Total caculation will be off when we don't go thorough entire dataset
+                            # but invalid figure will be always be one over as we fetch one past in all cases
+          fetching = False
     return srcData
 
   def _getPaginatedResult(self, objectType, paginatedParamValues, outputFN):
-    srcData = {}
-    if paginatedParamValues['sort'] is None:
-      srcData = self.__getObjectTypeListFromDBUsingQuery(
-        objectType,
-        paginatedParamValues['query'],
-        paginatedParamValues['offset'],
-        paginatedParamValues['pagesize']
-      )
-    else:
-      # Sort requires inspection of data. We must retrieve all data for it to work
-      # this requires a full load of data if sorting is required otherwise some rows
-      # won't be in order. This is one reason to move away from generic objectStore
-      # library
-      srcData = self.__getObjectTypeListFromDBUsingQuery(
-        objectType,
-        paginatedParamValues['query'],
-        None,
-        None
-      )
+    srcData = self.__getObjectTypeListFromDBUsingQuery(
+      objectType,
+      paginatedParamValues['query'],
+      paginatedParamValues['offset'],
+      paginatedParamValues['pagesize']
+    )
 
     return getPaginatedResult(
       list=srcData,
       outputFN=outputFN,
       offset=paginatedParamValues['offset'],
       pagesize=paginatedParamValues['pagesize'],
       query=paginatedParamValues['query'],
       sort=paginatedParamValues['sort'],
-      filterFN=self.filterFN_allowAll
+      filterFN=self._filterFN_allowAll
     )
 
   def _getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     superObj = self.__getObjectTypeListFromDBUsingQuery(
       objectType,
       queryString = whereClauseText,
       offset = None,
@@ -264,34 +281,14 @@
         outputLis.append(superObj[curKey])
     return list(map(outputFN, outputLis))
 
 
   def _close(self):
     self.connection.close()
 
-  def _getPaginatedResultIterator(self, query, sort, filterFN, getSortKeyValueFn, objectType):
-    iterator = Iterator(query, filterFN, getSortKeyValueFn, self, objectType)
-    if sort is None:
-      return iterator
-    srcData = {}
-    curItem=iterator.next()
-    while curItem is not None:
-      srcData[curItem[4]] = curItem
-      curItem=iterator.next()
-
-    # All filtering is already done, this iterator just sorts
-    dict, query, sort, filterFN, getSortKeyValueFn
-    return PaginatedResultIteratorFromDictWithAttrubtesAsKeysClass(
-      dict=srcData,
-      query=None,
-      sort=sort,
-      filterFN=None,
-      getSortKeyValueFn=getSortKeyValueFn
-    )
-
 
 class ObjectStore_SQLAlchemy(ObjectStore):
   engine = None
   objDataTable = None
   verTable = None
   objectPrefix = None
   def __init__(self, ConfigDict, externalFns, detailLogging, type, factoryFn):
@@ -304,43 +301,30 @@
     if "connectionString" not in ConfigDict:
       raise ObjectStoreConfigError("APIAPP_OBJECTSTORECONFIG SQLAlchemy ERROR - Expected connectionString")
     if "objectPrefix" in ConfigDict:
       self.objectPrefix = ConfigDict["objectPrefix"]
     else:
       self.objectPrefix = ""
 
-    otherArgsForCreateEngine = {}
-    if "create_engine_args" in ConfigDict:
-      otherArgsForCreateEngine = ConfigDict["create_engine_args"]
-    else:
-      otherArgsForCreateEngine = {
-        "pool_recycle": 3600,
-        "pool_size": 40,
-        "max_overflow": 0
-      }
-      if "connect_args" in ConfigDict:
-        if ConfigDict["connect_args"] is not None:
-          otherArgsForCreateEngine["connect_args"] = ConfigDict["connect_args"]
-
+    connect_args = None
     if "ssl_ca" in ConfigDict:
-      #print("ssl_ca:", ConfigDict['ssl_ca'])
+      print("ssl_ca:", ConfigDict['ssl_ca'])
       if not os.path.isfile(ConfigDict['ssl_ca']):
         raise Exception("Supplied ssl_ca dosen't exist")
-      if "connect_args" not in ConfigDict:
-        ConfigDict["connect_args"] = {}
-
-      ConfigDict["connect_args"]["ssl"] = {'ca': ConfigDict['ssl_ca']}
+      connect_args = {
+        "ssl": {'ca': ConfigDict['ssl_ca']}
+      }
 
-    if "poolclass" in otherArgsForCreateEngine:
-      if otherArgsForCreateEngine["poolclass"] == "StaticPool":
-        otherArgsForCreateEngine["poolclass"] = StaticPool
+    #My experiment for SSL https://code.metcarob.com/node/249
+    #debugging https://github.com/PyMySQL/PyMySQL/blob/master/pymysql/connections.py
 
-    if detailLogging:
-      print("Creating connection with args:", otherArgsForCreateEngine)
-    self.engine = create_engine(ConfigDict["connectionString"], **otherArgsForCreateEngine)
+    if connect_args is None:
+      self.engine = create_engine(ConfigDict["connectionString"], pool_recycle=3600, pool_size=40, max_overflow=0)
+    else:
+      self.engine = create_engine(ConfigDict["connectionString"], pool_recycle=3600, pool_size=40, max_overflow=0, connect_args=connect_args)
 
     metadata = MetaData()
     #(objDICT, objectVersion, creationDate, lastUpdateDate)
     #from https://stackoverflow.com/questions/15157227/mysql-varchar-index-length
     #MySQL assumes 3 bytes per utf8 character. 255 characters is the maximum index size you can specify per column, because 256x3=768, which breaks the 767 byte limit.
     self.objDataTable = Table(self.objectPrefix + '_objData', metadata,
         #Tired intorudcing a seperate primary key and using key column as index but
@@ -397,66 +381,7 @@
     def someFn(connectionContext):
       query = self.objDataTable.delete()
       connectionContext._INT_execute(query)
     self.executeInsideTransaction(someFn)
 
   def _getConnectionContext(self):
     return ConnectionContext(self)
-
-class Iterator(PaginatedResultIteratorBaseClass):
-  sqlAlchemyStoreConnectionContext = None
-  objectType = None
-  result = None
-
-  def __init__(self, query, filterFN, getSortKeyValueFn, sqlAlchemyStoreConnectionContext, objectType):
-    if query is not None:
-      # This mode deals with queries without a filter function
-      if filterFN is None:
-        def defFilterFn(item, whereClause):
-          return True
-        filterFN = defFilterFn
-    PaginatedResultIteratorBaseClass.__init__(self, query, filterFN)
-    self.sqlAlchemyStoreConnectionContext = sqlAlchemyStoreConnectionContext
-    self.objectType = objectType
-
-    self.sqlAlchemyStoreConnectionContext.objectStore.detailLog('__getObjectTypeListFromDBUsingQuery')
-    self.sqlAlchemyStoreConnectionContext.objectStore.detailLog('   objectType:' + str(self.objectType))
-    self.sqlAlchemyStoreConnectionContext.objectStore.detailLog('  query:' + str(query))
-    whereclauseToUse = self.sqlAlchemyStoreConnectionContext.objectStore.objDataTable.c.type==self.objectType
-    if query is not None:
-      if query != '':
-        self.sqlAlchemyStoreConnectionContext.objectStore.detailLog('   **Adding where clause**')
-        whereclauseToUse = and_(
-          whereclauseToUse,
-          self.sqlAlchemyStoreConnectionContext.objectStore.objDataTable.c.objectDICT.ilike('%' + query + '%')
-        )
-    queryObj = self.sqlAlchemyStoreConnectionContext.objectStore.objDataTable.select(
-      whereclause=whereclauseToUse,
-      order_by=self.sqlAlchemyStoreConnectionContext.objectStore.objDataTable.c.key
-    )
-    # print("SQLAlch Itr queryObj", queryObj)
-    self.result =  self.sqlAlchemyStoreConnectionContext._INT_execute(queryObj)
-
-  def _next(self):
-    row = self.result.fetchone()
-    if row is None:
-      return None
-    return self.sqlAlchemyStoreConnectionContext._INT_getTupleFromRow(row)
-
-'''
-
-    srcData = {}
-    fetching = True
-    numFetched = 0
-    while (fetching):
-      row = result.fetchone()
-      numFetched = numFetched + 1
-      if row is None:
-        fetching = False
-      else:
-        srcData[row['key']] = self._INT_getTupleFromRow(row)
-      if offset != None: # allows this to work in non-pagination mode
-        if numFetched > (offset + pagesize): #Total caculation will be off when we don't go thorough entire dataset
-                            # but invalid figure will be always be one over as we fetch one past in all cases
-          fetching = False
-    return srcData
-  '''
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_SimpleFileStore.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_SimpleFileStore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .objectStores_base import ObjectStore, ObjectStoreConnectionContext, StoringNoneObjectAfterUpdateOperationException, WrongObjectVersionException, TriedToDeleteMissingObjectException, TryingToCreateExistingObjectException, SuppliedObjectVersionWhenCreatingException, ObjectStoreConfigError
 import os
 import threading
 import base64
 from dateutil.parser import parse
 import pytz
 from .paginatedResult import getPaginatedResult
-from .paginatedResultIterator import PaginatedResultIteratorBaseClass, sortListOfKeysToDictBySortString
 
 import shutil #For remove dir and contents
 
 import sys
 
 # SimpleFileStore module
 #  transactions not implemented
@@ -74,16 +73,17 @@
     if not createObjectDir:
       return None
     os.mkdir(dirString)
     self.objectStore.setKnownObjectType(objectType)
     return dirString
 
   def _list_all_objectTypes(self):
-    with self.objectStore.fileAccessLock:
-      lis = localScanDir(self.objectStore.baseLocation, OnlyReturnDirectories=True)
+    self.objectStore.fileAccessLock.acquire()
+    lis = localScanDir(self.objectStore.baseLocation, OnlyReturnDirectories=True)
+    self.objectStore.fileAccessLock.release()
     results = []
     for x in lis:
       if x.startswith(directoryNamePrefix):
         results.append(getKeyFromFileSystemSafeString(x[1:]))
     return results
 
   def getObjectFile(self, objectType, objectKey, createObjectDir):
@@ -121,117 +121,110 @@
     pass
   def _commitTransaction(self):
     pass
   def _rollbackTransaction(self):
     pass
 
 
-  def _saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion):
-    createDateToReturn = None
-    lastUpdateDataToReturn = None
-    with self.objectStore.fileAccessLock:
-      curTime = self.objectStore.externalFns['getCurDateTime']()
-      curTimeValue = curTime.isoformat()
-
-      (o_objectDICT, o_ObjectVersion, o_creationDate, o_lastUpdateDate, o_objectKey) = self.getObjectJSONWithoutLock(objectType, objectKey)
-
-      newObjectVersion = None
-      createDate = None
-      updateDate = None
-
-      if o_ObjectVersion is None:
-        # Object dosen't exist we are creating it
-        if objectVersion is not None:
-          raise SuppliedObjectVersionWhenCreatingException
-        newObjectVersion = 1
-        createDate = curTimeValue
-        updateDate = curTimeValue
-        createDateToReturn = curTime
-        lastUpdateDataToReturn = curTime
-      else:
-        # OBject exists we are updating it
-        if objectVersion is None:
-          raise TryingToCreateExistingObjectException
-        #print("1:", str(objectVersion), ":", o_ObjectVersion, ":")
-        if (int(str(objectVersion)) != int(o_ObjectVersion)):
-          raise WrongObjectVersionException
-        newObjectVersion = int(objectVersion) + 1
-        createDate = o_creationDate.isoformat()
-        updateDate = curTimeValue
-        createDateToReturn = o_creationDate
-        lastUpdateDataToReturn = curTime
-
-      DictToSave = {
-        "Data": JSONString,
-        "ObjVer": newObjectVersion,
-        "Create": createDate,
-        "LastUpdate": updateDate
-      }
-
-      fileName = self.getObjectFile(objectType, objectKey, True)
-
-      target = open(fileName, 'w') #w mode overwrites file content
-      target.write(str(DictToSave))
-      target.close()
+  def _saveJSONObject(self, objectType, objectKey, JSONString, objectVersion):
+    self.objectStore.fileAccessLock.acquire()
+    curTimeValue = self.objectStore.externalFns['getCurDateTime']().isoformat()
+
+    (o_objectDICT, o_ObjectVersion, o_creationDate, o_lastUpdateDate, o_objectKey) = self.getObjectJSONWithoutLock(objectType, objectKey)
+
+    newObjectVersion = None
+    createDate = None
+    updateDate = None
+
+    if o_ObjectVersion is None:
+      # Object dosen't exist we are creating it
+      if objectVersion is not None:
+        raise SuppliedObjectVersionWhenCreatingException
+      newObjectVersion = 1
+      createDate = curTimeValue
+      updateDate = curTimeValue
+    else:
+      # OBject exists we are updating it
+      if objectVersion is None:
+        raise TryingToCreateExistingObjectException
+      #print("1:", str(objectVersion), ":", o_ObjectVersion, ":")
+      if (int(str(objectVersion)) != int(o_ObjectVersion)):
+        raise WrongObjectVersionException
+      newObjectVersion = int(objectVersion) + 1
+      createDate = o_creationDate.isoformat()
+      updateDate = curTimeValue
+
+    DictToSave = {
+      "Data": JSONString,
+      "ObjVer": newObjectVersion,
+      "Create": createDate,
+      "LastUpdate": updateDate
+    }
+
+    fileName = self.getObjectFile(objectType, objectKey, True)
+
+    target = open(fileName, 'w') #w mode overwrites file content
+    target.write(str(DictToSave))
+    target.close()
 
-    return (newObjectVersion, createDateToReturn, lastUpdateDataToReturn)
+    self.objectStore.fileAccessLock.release()
+    return newObjectVersion
 
   def _removeJSONObject(self, objectType, objectKey, objectVersion, ignoreMissingObject):
     if not self.objectStore.isKnownObjectType(objectType):
       if ignoreMissingObject:
         return None
       raise TriedToDeleteMissingObjectException
-    if objectVersion is not None:
-      (o_objectDICT, o_ObjectVersion, o_creationDate, o_lastUpdateDate, o_objectKey) = self.getObjectJSONWithoutLock(objectType, objectKey)
-      if o_objectDICT is not None:
-        if str(o_ObjectVersion) != str(objectVersion):
-          raise WrongObjectVersionException
-
-    with self.objectStore.fileAccessLock:
-      #Simple way of doing it - call a get and see what is returned
-      #(o_objectDICT, o_ObjectVersion, o_creationDate, o_lastUpdateDate) = self.getObjectJSONWithoutLock(objectType, objectKey)
-      #if o_objectDICT is None:
-      #  if ignoreMissingObject:
-      #    return None
-      #  raise TriedToDeleteMissingObjectException
-
-      #It is more efficient to check the file exists - we don't need to get it
-      fileName = self.getObjectFile(objectType, objectKey, True)
-      if fileName is None:
-        if ignoreMissingObject:
-          return None
-        raise TriedToDeleteMissingObjectException
-      if not os.path.exists(fileName):
-        if ignoreMissingObject:
-          return None
-        raise TriedToDeleteMissingObjectException
+    self.objectStore.fileAccessLock.acquire()
 
-      os.remove(fileName)
+    #Simple way of doing it - call a get and see what is returned
+    #(o_objectDICT, o_ObjectVersion, o_creationDate, o_lastUpdateDate) = self.getObjectJSONWithoutLock(objectType, objectKey)
+    #if o_objectDICT is None:
+    #  if ignoreMissingObject:
+    #    return None
+    #  raise TriedToDeleteMissingObjectException
+
+    #It is more efficient to check the file exists - we don't need to get it
+    fileName = self.getObjectFile(objectType, objectKey, True)
+    if fileName is None:
+      if ignoreMissingObject:
+        return None
+      raise TriedToDeleteMissingObjectException
+    if not os.path.exists(fileName):
+      if ignoreMissingObject:
+        return None
+      raise TriedToDeleteMissingObjectException
+
+
+    os.remove(fileName)
+
+    self.objectStore.fileAccessLock.release()
     return None
 
   #Return value is objectDICT, ObjectVersion, creationDate, lastUpdateDate
   #Return None, None, None, None if object isn't in store
   def _getObjectJSON(self, objectType, objectKey):
-    with self.objectStore.fileAccessLock:
-      a = self.getObjectJSONWithoutLock(objectType, objectKey)
+    self.objectStore.fileAccessLock.acquire()
+    a = self.getObjectJSONWithoutLock(objectType, objectKey)
+    self.objectStore.fileAccessLock.release()
     return a
 
 
   def _getPaginatedResult(self, objectType, paginatedParamValues, outputFN):
     collectedObjects = self.__getAllRowsForObjectType(objectType)
 
     ##print('objectStoresMemory._getPaginatedResult self.objectType.objectData[objectType]:', self.objectType.objectData[objectType])
     return getPaginatedResult(
       list=collectedObjects,
       outputFN=outputFN,
       offset=paginatedParamValues['offset'],
       pagesize=paginatedParamValues['pagesize'],
       query=paginatedParamValues['query'],
       sort=paginatedParamValues['sort'],
-      filterFN=self.filterFN_basicTextInclusion
+      filterFN=self._filterFN_basicTextInclusion
     )
 
   def __getAllRowsForObjectType(self, objectType):
     #This is as simple as getting a directory listing
     collectedObjects = {}
 
     otd = self.getObjectTypeDirectory(objectType, createObjectDir=False)
@@ -246,30 +239,24 @@
 
     return collectedObjects
 
   def _getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     superObj = self.__getAllRowsForObjectType(objectType)
     outputLis = []
     for curKey in superObj:
-      if self.filterFN_basicTextInclusion(superObj[curKey], whereClauseText):
+      if self._filterFN_basicTextInclusion(superObj[curKey], whereClauseText):
         if filterFN(superObj[curKey], whereClauseText):
           outputLis.append(superObj[curKey])
     return list(map(outputFN, outputLis))
 
-  def _getPaginatedResultIterator(self, query, sort, filterFN, getSortKeyValueFn, objectType):
-    return Iterator(query, sort, filterFN, getSortKeyValueFn, self, objectType)
-
 
 # Class that will store objects as directoryies and files in the file system
 class ObjectStore_SimpleFileStore(ObjectStore):
   baseLocation = ""
   fileAccessLock = None #Make sure we do one operation at a time
-  # using with when accessing see https://www.bogotobogo.com/python/Multithread/python_multithreading_Using_Locks_with_statement_Context_Manager.php
-  #  this deals properly with exceptions
-
   knownExistingObjectTypes = None #reduce os.dir exist calls by storeing objects we know have a dir
 
   def isKnownObjectType(self, objectType):
     return objectType in self.knownExistingObjectTypes
   def setKnownObjectType(self, objectType):
     self.knownExistingObjectTypes[objectType] = True
 
@@ -299,20 +286,14 @@
       f = open(self.baseLocation + "/writetest.tmp","w+")
       f.write("Test")
       f.close()
       os.remove(self.baseLocation + "/writetest.tmp")
     except:
       raise ObjectStoreConfigError("APIAPP_OBJECTSTORECONFIG SimpleFileStore ERROR - Write test to base location failed")
 
-    # Scan base directory and load in all known object types
-    subDirs = localScanDir(directoryToScan=self.baseLocation, OnlyReturnDirectories=True)
-    for curDir in subDirs:
-      if curDir.startswith(directoryNamePrefix):
-        self.setKnownObjectType(getKeyFromFileSystemSafeString(curDir[len(directoryNamePrefix):]))
-
   def _INT_getDictForObjectType(self, objectType):
     if objectType not in self.objectData:
       #print("Creating dict for " + objectType)
       self.objectData[objectType] = dict()
     return self.objectData[objectType]
 
   #required for unit testing
@@ -321,59 +302,15 @@
     def someFn(connectionContext):
       subDirsToDel = localScanDir(directoryToScan=self.baseLocation, OnlyReturnDirectories=True)
 
       for curDir in subDirsToDel:
         if curDir.startswith(directoryNamePrefix):
           shutil.rmtree(self.baseLocation + "/" + curDir)
 
-    with self.fileAccessLock:
-      self.knownExistingObjectTypes = {}
-      # print("SFS 279: reseting all known types")
-      self.executeInsideTransaction(someFn)
+    self.fileAccessLock.acquire()
+    self.knownExistingObjectTypes = {}
+    # print("SFS 279: reseting all known types")
+    self.executeInsideTransaction(someFn)
+    self.fileAccessLock.release()
 
   def _getConnectionContext(self):
     return ConnectionContext(self)
-
-class Iterator(PaginatedResultIteratorBaseClass):
-  objectKeys = None
-  objects = None # load the objects - only required if we are sorting
-  curIdx = None
-  simpleFileStoreConnectionContext = None
-  objectType = None
-  def __init__(self, query, sort, filterFN, getSortKeyValueFn, simpleFileStoreConnectionContext, objectType):
-    PaginatedResultIteratorBaseClass.__init__(self, query, filterFN)
-    self.simpleFileStoreConnectionContext = simpleFileStoreConnectionContext
-    self.objectType = objectType
-    self.objectFiles = []
-    otd = simpleFileStoreConnectionContext.getObjectTypeDirectory(objectType, createObjectDir=False)
-    objFilenames = []
-    if otd is not None:
-      objFilenames = localScanDir(otd, False)
-    self.objectKeys = []
-    for curObjFilename in objFilenames:
-      self.objectKeys.append(getKeyFromFileSystemSafeString(curObjFilename))
-
-    if sort is not None:
-      # Load all objects into dict indexed by key
-      self.objects = {}
-      for curKey in self.objectKeys:
-        self.objects[curKey] = self.simpleFileStoreConnectionContext._getObjectJSON(self.objectType, curKey)
-
-      sortListOfKeysToDictBySortString(self.objectKeys, self.objects, sort, getSortKeyValueFn)
-
-
-    self.curIdx = 0
-
-    #print(self.objectFiles)
-
-  def _next(self):
-    self.curIdx = self.curIdx + 1
-    if self.curIdx > len(self.objectKeys):
-      return None
-
-
-    #print("OK:" + objectKey)
-    if self.objects is None:
-      return self.simpleFileStoreConnectionContext._getObjectJSON(self.objectType, self.objectKeys[self.curIdx-1])
-    else:
-      # All objects were loaded so just output the object
-      return self.objects[self.objectKeys[self.curIdx-1]]
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_TenantAware.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_TenantAware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-objectTypeSeperator = "$:}wol{}"
+objectTypeSeperator = "$:_}wol{}"
 
 class CallingNonTenantAwareVersion(Exception):
   pass
 CallingNonTenantAwareVersionException = CallingNonTenantAwareVersion('Tried to call a non-tenant aware version')
 class UnsupportedTenantName(Exception):
   pass
 UnsupportedTenantNameException = UnsupportedTenantName('Tenant Name contains a reserved word')
@@ -36,17 +36,14 @@
       raise
     return retVal
 
 
   def saveJSONObject(self, objectType, objectKey, JSONString, objectVersion = None):
     return self.objectStoreContext.saveJSONObject(self.__INT__getDirivedObjectType(objectType), objectKey, JSONString, objectVersion)
 
-  def saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion = None):
-    return self.objectStoreContext.saveJSONObjectV2(self.__INT__getDirivedObjectType(objectType), objectKey, JSONString, objectVersion)
-
   def removeJSONObject(self, objectType, objectKey, objectVersion = None, ignoreMissingObject = False):
     return self.objectStoreContext.removeJSONObject(self.__INT__getDirivedObjectType(objectType), objectKey, objectVersion, ignoreMissingObject)
 
   def updateJSONObject(self, objectType, objectKey, updateFn, objectVersion = None):
     return self.objectStoreContext.updateJSONObject(self.__INT__getDirivedObjectType(objectType), objectKey, updateFn, objectVersion)
 
   def getObjectJSON(self, objectType, objectKey):
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/objectStores_base.py` & `object_store_abstraction-0.3.9/object_store_abstraction/objectStores_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-from .paginatedResult import sanatizePaginatedParamValues, getPaginatedResultUsingIterator
-import datetime
-
-#Definition of Offset
-# offset is the number to skip before outputing
-# e.g. for 1,2,3,4,5,6,7,8,9 and pagesize 3
-#  offset 0 is default and outputs 1,2,3
-#  offset 1                outputs 2,3,4
-#  offset 2                outputs 3,4,5
+from .paginatedResult import sanatizePaginatedParamValues
 
 # Code to save JSON objects into a store.
 #  Allows abstraction of particular store
 #  This is the baseClass other stores inherit from
 StoringNoneObjectAfterUpdateOperationException = Exception('Storing None Object After Update Operation')
 SavedObjectShouldNotContainObjectVersionException = Exception('SavedObjectShouldNotContainObjectVersion')
-SavingDateTimeTypeException = Exception('Saving datetime into objectstore not supported')
 
 class WrongObjectVersionExceptionClass(Exception):
   pass
 WrongObjectVersionException = WrongObjectVersionExceptionClass('Wrong object version supplied - Has another change occured since loading?')
 
 class SuppliedObjectVersionWhenCreatingExceptionClass(Exception):
   pass
@@ -38,23 +29,14 @@
   pass
 TriedToDeleteMissingObjectException = TriedToDeleteMissingObjectExceptionClass("Tried to delete non existant object")
 
 class TryingToCreateExistingObjectExceptionClass(Exception):
   pass
 TryingToCreateExistingObjectException = TryingToCreateExistingObjectExceptionClass("Tried to create an object that already exists")
 
-class InvalidObjectTypeExceptionClass(Exception):
-  pass
-InvalidObjectTypeException = InvalidObjectTypeExceptionClass("Object Type Name is invalid")
-
-def getDefaultGetSortKeyValueFn(outputFN):
-  def defaultGetSortKeyValueFn(item, sortkeyName):
-    return outputFN(item)[sortkeyName]
-  return defaultGetSortKeyValueFn
-
 '''
 Calling pattern for connection where obj is and instance of ObjectStore:
 
 storeConnection = obj.getConnectionContext()
 def someFn(connectionContext):
   ##DO STUFF
 storeConnection.executeInsideTransaction(someFn)
@@ -72,40 +54,14 @@
   storeConnection.commitTransaction()
 except:
   storeConnection.rollbackTransaction()
   raise
 
 '''
 
-#Utility read config functions
-def readOptionalBooleanValueFromConfigDict(key,default,configDict):
-  shouldReturnDefault = False
-  if key not in configDict:
-    shouldReturnDefault = True
-  else:
-    val = configDict[key]
-    if val is None:
-      shouldReturnDefault = True
-
-  if shouldReturnDefault:
-    if default is not None:
-      return default
-    raise ObjectStoreConfigError("readOptionalBooleanValueFromConfigDict ERROR - " + key + " not specified and no default")
-
-  if isinstance(val, bool):
-    return val
-  if isinstance(val, str):
-    val = val.strip().upper()
-    if val == "TRUE":
-      return True
-    if val == "FALSE":
-      return False
-  raise ObjectStoreConfigError("readOptionalBooleanValueFromConfigDict ERROR - " + key + " must be true or false (got " + str(val) + ")")
-
-
 #Utility output functions
 def outputFnJustKeys(item):
   (objectDICT, ObjectVersion, creationDate, lastUpdateDate, objectKey) = item
   #print("objectDICT:", objectDICT)
   #print("ObjectVersion:", ObjectVersion)
   #print("creationDate:", creationDate)
   #print("lastUpdateDate:", lastUpdateDate)
@@ -151,44 +107,20 @@
       retVal = fnToExecute(self)
       self._INT_commitTransaction()
     except:
       self._INT_rollbackTransaction()
       raise
     return retVal
 
-  def validateObjectType(self, objectType):
-    if '_' in objectType:
-      raise InvalidObjectTypeException
-
-  def validateObjectDict(self, objectToSTore):
-    if objectToSTore is None:
-      return
-    if isinstance(objectToSTore, datetime.datetime):
-      raise SavingDateTimeTypeException
-    if isinstance(objectToSTore, dict):
-      for x in objectToSTore:
-        self.validateObjectDict(objectToSTore=objectToSTore[x])
-    if isinstance(objectToSTore, list):
-      for x in objectToSTore:
-        self.validateObjectDict(objectToSTore=x)
-    return
-
   #Return value is objectVersion of object saved
   def saveJSONObject(self, objectType, objectKey, JSONString, objectVersion = None):
-    ret = self.saveJSONObjectV2(objectType, objectKey, JSONString, objectVersion)
-    return ret[0] #just return object version
-
-  #NEw version with Return value (newObjVersion, creationDateTime, lastUpdateDateTime)
-  def saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion = None):
-    self.validateObjectType(objectType=objectType)
-    self.validateObjectDict(objectToSTore=JSONString)
     if 'ObjectVersion' in JSONString:
       raise SavedObjectShouldNotContainObjectVersionException
     self._INT_varifyWeCanMutateData()
-    return self._saveJSONObjectV2(objectType, objectKey, JSONString, objectVersion)
+    return self._saveJSONObject(objectType, objectKey, JSONString, objectVersion)
 
   #Return value is None
   def removeJSONObject(self, objectType, objectKey, objectVersion = None, ignoreMissingObject = False):
     self._INT_varifyWeCanMutateData()
     return self._removeJSONObject(objectType, objectKey, objectVersion, ignoreMissingObject)
 
   # Update the object in single operation. make transaction safe??
@@ -226,57 +158,39 @@
         'query': None,
         'sort': None,
       }
       return connectionContext.getPaginatedResult(objectType, paginatedParamValues=paginatedParamValues, outputFN=None)
     loadedData = storeConnection.executeInsideTransaction(someFn)
   '''
 
-  def getPaginatedResult(self, objectType, paginatedParamValues, outputFN, filterFn=None, getSortKeyValueFn=None):
+  def getPaginatedResult(self, objectType, paginatedParamValues, outputFN):
     if outputFN is None:
       outputFN = outputFnItems
-    sanatizedPaginatedParamValues = sanatizePaginatedParamValues(paginatedParamValues)
-    if filterFn is None:
-      return self._getPaginatedResult(objectType, sanatizedPaginatedParamValues, outputFN)
-    if getSortKeyValueFn is None:
-      getSortKeyValueFn = getDefaultGetSortKeyValueFn(outputFN)
-    return getPaginatedResultUsingIterator (
-      iteratorObj=self._getPaginatedResultIterator(
-        query=paginatedParamValues['query'],
-        sort=paginatedParamValues['sort'],
-        filterFN=filterFn,
-        getSortKeyValueFn=getSortKeyValueFn,
-        objectType=objectType
-      ),
-      outputFN=outputFN,
-      offset=paginatedParamValues['offset'],
-      pagesize=paginatedParamValues['pagesize']
-    )
+    return self._getPaginatedResult(objectType, sanatizePaginatedParamValues(paginatedParamValues), outputFN)
 
   # filterFN is applied first, then outputFN
   #  output fn is fed same params as getObjectJSON returns
   def getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     if outputFN is None:
       outputFN = outputFnItems
     def defFilter(item, whereClauseText):
       return True
     if filterFN is None:
       filterFN = defFilter
     return self._getAllRowsForObjectType(objectType, filterFN, outputFN, whereClauseText)
 
 
-  def _saveJSONObjectV2(self, objectType, objectKey, JSONString, objectVersion):
-    raise Exception('_saveJSONObjectV2 Not Overridden')
+  def _saveJSONObject(self, objectType, objectKey, JSONString, objectVersion):
+    raise Exception('_saveJSONObject Not Overridden')
   def _removeJSONObject(self, objectType, objectKey, objectVersion, ignoreMissingObject):
     raise Exception('_removeJSONObject Not Overridden')
   def _getObjectJSON(self, objectType, objectKey):
     raise Exception('_getObjectJSON Not Overridden')
   def _getPaginatedResult(self, objectType, paginatedParamValues, outputFN):
     raise Exception('_getPaginatedResult Not Overridden')
-  def _getPaginatedResultIterator(self, query, sort, filterFN, getSortKeyValueFn, objectType):
-    raise Exception('_getPaginatedResultIterator Not Overridden')
 
   #should return a fresh transaction context
   def _startTransaction(self):
     raise Exception('_startTransaction Not Overridden')
   def _commitTransaction(self):
     raise Exception('_commitTransaction Not Overridden')
   def _rollbackTransaction(self):
@@ -285,26 +199,26 @@
   def _getAllRowsForObjectType(self, objectType, filterFN, outputFN, whereClauseText):
     raise Exception('_getAllRowsForObjectType Not Implemented for this objectstore type')
 
   #Optional override for closing the context
   def _close(self):
     pass
 
-  def filterFN_basicTextInclusion(self, item, whereClauseText):
+  def _filterFN_basicTextInclusion(self, item, whereClauseText):
     #baseapp passes in whereClauseText as all upper case
     if whereClauseText is None:
       return True
     if whereClauseText == '':
       return True
     ###userDICT = CreateUserObjFromUserDict(appObj, item[0],item[1],item[2],item[3]).getJSONRepresenation()
     #TODO replace with a dict awear generic function
     #  we also need to consider removing spaces from consideration
     return whereClauseText in str(item).upper()
 
-  def filterFN_allowAll(self, item, whereClauseText):
+  def _filterFN_allowAll(self, item, whereClauseText):
     return True
 
   #This won't work via a cache since not all objectTypes are read
   def list_all_objectTypes(self):
     return self._list_all_objectTypes()
 
   def _list_all_objectTypes(self):
```

### Comparing `object_store_abstraction-0.3.48/object_store_abstraction/paginatedResultIterator.py` & `object_store_abstraction-0.3.9/object_store_abstraction/paginatedResult.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,131 @@
+#Function to return paginated result for query
+from sortedcontainers import SortedDict
 
-
-class PaginatedResultIteratorBaseClass():
-  whereClauses = None
-  filterFn = None
-
-  def __init__(self, query, filterFn):
-    if query is not None:
-      if query != "":
-        self.whereClauses = query.strip().upper().split(" ")
-    self.filterFn = filterFn
-
-  def includeResult(self, res):
-    # print("paginatedResItBase includeResult Start", res)
-    if res is None:
-      return True # we get a none at the end - it's the stop signal
-    if self.whereClauses is None:
-      if self.filterFn is None:
-        return True
-      return self.filterFn(res, None) # Filter function with no where clauses
-    for curClause in self.whereClauses:
-      if not self.filterFn(res, curClause):
-        return False
-    return True
-
-  def next(self):
-    a = self._next()
-    while not self.includeResult(a):
-      a = self._next()
-      if a is None:
-        return None
-    return a
-
-  def _next(self):
-    raise Exception("_next is Not Implemented")
-
-def sortListOfKeysToDictBySortString(listOfKeys, dictOfData, sortString, getSortKeyValueFn):
-  def getSortTuple(key):
-    #sort keys are case sensitive
-    kk = key.split(":")
-    if len(kk)==0:
-      raise Exception('Invalid sort key')
-    elif len(kk)==1:
-      return {'name': kk[0], 'desc': False}
-    elif len(kk)==2:
-      if kk[1].lower() == 'desc':
-        return {'name': kk[0], 'desc': True}
-      elif kk[1].lower() == 'asc':
+def isValue(val):
+  if val is None:
+    return False
+  if len(val.strip())==0:
+    return False
+  return True
+
+def sanatizePaginatedParamValues(origValues):
+  pagesizemax = 100
+
+  offset = -1  #number from 0 upwards
+  pagesize = -1 #number from 0 upwards
+  query = None #none or string not empty
+  sort = None #none or string not empty
+
+  #'offset': offset,
+  if origValues['offset'] is None:
+    offset = 0
+  else:
+    offset = int(origValues['offset'])
+
+  #'pagesize': pagesize,
+  if origValues['pagesize'] is None:
+    pagesize = 100
+  else:
+    pagesize = int(origValues['pagesize'])
+
+  if pagesize > pagesizemax:
+    pagesize = pagesizemax
+
+  #'query': query,
+  if isValue(origValues['query']):
+    query = origValues['query']
+
+  #'sort': sort,
+  if isValue(origValues['sort']):
+    sort = origValues['sort']
+
+
+  return {
+    'offset': offset,
+    'pagesize': pagesize,
+    'query': query,
+    'sort': sort,
+  }
+
+def getPaginatedResult(
+  list,
+  outputFN,
+  offset,
+  pagesize,
+  query,
+  sort,
+  filterFN
+):
+  if query is not None:
+    origList = SortedDict(list)
+    list = SortedDict()
+    where_clauses = query.strip().upper().split(" ")
+    def includeItem(item):
+      for curClause in where_clauses:
+        if not filterFN(item, curClause):
+          return False
+      return True
+    for cur in origList:
+      if includeItem(origList[cur]):
+        list[cur]=origList[cur]
+
+  # we now have "list" which is a filtered down list of things we need to return
+  #construct a list of keys to the object, all null
+  sortedKeys = []
+  for cur in list:
+    sortedKeys.append(cur)
+
+  #Sort sortedKeys
+  if sort is not None:
+    def getSortTuple(key):
+      #sort keys are case sensitive
+      kk = key.split(":")
+      if len(kk)==0:
+        raise Exception('Invalid sort key')
+      elif len(kk)==1:
         return {'name': kk[0], 'desc': False}
-    raise Exception('Invalid sort key - ' + key)
-
-  def genSortKeyGenFn(listBeingSorted, sortkey):
-    def sortKeyGenFn(ite):
-      try:
-        # print(sortkey)
-        # print(outputFN(listBeingSorted[ite])[sortkey])
-        ret = getSortKeyValueFn(listBeingSorted[ite], sortkey)
-        if ret is None:
-          return ''
-        if isinstance(ret, int):
-          return ('000000000000000000000000000000000000000000000000000' + str(ret))[-50:]
-        if isinstance(ret, bool):
-          if ret:
-            return 'True'
-          return 'False'
-        return ret
-      except KeyError:
-        raise Exception('Sort key ' + sortkey + ' not found')
-    return sortKeyGenFn
-
-  # sort by every sort key one at a time starting with the least significant
-  for curSortKey in sortString.split(",")[::-1]:
-    sk = getSortTuple(curSortKey)
-    listOfKeys.sort(key=genSortKeyGenFn(dictOfData, sk['name']), reverse=sk['desc'])
-
-class PaginatedResultIteratorFromDictWithAttrubtesAsKeysClass(PaginatedResultIteratorBaseClass):
-  dict = None
-  curIdx = None
-  listOfKeys = None
-
-  def __init__(self, dict, query, sort, filterFN, getSortKeyValueFn):
-    PaginatedResultIteratorBaseClass.__init__(self, query, filterFN)
-    self.curIdx = 0
-    self.dict = dict
-    self.listOfKeys = []
-    for cur in self.dict:
-      self.listOfKeys.append(cur)
-
-    if sort is not None:
-      sortListOfKeysToDictBySortString(self.listOfKeys, self.dict, sort, getSortKeyValueFn)
-
-  #def hasMore(self):
-  #  return self.curIdx < len(self.listOfKeys)
-
-  def _next(self):
-    self.curIdx = self.curIdx + 1
-    if self.curIdx > len(self.listOfKeys):
-      return None
-    return self.dict[self.listOfKeys[self.curIdx-1]]
+      elif len(kk)==2:
+        if kk[1].lower() == 'desc':
+          return {'name': kk[0], 'desc': True}
+        elif kk[1].lower() == 'asc':
+          return {'name': kk[0], 'desc': False}
+      raise Exception('Invalid sort key - ' + key)
+
+    def genSortKeyGenFn(listBeingSorted, sortkey):
+      def sortKeyGenFn(ite):
+        try:
+          # print(sortkey)
+          # print(outputFN(listBeingSorted[ite])[sortkey])
+          ret = outputFN(listBeingSorted[ite])[sortkey]
+          if ret is None:
+            return ''
+          if isinstance(ret, int):
+            return ('000000000000000000000000000000000000000000000000000' + str(ret))[-50:]
+          if isinstance(ret, bool):
+            if ret:
+              return 'True'
+            return 'False'
+          return ret
+        except KeyError:
+          raise Exception('Sort key ' + sortkey + ' not found')
+      return sortKeyGenFn
+
+    # sort by every sort key one at a time starting with the least significant
+    for curSortKey in sort.split(",")[::-1]:
+      sk = getSortTuple(curSortKey)
+      sortedKeys.sort(key=genSortKeyGenFn(list, sk['name']), reverse=sk['desc'])
+
+  output = []
+  for cur in range(offset, (pagesize + offset)):
+    if (cur<len(list)):
+      output.append(outputFN(list[sortedKeys[cur]]))
+      #output.append(outputFN(list[list.keys()[sortedKeys[cur]]]))
+
+  return {
+    'pagination': {
+      'offset': offset,
+      'pagesize': pagesize,
+      'total': len(list)
+    },
+    'result': output
+  }
```

### Comparing `object_store_abstraction-0.3.48/versioneer.py` & `object_store_abstraction-0.3.9/versioneer.py`

 * *Files identical despite different names*

