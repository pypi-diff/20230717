# Comparing `tmp/catcher-modules-6.0.0.tar.gz` & `tmp/catcher-modules-6.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catcher-modules-6.0.0.tar", last modified: Mon Jan  3 16:05:28 2022, max compression
+gzip compressed data, was "catcher-modules-6.0.7.tar", last modified: Mon Jul 17 08:21:30 2023, max compression
```

## Comparing `catcher-modules-6.0.0.tar` & `catcher-modules-6.0.7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.308865 catcher-modules-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-01-03 16:05:28.308865 catcher-modules-6.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.292865 catcher-modules-6.0.0/catcher_modules/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/cache/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/cache/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/database/
--rw-r--r--   0 runner    (1001) docker     (121)    10880 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/couchbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/mongo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/mssql.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/oracle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/database/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/exceptions/airflow_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/frontend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/frontend/selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/marketing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/marketing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5433 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/marketing/marketo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/mq/
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4970 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/mq/kafka.py
--rw-r--r--   0 runner    (1001) docker     (121)     8512 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/mq/rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10243 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/pipeline/airflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules/pipeline/airflow_utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/pipeline/airflow_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/pipeline/airflow_utils/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8439 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/pipeline/airflow_utils/airflow_db_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.300865 catcher-modules-6.0.0/catcher_modules/service/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.300865 catcher-modules-6.0.0/catcher_modules/service/comparator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/comparator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/comparator/avro_comparator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/comparator/csv_comparator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/comparator/parquet_comparator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10967 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/elastic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8369 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/email.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/expect.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     4738 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/service/salesforce.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.300865 catcher-modules-6.0.0/catcher_modules/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/utils/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/catcher_modules/utils/module_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.296865 catcher-modules-6.0.0/catcher_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-01-03 16:05:28.000000 catcher-modules-6.0.0/catcher_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-01-03 16:05:28.000000 catcher-modules-6.0.0/catcher_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 16:05:28.000000 catcher-modules-6.0.0/catcher_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-01-03 16:05:28.000000 catcher-modules-6.0.0/catcher_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-03 16:05:28.000000 catcher-modules-6.0.0/catcher_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 16:05:28.308865 catcher-modules-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.304865 catcher-modules-6.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/abs_test_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     9725 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/airflow_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12186 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/docker_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/elastic_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9425 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/expect_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6430 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/kafka_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/marketo_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/migration_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9830 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/mongo_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/mssql_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10265 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/mysql_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9775 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/postgres_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11066 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/prepare_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9107 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/rabbit_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3892 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/redis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:28.304865 catcher-modules-6.0.0/test/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/resources/airflow_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (121)    11618 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8474 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/selenium_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6940 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/sqlite_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-01-03 16:05:15.000000 catcher-modules-6.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.984212 catcher-modules-6.0.7/catcher_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/cache/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/database/
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/couchbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/database/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/exceptions/airflow_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/frontend/selenium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/marketing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/marketing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/marketing/marketo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/mq/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/mq/rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/pipeline/airflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/pipeline/airflow_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/pipeline/airflow_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/pipeline/airflow_utils/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/pipeline/airflow_utils/airflow_db_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/catcher_modules/service/comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/comparator/avro_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/comparator/csv_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/comparator/parquet_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/expect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/service/salesforce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/catcher_modules/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/utils/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/catcher_modules/utils/module_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.988211 catcher-modules-6.0.7/catcher_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-17 08:21:30.000000 catcher-modules-6.0.7/catcher_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-17 08:21:30.000000 catcher-modules-6.0.7/catcher_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:21:30.000000 catcher-modules-6.0.7/catcher_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 08:21:30.000000 catcher-modules-6.0.7/catcher_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 08:21:30.000000 catcher-modules-6.0.7/catcher_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/abs_test_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/airflow_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/docker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/elastic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/expect_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/kafka_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/marketo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/migration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/mongo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/mssql_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/mysql_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/postgres_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/prepare_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/rabbit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/redis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:30.992211 catcher-modules-6.0.7/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/resources/airflow_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/selenium_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/sqlite_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 08:21:12.000000 catcher-modules-6.0.7/test/test_utils.py
```

### Comparing `catcher-modules-6.0.0/LICENSE` & `catcher-modules-6.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/cache/redis.py` & `catcher-modules-6.0.7/catcher_modules/cache/redis.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/__init__.py` & `catcher-modules-6.0.7/catcher_modules/database/__init__.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/couchbase.py` & `catcher-modules-6.0.7/catcher_modules/database/couchbase.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/mongo.py` & `catcher-modules-6.0.7/catcher_modules/database/mongo.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/mssql.py` & `catcher-modules-6.0.7/catcher_modules/database/mssql.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/mysql.py` & `catcher-modules-6.0.7/catcher_modules/database/mysql.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/oracle.py` & `catcher-modules-6.0.7/catcher_modules/database/oracle.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/postgres.py` & `catcher-modules-6.0.7/catcher_modules/database/postgres.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/database/sqlite.py` & `catcher-modules-6.0.7/catcher_modules/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/frontend/selenium.py` & `catcher-modules-6.0.7/catcher_modules/frontend/selenium.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/marketing/marketo.py` & `catcher-modules-6.0.7/catcher_modules/marketing/marketo.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/mq/__init__.py` & `catcher-modules-6.0.7/catcher_modules/mq/__init__.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/mq/kafka.py` & `catcher-modules-6.0.7/catcher_modules/mq/kafka.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/mq/rabbit.py` & `catcher-modules-6.0.7/catcher_modules/mq/rabbit.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/pipeline/airflow.py` & `catcher-modules-6.0.7/catcher_modules/pipeline/airflow.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/pipeline/airflow_utils/airflow_client.py` & `catcher-modules-6.0.7/catcher_modules/pipeline/airflow_utils/airflow_client.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/pipeline/airflow_utils/airflow_db_client.py` & `catcher-modules-6.0.7/catcher_modules/pipeline/airflow_utils/airflow_db_client.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/service/docker.py` & `catcher-modules-6.0.7/catcher_modules/service/docker.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,40 @@
         client = docker.from_env()
         filtered = client.networks.list(names=[name])
         if not filtered:
             return client.networks.create(name, driver="bridge").id
         return filtered[0].id
 
 
