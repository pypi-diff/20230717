# Comparing `tmp/datasette-auth-tokens-0.3.tar.gz` & `tmp/datasette-auth-tokens-0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-auth-tokens-0.3.tar", last modified: Fri Oct 15 00:58:48 2021, max compression
+gzip compressed data, was "datasette-auth-tokens-0.4a0.tar", last modified: Mon Jul 17 19:12:58 2023, max compression
```

## Comparing `datasette-auth-tokens-0.3.tar` & `datasette-auth-tokens-0.4a0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 00:58:48.401335 datasette-auth-tokens-0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-15 00:58:39.000000 datasette-auth-tokens-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7134 2021-10-15 00:58:48.397335 datasette-auth-tokens-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2021-10-15 00:58:39.000000 datasette-auth-tokens-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 00:58:48.397335 datasette-auth-tokens-0.3/datasette_auth_tokens/
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-10-15 00:58:39.000000 datasette-auth-tokens-0.3/datasette_auth_tokens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 00:58:48.397335 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7134 2021-10-15 00:58:48.000000 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-10-15 00:58:48.000000 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 00:58:48.000000 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-15 00:58:48.000000 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-15 00:58:48.000000 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-15 00:58:48.000000 datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 00:58:48.401335 datasette-auth-tokens-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2021-10-15 00:58:39.000000 datasette-auth-tokens-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:12:58.684663 datasette-auth-tokens-0.4a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-17 19:12:58.684663 datasette-auth-tokens-0.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:12:58.684663 datasette-auth-tokens-0.4a0/datasette_auth_tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:12:58.684663 datasette-auth-tokens-0.4a0/datasette_auth_tokens/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens/templates/create_api_token.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens/templates/token_details.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:12:58.684663 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-17 19:12:58.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-17 19:12:58.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:12:58.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 19:12:58.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 19:12:58.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:12:58.000000 datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:12:58.684663 datasette-auth-tokens-0.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 19:12:45.000000 datasette-auth-tokens-0.4a0/setup.py
```

### Comparing `datasette-auth-tokens-0.3/LICENSE` & `datasette-auth-tokens-0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-auth-tokens-0.3/PKG-INFO` & `datasette-auth-tokens-0.4a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: datasette-auth-tokens
-Version: 0.3
+Version: 0.4a0
 Summary: Datasette plugin for authenticating access using API tokens
 Home-page: https://github.com/simonw/datasette-auth-tokens
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-auth-tokens/issues
 Project-URL: CI, https://github.com/simonw/datasette-auth-tokens/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-auth-tokens/releases
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # datasette-auth-tokens
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-auth-tokens.svg)](https://pypi.org/project/datasette-auth-tokens/)
@@ -129,17 +128,42 @@
 ```
 
 You can now run authenticated API queries like this:
 
     $ curl http://127.0.0.1:8001/:memory:/show_version.json?_shape=array&_auth_token=this-is-the-secret-token
     [{"sqlite_version()": "3.31.1"}]
 
-## Tokens from your database
+## Managed tokens mode
 
-As an alternative (or in addition) to the hard-coded list of tokens you can store tokens in a database table and configure the plugin to access them using a SQL query.
+`datasette-auth-tokens` provides a managed tokens mode, where tokens are stored in a SQLite database table and the plugin provides an interface for creating and revoking tokens.
+
+To turn this mode on, add `"manage_tokens": true` to your plugin configuration in `metadata.json`:
+
+```json
+{
+    "plugins": {
+        "datasette-auth-tokens": {
+            "manage_tokens": true
+        }
+    }
+}
+```
+This will add a "Create API token" option to the Datasette menu.
+
+Tokens that are created will be kept in a new `_datasette_auth_tokens` table.
+
+Navigating to that table page will provide the option to view and revoke tokens.
+
+When you create a new token a signed token string will be presented to you. You need to store this, as it is not stored directly in the database table and can only be retrieved once.
+
+## Custom tokens from your database
+
+If you decide not to use managed tokens mode, you can instead configure `datasette-auth-tokens` to use tokens that are stored in your own custom database tables.
+
+You can do this by configuring a custom SQL query that will execute to test if an incoming token is valid.
 
 Your query needs to take a `:token_id` parameter and return at least two columns: one called `token_secret` and one called `actor_*` - usually `actor_id`. Further `actor_` prefixed columns can be returned to provide more details for the authenticated actor.
 
 Here's a simple example of a configuration query:
 
 ```sql
 select actor_id, actor_name, token_secret from tokens where token_id = :token_id
@@ -180,14 +204,12 @@
             "allow": {}
         }
     }
 }
 ```
 The `"sql"` key here contains the SQL query. The `"database"` key has the name of the attached database file that the query should be executed against - in this case it would execute against `tokens.db`.
 
-### Securing your tokens
+### Securing your custom tokens
 
 Anyone with access to your Datasette instance can use it to read the `token_secret` column in your tokens table. This probably isn't what you want!
 
 To avoid this, you should lock down access to that table. The configuration example above shows how to do this using an `"allow": {}` block. Consult Datasette's [Permissions documentation](https://datasette.readthedocs.io/en/stable/authentication.html#permissions) for more information about how to lock down this kind of access.
-
-
```

