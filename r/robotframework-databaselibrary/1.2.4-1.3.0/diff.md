# Comparing `tmp/robotframework-databaselibrary-1.2.4.tar.gz` & `tmp/robotframework-databaselibrary-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-databaselibrary-1.2.4.tar", last modified: Thu Jul 18 17:44:40 2019, max compression
+gzip compressed data, was "robotframework-databaselibrary-1.3.0.tar", last modified: Mon Jul 17 17:25:52 2023, max compression
```

## Comparing `robotframework-databaselibrary-1.2.4.tar` & `robotframework-databaselibrary-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2019-07-18 17:44:40.000000 robotframework-databaselibrary-1.2.4/
--rw-rw-rw-   0        0        0      359 2019-07-18 17:44:40.000000 robotframework-databaselibrary-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      303 2019-07-18 15:05:58.000000 robotframework-databaselibrary-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2019-07-18 17:44:40.000000 robotframework-databaselibrary-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1579 2019-07-18 15:05:58.000000 robotframework-databaselibrary-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2019-07-18 17:44:40.000000 robotframework-databaselibrary-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2019-07-18 17:44:40.000000 robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/
--rw-rw-rw-   0        0        0    12068 2019-07-18 15:05:58.000000 robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/assertion.py
--rw-rw-rw-   0        0        0     9680 2019-07-18 15:05:58.000000 robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/connection_manager.py
--rw-rw-rw-   0        0        0    15414 2019-07-18 15:05:58.000000 robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/query.py
--rw-rw-rw-   0        0        0       19 2019-07-18 17:41:33.000000 robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/version.py
--rw-rw-rw-   0        0        0     2572 2019-07-18 15:05:58.000000 robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2019-07-18 17:44:40.000000 robotframework-databaselibrary-1.2.4/src/robotframework_databaselibrary.egg-info/
--rw-rw-rw-   0        0        0        1 2019-07-18 17:44:39.000000 robotframework-databaselibrary-1.2.4/src/robotframework_databaselibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      359 2019-07-18 17:44:39.000000 robotframework-databaselibrary-1.2.4/src/robotframework_databaselibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2019-07-18 17:44:39.000000 robotframework-databaselibrary-1.2.4/src/robotframework_databaselibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2019-07-18 17:44:39.000000 robotframework-databaselibrary-1.2.4/src/robotframework_databaselibrary.egg-info/top_level.txt
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.982480 robotframework-databaselibrary-1.3.0/
+-rw-r--r--   0 andremochinin   (501) staff       (20)      570 2023-07-11 18:41:08.000000 robotframework-databaselibrary-1.3.0/LICENSE
+-rw-r--r--   0 andremochinin   (501) staff       (20)     4195 2023-07-17 17:25:52.982344 robotframework-databaselibrary-1.3.0/PKG-INFO
+-rw-r--r--   0 andremochinin   (501) staff       (20)     2900 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/README.md
+-rw-r--r--   0 andremochinin   (501) staff       (20)      913 2023-07-17 17:25:42.000000 robotframework-databaselibrary-1.3.0/pyproject.toml
+-rw-r--r--   0 andremochinin   (501) staff       (20)       38 2023-07-17 17:25:52.982522 robotframework-databaselibrary-1.3.0/setup.cfg
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.979577 robotframework-databaselibrary-1.3.0/src/
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.981253 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/
+-rw-r--r--   0 andremochinin   (501) staff       (20)     2955 2023-07-17 17:15:49.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/__init__.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)    14306 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/assertion.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)    13763 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/connection_manager.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)    22829 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/query.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)       18 2023-07-17 17:14:02.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/version.py
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.982133 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/
+-rw-r--r--   0 andremochinin   (501) staff       (20)     4195 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/PKG-INFO
+-rw-r--r--   0 andremochinin   (501) staff       (20)      488 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 andremochinin   (501) staff       (20)        1 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 andremochinin   (501) staff       (20)       39 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/requires.txt
+-rw-r--r--   0 andremochinin   (501) staff       (20)       16 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/assertion.py` & `robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/assertion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,252 @@
-#  Copyright (c) 2010 Franz Allan Valencia See
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-from robot.api import logger
-
-
-class Assertion(object):
-    """
-    Assertion handles all the assertions of Database Library.
-    """
-
-    def check_if_exists_in_database(self, selectStatement, sansTran=False):
-        """
-        Check if any row would be returned by given the input `selectStatement`. If there are no results, then this will
-        throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit transaction
-        commit or rollback.
-
-        For example, given we have a table `person` with the following data:
-        | id | first_name  | last_name |
-        |  1 | Franz Allan | See       |
-
-        When you have the following assertions in your robot
-        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' |
-        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' |
-
-        Then you will get the following:
-        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' | # PASS |
-        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' | # FAIL |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' | True |
-        """
-        logger.info ('Executing : Check If Exists In Database  |  %s ' % selectStatement)
-        if not self.query(selectStatement, sansTran):
-            raise AssertionError("Expected to have have at least one row from '%s' "
-                                 "but got 0 rows." % selectStatement)
-
-    def check_if_not_exists_in_database(self, selectStatement, sansTran=False):
-        """
-        This is the negation of `check_if_exists_in_database`.
-
-        Check if no rows would be returned by given the input `selectStatement`. If there are any results, then this
-        will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
-        transaction commit or rollback.
-
-        For example, given we have a table `person` with the following data:
-        | id | first_name  | last_name |
-        |  1 | Franz Allan | See       |
-
-        When you have the following assertions in your robot
-        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'John' |
-        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' |
-
-        Then you will get the following:
-        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'John' | # PASS |
-        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' | # FAIL |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'John' | True |
-        """
-        logger.info('Executing : Check If Not Exists In Database  |  %s ' % selectStatement)
-        queryResults = self.query(selectStatement, sansTran)
-        if queryResults:
-            raise AssertionError("Expected to have have no rows from '%s' "
-                                 "but got some rows : %s." % (selectStatement, queryResults))
-
-    def row_count_is_0(self, selectStatement, sansTran=False):
-        """
-        Check if any rows are returned from the submitted `selectStatement`. If there are, then this will throw an
-        AssertionError. Set optional input `sansTran` to True to run command without an explicit transaction commit or
-        rollback.
-
-        For example, given we have a table `person` with the following data:
-        | id | first_name  | last_name |
-        |  1 | Franz Allan | See       |
-
-        When you have the following assertions in your robot
-        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'Franz Allan' |
-        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'John' |
-
-        Then you will get the following:
-        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'Franz Allan' | # FAIL |
-        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'John' | # PASS |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'John' | True |
-        """
-        logger.info('Executing : Row Count Is 0  |  %s ' % selectStatement)
-        num_rows = self.row_count(selectStatement, sansTran)
-        if num_rows > 0:
-            raise AssertionError("Expected zero rows to be returned from '%s' "
-                                 "but got rows back. Number of rows returned was %s" % (selectStatement, num_rows))
-
-    def row_count_is_equal_to_x(self, selectStatement, numRows, sansTran=False):
-        """
-        Check if the number of rows returned from `selectStatement` is equal to the value submitted. If not, then this
-        will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
-        transaction commit or rollback.
-
-        For example, given we have a table `person` with the following data:
-        | id | first_name  | last_name |
-        |  1 | Franz Allan | See       |
-        |  2 | Jerry       | Schneider |
-
-        When you have the following assertions in your robot
-        | Row Count Is Equal To X | SELECT id FROM person | 1 |
-        | Row Count Is Equal To X | SELECT id FROM person WHERE first_name = 'John' | 0 |
-
-        Then you will get the following:
-        | Row Count Is Equal To X | SELECT id FROM person | 1 | # FAIL |
-        | Row Count Is Equal To X | SELECT id FROM person WHERE first_name = 'John' | 0 | # PASS |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Row Count Is Equal To X | SELECT id FROM person WHERE first_name = 'John' | 0 | True |
-        """
-        logger.info('Executing : Row Count Is Equal To X  |  %s  |  %s ' % (selectStatement, numRows))
-        num_rows = self.row_count(selectStatement, sansTran)
-        if num_rows != int(numRows.encode('ascii')):
-            raise AssertionError("Expected same number of rows to be returned from '%s' "
-                                 "than the returned rows of %s" % (selectStatement, num_rows))
-
-    def row_count_is_greater_than_x(self, selectStatement, numRows, sansTran=False):
-        """
-        Check if the number of rows returned from `selectStatement` is greater than the value submitted. If not, then
-        this will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
-        transaction commit or rollback.
-
-        For example, given we have a table `person` with the following data:
-        | id | first_name  | last_name |
-        |  1 | Franz Allan | See       |
-        |  2 | Jerry       | Schneider |
-
-        When you have the following assertions in your robot
-        | Row Count Is Greater Than X | SELECT id FROM person | 1 |
-        | Row Count Is Greater Than X | SELECT id FROM person WHERE first_name = 'John' | 0 |
-
-        Then you will get the following:
-        | Row Count Is Greater Than X | SELECT id FROM person | 1 | # PASS |
-        | Row Count Is Greater Than X | SELECT id FROM person WHERE first_name = 'John' | 0 | # FAIL |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Row Count Is Greater Than X | SELECT id FROM person | 1 | True |
-        """
-        logger.info('Executing : Row Count Is Greater Than X  |  %s  |  %s ' % (selectStatement, numRows))
-        num_rows = self.row_count(selectStatement, sansTran)
-        if num_rows <= int(numRows.encode('ascii')):
-            raise AssertionError("Expected more rows to be returned from '%s' "
-                                 "than the returned rows of %s" % (selectStatement, num_rows))
-
-    def row_count_is_less_than_x(self, selectStatement, numRows, sansTran=False):
-        """
-        Check if the number of rows returned from `selectStatement` is less than the value submitted. If not, then this
-        will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
-        transaction commit or rollback.
-
-        For example, given we have a table `person` with the following data:
-        | id | first_name  | last_name |
-        |  1 | Franz Allan | See       |
-        |  2 | Jerry       | Schneider |
-
-        When you have the following assertions in your robot
-        | Row Count Is Less Than X | SELECT id FROM person | 3 |
-        | Row Count Is Less Than X | SELECT id FROM person WHERE first_name = 'John' | 1 |
-
-        Then you will get the following:
-        | Row Count Is Less Than X | SELECT id FROM person | 3 | # PASS |
-        | Row Count Is Less Than X | SELECT id FROM person WHERE first_name = 'John' | 1 | # FAIL |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Row Count Is Less Than X | SELECT id FROM person | 3 | True |
-        """
-        logger.info('Executing : Row Count Is Less Than X  |  %s  |  %s ' % (selectStatement, numRows))
-        num_rows = self.row_count(selectStatement, sansTran)
-        if num_rows >= int(numRows.encode('ascii')):
-            raise AssertionError("Expected less rows to be returned from '%s' "
-                                 "than the returned rows of %s" % (selectStatement, num_rows))
-
-    def table_must_exist(self, tableName, sansTran=False):
-        """
-        Check if the table given exists in the database. Set optional input `sansTran` to True to run command without an
-        explicit transaction commit or rollback.
-
-        For example, given we have a table `person` in a database
-
-        When you do the following:
-        | Table Must Exist | person |
-
-        Then you will get the following:
-        | Table Must Exist | person | # PASS |
-        | Table Must Exist | first_name | # FAIL |
-
-        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
-        | Table Must Exist | person | True |
-        """
-        logger.info('Executing : Table Must Exist  |  %s ' % tableName)
-        if self.db_api_module_name in ["cx_Oracle"]:
-            selectStatement = ("SELECT * FROM all_objects WHERE object_type IN ('TABLE','VIEW') AND owner = SYS_CONTEXT('USERENV', 'SESSION_USER') AND object_name = UPPER('%s')" % tableName)
-        elif self.db_api_module_name in ["sqlite3"]:
-            selectStatement = ("SELECT name FROM sqlite_master WHERE type='table' AND name='%s' COLLATE NOCASE" % tableName)
-        elif self.db_api_module_name in ["ibm_db", "ibm_db_dbi"]:
-            selectStatement = ("SELECT name FROM SYSIBM.SYSTABLES WHERE type='T' AND name=UPPER('%s')" % tableName)
-        else:
-            selectStatement = ("SELECT * FROM information_schema.tables WHERE table_name='%s'" % tableName)
-        num_rows = self.row_count(selectStatement, sansTran)
-        if num_rows == 0:
-            raise AssertionError("Table '%s' does not exist in the db" % tableName)
+#  Copyright (c) 2010 Franz Allan Valencia See
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+from robot.api import logger
+
+
+class Assertion(object):
+    """
+    Assertion handles all the assertions of Database Library.
+    """
+
+    def check_if_exists_in_database(self, selectStatement, sansTran=False, msg=None):
+        """
+        Check if any row would be returned by given the input `selectStatement`. If there are no results, then this will
+        throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit transaction
+        commit or rollback. The default error message can be overridden with the `msg` argument.
+
+        For example, given we have a table `person` with the following data:
+        | id | first_name  | last_name |
+        |  1 | Franz Allan | See       |
+
+        When you have the following assertions in your robot
+        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' |
+        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' |
+
+        Then you will get the following:
+        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' | # PASS |
+        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' | # FAIL |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' | True |
+
+        Using optional `msg` to override the default error message:
+        | Check If Exists In Database | SELECT id FROM person WHERE first_name = 'John' | msg=my error message |
+        """
+        logger.info (f"Executing : Check If Exists In Database  |  {selectStatement}")
+        if not self.query(selectStatement, sansTran):
+            raise AssertionError(msg or f"Expected to have have at least one row, "
+                                 f"but got 0 rows from: '{selectStatement}'")
+
+    def check_if_not_exists_in_database(self, selectStatement, sansTran=False, msg=None):
+        """
+        This is the negation of `check_if_exists_in_database`.
+
+        Check if no rows would be returned by given the input `selectStatement`. If there are any results, then this
+        will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
+        transaction commit or rollback. The default error message can be overridden with the `msg` argument.
+
+        For example, given we have a table `person` with the following data:
+        | id | first_name  | last_name |
+        |  1 | Franz Allan | See       |
+
+        When you have the following assertions in your robot
+        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'John' |
+        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' |
+
+        Then you will get the following:
+        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'John' | # PASS |
+        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' | # FAIL |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'John' | True |
+
+        Using optional `msg` to override the default error message:
+        | Check If Not Exists In Database | SELECT id FROM person WHERE first_name = 'Franz Allan' | msg=my error message |
+        """
+        logger.info(f"Executing : Check If Not Exists In Database  |  {selectStatement}")
+        queryResults = self.query(selectStatement, sansTran)
+        if queryResults:
+            raise AssertionError(msg or f"Expected to have have no rows from '{selectStatement}', "
+                                        f"but got some rows: {queryResults}")
+
+    def row_count_is_0(self, selectStatement, sansTran=False, msg=None):
+        """
+        Check if any rows are returned from the submitted `selectStatement`. If there are, then this will throw an
+        AssertionError. Set optional input `sansTran` to True to run command without an explicit transaction commit or
+        rollback. The default error message can be overridden with the `msg` argument.
+
+        For example, given we have a table `person` with the following data:
+        | id | first_name  | last_name |
+        |  1 | Franz Allan | See       |
+
+        When you have the following assertions in your robot
+        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'Franz Allan' |
+        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'John' |
+
+        Then you will get the following:
+        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'Franz Allan' | # FAIL |
+        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'John' | # PASS |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'John' | True |
+
+        Using optional `msg` to override the default error message:
+        | Row Count is 0 | SELECT id FROM person WHERE first_name = 'Franz Allan' | msg=my error message |
+        """
+        logger.info(f"Executing : Row Count Is 0  |  selectStatement")
+        num_rows = self.row_count(selectStatement, sansTran)
+        if num_rows > 0:
+            raise AssertionError(msg or f"Expected 0 rows, but {num_rows} were returned from: '{selectStatement}'")
+
+    def row_count_is_equal_to_x(self, selectStatement, numRows, sansTran=False, msg=None):
+        """
+        Check if the number of rows returned from `selectStatement` is equal to the value submitted. If not, then this
+        will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
+        transaction commit or rollback. The default error message can be overridden with the `msg` argument.
+
+        For example, given we have a table `person` with the following data:
+        | id | first_name  | last_name |
+        |  1 | Franz Allan | See       |
+        |  2 | Jerry       | Schneider |
+
+        When you have the following assertions in your robot
+        | Row Count Is Equal To X | SELECT id FROM person | 1 |
+        | Row Count Is Equal To X | SELECT id FROM person WHERE first_name = 'John' | 0 |
+
+        Then you will get the following:
+        | Row Count Is Equal To X | SELECT id FROM person | 1 | # FAIL |
+        | Row Count Is Equal To X | SELECT id FROM person WHERE first_name = 'John' | 0 | # PASS |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Row Count Is Equal To X | SELECT id FROM person WHERE first_name = 'John' | 0 | True |
+
+        Using optional `msg` to override the default error message:
+        | Row Count Is Equal To X | SELECT id FROM person | 1 | msg=my error message |
+        """
+        logger.info(f"Executing : Row Count Is Equal To X  |  {selectStatement}  |  {numRows}")
+        num_rows = self.row_count(selectStatement, sansTran)
+        if num_rows != int(numRows.encode('ascii')):
+            raise AssertionError(msg or f"Expected {numRows} rows, "
+                                 f"but {num_rows} were returned from: '{selectStatement}'")
+
+    def row_count_is_greater_than_x(self, selectStatement, numRows, sansTran=False, msg=None):
+        """
+        Check if the number of rows returned from `selectStatement` is greater than the value submitted. If not, then
+        this will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
+        transaction commit or rollback. The default error message can be overridden with the `msg` argument.
+
+        For example, given we have a table `person` with the following data:
+        | id | first_name  | last_name |
+        |  1 | Franz Allan | See       |
+        |  2 | Jerry       | Schneider |
+
+        When you have the following assertions in your robot
+        | Row Count Is Greater Than X | SELECT id FROM person | 1 |
+        | Row Count Is Greater Than X | SELECT id FROM person WHERE first_name = 'John' | 0 |
+
+        Then you will get the following:
+        | Row Count Is Greater Than X | SELECT id FROM person | 1 | # PASS |
+        | Row Count Is Greater Than X | SELECT id FROM person WHERE first_name = 'John' | 0 | # FAIL |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Row Count Is Greater Than X | SELECT id FROM person | 1 | True |
+
+        Using optional `msg` to override the default error message:
+        | Row Count Is Greater Than X | SELECT id FROM person WHERE first_name = 'John' | 0 | msg=my error message |
+        """
+        logger.info(f"Executing : Row Count Is Greater Than X  |  {selectStatement}  |  {numRows}")
+        num_rows = self.row_count(selectStatement, sansTran)
+        if num_rows <= int(numRows.encode('ascii')):
+            raise AssertionError(msg or f"Expected more than {numRows} rows, "
+                                 f"but {num_rows} were returned from '{selectStatement}'")
+
+    def row_count_is_less_than_x(self, selectStatement, numRows, sansTran=False, msg=None):
+        """
+        Check if the number of rows returned from `selectStatement` is less than the value submitted. If not, then this
+        will throw an AssertionError. Set optional input `sansTran` to True to run command without an explicit
+        transaction commit or rollback.
+
+        For example, given we have a table `person` with the following data:
+        | id | first_name  | last_name |
+        |  1 | Franz Allan | See       |
+        |  2 | Jerry       | Schneider |
+
+        When you have the following assertions in your robot
+        | Row Count Is Less Than X | SELECT id FROM person | 3 |
+        | Row Count Is Less Than X | SELECT id FROM person WHERE first_name = 'John' | 1 |
+
+        Then you will get the following:
+        | Row Count Is Less Than X | SELECT id FROM person | 3 | # PASS |
+        | Row Count Is Less Than X | SELECT id FROM person WHERE first_name = 'John' | 1 | # FAIL |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Row Count Is Less Than X | SELECT id FROM person | 3 | True |
+
+        Using optional `msg` to override the default error message:
+        | Row Count Is Less Than X | SELECT id FROM person WHERE first_name = 'John' | 1 | msg=my error message |
+        """
+        logger.info(f"Executing : Row Count Is Less Than X  |  {selectStatement}  |  {numRows}")
+        num_rows = self.row_count(selectStatement, sansTran)
+        if num_rows >= int(numRows.encode('ascii')):
+            raise AssertionError(msg or f"Expected less than {numRows} rows, "
+                                 f"but {num_rows} were returned from '{selectStatement}'")
+
+    def table_must_exist(self, tableName, sansTran=False, msg=None):
+        """
+        Check if the table given exists in the database. Set optional input `sansTran` to True to run command without an
+        explicit transaction commit or rollback. The default error message can be overridden with the `msg` argument.
+
+        For example, given we have a table `person` in a database
+
+        When you do the following:
+        | Table Must Exist | person |
+
+        Then you will get the following:
+        | Table Must Exist | person | # PASS |
+        | Table Must Exist | first_name | # FAIL |
+
+        Using optional `sansTran` to run command without an explicit transaction commit or rollback:
+        | Table Must Exist | person | True |
+
+        Using optional `msg` to override the default error message:
+        | Table Must Exist | first_name | msg=my error message |
+        """
+        logger.info('Executing : Table Must Exist  |  %s ' % tableName)
+        if self.db_api_module_name in ["cx_Oracle", "oracledb"]:
+            selectStatement = ("SELECT * FROM all_objects WHERE object_type IN ('TABLE','VIEW') AND owner = SYS_CONTEXT('USERENV', 'SESSION_USER') AND object_name = UPPER('%s')" % tableName)
+            table_exists = self.row_count(selectStatement, sansTran) > 0
+        elif self.db_api_module_name in ["sqlite3"]:
+            selectStatement = ("SELECT name FROM sqlite_master WHERE type='table' AND name='%s' COLLATE NOCASE" % tableName)
+            table_exists = self.row_count(selectStatement, sansTran) > 0
+        elif self.db_api_module_name in ["ibm_db", "ibm_db_dbi"]:
+            selectStatement = ("SELECT name FROM SYSIBM.SYSTABLES WHERE type='T' AND name=UPPER('%s')" % tableName)
+            table_exists = self.row_count(selectStatement, sansTran) > 0
+        elif self.db_api_module_name in ["teradata"]:
+            selectStatement = ("SELECT TableName FROM DBC.TablesV WHERE TableKind='T' AND TableName='%s'" % tableName)
+            table_exists = self.row_count(selectStatement, sansTran) > 0
+        else:
+            try:
+                selectStatement = (f"SELECT * FROM information_schema.tables WHERE table_name='{tableName}'")
+                table_exists = self.row_count(selectStatement, sansTran) > 0
+            except:
+                logger.info("Database doesn't support information schema, try using a simple SQL request")
+                try:
+                    selectStatement = (f"SELECT 1 from {tableName} where 1=0")
+                    num_rows = self.row_count(selectStatement, sansTran)
+                    table_exists = True
+                except:
+                    table_exists = False
+        assert table_exists, msg or f"Table '{tableName}' does not exist in the db"
+
```

### Comparing `robotframework-databaselibrary-1.2.4/src/DatabaseLibrary/__init__.py` & `robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,76 @@
-#  Copyright (c) 2010 Franz Allan Valencia See
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import os
-
-from DatabaseLibrary.connection_manager import ConnectionManager
-from DatabaseLibrary.query import Query
-from DatabaseLibrary.assertion import Assertion
-from DatabaseLibrary.version import VERSION
-
-_version_ = VERSION
-
-class DatabaseLibrary(ConnectionManager, Query, Assertion):
-    """
-    Database Library contains utilities meant for Robot Framework's usage.
-
-    This can allow you to query your database after an action has been made to verify the results.
-
-    This is `compatible*` with any Database API Specification 2.0 module.
-
-
-
-    References:
-
-     + Database API Specification 2.0 - http://www.python.org/dev/peps/pep-0249/
-
-     + Lists of DB API 2.0 - http://wiki.python.org/moin/DatabaseInterfaces
-
-     + Python Database Programming - http://wiki.python.org/moin/DatabaseProgramming/
-
-    Notes:
-
-
-
-    `compatible* - or at least theoretically it should be compatible. Currently tested only with postgresql
-    (using psycopg2).`
-
-    Example Usage:
-    | # Setup |
-    | Connect to Database |
-    | # Guard assertion (verify that test started in expected state). |
-    | Check if not exists in database | select id from person where first_name = 'Franz Allan' and last_name = 'See' |
-    | # Drive UI to do some action |
-    | Go To | http://localhost/person/form.html | | # From selenium library |
-    | Input Text |  name=first_name | Franz Allan | # From selenium library |
-    | Input Text |  name=last_name | See | # From selenium library |
-    | Click Button | Save | | # From selenium library |
-    | # Log results |
-    | @{queryResults} | Query | select * from person |
-    | Log Many | @{queryResults} |
-    | # Verify if persisted in the database |
-    | Check if exists in database | select id from person where first_name = 'Franz Allan' and last_name = 'See' |
-    | # Teardown |
-    | Disconnect from Database |
-    """
-
-    ROBOT_LIBRARY_SCOPE = 'GLOBAL'
+#  Copyright (c) 2010 Franz Allan Valencia See
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import os
+
+from DatabaseLibrary.connection_manager import ConnectionManager
+from DatabaseLibrary.query import Query
+from DatabaseLibrary.assertion import Assertion
+from DatabaseLibrary.version import VERSION
+
+__version__ = VERSION
+
+class DatabaseLibrary(ConnectionManager, Query, Assertion):
+    """
+    The Database Library for [https://robotframework.org|Robot Framework] allows you to query a database and verify the results.
+    It requires an appropriate *Python module to be installed separately* - depending on your database, like e.g. `oracledb` or `pymysql`. 
+
+    == Requirements ==
+    - Python
+    - Robot Framework
+    - Python database module you're going to use - e.g. `oracledb`
+
+    == Installation ==
+    | pip install robotframework-databaselibrary
+    Don't forget to install the required Python database module!
+
+    == Usage example ==
+    
+    | *** Settings ***
+    | Library       DatabaseLibrary
+    | Test Setup    Connect To My Oracle DB
+    | 
+    | *** Keywords ***
+    | Connect To My Oracle DB
+    |     Connect To Database
+    |     ...    oracledb
+    |     ...    dbName=db
+    |     ...    dbUsername=my_user
+    |     ...    dbPassword=my_pass
+    |     ...    dbHost=127.0.0.1
+    |     ...    dbPort=1521
+    | 
+    | *** Test Cases ***
+    | Person Table Contains Expected Records
+    |     ${output}=    Query    select LAST_NAME from person
+    |     Length Should Be    ${output}    2
+    |     Should Be Equal    ${output}[0][0]    See
+    |     Should Be Equal    ${output}[1][0]    Schneider
+    | 
+    | Person Table Contains No Joe
+    |     ${sql}=    Catenate    SELECT id FROM person
+    |     ...                    WHERE FIRST_NAME= 'Joe'    
+    |     Check If Not Exists In Database    ${sql}
+    | 
+
+    == Database modules compatibility ==
+    The library is basically compatible with any [https://peps.python.org/pep-0249|Python Database API Specification 2.0] module.
+
+    However, the actual implementation in existing Python modules is sometimes quite different, which requires custom handling in the library.
+    Therefore there are some modules, which are "natively" supported in the library - and others, which may work and may not.
+
+    See more on the [https://github.com/MarketSquare/Robotframework-Database-Library|project page on GitHub].
+    """
+
+    ROBOT_LIBRARY_SCOPE = 'GLOBAL'
```