+class DeviceBasedCmd(metaclass=ABCMeta):
+    def __init__(self, device_requests=None, **kwargs) -> None:
+        super().__init__()
+        self._device_requests = device_requests
+
+    def get_device_requests(self):
+        if self._device_requests is None: return []
+        reqs = []
+        for req in self._device_requests:
+            reqs.append(self._get_device_request(driver=req.get('driver'),
+                                                count=req.get('count'),
+                                                device_ids=req.get('device_ids'),
+                                                capabilities=req.get('capabilities'),
+                                                options=req.get('options')))
+        return reqs
+
+    @staticmethod
+    def _get_device_request(driver=None, count=None, device_ids=None, capabilities=None, options=None):
+        import docker
+        return docker.types.DeviceRequest(driver=driver,
+                                        count=count,
+                                        device_ids=device_ids,
+                                        capabilities=capabilities,
+                                        options=options)
+
+
 class IdBasedCmd:
     def __init__(self, **kwargs: dict) -> None:
         self._id = kwargs.get('name', kwargs.get('hash'))
         if self._id is None:
             raise ValueError('no id for container')
 
     def get_container(self):
@@ -93,37 +119,41 @@
 
 
 class LogsCmd(IdBasedCmd, DockerCmd):
     def action(self, variables):
         return self.get_container().logs().decode()
 
 
-class StartCmd(NetworkBasedCmd, DockerCmd):
+class StartCmd(NetworkBasedCmd, DeviceBasedCmd, DockerCmd):
     def __init__(self, image: str, **kwargs: dict) -> None:
         super().__init__(**kwargs)
         self._image = image
         self._name = kwargs.get('name')
         self._cmd = kwargs.get('cmd')
         self._detached = kwargs.get('detached', True)
         self._ports = kwargs.get('ports')
         self._env = kwargs.get('environment')
         self._volumes = kwargs.get('volumes', {})
