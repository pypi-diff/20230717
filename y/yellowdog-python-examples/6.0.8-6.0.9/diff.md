# Comparing `tmp/yellowdog-python-examples-6.0.8.tar.gz` & `tmp/yellowdog-python-examples-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-6.0.8.tar", last modified: Fri Jun 30 07:27:36 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.9.tar", last modified: Mon Jul 10 07:26:46 2023, max compression
```

## Comparing `yellowdog-python-examples-6.0.8.tar` & `yellowdog-python-examples-6.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-30 07:27:36.452457 yellowdog-python-examples-6.0.8/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.8/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-30 07:27:36.452558 yellowdog-python-examples-6.0.8/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.8/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   112934 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.8/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.8/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-30 07:27:36.452869 yellowdog-python-examples-6.0.8/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.8/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-30 07:27:36.451578 yellowdog-python-examples-6.0.8/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-06-28 17:10:43.000000 yellowdog-python-examples-6.0.8/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.8/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    19764 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.8/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.8/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.8/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.8/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.8/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1565 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3303 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     4557 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.8/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7844 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.8/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.8/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.8/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.8/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    41866 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.8/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     7560 2023-06-27 15:17:32.000000 yellowdog-python-examples-6.0.8/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.8/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2545 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.8/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.8/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.8/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.8/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.8/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2980 2023-06-28 21:31:31.000000 yellowdog-python-examples-6.0.8/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-30 07:27:36.452357 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-30 07:27:36.000000 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-30 07:27:36.000000 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-30 07:27:36.000000 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-30 07:27:36.000000 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-30 07:27:36.000000 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-30 07:27:36.000000 yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-07-10 07:26:46.282497 yellowdog-python-examples-6.0.9/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.9/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-07-10 07:26:46.282566 yellowdog-python-examples-6.0.9/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.9/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   112934 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.9/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.9/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.9/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-07-10 07:26:46.282853 yellowdog-python-examples-6.0.9/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.9/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-07-10 07:26:46.281576 yellowdog-python-examples-6.0.9/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3194 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.9/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    19764 2023-06-30 07:26:49.000000 yellowdog-python-examples-6.0.9/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.9/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.9/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17968 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.9/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.9/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1637 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3335 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     4556 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.9/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7950 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.9/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.9/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.9/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    41866 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.9/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     7553 2023-07-10 07:26:03.000000 yellowdog-python-examples-6.0.9/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.9/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2545 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.9/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.9/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.9/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.9/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.9/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2980 2023-06-28 21:31:31.000000 yellowdog-python-examples-6.0.9/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-07-10 07:26:46.282396 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-07-10 07:26:46.000000 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-07-10 07:26:46.000000 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-07-10 07:26:46.000000 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-07-10 07:26:46.000000 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       75 2023-07-10 07:26:46.000000 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-07-10 07:26:46.000000 yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-6.0.8/LICENSE` & `yellowdog-python-examples-6.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/PKG-INFO` & `yellowdog-python-examples-6.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.8
+Version: 6.0.9
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.8/PYPI_README.md` & `yellowdog-python-examples-6.0.9/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/README.md` & `yellowdog-python-examples-6.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/pyproject.toml` & `yellowdog-python-examples-6.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/setup.cfg` & `yellowdog-python-examples-6.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/abort.py` & `yellowdog-python-examples-6.0.9/yd_commands/abort.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,64 +46,63 @@
                 WorkRequirementStatus.FAILED,
             ],
         )
     )
 
     if len(selected_work_requirement_summaries) != 0:
         selected_work_requirement_summaries = select(
-            CLIENT, selected_work_requirement_summaries, override_quiet=True
+            CLIENT,
+            selected_work_requirement_summaries,
+            single_result=True,
+            override_quiet=True,
         )
     else:
         print_log("No matching Work Requirements found")
 
-    if len(selected_work_requirement_summaries) != 0:
-        abort_tasks_selectively(selected_work_requirement_summaries)
+    if len(selected_work_requirement_summaries) == 1:
+        abort_tasks_selectively(selected_work_requirement_summaries[0])
 
 
 def abort_tasks_selectively(
-    selected_work_requirement_summaries: List[WorkRequirementSummary],
+    wr_summary: WorkRequirementSummary,
 ) -> None:
     """
-    Abort selected Tasks in a list of Work Requirements.
+    Abort selected Tasks in a Work Requirements
     """
     aborted_tasks = 0
