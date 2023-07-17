# Comparing `tmp/metget-0.2.5.tar.gz` & `tmp/metget-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.2.5.tar", last modified: Thu Jul 13 19:37:07 2023, max compression
+gzip compressed data, was "metget-0.2.6.tar", last modified: Mon Jul 17 00:53:14 2023, max compression
```

## Comparing `metget-0.2.5.tar` & `metget-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.993081 metget-0.2.5/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.5/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-13 19:37:07.992939 metget-0.2.5/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.5/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-13 18:52:45.000000 metget-0.2.5/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-13 19:37:07.993121 metget-0.2.5/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.987687 metget-0.2.5/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.989073 metget-0.2.5/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.991542 metget-0.2.5/src/metget_client/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-13 18:52:45.000000 metget-0.2.5/src/metget_client/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    19413 2023-07-11 21:17:13.000000 metget-0.2.5/src/metget_client/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)    10010 2023-07-11 21:30:40.000000 metget-0.2.5/src/metget_client/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    17369 2023-07-13 18:47:43.000000 metget-0.2.5/src/metget_client/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3981 2023-07-13 18:48:29.000000 metget-0.2.5/src/metget_client/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/spinnerlogger.py
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.992683 metget-0.2.5/test/
--rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.5/test/test_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.5/test/test_cli.py
--rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.5/test/test_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     8688 2023-07-13 18:49:26.000000 metget-0.2.5/test/test_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2560 2023-07-13 18:49:26.000000 metget-0.2.5/test/test_track.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-17 00:53:14.886122 metget-0.2.6/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.6/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-17 00:53:14.885891 metget-0.2.6/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.6/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-17 00:52:18.000000 metget-0.2.6/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-17 00:53:14.886179 metget-0.2.6/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-17 00:53:14.874703 metget-0.2.6/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-17 00:53:14.876433 metget-0.2.6/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-17 00:53:14.000000 metget-0.2.6/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-17 00:53:14.000000 metget-0.2.6/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-17 00:53:14.000000 metget-0.2.6/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-17 00:53:14.000000 metget-0.2.6/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-17 00:53:14.000000 metget-0.2.6/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-17 00:53:14.000000 metget-0.2.6/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-17 00:53:14.879372 metget-0.2.6/src/metget_client/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-17 00:52:18.000000 metget-0.2.6/src/metget_client/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    19413 2023-07-11 21:17:13.000000 metget-0.2.6/src/metget_client/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10010 2023-07-11 21:30:40.000000 metget-0.2.6/src/metget_client/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.6/src/metget_client/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.6/src/metget_client/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.6/src/metget_client/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    19139 2023-07-17 00:41:29.000000 metget-0.2.6/src/metget_client/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3981 2023-07-13 18:48:29.000000 metget-0.2.6/src/metget_client/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.6/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-17 00:53:14.885502 metget-0.2.6/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.6/test/test_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.6/test/test_cli.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.6/test/test_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     8688 2023-07-13 18:49:26.000000 metget-0.2.6/test/test_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2560 2023-07-13 18:49:26.000000 metget-0.2.6/test/test_track.py
```

### Comparing `metget-0.2.5/LICENSE.md` & `metget-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/PKG-INFO` & `metget-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.5
+Version: 0.2.6
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.2.5/README.md` & `metget-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/pyproject.toml` & `metget-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.2.5"
+version = "0.2.6"
 description = "A client package for interaction with a MetGet server instance"
 authors = [
     { name = "Zach Cobell", email = "zcobell@thewaterinstitute.org" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.8"
@@ -40,15 +40,15 @@
 [tool.setuptools.dynamic]
 version = { attr = "metget_client.__version__" }
 
 [project.scripts]
 metget = "metget_client:metget_client_cli"
 
 [tool.bumpver]
-current_version = "0.2.5"
+current_version = "0.2.6"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.2.5/src/metget.egg-info/PKG-INFO` & `metget-0.2.6/src/metget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.5
+Version: 0.2.6
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.2.5/src/metget.egg-info/SOURCES.txt` & `metget-0.2.6/src/metget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/metget_build.py` & `metget-0.2.6/src/metget_client/metget_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/metget_client.py` & `metget-0.2.6/src/metget_client/metget_client.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/metget_credits.py` & `metget-0.2.6/src/metget_client/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/metget_data.py` & `metget-0.2.6/src/metget_client/metget_data.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/metget_environment.py` & `metget-0.2.6/src/metget_client/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/metget_status.py` & `metget-0.2.6/src/metget_client/metget_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -238,30 +238,51 @@
                         "Last Forecast Cycle",
                         "Earliest Forecast Time",
                         "Latest Forecast Time",
                         "Cycle Count",
                         "Ensemble Members",
                     ]
                 )