### Comparing `datasette-auth-tokens-0.3/README.md` & `datasette-auth-tokens-0.4a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -114,17 +114,42 @@
 ```
 
 You can now run authenticated API queries like this:
 
     $ curl http://127.0.0.1:8001/:memory:/show_version.json?_shape=array&_auth_token=this-is-the-secret-token
     [{"sqlite_version()": "3.31.1"}]
 
-## Tokens from your database
+## Managed tokens mode
 
-As an alternative (or in addition) to the hard-coded list of tokens you can store tokens in a database table and configure the plugin to access them using a SQL query.
+`datasette-auth-tokens` provides a managed tokens mode, where tokens are stored in a SQLite database table and the plugin provides an interface for creating and revoking tokens.
+
+To turn this mode on, add `"manage_tokens": true` to your plugin configuration in `metadata.json`:
+
+```json
+{
+    "plugins": {
+        "datasette-auth-tokens": {
+            "manage_tokens": true
+        }
+    }
+}
+```
+This will add a "Create API token" option to the Datasette menu.
+
+Tokens that are created will be kept in a new `_datasette_auth_tokens` table.
+
+Navigating to that table page will provide the option to view and revoke tokens.
+
+When you create a new token a signed token string will be presented to you. You need to store this, as it is not stored directly in the database table and can only be retrieved once.
+
+## Custom tokens from your database
+
+If you decide not to use managed tokens mode, you can instead configure `datasette-auth-tokens` to use tokens that are stored in your own custom database tables.
+
+You can do this by configuring a custom SQL query that will execute to test if an incoming token is valid.
 
 Your query needs to take a `:token_id` parameter and return at least two columns: one called `token_secret` and one called `actor_*` - usually `actor_id`. Further `actor_` prefixed columns can be returned to provide more details for the authenticated actor.
 
 Here's a simple example of a configuration query:
 
 ```sql
 select actor_id, actor_name, token_secret from tokens where token_id = :token_id
@@ -165,12 +190,12 @@
             "allow": {}
         }
     }
 }
 ```
 The `"sql"` key here contains the SQL query. The `"database"` key has the name of the attached database file that the query should be executed against - in this case it would execute against `tokens.db`.
 
-### Securing your tokens
+### Securing your custom tokens
 
 Anyone with access to your Datasette instance can use it to read the `token_secret` column in your tokens table. This probably isn't what you want!
 
 To avoid this, you should lock down access to that table. The configuration example above shows how to do this using an `"allow": {}` block. Consult Datasette's [Permissions documentation](https://datasette.readthedocs.io/en/stable/authentication.html#permissions) for more information about how to lock down this kind of access.
```

