# Comparing `tmp/azureml-assets-1.5.1.tar.gz` & `tmp/azureml-assets-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.5.1.tar", last modified: Tue Jul 11 18:59:13 2023, max compression
+gzip compressed data, was "azureml-assets-1.5.2.tar", last modified: Mon Jul 17 14:36:55 2023, max compression
```

## Comparing `azureml-assets-1.5.1.tar` & `azureml-assets-1.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.134351 azureml-assets-1.5.1/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.134351 azureml-assets-1.5.1/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17053 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17280 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-11 18:59:13.000000 azureml-assets-1.5.1/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-11 18:59:13.138351 azureml-assets-1.5.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-11 18:58:34.000000 azureml-assets-1.5.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.732984 azureml-assets-1.5.2/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.736984 azureml-assets-1.5.2/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.740984 azureml-assets-1.5.2/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17109 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.740984 azureml-assets-1.5.2/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17280 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-17 14:36:55.748984 azureml-assets-1.5.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/setup.py
```

### Comparing `azureml-assets-1.5.1/PKG-INFO` & `azureml-assets-1.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.5.1
+Version: 1.5.2
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.5.1/azureml/assets/__init__.py` & `azureml-assets-1.5.2/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/asset_utils.py` & `azureml-assets-1.5.2/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/config.py` & `azureml-assets-1.5.2/azureml/assets/config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/copy_assets.py` & `azureml-assets-1.5.2/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/deployment_config.py` & `azureml-assets-1.5.2/azureml/assets/deployment_config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/environment/build.py` & `azureml-assets-1.5.2/azureml/assets/environment/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,138 +27,130 @@
 TRIVY_TIMEOUT = "15m0s"
 SUCCESS_COUNT = "success_count"
 FAILED_COUNT = "failed_count"
 COUNTERS = [SUCCESS_COUNT, FAILED_COUNT]
 
 
 def create_acr_task(image_name: str,
-                    build_context_dir: Path,
                     dockerfile: str,
+                    os: assets.Os,
                     task_filename: str,
                     test_command: str = None,
                     push: bool = False,
-                    trivy_url: str = None) -> Path:
+                    trivy_url: str = None):
     """Create ACR build task file.
 
     Args:
         image_name (str): Image name.
-        build_context_dir (Path): Build context directory.
         dockerfile (str): Dockerfile name.
+        os (assets.Os): Operating system of the image.
         task_filename (str): File to which the task will be written.
         test_command (str, optional): Command used to test the image. Defaults to None.
         push (bool, optional): Push the image to the ACR. Defaults to False.
         trivy_url (str, optional): URL to download Trivy for vulnerability scanning. Defaults to None.
-
-    Returns:
-        Path: The task file.
     """
     # Start task with just the build step
     task = {
         'version': 'v1.1.0',
         'stepTimeout': BUILD_STEP_TIMEOUT_SECONDS,
         'steps': [{
             'id': "build",
             'build': f"-t $Registry/{image_name} -f {dockerfile} ."
         }]}
 
-    # Add output conda export command
+    # Add command to output packages
+    if os is assets.Os.LINUX:
+        # Quoted string required to handle && and ||
+        cmd = r'/bin/sh -c "[ -n \"\$CONDA_DEFAULT_ENV\" ] && conda env export || pip freeze"'
+    else:
+        # Requires Windows batch
+        cmd = r'cmd /C "if defined CONDA_DEFAULT_ENV (conda env export) else (pip freeze)"'
     task['steps'].append({
-        'id': 'conda_export',
-        'cmd': f"$Registry/{image_name} conda env export",
+        'id': "package_export",
+        'cmd': f"$Registry/{image_name} {cmd}",
         'ignoreErrors': True
     })
 
     # Add test command if provided
     if test_command:
         task['steps'].append({
-            'id': 'test',
+            'id': "test",
             'cmd': f"$Registry/{image_name} {test_command}"
         })
 
-        if trivy_url is not None:
+    # Add vulnerability scanning step if requested
+    if trivy_url is not None:
+        if os is assets.Os.LINUX:
             task['steps'].append({
-                'id': 'scan',
+                'id': "scan",
                 'stepTimeout': SCAN_STEP_TIMEOUT_SECONDS,
                 'cmd': f"aquasec/trivy -q --timeout {TRIVY_TIMEOUT} image --scanners vuln --ignore-unfixed "
                        f"$Registry/{image_name}",
                 'ignoreErrors': True,
                 'privileged': True
             })
+        else:
+            logger.log_warning(f"Skipped vulnerability scan for Windows image {image_name} - not supported")
 
     # Add push step if requested
     if push:
         task['steps'].append({
-            'id': 'push',
+            'id': "push",
             'push': [f"$Registry/{image_name}"]
         })
 
     # Write YAML file to disk
