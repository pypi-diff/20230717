# Comparing `tmp/pgsqlx-1.0.1.tar.gz` & `tmp/pgsqlx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.1.tar", last modified: Sun Jul 16 06:57:58 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.0.2.tar", last modified: Mon Jul 17 10:13:26 2023, max compression
```

## Comparing `pgsqlx-1.0.1.tar` & `pgsqlx-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-14 14:50:12.000000 pgsqlx-1.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx/
--rw-rw-rw-   0        0        0      678 2023-07-15 12:19:37.000000 pgsqlx-1.0.1/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    19259 2023-07-15 12:23:23.000000 pgsqlx-1.0.1/pgsqlx/db.py
--rw-rw-rw-   0        0        0    13886 2023-07-15 04:16:12.000000 pgsqlx-1.0.1/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.1/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    37094 2023-07-16 02:08:15.000000 pgsqlx-1.0.1/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.1/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.1/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6442 2023-07-15 12:25:53.000000 pgsqlx-1.0.1/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.1/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 04:29:07.000000 pgsqlx-1.0.1/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4292 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4292 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-07-16 06:57:53.000000 pgsqlx-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-14 14:50:12.000000 pgsqlx-1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx/
+-rw-rw-rw-   0        0        0      678 2023-07-15 12:19:37.000000 pgsqlx-1.0.2/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0    19259 2023-07-17 09:29:32.000000 pgsqlx-1.0.2/pgsqlx/db.py
+-rw-rw-rw-   0        0        0    13886 2023-07-17 09:29:32.000000 pgsqlx-1.0.2/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.2/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0    37747 2023-07-17 09:02:03.000000 pgsqlx-1.0.2/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.2/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.2/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6487 2023-07-17 09:30:08.000000 pgsqlx-1.0.2/pgsqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.2/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 04:29:07.000000 pgsqlx-1.0.2/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4292 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      365 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4292 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-07-17 10:12:52.000000 pgsqlx-1.0.2/setup.py
```

### Comparing `pgsqlx-1.0.1/LICENSE` & `pgsqlx-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/constant.py` & `pgsqlx-1.0.2/pgsqlx/constant.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/db.py` & `pgsqlx-1.0.2/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/dbx.py` & `pgsqlx-1.0.2/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/log_support.py` & `pgsqlx-1.0.2/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/orm.py` & `pgsqlx-1.0.2/pgsqlx/orm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
-from .support import DBError, simple_sql
+from .support import DBError, simple_sql, NotFoundError
 from typing import Sequence, Union, List, Tuple
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, PK_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, \
     PK_STRATEGY, COLUMN_SQL, CONFIG_DICT, CACHE_SIZE
 from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
     do_query_page, do_select_page, do_get
 from .log_support import logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, orm_find_by_id_log, \
     orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_ids_log
@@ -61,21 +61,21 @@
     """
 
     def __str__(self):
         return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
 
     def __getattr__(self, name):
         if PK == name:
-            return _get_pk(self.__class__)
+            return self._get_pk()
         elif TABLE == name:
-            return _get_table(self.__class__)
+            return self._get_table()
         elif UPDATE_BY == name:
-            return _get_update_by_field(self.__class__)
+            return self._get_update_by_field()
         elif UPDATE_TIME == name:
-            return _get_update_time_field(self.__class__)
+            return self._get_update_time_field()
         else:
             return None
 
     def persist(self):
         """
         person = Person(name='张三', age=55)
         effect_rowcount = person.persist()
