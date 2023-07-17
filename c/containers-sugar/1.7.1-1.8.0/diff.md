# Comparing `tmp/containers_sugar-1.7.1.tar.gz` & `tmp/containers_sugar-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "containers_sugar-1.7.1.tar", max compression
+gzip compressed data, was "containers_sugar-1.8.0.tar", max compression
```

## Comparing `containers_sugar-1.7.1.tar` & `containers_sugar-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      965 2023-06-15 12:02:14.847470 containers_sugar-1.7.1/.containers-sugar.yaml
--rw-r--r--   0        0        0       88 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      327 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1395 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1704 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1889 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1799 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.gitignore
--rw-r--r--   0        0        0     1422 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1887 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/.releaserc.json
--rw-r--r--   0        0        0     1514 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/LICENSE
--rw-r--r--   0        0        0     4393 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/Makefile
--rw-r--r--   0        0        0     3474 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/README.md
--rw-r--r--   0        0        0      197 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/conda/dev.yaml
--rw-r--r--   0        0        0      216 2023-06-15 12:05:27.120888 containers_sugar-1.7.1/containers_sugar/__init__.py
--rw-r--r--   0        0        0      135 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/containers_sugar/__main__.py
--rw-r--r--   0        0        0     4451 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/containers_sugar/cli.py
--rw-r--r--   0        0        0     1084 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/containers_sugar/logs.py
--rw-r--r--   0        0        0    16854 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/containers_sugar/sugar.py
--rw-r--r--   0        0        0     7468 2023-06-15 12:05:27.136887 containers_sugar-1.7.1/docs/changelog.md
--rw-r--r--   0        0        0     5038 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/contributing.md
--rw-r--r--   0        0        0      956 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/images/logo.png
--rw-r--r--   0        0        0      352 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/index.md
--rw-r--r--   0        0        0     1000 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/installation.md
--rw-r--r--   0        0        0     3908 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/docs/mkdocs.yaml
--rw-r--r--   0        0        0   149270 2023-06-15 12:02:14.851470 containers_sugar-1.7.1/poetry.lock
--rw-r--r--   0        0        0     1963 2023-06-15 12:05:27.124888 containers_sugar-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 containers_sugar-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1247 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.containers-sugar.yaml
+-rw-r--r--   0        0        0       88 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      327 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1395 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1786 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1889 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1799 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1422 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1887 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/.releaserc.json
+-rw-r--r--   0        0        0     1514 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/LICENSE
+-rw-r--r--   0        0        0     5479 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/Makefile
+-rw-r--r--   0        0        0     3483 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/README.md
+-rw-r--r--   0        0        0      197 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/conda/dev.yaml
+-rw-r--r--   0        0        0      216 2023-07-17 19:14:01.794067 containers_sugar-1.8.0/containers_sugar/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/containers_sugar/__main__.py
+-rw-r--r--   0        0        0     4452 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/containers_sugar/cli.py
+-rw-r--r--   0        0        0     1084 2023-07-17 19:10:16.928179 containers_sugar-1.8.0/containers_sugar/logs.py
+-rw-r--r--   0        0        0    17574 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/containers_sugar/sugar.py
+-rw-r--r--   0        0        0     7799 2023-07-17 19:14:01.810067 containers_sugar-1.8.0/docs/changelog.md
+-rw-r--r--   0        0        0     5038 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/contributing.md
+-rw-r--r--   0        0        0      956 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/images/logo.png
+-rw-r--r--   0        0        0      352 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/index.md
+-rw-r--r--   0        0        0     1000 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/installation.md
+-rw-r--r--   0        0        0     3908 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/docs/mkdocs.yaml
+-rw-r--r--   0        0        0   149270 2023-07-17 19:10:16.932179 containers_sugar-1.8.0/poetry.lock
+-rw-r--r--   0        0        0     1963 2023-07-17 19:14:01.798067 containers_sugar-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 containers_sugar-1.8.0/PKG-INFO
```

### Comparing `containers_sugar-1.7.1/.containers-sugar.yaml` & `containers_sugar-1.8.0/.containers-sugar.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 version: 1.0
 compose-app: docker-compose
 env-file: .env
 defaults:
   group: {{ env.KXGR_GROUP }}
