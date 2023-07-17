# Comparing `tmp/sqlitebiter-0.8.1.tar.gz` & `tmp/sqlitebiter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlitebiter-0.8.1.tar", last modified: Fri May  5 11:42:56 2017, max compression
+gzip compressed data, was "dist/sqlitebiter-0.9.0.tar", last modified: Sun May 28 15:02:17 2017, max compression
```

## Comparing `sqlitebiter-0.8.1.tar` & `sqlitebiter-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/docs/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/docs/pages/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/docs/pages/introduction/
--rw-r--r--   0 travis    (1000) travis    (1000)      108 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/requirements/
--rw-r--r--   0 travis    (1000) travis    (1000)       51 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/requirements/docs_requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      122 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/requirements/requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       22 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/requirements/test_requirements.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter/
--rw-r--r--   0 travis    (1000) travis    (1000)      154 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      825 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/_config.py
--rw-r--r--   0 travis    (1000) travis    (1000)      216 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/_const.py
--rw-r--r--   0 travis    (1000) travis    (1000)      941 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/_counter.py
--rw-r--r--   0 travis    (1000) travis    (1000)      391 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/_enum.py
--rw-r--r--   0 travis    (1000) travis    (1000)      142 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/_version.py
--rw-r--r--   0 travis    (1000) travis    (1000)    12838 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/sqlitebiter/sqlitebiter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)    11359 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      689 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       61 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      122 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       12 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/sqlitebiter.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/test/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/test/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7580 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/test/dataset.py
--rw-r--r--   0 travis    (1000) travis    (1000)      737 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/test/test_counter.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9806 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/test/test_file_subcommand.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3357 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/test/test_file_subcommand_sqlite.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1084 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/LICENSE
--rw-r--r--   0 travis    (1000) travis    (1000)      223 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     8914 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     2260 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      109 2017-05-05 11:42:16.000000 sqlitebiter-0.8.1/tox.ini
--rw-r--r--   0 travis    (1000) travis    (1000)    11359 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      107 2017-05-05 11:42:56.000000 sqlitebiter-0.8.1/setup.cfg
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/docs/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/docs/pages/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/docs/pages/introduction/
+-rw-r--r--   0 travis    (1000) travis    (1000)      108 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/docs/pages/introduction/summary.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/requirements/
+-rw-r--r--   0 travis    (1000) travis    (1000)       51 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/requirements/docs_requirements.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      124 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/requirements/requirements.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       22 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/requirements/test_requirements.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/sqlitebiter/
+-rw-r--r--   0 travis    (1000) travis    (1000)      154 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      825 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/_config.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      216 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/_const.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      941 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/_counter.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      391 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/_enum.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      142 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/_version.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    15159 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/sqlitebiter/sqlitebiter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)    11359 2017-05-28 15:02:16.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      704 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-28 15:02:16.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       61 2017-05-28 15:02:16.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      124 2017-05-28 15:02:16.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       12 2017-05-28 15:02:16.000000 sqlitebiter-0.9.0/sqlitebiter.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/test/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/test/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      438 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/test/common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9106 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/test/dataset.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      737 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/test/test_counter.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    16166 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/test/test_file_subcommand.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3474 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/test/test_file_subcommand_sqlite.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1084 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/LICENSE
+-rw-r--r--   0 travis    (1000) travis    (1000)      223 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)     8914 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)     2260 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      109 2017-05-28 15:01:22.000000 sqlitebiter-0.9.0/tox.ini
+-rw-r--r--   0 travis    (1000) travis    (1000)    11359 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      107 2017-05-28 15:02:17.000000 sqlitebiter-0.9.0/setup.cfg
```

### Comparing `sqlitebiter-0.8.1/sqlitebiter/_config.py` & `sqlitebiter-0.9.0/sqlitebiter/_config.py`

 * *Files identical despite different names*

### Comparing `sqlitebiter-0.8.1/sqlitebiter/_counter.py` & `sqlitebiter-0.9.0/sqlitebiter/_counter.py`

 * *Files identical despite different names*

### Comparing `sqlitebiter-0.8.1/sqlitebiter/sqlitebiter.py` & `sqlitebiter-0.9.0/sqlitebiter/sqlitebiter.py`

 * *Files 13% similar despite different names*

```diff
@@ -146,14 +146,74 @@
 def cmd(ctx, is_append_table, verbosity_level, log_level):
     ctx.obj[Context.IS_APPEND_TABLE] = is_append_table
     ctx.obj[Context.VERBOSITY_LEVEL] = verbosity_level
     ctx.obj[Context.LOG_LEVEL] = (
         logbook.INFO if log_level is None else log_level)
 
 
