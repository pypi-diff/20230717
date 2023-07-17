# Comparing `tmp/treemodel2sql-0.1.0.tar.gz` & `tmp/treemodel2sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treemodel2sql-0.1.0.tar", last modified: Mon Jul 17 02:33:58 2023, max compression
+gzip compressed data, was "dist/treemodel2sql-0.1.1.tar", last modified: Mon Jul 17 12:43:55 2023, max compression
```

## Comparing `treemodel2sql-0.1.0.tar` & `treemodel2sql-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/.editorconfig
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/.github/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      324 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/.gitignore
--rw-r--r--   0 ryanzheng   (501) staff       (20)      693 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/.travis.yml
--rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/AUTHORS.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3583 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/HISTORY.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/LICENSE
--rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/MANIFEST.in
--rw-r--r--   0 ryanzheng   (501) staff       (20)     2301 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)    43474 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)    42732 2023-07-17 01:46:18.000000 treemodel2sql-0.1.0/README.md
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/docs/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      614 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/authors.rst
--rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4847 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/conf.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/contributing.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/history.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      310 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/index.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1166 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/installation.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      811 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/make.bat
--rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/readme.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       81 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/docs/usage.rst
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/examples/
--rw-r--r--   0 ryanzheng   (501) staff       (20)   114849 2023-07-16 14:07:18.000000 treemodel2sql-0.1.0/examples/tutorial_code_lightgbm_model_transform_sql.ipynb
--rw-r--r--   0 ryanzheng   (501) staff       (20)   100000 2023-07-16 07:19:40.000000 treemodel2sql-0.1.0/examples/tutorial_code_xgboost_model_transform_sql.ipynb
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/images/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    39768 2023-06-11 07:05:08.000000 treemodel2sql-0.1.0/images/干饭人.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)    27731 2023-06-10 10:02:05.000000 treemodel2sql-0.1.0/images/魔都数据干饭人.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)       26 2023-07-16 14:06:54.000000 treemodel2sql-0.1.0/requirements.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)      430 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/setup.cfg
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1710 2023-07-16 06:35:12.000000 treemodel2sql-0.1.0/setup.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/tests/
--rw-r--r--   0 ryanzheng   (501) staff       (20)       43 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/tests/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)      571 2023-07-15 14:18:03.000000 treemodel2sql-0.1.0/tests/test_treemodel2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      200 2023-07-16 06:49:05.000000 treemodel2sql-0.1.0/treemodel2sql/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4656 2023-07-16 05:19:29.000000 treemodel2sql-0.1.0/treemodel2sql/lgb2sql.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     7583 2023-06-11 02:53:26.000000 treemodel2sql-0.1.0/treemodel2sql/xgboost2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    43474 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)      898 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       57 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/not-zip-safe
--rw-r--r--   0 ryanzheng   (501) staff       (20)       25 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/requires.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       14 2023-07-17 02:33:58.000000 treemodel2sql-0.1.0/treemodel2sql.egg-info/top_level.txt
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.editorconfig
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/.github/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      324 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.gitignore
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      693 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.travis.yml
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/AUTHORS.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3583 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-07-17 12:41:25.000000 treemodel2sql-0.1.1/HISTORY.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/LICENSE
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/MANIFEST.in
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     2301 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    32641 2023-07-17 12:39:53.000000 treemodel2sql-0.1.1/README.md
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/docs/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      614 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4847 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/conf.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/contributing.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/history.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      310 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/index.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1166 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/installation.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      811 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/make.bat
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/readme.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       81 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/usage.rst
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/examples/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   115765 2023-07-17 12:40:38.000000 treemodel2sql-0.1.1/examples/tutorial_code_lightgbm_model_transform_sql.ipynb
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   100911 2023-07-17 12:40:39.000000 treemodel2sql-0.1.1/examples/tutorial_code_xgboost_model_transform_sql.ipynb
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/images/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    39768 2023-06-11 07:05:08.000000 treemodel2sql-0.1.1/images/干饭人.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    27731 2023-06-10 10:02:05.000000 treemodel2sql-0.1.1/images/魔都数据干饭人.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       26 2023-07-16 14:06:54.000000 treemodel2sql-0.1.1/requirements.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      430 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/setup.cfg
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1710 2023-07-17 12:40:47.000000 treemodel2sql-0.1.1/setup.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/tests/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       43 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/tests/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      571 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/tests/test_treemodel2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      200 2023-07-16 06:49:05.000000 treemodel2sql-0.1.1/treemodel2sql/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     4656 2023-07-16 05:19:29.000000 treemodel2sql-0.1.1/treemodel2sql/lgb2sql.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     7583 2023-06-11 02:53:26.000000 treemodel2sql-0.1.1/treemodel2sql/xgboost2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      898 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       57 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/not-zip-safe
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       25 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/requires.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       14 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/top_level.txt
```

### Comparing `treemodel2sql-0.1.0/.gitignore` & `treemodel2sql-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/.travis.yml` & `treemodel2sql-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/CONTRIBUTING.rst` & `treemodel2sql-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/LICENSE` & `treemodel2sql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/Makefile` & `treemodel2sql-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/docs/Makefile` & `treemodel2sql-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/docs/conf.py` & `treemodel2sql-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/docs/installation.rst` & `treemodel2sql-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/docs/make.bat` & `treemodel2sql-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/examples/tutorial_code_lightgbm_model_transform_sql.ipynb` & `treemodel2sql-0.1.1/examples/tutorial_code_lightgbm_model_transform_sql.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985054112554113%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '###训练1个lightgbm二分类模型\\n')], delete: [0]}}, 4: "*

 * *            "{'source': {insert: [(0, 'from treemodel2sql import Lgb2Sql\\n'), (1, "*

 * *            "'###使用treemodel2sql包将模型转换成的sql语句\\n')], delete: [1, 0]}}, 5: {'source': {insert: "*

 * *            "[(14, 'sql_pred_df.head(2)\\n'), (15, '\\n'), (16, '\\n'), (17, '# "*

 * *            "###注意如果核验的测试数据集在本地的某个路径下，使用如下方式读取测试数据\\n'), (18, '# "*

 * *            "###注意如果核验的测试数据集在本地的某个路径下，使用如下方式读取测试数据\\n'), (19, '# "*

 * *            "###注意如果核验的测 […]*