+  project-name: sugar-{{ env.KXGR_PROJECT_NAME }}
 service-groups:
   - name: group1
     project-name: project1  # optional
     compose-path: tests/containers/group1/compose.yaml
     env-file: .env
     services:
       default: service1-1,service1-3
@@ -34,7 +35,17 @@
     services:
       default: null
       available:
         - name: service1-1
         - name: service1-2
         - name: service2-1
         - name: service2-2
+
+  - name: group-defaults
+    compose-path:
+      - tests/containers/group1/compose.yaml
+    env-file: .env
+    services:
+      # default: service1-1,service1-2
+      available:
+        - name: service1-1
+        - name: service1-2
```

### Comparing `containers_sugar-1.7.1/.github/PULL_REQUEST_TEMPLATE.md` & `containers_sugar-1.8.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/.github/workflows/main.yaml` & `containers_sugar-1.8.0/.github/workflows/main.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
       matrix:
         python_version: ["3.8.1", "3.9", "3.10"]
 
     concurrency:
       group: ci-tests-${{ matrix.python_version }}-${{ github.ref }}
       cancel-in-progress: true
 
+    env:
+      KXGR_PROJECT_NAME: ${{ matrix.python_version }}-${{ github.ref }}
+
     steps:
     - uses: actions/checkout@v3
 
     - name: Prepare conda environment
       run: |
         sed -i s/python\ 3\.8\.1/python\ ${{ matrix.python_version }}/ conda/dev.yaml
         cat conda/dev.yaml
```

### Comparing `containers_sugar-1.7.1/.github/workflows/release.yaml` & `containers_sugar-1.8.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/.gitignore` & `containers_sugar-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/.pre-commit-config.yaml` & `containers_sugar-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/.releaserc.json` & `containers_sugar-1.8.0/.releaserc.json`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/LICENSE` & `containers_sugar-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/README.md` & `containers_sugar-1.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 * up
 * version
 
 These commands are available in the main profile/plugin, so
 you don't need to specify any extra parameter to access them.
 
 For extra commands, we are gathering them into a profile/plugin called
-`ext`, so you can access them using something like: `kxgr ext restart`.
+`ext`, so you can access them using something like: `sugar ext restart`.
 
 The current available **ext** commands are:
 
 * start -> alias for `up`
 * restart -> runs `stop` and `up`
 
 
@@ -96,36 +96,36 @@
     services:
       # default: null
       available:
         - name: service1
         - name: service1
 ```
 
-**NOTE**: containers-sugar has an convenient alias `kxgr` that helps to
+**NOTE**: containers-sugar has an convenient alias `sugar` that helps to
 keep the command line shorter, where **k** stands for *containers*,
 **x** stands for *su* (*shu* sound), and **gr** stands for *gar*.
-In another words, you can use `containers-sugar` or `kxgr` CLI.
+In another words, you can use `containers-sugar` or `sugar` CLI.
 
 Some examples of how to use it:
 
 * build the defaults services (service1,service3) for group1:
-  `kxgr build --group group1`
+  `sugar build --group group1`
 
 * build the all services (there is no default service defined) for group2:
-  `kxgr build --group group2`
+  `sugar build --group group2`
 
 * build all services (ignore default) for group1:
-  `kxgr build --group group1 --all`
+  `sugar build --group group1 --all`
 
 * start the default services for group1:
-  `kxgr ext start --group group1`
+  `sugar ext start --group group1`
 
 * restart all services (ignore defaults) for group1:
-  `kxgr ext restart --group group1 --all`
+  `sugar ext restart --group group1 --all`
 
 * restart service1 and service2 for group1:
-  `kxgr ext restart --group group1 --services service1,service2`
+  `sugar ext restart --group group1 --services service1,service2`
 
 
 **NOTE**: If you use: ```default: group: {{ env.ENV }}```, you don't need to
 give `--group <GROUP_NAME>`, except if you want a different group than the
 default one.
