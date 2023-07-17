# Comparing `tmp/mycluster-2.0.5.tar.gz` & `tmp/mycluster-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycluster-2.0.5.tar", last modified: Fri Jul 14 11:37:06 2023, max compression
+gzip compressed data, was "mycluster-2.0.6.tar", last modified: Mon Jul 17 10:50:58 2023, max compression
```

## Comparing `mycluster-2.0.5.tar` & `mycluster-2.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-14 11:36:57.000000 mycluster-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 11:36:57.000000 mycluster-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-14 11:37:06.745287 mycluster-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-14 11:36:57.000000 mycluster-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.741287 mycluster-2.0.5/mycluster/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/mycluster/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/mycluster/schedulers/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/lsf.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/pbs.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/sge.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/slurm.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.741287 mycluster-2.0.5/mycluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 11:36:57.000000 mycluster-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-14 11:37:06.745287 mycluster-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-14 11:36:57.000000 mycluster-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/share/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-OF-simpleFoam.bsh
--rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-fluent.bsh
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-paraview.bsh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-zcfd.bsh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:58.322708 mycluster-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-17 10:50:47.000000 mycluster-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 10:50:47.000000 mycluster-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-17 10:50:58.322708 mycluster-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-17 10:50:47.000000 mycluster-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:58.318708 mycluster-2.0.6/mycluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:58.318708 mycluster-2.0.6/mycluster/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:58.318708 mycluster-2.0.6/mycluster/schedulers/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/templates/lsf.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/templates/pbs.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/templates/sge.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-17 10:50:47.000000 mycluster-2.0.6/mycluster/schedulers/templates/slurm.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:58.318708 mycluster-2.0.6/mycluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-17 10:50:58.000000 mycluster-2.0.6/mycluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-17 10:50:58.000000 mycluster-2.0.6/mycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:50:58.000000 mycluster-2.0.6/mycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 10:50:58.000000 mycluster-2.0.6/mycluster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 10:50:58.000000 mycluster-2.0.6/mycluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 10:50:58.000000 mycluster-2.0.6/mycluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 10:50:47.000000 mycluster-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-17 10:50:58.322708 mycluster-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 10:50:47.000000 mycluster-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:58.322708 mycluster-2.0.6/share/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-17 10:50:47.000000 mycluster-2.0.6/share/mycluster-OF-simpleFoam.bsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-07-17 10:50:47.000000 mycluster-2.0.6/share/mycluster-fluent.bsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-07-17 10:50:47.000000 mycluster-2.0.6/share/mycluster-paraview.bsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-07-17 10:50:47.000000 mycluster-2.0.6/share/mycluster-zcfd.bsh
```

### Comparing `mycluster-2.0.5/LICENSE` & `mycluster-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/PKG-INFO` & `mycluster-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycluster
-Version: 2.0.5
+Version: 2.0.6
 Summary: "Utilities to support interacting with multiple HPC clusters"
 Home-page: https://github.com/zenotech/MyCluster
 Author: "Zenotech Ltd"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mycluster-2.0.5/README.md` & `mycluster-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/__init__.py` & `mycluster-2.0.6/mycluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/cli.py` & `mycluster-2.0.6/mycluster/cli.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/exceptions.py` & `mycluster-2.0.6/mycluster/exceptions.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/__init__.py` & `mycluster-2.0.6/mycluster/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/base.py` & `mycluster-2.0.6/mycluster/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/lsf.py` & `mycluster-2.0.6/mycluster/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/pbs.py` & `mycluster-2.0.6/mycluster/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/sge.py` & `mycluster-2.0.6/mycluster/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/slurm.py` & `mycluster-2.0.6/mycluster/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/templates/lsf.jinja` & `mycluster-2.0.6/mycluster/schedulers/templates/lsf.jinja`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/templates/pbs.jinja` & `mycluster-2.0.6/mycluster/schedulers/templates/pbs.jinja`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/templates/sge.jinja` & `mycluster-2.0.6/mycluster/schedulers/templates/sge.jinja`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/mycluster/schedulers/templates/slurm.jinja` & `mycluster-2.0.6/mycluster/schedulers/templates/slurm.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 # Number of nodes
 #SBATCH --nodes {{num_nodes}}
 # Number of tasks
 #SBATCH --ntasks {{num_tasks}}
 {% if exclusive %}
 # Exclusive node use
 #SBATCH --exclusive
+{% else %}
+#SBATCH --cpus-per-task={{num_threads_per_task}}
 {% endif %}
 # Do not requeue job on node failure
 #SBATCH --no-requeue
 # High performance cpu governor
 #SBATCH --cpu-freq=Performance
 # How much wallclock time will be required?
 #SBATCH --time={{wall_clock}}
```

### Comparing `mycluster-2.0.5/mycluster.egg-info/PKG-INFO` & `mycluster-2.0.6/mycluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycluster
-Version: 2.0.5
+Version: 2.0.6
 Summary: "Utilities to support interacting with multiple HPC clusters"
 Home-page: https://github.com/zenotech/MyCluster
 Author: "Zenotech Ltd"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mycluster-2.0.5/mycluster.egg-info/SOURCES.txt` & `mycluster-2.0.6/mycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/setup.cfg` & `mycluster-2.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.5/share/mycluster-zcfd.bsh` & `mycluster-2.0.6/share/mycluster-zcfd.bsh`

 * *Files identical despite different names*

