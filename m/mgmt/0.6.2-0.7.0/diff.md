# Comparing `tmp/mgmt-0.6.2.tar.gz` & `tmp/mgmt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgmt-0.6.2.tar", max compression
+gzip compressed data, was "mgmt-0.7.0.tar", max compression
```

## Comparing `mgmt-0.6.2.tar` & `mgmt-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-09 07:20:01.948364 mgmt-0.6.2/LICENSE
--rw-r--r--   0        0        0     4773 2023-07-09 07:20:01.948364 mgmt-0.6.2/README.md
--rw-r--r--   0        0        0      553 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/__init__.py
--rw-r--r--   0        0        0       44 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/__main__.py
--rw-r--r--   0        0        0     6935 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/app.py
--rw-r--r--   0        0        0     6653 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/aws.py
--rw-r--r--   0        0        0     1762 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/config.py
--rw-r--r--   0        0        0     4012 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/files.py
--rw-r--r--   0        0        0     1744 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/log.py
--rw-r--r--   0        0        0      338 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/utils.py
--rw-r--r--   0        0        0     2304 2023-07-09 07:20:01.948364 mgmt-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 mgmt-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-17 02:33:10.918450 mgmt-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4773 2023-07-17 02:33:10.918450 mgmt-0.7.0/README.md
+-rw-r--r--   0        0        0      553 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/__main__.py
+-rw-r--r--   0        0        0     7759 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/app.py
+-rw-r--r--   0        0        0     6839 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/aws.py
+-rw-r--r--   0        0        0     2315 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/config.py
+-rw-r--r--   0        0        0     4287 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/files.py
+-rw-r--r--   0        0        0     1744 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/log.py
+-rw-r--r--   0        0        0      338 2023-07-17 02:33:10.918450 mgmt-0.7.0/mgmt/utils.py
+-rw-r--r--   0        0        0     2304 2023-07-17 02:33:10.918450 mgmt-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 mgmt-0.7.0/PKG-INFO
```

### Comparing `mgmt-0.6.2/LICENSE` & `mgmt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.2/README.md` & `mgmt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.2/mgmt/__init__.py` & `mgmt-0.7.0/mgmt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .app import entry_point as cli  # noqa: F401
 
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 __docformat__ = "restructuredtext"
 
 # module level doc-string
 # https://stackoverflow.com/questions/3898572/what-are-the-most-common-python-docstring-formats
 __doc__ = """
 mgmt - an intuitive cli wrapper around boto3 to search and manage media assets
 =====================================================================
```

### Comparing `mgmt-0.6.2/mgmt/app.py` & `mgmt-0.7.0/mgmt/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 import typer
 from rich import box
 from typer import echo
 from rich.table import Table
 from rich.console import Console
 
 from mgmt.aws import AwsStorageMgmt
-from mgmt.log import Log
 from mgmt.files import FileManager
 from mgmt.utils import check_selection
 from mgmt.config import Config
 
 app = typer.Typer(add_completion=False)
 aws = AwsStorageMgmt()
-logger = Log(debug=False)
-file_mgmt = FileManager()
 
 
 @app.command()
 def upload(filename: str, compression: Optional[str] = "gzip") -> None:
     """
     Uploads the specified file to S3
 
     Args:
-        filename (str): The name of the file or directory to upload. Use 'all' to upload all files in the directory.
+        filename (str): The name of the file or directory to upload.
+            Use 'all' to upload all files in the directory.
         compression (Optional[str]): The compression algorithm to use. Defaults to 'gzip'.
     """
     target = filename
     cwd = Path(".").resolve()
     target_path = cwd / target
     files_created = []
     skip_files = [".DS_Store"]
@@ -50,78 +48,83 @@
             echo("file found, compressing...")
             echo(str(target))
             files_created.append(aws.upload_target(target_path, compression))
         else:
             echo("invalid file or directory")
             return False
     except Exception as e:
-        logger.error(f"An error occurred while uploading: {e}")
+        echo(f"An error occurred while uploading: {e}", err=True)
     finally:
         if files_created:
             for file in files_created:
                 os.remove(file)
     return
 
 
 @app.command()
-def search(keyword: str, location: Optional[str] = "global") -> None:
+def search(keyword: str) -> None:
     """
     Searches for files that contain the specified keyword in their names
 
     Args:
-        keyword (str): The keyword to search for in file names.
-        location (Optional[str]): The location to search in. Defaults to 'global'.
+        keyword (str): The keyword to search for in file names
     """
+    location = "global"
+    file_mgmt = FileManager()
     local_files, s3_keys = aws.get_files(location=location)
-
     echo(f"\nSearching `{location}` for keyword `{keyword}`...")
     local_matches = [file for file in local_files if file_mgmt.keyword_in_string(keyword, file)]
     s3_matches = [file for file in s3_keys if file_mgmt.keyword_in_string(keyword, file)]
 
     if len(local_matches + s3_matches) >= 1:
         echo("at least one match found\n")
         echo("Local File Matches")
         echo("\n".join(local_matches))
-
         console = Console()
         table = Table(title="AWS S3 Search Matches", box=box.SIMPLE)
         table.add_column("Option #", style="cyan", no_wrap=True)
         table.add_column("Storage Tier", style="green")
         table.add_column("Last Modified")
         table.add_column("Object Key", style="magenta")
         table.add_column("Restored Status")
         doptions = {}
+
         for i, file_name in enumerate(s3_matches):
             try:
                 resp = aws.get_obj_head(file_name)
                 storage_class = resp.get("StorageClass", "STANDARD")
                 last_modified = resp.get("LastModified", "")
                 restored_status = resp.get("Restore")
+
                 if restored_status:
                     restored_status = str(restored_status).split("expiry-date=")[-1].replace('"', "")
+
                 table.add_row(str(i), storage_class, str(last_modified).split(" ")[0], file_name, str(restored_status))
                 doptions[i] = file_name
             except Exception as e:
-                logger.error(f"An error occurred while getting metadata: {e}")
+                echo(f"An error occurred while getting metadata: {e}", err=True)
 
         console.print(table)
+
         if not typer.confirm("Download?", default=False):
             echo("Aborted.")
         else:
             resp = typer.prompt("Which file? [option #]", type=int)
+
             if check_selection(resp, list(doptions)):
-                aws.download_file(object_name=doptions[resp])
+                aws.download(object_name=doptions[resp])
                 return
             else:
                 return
 
         if not typer.confirm("Check Status?", default=False):
             echo("Aborted.")
         else:
             resp = typer.prompt("Which file? [option #]", type=int)
+
             if check_selection(resp, list(doptions)):
                 aws.get_obj_head(object_name=doptions[resp])
                 echo(json.dumps(aws.obj_head, indent=4, sort_keys=True, default=str))
                 return
             else:
                 return
     return
@@ -133,15 +136,15 @@
     Downloads the specified file from S3
 
     Args:
         filename (str): The name of the file to download.
         bucket_name (Optional[str]): The name of the bucket from which to download the file. If not provided, the default bucket is used.
     """
     echo(f"Downloading {filename} from S3...")
-    aws.download_file(object_name=filename, bucket_name=bucket_name)
+    aws.download(object_name=filename, bucket_name=bucket_name)
     return
 
 
 @app.command()
 def status(filename: str) -> None:
     """
     Retrieves and prints the metadata of the specified file
@@ -160,52 +163,97 @@
     Deletes the specified file from S3; requires confirmation
 
     Args:
         filename (str): The name of the file to delete.
     """
     aws.get_obj_head(object_name=filename)
     echo(json.dumps(aws.obj_head, indent=4, sort_keys=True, default=str))
+
     if not typer.confirm("Confirm deletion?", default=False):
         echo("Aborted.")
         return
     else:
         try:
             aws.delete_file(filename)
             echo(f"{filename} successfully deleted from S3")
         except Exception as e:
-            logger.error(f"An error occurred while deleting {filename}: {e}")
+            echo(f"An error occurred while deleting {filename}: {e}", err=True)
     return
 
 
 @app.command()
 def ls(location: Optional[str] = "global") -> None:
     """
     Lists the files in the specified location
 
     Args:
-        location (Optional[str]): The location to list files in. Defaults to 'global'.
-        bucket_name (Optional[str]): The name of the bucket to list files in. If not provided, the default bucket is used.
+        location (Optional[str]): The location to list files in: 'local', 'gloabl', or 's3'.
+        Defaults to 'global'.
     """
-    local_files, s3_keys = aws.get_files(location=location)
-    obj_list = local_files + s3_keys
-    for obj in obj_list:
+    if location == "global":
+        local_files, s3_keys = aws.get_files(location=location)
+    elif location == "local":
+        local_files = aws.get_files(location=location)
+        s3_keys = [""]
+    elif location == "s3":
+        s3_keys = aws.get_files(location=location)
+        local_files = [""]
+
+    echo()
+    echo("Local Files...")
+
+    for obj in local_files:
         echo(obj)
-    return
+
+    echo()
+    echo("Bucket Objects...")
+
+    for obj in s3_keys:
+        echo(obj)
+
+
+def write_config(config):
+    echo("aws buckets...")
+    echo("\n".join(aws.get_bucket_list()))
+    config.dotenv_path.unlink(missing_ok=True)
+    config.dotenv_path.touch()
+    echo()
+    env_vars = {}
+    config_dict = config.configs
+
+    for _, val in config.keys_dict.items():
+        key = val.get("name")
+
+        if config_dict:
+            res_default = config_dict.get(key)
+        else:
+            res_default = None
+
+        res = typer.prompt(f"{key} ({val.get('note')})", type=str, default=res_default)
+        env_vars[key] = res
+
+    config.write_env_vars(env_vars)
+    config.print_current_config()
 
 
 @app.command()
 def config() -> None:
     """
     Configures the application
     """
     config = Config()
-    config.load_env()
-    config.print_current_config()
-    if not config.ask_overwrite():
-        return
+
+    if config.check_exists():
+        config.load_env()
+        config.print_current_config()
+
+        if config.ask_overwrite():
+            write_config(config)
+    else:
+        write_config(config)
 
     echo("Configuration complete.")
 
 
 def entry_point() -> None:
     app()
```

### Comparing `mgmt-0.6.2/mgmt/aws.py` & `mgmt-0.7.0/mgmt/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         self.config = Config()
         self.logger = Log(debug=False)
         self.load_config_file()
 
     def load_config_file(self):
         if self.config.check_exists():
             self.configs = self.config.get_configs()
-            self.bucket = self.configs.get("BUCKET")
-            self.object_prefix = self.configs.get("OBJECT_PREFIX")
-            self.local_dir = self.configs.get("LOCAL_DIR")
+            self.bucket = self.configs.get("MGMT_BUCKET")
+            self.object_prefix = self.configs.get("MGMT_OBJECT_PREFIX")
+            self.local_dir = self.configs.get("MGMT_LOCAL_DIR")
             self.file_mgmt = FileManager(self.local_dir)
         else:
             self.logger.debug("Config file not found. Please run `mgmt config` to set up the configuration.")
 
     def upload_file(self, file_name) -> bool:
         self.logger.debug("upload_file")
         object_name = file_name.split("/")[-1]
@@ -40,24 +40,24 @@
             with open(file_name, "rb") as data:
                 self.s3_client.upload_fileobj(data, self.bucket, object_name)
         except ClientError as e:
             self.logger.error(e)
             return False
         return True
 
-    def download_file(self, object_name: str, bucket_name: str = None) -> bool:
+    def download_standard(self, object_name: str, bucket_name: str = None) -> bool:
         if not bucket_name:
             bucket_name = self.bucket
         self.logger.info(f"Downloading `{object_name}` from `{bucket_name}`")
         file_name = object_name.split("/")[-1]
         try:
             with open(file_name, "wb") as data:
-                self.s3_client.download_fileobj(bucket_name, object_name, data)
+                self.s3_client.download_standardobj(bucket_name, object_name, data)
         except ClientError as e:
-            self.logger.error(f"-- ClientError --\n{str(e)}")
+            self.logger.error(f"-- ClientError -- {str(e)}")
             os.remove(file_name)
             return False
         return True
 
     def get_bucket_objs(self, bucket_name=None):
         if not bucket_name:
             bucket_name = self.bucket
@@ -102,15 +102,15 @@
                 "GlacierJobParameters": {
                     "Tier": restore_tier,
                 },
             },
         )
         return response
 
-    def download_from_glacier(self, object_name: str):
+    def download(self, object_name: str):
         self.get_obj_head(object_name)
         try:
             tier = self.obj_head["StorageClass"]
             if tier == "DEEP_ARCHIVE":
                 restore_tier = "Standard"
             elif tier == "GLACIER":
                 restore_tier = "Expedited"
@@ -131,15 +131,15 @@
                 elif status == "complete":
                     self.logger.debug("restored = True")
                     restored = True
                 else:
                     self.logger.debug(f"status: {status}, exiting...")
                     return
             self.logger.debug("downloading restored file")
-            return self.download_file(object_name=object_name)
+            return self.download_standard(object_name=object_name)
         else:
             self.logger.debug(f"object in {tier}, object will be restored in 12-24 hours")
             return
 
     def upload_target(self, target_path, compression):
         self.logger.debug(f"upload_target: {str(target_path)} {compression}")
         if compression == "zip":
@@ -171,7 +171,12 @@
         elif location == "here":
             p = Path(".")
             file_list = os.listdir(p)
         else:
             self.logger.error("invalid location input")
             self.logger.error(location)
         return file_list
+
+    def get_bucket_list(self):
+        response = self.s3_client.list_buckets()
+        buckets = [bucket["Name"] for bucket in response["Buckets"]]
+        return buckets
```

### Comparing `mgmt-0.6.2/mgmt/config.py` & `mgmt-0.7.0/mgmt/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,27 @@
 
 class Config:
     def __init__(self):
         self.path = Path("~/.config/mgmt").expanduser()
         self.path.mkdir(parents=True, exist_ok=True)
         self.dotenv_path = self.path / "config"
         self.logger = Log(debug=False)
+        self.keys_dict = {
+            "aws_bucket": {"name": "MGMT_BUCKET", "note": "storage bucket in aws"},
+            "object_prefix": {"name": "MGMT_OBJECT_PREFIX", "note": "prefix added to storage blob"},
+            "local_dir": {"name": "MGMT_LOCAL_DIR", "note": "full path to media dir on local machine"},
+        }
+        self.keys = [ele.get("name") for key, ele in self.keys_dict.items()]
         if not self.check_exists():
             self.logger.error("config file not found")
-            self.logger.info(f"check config file exists: {str(self.check_exists())}")
+            # self.logger.info(f"check config file exists: {str(self.check_exists())}")
             self.logger.info(f"dotenv_path: {str(self.dotenv_path)}")
+            self.configs = None
+        else:
+            self.configs = self.get_configs()
 
     def load_env(self):
         dotenv.load_dotenv(dotenv_path=self.dotenv_path)
 
     def log_current_config(self):
         if self.dotenv_path.is_file():
             with self.dotenv_path.open() as f:
@@ -29,26 +38,27 @@
         if self.dotenv_path.is_file():
             with self.dotenv_path.open() as f:
                 print(f"Current configuration:\n{f.read()}")
 
     def get_configs(self):
         if self.dotenv_path.is_file():
             self.load_env()
