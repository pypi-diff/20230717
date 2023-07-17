# Comparing `tmp/data_ecosystem_flask-202306.0.34.tar.gz` & `tmp/data_ecosystem_flask-202307.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202306.0.34.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202307.0.2.tar", max compression
```

## Comparing `data_ecosystem_flask-202306.0.34.tar` & `data_ecosystem_flask-202307.0.2.tar`

### file list

```diff
@@ -1,25 +1,17 @@
--rw-r--r--   0        0        0    10359 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/Makefile
--rw-r--r--   0        0        0      863 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/Makefile.ps1
--rw-r--r--   0        0        0    58465 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    12102 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0   145583 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
--rw-r--r--   0        0        0   145583 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
--rw-r--r--   0        0        0   325863 2023-06-27 22:56:53.967202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
--rw-r--r--   0        0        0   325863 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
--rw-r--r--   0        0        0   145835 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
--rw-r--r--   0        0        0     1692 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_posit_manifests/manifest.json
--rw-r--r--   0        0        0    12165 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
--rw-r--r--   0        0        0    28571 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/install.py
--rw-r--r--   0        0        0     2082 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0     5285 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
--rw-r--r--   0        0        0     5240 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
--rw-r--r--   0        0        0      374 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
--rw-r--r--   0        0        0    17091 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0    14015 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/schema/manifest.schema.json
--rw-r--r--   0        0        0     2401 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/data_ecosystem_flask/templates/log_file.html
--rw-r--r--   0        0        0    11357 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/license.md
--rw-r--r--   0        0        0     2463 2023-06-27 23:05:49.285044 data_ecosystem_flask-202306.0.34/pyproject.toml
--rw-r--r--   0        0        0    15006 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/readme.md
--rw-r--r--   0        0        0      126 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-27 22:56:53.971202 data_ecosystem_flask-202306.0.34/setup.py
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.34/PKG-INFO
+-rw-r--r--   0        0        0      863 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0     1155 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/__init__.py
+-rw-r--r--   0        0        0    41602 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    13216 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0    28571 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0     2082 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0    16945 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0     1572 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/download.html
+-rw-r--r--   0        0        0      432 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/error.html
+-rw-r--r--   0        0        0     2723 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0     1905 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/upload.html
+-rw-r--r--   0        0        0    11357 2023-07-17 03:03:08.516189 data_ecosystem_flask-202307.0.2/license.md
+-rw-r--r--   0        0        0     2559 2023-07-17 03:09:37.323715 data_ecosystem_flask-202307.0.2/pyproject.toml
+-rw-r--r--   0        0        0    15040 2023-07-17 03:03:08.520189 data_ecosystem_flask-202307.0.2/readme.md
+-rw-r--r--   0        0        0      126 2023-07-17 03:03:08.520189 data_ecosystem_flask-202307.0.2/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-17 03:03:08.520189 data_ecosystem_flask-202307.0.2/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.2/PKG-INFO
```

### Comparing `data_ecosystem_flask-202306.0.34/data_ecosystem_flask/Makefile.ps1` & `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/Makefile.ps1`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.34/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app_startup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from flask import Flask
-from flask_restx import Api, Resource, fields, Namespace
-from datetime import datetime
+from flask_restx import Api
 from pathlib import Path
 import shutil
 from dotenv import load_dotenv, set_key, dotenv_values
 import os
 from flask import request
+from werkzeug.middleware.proxy_fix import ProxyFix
 
 # Importing necessary modules from data_ecosystem_services package
 # These modules seem to be related to environment metadata, tracing and logging.
 from data_ecosystem_services.cdc_self_service import (
     environment_metadata as pade_env_metadata
 )
 from data_ecosystem_services.cdc_admin_service import (
@@ -23,25 +23,40 @@
 
 import os
 import sys
 import importlib
 
 # Constant indicating if the application is running inside Windows Subsystem for Linux (WSL)
 RUNNING_IN_WSL = False
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
+def change_to_root_directory():
+    # Get the absolute path of the current script
+    current_script_path = os.path.abspath(__file__)
+
+    # Get the project root directory by going up one or more levels
+    project_root = os.path.dirname(os.path.dirname(current_script_path))
+
+    # Change the current working directory to the project root directory
+    os.chdir(project_root)
 
 
 def change_to_flask_directory():
     current_directory = os.getcwd()  # get current directory
     base_directory = os.path.basename(
         current_directory)  # get the base directory
 
     if base_directory != 'data_ecosystem_flask':
         # path to the directory you want to change to
         new_directory = os.path.join(
-            current_directory, 'pade-flask/data_ecosystem_flask')
+            current_directory, 'pade_flask/data_ecosystem_flask')
 
         # change to new directory
         os.chdir(new_directory)
         print(f"Directory changed to {os.getcwd()}")
     else:
         print("Current directory is already 'data_ecosystem_flask'")
 
@@ -99,15 +114,15 @@
         url="/",
     )
 
     ns_welcome = api.namespace(
         "welcome", description="Welcome to the CDC Data Ecosystem API")
 
     TECH_ENVIRONMENT_DESCRIPTION = (
-        "The tech-environment service manages the technical environment in which "
+        "The tech-environment service manages the technical environment in whFich "
         "the data products and associated services are developed, deployed, and "
         "managed. This package contains datasets that provide critical information "
         "for understanding the technical architecture, components, and "
         "resources used to support the data products and associated services."
     )
 
     ns_tech_environment = api.namespace(
@@ -201,69 +216,80 @@
     Note:
         This function currently has no functionality. You should add Flask app creation and configuration logic inside it.
 
     """
     # Add your Flask app creation and configuration logic here
 
     # Get the path to the .env file
+
+    CURRENT_USER_NAME = os.getenv('USERNAME') or os.getenv('USER')
+    API_PATH = "/data-ecosystem-services/data_ecosystem_services"
     dotenv_path = os.path.join(os.path.dirname(__file__), '.env')
 
     # Load the .env file
     load_dotenv(dotenv_path)
     instrumentation_key = "d091b27b-14e0-437f-ae3c-90f3f04ef3dc"
     set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE",
             "1")
     set_key(dotenv_path, "APPLICATIONINSIGHTS_CONNECTION_STRING",
             f"InstrumentationKey={instrumentation_key};IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/")
     set_key(dotenv_path, "APPINSIGHTS_INSTRUMENTATIONKEY",
             instrumentation_key)
     # Reload the updated .env file
     load_dotenv(dotenv_path)
 
-    logger_singleton = pade_env_logging.LoggerSingleton.instance()
+    logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        NAMESPACE_NAME, SERVICE_NAME)
     logger = logger_singleton.get_logger()
-    tracer_singleton = pade_env_tracing.TracerSingleton.instance()
+    tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        NAMESPACE_NAME, SERVICE_NAME)
     tracer = tracer_singleton.get_tracer()
+    app = None
 
     try:
         with tracer.start_as_current_span("create_app"):
 
+            # Get the absolute path of the directory of the current script
+            dir_path = os.path.dirname(os.path.realpath(__file__))
+
+            # Add this path to PYTHONPATH
+            sys.path.insert(0, dir_path)
+
             logger.info("ran create_app")
 
             obj_env_metadata = pade_env_metadata.EnvironmentMetaData()
             environment = get_environment_name()
-            yyyy = str(datetime.now().year)
-            dd = str(datetime.now().day).zfill(2)
-            mm = str(datetime.now().month).zfill(2)
             running_local = True
-            change_to_flask_directory()
+            change_to_root_directory()
             path = Path(os.getcwd())
             repository_path_default = str(path)
 
             logger.info(
                 f"repository_path_default:{repository_path_default}")
 
             parameters = {
                 "project_id": "ocio_pade_dev",
                 "project_id_root": "ocio",
                 "project_id_individual": "PADE",
                 "environment": environment,
-                "yyyy": yyyy,
-                "dd": dd,
-                "mm": mm,
                 "azure_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
                 "repository_path": repository_path_default,
                 "running_local": running_local,
             }
             config = obj_env_metadata.get_configuration_common(
                 parameters, None)
 
-            logger.info(f"config:{config}")
+            logger.info(f"config_length:{len(config)}")
 
             app = Flask(__name__)
+
+            app.wsgi_app = ProxyFix(
+                app.wsgi_app, x_for=1, x_proto=1, x_host=1, x_prefix=1
+            )
+
             app.env = 'development'
             app.debug = True  # Enable debug mode
 
             app.cdc_config = config
             env_file_path = config.get("env_file_path")
 
             shutil.copy(env_file_path, app.root_path)
@@ -272,29 +298,29 @@
             az_kv_az_sub_client_secret_key = config.get(
                 "az_kv_az_sub_client_secret_key")
             az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
                 "-", "_")
             client_secret = os.getenv(az_kv_az_sub_client_secret_key)
             logger.info(
                 f"az_kv_az_sub_client_secret_key:{az_kv_az_sub_client_secret_key}")
-            logger.info(f"client_secret:{client_secret}")
+            logger.info(f"client_secret length:{len(client_secret)}")
 
             # Set the new value
             set_key(dotenv_path, "FLASK_DEBUG", "1")
             set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE", "1")
             tenant_id = config.get("tenant_id")
             client_id = config.get("client_id")
             az_kv_key_vault_name = config.get("az_kv_key_vault_name")
 
             # Reload the updated .env file
             load_dotenv(dotenv_path)
 
             # Trim leading and trailing whitespace from client_secret
             if client_secret is None:
-                logger.error(f"client_secret is None")
+                logger.warning(f"client_secret is None")
             else:
                 client_secret = client_secret.strip()
 
             running_interactive = False
 
             # Check if the client_secret is None or a zero-length string
             if not client_secret:
@@ -310,34 +336,37 @@
             logger.info(f"env_file_path:{env_file_path}")
             pade_env_tracing.TracerSingleton.log_to_console = False
 
             try:
                 importlib.import_module("data_ecosystem_services")
                 logger.info("data_ecosystem_services is module in pythonpath")
             except ImportError:
-                logger.error(
+                logger.warning(
                     "data_ecosystem_services is not a module in pythonpath")
 
             if RUNNING_IN_WSL is True:
                 sys.path.append(f"/home/{CURRENT_USER_NAME}{API_PATH}")
                 logger.info(f"RUNNING_IN_WSL: {RUNNING_IN_WSL}")
                 logger.info(f"/home/{CURRENT_USER_NAME}{API_PATH}")
             else:
                 sys.path.append(os.path.abspath(
-                    __file__ + "/../../../pade_python/"
+                    __file__ + "/../../../data_ecosystem_services/"
                 ))
                 logger.info(f"RUNNING_IN_WSL: {RUNNING_IN_WSL}")
                 logger.info(
                     os.path.abspath(
-                        __file__ + "/../../../pade_python/"
+                        __file__ + "/../../../data_ecosystem_services/"
                     )
                 )
 
             app.tracer = tracer
             app.logger = logger
 
             return app
-    except Exception as e:
-        app.tracer = tracer
-        app.logger = logger
-        logger.error(f"An error occurred in create_app: {str(e)}")
-        raise e
+    except Exception as ex:
+        if app is not None:
+            app.tracer = tracer
+            app.logger = logger
+            error_message = f"An error occurred in create_app: {str(ex)}"
+            exc_info = sys.exc_info()
+            logger_singleton.error_with_exception(error_message, exc_info)
+        raise
```