### Comparing `datasette-auth-tokens-0.3/datasette_auth_tokens.egg-info/PKG-INFO` & `datasette-auth-tokens-0.4a0/datasette_auth_tokens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: datasette-auth-tokens
-Version: 0.3
+Version: 0.4a0
 Summary: Datasette plugin for authenticating access using API tokens
 Home-page: https://github.com/simonw/datasette-auth-tokens
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-auth-tokens/issues
 Project-URL: CI, https://github.com/simonw/datasette-auth-tokens/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-auth-tokens/releases
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # datasette-auth-tokens
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-auth-tokens.svg)](https://pypi.org/project/datasette-auth-tokens/)
@@ -129,17 +128,42 @@
 ```
 
 You can now run authenticated API queries like this:
 
     $ curl http://127.0.0.1:8001/:memory:/show_version.json?_shape=array&_auth_token=this-is-the-secret-token
     [{"sqlite_version()": "3.31.1"}]
 
-## Tokens from your database
+## Managed tokens mode
 
-As an alternative (or in addition) to the hard-coded list of tokens you can store tokens in a database table and configure the plugin to access them using a SQL query.
+`datasette-auth-tokens` provides a managed tokens mode, where tokens are stored in a SQLite database table and the plugin provides an interface for creating and revoking tokens.
+
+To turn this mode on, add `"manage_tokens": true` to your plugin configuration in `metadata.json`:
+
+```json
+{
+    "plugins": {
+        "datasette-auth-tokens": {
+            "manage_tokens": true
+        }
+    }
+}
+```
+This will add a "Create API token" option to the Datasette menu.
+
+Tokens that are created will be kept in a new `_datasette_auth_tokens` table.
+
+Navigating to that table page will provide the option to view and revoke tokens.
+
+When you create a new token a signed token string will be presented to you. You need to store this, as it is not stored directly in the database table and can only be retrieved once.
+
+## Custom tokens from your database
+
+If you decide not to use managed tokens mode, you can instead configure `datasette-auth-tokens` to use tokens that are stored in your own custom database tables.
+
+You can do this by configuring a custom SQL query that will execute to test if an incoming token is valid.
 
 Your query needs to take a `:token_id` parameter and return at least two columns: one called `token_secret` and one called `actor_*` - usually `actor_id`. Further `actor_` prefixed columns can be returned to provide more details for the authenticated actor.
 
 Here's a simple example of a configuration query:
 
 ```sql
 select actor_id, actor_name, token_secret from tokens where token_id = :token_id
@@ -180,14 +204,12 @@
             "allow": {}
         }
     }
 }
 ```
 The `"sql"` key here contains the SQL query. The `"database"` key has the name of the attached database file that the query should be executed against - in this case it would execute against `tokens.db`.
 
-### Securing your tokens
+### Securing your custom tokens
 
 Anyone with access to your Datasette instance can use it to read the `token_secret` column in your tokens table. This probably isn't what you want!
 
 To avoid this, you should lock down access to that table. The configuration example above shows how to do this using an `"allow": {}` block. Consult Datasette's [Permissions documentation](https://datasette.readthedocs.io/en/stable/authentication.html#permissions) for more information about how to lock down this kind of access.
-
-
```

### Comparing `datasette-auth-tokens-0.3/setup.py` & `datasette-auth-tokens-0.4a0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3"
+VERSION = "0.4a0"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -24,11 +24,14 @@
         "CI": "https://github.com/simonw/datasette-auth-tokens/actions",
         "Changelog": "https://github.com/simonw/datasette-auth-tokens/releases",
     },
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["datasette_auth_tokens"],
     entry_points={"datasette": ["auth_tokens = datasette_auth_tokens"]},
-    install_requires=["datasette>=0.44",],
+    install_requires=[
+        "datasette>=1.0a2",
+        "sqlite-utils",
+    ],
     extras_require={"test": ["pytest", "pytest-asyncio", "httpx", "sqlite-utils"]},
-    tests_require=["datasette-auth-tokens[test]"],
+    package_data={"datasette_auth_tokens": ["templates/*.html"]},
 )
```

