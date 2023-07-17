# Comparing `tmp/devpm-1.0.1.tar.gz` & `tmp/devpm-1.0.2.tar.gz`

## Comparing `devpm-1.0.1.tar` & `devpm-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 devpm-1.0.1/devpackage.schema.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/cli/base_command.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/cli/main.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/commands/__init__.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/commands/install.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/bash.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/code.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/context.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/git.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/log.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/pip.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.0.1/LICENSE
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 devpm-1.0.1/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 devpm-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 devpm-1.0.2/devpackage.schema.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/cli/base_command.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/cli/main.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/commands/install.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/bash.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/code.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/context.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/git.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/log.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 devpm-1.0.2/devpm/_internal/utils/pip.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 devpm-1.0.2/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 devpm-1.0.2/PKG-INFO
```

### Comparing `devpm-1.0.1/devpackage.schema.json` & `devpm-1.0.2/devpackage.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9204058159722223%*

 * *Differences: {"'definitions'": '{\'osDependency\': {\'description\': "Packages installed by custom bash script. '*

 * *                  'Key for excutable name after installed, value is an object describes script in '*

 * *                  "platforms. The platform is from python `sys.platform`, include 'darwin', "*

 * *                  '\'win32\' and \'linux\'.", \'patternProperties\': {\'.+\': {\'properties\': '*

 * *                  "{'win32': {'description': 'The dependency in win32, specified with a bash "*

 * *                  "script […]*

```diff
@@ -1,19 +1,12 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "definitions": {
-        "dependency": {
-            "additionalProperties": {
-                "type": "string"
-            },
-            "description": "Dependencies are specified with a simple hash of package name to version range. The version range is a string which has one or more space-separated descriptors. Dependencies can also be identified with a tarball or git URL.",
-            "type": "object"
-        },
         "gitHook": {
-            "description": "The git hooks, support commit-msg, pre-commit",
+            "description": "Write to git hooks for root project and it's git submodules. Support commit-msg, pre-commit",
             "properties": {
                 "commit-msg": {
                     "description": "The commit-msg git hook.",
                     "properties": {
                         "pattern": {
                             "description": "The pattern for type regexp",
                             "type": "string"
@@ -53,29 +46,29 @@
                     },
                     "type": "object"
                 }
             },
             "type": "object"
         },
         "osDependency": {
-            "description": "Used to specify dependency in different os.",
+            "description": "Packages installed by custom bash script. Key for excutable name after installed, value is an object describes script in platforms. The platform is from python `sys.platform`, include 'darwin', 'win32' and 'linux'.",
             "patternProperties": {
                 ".+": {
                     "additionalProperties": false,
                     "properties": {
                         "darwin": {
-                            "description": "The dependency in darwin, specified with a simple hash of package name to version range. The version range is a string which has one or more space-separated descriptors. Dependencies can also be identified with a tarball or git URL.",
+                            "description": "The dependency in darwin, specified with a bash script or file URL.",
                             "type": "string"
                         },
                         "linux": {
-                            "description": "The dependency in linux, specified with a simple hash of package name to version range. The version range is a string which has one or more space-separated descriptors. Dependencies can also be identified with a tarball or git URL.",
+                            "description": "The dependency in linux, specified with a bash script or file URL.",
                             "type": "string"
                         },
                         "win32": {
-                            "description": "The dependency in win32, specified with a simple hash of package name to version range. The version range is a string which has one or more space-separated descriptors. Dependencies can also be identified with a tarball or git URL.",
+                            "description": "The dependency in win32, specified with a bash script or file URL.",
                             "type": "string"
                         }
                     },
                     "type": "object"
                 }
             },
             "type": "object"
@@ -106,32 +99,49 @@
                 "rev": {
                     "description": "The revision of the repo, see https://pre-commit.com/hooks.html",
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "vscodeUserSettingsItem": {
-            "properties": {},
+        "pythonDependency": {
+            "additionalProperties": {
+                "type": "string"
+            },
+            "description": "Packages installed by pip. Key for pip name, value for version. Version definitions: ''(empty) - install when not exists; 'latest' - uninstall and install latest, '1.0.0'(specified) - install when version mismatched.",
+            "type": "object"
+        },
+        "vscodeDependency": {
+            "additionalProperties": {
+                "type": "string"
+            },
+            "description": "Packages installed by visutal studio code. Key for vscode extension id, value for version. Version definitions: ''(empty) - install when not exists; 'latest' - uninstall and install latest, '1.0.0'(specified) - install when version mismatched.",
+            "type": "object"
+        },
+        "vscodeSettings": {
+            "additionalProperties": {
+                "type": "string"
+            },
+            "description": "Write to visual studio code user settings <https://code.visualstudio.com/docs/getstarted/settings#_settings-file-locations>. Key and value format same to the user settings. In addition, the value support `devpm expression`: `$bash.which:[bin]` - returns the bin path in system by `which [bin]`; `$pip.which:[bin]` - returns the bin path in pip by `pip show [bin]`",
             "type": "object"
         }
     },
     "properties": {
         "bashDependencies": {
             "$ref": "#/definitions/osDependency"
         },
         "gitHooks": {
             "$ref": "#/definitions/gitHook"
         },
         "pythonDependencies": {
-            "$ref": "#/definitions/dependency"
+            "$ref": "#/definitions/pythonDependency"
         },
         "vscodeDependencies": {
-            "$ref": "#/definitions/dependency"
+            "$ref": "#/definitions/vscodeDependency"
         },
         "vscodeUserSettings": {
-            "$ref": "#/definitions/dependency"
+            "$ref": "#/definitions/vscodeSettings"
         }
     },
     "title": "JSON schema for NPM package.json files",
     "type": "object"
 }
```

### Comparing `devpm-1.0.1/devpm/__main__.py` & `devpm-1.0.2/devpm/__main__.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/cli/main.py` & `devpm-1.0.2/devpm/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/commands/__init__.py` & `devpm-1.0.2/devpm/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/commands/install.py` & `devpm-1.0.2/devpm/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/utils/bash.py` & `devpm-1.0.2/devpm/_internal/utils/bash.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/utils/code.py` & `devpm-1.0.2/devpm/_internal/utils/code.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/utils/context.py` & `devpm-1.0.2/devpm/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/utils/git.py` & `devpm-1.0.2/devpm/_internal/utils/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,24 +196,26 @@
             has_repo = True
             repo['rev'] = cfg_repo['rev']
             if not 'hooks' in repo:
               repo['hooks'] = cfg_repo['hooks']
             else:
               for cfg_hook in cfg_repo['hooks']:
                 id = cfg_hook['id']
-                found = False
+                found = None
                 for hook in repo['hooks']:
                   if id == hook['id']:
                     found = True
+                    for key in cfg_hook:
+                      hook[key] = cfg_hook[key]
                     break
                 if not found:
                   repo['hooks'].append(cfg_hook)
           if not has_repo:
             data['repos'].append(cfg_repo)
-      new_file_content = yaml.dump(data)
+      new_file_content = yaml.dump(data, sort_keys=False)
       if file_content == new_file_content:
         new_file_content = None
     if new_file_content:
       print('update %s' % (name))
       with open(target_pre_commit_config, 'w', encoding='utf-8') as f:
         f.write(new_file_content)
```

### Comparing `devpm-1.0.1/devpm/_internal/utils/log.py` & `devpm-1.0.2/devpm/_internal/utils/log.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/devpm/_internal/utils/pip.py` & `devpm-1.0.2/devpm/_internal/utils/pip.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/.gitignore` & `devpm-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/LICENSE` & `devpm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devpm-1.0.1/pyproject.toml` & `devpm-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 sources = ["src"]
 directory = "devpm"
 include = ["**/*.py", "devpackage.schema.json"]
 
 [project]
 name = "devpm"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Galen Lin", email="oolgloo.2012@gmail.com" },
 ]
 description = "Development package manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

