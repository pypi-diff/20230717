# Comparing `tmp/cipromote-1.2.0.tar.gz` & `tmp/cipromote-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipromote-1.2.0.tar", max compression
+gzip compressed data, was "cipromote-1.3.0.tar", max compression
```

## Comparing `cipromote-1.2.0.tar` & `cipromote-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.2.0/README.md
--rw-r--r--   0        0        0      548 2023-07-14 11:50:44.367941 cipromote-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.2.0/src/cipromote/__init__.py
--rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.2.0/src/cipromote/ci-cli.py
--rw-r--r--   0        0        0    10721 2023-07-14 11:50:00.910215 cipromote-1.2.0/src/cipromote/cli.py
--rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.2.0/src/cipromote/constants.py
--rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.2.0/src/cipromote/instances.py
--rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.2.0/src/cipromote/label_versions.py
--rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.2.0/src/cipromote/labels.py
--rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.2.0/src/cipromote/login.py
--rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.2.0/src/cipromote/loginInput.py
--rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.2.0/src/cipromote/projects.py
--rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.2.0/src/cipromote/queries.py
--rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.2.0/src/cipromote/versioned_items.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.3.0/README.md
+-rw-r--r--   0        0        0      548 2023-07-17 21:27:06.094123 cipromote-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.3.0/src/cipromote/__init__.py
+-rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.3.0/src/cipromote/ci-cli.py
+-rw-r--r--   0        0        0    12027 2023-07-17 21:26:16.369881 cipromote-1.3.0/src/cipromote/cli.py
+-rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.3.0/src/cipromote/constants.py
+-rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.3.0/src/cipromote/instances.py
+-rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.3.0/src/cipromote/label_versions.py
+-rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.3.0/src/cipromote/labels.py
+-rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.3.0/src/cipromote/login.py
+-rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.3.0/src/cipromote/loginInput.py
+-rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.3.0/src/cipromote/projects.py
+-rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.3.0/src/cipromote/queries.py
+-rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.3.0/src/cipromote/versioned_items.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.3.0/PKG-INFO
```

### Comparing `cipromote-1.2.0/pyproject.toml` & `cipromote-1.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cipromote"
-version = "1.2.0"
+version = "1.3.0"
 description = "Promote MotionCI Labels"
 authors = ["Michael MacKenna <mmackenna@ufginsurance.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
```

### Comparing `cipromote-1.2.0/src/cipromote/ci-cli.py` & `cipromote-1.3.0/src/cipromote/ci-cli.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/cli.py` & `cipromote-1.3.0/src/cipromote/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import cipromote.instances as instances
 import cipromote.queries as queries
 import cipromote.loginInput as loginInput
 import cipromote.login as login
 import cipromote.labels as labels
 import cipromote.label_versions as label_versions
 import cipromote.projects as projects
+import logging
 from termcolor import cprint
 from pprint import pprint
 from requests import Session
 from requests.auth import HTTPBasicAuth
 from urllib3.exceptions import InsecureRequestWarning
 
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
@@ -63,15 +64,14 @@
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
     constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
     print('Sending query to the following url')
     print(constants.GRAPH_URL)
     instance_object = instances.get_instances_default()
     pprint(instance_object)
-    print(f"Instance 0 has these namespaces {instance_object[0]['node']['namespaces']}")
     return instance_object
 
 @main.command("get-instance", short_help="Get an instance by name")
 @click.argument("instance-name")
 def get_instance(instance_name):
     """ Get a particular instance by name """
     server_url = os.getenv("MOTIOCI_SERVERURL")
@@ -86,15 +86,15 @@
             print(f"The target instance is {target_instance['name']}")
             pprint(target_instance)
     return target_instance
 
 @main.command("monitor-instance", short_help="Check an instance by name every X seconds")
 @click.argument("instance-name")
 @click.argument("seconds")
-def get_instance(instance_name, seconds):
+def monitor_instance(instance_name, seconds):
     """ Check a particular instance by name every X seconds """
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
     constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
     print('Sending query to the following url')
     print(constants.GRAPH_URL)
     while True:
@@ -103,14 +103,46 @@
             if instance['node']['name'].lower() == instance_name.lower():
                 target_instance = instance['node']
                 print(f"The target instance is {target_instance['name']}")
                 pprint(target_instance)
                 time.sleep(int(seconds))
     return target_instance
 
+
+@main.command("monitor-instance-namespaces", short_help="Check namespaces for a particular instance every X seconds")
+@click.argument("instance-name")
+@click.argument("namespaces")
+@click.argument("seconds")
+def monitor_instance_namespaces(instance_name, namespaces, seconds):
+    """ Check a particular instance by name every X seconds """
+    server_url = os.getenv("MOTIOCI_SERVERURL")
+    constants.CI_URL = server_url
+    constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
+    svc_names = namespaces.split(",")
+    logging.basicConfig(
+            format='%(asctime)s %(levelname)-8s %(message)s',
+            level=logging.INFO,
+            datefmt='%Y-%m-%d %H:%M:%S')
+    while True:
+        instance_object = instances.get_instances_default()
+        for instance in instance_object:
+            if instance['node']['name'].lower() == instance_name.lower():
+                target_instance = instance['node']
+                up = []
+                for ns in target_instance['namespaces']:
+                    up.append(ns['name'].lower())
+                for svc in svc_names:
+                    if svc.lower() in up:
+                        logging.info(f"{svc} is up in production")
+                    else:
+                        logging.error(f"{svc} is down in production")
+                time.sleep(int(seconds))
+    return target_instance
+
+
 @main.command("check-instance-namespace", short_help="Check if a particular namespace is present")
 @click.argument("instance-name")
 @click.argument("namespace-name")
 def check_instance_namespace(instance_name, namespace_name):
     """ Check if a particular namespace is present in a particular instance """
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
@@ -143,15 +175,15 @@
 def get_labels():
     """Gets a lit of available labels"""
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
     constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
     existing_token = os.getenv("MOTIOCI_TOKEN", '""')
     if (os.getenv("MOTIOCI_TOKEN") == "") or (os.getenv("MOTIOCI_TOKEN") == None):
-        print(f"You need a valid token defined in your environment"
+        print(f"You need a valid token defined in your environment.\n"
                 f"You should try check-env to check your environment."
                 )
         raise SystemExit(1)
     else:
         constants.X_AUTH_TOKEN = os.getenv("MOTIOCI_TOKEN")
     labels_object = labels.get_labels_default()
     if labels_object == 'None':
```

### Comparing `cipromote-1.2.0/src/cipromote/instances.py` & `cipromote-1.3.0/src/cipromote/instances.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/label_versions.py` & `cipromote-1.3.0/src/cipromote/label_versions.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/labels.py` & `cipromote-1.3.0/src/cipromote/labels.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/loginInput.py` & `cipromote-1.3.0/src/cipromote/loginInput.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/projects.py` & `cipromote-1.3.0/src/cipromote/projects.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/queries.py` & `cipromote-1.3.0/src/cipromote/queries.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/src/cipromote/versioned_items.py` & `cipromote-1.3.0/src/cipromote/versioned_items.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.2.0/PKG-INFO` & `cipromote-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipromote
-Version: 1.2.0
+Version: 1.3.0
 Summary: Promote MotionCI Labels
 Author: Michael MacKenna
 Author-email: mmackenna@ufginsurance.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