### Comparing `data_ecosystem_flask-202306.0.34/data_ecosystem_flask/install.py` & `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/install.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.34/data_ecosystem_flask/manifest.json` & `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.34/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,16 @@
 certifi==2023.5.7 ; python_version >= "3.9" and python_version < "4.0"
 cffi==1.15.1 ; python_version >= "3.9" and python_version < "4.0"
 chardet==5.1.0 ; python_version >= "3.9" and python_version < "4.0"
 charset-normalizer==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.9" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and (platform_system == "Windows" or sys_platform == "win32")
 comm==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
-coverage[toml]==7.2.7 ; python_version >= "3.9" and python_version < "4.0"
 cryptography==41.0.1 ; python_version >= "3.9" and python_version < "4.0"
-data-ecosystem-services==202306.0.26 ; python_version >= "3.9" and python_version < "4.0"
+data-ecosystem-services==202306.0.41 ; python_version >= "3.9" and python_version < "4.0"
 ddlparse==1.10.0 ; python_version >= "3.9" and python_version < "4.0"
 debugpy==1.6.7 ; python_version >= "3.9" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.9" and python_version < "4.0"
 defusedxml==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
 deprecated==1.2.14 ; python_version >= "3.9" and python_version < "4.0"
 docutils==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 entrypoints==0.4 ; python_version >= "3.9" and python_version < "4.0"