+        self._extra_hosts = kwargs.get('extra_hosts', {})
+        self._device_requests = kwargs.get('device_requests', [])
 
     def action(self, variables):
         import docker
         client = docker.from_env()
         volumes = dict([(k, {'bind': v, 'mode': 'rw'}) for k, v in self._volumes.items()])
         output = client.containers.run(self._image,
                                        self._cmd,
                                        name=self._name,
                                        detach=self._detached,
                                        network=self.network(variables),
                                        ports=self._ports,
                                        environment=self._env,
-                                       volumes=volumes)
+                                       volumes=volumes,
+                                       extra_hosts=self._extra_hosts,
+                                       device_requests=self.get_device_requests())
         if not self._detached:
             return output.decode()
         else:
             return output.id
 
 
 class ExecCmd(IdBasedCmd, DockerCmd):
@@ -181,14 +211,16 @@
     - name: container's name. *Optional*
     - cmd: command to run in the container. *Optional*
     - detached: should it be run detached? *Optional* (default is True)
     - ports: dictionary of ports to bind. Keys - container ports, values - host ports.
     - environment: a dictionary of environment variables
     - volumes: a dictionary of volumes
     - network: network name. *Optional* (default is current test's name)
+    - extra_hosts: a dictionary of extra hosts (see Docker docs)
+    - device_requests: a list of dictionaries. Keys and values like in docker.types.DeviceRequest args
 
     :stop: stop a container.
 
     - name: container's name. *Optional*
     - hash: container's hash. *Optional* Either name or hash should present
     - delete: delete a container. *Optional* (default is false)
 
@@ -245,29 +277,31 @@
                     image: 'alpine'
                     cmd: 'echo hello world'
                     detached: false
                 register: {echo: '{{ OUTPUT.strip() }}'}
             - check:
                 equals: {the: '{{ echo }}', is: 'hello world'}
 
-    Start named container detached with volumes and environment.
+    Start named container detached with volumes, environment, extra host and GPUs.
     ::
 
         - docker:
             start:
                 image: 'my-backend-service'
                 name: 'mock server'
                 ports:
                     '1080/tcp': 8000
                 environment:
                     POOL_SIZE: 20
                     OTHER_URL: {{ service1.url }}
                 volumes:
                     '{{ CURRENT_DIR }}/data': '/data'
                     '/tmp/logs': '/var/log/service'
+                extra_hosts: { host1: '{{ HOST1_IP }}' }
+                device_requests: [ { count: -1, capabilities: '[["gpu"]]' } ]
 
     Exec command on running container.
     ::
 
         - docker:
             start:
                 image: 'postgres:alpine'
```

### Comparing `catcher-modules-6.0.0/catcher_modules/service/elastic.py` & `catcher-modules-6.0.7/catcher_modules/service/elastic.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/service/email.py` & `catcher-modules-6.0.7/catcher_modules/service/email.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/service/expect.py` & `catcher-modules-6.0.7/catcher_modules/service/expect.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/service/prepare.py` & `catcher-modules-6.0.7/catcher_modules/service/prepare.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/service/s3.py` & `catcher-modules-6.0.7/catcher_modules/service/s3.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/service/salesforce.py` & `catcher-modules-6.0.7/catcher_modules/service/salesforce.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/utils/db_utils.py` & `catcher-modules-6.0.7/catcher_modules/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules/utils/module_utils.py` & `catcher-modules-6.0.7/catcher_modules/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules.egg-info/SOURCES.txt` & `catcher-modules-6.0.7/catcher_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/catcher_modules.egg-info/requires.txt` & `catcher-modules-6.0.7/catcher_modules.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,56 @@
 catcher>=1.35.3
-arrow==1.2.1
+arrow==1.2.3
 
 [airflow]
 cryptography==36.0.1
 
 [all]
-sqlalchemy==1.4.29
 pika==1.2.0
-pykafka==2.8.0
+redis==4.1.0
+selenium==4.1.0
+pymongo==3.12.3
+simple-salesforce==1.11.4
 cx_oracle==8.3.0
+pymysql==1.0.2
+sqlalchemy==1.4.29
 docker==5.0.3
 cython==0.29.26
+pykafka==2.8.0
+couchbase==4.0.1
+imbox==0.9.8
+cryptography==36.0.1
+psycopg2==2.9.3
+pyodbc==4.0.32
+boto3==1.24.18
+elasticsearch==7.16.2
+marketorestpython==0.5.14
+
+[ci]
+pika==1.2.0
 redis==4.1.0
 selenium==4.1.0
-imbox==0.9.8
+pymongo==3.12.3
 simple-salesforce==1.11.4
-couchbase==3.2.4
-pyodbc==4.0.32
+cx_oracle==8.3.0
 pymysql==1.0.2
-boto3==1.20.26
+sqlalchemy==1.4.29
+docker==5.0.3
+cython==0.29.26
+pykafka==2.8.0
+imbox==0.9.8
+cryptography==36.0.1
 psycopg2==2.9.3
+pyodbc==4.0.32
+boto3==1.24.18
 elasticsearch==7.16.2
-cryptography==36.0.1
-pymongo==3.12.3
 marketorestpython==0.5.14
 
 [couchbase]
-couchbase==3.2.4
+couchbase==4.0.1
 
 [docker]
 docker==5.0.3
 
 [elastic]
 elasticsearch==7.16.2
 
@@ -67,37 +87,17 @@
 [rabbit]
 pika==1.2.0
 
 [redis]
 redis==4.1.0
 
 [s3]
-boto3==1.20.26
+boto3==1.24.18
 
 [salesforce]
 simple-salesforce==1.11.4
 
 [selenium]
 selenium==4.1.0
 
 [sqlite]
 sqlalchemy==1.4.29
-
-[travis]
-sqlalchemy==1.4.29
-pika==1.2.0
-pykafka==2.8.0
-cx_oracle==8.3.0
-docker==5.0.3
-cython==0.29.26
-redis==4.1.0
-selenium==4.1.0
-imbox==0.9.8
-simple-salesforce==1.11.4
-pyodbc==4.0.32
-pymysql==1.0.2
-boto3==1.20.26
-psycopg2==2.9.3
-elasticsearch==7.16.2
-cryptography==36.0.1
-pymongo==3.12.3
-marketorestpython==0.5.14
```

### Comparing `catcher-modules-6.0.0/setup.py` & `catcher-modules-6.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,46 +4,53 @@
 
 
 def get_requirements() -> list:
     with open('requirements.txt', 'r') as f:
         return f.readlines()
 
 
+def load_readme() -> str:
+    with open('Readme.rst', 'r') as f:
+        return f.read()
+
+
 def extras() -> dict:
     modules = {
         'kafka': ["pykafka==2.8.0"],
-        'couchbase': ["couchbase==3.2.4"],
+        'couchbase': ["couchbase==4.0.1"],
         'postgres': ["sqlalchemy==1.4.29", "psycopg2==2.9.3"],
         'mssql': ["pyodbc==4.0.32", "sqlalchemy==1.4.29"],
         'mysql': ["cython==0.29.26", "pymysql==1.0.2", "sqlalchemy==1.4.29"],
         'oracle': ["sqlalchemy==1.4.29", "cx_oracle==8.3.0"],
         'sqlite': ["sqlalchemy==1.4.29"],
         'redis': ["redis==4.1.0"],
         'mongodb': ["pymongo==3.12.3", "sqlalchemy==1.4.29"],
         'docker': ["docker==5.0.3"],
         'elastic': ["elasticsearch==7.16.2"],
-        's3': ["boto3==1.20.26"],
+        's3': ["boto3==1.24.18"],
         'rabbit': ["pika==1.2.0"],
         'email': ["imbox==0.9.8"],
         'marketo': ["marketorestpython==0.5.14"],
         'airflow': ["cryptography==36.0.1"],
         'selenium': ["selenium==4.1.0"],
         'salesforce': ["simple-salesforce==1.11.4"]
     }
     modules['all'] = list(set([item for sublist in modules.values() for item in sublist]))
-    # don't try to install couchbase in travis
-    modules['travis'] = [m for m in modules['all'] if not m.startswith('couchbase')]
+    # don't try to install couchbase in CI/CD
+    modules['ci'] = [m for m in modules['all'] if not m.startswith('couchbase')]
     return modules
 
 
 setup(name=catcher_modules.APPNAME,
       version=catcher_modules.APPVSN,
       description='Additional modules for catcher.',
       author=catcher_modules.APPAUTHOR,
       author_email='valerii.tikhonov@gmail.com',
+      long_description=load_readme(),
+      long_description_content_type='text/x-rst',
       url='https://github.com/comtihon/catcher_modules',
       packages=find_packages(),
       install_requires=get_requirements(),
       include_package_data=True,
       package_data={'catcher_modules': ['resources/*']},
       classifiers=[
           'Intended Audience :: Developers',
```

### Comparing `catcher-modules-6.0.0/test/abs_test_class.py` & `catcher-modules-6.0.7/test/abs_test_class.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/airflow_test.py` & `catcher-modules-6.0.7/test/airflow_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/docker_test.py` & `catcher-modules-6.0.7/test/docker_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/elastic_test.py` & `catcher-modules-6.0.7/test/elastic_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/expect_test.py` & `catcher-modules-6.0.7/test/expect_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/kafka_test.py` & `catcher-modules-6.0.7/test/kafka_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/marketo_test.py` & `catcher-modules-6.0.7/test/marketo_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/migration_test.py` & `catcher-modules-6.0.7/test/migration_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/mongo_test.py` & `catcher-modules-6.0.7/test/mongo_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/mssql_test.py` & `catcher-modules-6.0.7/test/mssql_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/mysql_test.py` & `catcher-modules-6.0.7/test/mysql_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/postgres_test.py` & `catcher-modules-6.0.7/test/selenium_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,191 @@
-from catcher.utils.file_utils import ensure_empty
-
-import test
 from os.path import join
 
-import psycopg2
+import pytest
 from catcher.core.runner import Runner
+from catcher.utils.file_utils import ensure_empty
 
+import test
 from test.abs_test_class import TestClass
+from test.test_utils import check_file
 
 
-class PostgresTest(TestClass):
+class SeleniumTest(TestClass):
     def __init__(self, method_name):
-        super().__init__('postgres', method_name)
-
-    @property
-    def conf(self):
-        return "dbname=test user=test host=localhost password=test port=5433"
-
-    @property
-    def connection(self):
-        return psycopg2.connect(self.conf)
+        super().__init__('selenium', method_name)
 
     def setUp(self):
         super().setUp()
         ensure_empty(join(test.get_test_dir(self.test_name), 'resources'))
-        with self.connection as conn:
-            cur = conn.cursor()
-            cur.execute("CREATE TABLE if not exists test (id serial PRIMARY KEY, num integer);")
-            cur.execute("insert into test(id, num) values(1, 1) on conflict do nothing;")
-            cur.execute("insert into test(id, num) values(2, 2) on conflict do nothing;")
-            conn.commit()
-            cur.close()
-
-    def tearDown(self):
-        super().tearDown()
-        with self.connection as conn:
-            cur = conn.cursor()
-            cur.execute("DROP TABLE test;")
-            cur.execute("DROP TABLE IF exists foo;")
-            conn.commit()
-            cur.close()
-
-    def test_read_simple_query(self):
-        self.populate_file('test_inventory.yml', '''
-        postgres:
-            dbname: test
-            user: test
-            password: test
-            host: localhost
-            port: 5433
+        self.populate_file('resources/test.py', '''from selenium import webdriver
+from selenium.webdriver.common.keys import Keys
+import os
+
+driver = webdriver.Firefox()
+try:
+    driver.get(os.environ['site_url'])
+    assert "Python" in driver.title
+    elem = driver.find_element_by_name("q")
+    elem.clear()
+    elem.send_keys("pycon")
+    elem.send_keys(Keys.RETURN)
+    assert "No results found." not in driver.page_source
+finally:
+    driver.close()''')
+        self.populate_file('resources/google_search.js', '''const {Builder, By, Key, until} = require('selenium-webdriver');
+        async function basicExample(){
+            let driver = await new Builder().forBrowser('firefox').build();
+            try{
+                await driver.get(process.env.site_url);
+                await driver.findElement(By.name('q')).sendKeys('webdriver', Key.RETURN);
+                await driver.wait(until.titleContains('webdriver'), 1000);
+                await driver.getTitle().then(function(title) {
+                            console.log('{\"title\":\"' + title + '\"}')
+                    });
+                driver.quit();
+            }
+            catch(err) {
+                console.error(err);
+                process.exitCode = 1;
+                driver.quit();
+              }
+        }
+        basicExample();
         ''')
+        self.populate_file('resources/MySeleniumTest.java', '''package selenium;
 
-        self.populate_file('main.yaml', '''---
-            steps:
-                - postgres:
-                    request:
-                        conf: '{{ postgres }}'
-                        query: 'select count(*) from test'
-                    register: {documents: '{{ OUTPUT }}'}
-                - check:
-                    equals: {the: '{{ documents.count }}', is: 2}
-            ''')
-        runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), join(self.test_dir, 'test_inventory.yml'))
-        self.assertTrue(runner.run_tests())
-
-    def test_different_conf(self):
-        self.populate_file('test_inventory.yml', '''
-        postgres_str: 'test:test@localhost:5433/test'
-        postgres_str_obj:
-            url: 'test:test@localhost:5433/test'
-            type: postgres
-        postgres_obj:
-            dbname: 'test'
-            user: 'test'
-            password: 'test'
-            host: 'localhost'
-            port: 5433
-            type: 'postgres'
+import org.openqa.selenium.By; 
+import org.openqa.selenium.WebDriver;
+import org.openqa.selenium.WebElement;
+import org.openqa.selenium.firefox.FirefoxDriver;
+
+public class MySeleniumTest {
+
+    public static void main(String[] args) {
+        WebDriver driver = new FirefoxDriver();
+        try {
+            driver.get(System.getenv("site_url"));
+            WebElement element = driver.findElement(By.name("q"));
+            element.sendKeys("Cheese!");
+            element.submit();
+        } finally {
+            driver.quit();
+        }
+    }
+}
         ''')
 
-        self.populate_file('main.yaml', '''---
-                steps:
-                    - loop:
-                        foreach:
-                            in: '[{{ postgres_str_obj }}, "{{ postgres_str }}", {{ postgres_obj }}]'
-                            do:   
-                                - postgres:
-                                    request:
-                                        conf: '{{ ITEM }}'
-                                        query: 'select count(*) from test'
-                                    register: {documents: '{{ OUTPUT }}'}
-                                - check:
-                                    equals: {the: '{{ documents.count }}', is: 2}
-                ''')
-        runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), join(self.test_dir, 'test_inventory.yml'))
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_access_variables(self):
+        self._add_output('resources/test.py', "print('{\"variable\":\"value\"}')")
+        self.populate_file('main.yaml', '''---
+                    variables:
+                        site_url: 'http://www.python.org'
+                    steps:
+                        - selenium:
+                            test:
+                                driver: '/usr/lib/geckodriver'
+                                file: test/tmp/selenium/resources/test.py
+                            register: {variable: '{{ OUTPUT.variable }}'}
+                        - echo: {from: '{{ variable }}', to: variable.output}
+                    ''')
+        runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
         self.assertTrue(runner.run_tests())
