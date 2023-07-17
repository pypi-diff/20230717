# Comparing `tmp/mystring-0.0.98.tar.gz` & `tmp/mystring-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystring-0.0.98.tar", last modified: Thu Jun 29 16:26:08 2023, max compression
+gzip compressed data, was "mystring-0.0.99.tar", last modified: Thu Jun 29 16:28:14 2023, max compression
```

## Comparing `mystring-0.0.98.tar` & `mystring-0.0.99.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:26:08.389319 mystring-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 16:26:02.000000 mystring-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 16:26:08.389319 mystring-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 16:26:02.000000 mystring-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:26:08.389319 mystring-0.0.98/mystring/
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-06-29 16:26:02.000000 mystring-0.0.98/mystring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:26:08.389319 mystring-0.0.98/mystring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 16:26:08.000000 mystring-0.0.98/mystring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 16:26:08.000000 mystring-0.0.98/mystring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:26:08.000000 mystring-0.0.98/mystring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 16:26:08.000000 mystring-0.0.98/mystring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 16:26:08.000000 mystring-0.0.98/mystring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:26:08.389319 mystring-0.0.98/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3476 2023-06-29 16:26:02.000000 mystring-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:28:14.133620 mystring-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 16:28:09.000000 mystring-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 16:28:14.129620 mystring-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 16:28:09.000000 mystring-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:28:14.129620 mystring-0.0.99/mystring/
+-rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-06-29 16:28:09.000000 mystring-0.0.99/mystring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:28:14.129620 mystring-0.0.99/mystring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 16:28:14.000000 mystring-0.0.99/mystring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 16:28:14.000000 mystring-0.0.99/mystring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:28:14.000000 mystring-0.0.99/mystring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 16:28:14.000000 mystring-0.0.99/mystring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 16:28:14.000000 mystring-0.0.99/mystring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:28:14.133620 mystring-0.0.99/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3476 2023-06-29 16:28:09.000000 mystring-0.0.99/setup.py
```

### Comparing `mystring-0.0.98/LICENSE` & `mystring-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `mystring-0.0.98/mystring/__init__.py` & `mystring-0.0.99/mystring/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,14 +428,15 @@
 			self.rename_column(column, str(column_itr)+"_"+column)
 		return self
 	
 	def to_sqlite(self, file="out.sqlite", table_name="default"):
 		from sqlalchemy import create_engine
 		with create_engine('sqlite://{0}'.format(file), echo=False).begin() as connection:
 			self.to_sql(table_name, con=connection, if_exists='replace')
+		return file
 
 	def to_sqlcreate(self, file="out.sql", name="temp", number_columnz = False, every_x_rows=-1):
 		working = self.dup()
 
 		if number_columnz:
 			working.enumerate_kol()
 			#columns = working.kolz
```

### Comparing `mystring-0.0.98/setup.py` & `mystring-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.98"
+VERSION = "0.0.99"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