@@ -59,41 +58,41 @@
 flake8==4.0.1 ; python_version >= "3.9" and python_version < "4.0"
 flask-restful==0.3.10 ; python_version >= "3.9" and python_version < "4.0"
 flask-restx==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
 flask==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 fqdn==1.5.1 ; python_version >= "3.9" and python_version < "4"
 fsspec==2023.6.0 ; python_version >= "3.9" and python_version < "4.0"
 google-api-core==2.11.1 ; python_version >= "3.9" and python_version < "4.0"
-google-auth==2.20.0 ; python_version >= "3.9" and python_version < "4.0"
+google-auth==2.21.0 ; python_version >= "3.9" and python_version < "4.0"
 googleapis-common-protos==1.59.1 ; python_version >= "3.9" and python_version < "4.0"
 html2text==2020.1.16 ; python_version >= "3.9" and python_version < "4.0"
-humanize==4.6.0 ; python_version >= "3.9" and python_version < "4.0"
+humanize==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.9" and python_version < "4.0"
 imagesize==1.4.1 ; python_version >= "3.9" and python_version < "4.0"
 importlib-metadata==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
 importlib-resources==5.12.0 ; python_version >= "3.9" and python_version < "4.0"
 iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
 ipykernel==6.23.3 ; python_version >= "3.9" and python_version < "4.0"
 ipython-genutils==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 ipython==8.14.0 ; python_version >= "3.9" and python_version < "4.0"
 isodate==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
 isoduration==20.11.0 ; python_version >= "3.9" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.9" and python_version < "4.0"
 jedi==0.18.2 ; python_version >= "3.9" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
 jmespath==0.10.0 ; python_version >= "3.9" and python_version < "4.0"