@@ -89,233 +89,229 @@
         """
         person = Person(name='张三', age=55)
         id = person.save()
         :return: Primary key
         """
         orm_inst_log('inst_save', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        pk = _get_pk(self.__class__)
+        pk = self._get_pk()
         _id = self.save(**kv)
         if pk not in kv:
             self.__dict__.update({pk: _id})
         return _id
 
-    def update(self):
+    def update(self, ignored_none=True):
         """
         person = Person(id=1, name='李四', age=66)
         rowcount = person.update()
         :return: Effect rowcount
         """
         orm_inst_log('update', self.__class__.__name__)
-        pk, table = _get_pk_and_table(self.__class__)
-        kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        if pk not in kv:
-            raise KeyError("Not primary key.")
-
+        pk, table = self._get_pk_and_table()
+        if ignored_none:
+            kv = {k: v for k, v in self.__dict__.items() if v is not None}
+        else:
+            kv = {k: v for k, v in self.__dict__.items()}
+        _id = kv[pk]
+        assert _id is not None, 'Primary key must not be None.'
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
-            return self.update_by_id(kv[pk], **update_kv)
+            return self.update_by_id(_id, **update_kv)
         else:
             logger.warning("Exec func 'mysqlx.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
             return 0
 
     def load(self, *fields):
         """
         Return new object from database and update itself.
         :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
         person = Person(id=1)
         person2 = person.load()
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
-        pk = _get_pk(self.__class__)
+        pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
-        if _id is not None:
-            if not fields:
-                fields, _ = zip(*kv.items())
-            m = self.query_by_id(_id, *fields)
-            if m:
-                self.__dict__.update(m)
-                return self
-            else:
-                msg = "Exec func 'mysqlx.orm.Model.%s' load none, Class: '%s', %s=%d." % ('load', self.__class__.__name__, pk, _id)
-                logger.error(msg)
-                raise DBError(msg)
+        assert _id is not None, 'Primary key must not be None.'
+        if not fields:
+            fields, _ = zip(*kv.items())
+        result = self.query_by_id(_id, *fields)
+        if result:
+            self.__dict__.update(result)
+            return self
         else:
-            raise KeyError("Not primary key.")
+            raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, pk, _id))
 
     def logical_delete(self):
         """
         Logic delete only update the del flag
         person = Person(id=1)
         rowcount = person.logical_delete()
         """
         orm_inst_log('logical_delete', self.__class__.__name__)
-        pk = _get_pk(self.__class__)
-        _id = self.__dict__.get(pk)
-        update_by = self.__dict__.get(_get_update_by_field(self.__class__))
-        if _id is None:
-            raise KeyError("Not primary key.")
-
+        pk = self._get_pk()
+        kv = self.__dict__
+        _id = kv.get(pk)
+        assert _id is not None, 'Primary key must not be None.'
+        update_by = kv.get(self._get_update_by_field())
         return self.logical_delete_by_id(_id, update_by)
 
     def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         person = Person(id=1)
         rowcount = person.un_logical_delete()
         """
         orm_inst_log('un_logical_delete', self.__class__.__name__)
-        pk = _get_pk(self.__class__)
-        _id = self.__dict__.get(pk)
-        update_by = self.__dict__.get(self._get_update_by_field())
-        if _id is None:
-            raise KeyError("Not primary key.")
+        pk = self._get_pk()
+        kv = self.__dict__
+        _id = kv.get(pk)
+        assert _id is not None, 'Primary key must not be None.'
+        update_by = kv.get(self._get_update_by_field())
         return self.un_logical_delete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         person = Person(id=1)
         rowcount = person.delete()
         """
         orm_inst_log('delete', self.__class__.__name__)
-        pk = _get_pk(self.__class__)
+        pk = self._get_pk()
         _id = self.__dict__.get(pk)
-        if _id is None:
-            raise KeyError("Not primary key.")
+        assert _id is not None, 'Primary key must not be None.'
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = Person.insert(name='张三', age=20)
         return: Effect rowcount
         """
         orm_insert_log('insert', cls.__name__, **kwargs)
-        pk, table = _get_pk_and_table(cls)
-        pk_strategy = _get_pk_strategy(cls)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
             kwargs[pk] = get_id()
         return insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = Person.save(name='张三', age=20)
         :return: Primary key
         """
         orm_insert_log('save', cls.__name__, **kwargs)
-        pk, table = _get_pk_and_table(cls)
-        pk_strategy = _get_pk_strategy(cls)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE:
             if pk in kwargs:
                 _id = kwargs[pk]
             else:
                 _id = get_id()
                 kwargs[pk] = _id
             insert(table, **kwargs)
         else:
-            kwargs['pk_seq'] = _get_pk_seq(cls)
+            kwargs['pk_seq'] = cls._get_pk_seq()
             _id = save(table, **kwargs)
         return _id
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
         orm_insert_log('create', cls.__name__, **kwargs)
-        pk = _get_pk(cls)
+        pk = cls._get_pk()
         _id = cls.save(**kwargs)
         if pk not in kwargs:
             kwargs[pk] = _id
         return cls.to_obj(**kwargs)
 
     @classmethod
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = Person.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
-        pk = _get_pk(cls)
+        pk = cls._get_pk()
         where = '%s=?' % pk
         cols, args = zip(*kwargs.items())
-        sql, update_time_arg = _update_sql(cls, where, *cols)
+        sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
         return do_execute(sql, *args, _id)
 
     @classmethod
     def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = Person.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
-        return _logical_delete_by_id_op(cls, _id, update_by, DelFlag.DELETED)
+        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
     def un_logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = Person.un_logical_delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
-        return _logical_delete_by_id_op(cls, _id, update_by, DelFlag.UN_DELETE)
+        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
     def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = Person.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
-        return _logical_delete_by_ids_op(cls, ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
+        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
     def un_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = Person.un_logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         orm_logical_delete_by_ids_log('un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
-        return _logical_delete_by_ids_op(cls, ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
+        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
     def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
         rowcount = Person.delete_by('where name=? and age=?', '张三', 55)
         return: Effect rowcount
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = 'DELETE FROM %s %s' % (table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_execute(sql, *args)
 
     @classmethod
     def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
-        pk, table = _get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM %s WHERE %s=?' % (table, pk)
         return do_execute(sql, _id)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Batch physical delete, they will be executed in batches if there are too many
@@ -339,76 +335,76 @@
     def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         """
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         ids_size = len(ids)
-        pk, table = _get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
         return do_execute(sql, *ids)
 
     @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
         assert len(args) > 0, 'args must not be empty.'
-        pk, table = _get_pk_and_table(cls)
-        pk_strategy = _get_pk_strategy(cls)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE:
             for arg in args:
                 if pk not in arg:
                     arg[pk] = get_id()
 
         return batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = Person.count(name='张三', age=55)
         """
         orm_count_log('count', cls.__name__, **kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
         sql = _select_sql(table, where, LIMIT_1, fields)
         return do_get_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = Person.count_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = "SELECT count(1) FROM {} {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
         orm_count_log('exists', cls.__name__, **kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = "SELECT 1 FROM {} {} limit ?".format(table, where)
         return do_get_limit(sql, *args, LIMIT_1) == 1
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = "SELECT 1 FROM {} {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_get(sql, *args) == 1
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
@@ -489,15 +485,15 @@
         """
         Return list(dict) or empty list if no result.
         persons = Person.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('query', cls.__name__, *fields, **kwargs)
         where, args, limit = _get_where_arg_limit(**kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return do_query(sql, *args)
@@ -507,65 +503,65 @@
         """
         Return unique result(dict) or None if no result.
         persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('query_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_query_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.query_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
-        sql = _where_sql(cls, where)
+        sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query(sql, *args)
 
     @classmethod
     def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = Person.query_by_page(1, 10, 'where name=?', '李四')
         """
         orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        sql = _where_sql(cls, where)
+        sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
-        pk, table = _get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         where = 'WHERE {}=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_query_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
@@ -574,29 +570,29 @@
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = _get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         where = 'WHERE {} in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('select', cls.__name__, *fields, **kwargs)
         where, args, limit = _get_where_arg_limit(**kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return do_select(sql, *args)
@@ -606,65 +602,65 @@
         """
         Return unique result(tuple) or None if no result.
         row = Person.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('select_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_select_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
-        sql = _where_sql(cls, where)
+        sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select(sql, *args)
 
     @classmethod
     def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = _get_table(cls)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = Person.select_by_page(1, 10, 'where name=?', '李四')
         """
         orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        sql = _where_sql(cls, where)
+        sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
-        pk, table = _get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         where = 'WHERE {}=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_select_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
@@ -673,151 +669,151 @@
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = _get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         where = 'WHERE {} in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_select(sql, *ids, ids_size)
 
     @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
+    # ------------------------------------------------Private class method------------------------------------------------------------------
+    @classmethod
+    def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
+        pk, table = cls._get_pk_and_table()
+        del_flag_field = cls._get_del_flag_field()
+        update_by_field = cls._get_update_by_field()
 
-# ------------------------------------------------Private function------------------------------------------------------------------
-def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-    pk, table = _get_pk_and_table(cls)
-    del_flag_field = _get_del_flag_field(cls)
-    update_by_field = _get_update_by_field(cls)
-
-    where = '%s=?' % pk
-    if update_by is not None and update_by_field is not None:
-        sql, update_time_arg = _update_sql(cls, where, del_flag_field, update_by_field)
-        if update_time_arg:
-            return do_execute(sql, del_status.value, update_by, update_time_arg, _id)
-        return do_execute(sql, del_status.value, update_by, _id)
-    else:
-        sql, update_time_arg = _update_sql(cls, where, del_flag_field)
-        if update_time_arg:
-            return do_execute(sql, del_status.value, update_time_arg, _id)
-        return do_execute(sql, del_status.value, _id)
-
-
-def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
-        del_status=DelFlag.DELETED):
-    ids_size = len(ids)
-    assert ids_size > 0, 'ids must not be empty.'
-
-    if ids_size == 1:
-        return _logical_delete_by_id_op(cls, ids[0], update_by, del_status)
-    elif ids_size <= batch_size:
-        return _do_logical_delete_by_ids(cls, ids, update_by, del_status)
-    else:
-        split_ids = _split_ids(ids, batch_size)
-        with transaction():
-            results = [_do_logical_delete_by_ids(cls, ids, update_by, del_status) for ids in split_ids]
-        return sum(results)
-
-
-def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-    ids_size = len(ids)
-    pk = _get_pk(cls)
-    del_flag_field = _get_del_flag_field(cls)
-    update_by_field = _get_update_by_field(cls)
-
-    where = '%s in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
-    if update_by is not None and update_by_field is not None:
-        sql, update_time_arg = _update_sql(cls, where, del_flag_field, update_by_field)
-        if update_time_arg:
-            return do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
-        return do_execute(sql, del_status.value, update_by, *ids)
-    else:
-        sql, update_time_arg = _update_sql(cls, where, del_flag_field)
-        if update_time_arg:
-            return do_execute(sql, del_status.value, update_time_arg, *ids)
-        return do_execute(sql, del_status.value, *ids)
-
-
-def _get_pk(cls):
-    if hasattr(cls, PK):
-        return cls.__pk__
-    logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
-    return DEFAULT_PK_FIELD
-
-
-def _get_pk_seq(cls):
-    if hasattr(cls, PK_SEQ):
-        return cls.__pk_seq__
-    logger.warning("%s not set attribute '%s'" % (cls.__name__, PK_SEQ))
-    pk, table = _get_pk_and_table(cls)
-    return "{}_{}_seq".format(table, pk)
-
-
-def _get_table(cls):
-    if hasattr(cls, TABLE):
-        return cls.__table__
-    logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
-    return _get_table_name(cls.__name__)
-
+        where = '%s=?' % pk
+        if update_by is not None and update_by_field is not None:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
+            if update_time_arg:
+                return do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
+            return do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
+        else:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field)
+            if update_time_arg:
+                return do_execute(sql, del_status.value, update_time_arg, _id)
+            return do_execute(sql, del_status.value, _id)
 
-def _get_pk_and_table(cls):
-    return _get_pk(cls), _get_table(cls)
+    @classmethod
+    def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
+            del_status=DelFlag.DELETED):
+        ids_size = len(ids)
+        assert ids_size > 0, 'ids must not be empty.'
 
+        if ids_size == 1:
+            return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
+        elif ids_size <= batch_size:
+            return cls._do_logical_delete_by_ids(ids, update_by, del_status)
+        else:
+            split_ids = _split_ids(ids, batch_size)
+            with transaction():
+                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
+            return sum(results)
 
-def _get_pk_strategy(cls):
-    if hasattr(cls, PK_STRATEGY):
-        return cls.__pk_strategy__
-    return None
+    @classmethod
+    def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
+        pk = cls._get_pk()
+        del_flag_field = cls._get_del_flag_field()
+        update_by_field = cls._get_update_by_field()
+
+        where = '%s in (%s)' % (pk, ','.join(['?' for _ in range(len(ids))]))
+        if update_by is not None and update_by_field is not None:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
+            if update_time_arg:
+                return do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
+            return do_execute(sql, del_status.value, update_by, *ids)
+        else:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field)
+            if update_time_arg:
+                return do_execute(sql, del_status.value, update_time_arg, *ids)
+            return do_execute(sql, del_status.value, *ids)
 