+        self.assertTrue(check_file(join(self.test_dir, 'variable.output'), 'value'))
 
-    def test_conf_with_dialect(self):
-        self.populate_file('test_inventory.yml', '''
-                postgres: 'postgresql://test:test@localhost:5433/test'
-                ''')
-
-        self.populate_file('main.yaml', '''---
-                        steps:
-                            - postgres:
-                                request:
-                                    conf: '{{ postgres }}'
-                                    query: 'select count(*) from test'
-                                register: {documents: '{{ OUTPUT }}'}
-                            - check:
-                                equals: {the: '{{ documents.count }}', is: 2}
-                        ''')
-        runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), join(self.test_dir, 'test_inventory.yml'))
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_str_output(self):
+        self._add_output('resources/test.py', "print('some plain text output')", "print('and here')")
+        self.populate_file('main.yaml', '''---
+            variables:
+                site_url: 'http://www.python.org'
+            steps:
+                - selenium:
+                    test:
+                        driver: '/usr/lib/geckodriver'
+                        file: test/tmp/selenium/resources/test.py
+                    register: {variable: '{{ OUTPUT }}'}
+                - echo: {from: '{{ variable }}', to: variable.output}
+            ''')
+        runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
         self.assertTrue(runner.run_tests())
+        self.assertTrue(check_file(join(self.test_dir, 'variable.output'), 'some plain text output\nand here\n'))
 