+class TableCreator(object):
+
+    def __init__(self, dst_con, tabledata):
+        self.__dst_con = dst_con
+        self.__tabledata = tabledata
+
+    def create(self):
+        is_rename, con_mem = self.__require_rename_table()
+        src_table_name = con_mem.get_table_name_list()[0]
+        dst_table_name = src_table_name
+
+        if is_rename:
+            dst_table_name = self.__make_unique_table_name(src_table_name)
+
+            simplesqlite.copy_table(
+                src_con=con_mem, dst_con=self.__dst_con,
+                src_table_name=src_table_name,
+                dst_table_name=dst_table_name)
+        else:
+            simplesqlite.append_table(
+                src_con=con_mem, dst_con=self.__dst_con,
+                table_name=dst_table_name)
+
+    def __require_rename_table(self):
+        con_mem = simplesqlite.connect_sqlite_db_mem()
+        con_mem.create_table_from_tabledata(tabledata=self.__tabledata)
+
+        if not self.__dst_con.has_table(self.__tabledata.table_name):
+            return (False, con_mem)
+
+        if self.__dst_con.get_attr_name_list(self.__tabledata.table_name) != self.__tabledata.header_list:
+            return (True, con_mem)
+
+        con_schema_extractor = SqliteSchemaExtractor(
+            self.__dst_con, verbosity_level=1)
+        con_mem_schema_extractor = SqliteSchemaExtractor(
+            con_mem, verbosity_level=1)
+
+        if con_schema_extractor.get_database_schema() == con_mem_schema_extractor.get_database_schema():
+            return (False, con_mem)
+
+        return (True, con_mem)
+
+    def __make_unique_table_name(self, table_name_base):
+        exist_table_name_list = self.__dst_con.get_table_name_list()
+
+        if table_name_base not in exist_table_name_list:
+            return table_name_base
+
+        suffix_id = 1
+        while True:
+            table_name_candidate = u"{:s}_{:d}".format(
+                table_name_base, suffix_id)
+
+            if table_name_candidate not in exist_table_name_list:
+                return table_name_candidate
+
+            suffix_id += 1
+
+
 @cmd.command()
 @click.argument("files", type=str, nargs=-1)
 @click.option(
     "-o", "--output-path", metavar="PATH", default=Default.OUTPUT_FILE,
     help="Output path of the SQLite database file. Defaults to '{:s}'.".format(
         Default.OUTPUT_FILE))
 @click.pass_context