-    for wr_summary in selected_work_requirement_summaries:
+    print_log(f"Aborting Tasks in Work Requirement '{wr_summary.name}'")
+    task_search = TaskSearch(
+        workRequirementId=wr_summary.id,
+        statuses=[TaskStatus.EXECUTING],
+    )
+    tasks: List[Task] = CLIENT.work_client.find_tasks(task_search)
+    if len(tasks) > 0:
+        tasks = select(
+            CLIENT, sorted_objects(tasks), parent=wr_summary, override_quiet=True
+        )
+    else:
         print_log(
-            f"Aborting Tasks in Work Requirement '{wr_summary.name}'",
+            "No currently executing Tasks in this Work Requirement",
             override_quiet=True,
         )
-        task_search = TaskSearch(
-            workRequirementId=wr_summary.id,
-            statuses=[TaskStatus.EXECUTING],
-        )
-        tasks: List[Task] = CLIENT.work_client.find_tasks(task_search)
-        if len(tasks) > 0:
-            tasks = select(
-                CLIENT, sorted_objects(tasks), parent=wr_summary, override_quiet=True
-            )
-        else:
-            print_log(
-                "No currently running Tasks in this Work Requirement",
-                override_quiet=True,
-            )
-        if len(tasks) != 0 and confirmed(f"Abort {len(tasks)} Tasks?"):
-            for task in tasks:
-                try:
-                    CLIENT.work_client.cancel_task(task, abort=True)
-                    print_log(
-                        f"Aborting Task '{task.name}' in Task Group"
-                        f" '{get_task_group_name(CLIENT, wr_summary, task)}' in Work"
-                        f" Requirement '{wr_summary.name}'"
-                    )
-                    aborted_tasks += 1
-                except Exception as e:
-                    print_error(e)
-                    continue
-        if aborted_tasks == 0:
-            print_log("No Tasks Aborted")
-        else:
-            print_log(f"Aborted {aborted_tasks} Task(s)")
+    if len(tasks) != 0 and confirmed(f"Abort {len(tasks)} Tasks?"):
+        for task in tasks:
+            try:
+                CLIENT.work_client.cancel_task(task, abort=True)
+                print_log(
+                    f"Aborting Task '{task.name}' in Task Group"
+                    f" '{get_task_group_name(CLIENT, wr_summary, task)}' in Work"
+                    f" Requirement '{wr_summary.name}'"
+                )
+                aborted_tasks += 1
+            except Exception as e:
+                print_error(e)
+                continue
+    if aborted_tasks == 0:
+        print_log("No Tasks Aborted")
+    else:
+        print_log(f"Aborted {aborted_tasks} Task(s)")
 
 
 # Entry point
 if __name__ == "__main__":
     main()
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/admin.py` & `yellowdog-python-examples-6.0.9/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/args.py` & `yellowdog-python-examples-6.0.9/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.9/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.9/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.9/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/config.py` & `yellowdog-python-examples-6.0.9/yd_commands/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 YD_NAMESPACE = "YD_NAMESPACE"
 YD_TAG = "YD_TAG"
 YD_URL = "YD_URL"
 
 TASK_BATCH_SIZE_DEFAULT = 2000
 DEFAULT_URL = "https://portal.yellowdog.co/api"
 
+NAMESPACE_SEPARATOR = "::"
+
 
 @dataclass
 class ConfigWorkRequirement:
     args: List[str] = field(default_factory=list)
     capture_taskoutput: bool = True
     completed_task_ttl: Optional[float] = None  # In minutes
     csv_files: Optional[List[str]] = None
@@ -471,7 +473,19 @@
     """
     Update a ConfigWorkRequirement Object with the current dictionary of
     variable substitutions. Returns the updated object.
     """
     config_wr_str_processed = substitute_variable_str(str(config_wr))
     # Note: 'literal_eval' doesn't work here
     return eval(config_wr_str_processed)