-joblib==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
+joblib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 jsonpointer==2.4 ; python_version >= "3.9" and python_version < "4.0"
 jsonschema==4.17.3 ; python_version >= "3.9" and python_version < "4.0"
 jsonschema[format-nongpl]==4.17.3 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-client==8.3.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-core==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-events==0.6.3 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-server-terminals==0.4.4 ; python_version >= "3.9" and python_version < "4.0"
-jupyter-server==2.6.0 ; python_version >= "3.9" and python_version < "4.0"
+jupyter-server==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyterlab-pygments==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
 lazy-object-proxy==1.9.0 ; python_version >= "3.9" and python_version < "4.0"
 lxml==4.9.2 ; python_version >= "3.9" and python_version < "4.0"
 markdown-it-py==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
 markdown==3.4.3 ; python_version >= "3.9" and python_version < "4.0"
 markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0"
 matplotlib-inline==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
@@ -123,15 +122,15 @@
 opentelemetry-instrumentation-wsgi==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-sdk==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-semantic-conventions==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-util-http==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 overrides==7.3.1 ; python_version >= "3.9" and python_version < "4.0"
 packaging==23.1 ; python_version >= "3.9" and python_version < "4.0"
-pandas==2.0.2 ; python_version >= "3.9" and python_version < "4.0"
+pandas==2.0.3 ; python_version >= "3.9" and python_version < "4.0"
 pandocfilters==1.5.0 ; python_version >= "3.9" and python_version < "4.0"
 parso==0.8.3 ; python_version >= "3.9" and python_version < "4.0"
 pathlib==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
 pbr==5.11.1 ; python_version >= "3.9" and python_version < "4.0"
 pexpect==4.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32"
 pickleshare==0.7.5 ; python_version >= "3.9" and python_version < "4.0"
 pins==0.8.1 ; python_version >= "3.9" and python_version < "4.0"
@@ -155,15 +154,14 @@
 pyflakes==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 pygments==2.15.1 ; python_version >= "3.9" and python_version < "4.0"
 pyjwt==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 pyjwt[crypto]==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 pyparsing==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
 pyreadstat==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
 pyrsistent==0.19.3 ; python_version >= "3.9" and python_version < "4.0"
