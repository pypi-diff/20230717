# Comparing `tmp/hydrusvideodeduplicator-0.2.5.tar.gz` & `tmp/hydrusvideodeduplicator-0.3.0.tar.gz`

## Comparing `hydrusvideodeduplicator-0.2.5.tar` & `hydrusvideodeduplicator-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/docker-compose.yml
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/docker-entrypoint.sh
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    20971 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/LICENSE
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/README.md
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/docker-compose.yml
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/docker-entrypoint.sh
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    21111 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/README.md
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.2.5/docker-compose.yml` & `hydrusvideodeduplicator-0.3.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.3.0/docker-entrypoint.sh`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env bash
 
 Command="python3.11 -m hydrusvideodeduplicator"
 [[ -n "${API_KEY}" ]] && Command="${Command} --api-key='${API_KEY}'"
 [[ -n "${API_URL}" ]] && Command="${Command} --api-url='${API_URL}'"
 [[ -n "${THRESHOLD}" ]] && Command="${Command} --threshold=${THRESHOLD}"
+[[ -n "${JOB_COUNT}" ]] && Command="${Command} --job-count=${JOB_COUNT}"
 
 [[ ${CERT} = "true" ]] && Command="${Command} --verify-cert=cert"
 
 [[ ${OVERWRITE} = "true" ]] && Command="${Command} --overwrite" || Command="${Command} --no-overwrite"
 [[ ${SKIP_HASHING} = "true" ]] && Command="${Command} --skip-hashing" || Command="${Command} --no-skip-hashing"
 [[ ${CLEAR_SEARCH_CACHE} = "true" ]] && Command="${Command} --clear-search-cache" || Command="${Command} --no-clear-search-cache"
 [[ ${VERBOSE} = "true" ]] && Command="${Command} --verbose" || Command="${Command} --no-verbose"
```

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Annotated, List, Optional
 
 import typer
-from rich import print as rprint
+from rich import print
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 
 from .__about__ import __version__
 from .config import HYDRUS_API_KEY, HYDRUS_API_URL, HYDRUS_LOCAL_FILE_SERVICE_KEYS, HYDRUS_QUERY, REQUESTS_CA_BUNDLE
 from .dedup import HydrusVideoDeduplicator
 