-    task_file = build_context_dir / task_filename
-    with open(task_file, "w") as f:
+    with open(task_filename, "w") as f:
         yaml = YAML()
         yaml.default_flow_style = False
         YAML().dump(task, f)
 
-    return task_file
-
 
 def build_image(asset_config: assets.AssetConfig,
+                env_config: assets.EnvironmentConfig,
                 image_name: str,
-                build_context_dir: Path,
-                dockerfile: str,
                 build_log: Path,
-                build_os: str = None,
                 resource_group: str = None,
                 registry: str = None,
                 test_command: str = None,
                 push: bool = False,
                 trivy_url: str = None) -> Tuple[assets.AssetConfig, int, str]:
     """Build a Docker image locally or via ACR task.
 
     Args:
         asset_config (assets.AssetConfig): Asset config.
+        env_config (assets.EnvironmentConfig): Environment config.
         image_name (str): Image name.
-        build_context_dir (Path): Build context directory.
-        dockerfile (str): Dockerfile name.
         build_log (Path): File to which the build log will be written.
-        build_os (str, optional): Operating system used to build the image on ACR. Defaults to None.
         resource_group (str, optional): Resource group of the ACR. Defaults to None.
         registry (str, optional): ACR name. Defaults to None.
         test_command (str, optional): Command used to test the image. Defaults to None.
         push (bool, optional): Push the image to the ACR. Defaults to False.
         trivy_url (str, optional): URL to download Trivy for vulnerability scanning. Defaults to None.
 
     Returns:
         Tuple[assets.AssetConfig, int, str]: Asset config, return code, and contents of stdout.
     """
     logger.print(f"Building image for {asset_config.name}")
     start = timer()
     with tempfile.TemporaryDirectory() as temp_dir:
         if registry is not None:
-            # Build on ACR
-            cmd = ["az", "acr"]
-            common_args = ["-g", resource_group, "-r", registry, "--platform", build_os]
-            if not test_command and push:
-                # Simple build and push
-                cmd.append("build")
-                cmd.extend(common_args)
-                cmd.extend(["--file", dockerfile, "--image", image_name, "."])
-            else:
-                # Use ACR task from build context in temp dir
-                temp_dir_path = Path(temp_dir)
-                shutil.copytree(build_context_dir, temp_dir_path, dirs_exist_ok=True)
-                build_context_dir = temp_dir_path
-                create_acr_task(image_name, build_context_dir, dockerfile, TASK_FILENAME, test_command,
-                                push, trivy_url)
-                cmd.append("run")
-                cmd.extend(common_args)
-                cmd.extend(["-f", TASK_FILENAME, "."])
+            # Build via ACR task
+            temp_dir_path = Path(temp_dir)
+            shutil.copytree(env_config.context_dir_with_path, temp_dir_path, dirs_exist_ok=True)
+            build_context_dir = temp_dir_path
+            create_acr_task(image_name=image_name, dockerfile=env_config.dockerfile,
+                            os=env_config.os, task_filename=build_context_dir / TASK_FILENAME,
+                            test_command=test_command, push=push, trivy_url=trivy_url)
+            cmd = ["az", "acr", "run", "-g", resource_group, "-r", registry, "--platform", env_config.os.value,
+                   "-f", TASK_FILENAME, "."]
         else:
             # Build locally
-            cmd = ["docker", "build", "--file", dockerfile, "--progress", "plain", "--tag", image_name, "."]
+            build_context_dir = env_config.context_dir_with_path
+            cmd = ["docker", "build", "--file", env_config.dockerfile, "--progress", "plain", "--tag", image_name, "."]
         p = run(cmd,
                 cwd=build_context_dir,
                 stdout=PIPE,
                 stderr=STDOUT)
     end = timer()
     logger.print(f"Image for {asset_config.name} built in {timedelta(seconds=end-start)}")
     os.makedirs(build_log.parent, exist_ok=True)
@@ -191,15 +183,15 @@
                  asset_config_filename: str,
                  output_directory: Path,
                  build_logs_dir: Path,
                  pin_versions: bool,
                  max_parallel: int,
                  changed_files: List[Path],
                  tag_with_version: bool,
