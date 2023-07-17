# Comparing `tmp/glean-cli-0.6.2.tar.gz` & `tmp/glean-cli-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.6.2.tar", last modified: Mon Jul 10 17:31:39 2023, max compression
+gzip compressed data, was "glean-cli-0.6.3.tar", last modified: Mon Jul 17 14:37:33 2023, max compression
```

## Comparing `glean-cli-0.6.2.tar` & `glean-cli-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.923319 glean-cli-0.6.2/
--rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 glean-cli-0.6.2/LICENSE
--rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-10 17:31:39.923386 glean-cli-0.6.2/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      832 2023-01-19 16:41:15.000000 glean-cli-0.6.2/README.md
--rw-r--r--   0 anixon     (501) staff       (20)      103 2022-12-17 00:47:55.000000 glean-cli-0.6.2/pyproject.toml
--rw-r--r--   0 anixon     (501) staff       (20)      831 2023-07-10 17:31:39.923738 glean-cli-0.6.2/setup.cfg
--rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 glean-cli-0.6.2/setup.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.918247 glean-cli-0.6.2/src/
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.920266 glean-cli-0.6.2/src/glean/
--rw-r--r--   0 anixon     (501) staff       (20)       18 2023-07-10 17:30:58.000000 glean-cli-0.6.2/src/glean/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)    31995 2023-07-10 17:30:58.000000 glean-cli-0.6.2/src/glean/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1598 2022-12-17 00:47:55.000000 glean-cli-0.6.2/src/glean/credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3904 2023-06-20 13:04:07.000000 glean-cli-0.6.2/src/glean/filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)    14250 2023-07-07 16:24:44.000000 glean-cli-0.6.2/src/glean/glean_api.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.921378 glean-cli-0.6.2/src/glean/utils/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2022-12-17 00:47:55.000000 glean-cli-0.6.2/src/glean/utils/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)      509 2023-01-03 16:54:54.000000 glean-cli-0.6.2/src/glean/utils/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     2622 2023-06-15 18:48:08.000000 glean-cli-0.6.2/src/glean/utils/grn.py
--rw-r--r--   0 anixon     (501) staff       (20)     1356 2023-06-23 20:05:46.000000 glean-cli-0.6.2/src/glean/utils/resource.py
--rw-r--r--   0 anixon     (501) staff       (20)     1089 2023-06-15 18:48:08.000000 glean-cli-0.6.2/src/glean/utils/validate_config.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.922240 glean-cli-0.6.2/src/glean_cli.egg-info/
--rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      616 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anixon     (501) staff       (20)        1 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anixon     (501) staff       (20)       41 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 anixon     (501) staff       (20)      116 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 anixon     (501) staff       (20)        6 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.923189 glean-cli-0.6.2/tests/
--rw-r--r--   0 anixon     (501) staff       (20)      309 2022-12-17 00:47:55.000000 glean-cli-0.6.2/tests/test_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1652 2022-12-17 00:47:55.000000 glean-cli-0.6.2/tests/test_credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     4632 2023-06-23 20:05:46.000000 glean-cli-0.6.2/tests/test_filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      666 2022-12-17 00:47:55.000000 glean-cli-0.6.2/tests/test_glean_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.316254 glean-cli-0.6.3/
+-rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 glean-cli-0.6.3/LICENSE
+-rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-17 14:37:33.316319 glean-cli-0.6.3/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      832 2023-01-19 16:41:15.000000 glean-cli-0.6.3/README.md
+-rw-r--r--   0 anixon     (501) staff       (20)      103 2022-12-17 00:47:55.000000 glean-cli-0.6.3/pyproject.toml
+-rw-r--r--   0 anixon     (501) staff       (20)      831 2023-07-17 14:37:33.316624 glean-cli-0.6.3/setup.cfg
+-rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 glean-cli-0.6.3/setup.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.311422 glean-cli-0.6.3/src/
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.313217 glean-cli-0.6.3/src/glean/
+-rw-r--r--   0 anixon     (501) staff       (20)       18 2023-07-17 14:36:59.000000 glean-cli-0.6.3/src/glean/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)    29317 2023-07-17 14:36:59.000000 glean-cli-0.6.3/src/glean/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1598 2022-12-17 00:47:55.000000 glean-cli-0.6.3/src/glean/credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3904 2023-06-20 13:04:07.000000 glean-cli-0.6.3/src/glean/filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)    11337 2023-07-17 14:36:59.000000 glean-cli-0.6.3/src/glean/glean_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.314408 glean-cli-0.6.3/src/glean/utils/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2022-12-17 00:47:55.000000 glean-cli-0.6.3/src/glean/utils/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)      509 2023-01-03 16:54:54.000000 glean-cli-0.6.3/src/glean/utils/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2622 2023-06-15 18:48:08.000000 glean-cli-0.6.3/src/glean/utils/grn.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1356 2023-06-23 20:05:46.000000 glean-cli-0.6.3/src/glean/utils/resource.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1089 2023-06-15 18:48:08.000000 glean-cli-0.6.3/src/glean/utils/validate_config.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.315216 glean-cli-0.6.3/src/glean_cli.egg-info/
+-rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      616 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        1 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       41 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anixon     (501) staff       (20)      116 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        6 2023-07-17 14:37:33.000000 glean-cli-0.6.3/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-17 14:37:33.316133 glean-cli-0.6.3/tests/
+-rw-r--r--   0 anixon     (501) staff       (20)      309 2022-12-17 00:47:55.000000 glean-cli-0.6.3/tests/test_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1652 2022-12-17 00:47:55.000000 glean-cli-0.6.3/tests/test_credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4632 2023-06-23 20:05:46.000000 glean-cli-0.6.3/tests/test_filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      666 2022-12-17 00:47:55.000000 glean-cli-0.6.3/tests/test_glean_api.py
```

### Comparing `glean-cli-0.6.2/LICENSE` & `glean-cli-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/PKG-INFO` & `glean-cli-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.2
+Version: 0.6.3
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.6.2/README.md` & `glean-cli-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/setup.cfg` & `glean-cli-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/src/glean/cli.py` & `glean-cli-0.6.3/src/glean/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,34 @@
 from itertools import count
 import logging
 import os
 import string
 import subprocess
 from typing import Optional, List
 from uuid import UUID, uuid3