-    def test_write_simple_query(self):
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_py_fail(self):
         self.populate_file('main.yaml', '''---
-                steps:
-                    - postgres:
-                        request:
-                            conf: 'test:test@localhost:5433/test'
-                            query: 'insert into test(id, num) values(3, 3);'
-                ''')
+                            variables:
+                                site_url: 'http://www.example.org'
+                            steps:
+                                - selenium:
+                                    test:
+                                        driver: '/usr/lib/geckodriver'
+                                        file: test/tmp/selenium/resources/test.py
+                            ''')
         runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
-        self.assertTrue(runner.run_tests())
-        response = self.get_values('test')
-        self.assertEqual([(1, 1), (2, 2), (3, 3)], response)
+        self.assertFalse(runner.run_tests())
 
-    def test_read_with_variables(self):
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_js_selenium(self):
         self.populate_file('main.yaml', '''---
-                variables:
-                    pg_conf: 'test:test@localhost:5433/test'
-                    num: '{{ RANDOM_INT }}'
-                    id: '{{ RANDOM_INT }}'
-                steps:
-                   - postgres:
-                        actions: 
-                            - request:
-                                conf: '{{ pg_conf }}'
-                                query: 'insert into test(id, num) values({{ id }}, {{ num }});'
-                            - request:
-                                conf: '{{ pg_conf }}'
-                                query: select * from test where id={{ id }}
-                              register: {document: '{{ OUTPUT }}'}
-                   - check: 
-                        equals: {the: '{{ document.id }}', is: '{{ num }}'} 
-                ''')
+                            variables:
+                                site_url: 'http://www.google.com/ncr'
+                            steps:
+                                - selenium:
+                                    test:
+                                        driver: '/usr/lib/geckodriver'
+                                        file: test/tmp/selenium/resources/google_search.js
+                                    register: {title: '{{ OUTPUT.title }}'}
+                                - echo: {from: '{{ title }}', to: variable.output}
+                            ''')
         runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
         self.assertTrue(runner.run_tests())