@@ -164,29 +224,30 @@
     """
 
     if typepy.is_empty_sequence(files):
         sys.exit(ExitCode.NO_INPUT)
 
     con = create_database(ctx, output_path)
     verbosity_level = ctx.obj.get(Context.VERBOSITY_LEVEL)
-    extractor = get_schema_extractor(con, verbosity_level)
+    schema_extractor = get_schema_extractor(con, verbosity_level)
     result_counter = ResultCounter()
     logger = make_logger("{:s} file".format(
         PROGRAM_NAME), ctx.obj[Context.LOG_LEVEL])
 
     for file_path in files:
         file_path = path.Path(file_path)
+
         if not file_path.isfile():
             logger.error(u"file not found: {}".format(file_path))
             result_counter.inc_fail()
             continue
 
         if file_path == output_path:
             logger.warn(
-                u"skip a file which same path as the output file ({})".format(
+                u"skip a file which has the same path as the output file ({})".format(
                     file_path))
             continue
 
         logger.debug(u"converting '{}'".format(file_path))
 
         try:
             loader = ptr.TableFileLoader(file_path)
@@ -202,25 +263,26 @@
 
         try:
             for tabledata in loader.load():
                 sqlite_tabledata = ptr.SQLiteTableDataSanitizer(
                     tabledata).sanitize()
 
                 try:
-                    con.create_table_from_tabledata(sqlite_tabledata)
+                    TableCreator(
+                        dst_con=con, tabledata=sqlite_tabledata).create()
                     result_counter.inc_success()
                 except (ValueError, IOError) as e:
                     logger.debug(
                         u"path={}, message={}".format(file_path, e))
                     result_counter.inc_fail()
                     continue
 
                 logger.info(get_success_message(
                     verbosity_level, file_path,
-                    extractor.get_table_schema_text(
+                    schema_extractor.get_table_schema_text(
                         sqlite_tabledata.table_name).strip()))
         except ptr.OpenError as e:
             logger.error(u"open error: file={}, message='{}'".format(
                 file_path, str(e)))
             result_counter.inc_fail()
         except ptr.ValidationError as e:
             logger.error(
@@ -261,15 +323,15 @@
     """
 
     if typepy.is_empty_sequence(url):
         sys.exit(ExitCode.NO_INPUT)
 
     con = create_database(ctx, output_path)
     verbosity_level = ctx.obj.get(Context.VERBOSITY_LEVEL)
-    extractor = get_schema_extractor(con, verbosity_level)
+    schema_extractor = get_schema_extractor(con, verbosity_level)
     result_counter = ResultCounter()
     logger = make_logger("{:s} url".format(
         PROGRAM_NAME), ctx.obj[Context.LOG_LEVEL])
 
     if typepy.is_null_string(proxy):
         proxy = app_config_manager.load().get(ConfigKey.PROXY_SERVER)
 
@@ -289,25 +351,26 @@
 
     try:
         for tabledata in loader.load():
             sqlite_tabledata = ptr.SQLiteTableDataSanitizer(
                 tabledata).sanitize()
 
             try:
-                con.create_table_from_tabledata(sqlite_tabledata)
+                TableCreator(
+                    dst_con=con, tabledata=sqlite_tabledata).create()
                 result_counter.inc_success()
             except (ValueError) as e:
                 logger.debug(
                     u"url={}, message={}".format(url, str(e)))
                 result_counter.inc_fail()
                 continue
 
             logger.info(get_success_message(
                 verbosity_level, url,
-                extractor.get_table_schema_text(
+                schema_extractor.get_table_schema_text(
                     sqlite_tabledata.table_name).strip()))
     except ptr.InvalidDataError as e:
         logger.error(u"invalid data: url={}, message={}".format(url, str(e)))
         result_counter.inc_fail()
 
     write_completion_message(logger, output_path, result_counter)
 
@@ -330,38 +393,42 @@
 
     CREDENTIALS: OAuth2 Google credentials file.
     TITLE: Title of the Google Sheets to convert.
     """
 
     con = create_database(ctx, output_path)
     verbosity_level = ctx.obj.get(Context.VERBOSITY_LEVEL)
-    extractor = get_schema_extractor(con, verbosity_level)
+    schema_extractor = get_schema_extractor(con, verbosity_level)
     result_counter = ResultCounter()
     logger = make_logger("{:s} gs".format(
         PROGRAM_NAME), ctx.obj[Context.LOG_LEVEL])
 
     loader = ptr.GoogleSheetsTableLoader()
     loader.source = credentials
     loader.title = title
 
     # if typepy.is_null_string(loader.source):
     #     loader.source = app_config_manager.load().get(
     #         ConfigKey.GS_CREDENTIALS_FILE_PATH)
 
     try:
         for tabledata in loader.load():
+            sqlite_tabledata = ptr.SQLiteTableDataSanitizer(
+                tabledata).sanitize()
+
             try:
-                con.create_table_from_tabledata(tabledata)
+                TableCreator(
+                    dst_con=con, tabledata=sqlite_tabledata).create()
                 result_counter.inc_success()
             except (ptr.ValidationError, ptr.InvalidDataError):
                 result_counter.inc_fail()
 
             logger.info(get_success_message(
                 verbosity_level, "google sheets",
-                extractor.get_table_schema_text(tabledata.table_name).strip()))
+                schema_extractor.get_table_schema_text(tabledata.table_name).strip()))
     except ptr.OpenError as e:
         logger.error(e)
         result_counter.inc_fail()
     except AttributeError:
         logger.error(u"invalid credentials data: path={}".format(credentials))
         result_counter.inc_fail()
     except (ptr.ValidationError, ptr.InvalidDataError) as e:
```

### Comparing `sqlitebiter-0.8.1/sqlitebiter.egg-info/PKG-INFO` & `sqlitebiter-0.9.0/sqlitebiter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sqlitebiter
-Version: 0.8.1
+Version: 0.9.0
 Summary: A CLI tool to convert CSV/Excel/HTML/JSON/LTSV/Markdown/SQLite/TSV/Google-Sheets to a SQLite database file.
 
 Home-page: https://github.com/thombashi/sqlitebiter
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: sqlitebiter
```

### Comparing `sqlitebiter-0.8.1/sqlitebiter.egg-info/SOURCES.txt` & `sqlitebiter-0.9.0/sqlitebiter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 sqlitebiter.egg-info/PKG-INFO
 sqlitebiter.egg-info/SOURCES.txt
 sqlitebiter.egg-info/dependency_links.txt
 sqlitebiter.egg-info/entry_points.txt
 sqlitebiter.egg-info/requires.txt
 sqlitebiter.egg-info/top_level.txt
 test/__init__.py
+test/common.py
 test/dataset.py
 test/test_counter.py
 test/test_file_subcommand.py
 test/test_file_subcommand_sqlite.py
```

### Comparing `sqlitebiter-0.8.1/test/dataset.py` & `sqlitebiter-0.9.0/test/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # encoding: utf-8
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
-from __future__ import unicode_literals
+from __future__ import absolute_import
 from __future__ import print_function
+from __future__ import unicode_literals
+
 import io
 
 import path
 import xlsxwriter
 
 
 def valid_json_single_file():
@@ -22,84 +24,144 @@
         ]""")
 
     return file_path
 
 
 def invalid_json_single_file():
     file_path = "invalid_json_a.json"
+
     with open(file_path, "w") as f:
         f.write("""[
             {"attr_b": 4, "attr_c": "a", "attr_a": [1]},
             {"attr_b": 2.1, "attr_c": "bb", "attr_a": [2]},
             {"attr_b": 120.9, "attr_c": "ccc", "attr_a": [3]}
         ]""")
 
     return file_path
 
 
-def valid_json_multi_file():
+def valid_json_multi_file_1():
     file_path = "multijson.json"
+
     with open(file_path, "w") as f:
         f.write("""{
-            "table1" : [
+            "multij1" : [
                 {"attr_b": 4, "attr_c": "a", "attr_a": 1},
                 {"attr_b": 2.1, "attr_c": "bb", "attr_a": 2},
                 {"attr_b": 120.9, "attr_c": "ccc", "attr_a": 3}
             ],
-            "table2" : [
+            "multij2" : [
                 {"a": 1, "b": 4},
                 {"a": 2 },
                 {"a": 3, "b": 120.9}
             ]
         }""")
 
     return file_path
 
 
+def valid_json_multi_file_2_1():
+    file_path = "multijson_2_1.json"
+
+    with open(file_path, "w") as f:
+        f.write("""{
+            "multij2" : [
+                {"attr_b": 4, "attr_c": "a", "attr_a": 1},
+                {"attr_b": 2.1, "attr_c": "bb", "attr_a": 2},
+                {"attr_b": 120.9, "attr_c": "ccc", "attr_a": 3}
+            ]
+        }""")
+
+    return file_path
+
+
+def valid_json_multi_file_2_2():
+    file_path = "multijson_2_2.json"
+
+    with open(file_path, "w") as f:
+        f.write("""{
+            "multij2" : [
+                {"attr_b": 4, "attr_c": "a", "attr_a": 1},
+                {"attr_b": 2.1, "attr_c": "bb", "attr_a": 2},
+                {"attr_b": 120.9, "attr_c": "ccc", "attr_a": 3}
+            ]
+        }""")
+
+    return file_path
+
+
+def valid_json_multi_file_2_3():
+    file_path = "multijson_2_3.json"
+
+    with open(file_path, "w") as f:
+        f.write("""{
+            "multij2" : [
+                {"attr_b": "a", "attr_c": 4, "attr_a": "abc"},
+                {"attr_b": "bb", "attr_c": 2.1, "attr_a": "abc"},
+                {"attr_b": "ccc", "attr_c": 120.9, "attr_a": "abc"}
+            ]
+        }""")
+
+    return file_path
+
+
 def invalid_json_multi_file():
     file_path = "invalid_multi.json"
