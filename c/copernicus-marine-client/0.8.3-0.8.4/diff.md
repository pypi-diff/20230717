# Comparing `tmp/copernicus_marine_client-0.8.3.tar.gz` & `tmp/copernicus_marine_client-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.8.3.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.4.tar", max compression
```

## Comparing `copernicus_marine_client-0.8.3.tar` & `copernicus_marine_client-0.8.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     9103 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/README.md
--rw-r--r--   0        0        0     3171 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22196 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6086 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3797 2023-07-11 08:16:13.394928 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4811 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_login.py
--rw-r--r--   0        0        0     7976 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    16597 2023-07-04 16:17:47.922157 copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     5504 2023-07-04 16:10:02.508215 copernicus_marine_client-0.8.3/copernicus_marine_client/configuration_files_creator.py
--rw-r--r--   0        0        0     7410 2023-07-03 13:46:52.425573 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     4542 2023-07-03 13:46:52.425573 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0     8265 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     8203 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     3964 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0     4387 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/subset_xarray.py
--rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.3/copernicus_marine_client/logging_conf.json
--rw-r--r--   0        0        0      887 2023-07-11 15:22:50.028698 copernicus_marine_client-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    10631 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.3/setup.py
--rw-r--r--   0        0        0    10038 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     9742 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.4/README.md
+-rw-r--r--   0        0        0     3171 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.4/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22196 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6162 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3797 2023-07-11 08:16:13.394928 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4823 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     8870 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    17026 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     5550 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7868 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4616 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     8748 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     8501 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     4397 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0     4456 2023-07-13 15:58:15.755707 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.4/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      623 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/utils.py
+-rw-r--r--   0        0        0      887 2023-07-17 09:15:30.602198 copernicus_marine_client-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    11278 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.4/setup.py
+-rw-r--r--   0        0        0    10677 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.4/PKG-INFO
```

### Comparing `copernicus_marine_client-0.8.3/README.md` & `copernicus_marine_client-0.8.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -110,46 +110,53 @@
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB
 
 Total size of the download: 19.62 MB
 
 
-Do you want to continue? [y/N]:
+Do you want to proceed with download? [y/N]:
 ```
 
 File(s) downloaded to ./{path}/{filename} if not specified otherwise:
 
 - "--output-path" specifies a directory to dump the files in
 - "--no-directories" to not recreate the folder structure
 
 If not specified otherwise, after the header display with a summary of the request,
 the user is asked for confirmation:
 
 - "--no-confirmation" to turn down the confirmation prompt
 - "--show-outputnames" to display the full paths of the outputs files
 
+Option `--filter TEXT` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files. It work with both `--dataset-id` and `--dataset-url` options.
+
 Option `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.
-**Be aware that the regular expression must match the full absolute path of the files to filter.**
 
 Example:
 ```
-> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"
+> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"
 Password:
 You requested the download of the following files:
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 
 Total size of the download: 9.82 MB
 
 
-Do you want to continue? [y/N]:
+Do you want to proceed with download? [y/N]:
 ```
 
+### The overwrite option
+
+Both `native` and `subset` commands provide an `--overwrite-ouput-data` option.
+When not provided (default behavior), once the download has been accepted (or if the `--force-download` option was provided), if the file already exists on destination, then a new one with a unique index will be created.
+On the other hand, if the `--overwrite-ouput-data` option is provided and the file already exists, then it'll be overwritten.
+
 ### The `--help` argument
 
 In any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.
 
 ## Python functions
 
 The library also provide python functions to help with catalogue
@@ -191,15 +198,15 @@
     maximal_longitude=0.2,
     minimal_depth=100,
     maximal_depth=1000,
     variables=["zooc"],
     force_protocol="zarr-map",
     output_directory="data_folder",
     output_filename="datastore.zarr",
-    assume_yes=True,
+    force_download=True,
 )
 
 # Step 3: Download the subset based on request content
 filename = cmc.download_subset(
     login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request
 )
 
@@ -242,10 +249,10 @@
     maximal_latitude: Optional[float] = None
     minimal_depth: Optional[float] = None
     maximal_depth: Optional[float] = None
     start_datetime: Optional[datetime] = None
     end_datetime: Optional[datetime] = None
     output_directory: Optional[str] = None
     output_filename: Optional[str] = None
-    assume_yes: Optional[bool] = None
+    force_download: Optional[bool] = None
     force_protocol: Optional[str] = None
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 
 @dataclass
 class SubsetRequest:
     dataset_url: Optional[str] = None
     dataset_id: Optional[str] = None
     output_directory: str = ""