-import webbrowser
 from pathlib import Path, PurePath, PurePosixPath
 
 import click
 import git
 from requests import Session
 import ruamel.yaml as yaml
-from yaspin import yaspin
 
 from glean import VERSION
 
 from glean.filesystem import local_resources
 from glean.credentials import get_credentials
 from glean.glean_api import (
     build_details_uri,
     clear_model_cache,
     create_build_from_git_revision,
     create_build_from_local_files,
+    upload_files_to_glean,
     login,
-    preview_model_uri,
     get_datasources,
     get_tables,
-    get_model_and_build_summary,
-    export_query,
     pull_resource,
 )
 from glean.utils.cli import cli_error_boundary, getenv_bool
 from glean.utils.grn import GRN_TYPE_KEY_MODEL, GRNComponents, parse_grn
 from glean.utils.resource import Resource
 
 
@@ -84,15 +80,15 @@
 )
 run_dbt_parse_option = click.option(
     "--dbt",
     "run_dbt_parse",
     required=False,
     help="If specified, runs `dbt parse` and uses the resulting manifest.",
     is_flag=True,
-    default=False
+    default=False,
 )
 dbt_parse_flags_argument = click.argument(
     "DBT_FLAGS",
     type=click.STRING,
     nargs=-1,
 )
 local_path_argument = click.argument(
@@ -124,28 +120,58 @@
     if GLEAN_DEBUG or GLEAN_VERBOSE_DEBUG_UNSAFE:
         _enable_http_logging()
     ctx.ensure_object(dict)
     ctx.obj["credentials"] = get_credentials(os.path.expanduser(credentials_filepath))
 
 
 @cli.command(
+    "upload",
+    context_settings=dict(),
+)
+@click.argument("database")
+@click.argument(
+    "filepath", type=click.Path(exists=True, dir_okay=False, allow_dash=True)
+)
+@click.pass_context
+def upload(ctx, database, filepath):
+    """Pushes a file to a Glean duckdb database connection that can be queried using duckdb or used as the basis for a data model."""
+
+    s = Session()
+    project_id = login(s, ctx.obj["credentials"])
+    fp = os.path.expanduser(filepath)
+
+    click.echo("📄 Uploading file to Glean...")
+    filename = upload_files_to_glean(s, project_id, database, fp)
+    click.echo(f'✅ successfully uploaded "{filename}"')
+
+
+@cli.command(
     "preview",
     context_settings=dict(
         ignore_unknown_options=True,
     ),
 )
 @allow_dangerous_empty_build_option
 @git_revision_option
 @git_path_option
 @dbt_manifest_option
 @run_dbt_parse_option
 @local_path_argument
 @dbt_parse_flags_argument
 @click.pass_context
-def preview(ctx, git_revision, git_path, dbt_manifest_path, filepath, run_dbt_parse, dbt_flags, allow_dangerous_empty_build):
+def preview(
+    ctx,
+    git_revision,
+    git_path,
+    dbt_manifest_path,
+    filepath,
+    run_dbt_parse,
+    dbt_flags,
+    allow_dangerous_empty_build,
+):
     """Validates resource configurations and generates a preview link."""
     dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
 
     click.echo("🏗️  Creating preview build...")
     build_results = _create_build_using_options(
         ctx,
         filepath,
@@ -206,14 +232,15 @@
     build_results = _create_build_using_options(
         ctx,
         filepath,
         git_revision=git_revision,
         git_path=git_path,
         deploy=True,
         dbt_manifest_path=dbt_manifest_path,
+        allow_dangerous_empty_build=allow_dangerous_empty_build,
     )
     _echo_build_results(build_results, True)
     click.echo("")
     click.echo(click.style("✅ Deploy complete.", fg="bright_green"))
 
 
 @cli.command()
@@ -451,112 +478,14 @@
     if updated_files:
         click.echo("✅ Done. Files created or modified:")
         _echo_list([str(p) for p in updated_files])
     else:
         click.echo("✅ Done. No files were updated.")
 
 
-@cli.command()
-@click.argument("database")
-@click.argument("table")
-@click.option(
-    "--exclude",
-    "-e",
-    help="A comma-separated list of columns to exclude from the preview.",
-)
-@click.option(
-    "--include",
-    "-i",
-    help="A comma-separated list of columns to include in the preview.",
-)
-@click.option(
-    "--regex",
-    "-r",
-    help="A regular expression to filter column names by. You can use this along with the --include and/or --exclude options to include columns regardless of the regex result.",
-)
-@click.option(
-    "--skip-confirmation",
-    is_flag=True,
-    help="If set, the generated model configuration file will silently overwrite any existing files with the same name in your current directory.",
-)
-@click.pass_context
-def explore(
-    ctx: click.Context,
-    database: str,
-    table: str,
-    exclude: str = "",
-    include: str = "",
-    regex: str = "",
-    skip_confirmation: bool = False,
-):
-    """Explore your data! Specify a database and table to generate a Glean preview for it.
-
-    DATABASE is the name of a Glean database connection you want to explore.
-    TABLE is the name of a table within your DATABASE. Alternatively, it can be a SQL query wrapped in quotes.
-
-    Usage examples:
-
-    $ glean explore database_connection_name table_name
-
-    $ glean explore database_connection_name "SELECT * FROM table_name"
-
-    $ glean explore database_connection_name table_name --regex "[^date]$" --include important_date --exclude extra_info
-
-    """
-    s = Session()
-    project_id = login(s, ctx.obj["credentials"])
-
-    datasources = get_datasources(s, project_id)
-    if database not in datasources:
-        _echo_datasource_not_found(database, datasources)
-        exit(1)
-    datasource_id = datasources[database]
-
-    _limit_column_filters(exclude, include, regex)
-
-    model_spec = {
-        "columnsToExclude": exclude.split(",") if exclude else [],
-        "columnsToInclude": include.split(",") if include else [],
-        "columnsRegex": regex if regex else "",
-    }
-
-    if not _infer_if_sql(table):
-        tables = get_tables(s, datasource_id)
-        if table not in tables:
-            _echo_table_not_found(table, tables, database)
-            exit(1)
-
-        with yaspin(text="Generating your data model...", color="yellow") as spinner:
-            model_spec["schema"] = tables[table]["schema"]
-            model_spec["tableName"] = tables[table]["name"]
-            model, build_summary = get_model_and_build_summary(
-                s, datasource_id, project_id, **model_spec
-            )
-    else:
-        with yaspin(text="Generating your data model...", color="yellow") as spinner:
-            model_spec["sqlStatement"] = table
-            model, build_summary = get_model_and_build_summary(
-                s, datasource_id, project_id, **model_spec
-            )
-
-    config = export_query(
-        s, "model", model, additional_headers={"Content-Type": "yaml"}
-    )
-    model_yaml = yaml.load(config, Loader=yaml.RoundTripLoader)
-    if "grn" in model_yaml:
-        del model_yaml["grn"]
-    config = yaml.dump(model_yaml, Dumper=yaml.RoundTripDumper)
-
-    filename = model["name"]
-    _save_config(config, filename, skip_confirmation=skip_confirmation)
-
-    _echo_build_results(build_summary, False, query_name="modelPreviewBuildFromGleanDb")
-    webbrowser.open(preview_model_uri(model["id"], build_summary))
-
-
 def _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags):
     """Convenience wrapper for running `dbt parse` before `glean preview` or `glean deploy`.
     Must be run from your Glean project directory.
 
     Flags passed in after the Glean subcommand will be passed onwards to dbt.
     """
 
@@ -565,15 +494,17 @@
         if dbt_manifest_path is not None:
             # user specified --dbt-manifest explicitly
             click.echo(f"✅ Using manifest file at {dbt_manifest_path}\n")
         return dbt_manifest_path
 
     if dbt_manifest_path is not None:
         click.echo()
-        click.echo("🚨 `--dbt-manifest` is redundant when running with `--dbt` and will be ignored.")
+        click.echo(
+            "🚨 `--dbt-manifest` is redundant when running with `--dbt` and will be ignored."
+        )
         click.echo()
     click.echo("🐇 Running `dbt parse` to generate a manifest file.")
 
     click.echo()
 
     dbt_flags = list(dbt_flags) or []
     # find the dbt target dir (some manual flags parsing)
@@ -595,15 +526,17 @@
     ret_code = subprocess.Popen(dbt_command.split(" ")).wait()
     click.echo("--- end of dbt output ---")
     if ret_code != 0:
         raise click.ClickException(f"dbt returned nonzero exit code ({ret_code})")
 
     manifest_path = target_dir / "manifest.json"
     if not manifest_path.is_file():
-        raise click.ClickException("⚠️ manifest file does not exist after `dbt parse` ran successfully.")
+        raise click.ClickException(
+            "⚠️ manifest file does not exist after `dbt parse` ran successfully."
+        )
 
     click.echo()
     click.echo(f"✅ Using manifest file at {manifest_path}\n")
     return manifest_path
 
 
 def _infer_if_sql(table: str) -> bool:
```

### Comparing `glean-cli-0.6.2/src/glean/credentials.py` & `glean-cli-0.6.3/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/src/glean/filesystem.py` & `glean-cli-0.6.3/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/src/glean/glean_api.py` & `glean-cli-0.6.3/src/glean/glean_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import os
 from pathlib import PurePath
-from typing import List, Optional, Tuple, Dict
-from collections import OrderedDict
+from typing import List, Optional, Dict
 
 import click
 from click import ClickException
 from requests import Session
 
 from glean.credentials import CliCredentials
 from glean.filesystem import build_spec_from_local
 from glean import VERSION
 from glean.utils.resource import Resource
 
 GLEAN_BASE_URI = os.environ.get("GLEAN_CLI_BASE_URI", default="https://glean.io")
+FILE_SIZE_LIMIT_MB = 50
 
 
 def login(session: Session, credentials: CliCredentials):
     """Authenticates the session with the provided credentials.
 
     :return The user's project ID, if successfully logged in.
     :raises ClickException if the login is not successful.
@@ -80,42 +80,14 @@
     """Creates a build using local files and returns the result."""
     build_spec = build_spec_from_local(path, project_id, targets, dbt_manifest_path)
     return _create_build(
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
-def get_model_and_build_summary(
-    session: Session,
-    datasource_id: str,
-    project_id: str,
-    **kwargs,
-) -> Tuple[dict, dict]:
-    build_summary = _model_build_from_db(
-        session,
-        project_id,
-        datasource_id,
-        add_all_columns_as_attributes=True,
-        **kwargs,
-    )
-
-    if "errors" in build_summary:
-        click.secho("Error encountered when creating your build: ", fg="red")
-        error = build_summary["errors"][0]
-        if "extensions" in error:
-            if "userMessage" in error["extensions"]:
-                raise RuntimeError(error["extensions"]["userMessage"])
-        raise RuntimeError(error.get("message", "Unknown error"))
-
-    model = build_summary["data"]["modelPreviewBuildFromGleanDb"]["resources"]["added"][
-        "modelBundles"
-    ][0]["model"]
-    return model, build_summary
-
-
 def get_datasources(s: Session, project_id: str) -> dict:
     """Queries and formats datasources"""
     query = _get_data_connections(s, project_id)
     data_sources = {d["name"]: d["id"] for d in query["data"]["dataConnections"]}
     return data_sources
 
 
@@ -236,108 +208,14 @@
         }
         """,
         {"datasourceId": datasource_id},
     )
     return query
 
 