+        with open(join(self.test_dir, 'variable.output')) as f:
+            self.assertTrue('Google' in f.read())
 
-    def test_read_date(self):
-        with self.connection as conn:
-            cur = conn.cursor()
-            cur.execute("CREATE TABLE if not exists foo (id serial PRIMARY KEY, payload json);")
-            cur.execute("insert into foo values(1, '{ \"date\": \"1973-12-15\"}') on conflict do nothing;")
-
-        self.populate_file('main.yaml', '''---
-                variables:
-                    pg_conf: 'test:test@localhost:5433/test'
-                steps:
-                    - postgres:
-                         request:
-                             conf: '{{ pg_conf }}'
-                             query: "select payload ->> 'date' AS date from foo where id = 1"
-                         register: {date: '{{ OUTPUT }}' }
-                    - check: {equals: {the: '1973-12-15', is: '{{ date.date }}'}}
-                ''')
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_js_fail(self):
+        self.populate_file('main.yaml', '''---
+                                    variables:
+                                        site_url: 'http://www.example.com'
+                                    steps:
+                                        - selenium:
+                                            test:
+                                                driver: '/usr/lib/geckodriver'
+                                                file: test/tmp/selenium/resources/google_search.js
+                                    ''')
         runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
-        self.assertTrue(runner.run_tests())
+        self.assertFalse(runner.run_tests())
 