-    assume_yes: bool = False
+    force_download: bool = False
+    overwrite: bool = False
     variables: Optional[List[str]] = None
     minimal_longitude: Optional[float] = None
     maximal_longitude: Optional[float] = None
     minimal_latitude: Optional[float] = None
     maximal_latitude: Optional[float] = None
     minimal_depth: Optional[float] = None
     maximal_depth: Optional[float] = None
@@ -61,15 +62,15 @@
             ]:
                 new_value = float(value) if value is not None else None
             elif key in [
                 "start_datetime",
                 "end_datetime",
             ]:
                 new_value = datetime_parser(value) if value else None
-            elif key in ["assume_yes"]:
+            elif key in ["force_download"]:
                 new_value = (
                     True if value in [True, "true", "True", 1] else False
                 )
             elif key in ["variables"]:
                 new_value = list(value) if value is not None else None
             else:
                 new_value = str(value) if value else None
@@ -105,15 +106,15 @@
         if arg == "variable":
             # special case for variable, since it can have multiple values
             motu_api_request_dict.setdefault(arg, []).append(value)
         else:
             motu_api_request_dict[arg] = value
     subset_request = SubsetRequest(
         output_directory=".",
-        assume_yes=False,
+        force_download=False,
         output_filename=None,
         force_protocol=None,
     )
     conversion_dict = {
         "product-id": "dataset_id",
         "latitude-min": "minimal_latitude",
         "latitude-max": "maximal_latitude",
@@ -135,15 +136,16 @@
 @dataclass
 class NativeRequest:
     dataset_url: Optional[str] = None
     dataset_id: Optional[str] = None
     no_directories: bool = False
     show_outputnames: bool = False
     output_directory: str = "."
-    assume_yes: bool = False
+    force_download: bool = False
+    overwrite: bool = False
     force_protocol: Optional[str] = None
     regex: Optional[str] = None
 
     def update(self, new_dict: dict):
         """Method to update values in NativeRequest object.
         Skips "None" values
         """
@@ -155,15 +157,15 @@
 
     def enforce_types(self):
         type_enforced_dict = {}
         for key, value in self.__dict__.items():
             if key in [
                 "no_directories",
                 "show_outputnames",
-                "assume_yes",
+                "force_download",
             ]:
                 new_value = bool(value) if value is not None else None
             else:
                 new_value = str(value) if value else None
             type_enforced_dict[key] = new_value
         self.__dict__.update(type_enforced_dict)
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_login.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,28 +95,28 @@
         "(based on standard logging library)."
     ),
 )
 def login(
     username: str,
     password: str,
     config_file_directory: str,
-    assume_yes: bool,
+    force_download: bool,
     verbose: str = "INFO",
 ) -> None:
     if verbose == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
     else:
         logging.root.setLevel(level=verbose)
     check_copernicus_marine_credentials(username, password)
     configuration_files_creator(
         username=username,
         password=password,
         config_file_directory=config_file_directory,
-        assume_yes=assume_yes,
+        force_download=force_download,
     )
     logging.info(f"Configuration files stored in {config_file_directory}")
 
 
 def get_credential(
     credential: Optional[str],
     credential_type: Literal["username", "password"],
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import fnmatch
 import logging
 import logging.config
 import os
 from typing import Optional
 
 import click
 
@@ -20,14 +21,19 @@
 )
 from copernicus_marine_client.download_functions.download_ftp import (
     download_ftp,
 )
 from copernicus_marine_client.download_functions.download_s3native import (
     download_s3native,
 )
+from copernicus_marine_client.utils import (
+    OVERWRITE_LONG_OPTION,
+    OVERWRITE_OPTION_HELP_TEXT,
+    OVERWRITE_SHORT_OPTION,
+)
 
 PROTOCOL_KEYS_ORDER = {"s3native": S3NATIVE_KEY, "ftp": FTP_KEY}
 
 CREDENTIALS_REQUIRED_PROTOCOLS = [
     "ftp",
 ]
 