-pytest-cov==4.1.0 ; python_version >= "3.9" and python_version < "4.0"
 pytest==7.4.0 ; python_version >= "3.9" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0"
 python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 python-json-logger==2.0.7 ; python_version >= "3.9" and python_version < "4.0"
 pytz==2023.3 ; python_version >= "3.9" and python_version < "4.0"
 pywin32==306 ; python_version >= "3.9" and (sys_platform == "win32" or platform_system == "Windows") and python_version < "4.0" and (platform_python_implementation != "PyPy" or platform_system == "Windows")
 pywinpty==2.0.10 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
@@ -172,15 +170,15 @@
 requests-oauthlib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0"
 rfc3339-validator==0.1.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3986-validator==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
 rich==13.4.2 ; python_version >= "3.9" and python_version < "4.0"
 rsa==4.9 ; python_version >= "3.9" and python_version < "4"
 rsconnect-jupyter==1.8.0 ; python_version >= "3.9" and python_version < "4.0"
-rsconnect-python==1.17.1 ; python_version >= "3.9" and python_version < "4.0"
+rsconnect-python==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 rsconnect==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
 s3transfer==0.5.2 ; python_version >= "3.9" and python_version < "4.0"
 semver==2.13.0 ; python_version >= "3.9" and python_version < "4.0"
 send2trash==1.8.2 ; python_version >= "3.9" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.9" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0"
 sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
@@ -208,15 +206,15 @@
 testresources==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tinycss2==1.2.1 ; python_version >= "3.9" and python_version < "4.0"
 toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tornado==6.3.2 ; python_version >= "3.9" and python_version < "4.0"
 traitlets==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
 tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
-typing-extensions==4.6.3 ; python_version >= "3.9" and python_version < "4.0"
+typing-extensions==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 tzdata==2023.3 ; python_version >= "3.9" and python_version < "4.0"
 unify==0.5 ; python_version >= "3.9" and python_version < "4.0"
 untokenize==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
 uri-template==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
 urllib3==1.26.16 ; python_version >= "3.9" and python_version < "4.0"
 wcwidth==0.2.6 ; python_version >= "3.9" and python_version < "4.0"
 webcolors==1.13 ; python_version >= "3.9" and python_version < "4.0"
```

### Comparing `data_ecosystem_flask-202306.0.34/data_ecosystem_flask/templates/log_file.html` & `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/log_file.html`

 * *Files 14% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     <!-- jQuery, DataTables JS, Bootstrap JS -->
     <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
     <script src="https://cdn.datatables.net/1.10.23/js/jquery.dataTables.min.js"></script>
     <script src="https://cdn.datatables.net/1.10.23/js/dataTables.bootstrap4.min.js"></script>
     <!-- DataTables initialization -->
     <script>
       $(document).ready(function () {
-        var table = $("#logTable").DataTable();
+        var table = $("#logTable").DataTable({ order: [[0, "desc"]] });
 
         // Add a filter for log level
         $("#logLevelFilter").on("change", function () {
-          table.column(3).search($(this).val()).draw();
+          table.column(5).search($(this).val()).draw();
         });
       });
     </script>
   </head>
   <body>
     <div class="container">
       <h2 class="mt-4">Log File</h2>
@@ -51,29 +51,33 @@
         </select>
       </div>
 
       <table id="logTable" class="table table-striped table-theme-blue">
         <thead>
           <tr>
             <th scope="col">Date</th>
-            <th scope="col">Time</th>
+            <th scope="col">Service</th>
+            <th scope="col">Module</th>
             <th scope="col">Line Number</th>
             <th scope="col">Level</th>
             <th scope="col">Message</th>
           </tr>
         </thead>
         <tbody>
           {% for entry in entries %}
           <tr>
-            <td>{{ entry[0]}}</td>
-            <td>{{ entry[1]}}</td>
-            <td>{{ entry[2]}}</td>
-            <td>{{ entry[3]}}</td>
-            <td class="text-{{ entry[4].lower()}}">
-              {{ entry[4]}} {{ ' '.join(entry[5:])}}
+            <td>{{ entry[0] if entry|length > 0 else 'N/A'}}</td>
+            <td>{{ entry[1] if entry|length > 1 else 'N/A'}}</td>
+            <td>{{ entry[2] if entry|length > 2 else 'N/A'}}</td>
+            <td>{{ entry[3] if entry|length > 3 else 'N/A'}}</td>
+            <td>{{ entry[4] if entry|length > 4 else 'N/A'}}</td>
+            <td
+              class="text-{{ entry[4].lower() if entry|length > 4 else 'info'}}"
+            >
+              {{ entry[5] if entry|length > 5 else 'N/A'}}
             </td>
           </tr>
           {% endfor %}
         </tbody>
       </table>
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 
 
 
 
 ***** Log File *****
 Filter by Log Level: [One of: All/INFO/WARNING/ERROR]
-Date          Time          Line Number   Level         Message
-{{ entry[0]}} {{ entry[1]}} {{ entry[2]}} {{ entry[3]}} {{ entry[4]}} {{ '
-                                                        '.join(entry[5:])}}
+Date         Service      Module       Line Number  Level        Message
+{{ entry[0]  {{ entry[1]  {{ entry[2]  {{ entry[3]  {{ entry[4]
+if           if           if           if           if           {{ entry[5] if
+entry|length entry|length entry|length entry|length entry|length entry|length >
+> 0 else 'N/ > 1 else 'N/ > 2 else 'N/ > 3 else 'N/ > 4 else 'N/ 5 else 'N/A'}}
+A'}}         A'}}         A'}}         A'}}         A'}}
```