-                 os_to_build: str = None,
+                 os_to_build: assets.Os = None,
                  resource_group: str = None,
                  registry: str = None,
                  test_command: str = None,
                  push: bool = False,
                  use_version_dirs: bool = False,
                  trivy_url: str = None) -> bool:
     """Build Docker images in parallel, either locally or via ACR.
@@ -209,15 +201,15 @@
         asset_config_filename (str): Asset config filename to search for.
         output_directory (Path): Directory to which assets successfully built will be copied.
         build_logs_dir (Path): Directory to receive build logs.
         pin_versions (bool): Pin image versions.
         max_parallel (int): Maximum number of images to build in parallel.
         changed_files (List[Path]): List of changed files, used to filter environments.
         tag_with_version (bool): Tag image with asset version.
-        os_to_build (str, optional): Operating system to build on via ACR. Defaults to None.
+        os_to_build (assets.Os, optional): Operating system to build on via ACR. Defaults to None.
         resource_group (str, optional): Resource group name for ACR builds. Defaults to None.
         registry (str, optional): ACR name. Defaults to None.
         test_command (str, optional): Command used to test images. Defaults to None.
         push (bool, optional): Push images to ACR. Defaults to False.
         use_version_dirs (bool, optional): Use version directories for output. Defaults to False.
         trivy_url (str, optional): URL to download Trivy for vulnerability scanning. Defaults to None.
 
@@ -229,17 +221,17 @@
         # Find environments under image root directories
         futures = []
         for asset_config in util.find_assets(input_dirs, asset_config_filename, assets.AssetType.ENVIRONMENT,
                                              changed_files):
             env_config = asset_config.extra_config_as_object()
 
             # Filter by OS
-            if os_to_build and env_config.os.value != os_to_build:
+            if os_to_build and env_config.os != os_to_build:
                 logger.print(f"Skipping build of image for {asset_config.name}: "
-                             f"Operating system {env_config.os.value} != {os_to_build}")
+                             f"Operating system {env_config.os.value} != {os_to_build.value}")
                 continue
 
             # Pin versions
             if pin_versions:
                 try:
                     assets.pin_env_files(env_config)
                 except Exception as e:
@@ -267,18 +259,18 @@
                 version = asset_config.version
                 image_name = env_config.get_image_name_with_tag(version)
             else:
                 image_name = env_config.image_name
 
             # Start building image
             build_log = build_logs_dir / f"{asset_config.name}.log"
-            futures.append(pool.submit(build_image, asset_config, image_name,
-                                       env_config.context_dir_with_path, env_config.dockerfile, build_log,
-                                       env_config.os.value, resource_group, registry, test_command,
-                                       push_this_image, trivy_url))
+            futures.append(pool.submit(build_image, asset_config=asset_config, env_config=env_config,
+                                       image_name=image_name, build_log=build_log, resource_group=resource_group,
+                                       registry=registry, test_command=test_command, push=push_this_image,
+                                       trivy_url=trivy_url))
 
         # Wait for builds to complete
         for future in as_completed(futures):
             (asset_config, return_code, output) = future.result()
             logger.start_group(f"{asset_config.name} build log")
             logger.print(output)
             logger.end_group()
@@ -344,28 +336,29 @@
     if args.test_command and not (args.registry and args.resource_group):
         parser.error("--test-command requires both --registry and --resource-group")
     if args.push and not (args.registry and args.resource_group):
         parser.error("--push requires both --registry and --resource-group")
     if args.use_version_dirs and not args.output_directory:
         parser.error("--use-version-dirs requires --output-directory")
 
-    # Convert comma-separated values to lists
+    # Reformat arg values
     input_dirs = [Path(d) for d in args.input_dirs.split(",")]
     changed_files = [Path(f) for f in args.changed_files.split(",")] if args.changed_files else []
+    os_to_build = assets.Os(args.os_to_build) if args.os_to_build else None
 
     # Build images
     success = build_images(input_dirs=input_dirs,
                            asset_config_filename=args.asset_config_filename,
                            output_directory=args.output_directory,
                            build_logs_dir=args.build_logs_dir,
                            pin_versions=args.pin_versions,
                            max_parallel=args.max_parallel,
                            changed_files=changed_files,
                            tag_with_version=args.tag_with_version,
-                           os_to_build=args.os_to_build,
+                           os_to_build=os_to_build,
                            resource_group=args.resource_group,
                            registry=args.registry,
                            test_command=args.test_command,
                            push=args.push,
                            use_version_dirs=args.use_version_dirs,
                            trivy_url=args.trivy_url)
     if not success:
```

### Comparing `azureml-assets-1.5.1/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.5.2/azureml/assets/environment/pin_image_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.5.2/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.5.2/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.5.2/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.5.2/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/model/utils.py` & `azureml-assets-1.5.2/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/tag_released_assets.py` & `azureml-assets-1.5.2/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/update_assets.py` & `azureml-assets-1.5.2/azureml/assets/update_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/update_spec.py` & `azureml-assets-1.5.2/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/util/__init__.py` & `azureml-assets-1.5.2/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/util/logger.py` & `azureml-assets-1.5.2/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/util/template.py` & `azureml-assets-1.5.2/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/util/util.py` & `azureml-assets-1.5.2/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml/assets/validate_assets.py` & `azureml-assets-1.5.2/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.5.2/azureml_assets.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.5.1
+Version: 1.5.2
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.5.1/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.5.2/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.1/setup.py` & `azureml-assets-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.5.1",
+   version="1.5.2",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