@@ -115,20 +121,27 @@
     type=str,
     default=os.path.join(os.path.expanduser("~"), ".copernicus_marine_client"),
     help="Path to a directory where a configuration file is stored. Accepts "
     + ".copernicus_marine_client_credentials / .netrc or _netrc / "
     + ".motuclient-python.ini files",
 )
 @click.option(
-    "--assume-yes",
+    "--force-download",
     is_flag=True,
     default=False,
     help="Flag to skip confirmation before download",
 )
 @click.option(
+    OVERWRITE_LONG_OPTION,
+    OVERWRITE_SHORT_OPTION,
+    is_flag=True,
+    default=False,
+    help=OVERWRITE_OPTION_HELP_TEXT,
+)
+@click.option(
     "--force-protocol",
     type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
     help="Force download through one of the available protocols",
 )
 @click.option(
     "--request-file",
     type=click.Path(),
@@ -141,33 +154,44 @@
     default="INFO",
     help=(
         "Set the details printed to console by the command "
         "(based on standard logging library)."
     ),
 )
 @click.option(
+    "--filter",
+    "--filter-with-globbing-pattern",
+    type=str,
+    default=None,
+    help="A pattern that must match the absolute paths of "
+    "the files to download. ",
+)
+@click.option(
     "--regex",
+    "--filter-with-regular-expression",
     type=str,
     default=None,
     help="The regular expression that must match the absolute paths of "
     "the files to download. ",
 )
 def native(
     dataset_url: str,
     dataset_id: str,
     username: Optional[str],
     password: Optional[str],
     no_directories: bool,
     show_outputnames: bool,
     output_directory: str,
     config_file_directory: str,
-    assume_yes: bool,
+    force_download: bool,
+    overwrite_output_data: bool,
     request_file: str,
     force_protocol: str,
     log_level: str = "INFO",
+    filter: Optional[str] = None,
     regex: Optional[str] = None,
 ):
     if log_level == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
     else:
         logging.root.setLevel(level=log_level)
@@ -184,20 +208,28 @@
 
     # Specific treatment for default values:
     # In order to not overload arguments with default values
     if no_directories:
         native_request.no_directories = no_directories
     if show_outputnames:
         native_request.show_outputnames = show_outputnames
-    if assume_yes:
-        native_request.assume_yes = assume_yes
+    if force_download:
+        native_request.force_download = force_download
+    if overwrite_output_data:
+        native_request.overwrite = overwrite_output_data
     if force_protocol:
         native_request.force_protocol = force_protocol
+    if filter:
+        native_request.regex = fnmatch.translate(filter)
     if regex:
-        native_request.regex = regex
+        native_request.regex = (
+            regex
+            if not filter
+            else "(" + regex + "|" + fnmatch.translate(filter) + ")"
+        )
 
     native_function(
         username,
         password,
         native_request,
         config_file_directory,
     )
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 from copernicus_marine_client.download_functions.download_opendap import (
     download_opendap,
 )
 from copernicus_marine_client.download_functions.download_zarr import (
     download_zarr,
     get_optimized_chunking,
 )
+from copernicus_marine_client.utils import (
+    OVERWRITE_LONG_OPTION,
+    OVERWRITE_OPTION_HELP_TEXT,
+    OVERWRITE_SHORT_OPTION,
+)
 
 PROTOCOL_KEYS_ORDER = {
     "zarr": (TIMECHUNKED_KEY, GEOCHUNKED_KEY),
     "zarr-map": TIMECHUNKED_KEY,
     "zarr-timeserie": GEOCHUNKED_KEY,
     "opendap": OPENDAP_KEY,
     "motu": MOTU_KEY,
@@ -193,20 +198,27 @@
         "Concatenate the downloaded data in the given file name "
         "(under the output directory). If "
         "the output-filename argument ends with '.nc' suffix, the file will be "
         "downloaded as a netCDF file."
     ),
 )
 @click.option(
-    "--assume-yes",
+    "--force-download",
     is_flag=True,
     default=False,
     help="Flag to skip confirmation before download",
 )
 @click.option(
+    OVERWRITE_LONG_OPTION,
+    OVERWRITE_SHORT_OPTION,
+    is_flag=True,
+    default=False,
+    help=OVERWRITE_OPTION_HELP_TEXT,
+)
+@click.option(
     "--force-protocol",
     type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
     help="Force download through one of the available protocols",
 )
 @click.option(
     "--request-file",
     type=click.Path(),
@@ -247,15 +259,16 @@
     end_datetime: Optional[datetime],
     output_filename: Optional[str],
     force_protocol: Optional[str],
     request_file: Optional[str],
     output_directory: str,
     config_file_directory: str,
     motu_api_request: Optional[str],
-    assume_yes: bool = False,
+    force_download: bool = False,
+    overwrite_output_data: bool = False,
     log_level: str = "INFO",
 ):
     if log_level == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
     else:
         logging.root.setLevel(level=log_level)
@@ -282,16 +295,19 @@
         "output_directory": output_directory,
         "output_filename": output_filename,
         "force_protocol": force_protocol,
     }
     subset_request.update(request_update_dict)
     # Specific treatment for default values:
     # In order to not overload arguments with default values
