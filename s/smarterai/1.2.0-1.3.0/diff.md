# Comparing `tmp/smarterai-1.2.0.tar.gz` & `tmp/smarterai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smarterai-1.2.0.tar", last modified: Wed Mar 22 19:03:08 2023, max compression
+gzip compressed data, was "dist/smarterai-1.3.0.tar", last modified: Mon Jul 17 16:06:16 2023, max compression
```

## Comparing `smarterai-1.2.0.tar` & `smarterai-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:03:08.000000 smarterai-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-03-22 19:02:48.000000 smarterai-1.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7027 2023-03-22 19:03:08.000000 smarterai-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5307 2023-03-22 19:02:48.000000 smarterai-1.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-03-22 19:02:48.000000 smarterai-1.2.0/VERSION.txt
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-22 19:02:48.000000 smarterai-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-03-22 19:03:08.000000 smarterai-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-22 19:02:48.000000 smarterai-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:03:08.000000 smarterai-1.2.0/smarterai/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-03-22 19:02:48.000000 smarterai-1.2.0/smarterai/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26555 2023-03-22 19:02:48.000000 smarterai-1.2.0/smarterai/smarterApi.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-03-22 19:02:48.000000 smarterai-1.2.0/smarterai/smarterInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8025 2023-03-22 19:02:48.000000 smarterai-1.2.0/smarterai/smarterStore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:03:08.000000 smarterai-1.2.0/smarterai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7027 2023-03-22 19:03:07.000000 smarterai-1.2.0/smarterai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2023-03-22 19:03:08.000000 smarterai-1.2.0/smarterai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 19:03:07.000000 smarterai-1.2.0/smarterai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-22 19:03:07.000000 smarterai-1.2.0/smarterai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:06:16.000000 smarterai-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-17 16:05:58.000000 smarterai-1.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-07-17 16:06:16.000000 smarterai-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5307 2023-07-17 16:05:58.000000 smarterai-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-17 16:05:58.000000 smarterai-1.3.0/VERSION.txt
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-17 16:05:58.000000 smarterai-1.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-17 16:06:16.000000 smarterai-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-17 16:05:58.000000 smarterai-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30853 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/smarterApi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/smarterInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8025 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/smarterStore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/top_level.txt
```

### Comparing `smarterai-1.2.0/LICENSE.txt` & `smarterai-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smarterai-1.2.0/PKG-INFO` & `smarterai-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterai
-Version: 1.2.0
+Version: 1.3.0
 Summary: smarter.ai Python API
 Home-page: https://www.smarter.ai/
 Author: Nevine Soliman and Carlos Medina
 Author-email: dev@smarter.ai
 License: UNKNOWN
 Description: [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
         [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip/)
```

### Comparing `smarterai-1.2.0/README.md` & `smarterai-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `smarterai-1.2.0/setup.cfg` & `smarterai-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `smarterai-1.2.0/setup.py` & `smarterai-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `smarterai-1.2.0/smarterai/smarterApi.py` & `smarterai-1.3.0/smarterai/smarterApi.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,19 @@
 
 
 class SmarterApi:
     def __init__(self,
                  app_slug: str,
                  deploy_dir: str,
                  delegate: Callable[[SmarterMessage, str], Optional[SmarterMessage]],
-                 user_id: str,
-                 user_email: str,
                  db,
                  task_manager):
         self.__smarter_store = SmarterStore(deploy_dir=deploy_dir)
         self.__core = self.__smarter_store.get_manifest_property(property_sequence="core")
         self.__usage_key = "_usageKey"
-        self.__user_id = user_id
-        self.__user_email = user_email
         self.delegate = delegate
         self.__db = db
         self.app_slug = app_slug
         self.task_manager = task_manager
 
     @staticmethod
     def __is_number(val: Any) -> bool:
@@ -78,14 +74,87 @@
         return usage_data[exp_slug]
 
     def __get_usage(self, user_id: str) -> int:
         usage_data = self.__smarter_store.read_global_store(pattern=self.__usage_key)
         exp_slug = self.__core.get("expSlug")
         return usage_data.get(user_id, {}).get(exp_slug, 0)
 
+    def __get_user(self, schema_id: str, user_id: str, data_type_filter: str = None) -> Tuple:
+        """
+           Gets the current user's previously persisted data.
+            Args:
+                :param data_type_filter:  Optional - It can be used to identify what type of data are you getting.
+                    Use this if you had data_type_id in SmarterApi.set_user_data
+                :param user_id: Ignored for backward compatability
+           Returns:
+                A tuple of all current user's data
+        """
+        if not user_id or not schema_id:
+            logger.error(f"set_user_data found missing ids for the current message. "
+                         f"Got currentId: {user_id} and schemaId: {schema_id}")
+            return ()
+        if not self.check_table_exists(schema_name=schema_id, table_name='static'):
+            return ()
+        if data_type_filter:
+            query = f"SELECT rawdata " \
+                    f"FROM {schema_id}.static " \
+                    f"WHERE type='{self.app_slug}' " \
+                    f"AND sourcetype='APP' " \
+                    f"AND subtype='{data_type_filter}'" \
+                    f"AND custid='{user_id}'"
+        else:
+            query = f"SELECT rawdata " \
+                    f"FROM {schema_id}.static " \
+                    f"WHERE type='{self.app_slug}' " \
+                    f"AND sourcetype='APP' " \
+                    f"AND custid='{user_id}'"
+        return self.query_data_lake(sql_query=query, commit=False)
+
+    def __set_user(self, schema_id: str, user_id: str, data: Any, data_type_id: str = None) -> None:
+        def merge_data(old_data: Any, new_data: Any) -> Any:
+            if type(old_data) == type(new_data) == dict:
+                return {**old_data, **new_data}
+            else:
+                return new_data
+
+        existing_data = self.__get_user(schema_id=schema_id,
+                                        user_id=user_id,
+                                        data_type_filter=data_type_id)
+        existing_data = existing_data[0][0] if existing_data else None
+        updated_data = merge_data(old_data=existing_data, new_data=data)
+        try:
+            string_data = json.dumps(updated_data)
+        except Exception:
+            logger.error(f"Failed to convert user data to JSON for the user {user_id}")
+            logger.error(traceback.format_exc())
+            return
+        if data_type_id:
+            insert_query = "INSERT INTO %s.static (custid, type, sourcetype, subtype, rawdata, normdata) " \
+                           "VALUES %s" % (
+                               schema_id,
+                               (user_id, self.app_slug, 'APP', data_type_id, string_data, '{}'))
+
+            delete_query = f"DELETE FROM {schema_id}.static " \
+                           f"WHERE type='{self.app_slug}' " \
+                           f"AND sourcetype='APP' " \
+                           f"AND custid='{user_id}'" \
+                           f"AND subtype='{data_type_id}'"
+
+        else:
+            insert_query = "INSERT INTO %s.static (custid, type, sourcetype, rawdata, normdata) " \
+                           "VALUES %s" % (schema_id, (user_id, self.app_slug, 'APP', string_data, '{}'))
+
+            delete_query = f"DELETE FROM {schema_id}.static " \
+                           f"WHERE type='{self.app_slug}' " \
+                           f"AND sourcetype='APP'" \
+                           f"AND custid='{user_id}'"
+
+        self.query_data_lake(sql_query=delete_query)
+        self.query_data_lake(sql_query=insert_query)
+
     def get_app_slug(self) -> str:
         """Returns the current app's slug"""
         return self.app_slug
 
     def send_message(self, message: SmarterMessage, port: str) -> Optional[SmarterMessage]:
         """
         Takes in a message from a python code component and sends it to its output port.
@@ -102,70 +171,70 @@
         :param data: The data to be sent to the GUI. It needs to match the format the pattern expects the data in.
                         Example a chart expects a table-like format, while a textField expects some text.
         :return: None
         """
         message = SmarterMessage({"action": "setData",
                                   "args": {"pattern": pattern, "data": data}})
         return_message = self.send_message(message=message, port='#gui')
-        user_id = return_message.get("user", {}).get("id")
-        self.__smarter_store.set_pattern_data(pattern=pattern, data=data, user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        self.__smarter_store.set_pattern_data(pattern=pattern, data=data, user_id=current_user_id)
 
     def clear_data(self, pattern: str) -> None:
         """
         Clears any data associated with a specific pattern in the GUI components
         :param pattern: The front-end GUI pattern to set the data to
         :return: None
         """
         message = SmarterMessage({"action": "setData",
                                   "args": {"pattern": pattern, "data": None}})
         return_message = self.send_message(message=message, port='#gui')
-        user_id = return_message.get("user", {}).get("id")
-        self.__smarter_store.set_pattern_data(pattern=pattern, data=None, user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        self.__smarter_store.set_pattern_data(pattern=pattern, data=None, user_id=current_user_id)
 
     def append_data(self, pattern: str, data: Any, limit: int) -> None:
         """
         Appends new data to previously sent data to a specific pattern.
         :param pattern: The front-end GUI pattern to append the data to.
         :param data: The data to be appended to a GUI component's previous data.
         :param limit: If the data's total size is bigger than limit, then a sliding window will be implemented to hold
             the latest added elements
         :return: None
         """
         message = SmarterMessage({"action": "setData",
                                   "args": {"pattern": pattern, "data": data if type(data) == list else [data]},
                                   "options": {"append": True, "limitLength": limit}})
         return_message = self.send_message(message=message, port='#gui')
-        user_id = return_message.get("user", {}).get("id")
-        self.__smarter_store.append_pattern_data(pattern=pattern, data=data, user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        self.__smarter_store.append_pattern_data(pattern=pattern, data=data, user_id=current_user_id)
 
     def prepend_data(self, pattern: str, data: Any, limit: int) -> None:
         """
         Prepends new data to previously sent data to a specific pattern.
         :param pattern: The front-end GUI pattern to append the data to.
         :param data: The data to be prepended to a GUI component's previous data.
         :param limit: If the data's total size is bigger than limit, then a sliding window will be implemented to hold
             the latest added elements
         :return: None
         """
         message = SmarterMessage({"action": "setData",
                                   "args": {"pattern": pattern, "data": data if type(data) == list else [data]},
                                   "options": {"prepend": True, "limitLength": limit}})
         return_message = self.send_message(message=message, port='#gui')
-        user_id = return_message.get("user", {}).get("id")
-        self.__smarter_store.prepend_pattern_data(pattern=pattern, data=data, user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        self.__smarter_store.prepend_pattern_data(pattern=pattern, data=data, user_id=current_user_id)
 
     def get_data(self, pattern: str) -> Any:
         """
         Returns the data set to a specific pattern if it exists, otherwise returns None
         :param pattern: The pattern to return
         :return: json serializable SmarterMessage
         """
         return_message = self.send_message(message=SmarterMessage(), port="#user")
-        user_id = return_message.get("user", {}).get("id")
-        return self.__smarter_store.get_pattern_data(pattern=pattern, user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        return self.__smarter_store.get_pattern_data(pattern=pattern, user_id=current_user_id)
 
     def reply_back(self, message: SmarterMessage) -> None:
         """
         Takes in a message to reply back to front-end REST/Websocket topics. An equivalent  to 'return' with a message.
         Uses built-in port #action to identify the front-end topic
         :param message: A SmarterMessage JSON Serializable
         :return: None
@@ -241,28 +310,29 @@
         can be used to track the usage of the users of the solutions and allowing them to "try" it in a limited fashion.
         :param increment_value: incremental value to be added to the user's usage counter
         :return: The user's updated usage.
                  Returns -1 if they reached or exceeded the trial limit.
                  Returns 0 if no trial limit was set
                  Otherwise returns a value >= 1 depending on the user's current usage after increment.
         """
+        # TODO: use currentId for the user Id
         return_message = self.send_message(message=SmarterMessage(), port="#user")
-        user_id = return_message.get("user", {}).get("id")
-        return self.__increment_usage(increment_value, user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        return self.__increment_usage(increment_value, user_id=current_user_id)
 
     def get_usage(self) -> int:
         """
         Gets the current trial usage of the user.
         :return: The user's current usage.
                  Returns 0 if no trial limit was set or if the user is the solution's creator
                  Otherwise returns a value >= 1 depending on the user's current usage.
         """
         return_message = self.send_message(message=SmarterMessage(), port="#user")
-        user_id = return_message.get("user", {}).get("id")
-        return self.__get_usage(user_id=user_id)
+        current_user_id = return_message.get("user", {}).get("currentId")
+        return self.__get_usage(user_id=current_user_id)
 
     def query_data_lake(self, sql_query: str, parameters=None, paramstyle: str = "format", commit=True, *args,
                         **kwargs) -> Tuple:
         """
         Takes an SQL query on the data lake and returns all remaining rows of a query result.
         Args:
             :param sql_query: The SQL statement to execute on the data Lake
@@ -308,55 +378,58 @@
                                        **kwargs)
 
     def set_user_data(self, data: Any, user_id: str = None, data_type_id: str = None) -> None:
         """
         Persists user-specific data in the data lake. This can be handy for shared apps,
         rebooting/restarting apps, and running apps in a stateless manner.
         Args:
-            :param user_id: Optional, it will default to the current user, but you can set to other users
             :param data: JSON Serializable dictionary that will be stored in the user's data lake
             :param data_type_id:  Optional - It can be used to identify what type of data are you setting.
                 This will help in indexing and retrieving relevant data when using get_user_data.
+            :param user_id: Ignored for backward compatability
        Returns:
             None
         """
-
-        def merge_data(old_data: Any, new_data: Any) -> Any:
-            if type(old_data) == type(new_data) == dict:
-                return {**old_data, **new_data}
-            else:
-                return new_data
-
-        if not user_id:
-            return_message = self.send_message(message=SmarterMessage(), port="#user")
-            user_id = return_message.get("user", {}).get("id")
-        existing_data = self.get_user_data(user_id=user_id, data_type_filter=data_type_id)
-        existing_data = existing_data[0][0] if existing_data else None
-        updated_data = merge_data(old_data=existing_data, new_data=data)
-        try:
-            string_data = json.dumps(updated_data)
-        except Exception:
-            logger.error(f"Failed to convert user data to JSON for the user {user_id}")
-            logger.error(traceback.format_exc())
+        if user_id is not None:
+            logger.warning("DeprecationWarning: use of user_id in set_user_data is deprecated and will be ignored!")
+        return_message = self.send_message(message=SmarterMessage(), port="#user")
+        current_user_id = return_message.get("user", {}).get("currentId")
+        current_schema_id = return_message.get("user", {}).get("currentSchema")
+        if not current_user_id or not current_schema_id:
+            logger.error(f"set_user_data found missing ids for the current message. "
+                         f"Got currentId: {current_user_id} and schemaId: {current_schema_id}")
             return
-        if data_type_id:
-            insert_query = "INSERT INTO %s.static (type, sourcetype, otherid, rawdata, normdata) " \
-                           "VALUES %s" % (user_id, (self.app_slug, 'APP', data_type_id, string_data, '{}'))
-
-            delete_query = f"DELETE FROM {user_id}.static " \
-                           f"WHERE type='{self.app_slug}' AND sourcetype='APP' AND otherid='{data_type_id}'"
-        else:
-            insert_query = "INSERT INTO %s.static (type, sourcetype, rawdata, normdata) " \
-                           "VALUES %s" % (user_id, (self.app_slug, 'APP', string_data, '{}'))
+        self.__set_user(schema_id=current_schema_id,
+                        user_id=current_user_id,
+                        data=data,
+                        data_type_id=data_type_id)
 
-            delete_query = f"DELETE FROM {user_id}.static " \
-                           f"WHERE type='{self.app_slug}' AND sourcetype='APP'"
+    def set_user_session(self, data: Any, data_type_id: str = None) -> None:
+        """
+        Persists user's session-specific data in the data lake. This can be handy for apps remembering the user's
+        session's usage data
+        Args:
+            :param data: JSON Serializable dictionary that will be stored in the user's data lake
+            :param data_type_id:  Optional - It can be used to identify what type of data are you setting.
+                This will help in indexing and retrieving relevant data when using get_user_data.
+       Returns:
+            None
+        """
 
-        self.query_data_lake(sql_query=delete_query)
-        self.query_data_lake(sql_query=insert_query)
+        return_message = self.send_message(message=SmarterMessage(), port="#user")
+        user_id = return_message.get("user", {}).get("userId")
+        current_schema_id = return_message.get("user", {}).get("currentSchema")
+        if not user_id or not current_schema_id:
+            logger.error(f"set_user_data found missing ids for the current message. "
+                         f"Got currentId: {user_id} and schemaId: {current_schema_id}")
+            return
+        self.__set_user(schema_id=current_schema_id,
+                        user_id=user_id,
+                        data=data,
+                        data_type_id=data_type_id)
 
     def check_table_exists(self, table_name: str, schema_name: str = None) -> bool:
         """
         Checks if a table exists in the Data Lake.
         Usage Examples:
         1. check_table_exists(table_name='static')
             => Returns True if <current_user_id>.static exists
@@ -371,54 +444,49 @@
             schema_name: the schema for the table. If not provided it will default to the current user's ID.
 
         Returns:
             True if the schema_name.table_name exits, False otherwise
         """
         if not schema_name:
             return_message = self.send_message(message=SmarterMessage(), port="#user")
-            schema_name = return_message.get("user", {}).get("id")
+            current_schema_id = return_message.get("user", {}).get("currentSchema")
         if "." in table_name:
             s_t = table_name.split(".")
             if len(s_t) != 2:
                 return False
-            schema_name = s_t[0]
+            current_schema_id = s_t[0]
             table_name = s_t[1]
         query = f"SELECT EXISTS (" \
                 f"SELECT FROM pg_tables " \
-                f"WHERE schemaname = '{schema_name}'" \
+                f"WHERE schemaname = '{current_schema_id}'" \
                 f"AND tablename  = '{table_name}')"
         res = self.query_data_lake(sql_query=query, commit=False)
         return res[0][0] if res else False
 
     def get_user_data(self, user_id: str = None, data_type_filter: str = None) -> Tuple:
         """
            Gets the current user's previously persisted data.
             Args:
-                :param user_id: Optional, it will default to the current user, but you can set to other users
                 :param data_type_filter:  Optional - It can be used to identify what type of data are you getting.
                     Use this if you had data_type_id in SmarterApi.set_user_data
+                :param user_id: Ignored for backward compatability
            Returns:
                 A tuple of all current user's data
         """
-        if not user_id:
-            return_message = self.send_message(message=SmarterMessage(), port="#user")
-            user_id = return_message.get("user", {}).get("id")
-        if not self.check_table_exists(schema_name=user_id, table_name='static'):
-            return ()
-        if not data_type_filter:
-            query = f"SELECT rawdata " \
-                    f"FROM {user_id}.static " \
-                    f"WHERE type='{self.app_slug}' AND sourcetype='APP'"
-        else:
-            query = f"SELECT rawdata " \
-                    f"FROM {user_id}.static " \
-                    f"WHERE type='{self.app_slug}' AND sourcetype='APP' AND otherid='{data_type_filter}'"
-        return self.query_data_lake(sql_query=query, commit=False)
+        if user_id is not None:
+            logger.warning("DeprecationWarning: use of user_id in get_user_data is deprecated and will be ignored!")
+        return_message = self.send_message(message=SmarterMessage(), port="#user")
+        current_user_id = return_message.get("user", {}).get("currentId")
+        current_schema_id = return_message.get("user", {}).get("currentSchema")
+        return self.__get_user(schema_id=current_schema_id,
+                               user_id=current_user_id,
+                               data_type_filter=data_type_filter)
 
-    def notify_data_lake(self, table: str, user_id: str, source_type: str, type: str, last_id: Union[str, int]) -> None:
+    def notify_data_lake(self, table: str, user_id: str, source_type: str, type: str,
+                         last_id: Union[str, int, None]) -> None:
         """
         Notifies the data lake that an update has happened in case of some listeners watching for lake updates
         Args:
             table: Table name, 'events' or 'static'
             user_id: The id for the relevant user
             source_type: Source type that is updated in the data lake
             type: type that is updated in the data lake
@@ -431,14 +499,24 @@
                                   "userId": user_id,
                                   "type": type,
                                   "sourceType": source_type,
                                   "lastId": last_id})
         self.send_message(message=message, port='#lake')
         pass
 
+    def get_user_id(self) -> str:
+        """
+
+        :return: The current user's ID of type string. If no user exists (ex. calling get_user_id in boot)
+                the returned string will be an empty string
+        """
+        return_message = self.send_message(message=SmarterMessage(), port="#user")
+        current_user_id = return_message.get("user", {}).get("currentId", "")
+        return current_user_id
+
     def submit_task(self, app_task: Callable, maintain_sequential_execution=True, callback: Callable = None,
                     *args, **kwargs) -> None:
         """
         Time Expensive tasks can be executed in a threading environment to free up the main App thread
         to receive and process other messages easily. An expensive task can be training step, inference, etc.
         The API allows you to submit the function(s) (called tasks) you want to run,
         along with the functions’ parameters, and a flag to specify if you want to run multiple submitted tasks
@@ -459,16 +537,16 @@
             **kwargs:  All the keywords arguments you wish to pass to the app_task callable.
                 Make sure not to use core_user_id as that is unique to the api, and it will be overwritten.
 
         Returns:
             None
         """
         return_message = self.send_message(message=SmarterMessage(), port="#user")
-        core_user_id = return_message.get("user", {}).get("id")
-        self.task_manager.submit_task(core_user_id=core_user_id,
+        current_core_user_id = return_message.get("user", {}).get("currentId")
+        self.task_manager.submit_task(core_user_id=current_core_user_id,
                                       app_task=app_task,
                                       maintain_sequential_execution=maintain_sequential_execution,
                                       callback=callback,
                                       *args, **kwargs)
 
     def get_tasks_results(self, wait_for_return: bool = False, as_completed: bool = True,
                           clean_up_results: bool = False) -> Optional[list]:
@@ -488,36 +566,36 @@
                     it means that for each get_tasks_results you will receive a list of all the submitted tasks results.
                     If this is not a behaviour you want, then you need to set clean_up_results=True
 
             Returns:
                 List of returned results from each submitted task for the current user.
         """
         return_message = self.send_message(message=SmarterMessage(), port="#user")
-        core_user_id = return_message.get("user", {}).get("id")
+        current_core_user_id = return_message.get("user", {}).get("currentId")
         try:
-            res = self.task_manager.get_result(user_id=core_user_id,
+            res = self.task_manager.get_result(user_id=current_core_user_id,
                                                as_completed=as_completed,
                                                wait=wait_for_return,
                                                clean_up=clean_up_results)
             return res
         except Exception:
-            logger.error(f"Failed to get task results for user: {core_user_id}")
+            logger.error(f"Failed to get task results for user: {current_core_user_id}")
             logger.error(traceback.format_exc())
 
     def is_busy(self) -> bool:
         """
         Checks if the current user's thread(s) are busy executing tasks.
         It will raise InvalidUserException if the current user has been idle for a while/hasn't submitted
         a task recently.
         Returns:
             True if the current user's thread is busy with a previously submitted task
         """
         return_message = self.send_message(message=SmarterMessage(), port="#user")
-        user_id = return_message.get("user", {}).get("id")
+        current_user_id = return_message.get("user", {}).get("currentId")
         try:
-            return self.task_manager.is_busy(user_id=user_id)
+            return self.task_manager.is_busy(user_id=current_user_id)
         except Exception:
-            logger.error(f"Failed to check status for user{user_id}")
+            logger.error(f"Failed to check status for user{current_user_id}")
             logger.error(traceback.format_exc())
 
 
 SmarterSender = SmarterApi
```

### Comparing `smarterai-1.2.0/smarterai/smarterInterface.py` & `smarterai-1.3.0/smarterai/smarterInterface.py`

 * *Files identical despite different names*

### Comparing `smarterai-1.2.0/smarterai/smarterStore.py` & `smarterai-1.3.0/smarterai/smarterStore.py`

 * *Files identical despite different names*

### Comparing `smarterai-1.2.0/smarterai.egg-info/PKG-INFO` & `smarterai-1.3.0/smarterai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterai
-Version: 1.2.0
+Version: 1.3.0
 Summary: smarter.ai Python API
 Home-page: https://www.smarter.ai/
 Author: Nevine Soliman and Carlos Medina
 Author-email: dev@smarter.ai
 License: UNKNOWN
 Description: [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
         [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip/)
```