-def _model_build_from_db(
-    session: Session,
-    project_id: str,
-    datasource_id: str,
-    **kwargs,
-) -> dict:
-    """
-    Queries modelPreviewBuildFromGleanDb controller.
-    Returns relevant fields from model needed to generate a data ops config, as well the names of other resources for formatting purposes
-    """
-
-    add_all_columns_as_attributes = True
-    table_name = kwargs.get("tableName")
-    schema = kwargs.get("schema")
-    sql_statement = kwargs.get("sqlStatement")
-    columns_to_exclude = kwargs.get("columnsToExclude")
-    columns_to_include = kwargs.get("columnsToInclude")
-    columns_regex = kwargs.get("columnsRegex")
-
-    query = _graphql_query(
-        session,
-        """
-        mutation modelPreviewBuildFromGleanDb(
-            $datasourceId: String!,
-            $projectId: String!,
-            $tableName: String,
-            $schema: String,
-            $sqlStatement: String,
-            $columnsToExclude: [String]
-            $columnsToInclude: [String]
-            $columnsRegex: String
-            $addAllColumnsAsAttributes: Boolean,
-            ) {
-            modelPreviewBuildFromGleanDb(
-                datasourceId: $datasourceId,
-                projectId: $projectId
-                tableName: $tableName,
-                schema: $schema,
-                sqlStatement: $sqlStatement,
-                columnsToExclude: $columnsToExclude,
-                columnsToInclude: $columnsToInclude,
-                columnsRegex: $columnsRegex,
-                addAllColumnsAsAttributes: $addAllColumnsAsAttributes,
-                ) {
-                id,
-                resources {
-                    added {
-                        modelBundles {
-                            model {
-                                id,
-                                project,
-                                createdAt,
-                                updatedAt,
-                                name,
-                                createdById,
-                                isPrivate,
-                                markedPrivateBy,
-                                dataOpsRevision,
-                                sourceDataTable,
-                                attributes,
-                                metrics,
-                                cacheTtlSec,
-                                description
-                            }
-                        },
-                        savedViews { name },
-                        dashboards { name },
-                        colorPalettes { name },
-                        homepageLaunchpads { id }
-                    }
-                    changed { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    unchanged { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    deleted { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                },
-                warnings,
-                errors
-            }
-        }
-        """,
-        {
-            "datasourceId": datasource_id,
-            "projectId": project_id,
-            "tableName": table_name,
-            "schema": schema,
-            "sqlStatement": sql_statement,
-            "columnsToExclude": columns_to_exclude,
-            "columnsToInclude": columns_to_include,
-            "columnsRegex": columns_regex,
-            "addAllColumnsAsAttributes": add_all_columns_as_attributes,
-        },
-    )
-    return query
-
-
 def get_tables(s: Session, datasource_id: str) -> Dict[str, Dict[str, str]]:
     """Queries and formats table from datasource"""
     query = _get_table_data(s, datasource_id)
     tables = _parse_table_data(query)
     return tables
 
 