-    if assume_yes:
-        subset_request.assume_yes = assume_yes
+    if force_download:
+        subset_request.force_download = force_download
+    if overwrite_output_data:
+        subset_request.overwrite = overwrite_output_data
+
     subset_function(
         username,
         password,
         subset_request,
         config_file_directory,
     )
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/configuration_files_creator.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/configuration_files_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,25 +83,28 @@
         )
     else:
         credential = None
     return credential
 
 
 def create_copernicus_marine_client_config_file(
-    username: str, password: str, config_file_directory: str, assume_yes: bool
+    username: str,
+    password: str,
+    config_file_directory: str,
+    force_download: bool,
 ) -> None:
     config_lines = [
         "[credentials]\n",
         f"username={username}\n",
         f"password={password}\n",
     ]
     config_filename = os.path.join(
         config_file_directory, ".copernicus_marine_client_credentials"
     )
-    if os.path.exists(config_filename) and not assume_yes:
+    if os.path.exists(config_filename) and not force_download:
         click.confirm(
             f"File {config_filename} already exists, overwrite it ?",
             abort=True,
         )
     config_file = open(config_filename, "w")
     config_string = base64.b64encode(
         "".join(config_lines).encode("ascii", "strict")
@@ -147,17 +150,20 @@
         )
         logging.error(credential_error_message)
         return credential_error_message
     return None
 
 
 def main(
-    username: str, password: str, config_file_directory: str, assume_yes: bool
+    username: str,
+    password: str,
+    config_file_directory: str,
+    force_download: bool,
 ) -> None:
     if not os.path.exists(config_file_directory):
         os.makedirs(config_file_directory)
     create_copernicus_marine_client_config_file(
         username=username,
         password=password,
         config_file_directory=config_file_directory,
-        assume_yes=assume_yes,
+        force_download=force_download,
     )
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 import click
 from numpy import append, arange
 from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
 )
+from copernicus_marine_client.utils import (
+    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
+    get_unique_filename,
+)
 
 # /////////////////////////////
 # ---Using ftplib
 # /////////////////////////////
 
 
 def download_ftp(
@@ -27,45 +31,48 @@
     message, host, filenames_in = download_header(
         str(native_request.dataset_url),
         native_request.regex,
         username,
         password,
     )
     filenames_out = create_filenames_out(
-        filenames_in,
-        native_request.output_directory,
-        native_request.no_directories,
+        filenames_in=filenames_in,
+        output_directory=native_request.output_directory,
+        no_directories=native_request.no_directories,
+        overwrite=native_request.overwrite,
     )
     logging.info(message)
     if native_request.show_outputnames:
         logging.info("Output filenames:")
         for filename_out in filenames_out:
             logging.info(filename_out)
-    if not native_request.assume_yes:
-        click.confirm("Do you want to continue?", abort=True)
+    if not native_request.force_download:
+        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
+
     pool = ThreadPool()
     nfiles_per_process, nfiles = 1, len(filenames_in)
     indexes = append(
         arange(0, nfiles, nfiles_per_process, dtype=int),
         nfiles,
     )
     groups_in_files = [
         filenames_in[indexes[i] : indexes[i + 1]]
         for i in range(len(indexes) - 1)
     ]
     groups_out_files = [
         filenames_out[indexes[i] : indexes[i + 1]]
         for i in range(len(indexes) - 1)
     ]
+    groups_in_files_count = len(groups_in_files)
     download_summary_list = pool.map(
         download_files,
         zip(
-            [host] * len(groups_in_files),
-            [username] * len(groups_in_files),
-            [password] * len(groups_in_files),
+            [host] * groups_in_files_count,
+            [username] * groups_in_files_count,
+            [password] * groups_in_files_count,
             groups_in_files,
             groups_out_files,
         ),
     )
     download_summary = "".join(map(str, download_summary_list))
     return download_summary
 
@@ -196,23 +203,32 @@
 def parse_ftp_dataset_url(data_path: str) -> tuple[str, str]:
     host = data_path[len("ftp://") :].split("/")[0]
     path = data_path[len("ftp://" + host + "/") :]
     return (host, path)
 
 
 def create_filenames_out(
-    filenames_in: list[str], output_directory: str = "", no_directories=False
+    filenames_in: list[str],
+    overwrite: bool,
+    output_directory: str = "",
+    no_directories=False,
 ) -> list[str]:
     filenames_out = []
     for filename_in in filenames_in:
-        filename_out = f"{output_directory}/"
+        filename_out = f"{output_directory}{os.sep}"
         if no_directories:
-            filenames_out += [filename_out + filename_in.split("/")[-1]]
+            filename_out += filename_in.split(os.sep)[-1]
         elif filename_in.startswith("Core/"):
-            filenames_out += [filename_out + filename_in[len("Core/") :]]
+            filename_out += filename_in[len("Core/") :]
+
+        if os.path.exists(filename_out):
+            if not overwrite:
+                filename_out = get_unique_filename(filepath=filename_out)
+
+        filenames_out.append(filename_out)
     return filenames_out
 
 
 def format_file_size(
     size: float, decimals: int = 2, binary_system: bool = False
 ) -> str:
     if binary_system:
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_motu.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     CopernicusMarineCatalogue,
     get_product_from_url,
     parse_catalogue,
 )
 from copernicus_marine_client.catalogue_parser.request_structure import (
     SubsetRequest,
 )