-            configs = {
-                "BUCKET": os.getenv("BUCKET"),
-                "OBJECT_PREFIX": os.getenv("OBJECT_PREFIX"),
-                "LOCAL_DIR": os.getenv("LOCAL_DIR"),
-            }
+            configs = {key: os.getenv(key) for key in self.keys}
         return configs
 
     def ask_overwrite(self) -> bool:
         return input("Would you like to overwrite these settings? (y/n) ").lower() == "y"
 
     def set_key(self, key: str, value: str):
         dotenv.set_key(self.dotenv_path, key, value)
 
     def update_config(self, atts_dict: dict):
         for key, value in atts_dict.items():
             self.set_key(key, value)
 
     def check_exists(self):
         return self.dotenv_path.is_file()
+
+    def write_env_vars(self, env_vars: dict):
+        with self.dotenv_path.open(mode="a") as f:
+            for key, value in env_vars.items():
+                f.write(f"{key}={value}\n")
```

### Comparing `mgmt-0.6.2/mgmt/files.py` & `mgmt-0.7.0/mgmt/files.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from typing import List
 from pathlib import Path
 from zipfile import ZipFile
 
 import rarfile
 
 from mgmt.log import Log
+from mgmt.config import Config
 
 
 class FileManager:
     def __init__(self, base_path=None):
         self.logger = Log(debug=False)
         if base_path:
             self.base_path = Path(base_path)
         else:
-            self.base_path = Path.home() / "media"
-            self.base_path = self.base_path.resolve()
+            config = Config()
+            self.base_path = config.configs.get("MGMT_LOCAL_DIR")
         if not self.base_path.exists():
-            raise ValueError(f"Path {str(self.base_path)} does not exist")
+            self.logger.error(f"-- ValueError -- Path {str(self.base_path)} is not a valid path from root")
+            self.logger.error("rerun `mgmt config`")
 
     def zip_single_file(self, filename: str) -> str:
         zip_file = filename.split(".")[0] + ".zip"
         with ZipFile(zip_file, "w") as zipf:
             zipf.write(os.path.join(self.base_path, filename), arcname=filename)
         return zip_file
 
@@ -60,22 +62,26 @@
             tar.close()
             return gzip_file
         except NotADirectoryError as e:
             self.logger.error(e)
             return self.gzip_single_file(target_path)
 
     def files_in_media_dir(self) -> List[str]:
-        tmp = os.listdir(self.base_path)
-        tmp = [
-            os.listdir(os.path.join(self.base_path, folder))
-            if os.path.isdir(os.path.join(self.base_path, folder))
-            else [folder]
-            for folder in tmp
-        ]
-        return [item for sublist in tmp for item in sublist]
+        file_list = []
+        path = Path(self.base_path)
+        for file in path.glob("**/*"):
+            if (
+                file.is_file()
+                and file.suffix.lower() in [".rar", ".mkv", ".mp4"]
+                and "subs" not in str(file).lower()
+                and "sample" not in str(file).lower()
+            ):
+                # print(file)
+                file_list.append(file)
+        return ["/".join(str(file).split("/")[-2:]) for file in file_list]
 
     def list_all_files(self):
         for file in self.base_path.glob("**/*"):
             self.logger.info(file)
 
     def list_all_dirs(self):
         for directory in self.base_path.glob("**/"):
```

### Comparing `mgmt-0.6.2/mgmt/log.py` & `mgmt-0.7.0/mgmt/log.py`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.2/pyproject.toml` & `mgmt-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "mgmt"
-version = "0.6.2"
+version = "0.7.0"
 description = ""
 readme = "README.md"
 authors = ["Will Wright <willwright@example.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/will-wright-eng/media-mgmt-cli"
 homepage = "https://github.com/will-wright-eng/media-mgmt-cli"
```

### Comparing `mgmt-0.6.2/PKG-INFO` & `mgmt-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgmt
-Version: 0.6.2
+Version: 0.7.0
 Summary: 
 Home-page: https://github.com/will-wright-eng/media-mgmt-cli
 License: GNU GPL v3.0
 Author: Will Wright
 Author-email: willwright@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