+    @classmethod
+    def _get_pk(cls):
+        if hasattr(cls, PK):
+            return cls.__pk__
+        logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
+        return DEFAULT_PK_FIELD
 
-def _get_update_by_field(cls):
-    if hasattr(cls, UPDATE_BY):
-        return cls.__update_by__
-    return None
+    @classmethod
+    def _get_pk_seq(cls):
+        if hasattr(cls, PK_SEQ):
+            return cls.__pk_seq__
+        logger.warning("%s not set attribute '%s'" % (cls.__name__, PK_SEQ))
+        pk, table = cls._get_pk_and_table()
+        return "{}_{}_seq".format(table, pk)
 
+    @classmethod
+    def _get_table(cls):
+        if hasattr(cls, TABLE):
+            return cls.__table__
+        logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
+        return _get_table_name(cls.__name__)
 
-def _get_update_time_field(cls):
-    if hasattr(cls, UPDATE_TIME):
-        return cls.__update_time__
-    return None
+    @classmethod
+    def _get_pk_and_table(cls):
+        return cls._get_pk(), cls._get_table()
 
+    @classmethod
+    def _get_pk_strategy(cls):
+        if hasattr(cls, PK_STRATEGY):
+            return cls.__pk_strategy__
+        return None
 
-def _get_del_flag_field(cls):
-    assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
-    return cls.__del_flag__
+    @classmethod
+    def _get_update_by_field(cls):
+        if hasattr(cls, UPDATE_BY):
+            return cls.__update_by__
+        return None
 