+from copernicus_marine_client.utils import FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE
 
 
 def parse_motu_dataset_url(data_path: str) -> str:
     host = data_path.split("/motu-web/Motu")[0] + "/motu-web/Motu"
     return host
 
 
@@ -147,16 +148,16 @@
         ]
         + options_list
         + ["--quiet", "--size", "-o", "console"],
         capture_output=True,
     )
     size_dom = xml.dom.minidom.parseString(size_xml.stdout)
     logger.warn(size_dom.toprettyxml(newl=""))
-    if not subset_request.assume_yes:
-        click.confirm("Do you want to proceed with download ?", abort=True)
+    if not subset_request.force_download:
+        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
     run(
         [
             "motuclient",
         ]
         + options_list
     )
     return path.join(output_directory, output_filename)
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from pydap.net import HTTPError
 from xarray.backends import PydapDataStore
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     SubsetRequest,
 )
 from copernicus_marine_client.download_functions.subset_xarray import subset
+from copernicus_marine_client.utils import (
+    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
+    get_unique_filename,
+)
 
 
 def __parse_limit(message: str) -> Optional[float]:
     match = re.search(r", max=.+\";", message)
     if match:
         limit = match.group().strip(', max=";')
         return float(limit)
@@ -148,14 +152,15 @@
             Optional[float], Optional[float], Optional[float], Optional[float]
         ]
     ],
     temporal_subset: Optional[Tuple[Optional[datetime], Optional[datetime]]],
     depth_range: Optional[Tuple[Optional[float], Optional[float]]],
     limit: Optional[int],
     confirmation: Optional[bool],
+    overwrite: Optional[bool],
 ):
     def _open_subset(
         username: str,
         password: str,
         dataset_url: str,
         variables: Optional[list[str]],
         geographical_subset: Optional[
@@ -198,24 +203,34 @@
         password,
         dataset_url,
         variables,
         geographical_subset,
         temporal_subset,
         depth_range,
     )
+
+    complete_dataset = os.path.join(output_directory, output_filename)
+
     if confirmation:
         logger = logging.getLogger("blank_logger")
         logger.warn(dataset)
-        click.confirm("Do you want to continue?", abort=True, default=True)
+        click.confirm(
+            FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True, default=True
+        )
 
-    complete_dataset = os.path.join(output_directory, output_filename)
+    if os.path.exists(complete_dataset):
+        if not overwrite:
+            output_filename = get_unique_filename(filepath=complete_dataset)
+            complete_dataset = os.path.join(output_directory, output_filename)
+
+    write_mode = "w"
 
     try:
         logging.info("Trying to download as one file...")
-        dataset.to_netcdf(complete_dataset)
+        dataset.to_netcdf(complete_dataset, mode=write_mode)
         logging.info(f"Successfully downloaded to {complete_dataset}")
     except HTTPError as error:
         chunked_download(
             store,
             dataset,
             limit,
             error,
@@ -269,10 +284,11 @@
         output_directory=output_directory,
         output_filename=output_filename,
         variables=subset_request.variables,
         geographical_subset=geographical_subset,
         temporal_subset=temporal_subset,
         depth_range=depth_range,
         limit=limit,
-        confirmation=not subset_request.assume_yes,
+        confirmation=not subset_request.force_download,
+        overwrite=subset_request.overwrite,
     )
     return os.path.join(output_directory, output_filename)
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 import click
 from numpy import append, arange
 from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
 )
+from copernicus_marine_client.utils import (
+    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
+    get_unique_filename,
+)
 
 MARINE_DATA_LAKE_LISTING_ENDPOINT = "https://marine.copernicus.eu"
 MARINE_DATA_LAKE_LISTING_NATIVE_BUCKET = "mdl-native-list"
 MARINE_DATA_LAKE_DOWNLOAD_NATIVE_BUCKET = "mdl-native"
 MARINE_DATA_LAKE_S3_LISTING_NATIVE_ROOT_URI = (
     f"{MARINE_DATA_LAKE_LISTING_NATIVE_BUCKET}/native"
 )
@@ -34,25 +38,27 @@
     message, endpoint_url, filenames_in = download_header(
         [str(native_request.dataset_url)],
         native_request.regex,
         username,
         password,
     )
     filenames_out = create_filenames_out(
-        filenames_in,
-        native_request.output_directory,
-        native_request.no_directories,
+        filenames_in=filenames_in,
+        output_directory=native_request.output_directory,
+        no_directories=native_request.no_directories,
+        overwrite=native_request.overwrite,
     )
     logging.info(message)
     if native_request.show_outputnames:
         logging.info("Output filenames:")
         for filename_out in filenames_out:
             logging.info(filename_out)