### Comparing `data_ecosystem_flask-202306.0.34/license.md` & `data_ecosystem_flask-202307.0.2/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.34/pyproject.toml` & `data_ecosystem_flask-202307.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "data_ecosystem_flask"
 authors = [{name="John Bowyer", email="zfi4@cdc.gov" }]
 description = "Data Ecosystem Flask (PADE)  - Python "
 readme = "readme.md"
 requires-python = ">=3.9,<4.0"
-version = "202306.0.26"
+version = "202307.0.1"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9"
 ]
 
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202306.0.34"
+version="202307.0.2"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
@@ -35,14 +35,15 @@
     "Programming Language :: Python :: 3.9"
 ]
 include = [ "readme.md",
             "license.md",
             "setup.cfg",
             "setup.py",
             "pyproject.toml",
+            "data_ecosystem_flask/data_ecosystem_flask/**/*.py",
             "data_ecosystem_flask/**/*.py"]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 flask = "^2.0.0"
 six = "^1.16.0"
@@ -66,22 +67,22 @@
 data-ecosystem-services = "^202306.0.26"
 certifi = "2023.5.7"
  
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
-flaskapp = "app:app"
+flaskapp = "data_ecosystem_flask.app:app"
 
 
 [tool.pytest.ini_options]
 minversion="6.0"
 addopts="-ra -q --cov --cov-report html --cov-report term-missing --cov-fail-under 15"
 testpaths=[
-    "pade_python/tests"
+    "data_ecosystem_services/tests"
 ]
 
 [tool.mypy]
 warn_unused_configs=true
 namespace_packages=true
 explicit_package_bases=true
 ignore_missing_imports=true
```

### Comparing `data_ecosystem_flask-202306.0.34/readme.md` & `data_ecosystem_flask-202307.0.2/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# PADE-Flask API Application
+# pade_flask API Application
 
 - Point of contact: [John Bowyer](mailto:zfi4@cdc.gov)
 - Organizational unit: OCIO
 - Related projects: EDC
 - Related investments:  Pending Public Release
 - Governance status: Pending Public Release
-- Program official:  [Erik Knudsen](mailto:egk1@cdc.gov)
+- Program official:  [Erik Knudsen](mailto:knu1@cdc.gov)
 
-## PADE-Flask API Overview
+## pade_flask API Overview
 
 A Python Rest API with functionality to support a react client application and interface/extract information from a Synapse Serverless Database and Alation.
 
 ## Geting Started
 
 ### Clone the Flask App App Locally
 
@@ -43,40 +43,40 @@
 ```
 
 ### Run the Flask App Locally
 
 #### Run the Flask App Locally on POSIT  (Primary)
 
 ```sh