@@ -16,15 +16,15 @@
 - api_url will be read from env var $HYDRUS_API_URL or .env file
 - to add custom queries, do
   --custom-query="series:twilight" --custom-query="character:edward" ... etc for each query
 - threshold is the min % matching to be considered similar. 100% is identical.
 - verbose turns on logging
 - debug turns on logging and sets the logging level to debug
 """
-rprint(f"[blue] Hydrus Video Deduplicator {__version__} [/]")
+print(f"[blue] Hydrus Video Deduplicator {__version__} [/]")
 
 
 def main(
     api_key: Annotated[Optional[str], typer.Option(help="Hydrus API Key")] = None,
     api_url: Annotated[Optional[str], typer.Option(help="Hydrus API URL")] = HYDRUS_API_URL,
     overwrite: Annotated[Optional[bool], typer.Option(help="Overwrite existing perceptual hashes")] = False,
     query: Annotated[Optional[List[str]], typer.Option(help="Custom Hydrus tag query")] = HYDRUS_QUERY,
@@ -39,14 +39,15 @@
     ] = HYDRUS_LOCAL_FILE_SERVICE_KEYS,
     verify_cert: Annotated[
         Optional[str], typer.Option(help="Path to TLS cert. This forces verification.")
     ] = REQUESTS_CA_BUNDLE,
     clear_search_cache: Annotated[
         Optional[bool], typer.Option(help="Clear the cache that tracks what files have already been compared")
     ] = False,
+    job_count: Annotated[Optional[int], typer.Option(help="Number of CPUs to use. Default is all but one core.")] = -2,
     verbose: Annotated[Optional[bool], typer.Option(help="Verbose logging")] = False,
     debug: Annotated[Optional[bool], typer.Option(hidden=True)] = False,
 ):
     # CLI debug parameter sets log level to info or debug
     loglevel = logging.WARNING
     if debug:
         loglevel = logging.DEBUG
@@ -76,25 +77,29 @@
     if not api_url:
         print("Hydrus URL not set. Exiting...")
         raise typer.Exit(code=1)
 
     print(f"Connecting to {api_url}")
     # Client connection
     # TODO: Try to connect with https first and then fallback to http with a strong warning
-    _client = hydrus_api.Client(
+    hydrus_client = hydrus_api.Client(
         api_url=api_url,
         access_key=api_key,
         verify_cert=verify_cert,
     )
 
     error_connecting = True
     error_connecting_exception_msg = ""
     error_connecting_exception = ""
     try:
-        superdeduper = HydrusVideoDeduplicator(_client)
+        superdeduper = HydrusVideoDeduplicator(
+            hydrus_client,
+            file_service_keys=file_service_key,
+            job_count=job_count,
+        )
     except hydrus_api.InsufficientAccess as exc:
         error_connecting_exception_msg = "Invalid Hydrus API key."
         error_connecting_exception = exc
     except hydrus_api.DatabaseLocked as exc:
         error_connecting_exception_msg = "Hydrus database is locked. Try again later."
         error_connecting_exception = exc
     except hydrus_api.ServerError as exc:
@@ -117,33 +122,35 @@
         error_connecting_exception = exc
     else:
         error_connecting = False
 
     if error_connecting:
         logging.fatal("FATAL ERROR HAS OCCURRED")
         logging.fatal(error_connecting_exception)
-        rprint(f"[red] {error_connecting_exception_msg} ")
+        print(f"[red] {error_connecting_exception_msg} ")
         raise typer.Exit(code=1)
 
     # Deduplication parameters
 
     if debug:
         superdeduper.hydlog.setLevel(logging.DEBUG)
         superdeduper._DEBUG = True
 
     if threshold < 0:
-        rprint("[red] ERROR: Invalid similarity threshold. Must be between 0 and 100.")
+        print("[red] ERROR: Invalid similarity threshold. Must be between 0 and 100.")
         raise typer.Exit(code=1)
     superdeduper.threshold = threshold
 
     superdeduper.clear_trashed_files_from_db()
 
     # Run all deduplicate functionality
     superdeduper.deduplicate(
-        overwrite=overwrite, custom_query=query, skip_hashing=skip_hashing, file_service_keys=file_service_key
+        overwrite=overwrite,
+        custom_query=query,
+        skip_hashing=skip_hashing,
     )
 
     raise typer.Exit()
 
 
 try:
     typer.run(main)
```

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
 import os
+from collections import namedtuple
 from itertools import islice
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from joblib import Parallel, delayed
-from rich import print as rprint
+from rich import print
 from sqlitedict import SqliteDict
 from tqdm import tqdm
 
 if TYPE_CHECKING:
     from collections.abc import Generator, Iterable, Sequence
     from typing import Any
 
@@ -24,55 +25,69 @@
 
 
 class HydrusVideoDeduplicator:
     hydlog = logging.getLogger("hydlog")
     threshold: float = 75.0
     _DEBUG = False
 
-    def __init__(self, client: hydrus_api.Client, verify_connection: bool = True):
+    def __init__(
+        self,
+        client: hydrus_api.Client,
+        verify_connection: bool = True,
+        file_service_keys: Sequence[str] | None = None,
+        job_count: int = -2,
+    ):
         self.client = client
         if verify_connection:
             self.verify_api_connection()
-        self.hydlog.setLevel(logging.WARNING)
+        self.hydlog.setLevel(logging.INFO)
+        self.job_count = job_count
 
         # Commonly used things from the Hydrus database
         # If any of these are large they should probably be lazily loaded
         self.all_services = self.client.get_services()
 
+        # Set the file service keys to be used for hashing
+        # Default is "all local files"
+        if file_service_keys is None or not file_service_keys:
+            self.file_service_keys = [self.all_services["all_local_files"][0]["service_key"]]
+        else:
+            self.file_service_keys = [x for x in file_service_keys if x.strip()]
+        self.verify_file_service_keys()
+
     # Verify client connection and permissions
     # Will throw a hydrus_api.APIError if something is wrong
     def verify_api_connection(self) -> None:
         self.hydlog.info(
             (
                 f"Client API version: v{self.client.VERSION}"
                 "| Endpoint API version: v{self.client.get_api_version()['version']}"
             )
         )
         hydrus_api_utils.verify_permissions(self.client, hydrus_api.utils.Permission)
 
     # Verify that the supplied file_service_key is a valid key for a local file service
-    def verify_file_service_keys(self, file_service_keys: Iterable[str]) -> None:
+    def verify_file_service_keys(self) -> None:
         VALID_SERVICE_TYPES = [hydrus_api.ServiceType.ALL_LOCAL_FILES, hydrus_api.ServiceType.FILE_DOMAIN]
 
-        for file_service_key in file_service_keys:
+        for file_service_key in self.file_service_keys:
             file_service = self.all_services['services'].get(file_service_key)
             if file_service is None:
                 raise KeyError(f"Invalid file service key: '{file_service_key}'")
 
             service_type = file_service.get('type')
             if service_type not in VALID_SERVICE_TYPES:
                 raise KeyError("File service key must be a local file service")
 
     # This is the master function of the class
     def deduplicate(
         self,
         overwrite: bool = False,
         custom_query: Sequence[str] | None = None,
         skip_hashing: bool = False,
-        file_service_keys: Sequence[str] | None = None,
     ) -> None:
         # Add perceptual hashes to video files
         # system:filetype tags are really inconsistent
         search_tags = [
             'system:filetype=video, gif, apng',
             'system:has duration',
             'system:file service is not currently in trash',
@@ -80,137 +95,149 @@
 
         query = False
         if custom_query is not None:
             # Remove whitespace and empty strings
             custom_query = [x for x in custom_query if x.strip()]
             if len(custom_query) > 0:
                 search_tags.extend(custom_query)
-                rprint(f"[yellow] Custom Query: {custom_query}")
+                print(f"[yellow] Custom Query: {custom_query}")
                 query = True
 
-        # Set the file service keys to be used for hashing
-        # Default is "all local files"
-        if file_service_keys is None or not file_service_keys:
-            file_service_keys = [self.all_services["all_local_files"][0]["service_key"]]
-        else:
-            file_service_keys = [x for x in file_service_keys if x.strip()]
-        self.verify_file_service_keys(file_service_keys)
-
         video_hashes = None
         if skip_hashing:
-            rprint("[yellow] Skipping perceptual hashing")
+            print("[yellow] Skipping perceptual hashing")
             if query:
-                video_hashes = set(self._retrieve_video_hashes(search_tags, file_service_keys))
+                video_hashes = set(self._retrieve_video_hashes(search_tags))
         else:
-            all_video_hashes = self._retrieve_video_hashes(search_tags, file_service_keys)
-            self._add_perceptual_hashes_to_db(overwrite=overwrite, video_hashes=all_video_hashes)
+            all_video_hashes = list(self._retrieve_video_hashes(search_tags))
+            self.add_perceptual_hashes_to_db(overwrite=overwrite, video_hashes=all_video_hashes)
 
         if query and not skip_hashing:
-            video_hashes = set(self._retrieve_video_hashes(search_tags, file_service_keys))
+            video_hashes = set(self._retrieve_video_hashes(search_tags))
 
         if query:
-            self._find_potential_duplicates(limited_video_hashes=video_hashes, file_service_keys=file_service_keys)
+            self._find_potential_duplicates(limited_video_hashes=video_hashes)
         else:
-            self._find_potential_duplicates(limited_video_hashes=None, file_service_keys=file_service_keys)
+            self._find_potential_duplicates(limited_video_hashes=None)
 
         self.hydlog.info("Deduplication done.")
 
     @staticmethod
     def _calculate_perceptual_hash(video: Path | str | bytes) -> str:
         perceptual_hash = Vpdq.vpdq_to_json(Vpdq.computeHash(video))
         assert perceptual_hash != "[]"
         return perceptual_hash
 
     def _retrieve_video_hashes(
         self, search_tags: Iterable[str], file_service_keys: Iterable[str] | None = None
     ) -> Iterable[str]:
         all_video_hashes = self.client.search_files(
             tags=search_tags,
-            file_service_keys=file_service_keys,
             file_sort_type=hydrus_api.FileSortType.FILE_SIZE,
             return_hashes=True,
             file_sort_asc=True,
             return_file_ids=False,
         )["hashes"]
         return all_video_hashes
 
-    def _add_perceptual_hashes_to_db(self, overwrite: bool, video_hashes: Sequence[str]) -> None:
+    def fetch_and_hash_file(self, video_hash: str) -> tuple | None:
+        """
+        Retrieves the video from Hydrus,
+        calculates the perceptual hash,
+        """
+        try:
+            video_response = self.client.get_file(hash_=video_hash)
+        except hydrus_api.HydrusAPIException:
+            print("[red] Failed to get video from Hydrus.")
+            self.hydlog.error("Error getting video from Hydrus.")
+            return
+
+        # Calculate perceptual_hash
+        try:
+            perceptual_hash = self._calculate_perceptual_hash(video_response.content)
+        except Exception as exc:
+            print("[red] Failed to calculate a perceptual hash.")
+            self.hydlog.exception(exc)
+            self.hydlog.error(f"Errored file hash: {video_hash}")
+        else:
+            PHashedVideo = namedtuple("PHashedVideo", "video_hash perceptual_hash")
+            return PHashedVideo(video_hash, perceptual_hash)
+
+    def add_perceptual_hashes_to_db(self, overwrite: bool, video_hashes: Sequence[str]) -> None:
+        """
+        Retrieves the video from Hydrus,
+        calculates the perceptual hash,
+        and then add it to the database.
+        """
+
         # Create database folder
         try:
             os.makedirs(DEDUP_DATABASE_DIR, exist_ok=False)
             # Exception before this log if directory already exists
             self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
         except OSError:
             pass
 
-        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
-            dblen = len(hashdb)
+        with SqliteDict(
+            str(DEDUP_DATABASE_FILE), tablename="videos", flag="c", autocommit=True, outer_stack=False
+        ) as hashdb:
             dbsize = os.path.getsize(DEDUP_DATABASE_FILE)
 
-            if dblen > 0:
+            # Cache len(hashdb) because it's O(n) to get the length.
+            if (dblen := len(hashdb)) > 0:
                 self.hydlog.info(f"Database found of length {dblen}, size {dbsize} bytes")
             else:
                 self.hydlog.info(f"Database not found. Creating one at {DEDUP_DATABASE_FILE}")
 
+            if overwrite:
+                new_video_hashes = video_hashes
+                print(f"[yellow] Overwriting {dblen} existing hashes.")
+            else:
+                # Filter existing hashes
+                new_video_hashes = [
+                    video_hash
+                    for video_hash in video_hashes
+                    if video_hash not in hashdb or "perceptual_hash" not in hashdb[video_hash]
+                ]
+
+            print(f"[blue] Found {len(new_video_hashes)} videos to process")
+
+            hash_count = 0
             try:
-                with tqdm(total=len(video_hashes), dynamic_ncols=True, unit="video", colour="BLUE") as pbar:
-                    count_since_last_commit = 0
-                    COMMIT_INTERVAL = 16
-
-                    for video_hash in video_hashes:
-                        pbar.update(1)
-                        # Only calculate new hash if it's missing or if overwrite is true
-                        if not overwrite and video_hash in hashdb and "perceptual_hash" in hashdb[video_hash]:
-                            continue
-
-                        # Get video file from Hydrus
-                        try:
-                            video_response = self.client.get_file(hash_=video_hash)
-                        except hydrus_api.HydrusAPIException:
-                            rprint("[red] Failed to get video from Hydrus.")
-                            self.hydlog.error("Error getting video from Hydrus.")
-                            continue
-
-                        # Calculate perceptual_hash
-                        try:
-                            perceptual_hash = self._calculate_perceptual_hash(video_response.content)
-                        except Exception as exc:
-                            rprint("[red] Failed to calculate a perceptual hash.")
-                            self.hydlog.exception(exc)
-                            self.hydlog.error(f"Errored file hash: {video_hash}")
-                        else:
-                            # Write perceptual hash to DB
+                self.hydlog.info("Starting perceptual hash processing")
+
+                with tqdm(total=len(new_video_hashes), dynamic_ncols=True, unit="video", colour="BLUE") as pbar:
+                    # Change to return_as='unordered_generator' when joblib supports it! (should be soon)
+                    with Parallel(n_jobs=self.job_count, return_as='generator') as parallel:
+                        result_generator = parallel(
+                            delayed(self.fetch_and_hash_file)(video_hash) for video_hash in new_video_hashes
+                        )
+                        for result in result_generator:
+                            if result is None:
+                                continue
+                            video_hash = result.video_hash
+                            perceptual_hash = result.perceptual_hash
                             row = hashdb.get(video_hash, {})
                             row["perceptual_hash"] = perceptual_hash
                             hashdb[video_hash] = row
 
-                            # Batch DB commits to avoid excessive writes
-                            count_since_last_commit += 1
-                            if count_since_last_commit >= COMMIT_INTERVAL:
-                                hashdb.commit()
-                                count_since_last_commit = 0
-                                self.hydlog.debug("Committed perceptual hashes to database.")
-
-                            self.hydlog.debug("Perceptual hash calculated.")
+                            hash_count += 1
+                            pbar.update(1)
 
             except KeyboardInterrupt:
-                interrupt_msg = "Perceptual hash processing was interrupted!"
-                rprint(f"[yellow] {interrupt_msg}")
-                self.hydlog.error(interrupt_msg)
+                print("[yellow] Perceptual hash processing was interrupted!")
 
             else:
-                rprint("[green] Finished perceptual hash processing.")
+                print("[green] Finished perceptual hash processing.")
 
             finally:
-                hashdb.commit()
-                rprint(f"[green] Added {len(hashdb) - dblen} new videos to database.")
-                self.hydlog.info("Finished perceptual hash processing.")
+                print(f"[green] Added {hash_count} new videos to the database.")
 
-    def get_potential_duplicate_count_hydrus(self, file_service_keys: Iterable[str]) -> int:
-        return self.client.get_potentials_count(file_service_keys=file_service_keys)["potential_duplicates_count"]
+    def get_potential_duplicate_count_hydrus(self) -> int:
+        return self.client.get_potentials_count(file_service_keys=self.file_service_keys)["potential_duplicates_count"]
 
     def compare_videos(self, video1_hash: str, video2_hash: str, video1_phash: str, video2_phash: str) -> None:
         vpdq_hash1 = Vpdq.json_to_vpdq(video1_phash)
         vpdq_hash2 = Vpdq.json_to_vpdq(video2_phash)
         similar, similarity = Vpdq.is_similar(vpdq_hash1, vpdq_hash2, self.threshold)
 
         if similar:
@@ -237,25 +264,26 @@
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
             for key in hashdb:
                 row = hashdb[key]
                 if "farthest_search_index" in row:
                     del row["farthest_search_index"]
                 hashdb[key] = row
             hashdb.commit()
-        rprint("[green] Cleared search cache.")
+        print("[green] Cleared search cache.")
 
     def _find_potential_duplicates(
-        self, limited_video_hashes: Sequence[str] | None = None, file_service_keys: Iterable[str] | None = None
+        self,
+        limited_video_hashes: Sequence[str] | None = None,
     ) -> None:
         if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos", verbose=True):
-            rprint("[red] Could not search for duplicates.")
+            print("[red] Could not search for duplicates.")
             return
 
         # Number of potential duplicates before adding more. Just for user info.
-        pre_dedupe_count = self.get_potential_duplicate_count_hydrus(file_service_keys)
+        pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
 
         # BUG: If this process is interrupted, the farthest_search_index will not save for ANY entries.
         #      I think it might be because every entry in the column needs an entry for SQlite but I'm not sure.
         video_counter = 0
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
             try:
                 if limited_video_hashes is not None:
@@ -263,15 +291,15 @@
                 else:
                     total = len(hashdb)
 
                 with tqdm(
                     dynamic_ncols=True, total=total, desc="Finding duplicates", unit="video", colour="BLUE"
                 ) as pbar:
                     # -1 is all cores, -2 is all cores but one
-                    with Parallel(n_jobs=-2) as parallel:
+                    with Parallel(n_jobs=self.job_count) as parallel:
                         if limited_video_hashes is not None:
                             # Avoid checking if in hashdb for each hash. Just do it now.
                             clean_all_retrieved_video_hashes = [
                                 video_hash for video_hash in limited_video_hashes if video_hash in hashdb
                             ]
 
                             for i, video1_hash in enumerate(clean_all_retrieved_video_hashes):
@@ -323,25 +351,25 @@
                                 count_since_last_commit += 1
 
                                 if count_since_last_commit >= commit_interval:
                                     hashdb.commit()
                                     count_since_last_commit = 0
 
             except KeyboardInterrupt:
-                rprint("[yellow] Duplicate search was interrupted!")
+                print("[yellow] Duplicate search was interrupted!")
             finally:
                 hashdb.commit()
 
         # Statistics for user
-        post_dedupe_count = self.get_potential_duplicate_count_hydrus(file_service_keys)
+        post_dedupe_count = self.get_potential_duplicate_count_hydrus()
         new_dedupes_count = post_dedupe_count - pre_dedupe_count
         if new_dedupes_count > 0:
-            rprint(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
+            print(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
         else:
-            rprint("[green] No new potential duplicates found.")
+            print("[green] No new potential duplicates found.")
 
     @staticmethod
     def batched(iterable: Iterable, n: int) -> Generator[tuple, Any, None]:
         """
         Batch data into tuples of length n. The last batch may be shorter."
         batched('ABCDEFG', 3) --> ABC DEF G
         DO NOT use this for iterating over the database. Use batched_and_save_db instead.