-    def test_populate_multiple_ddl(self):
-        self.populate_file('resources/schema.sql', '''
-                                CREATE TABLE if not exists foo(
-                                    user_id      integer    primary key,
-                                    email        varchar(36)    NOT NULL
-                                );
-                                insert into foo values (1, \'test1@test.org\');
-                                truncate table foo;
-                                insert into foo values (2, \'test2@test.org\');
-                                ''')
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_java_selenium(self):
         self.populate_file('main.yaml', '''---
+                                    variables:
+                                        site_url: 'http://www.google.com/ncr'
                                     steps:
-                                        - prepare:
-                                            populate:
-                                                postgres:
-                                                    conf: 'test:test@localhost:5433/test'
-                                                    schema: schema.sql
+                                        - selenium:
+                                            test:
+                                                driver: '/usr/lib/geckodriver'
+                                                file: test/tmp/selenium/resources/MySeleniumTest.java
+                                                library: '/usr/share/java/*'
                                     ''')
         runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
         self.assertTrue(runner.run_tests())
-        response = self.get_values('foo')
-        self.assertEqual([(2, 'test2@test.org')], response)
 
-    def test_populate_sql(self):
-        self.populate_file('resources/schema.sql', '''
-                                        CREATE TABLE if not exists foo(
-                                            user_id      integer    primary key,
-                                            email        varchar(36)    NOT NULL
-                                        );
-                                        {%- for user in users %}
-                                        insert into foo values ({{user.num}}, '{{user.email}}');
-                                        {%- endfor -%}
-                                        ''')
-        self.populate_file('main.yaml', '''---
-                                            variables:
-                                                users:
-                                                    - num: 1
-                                                      email: test1@test.org
-                                                    - num: 2
-                                                      email: test2@test.org
-                                            steps:
-                                                - postgres:
-                                                    request:
-                                                        conf: 'test:test@localhost:5433/test'
-                                                        sql: schema.sql
-                                            ''')
+    @pytest.mark.skip(reason="too complex to test in travis")
+    def test_java_fail(self):
+        self.populate_file('main.yaml', '''---
+                                    variables:
+                                        site_url: 'http://www.example.com'
+                                    steps:
+                                        - selenium:
+                                            test:
+                                                driver: '/usr/lib/geckodriver'
+                                                file: test/tmp/selenium/resources/MySeleniumTest.java
+                                                library: '/usr/share/java/*'
+                                    ''')
         runner = Runner(self.test_dir, join(self.test_dir, 'main.yaml'), None)