+
+
+def unpack_namespace_in_prefix(namespace: str, prefix: str) -> (str, str):
+    """
+    Allow the prefix to include the namespace. Return the unpacked
+    namespace, prefix.
+    """
+    elems = prefix.split(NAMESPACE_SEPARATOR)
+    if len(elems) == 1:
+        return namespace, prefix.lstrip("/")
+    if len(elems) == 2:
+        return elems[0] if elems[0] != "" else namespace, elems[1].lstrip("/")
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.9/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.9/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/delete.py` & `yellowdog-python-examples-6.0.9/yd_commands/delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 A script to delete YellowDog Object Store items.
 """
 
 from typing import List
 
 from yellowdog_client.model import ObjectPath, ObjectPathsRequest
 
+from yd_commands.config import unpack_namespace_in_prefix
 from yd_commands.interactive import confirmed, select
 from yd_commands.printing import print_log
 from yd_commands.wrapper import ARGS_PARSER, CLIENT, CONFIG_COMMON, main_wrapper
 
 
 @main_wrapper
 def main():
-    tag = CONFIG_COMMON.name_tag.lstrip("/")
+    namespace, tag = unpack_namespace_in_prefix(
+        CONFIG_COMMON.namespace, CONFIG_COMMON.name_tag
+    )
     print_log(
-        f"Deleting Object Paths in namespace '{CONFIG_COMMON.namespace}' and "
+        f"Deleting Object Paths in namespace '{namespace}' and "
         f"names starting with '{tag}'"
     )
 
     object_paths_to_delete: List[ObjectPath] = (
         CLIENT.object_store_client.get_namespace_object_paths(
-            ObjectPathsRequest(
-                CONFIG_COMMON.namespace, prefix=tag, flat=ARGS_PARSER.all
-            )
+            ObjectPathsRequest(namespace=namespace, prefix=tag, flat=ARGS_PARSER.all)
         )
     )
 
     if len(object_paths_to_delete) > 0:
         object_paths_to_delete = select(CLIENT, object_paths_to_delete)
 
     if len(object_paths_to_delete) > 0 and confirmed(
         f"Delete {len(object_paths_to_delete)} Object Path(s)?"
     ):
         print_log(f"{len(object_paths_to_delete)} Object Path(s) to Delete")
         CLIENT.object_store_client.delete_objects(
-            CONFIG_COMMON.namespace, object_paths=object_paths_to_delete
+            namespace=namespace, object_paths=object_paths_to_delete
         )
         for object_path in object_paths_to_delete:
             print_log(f"Deleted Object Path: {object_path.displayName}")
         print_log(f"Deleted {len(object_paths_to_delete)} Object Path(s)")
     else:
         print_log("Nothing to delete")
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/download.py` & `yellowdog-python-examples-6.0.9/yd_commands/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 from yellowdog_client.model import ObjectPath, ObjectPathsRequest
 from yellowdog_client.object_store.download.abstracts.abstract_download_batch_builder import (
     AbstractDownloadBatchBuilder,
     AbstractTransferBatch,
 )
 from yellowdog_client.object_store.model import FileTransferStatus
 
+from yd_commands.config import unpack_namespace_in_prefix
 from yd_commands.interactive import confirmed, select
 from yd_commands.printing import print_log
 from yd_commands.wrapper import ARGS_PARSER, CLIENT, CONFIG_COMMON, main_wrapper
 
 
 @main_wrapper
 def main():
-    tag = CONFIG_COMMON.name_tag.lstrip("/")
+    namespace, tag = unpack_namespace_in_prefix(
+        CONFIG_COMMON.namespace, CONFIG_COMMON.name_tag
+    )
     print_log(
-        f"Downloading all Objects in namespace '{CONFIG_COMMON.namespace}' and "
+        f"Downloading all Objects in namespace '{namespace}' and "
         f"names starting with '{tag}'"
     )
 
     object_paths_to_download: List[ObjectPath] = (
         CLIENT.object_store_client.get_namespace_object_paths(
-            ObjectPathsRequest(
-                CONFIG_COMMON.namespace, prefix=tag, flat=ARGS_PARSER.all
-            )
+            ObjectPathsRequest(namespace=namespace, prefix=tag, flat=ARGS_PARSER.all)
         )
     )
 
     if len(object_paths_to_download) > 0:
         object_paths_to_download = select(CLIENT, object_paths_to_download)
 
     if len(object_paths_to_download) == 0:
@@ -45,26 +46,24 @@
 
     if not confirmed(f"Download {len(object_paths_to_download)} Object Path(s)?"):
         return
 
     print_log(f"{len(object_paths_to_download)} Object Path(s) to Download")
 
     download_dir: str = _create_download_directory(
-        CONFIG_COMMON.namespace
-        if ARGS_PARSER.directory == ""
-        else ARGS_PARSER.directory
+        namespace if ARGS_PARSER.directory == "" else ARGS_PARSER.directory
     )
 
     for object_path in object_paths_to_download:
         download_batch_builder: AbstractDownloadBatchBuilder = (
             CLIENT.object_store_client.build_download_batch()
         )
         download_batch_builder.destination_folder = download_dir
         download_batch_builder.find_source_objects(
-            namespace=CONFIG_COMMON.namespace,
+            namespace=namespace,
             object_name_pattern=f"{object_path.name}*",
         )
         download_batch: AbstractTransferBatch = (
             download_batch_builder.get_batch_if_objects_found()
         )
         if download_batch is None:
             print_log(f"No Objects found in Object Path {object_path.displayName}")
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.9/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.9/yd_commands/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,19 +105,19 @@
             continue
         else:
             break
 
     selected_list = sorted(list(selector_set))
     if len(selected_list) > 0:
         if not single_result:
-            if len(selected_list) > 30:
+            if len(selected_list) > 20:
                 display_selections = (
-                    ", ".join([str(x) for x in selected_list[:15]])
+                    ", ".join([str(x) for x in selected_list[:10]])
                     + " ... "
-                    + ", ".join([str(x) for x in selected_list[-15:]])
+                    + ", ".join([str(x) for x in selected_list[-8:]])
                 )
             else:
                 display_selections = ", ".join([str(x) for x in selected_list])
             print(print_string(f"Selected item number(s): {display_selections}"))
     else:
         print_log("No items selected")
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.9/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/list.py` & `yellowdog-python-examples-6.0.9/yd_commands/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     WorkerPoolStatus,
     WorkerPoolSummary,
     WorkRequirementStatus,
     WorkRequirementSummary,
 )
 
 from yd_commands.args import ARGS_PARSER
+from yd_commands.config import unpack_namespace_in_prefix
 from yd_commands.interactive import select
 from yd_commands.object_utilities import (
     get_filtered_work_requirements,
     get_task_groups_from_wr_summary,
 )
 from yd_commands.printing import print_log, print_numbered_object_list, sorted_objects
 from yd_commands.wrapper import CLIENT, CONFIG_COMMON, main_wrapper
@@ -135,25 +136,27 @@
     )
     tasks: List[Task] = CLIENT.work_client.find_tasks(task_search)
     tasks = sorted_objects(tasks)
     print_numbered_object_list(CLIENT, tasks, parent=work_summary)
 
 
 def list_object_paths():
-    tag = CONFIG_COMMON.name_tag.lstrip("/")
+    namespace, tag = unpack_namespace_in_prefix(
+        CONFIG_COMMON.namespace, CONFIG_COMMON.name_tag
+    )
     print_log(
-        f"Listing Object Paths in namespace '{CONFIG_COMMON.namespace}' and "
+        f"Listing Object Paths in namespace '{namespace}' and "
         f"names starting with '{tag}'"
     )
     if ARGS_PARSER.all:
         print_log("Listing all Objects")
     object_paths: List[ObjectPath] = (
         CLIENT.object_store_client.get_namespace_object_paths(
             ObjectPathsRequest(
-                CONFIG_COMMON.namespace,
+                namespace=namespace,
                 prefix=tag,
                 flat=ARGS_PARSER.all,
             )
         )
     )
     print_numbered_object_list(CLIENT, sorted_objects(object_paths))
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.9/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/printing.py` & `yellowdog-python-examples-6.0.9/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/provision.py` & `yellowdog-python-examples-6.0.9/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.9/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.9/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.9/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/submit.py` & `yellowdog-python-examples-6.0.9/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.9/yd_commands/submit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 from dataclasses import dataclass
 from glob import glob
 from typing import List, Optional
 
 from yellowdog_client import PlatformClient
 from yellowdog_client.model import ObjectPath, TaskInput, TaskInputVerification
 
-from yd_commands.config import ConfigCommon
+from yd_commands.config import NAMESPACE_SEPARATOR, ConfigCommon
 from yd_commands.printing import print_error, print_log
 from yd_commands.upload_utils import unique_upload_pathname, upload_file_core
 from yd_commands.wrapper import ARGS_PARSER
 
-NAMESPACE_SEPARATOR = "::"
-
 
 def generate_task_input_list(
     files: List[str],
     verification: Optional[TaskInputVerification],
     wr_name: Optional[str],
 ) -> List[TaskInput]:
     """
```

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.9/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.9/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/upload.py` & `yellowdog-python-examples-6.0.9/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.9/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/validate_properties.py` & `yellowdog-python-examples-6.0.9/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/variables.py` & `yellowdog-python-examples-6.0.9/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/version.py` & `yellowdog-python-examples-6.0.9/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.9/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.8
+Version: 6.0.9
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.8/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.9/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