-    if not native_request.assume_yes:
-        click.confirm("Do you want to continue?", abort=True)
+    if not native_request.force_download:
+        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
+
     pool = ThreadPool()
     nfiles_per_process, nfiles = 1, len(filenames_in)
     indexes = append(
         arange(0, nfiles, nfiles_per_process, dtype=int),
         nfiles,
     )
     groups_in_files = [
@@ -200,39 +206,42 @@
         endpoint_url, path = data_path.split("/mdl-native/", maxsplit=1)
         path = "s3://mdl-native/" + path
         path_dict.setdefault(endpoint_url, []).append(path)
     return path_dict
 
 
 def create_filenames_out(
-    filenames_in: list[str], output_directory: str = "", no_directories=False
+    filenames_in: list[str],
+    overwrite: bool,
+    output_directory: str = "",
+    no_directories=False,
 ) -> list[str]:
     filenames_out = []
     for filename_in in filenames_in:
         filename_out = f"{output_directory}/"
         if no_directories:
-            filenames_out += [filename_out + filename_in.split("/")[-1]]
+            filename_out += filename_in.split("/")[-1]
         elif filename_in.startswith(
-            f"s3://{MARINE_DATA_LAKE_S3_DOWNLOAD_NATIVE_ROOT_URI}/"
+            f"s3://{MARINE_DATA_LAKE_S3_DOWNLOAD_NATIVE_ROOT_URI}{os.sep}"
         ):
-            filenames_out += [
-                filename_out
-                + filename_in.split(
-                    f"s3://{MARINE_DATA_LAKE_S3_DOWNLOAD_NATIVE_ROOT_URI}/"
-                )[-1]
-            ]
+            filename_out += filename_in.split(
+                f"s3://{MARINE_DATA_LAKE_S3_DOWNLOAD_NATIVE_ROOT_URI}{os.sep}"
+            )[-1]
         elif filename_in.startswith(
-            f"s3://{MARINE_DATA_LAKE_S3_LISTING_NATIVE_ROOT_URI}/"
+            f"s3://{MARINE_DATA_LAKE_S3_LISTING_NATIVE_ROOT_URI}{os.sep}"
         ):
-            filenames_out += [
-                filename_out
-                + filename_in.split(
-                    f"s3://{MARINE_DATA_LAKE_S3_LISTING_NATIVE_ROOT_URI}/"
-                )[-1]
-            ]
+            filename_out += filename_in.split(
+                f"s3://{MARINE_DATA_LAKE_S3_LISTING_NATIVE_ROOT_URI}{os.sep}"
+            )[-1]
+
+        if os.path.exists(filename_out):
+            if not overwrite:
+                filename_out = get_unique_filename(filepath=filename_out)
+
+        filenames_out.append(filename_out)
     return filenames_out
 
 
 def format_file_size(
     size: float, decimals: int = 2, binary_system: bool = False
 ) -> str:
     if binary_system:
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 import xarray as xr
 import zarr
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     SubsetRequest,
 )
 from copernicus_marine_client.download_functions.subset_xarray import subset