```

### Comparing `containers_sugar-1.7.1/containers_sugar/cli.py` & `containers_sugar-1.8.0/containers_sugar/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_args():
     """Define and return the arguments used by the CLI."""
     parser = argparse.ArgumentParser(
         prog='containers-sugar',
         description=(
-            'containers-sugar (or kxgr) is a tool that help you to organize'
+            'containers-sugar (or sugar) is a tool that help you to organize'
             "and simplify your containers' stack."
         ),
         epilog=(
             'If you have any problem, open an issue at: '
             'https://github.com/osl-incubator/containers-sugar'
         ),
     )
```

### Comparing `containers_sugar-1.7.1/containers_sugar/logs.py` & `containers_sugar-1.8.0/containers_sugar/logs.py`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/containers_sugar/sugar.py` & `containers_sugar-1.8.0/containers_sugar/sugar.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,16 +132,29 @@
                     "group configuration weren't defined.",
                     KxgrErrorType.KXGR_INVALID_PARAMETER,
                 )
             group_name = default_group
         else:
             group_name = self.args.get('service_group')
 
+        default_project_name = self.defaults.get('project-name')
+
         for g in groups:
             if g['name'] == group_name:
+                if default_project_name and 'project-name' not in g:
+                    # just use default value if "project-name" is not set
+                    g['project-name'] = default_project_name
+                if not g.get('services', {}).get('default'):
+                    # if default is not given or it is empty or null,
+                    # use as default all the services available
+                    default_services = [
+                        service['name']
+                        for service in g.get('services', {}).get('available')
+                    ]
+                    g['services']['default'] = ','.join(default_services)
                 self.service_group = g
                 return
 
         KxgrLogs.raise_error(
             f'The given group service "{group_name}" was not found '
             'in the configuration file.',
             KxgrErrorType.KXGR_MISSING_PARAMETER,
```

### Comparing `containers_sugar-1.7.1/docs/changelog.md` & `containers_sugar-1.8.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Release Notes
 ---
 
+# [1.8.0](https://github.com/osl-incubator/containers-sugar/compare/1.7.1...1.8.0) (2023-07-17)
+
+
+### Features
+
+* Add default config for project-name ([#82](https://github.com/osl-incubator/containers-sugar/issues/82)) ([1dab380](https://github.com/osl-incubator/containers-sugar/commit/1dab3802439695396d94e3e1cfce3aeff686e6c6))
+
 ## [1.7.1](https://github.com/osl-incubator/containers-sugar/compare/1.7.0...1.7.1) (2023-06-15)
 
 
 ### Bug Fixes
 
 * **linter:** Refactor linter options and fixes issues pointed by linter tools and add new alias to the app ([#81](https://github.com/osl-incubator/containers-sugar/issues/81)) ([b6e13df](https://github.com/osl-incubator/containers-sugar/commit/b6e13dfa2f72e97cc22ea49ec512f8e8f00c5c70))
```

### Comparing `containers_sugar-1.7.1/docs/contributing.md` & `containers_sugar-1.8.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/docs/example.ipynb` & `containers_sugar-1.8.0/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/docs/images/favicon.ico` & `containers_sugar-1.8.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/docs/images/logo.png` & `containers_sugar-1.8.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/docs/installation.md` & `containers_sugar-1.8.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/docs/mkdocs.yaml` & `containers_sugar-1.8.0/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/poetry.lock` & `containers_sugar-1.8.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.7.1/pyproject.toml` & `containers_sugar-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "containers-sugar"
-version = "1.7.1"  # semantic-release
+version = "1.8.0"  # semantic-release
 description = "Simplify the usage of containers"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 include = [
   "*.cfg",
   "*.ini",
   "*.js",
```

### Comparing `containers_sugar-1.7.1/PKG-INFO` & `containers_sugar-1.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: containers-sugar
-Version: 1.7.1
+Version: 1.8.0
 Summary: Simplify the usage of containers
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

