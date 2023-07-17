# Comparing `tmp/barladb-0.1.5.tar.gz` & `tmp/barladb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barladb-0.1.5.tar", last modified: Sun Jul 16 10:49:17 2023, max compression
+gzip compressed data, was "barladb-0.1.7.tar", last modified: Mon Jul 17 12:14:55 2023, max compression
```

## Comparing `barladb-0.1.5.tar` & `barladb-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:17.492751 barladb-0.1.5/
--rw-rw-rw-   0        0        0     3588 2023-07-16 10:49:17.492751 barladb-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:17.488686 barladb-0.1.5/barladb/
--rw-rw-rw-   0        0        0      342 2023-07-15 11:58:29.000000 barladb-0.1.5/barladb/classes.py
--rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.5/barladb/config.py
--rw-rw-rw-   0        0        0     2979 2023-07-16 10:29:28.000000 barladb-0.1.5/barladb/db.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:17.491694 barladb-0.1.5/barladb.egg-info/
--rw-rw-rw-   0        0        0     3588 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 14:32:44.000000 barladb-0.1.5/barladb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:49:17.493803 barladb-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     3723 2023-07-16 10:34:55.000000 barladb-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:14:55.624768 barladb-0.1.7/
+-rw-rw-rw-   0        0        0     3456 2023-07-17 12:14:55.624768 barladb-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 12:14:55.619618 barladb-0.1.7/barladb/
+-rw-rw-rw-   0        0        0     1085 2023-07-17 11:56:23.000000 barladb-0.1.7/barladb/classes.py
+-rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.7/barladb/config.py
+-rw-rw-rw-   0        0        0     4307 2023-07-17 11:58:32.000000 barladb-0.1.7/barladb/db.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:14:55.623746 barladb-0.1.7/barladb.egg-info/
+-rw-rw-rw-   0        0        0     3456 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:14:55.624768 barladb-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     3618 2023-07-17 12:14:09.000000 barladb-0.1.7/setup.py
```

### Comparing `barladb-0.1.5/PKG-INFO` & `barladb-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.5
+Version: 0.1.7
 Summary: A very easy local database based on JSON
+Home-page: https://sites.google.com/view/barladb/
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
+Project-URL: Documentation, https://sites.google.com/view/barladb/
 Description-Content-Type: text/markdown
 
 
 # Изменения:
-- Добавлена новая тестовая функция:
+- Добавлены новые функции и документация - https://sites.google.com/view/barladb/
 ```python
-db.search(filepath, key)
+db.remove_column(filepath, key)
+db.columns(filepath)
 ```
-- Она парсит файл БД, и в случае прям точного совпадения (К примеру `age = age`) показывает значение данного столбца
-- В скором добавлю показывание нескольких совпадений (К примеру `age, ages`)
+
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
```

### Comparing `barladb-0.1.5/barladb.egg-info/PKG-INFO` & `barladb-0.1.7/barladb.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.5
+Version: 0.1.7
 Summary: A very easy local database based on JSON
+Home-page: https://sites.google.com/view/barladb/
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
+Project-URL: Documentation, https://sites.google.com/view/barladb/
 Description-Content-Type: text/markdown
 
 
 # Изменения:
-- Добавлена новая тестовая функция:
+- Добавлены новые функции и документация - https://sites.google.com/view/barladb/
 ```python
-db.search(filepath, key)
+db.remove_column(filepath, key)
+db.columns(filepath)
 ```
-- Она парсит файл БД, и в случае прям точного совпадения (К примеру `age = age`) показывает значение данного столбца
-- В скором добавлю показывание нескольких совпадений (К примеру `age, ages`)
+
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
```

### Comparing `barladb-0.1.5/setup.py` & `barladb-0.1.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 setup(
     name='barladb',
-    version='0.1.5',
+    version='0.1.7',
     description='A very easy local database based on JSON',
     packages=['barladb'],
     author_email='sasaigrypocta@gmail.com',
     author="barlin41k",
     zip_safe=False,
     long_description='''
 # Изменения:
-- Добавлена новая тестовая функция:
+- Добавлены новые функции и документация - https://sites.google.com/view/barladb/
 ```python
-db.search(filepath, key)
+db.remove_column(filepath, key)
+db.columns(filepath)
 ```
-- Она парсит файл БД, и в случае прям точного совпадения (К примеру `age = age`) показывает значение данного столбца
-- В скором добавлю показывание нескольких совпадений (К примеру `age, ages`)
+
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
@@ -51,8 +51,12 @@
 - `pip install barladb`
 
 # Особенности barlaDB
 - Простота в использовании
 - Очень лёгкий интерфейс
 - Базирована на всеми известном `JSON`
     ''',
-    long_description_content_type="text/markdown",)
+    long_description_content_type="text/markdown",
+    url="https://sites.google.com/view/barladb/",
+    project_urls={
+        "Documentation": "https://sites.google.com/view/barladb/",
+    })
```