+from copernicus_marine_client.utils import (
+    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
+    get_unique_filename,
+)
 
 
 def get_optimized_chunking(subset_request: SubsetRequest) -> str:
     """Function to calculate the optimized type of chunking,
     based on a subset_request.
     Returns a str: "map" if time-chunking is optimized,
     "timeserie" if geo-chunking is optimized
@@ -52,41 +56,48 @@
     ],
     temporal_subset: Optional[tuple[Optional[datetime], Optional[datetime]]],
     depth_range: Optional[tuple[Optional[float], Optional[float]]],
     dataset_url: str,
     output_directory: str,
     output_filename: str,
     variables: Optional[list[str]],
-    assume_yes: bool = False,
+    force_download: bool = False,
+    overwrite: bool = False,
 ):
 
     dataset = xr.open_zarr(dataset_url)
     dataset = subset(
         dataset, variables, geographical_subset, temporal_subset, depth_range
     )
     dataset = dataset.chunk(chunks="auto")
 
-    if not assume_yes:
+    output_path = path.join(output_directory, output_filename)
+
+    if not force_download:
         logger = logging.getLogger("blank_logger")
         logger.warn(dataset)
-        click.confirm("Do you want to continue?", abort=True, default=True)
+        click.confirm(
+            FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True, default=True
+        )
+
+    if os.path.exists(output_path):
+        if not overwrite:
+            output_filename = get_unique_filename(filepath=output_path)
+            output_path = path.join(output_directory, output_filename)
 
+    write_mode = "w"
     if output_filename.endswith(".nc"):
         if not os.path.isdir(output_directory):
             os.makedirs(output_directory)
-        dataset.to_netcdf(path.join(output_directory, output_filename))
+        dataset.to_netcdf(output_path, mode=write_mode)
     else:
-        store = zarr.DirectoryStore(
-            path.join(output_directory, output_filename)
-        )
-        dataset.to_zarr(store)
+        store = zarr.DirectoryStore(output_path)
+        dataset.to_zarr(store=store, mode=write_mode)
 
-    logging.info(
-        f"Successfully downloaded to {path.join(output_directory, output_filename)}"
-    )
+    logging.info(f"Successfully downloaded to {output_path}")
 
 
 def download_zarr(
     username: str,
     password: str,
     subset_request: SubsetRequest,
 ):
@@ -110,22 +121,23 @@
     )
     output_filename = (
         subset_request.output_filename
         if subset_request.output_filename
         else "data.zarr"
     )
     variables = subset_request.variables
-    assume_yes = subset_request.assume_yes
+    force_download = subset_request.force_download
 
     download_dataset(
         username=username,
         password=password,
         geographical_subset=geographical_subset,
         temporal_subset=temporal_subset,
         depth_range=depth_range,
         dataset_url=dataset_url,
         output_directory=output_directory,
         output_filename=output_filename,
         variables=variables,
-        assume_yes=assume_yes,
+        force_download=force_download,
+        overwrite=subset_request.overwrite,
     )
     return path.join(output_directory, output_filename)
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/download_functions/subset_xarray.py` & `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/subset_xarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,23 @@
     ] = None,
     depth_range: Optional[Tuple[Optional[float], Optional[float]]] = None,
 ) -> xr.Dataset:
 
     if variables:
         ds = ds[np.array(variables)]
 
-    if geographical_subset is not None and any(geographical_subset):
+    if geographical_subset is not None:
         (
             minimal_latitude,
             maximal_latitude,
             minimal_longitude,
             maximal_longitude,
         ) = geographical_subset
-        latitude_subset = (minimal_latitude, maximal_latitude)
-        longitude_subset = (minimal_longitude, maximal_longitude)
 
-        if any(latitude_subset):
+        if minimal_latitude is not None or maximal_latitude is not None:
             latitude_selection = (
                 minimal_latitude
                 if minimal_latitude == maximal_latitude
                 else slice(minimal_latitude, maximal_latitude)
             )
             latitude_method = (
                 "nearest" if minimal_latitude == maximal_latitude else None
@@ -46,15 +44,15 @@
                     latitude=latitude_selection, method=latitude_method
                 )
             if "nav_lat" in ds.coords:
                 ds = ds.sel(nav_lat=latitude_selection, method=latitude_method)
             if "x" in ds.coords:
                 ds = ds.sel(x=latitude_selection, method=latitude_method)
 
-        if any(longitude_subset):
+        if minimal_longitude is not None or maximal_longitude is not None:
             longitude_selection = (
                 minimal_longitude
                 if minimal_longitude == maximal_longitude
                 else slice(minimal_longitude, maximal_longitude)
             )
             longitude_method = (
                 "nearest" if minimal_longitude == maximal_longitude else None
@@ -88,39 +86,40 @@
 
         temporal_kwargs["method"] = (
             "nearest" if start_datetime == end_datetime else None
         )
 
         ds = ds.sel(**temporal_kwargs)
 
-    if depth_range is not None and any(depth_range):
-        depth_kwargs: dict[str, Any] = {}
+    if depth_range is not None:
         minimal_depth, maximal_depth = depth_range
+        if minimal_depth is not None or maximal_depth is not None:
+            depth_kwargs: dict[str, Any] = {}
 
-        if "depth" in ds.dims:
-            depth_kwargs["depth"] = (
-                minimal_depth
-                if minimal_depth == maximal_depth
-                else slice(minimal_depth, maximal_depth)
-            )
-        elif "deptht" in ds.dims:
-            depth_kwargs["deptht"] = (
-                minimal_depth
-                if minimal_depth == maximal_depth
-                else slice(minimal_depth, maximal_depth)
-            )
-        elif "elevation" in ds.dims:
-            minimal_depth = minimal_depth * -1.0 if minimal_depth else None
-            maximal_depth = maximal_depth * -1.0 if maximal_depth else None
-            depth_kwargs["elevation"] = (
-                minimal_depth
-                if minimal_depth == maximal_depth
-                else slice(maximal_depth, minimal_depth)
-            )
+            if "depth" in ds.dims:
+                depth_kwargs["depth"] = (
+                    minimal_depth
+                    if minimal_depth == maximal_depth
+                    else slice(minimal_depth, maximal_depth)
+                )
+            elif "deptht" in ds.dims:
+                depth_kwargs["deptht"] = (
+                    minimal_depth
+                    if minimal_depth == maximal_depth
+                    else slice(minimal_depth, maximal_depth)
+                )
+            elif "elevation" in ds.dims:
+                minimal_depth = minimal_depth * -1.0 if minimal_depth else None
+                maximal_depth = maximal_depth * -1.0 if maximal_depth else None
+                depth_kwargs["elevation"] = (
+                    minimal_depth
+                    if minimal_depth == maximal_depth
+                    else slice(maximal_depth, minimal_depth)
+                )
 
-        depth_kwargs["method"] = (
-            "nearest" if minimal_depth == maximal_depth else None
-        )
+            depth_kwargs["method"] = (
+                "nearest" if minimal_depth == maximal_depth else None
+            )
 
-        ds = ds.sel(**depth_kwargs)
+            ds = ds.sel(**depth_kwargs)
 
     return ds
```

### Comparing `copernicus_marine_client-0.8.3/copernicus_marine_client/logging_conf.json` & `copernicus_marine_client-0.8.4/copernicus_marine_client/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.3/pyproject.toml` & `copernicus_marine_client-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.8.3"
+version = "0.8.4"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `copernicus_marine_client-0.8.3/setup.py` & `copernicus_marine_client-0.8.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.8.3',
+    'version': '0.8.4',
     'description': '',
-    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n**Be aware that the regular expression must match the full absolute path of the files to filter.**\n\nExample:\n```\n> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to continue? [y/N]:\n```\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    assume_yes=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n```\n',
+    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to proceed with download? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--filter TEXT` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to proceed with download? [y/N]:\n```\n\n### The overwrite option\n\nBoth `native` and `subset` commands provide an `--overwrite-ouput-data` option.\nWhen not provided (default behavior), once the download has been accepted (or if the `--force-download` option was provided), if the file already exists on destination, then a new one with a unique index will be created.\nOn the other hand, if the `--overwrite-ouput-data` option is provided and the file already exists, then it\'ll be overwritten.\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    force_download=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    force_download: Optional[bool] = None\n    force_protocol: Optional[str] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `copernicus_marine_client-0.8.3/PKG-INFO` & `copernicus_marine_client-0.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -139,46 +139,53 @@
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB
 
 Total size of the download: 19.62 MB
 
 
-Do you want to continue? [y/N]:
+Do you want to proceed with download? [y/N]:
 ```
 
 File(s) downloaded to ./{path}/{filename} if not specified otherwise:
 
 - "--output-path" specifies a directory to dump the files in
 - "--no-directories" to not recreate the folder structure
 
 If not specified otherwise, after the header display with a summary of the request,
 the user is asked for confirmation:
 
 - "--no-confirmation" to turn down the confirmation prompt
 - "--show-outputnames" to display the full paths of the outputs files
 
+Option `--filter TEXT` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files. It work with both `--dataset-id` and `--dataset-url` options.
+
 Option `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.
-**Be aware that the regular expression must match the full absolute path of the files to filter.**
 
 Example:
 ```
-> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"
+> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"
 Password:
 You requested the download of the following files:
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 
 Total size of the download: 9.82 MB
 
 
-Do you want to continue? [y/N]:
+Do you want to proceed with download? [y/N]:
 ```
 
+### The overwrite option
+
+Both `native` and `subset` commands provide an `--overwrite-ouput-data` option.
+When not provided (default behavior), once the download has been accepted (or if the `--force-download` option was provided), if the file already exists on destination, then a new one with a unique index will be created.
+On the other hand, if the `--overwrite-ouput-data` option is provided and the file already exists, then it'll be overwritten.
+
 ### The `--help` argument
 
 In any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.
 
 ## Python functions
 
 The library also provide python functions to help with catalogue
@@ -220,15 +227,15 @@
     maximal_longitude=0.2,
     minimal_depth=100,
     maximal_depth=1000,
     variables=["zooc"],
     force_protocol="zarr-map",
     output_directory="data_folder",
     output_filename="datastore.zarr",
-    assume_yes=True,
+    force_download=True,
 )
 
 # Step 3: Download the subset based on request content
 filename = cmc.download_subset(
     login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request
 )
 
@@ -271,11 +278,11 @@
     maximal_latitude: Optional[float] = None
     minimal_depth: Optional[float] = None
     maximal_depth: Optional[float] = None
     start_datetime: Optional[datetime] = None
     end_datetime: Optional[datetime] = None
     output_directory: Optional[str] = None
     output_filename: Optional[str] = None
-    assume_yes: Optional[bool] = None
+    force_download: Optional[bool] = None
     force_protocol: Optional[str] = None
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