@@ -361,20 +389,16 @@
         Batch rows of into rows of length n and save changes after each batch or after chunk_size batches.
         """
         assert n >= 1
         assert chunk_size is None or chunk_size >= 1
         if chunk_size is None:
             chunk_size = n
         it = iter(db.items())
-        while batch_items := dict(islice(it, n)):
-            batch_dict = {
-                key: {col: val for col, val in row.items() if col != 'key'} for key, row in batch_items.items()
-            }
-
-            yield batch_dict
+        while batch_items := dict(islice(it, 1)):
+            yield batch_items
 
             # Save changes after each batch
             db.commit()
 
     def is_files_deleted_hydrus(self, file_hashes: Iterable[str]) -> dict[str, bool]:
         """
         Check if files are trashed or deleted in Hydrus
@@ -427,15 +451,15 @@
         try:
             with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c", outer_stack=False) as hashdb:
                 # This is EXPENSIVE. sqlitedict gets len by iterating over the entire database!
                 if (total := len(hashdb)) < 1:
                     return
 
                 delete_count = 0
-                rprint(f"[blue] Database found with {total} videos already hashed.")
+                print(f"[blue] Database found with {total} videos already hashed.")
                 try:
                     with tqdm(
                         dynamic_ncols=True,
                         total=total,
                         desc="Clearing trashed videos",
                         unit="video",
                         colour="BLUE",
@@ -447,15 +471,15 @@
                                 video_hash = result[0]
                                 is_trashed = result[1]
                                 if is_trashed is True:
                                     del hashdb[video_hash]
                                     delete_count += 1
                             pbar.update(min(CHUNK_SIZE, total - pbar.n))
                 except Exception as exc:
-                    rprint("[red] Error while clearing trashed videos cache.")
+                    print("[red] Error while clearing trashed videos cache.")
                     print(exc)
                     self.hydlog.error(exc)
                 finally:
                     if delete_count > 0:
                         print(f"Cleared {delete_count} trashed videos from the database.")
                     self.update_search_cache(total - delete_count)
```

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/.gitignore` & `hydrusvideodeduplicator-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/LICENSE` & `hydrusvideodeduplicator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/README.md` & `hydrusvideodeduplicator-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/pyproject.toml` & `hydrusvideodeduplicator-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.5/PKG-INFO` & `hydrusvideodeduplicator-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.2.5
+Version: 0.3.0
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator
 Author-email: hydrusvideodeduplicator <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