-cd pade-flask/data_ecosystem_flask
+cd pade_flask/data_ecosystem_flask
 workon OCIO_PADE_DEV
 make flask-run-posit-dev
 ```
 
 #### View Logs Locally
 
 Where zfi4=your_alias
 
-/r-share/home/zfi4/.virtualenvs/OCIO_PADE_DEV/share/.pade_python_services_errors.log
+/r-share/home/zfi4/.virtualenvs/OCIO_PADE_DEV/share/.data_ecosystem_services_services_errors.log
 
 #### SetUp Deployment Env
 
 ``` sh
 /opt/python/3.9.9/bin/python3 -m venv .venv-3.9.9
 source .venv-3.9.9/bin/activate
-cd ~/data-ecosystem-services/pade-flask/data_ecosystem_flask
+cd ~/data-ecosystem-services/pade_flask/data_ecosystem_flask
 poetry lock
 poetry install
 poetry export -f requirements.txt --output requirements.txt --without-hashes 
 ```
 
 #### Deploy the Flask App on POSIT (Primary)
 
 ``` sh
-cd ~/data-ecosystem-services/pade-flask/data_ecosystem_flask
+cd ~/data-ecosystem-services/pade_flask/data_ecosystem_flask
 workon OCIO_PADE_DEV
 make posit-deploy
 ```
 
 #### Run your Flask App Locally on Ubuntu or WSL
 
 Steps to test web site
@@ -84,27 +84,25 @@
 - Next go to posit exension in VS Code
 - Click the name of proxied server
 - Launch server - if you receive 404 you may need to add /swagger to proxied url
 - Test web site
 
 #### Run your Flask App Locally on Ubuntu or WSL
 
-
 ```sh
-cd pade-flask/data_ecosystem_flask
+cd pade_flask/data_ecosystem_flask
 workon OCIO_PADE_DEV
 make flask-run-wsl
 ```
 
 Browse the Application at http://127.0.0.1:5000/download-excel
 
-
 ## Debug
 
-nano ~/.virtualenvs/OCIO_PADE_DEV/share/pade_python_services_logging.txt
+nano ~/.virtualenvs/OCIO_PADE_DEV/share/data_ecosystem_services_services_logging.txt
 
 ## Installation
 
 ### Check if Python is installed
 
 Run in bash or powershell
 
@@ -182,15 +180,15 @@
 ```
 
 ### To Add a Library to Setup on All Platforms
 
 1. Go to project directory
 
 ```sh
-cd pade-flask/data_ecosystem_flask
+cd pade_flask/data_ecosystem_flask
 ```
 
 2. Open Terminal and workon virtual environment
 
 ```sh
 workon OCIO_PADE_DEV
 ```
@@ -489,23 +487,23 @@
 This will use the cert.pem and key.pem files to set up SSL for your Flask application.
 
 3. Run your Flask app:
 
 Run your Flask app with the following command:
 
 ```bash
-cd pade-flask/data_ecosystem_flask
+cd pade_flask/data_ecosystem_flask
 workon OCIO_PADE_DEV
 make run
 ```
 
 if you receive a port conflict error 
 
 ```bash
-cd pade-flask/data_ecosystem_flask
+cd pade_flask/data_ecosystem_flask
 make kill
 make run~
 ```
 
 This will start your Flask app with SSL enabled.
 
 Access your Flask app over HTTPS:
@@ -519,15 +517,15 @@
 1. Select Interpreter
 2. Select ctrl+shift+ps
 3. Select Python: Select Interpreter
 4. Select Python 3.9.7 64-bit ('OCIO_PADE_DEV': venv)
  
 ### Trouble Shooting
 
-To trouble shoot the application, see the [Trouble Shooting](../pade_python/readme.md) section of the PADE Python project.
+To trouble shoot the application, see the [Trouble Shooting](../data_ecosystem_services/readme.md) section of the PADE Python project.
 
 ### Check Cert
 
 openssl x509 -in custom-ca.pem -text
 openssl x509 -in cert.pem -text
 
 ### Export Cert list
```

### Comparing `data_ecosystem_flask-202306.0.34/PKG-INFO` & `data_ecosystem_flask-202307.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202306.0.34
+Version: 202307.0.2
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