+
     with open(file_path, "w") as f:
         f.write("""{
             "json_b" : "hoge",
             "json_c" : "bar"
         }""")
 
     return file_path
 
 
-def valid_csv_file_1():
+def valid_csv_file_1_1():
     file_path = "csv_a.csv"
     with open(file_path, "w") as f:
         f.write("\n".join([
             '"attr_a","attr_b","attr_c"',
             '1,4,"a"',
             '2,2.1,"bb"',
             '3,120.9,"ccc"',
         ]))
 
     return file_path
 
 
-def valid_csv_file_2():
-    # reserved keywod of SQLite
+def valid_csv_file_1_2():
+    file_path = "csv_a.csv"
+    with open(file_path, "w") as f:
+        f.write("\n".join([
+            '"attr_a","attr_b","attr_c"',
+            '4,1,"a"',
+            '2.1,2,2.1,"bb"',
+            '120.9,3,"ccc"',
+        ]))
 
+
+def valid_csv_file_2_1():
+    # filename that include a reserved keyword of SQLite
     file_path = "insert.csv"
+
     with open(file_path, "w") as f:
         f.write("\n".join([
             "index,No,Player_last_name,Age,Team",
             "1, 55,D Sam, 31,Raven",
             "2, 36,J Ifdgg, 30,Raven",
             "3, 91,K Wedfb, 28,Raven",
         ]))
 
     return file_path
 
 
 def invalid_csv_file():
     file_path = "invalid_csv.csv"
+
     with open(file_path, "w") as f:
         f.write("\n".join([
             '"attr_a"\t"attr_b"\t"attr_c"',
             '1\t4\t"tsv0"',
             '2\t2.1\t"tsv1"',
             '3\t120.9\t"tsv2"',
         ]))
@@ -118,14 +180,15 @@
         ]))
 
     return file_path
 
 
 def invalid_tsv_file():
     file_path = "invalid_tsv.tsv"
+
     with open(file_path, "w") as f:
         f.write("\n".join([
             '"attr_a","attr_b","attr_c"',
             '1,4,"a"',
             '2,2.1,"bb"',
             '3,120.9,"ccc"',
         ]))
@@ -207,14 +270,15 @@
     path.Path(file_path).touch()
 
     return file_path
 
 
 def valid_html_file():
     file_path = "htmltable.html"
+
     with open(file_path, "w") as f:
         f.write("""<title>testtitle</title>
 <table id="tablename">
     <caption>caption</caption>
     <tr>
       <th>a</th>
       <th>b</th>
@@ -257,14 +321,15 @@
 """)
 
     return file_path
 
 
 def invalid_html_file():
     file_path = "invalid_html.html"
+
     with open(file_path, "w") as f:
         f.write("""<html>
   <head>
     header
   </head>
   <body>
     hogehoge
@@ -273,59 +338,64 @@
 """)
 
     return file_path
 
 
 def valid_ltsv_file():
     file_path = "valid_ltsv_a.ltsv"
+
     with open(file_path, "w") as f:
         f.write("""a.0:1\tb-1:123.1\tc_2:"ltsv0"\t"dd":1.0\te.f-g_4:"1"
 a.0:2\tb-1:2.2\tc_2:"ltsv1"\t"dd":2.2\te.f-g_4:"2.2"
 a.0:3\tb-1:3.3\tc_2:"ltsv2"\t"dd":3.0\te.f-g_4:"cccc"
 """)
 
     return file_path
 
 
 def invalid_ltsv_file():
     file_path = "invalid_ltsv.ltsv"