+    @classmethod
+    def _get_update_time_field(cls):
+        if hasattr(cls, UPDATE_TIME):
+            return cls.__update_time__
+        return None
 
-def _update_sql(cls, where, *update_fields):
-    update_time_arg = None
-    table = _get_table(cls)
-    update_time_field = _get_update_time_field(cls)
-    if update_time_field is not None and update_time_field not in update_fields:
-        update_fields = [*update_fields, update_time_field]
-        update_time_arg = datetime.now()
+    @classmethod
+    def _get_del_flag_field(cls):
+        assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
+        return cls.__del_flag__
 
-    update_fields = ','.join(['{}=?'.format(col) for col in update_fields])
-    return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
+    @classmethod
+    def _update_sql(cls, where, *update_fields):
+        update_time_arg = None
+        table = cls._get_table()
+        update_time_field = cls._get_update_time_field()
+        if update_time_field is not None and update_time_field not in update_fields:
+            update_fields = [*update_fields, update_time_field]
+            update_time_arg = datetime.now()
 
+        update_fields = ','.join(['{}=?'.format(col) for col in update_fields])
+        return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
 
-def _where_sql(cls, where: str):
-    low_where = where.lower()
-    if low_where.startswith('where'):
-        table = _get_table(cls)
-        return _select_sql(table, where, NO_LIMIT)
-    elif low_where.startswith('select'):
-        return where
-    raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
+    @classmethod
+    def _where_sql(cls, where: str):
+        low_where = where.lower()
+        if low_where.startswith('where'):
+            table = cls._get_table()
+            return _select_sql(table, where, NO_LIMIT)
+        elif low_where.startswith('select'):
+            return where
+        raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
 
 
+# ----------------------------------------------------------Private function------------------------------------------------------------------
 def _select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
     if fields:
         fields = ','.join([col if '(' in col else '{}'.format(col) for col in fields])
     else:
         fields = _get_table_columns(table)
 
     if limit:
```

### Comparing `pgsqlx-1.0.1/pgsqlx/snowflake.py` & `pgsqlx-1.0.2/pgsqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/sql_mapper.py` & `pgsqlx-1.0.2/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/pgsqlx/support.py` & `pgsqlx-1.0.2/pgsqlx/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,18 @@
     pass
 
 
 class MapperError(DBError):
     pass
 
 
+class NotFoundError(DBError):
+    pass
+
+
 class MultiColumnsError(DBError):
     pass
 
 
 class Dict(dict):
     def __init__(self, names=(), values=(), **kw):
         super(Dict, self).__init__(**kw)
```

### Comparing `pgsqlx-1.0.1/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.0.2/pgsqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.1
+Version: 1.0.2
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.1/PKG-INFO` & `pgsqlx-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.1
+Version: 1.0.2
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.1/README.rst` & `pgsqlx-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.1/setup.py` & `pgsqlx-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
     ],
-    version='1.0.1',
+    version='1.0.2',
     url='https://gitee.com/summry/pgsqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

