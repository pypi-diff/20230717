# Comparing `tmp/ooo_dev_odh-0.1.0.tar.gz` & `tmp/ooo_dev_odh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooo_dev_odh-0.1.0.tar", max compression
+gzip compressed data, was "ooo_dev_odh-0.1.1.tar", max compression
```

## Comparing `ooo_dev_odh-0.1.0.tar` & `ooo_dev_odh-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1081 2023-07-17 17:16:34.449530 ooo_dev_odh-0.1.0/LICENSE
--rw-r--r--   0        0        0     1134 2023-07-17 17:16:34.445530 ooo_dev_odh-0.1.0/README.md
--rw-r--r--   0        0        0     1134 2023-07-17 16:43:35.141965 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/README.md
--rw-r--r--   0        0        0        0 2023-07-17 15:44:39.085366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/__init__.py
--rw-r--r--   0        0        0      177 2023-07-17 15:44:39.085366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cfg/__init__.py
--rw-r--r--   0        0        0      328 2023-07-17 16:40:28.764878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cfg/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2786 2023-07-17 16:40:28.776878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cfg/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     2269 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cfg/config.py
--rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cli/__init__.py
--rw-r--r--   0        0        0     6729 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cli/hlp.py
--rw-r--r--   0        0        0      985 2023-07-17 17:16:34.449530 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cli/interactive_hlp.py
--rw-r--r--   0        0        0      787 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/config.json
--rw-r--r--   0        0        0      135 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/__init__.py
--rw-r--r--   0        0        0      276 2023-07-17 16:40:28.860879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      745 2023-07-17 16:40:28.868879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/__pycache__/inventory.cpython-310.pyc
--rw-r--r--   0        0        0      465 2023-07-17 16:40:28.876879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/__pycache__/sphinx_info.cpython-310.pyc
--rw-r--r--   0        0        0      382 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/inventory.py
--rw-r--r--   0        0        0      124 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/sphinx_info.py
--rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/__init__.py
--rw-r--r--   0        0        0      159 2023-07-17 16:40:28.804878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/controller/__init__.py
--rw-r--r--   0        0        0      170 2023-07-17 16:40:28.812878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/controller/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1492 2023-07-17 16:40:28.816878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/controller/__pycache__/database_controller.cpython-310.pyc
--rw-r--r--   0        0        0     1027 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/controller/database_controller.py
--rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__init__.py
--rw-r--r--   0        0        0      168 2023-07-17 16:40:28.820878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1243 2023-07-17 16:40:28.856879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql.cpython-310.pyc
--rw-r--r--   0        0        0     2342 2023-07-17 16:40:28.852879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql_table.cpython-310.pyc
--rw-r--r--   0        0        0      944 2023-07-17 16:40:28.840879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/db_connect.cpython-310.pyc
--rw-r--r--   0        0        0     3262 2023-07-17 16:40:28.828878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/init_db.cpython-310.pyc
--rw-r--r--   0        0        0      957 2023-07-17 16:40:28.832878 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/sql_ctx.cpython-310.pyc
--rw-r--r--   0        0        0     3241 2023-07-17 16:40:29.284881 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_inventory.cpython-310.pyc
--rw-r--r--   0        0        0     3174 2023-07-17 16:40:28.844879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_sphinx_info.cpython-310.pyc
--rw-r--r--   0        0        0      560 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/base_sql.py
--rw-r--r--   0        0        0     1467 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/base_sql_table.py
--rw-r--r--   0        0        0      467 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/db_connect.py
--rw-r--r--   0        0        0     3065 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/init_db.py
--rw-r--r--   0        0        0      724 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/sql_ctx.py
--rw-r--r--   0        0        0     2477 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/tbl_inventory.py
--rw-r--r--   0        0        0     2672 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/tbl_sphinx_info.py
--rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/qry/__init__.py
--rw-r--r--   0        0        0      163 2023-07-17 16:40:28.884879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/qry/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5706 2023-07-17 16:40:28.888879 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/qry/__pycache__/qry_inv.cpython-310.pyc
--rw-r--r--   0        0        0     5798 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/qry/qry_inv.py
--rw-r--r--   0        0        0  9482240 2023-07-17 16:43:35.181965 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/res/db.sqlite3
--rw-r--r--   0        0        0       67 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/web_search/__init__.py
--rwxr-xr-x   0        0        0      208 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/web_search/browse.py
--rw-r--r--   0        0        0     1716 2023-07-17 17:16:34.449530 ooo_dev_odh-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ooo_dev_odh-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-17 18:50:42.577714 ooo_dev_odh-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1134 2023-07-17 18:50:42.573714 ooo_dev_odh-0.1.1/README.md
+-rw-r--r--   0        0        0     1134 2023-07-17 17:36:26.108947 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 15:44:39.085366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-17 15:44:39.085366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cfg/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-17 16:40:28.764878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cfg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2786 2023-07-17 16:40:28.776878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cfg/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     2269 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cfg/config.py
+-rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cli/__init__.py
+-rw-r--r--   0        0        0     6729 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cli/hlp.py
+-rw-r--r--   0        0        0      923 2023-07-17 18:50:42.585714 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cli/interactive_hlp.py
+-rw-r--r--   0        0        0      787 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/config.json
+-rw-r--r--   0        0        0      135 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-17 16:40:28.860879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      745 2023-07-17 16:40:28.868879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/__pycache__/inventory.cpython-310.pyc
+-rw-r--r--   0        0        0      465 2023-07-17 16:40:28.876879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/__pycache__/sphinx_info.cpython-310.pyc
+-rw-r--r--   0        0        0      382 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/inventory.py
+-rw-r--r--   0        0        0      124 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/sphinx_info.py
+-rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-17 16:40:28.804878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/controller/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-17 16:40:28.812878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/controller/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1492 2023-07-17 16:40:28.816878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/controller/__pycache__/database_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     1027 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/controller/database_controller.py
+-rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-17 16:40:28.820878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1243 2023-07-17 16:40:28.856879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql.cpython-310.pyc
+-rw-r--r--   0        0        0     2342 2023-07-17 16:40:28.852879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql_table.cpython-310.pyc
+-rw-r--r--   0        0        0      944 2023-07-17 16:40:28.840879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/db_connect.cpython-310.pyc
+-rw-r--r--   0        0        0     3262 2023-07-17 16:40:28.828878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/init_db.cpython-310.pyc
+-rw-r--r--   0        0        0      957 2023-07-17 16:40:28.832878 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/sql_ctx.cpython-310.pyc
+-rw-r--r--   0        0        0     3241 2023-07-17 16:40:29.284881 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_inventory.cpython-310.pyc
+-rw-r--r--   0        0        0     3174 2023-07-17 16:40:28.844879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_sphinx_info.cpython-310.pyc
+-rw-r--r--   0        0        0      560 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/base_sql.py
+-rw-r--r--   0        0        0     1467 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/base_sql_table.py
+-rw-r--r--   0        0        0      467 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/db_connect.py
+-rw-r--r--   0        0        0     3065 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/init_db.py
+-rw-r--r--   0        0        0      724 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/sql_ctx.py
+-rw-r--r--   0        0        0     2477 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/tbl_inventory.py
+-rw-r--r--   0        0        0     2672 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/tbl_sphinx_info.py
+-rw-r--r--   0        0        0        0 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/qry/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-17 16:40:28.884879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/qry/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5706 2023-07-17 16:40:28.888879 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/qry/__pycache__/qry_inv.cpython-310.pyc
+-rw-r--r--   0        0        0     5798 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/qry/qry_inv.py
+-rw-r--r--   0        0        0  9482240 2023-07-17 17:36:26.164947 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/res/db.sqlite3
+-rw-r--r--   0        0        0       67 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/web_search/__init__.py
+-rwxr-xr-x   0        0        0      208 2023-07-17 15:44:39.089366 ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/web_search/browse.py
+-rw-r--r--   0        0        0     1716 2023-07-17 18:50:42.585714 ooo_dev_odh-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ooo_dev_odh-0.1.1/PKG-INFO
```

### Comparing `ooo_dev_odh-0.1.0/LICENSE` & `ooo_dev_odh-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/README.md` & `ooo_dev_odh-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/README.md` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/README.md`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cfg/__pycache__/config.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cfg/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cfg/config.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cfg/config.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cli/hlp.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cli/hlp.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/cli/interactive_hlp.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/cli/interactive_hlp.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,10 +25,10 @@
         cmd (str, optional): odh command. Defaults to "hlp".
     """
     venv = os.environ.get("VIRTUAL_ENV", "")
     if not venv:
         ex_path = Path(sys.executable)
         venv = str(ex_path.parent.parent)
     if platform.system() == "Windows":
-        os.system(f"{sys.executable} {venv}\\Scripts\\odh.exe {cmd} {s}")
+        os.system(f"odh.exe {cmd} {s}")
     else:
-        os.system(f"{sys.executable} {venv}/bin/odh {cmd} {s}")
+        os.system(f"odh {cmd} {s}")
```

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/config.json` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/config.json`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_class/__pycache__/inventory.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_class/__pycache__/inventory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/controller/__pycache__/database_controller.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/controller/__pycache__/database_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/controller/database_controller.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/controller/database_controller.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql_table.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/base_sql_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/db_connect.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/db_connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/init_db.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/init_db.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/sql_ctx.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/sql_ctx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_inventory.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_inventory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_sphinx_info.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/__pycache__/tbl_sphinx_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/base_sql.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/base_sql.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/base_sql_table.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/base_sql_table.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/init_db.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/init_db.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/sql_ctx.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/sql_ctx.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/tbl_inventory.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/tbl_inventory.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/db_class/tbl_sphinx_info.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/db_class/tbl_sphinx_info.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/qry/__pycache__/qry_inv.cpython-310.pyc` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/qry/__pycache__/qry_inv.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/data_manage/qry/qry_inv.py` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/data_manage/qry/qry_inv.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/ooo_dev_cli_hlp/res/db.sqlite3` & `ooo_dev_odh-0.1.1/ooo_dev_cli_hlp/res/db.sqlite3`

 * *Files identical despite different names*

### Comparing `ooo_dev_odh-0.1.0/pyproject.toml` & `ooo_dev_odh-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 entry_point_name = "odh"
 build_dir = "build"
 build_readme="ooo_dev_cli_hlp/README.md"
 build_license="LICENSE"
 
 [tool.poetry]
 name = "ooo-dev-odh"
-version = "0.1.0"
+version = "0.1.1"
 description = "Command Line Help for my OooDev Project"
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 # Do not change this next line. Instead change the custom.metadata.pkg_out_name
 packages = [{include = "ooo_dev_cli_hlp"}]
```

### Comparing `ooo_dev_odh-0.1.0/PKG-INFO` & `ooo_dev_odh-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooo-dev-odh
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command Line Help for my OooDev Project
 License: MIT
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