+                table.align["Ensemble Members"] = "l"
 
-                for storm in data.keys():
-                    ensemble_members = []
-                    for ensemble_member in data[storm].keys():
-                        ensemble_members.append(ensemble_member)
-                    table.add_row(
-                        [
-                            storm,
-                            data[storm][ensemble_members[0]]["first_available_cycle"],
-                            data[storm][ensemble_members[0]]["latest_available_cycle"],
-                            data[storm][ensemble_members[0]]["min_forecast_date"],
-                            data[storm][ensemble_members[0]]["max_forecast_date"],
-                            len(data[storm][ensemble_members[0]]["cycles"]),
-                            ensemble_members,
-                        ]
-                    )
+                for year in data.keys():
+                    for storm in data[year].keys():
+                        ensemble_members = []
+
+                        break_counter = 0
+                        ensemble_members_str = ""
+                        for ensemble_member in data[year][storm].keys():
+                            ensemble_members.append(ensemble_member)
+                            if break_counter == 0:
+                                ensemble_members_str += "{:s}".format(ensemble_member)
+                            else:
+                                ensemble_members_str += ", {:s}".format(ensemble_member)
+                            break_counter += 1
+                            if break_counter == 5:
+                                ensemble_members_str += "\n"
+                                break_counter = 0
+                        table.add_row(
+                            [
+                                storm,
+                                data[year][storm][ensemble_members[0]][
+                                    "first_available_cycle"
+                                ],
+                                data[year][storm][ensemble_members[0]][
+                                    "latest_available_cycle"
+                                ],
+                                data[year][storm][ensemble_members[0]][
+                                    "min_forecast_date"
+                                ],
+                                data[year][storm][ensemble_members[0]][
+                                    "max_forecast_date"
+                                ],
+                                len(data[year][storm][ensemble_members[0]]["cycles"]),
+                                ensemble_members_str,
+                            ]
+                        )
                 print(table)
 
     def __status_ensemble(self, model: str) -> None:
         """
         This method is used to get the status of the ensemble data
 
         Args:
@@ -387,33 +408,45 @@
                             "Cycle Count",
                         ]
                     )
                     table.align["Storm"] = "r"
                 else:
                     raise ValueError("Unknown data type: {:s}".format(data_type))
 
-                for it in data.keys():
-                    table.add_row(
-                        [
-                            it,
-                            data[it]["first_available_cycle"],
-                            data[it]["latest_available_cycle"],
-                            data[it]["min_forecast_date"],
-                            data[it]["max_forecast_date"],
-                            len(data[it]["cycles"]),
-                        ]
-                    )
-                table.align["Cycle Count"] = "r"
-
                 if data_type == "ensemble":
+                    for it in data.keys():
+                        table.add_row(
+                            [
+                                it,
+                                data[it]["first_available_cycle"],
+                                data[it]["latest_available_cycle"],
+                                data[it]["min_forecast_date"],
+                                data[it]["max_forecast_date"],
+                                len(data[it]["cycles"]),
+                            ]
+                        )
+                    table.align["Cycle Count"] = "r"
                     print(
                         "Status for {:s} Model Ensemble Members".format(model.upper())
                     )
                     print(table.get_string(sortby="Ensemble Member"))
-                elif data_type == "storm":
+                else:
+                    for year in data.keys():
+                        for it in data[year].keys():
+                            table.add_row(
+                                [
+                                    it,
+                                    data[year][it]["first_available_cycle"],
+                                    data[year][it]["latest_available_cycle"],
+                                    data[year][it]["min_forecast_date"],
+                                    data[year][it]["max_forecast_date"],
+                                    len(data[year][it]["cycles"]),
+                                ]
+                            )
+                    table.align["Cycle Count"] = "r"
                     table.reversesort = True
                     print(
                         "Status for {:s} Model Storms (class: {:s})".format(
                             model.upper(), self.__model_class
                         )
                     )
                     print(table.get_string(sortby="First Forecast Cycle"))
```

### Comparing `metget-0.2.5/src/metget_client/metget_track.py` & `metget-0.2.6/src/metget_client/metget_track.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/src/metget_client/spinnerlogger.py` & `metget-0.2.6/src/metget_client/spinnerlogger.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/test/test_build.py` & `metget-0.2.6/test/test_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/test/test_credits.py` & `metget-0.2.6/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/test/test_status.py` & `metget-0.2.6/test/test_status.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.5/test/test_track.py` & `metget-0.2.6/test/test_track.py`

 * *Files identical despite different names*

