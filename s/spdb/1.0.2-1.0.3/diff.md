# Comparing `tmp/spdb-1.0.2.tar.gz` & `tmp/spdb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.0.2.tar", last modified: Mon Jul 17 10:52:26 2023, max compression
+gzip compressed data, was "spdb-1.0.3.tar", last modified: Mon Jul 17 12:51:24 2023, max compression
```

## Comparing `spdb-1.0.2.tar` & `spdb-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:52:26.712073 spdb-1.0.2/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      117 2023-07-17 10:52:26.712073 spdb-1.0.2/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 10:52:26.712073 spdb-1.0.2/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 10:52:20.000000 spdb-1.0.2/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:52:26.708740 spdb-1.0.2/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.2/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1448 2023-07-17 10:26:37.000000 spdb-1.0.2/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      584 2023-07-17 10:26:50.000000 spdb-1.0.2/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      974 2023-07-17 10:26:29.000000 spdb-1.0.2/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      316 2023-07-17 10:26:46.000000 spdb-1.0.2/spdb/text_validator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      633 2023-07-17 10:26:40.000000 spdb-1.0.2/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.2/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:52:26.712073 spdb-1.0.2/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      117 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      299 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.2/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 12:51:24.577708 spdb-1.0.3/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.3/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      139 2023-07-17 12:51:24.577708 spdb-1.0.3/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1655 2023-07-17 12:50:32.000000 spdb-1.0.3/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 12:51:24.577708 spdb-1.0.3/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 12:10:43.000000 spdb-1.0.3/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 12:51:24.554375 spdb-1.0.3/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.3/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.3/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.3/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.3/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.3/spdb/text_validator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.3/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.3/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 12:51:24.577708 spdb-1.0.3/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      139 2023-07-17 12:51:24.000000 spdb-1.0.3/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      317 2023-07-17 12:51:24.000000 spdb-1.0.3/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 12:51:24.000000 spdb-1.0.3/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.3/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 12:51:24.000000 spdb-1.0.3/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 12:51:24.000000 spdb-1.0.3/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.0.2/spdb/db.py` & `spdb-1.0.3/spdb/db.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sqlite3
 import json
 
 
 class Database:
-	def __init__(self, path):
+	def __init__(self, path: str):
 		self.path = path
 
 
-	def create_tables(self, tables_names):
+	def create_tables(self, tables_names: list[str]):
 		for table_name in tables_names:
 			self.execute(f'create table if not exists {table_name}(id text, data text)')
 
 
 	def execute(self, code: str) -> str:
 		database = sqlite3.connect(self.path, isolation_level=None)
 		cursor = database.cursor()
@@ -20,37 +20,42 @@
 		database.commit()
 		database.close()
 		return result
 
 
 	@staticmethod
 	def object_to_dict(object) -> dict:
+		if object is None:
+			return {}
 		return json.loads(json.dumps(object.__dict__))
 
 
 	@staticmethod
-	def dict_to_object(Class, Dict):
-		return Class(**Dict)
+	def dict_to_object(Class, Dict: dict):
+		try:
+			return Class(**Dict)
+		except TypeError:
+			return None
 
 
-	def read_dict(self, name, data_id) -> dict:
+	def read_dict(self, name: str, data_id: str) -> dict:
 		objects = self.execute(f'select data from {name} where id = \'{data_id}\'')
 		if len(objects) == 0:
 			return {}
 		return json.loads(objects[0][0])
 
 
-	def read_object(self, Class, name, object_id):
+	def read_object(self, Class, name: str, object_id: str):
 		return Database.dict_to_object(Class, self.read_dict(name, object_id))
 
 
-	def write_dict(self, name, data_id, data):
+	def write_dict(self, name:str, data_id: str, data: str):
 		data = json.dumps(data)
 		objects = self.execute(f'select data from {name} where id = \'{data_id}\'')
 		if len(objects) == 0:
 			self.execute(f'insert into {name}(id, data) values(\'{data_id}\', \'{data}\')')
 		else:
 			self.execute(f'update {name} set data = \'{data}\' where id = \'{data_id}\'')
 
 
-	def write_object(self, name, object_id, object):
+	def write_object(self, name: str, object_id: str, object: str):
 		self.write_dict(name, object_id, Database.object_to_dict(object))
```

### Comparing `spdb-1.0.2/spdb/generator_utils.py` & `spdb-1.0.3/spdb/generator_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import hashlib
 import base64
 import random
 
 
-def sha256(text: str):
+def sha256(text: str) -> str:
     m = hashlib.sha256()
     m.update(text.encode())
     return m.hexdigest()
 
 
 def b32encode(text: str) -> str:
 	return base64.b32encode(text.encode()).decode()
 
 
-def random_text(length=None) -> str:
+def random_text(length: int=None) -> str:
 	if length is None:
 		length = random.randint(1, 64)
 
 	BASE62 = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ123456789'
 
 	return ''.join(random.SystemRandom().choices(BASE62, k=length))
```

### Comparing `spdb-1.0.2/spdb/token_generator.py` & `spdb-1.0.3/spdb/token_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from spdb import generator_utils
 
 
 class TokenGenerator:
-	def __init__(self, code):
+	def __init__(self, code: str):
 		self.code = code
 
 
-	def gen(self, type: str, ID: str, key: str):
+	def gen(self, type: str, ID: str, key: str) -> stc:
 		return f'{self.code}.t.{type}.{ID}:{generator_utils.sha256(ID+generator_utils.sha256(key))}_{generator_utils.sha256(generator_utils.sha256(key)+ID+generator_utils.random_sha256())}'
 
 	@staticmethod
-	def parseToken(token: str):
+	def parse_token(token: str) -> dict:
 		return {
 			'code': token.split('.')[0],
 			'type': token.split('.')[2],
 			'ID': token.split('.')[3].split(':')[0],
 			'owner_hash': token.split('.')[3].split(':')[1].split('_')[0],
 			'token_hash': token.split('.')[3].split(':')[1].split('_')[1]
 		}
```