```diff
@@ -925,15 +925,15 @@
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "###\u8bad\u7ec31\u4e2axgboost\u4e8c\u5206\u7c7b\u6a21\u578b\n",
+                "###\u8bad\u7ec31\u4e2alightgbm\u4e8c\u5206\u7c7b\u6a21\u578b\n",
                 "import lightgbm as lgb\n",
                 "from sklearn.datasets import make_classification\n",
                 "from sklearn.model_selection import train_test_split\n",
                 "\n",
                 "X, y = make_classification(n_samples=10000,\n",
                 "                           n_features=10,\n",
                 "                           n_informative=3,\n",
@@ -1373,16 +1373,16 @@
                         "\t\tas tree_2_score\n",
                         "        from data_table)\n",
                         "        \n"
                     ]
                 }
             ],
             "source": [
-                "from lgb2sql import Lgb2Sql\n",
-                "###\u4f7f\u7528xgboost2sql\u5305\u5c06\u6a21\u578b\u8f6c\u6362\u6210\u7684sql\u8bed\u53e5\n",
+                "from treemodel2sql import Lgb2Sql\n",
+                "###\u4f7f\u7528treemodel2sql\u5305\u5c06\u6a21\u578b\u8f6c\u6362\u6210\u7684sql\u8bed\u53e5\n",
                 "lgb2sql = Lgb2Sql()\n",
                 "sql_str = lgb2sql.transform(model)\n",
                 "print(sql_str)"
             ]
         },
         {
             "cell_type": "code",
@@ -1451,15 +1451,29 @@
                 "X_test_df.rename(columns={'index':'key'}, inplace=True)\n",
                 "values = X_test_df.values.tolist()\n",
                 "columns = X_test_df.columns.tolist()\n",
                 "spark_df = spark.createDataFrame(values, columns)\n",
                 "spark_df.createOrReplaceTempView('data_table')\n",
                 "sql_pred_pysdf = spark.sql(sql_str)\n",
                 "sql_pred_df = sql_pred_pysdf.toPandas()\n",
-                "sql_pred_df.head(2)"
+                "sql_pred_df.head(2)\n",
+                "\n",
+                "\n",
+                "# ###\u6ce8\u610f\u5982\u679c\u6838\u9a8c\u7684\u6d4b\u8bd5\u6570\u636e\u96c6\u5728\u672c\u5730\u7684\u67d0\u4e2a\u8def\u5f84\u4e0b\uff0c\u4f7f\u7528\u5982\u4e0b\u65b9\u5f0f\u8bfb\u53d6\u6d4b\u8bd5\u6570\u636e\n",
+                "# ###\u6ce8\u610f\u5982\u679c\u6838\u9a8c\u7684\u6d4b\u8bd5\u6570\u636e\u96c6\u5728\u672c\u5730\u7684\u67d0\u4e2a\u8def\u5f84\u4e0b\uff0c\u4f7f\u7528\u5982\u4e0b\u65b9\u5f0f\u8bfb\u53d6\u6d4b\u8bd5\u6570\u636e\n",
+                "# ###\u6ce8\u610f\u5982\u679c\u6838\u9a8c\u7684\u6d4b\u8bd5\u6570\u636e\u96c6\u5728\u672c\u5730\u7684\u67d0\u4e2a\u8def\u5f84\u4e0b\uff0c\u4f7f\u7528\u5982\u4e0b\u65b9\u5f0f\u8bfb\u53d6\u6d4b\u8bd5\u6570\u636e\n",
+                "# from pyspark.sql import SparkSession\n",
+                "# spark = SparkSession.builder.getOrCreate()\n",
+                "\n",
+                "# spark_df = spark.read.format(\"csv\").option(\"header\", \"true\").option(\"inferSchema\", \"True\").load(\"/Users/ryanzheng/resources/test_data.csv\")\n",
+                "# spark_df = spark_df.withColumnRenamed(\"device_md5\", \"key\")\n",
+                "# spark_df.createOrReplaceTempView('data_table')\n",
+                "# sql_pred_pysdf = spark.sql(sql_str)\n",
+                "# sql_pred_df = sql_pred_pysdf.toPandas()\n",
+                "# sql_pred_df.head(2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
```