@@ -375,26 +253,82 @@
         graphql_exceptions
         and isinstance(graphql_exceptions[0], dict)
         and graphql_exceptions[0].get("message")
     ):
         error = graphql_exceptions[0]["message"]
 
         # Must match error message in server code at glean/services/data_ops/build_management.py line #543 (as of 7/5/23).
-        if error == "No Glean config files were found, and empty builds were not enabled, so the build was aborted.":
-            error += "\n\tTo enable empty builds, use the --allow-dangerous-empty-builds flag.\n\tWARNING: This will remove all data-ops managed resources, and any resources that depend on them, from your project."
+        if (
+            error
+            == "No Glean config files were found, and empty builds were not enabled, so the build was aborted."
+        ):
+            error += "\n\tTo enable empty builds, use the --allow-dangerous-empty-build flag.\n\tWARNING: This will remove all data-ops managed resources, and any resources that depend on them, from your project."
             from glean.cli import _echo_build_errors_and_exit
+
             _echo_build_errors_and_exit([error])
 
         raise ClickException(
             f"Unexpected error received from the Glean server:\n  {error}"
         )
 
     return results
 
 
+def upload_files_to_glean(
+    session: Session, project_id: str, database_name: str, path: str
+) -> str:
+    datasources = get_datasources(session, project_id)
+    db_id = datasources.get(database_name)
+
+    if db_id:
+        return _post_file(session, project_id, db_id, path)
+    else:
+        raise ClickException(
+            "Error uploading file\n  Datbase does not exist with name "
+            f'"{database_name}"'
+            "\n  run glean databases to see valid names "
+        )
+
+
+def _is_over_filesize_limit(file_path: str) -> bool:
+    size_in_bytes = os.path.getsize(file_path)
+    size_in_mb = size_in_bytes / (1024 * 1024)
+
+    return size_in_mb > FILE_SIZE_LIMIT_MB
+
+
+def _post_file(session: Session, project_id: str, db_id: str, file_path: str) -> str:
+    if _is_over_filesize_limit(file_path):
+        raise ClickException(
+            f"File exceeds upload limit of {FILE_SIZE_LIMIT_MB} megabytes"
+        )
+
+    r = session.post(
+        GLEAN_BASE_URI + "/upload/data-file",
+        data={
+            "projectId": project_id,
+            "dataConnectionId": db_id,
+        },
+        files={"file": open(file_path, "rb")},
+        headers={"Glean-CLI-Version": VERSION},
+    )
+
+    results = r.json()
+    file_errors = results.get("error")
+    if file_errors:
+        raise ClickException(f"Error uploading file\n  {file_errors}")
+
+    uploaded_filename = results.get("filename")
+
+    if uploaded_filename:
+        return uploaded_filename
+    else:
+        raise ClickException(f"Error uploading file\n  Unexpected result from server")
+
+
 def export_query(
     session: Session, endpoint: str, data: dict, additional_headers: dict = {}
 ):
     """POST request to export controllers"""
     r = session.post(
         GLEAN_BASE_URI + f"/export/{endpoint}",
         data=json.dumps(data),
```

### Comparing `glean-cli-0.6.2/src/glean/utils/grn.py` & `glean-cli-0.6.3/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/src/glean/utils/resource.py` & `glean-cli-0.6.3/src/glean/utils/resource.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/src/glean/utils/validate_config.py` & `glean-cli-0.6.3/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.6.3/src/glean_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.2
+Version: 0.6.3
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.6.2/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.6.3/src/glean_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/tests/test_credentials.py` & `glean-cli-0.6.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/tests/test_filesystem.py` & `glean-cli-0.6.3/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.2/tests/test_glean_api.py` & `glean-cli-0.6.3/tests/test_glean_api.py`

 * *Files identical despite different names*