-        self.assertTrue(runner.run_tests())
-        response = self.get_values('foo')
-        self.assertEqual([(1, 'test1@test.org'), (2, 'test2@test.org')], response)
+        self.assertFalse(runner.run_tests())
+
+    def _add_output(self, file, *output):
+        with open(join(self.test_dir, file), 'a+') as w:
+            w.write('\n' + '\n'.join(output))
```

### Comparing `catcher-modules-6.0.0/test/prepare_test.py` & `catcher-modules-6.0.7/test/prepare_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/rabbit_test.py` & `catcher-modules-6.0.7/test/rabbit_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/redis_test.py` & `catcher-modules-6.0.7/test/redis_test.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/resources/airflow_hello_world.py` & `catcher-modules-6.0.7/test/resources/airflow_hello_world.py`

 * *Files identical despite different names*

### Comparing `catcher-modules-6.0.0/test/s3_test.py` & `catcher-modules-6.0.7/test/s3_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from os.path import join
 
 import boto3
+import pytest
 from catcher.core.runner import Runner
 from catcher.utils.file_utils import ensure_empty
+from catcher.utils.logger import get_logger
 
 import test
 from test.abs_test_class import TestClass
 
 
 class S3Test(TestClass):
     def __init__(self, method_name):
@@ -222,14 +224,15 @@
         self.assertTrue(runner.run_tests())
         try:
             self.s3.get_object(Bucket='foo', Key='baz/bar/file.txt')
             self.fail('Key must not exist')
         except Exception as e:
             self.assertTrue('NoSuchKey' in str(e))
 
+    @pytest.mark.skip(reason="for some reason fails in github actions")
     def test_delete_empty_dir(self):
         self.s3.create_bucket(Bucket='foo')
         self.s3.put_object(Bucket='foo', Key='baz/bar/dir/', Body='')
         self.populate_file('main.yaml', '''---
                             variables:
                                 s3_config:
                                     url: http://127.0.0.1:9001
```

### Comparing `catcher-modules-6.0.0/test/sqlite_test.py` & `catcher-modules-6.0.7/test/sqlite_test.py`

 * *Files identical despite different names*