### Comparing `treemodel2sql-0.1.0/examples/tutorial_code_xgboost_model_transform_sql.ipynb` & `treemodel2sql-0.1.1/examples/tutorial_code_xgboost_model_transform_sql.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986190476190476%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, 'from treemodel2sql import XGBoost2Sql\\n'), (1, "*

 * *            "'###使用treemodel2sql包将模型转换成的sql语句\\n')], delete: [1, 0]}}, 5: {'source': {insert: "*

 * *            "[(14, 'sql_pred_df.head(2)\\n'), (15, '\\n'), (16, '\\n'), (17, '# "*

 * *            "###注意如果核验的测试数据集在本地的某个路径下，使用如下方式读取测试数据\\n'), (18, '# "*

 * *            "###注意如果核验的测试数据集在本地的某个路径下，使用如下方式读取测试数据\\n'), (19, '# "*

 * *            "###注意如果核验的测试数据集在本地的某个路径下，使用如下方式读取测试数据\\n'), (20, '# from pyspark.sql import "*

 * *            "Spa […]*

```diff
@@ -1392,16 +1392,16 @@
                         "\t\tas tree_3_score\n",
                         "    from data_table)\n",
                         "    \n"
                     ]
                 }
             ],
             "source": [
-                "from xgboost2sql import XGBoost2Sql\n",
-                "###\u4f7f\u7528xgboost2sql\u5305\u5c06\u6a21\u578b\u8f6c\u6362\u6210\u7684sql\u8bed\u53e5\n",
+                "from treemodel2sql import XGBoost2Sql\n",
+                "###\u4f7f\u7528treemodel2sql\u5305\u5c06\u6a21\u578b\u8f6c\u6362\u6210\u7684sql\u8bed\u53e5\n",
                 "xgb2sql = XGBoost2Sql()\n",
                 "sql_str = xgb2sql.transform(model)\n",
                 "print(sql_str)"
             ]
         },
         {
             "cell_type": "code",
@@ -1470,15 +1470,29 @@
                 "X_test_df.rename(columns={'index':'key'}, inplace=True)\n",
                 "values = X_test_df.values.tolist()\n",
                 "columns = X_test_df.columns.tolist()\n",
                 "spark_df = spark.createDataFrame(values, columns)\n",
                 "spark_df.createOrReplaceTempView('data_table')\n",
                 "sql_pred_pysdf = spark.sql(sql_str)\n",
                 "sql_pred_df = sql_pred_pysdf.toPandas()\n",
-                "sql_pred_df.head(2)"
+                "sql_pred_df.head(2)\n",
+                "\n",
+                "\n",
+                "# ###\u6ce8\u610f\u5982\u679c\u6838\u9a8c\u7684\u6d4b\u8bd5\u6570\u636e\u96c6\u5728\u672c\u5730\u7684\u67d0\u4e2a\u8def\u5f84\u4e0b\uff0c\u4f7f\u7528\u5982\u4e0b\u65b9\u5f0f\u8bfb\u53d6\u6d4b\u8bd5\u6570\u636e\n",
+                "# ###\u6ce8\u610f\u5982\u679c\u6838\u9a8c\u7684\u6d4b\u8bd5\u6570\u636e\u96c6\u5728\u672c\u5730\u7684\u67d0\u4e2a\u8def\u5f84\u4e0b\uff0c\u4f7f\u7528\u5982\u4e0b\u65b9\u5f0f\u8bfb\u53d6\u6d4b\u8bd5\u6570\u636e\n",
+                "# ###\u6ce8\u610f\u5982\u679c\u6838\u9a8c\u7684\u6d4b\u8bd5\u6570\u636e\u96c6\u5728\u672c\u5730\u7684\u67d0\u4e2a\u8def\u5f84\u4e0b\uff0c\u4f7f\u7528\u5982\u4e0b\u65b9\u5f0f\u8bfb\u53d6\u6d4b\u8bd5\u6570\u636e\n",
+                "# from pyspark.sql import SparkSession\n",
+                "# spark = SparkSession.builder.getOrCreate()\n",
+                "\n",
+                "# spark_df = spark.read.format(\"csv\").option(\"header\", \"true\").option(\"inferSchema\", \"True\").load(\"/Users/ryanzheng/resources/test_data.csv\")\n",
+                "# spark_df = spark_df.withColumnRenamed(\"device_md5\", \"key\")\n",
+                "# spark_df.createOrReplaceTempView('data_table')\n",
+                "# sql_pred_pysdf = spark.sql(sql_str)\n",
+                "# sql_pred_df = sql_pred_pysdf.toPandas()\n",
+                "# sql_pred_df.head(2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
```

### Comparing `treemodel2sql-0.1.0/images/干饭人.png` & `treemodel2sql-0.1.1/images/干饭人.png`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/images/魔都数据干饭人.png` & `treemodel2sql-0.1.1/images/魔都数据干饭人.png`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/setup.py` & `treemodel2sql-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     include_package_data=True,
     keywords='treemodel2sql',
     name=NAME,
     packages=find_packages(include=['treemodel2sql', 'treemodel2sql.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZhengRyan/treemodel2sql',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `treemodel2sql-0.1.0/tests/test_treemodel2sql.py` & `treemodel2sql-0.1.1/tests/test_treemodel2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/treemodel2sql/lgb2sql.py` & `treemodel2sql-0.1.1/treemodel2sql/lgb2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/treemodel2sql/xgboost2sql.py` & `treemodel2sql-0.1.1/treemodel2sql/xgboost2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.0/treemodel2sql.egg-info/SOURCES.txt` & `treemodel2sql-0.1.1/treemodel2sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

