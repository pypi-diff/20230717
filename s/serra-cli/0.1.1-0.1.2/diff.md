# Comparing `tmp/serra_cli-0.1.1.tar.gz` & `tmp/serra_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra_cli-0.1.1.tar", last modified: Mon Jul 17 09:40:38 2023, max compression
+gzip compressed data, was "serra_cli-0.1.2.tar", last modified: Mon Jul 17 11:37:46 2023, max compression
```

## Comparing `serra_cli-0.1.1.tar` & `serra_cli-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-07-17 09:40:38.193782 serra_cli-0.1.1/
--rw-r--r--   0 albertstanley   (501) staff       (20)      211 2023-07-17 09:40:38.193499 serra_cli-0.1.1/PKG-INFO
--rw-r--r--   0 albertstanley   (501) staff       (20)      150 2023-07-17 00:13:30.000000 serra_cli-0.1.1/README.md
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-07-17 09:40:38.191196 serra_cli-0.1.1/serra_cli/
--rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-07-15 19:07:34.000000 serra_cli-0.1.1/serra_cli/__init__.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     3225 2023-07-17 09:23:05.000000 serra_cli-0.1.1/serra_cli/cli.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      906 2023-07-16 05:07:03.000000 serra_cli-0.1.1/serra_cli/utils.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-07-17 09:40:38.193143 serra_cli-0.1.1/serra_cli.egg-info/
--rw-r--r--   0 albertstanley   (501) staff       (20)      211 2023-07-17 09:40:38.000000 serra_cli-0.1.1/serra_cli.egg-info/PKG-INFO
--rw-r--r--   0 albertstanley   (501) staff       (20)      308 2023-07-17 09:40:38.000000 serra_cli-0.1.1/serra_cli.egg-info/SOURCES.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-07-17 09:40:38.000000 serra_cli-0.1.1/serra_cli.egg-info/dependency_links.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)       46 2023-07-17 09:40:38.000000 serra_cli-0.1.1/serra_cli.egg-info/entry_points.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-07-15 19:19:11.000000 serra_cli-0.1.1/serra_cli.egg-info/not-zip-safe
--rw-r--r--   0 albertstanley   (501) staff       (20)       20 2023-07-17 09:40:38.000000 serra_cli-0.1.1/serra_cli.egg-info/requires.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)       10 2023-07-17 09:40:38.000000 serra_cli-0.1.1/serra_cli.egg-info/top_level.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)       38 2023-07-17 09:40:38.193868 serra_cli-0.1.1/setup.cfg
--rw-r--r--   0 albertstanley   (501) staff       (20)      503 2023-07-17 09:39:42.000000 serra_cli-0.1.1/setup.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-07-17 11:37:46.067047 serra_cli-0.1.2/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      211 2023-07-17 11:37:46.066749 serra_cli-0.1.2/PKG-INFO
+-rw-r--r--   0 albertstanley   (501) staff       (20)      150 2023-07-17 00:13:30.000000 serra_cli-0.1.2/README.md
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-07-17 11:37:46.063060 serra_cli-0.1.2/serra_cli/
+-rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-07-15 19:07:34.000000 serra_cli-0.1.2/serra_cli/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3219 2023-07-17 11:30:57.000000 serra_cli-0.1.2/serra_cli/cli.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      906 2023-07-16 05:07:03.000000 serra_cli-0.1.2/serra_cli/utils.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-07-17 11:37:46.066381 serra_cli-0.1.2/serra_cli.egg-info/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      211 2023-07-17 11:37:46.000000 serra_cli-0.1.2/serra_cli.egg-info/PKG-INFO
+-rw-r--r--   0 albertstanley   (501) staff       (20)      308 2023-07-17 11:37:46.000000 serra_cli-0.1.2/serra_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-07-17 11:37:46.000000 serra_cli-0.1.2/serra_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       46 2023-07-17 11:37:46.000000 serra_cli-0.1.2/serra_cli.egg-info/entry_points.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-07-15 19:19:11.000000 serra_cli-0.1.2/serra_cli.egg-info/not-zip-safe
+-rw-r--r--   0 albertstanley   (501) staff       (20)       20 2023-07-17 11:37:46.000000 serra_cli-0.1.2/serra_cli.egg-info/requires.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       10 2023-07-17 11:37:46.000000 serra_cli-0.1.2/serra_cli.egg-info/top_level.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       38 2023-07-17 11:37:46.067144 serra_cli-0.1.2/setup.cfg
+-rw-r--r--   0 albertstanley   (501) staff       (20)      503 2023-07-17 11:37:40.000000 serra_cli-0.1.2/setup.py
```

### Comparing `serra_cli-0.1.1/serra_cli/cli.py` & `serra_cli-0.1.2/serra_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         try:
             response = requests.post(url, data={'session_id': session_id}, files={'file': file})
             # Store the response in the shared variable
             response_holder['response'] = response
         except: 
             pass
 
-@main.command(name="run_local")
+@main.command(name="run")
 @click.argument("job_name")
 def cli_run_job_from_job_dir(job_name):
     """Run a specific job
     """
     # Send config to aws
     # tell aws server to run code and wait for response
     # Set the URL of the Flask endpoint
```

### Comparing `serra_cli-0.1.1/serra_cli/utils.py` & `serra_cli-0.1.2/serra_cli/utils.py`

 * *Files identical despite different names*

