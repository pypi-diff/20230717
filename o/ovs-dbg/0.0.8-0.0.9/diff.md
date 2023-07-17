# Comparing `tmp/ovs_dbg-0.0.8.tar.gz` & `tmp/ovs_dbg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ovs-dbg/ovs-dbg/dist/tmpl5qc_ly3/ovs_dbg-0.0.8.tar", last modified: Fri Sep 10 14:09:39 2021, max compression
+gzip compressed data, was "/home/runner/work/ovs-dbg/ovs-dbg/dist/tmp1f_na1hx/ovs_dbg-0.0.9.tar", last modified: Wed Sep 15 10:25:54 2021, max compression
```

## Comparing `ovs_dbg-0.0.8.tar` & `ovs_dbg-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      101 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/bin/ofparse
--rwxr-xr-x   0 runner    (1001) docker     (121)     4467 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/bin/ovs-lgrep
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      817 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg/
--rw-r--r--   0 runner    (1001) docker     (121)     8671 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/kv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5935 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofp_act.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5738 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    24564 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/odp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 14:09:39.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/
--rw-r--r--   0 runner    (1001) docker     (121)    13252 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/dp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/ofparse.conf
--rw-r--r--   0 runner    (1001) docker     (121)     4028 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/console.py
--rw-r--r--   0 runner    (1001) docker     (121)    10218 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     6546 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/ofp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/process.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofparse/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3650 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/list.py
--rw-r--r--   0 runner    (1001) docker     (121)    11845 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/ofp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7362 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    11804 2021-09-10 14:09:29.000000 ovs_dbg-0.0.8/ovs_dbg/decoders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      101 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/bin/ofparse
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4467 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/bin/ovs-lgrep
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg/
+-rw-r--r--   0 runner    (1001) docker     (121)     8671 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/kv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5935 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofp_act.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5738 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24564 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/odp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-15 10:25:54.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/
+-rw-r--r--   0 runner    (1001) docker     (121)    13252 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/dp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/ofparse.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     4028 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/console.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10218 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6559 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/ofp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/process.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3638 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofparse/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3650 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11845 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/ofp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2595 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7362 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11804 2021-09-15 10:25:39.000000 ovs_dbg-0.0.9/ovs_dbg/decoders.py
```

### Comparing `ovs_dbg-0.0.8/bin/ovs-lgrep` & `ovs_dbg-0.0.9/bin/ovs-lgrep`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg.egg-info/SOURCES.txt` & `ovs_dbg-0.0.9/ovs_dbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg.egg-info/PKG-INFO` & `ovs_dbg-0.0.9/ovs_dbg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovs-dbg
-Version: 0.0.8
+Version: 0.0.9
 Summary: OVS Debug contains scripts and libraries that help debug OVS and OVN
 Home-page: https://ovs-dbg.readthedocs.io/en/latest/
 Author: Adrián Moreno
 Author-email: amorenoz@redhat.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/amorenoz/ovs-dbg
 Keywords: ovs_dbg
```

### Comparing `ovs_dbg-0.0.8/PKG-INFO` & `ovs_dbg-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovs_dbg
-Version: 0.0.8
+Version: 0.0.9
 Summary: OVS Debug contains scripts and libraries that help debug OVS and OVN
 Home-page: https://ovs-dbg.readthedocs.io/en/latest/
 Author: Adrián Moreno
 Author-email: amorenoz@redhat.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/amorenoz/ovs-dbg
 Keywords: ovs_dbg
```

### Comparing `ovs_dbg-0.0.8/setup.py` & `ovs_dbg-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     data_files=["ovs_dbg/ofparse/ofparse.conf"],
     test_suite="tests",
     tests_require=test_requirements,
     url="https://ovs-dbg.readthedocs.io/en/latest/",
     project_urls={
         "Source": "https://github.com/amorenoz/ovs-dbg",
     },
-    version="0.0.8",
+    version="0.0.9",
     zip_safe=False,
 )
```

### Comparing `ovs_dbg-0.0.8/LICENSE` & `ovs_dbg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/README.md` & `ovs_dbg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/kv.py` & `ovs_dbg-0.0.9/ovs_dbg/kv.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofp_act.py` & `ovs_dbg-0.0.9/ovs_dbg/ofp_act.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/logs.py` & `ovs_dbg-0.0.9/ovs_dbg/logs.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/filter.py` & `ovs_dbg-0.0.9/ovs_dbg/filter.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/odp.py` & `ovs_dbg-0.0.9/ovs_dbg/odp.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/dp.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/dp.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/ofparse.conf` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/ofparse.conf`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/html.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/html.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/console.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/console.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/format.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/format.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/ofp.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/ofp.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
                 for flow in flows:
                     buf = ConsoleBuffer(Text())
                     highlighted = None
                     if opts.get("highlight"):
                         result = opts.get("highlight").evaluate(flow)
                         if result:
                             highlighted = result.kv
-                    ConsoleFormatter(console, opts).format_flow(buf, flow, highlighted)
+                    ConsoleFormatter(opts=opts, console=console).format_flow(buf, flow, highlighted)
                     lflow_tree.add(buf.text)
 
     with print_context(console, opts):
         console.print(tree)
 
 
 @openflow.command()
```

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/process.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Defines common flow processing functionality
 """
 import sys
 import json
-import rich
 
 from ovs_dbg.ofp import OFPFlow
 from ovs_dbg.decoders import FlowEncoder
 from ovs_dbg.ofparse.console import ConsoleFormatter, print_context
 
 
 def process_flows(flow_factory, callback, filename="", filter=None):
@@ -56,20 +55,15 @@
 
     flow_json = json.dumps(
         [flow.dict() for flow in flows],
         indent=4,
         cls=FlowEncoder,
     )
 
-    if opts["paged"]:
-        console = rich.Console()
-        with print_context(console, opts):
-            console.print(flow_json)
-    else:
-        print(flow_json)
+    print(flow_json)
 
 
 def pprint(flow_factory, opts):
     """
     Pretty print the flows
 
     Args:
```

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofparse/main.py` & `ovs_dbg-0.0.9/ovs_dbg/ofparse/main.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/list.py` & `ovs_dbg-0.0.9/ovs_dbg/list.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/ofp.py` & `ovs_dbg-0.0.9/ovs_dbg/ofp.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/flow.py` & `ovs_dbg-0.0.9/ovs_dbg/flow.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/fields.py` & `ovs_dbg-0.0.9/ovs_dbg/fields.py`

 * *Files identical despite different names*

### Comparing `ovs_dbg-0.0.8/ovs_dbg/decoders.py` & `ovs_dbg-0.0.9/ovs_dbg/decoders.py`

 * *Files identical despite different names*