+
     with open(file_path, "w") as f:
         f.write("\n".join([
             '"attr_a"\t"attr_b"\t"attr_c"',
             '1\t4\t"tsv0"',
             '2\t2.1\t"tsv1"',
             '3\t120.9\t"tsv2"',
         ]))
 
     return file_path
 
 
 def valid_markdown_file():
     file_path = "valid_mdtable.md"
+
     with open(file_path, "w") as f:
         f.write(""" a |  b  | c 
 --:|----:|---
   1|123.1|a  
   2|  2.2|bb 
   3|  3.3|ccc
 """)
 
     return file_path
 
 
 def valid_multibyte_char_file():
     file_path = "valid_multibyte_char.csv"
+
     with io.open(file_path, "w", encoding="utf-8") as f:
         f.write(""""姓","名","生年月日","郵便番号","住所","電話番号"
 "山田","太郎","2001/1/1","100-0002","東京都千代田区皇居外苑","03-1234-5678"
 "山田","次郎","2001/1/2","251-0036","神奈川県藤沢市江の島１丁目","03-9999-9999"
 """)
 
     return file_path
 
 
 def not_supported_format_file():
     file_path = "invalid_format.txt"
+
     with open(file_path, "w") as f:
         f.write("invalid format")
 
     return file_path
```

### Comparing `sqlitebiter-0.8.1/test/test_counter.py` & `sqlitebiter-0.9.0/test/test_counter.py`

 * *Files identical despite different names*

### Comparing `sqlitebiter-0.8.1/test/test_file_subcommand_sqlite.py` & `sqlitebiter-0.9.0/test/test_file_subcommand_sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     SqliteFileLoader,
 )
 import pytest
 from simplesqlite import SimpleSQLite
 from sqlitebiter._enum import ExitCode
 from sqlitebiter.sqlitebiter import cmd
 
+from .common import print_traceback
+
 
 TEST_TABLE_NAME_A = "test_table_a"
 TEST_TABLE_NAME_B = "test_table_b"
 
 
 @pytest.fixture
 def con_a0():
@@ -60,27 +62,28 @@
             [101, 102],
             [103, 104],
         ])
 
     return con
 
 
-class Test_sqlitebiter_file_sqlite_merge:
+class Test_sqlitebiter_file_sqlite_merge(object):
 
     def test_normal_same_table(self, con_a0, con_a1):
         out_db_path = "test.sqlite"
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             result = runner.invoke(
                 cmd,
                 [
                     "file", con_a0.database_path, con_a1.database_path,
                     "-o", out_db_path,
                 ])
+            print_traceback(result)
             assert result.exit_code == ExitCode.SUCCESS
 
             expected = TableData(
                 table_name=TEST_TABLE_NAME_A,
                 header_list=["attra", "attrb"],
                 record_list=[
                     [1, 2],
@@ -98,14 +101,15 @@
         with runner.isolated_filesystem():
             result = runner.invoke(
                 cmd,
                 [
                     "file", con_a0.database_path, con_b0.database_path,
                     "-o", out_db_path,
                 ])
+            print_traceback(result)
             assert result.exit_code == ExitCode.SUCCESS
 
             expected_list = [
                 TableData(
                     table_name=TEST_TABLE_NAME_A,
                     header_list=["attra", "attrb"],
                     record_list=[
```

### Comparing `sqlitebiter-0.8.1/LICENSE` & `sqlitebiter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlitebiter-0.8.1/README.rst` & `sqlitebiter-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlitebiter-0.8.1/setup.py` & `sqlitebiter-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `sqlitebiter-0.8.1/PKG-INFO` & `sqlitebiter-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sqlitebiter
-Version: 0.8.1
+Version: 0.9.0
 Summary: A CLI tool to convert CSV/Excel/HTML/JSON/LTSV/Markdown/SQLite/TSV/Google-Sheets to a SQLite database file.
 
 Home-page: https://github.com/thombashi/sqlitebiter
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: sqlitebiter
```

