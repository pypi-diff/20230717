# Comparing `tmp/pilot_platform_object_storage-1.3.0.tar.gz` & `tmp/pilot_platform_object_storage-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot_platform_object_storage-1.3.0.tar", max compression
+gzip compressed data, was "pilot_platform_object_storage-1.4.0.tar", max compression
```

## Comparing `pilot_platform_object_storage-1.3.0.tar` & `pilot_platform_object_storage-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3493 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/README.md
--rw-r--r--   0        0        0      120 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/__init__.py
--rw-r--r--   0        0        0      324 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/clients/__init__.py
--rw-r--r--   0        0        0     6476 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/clients/azure_blob_client.py
--rw-r--r--   0        0        0     7117 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/clients/azure_container_client.py
--rw-r--r--   0        0        0     2143 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/clients/base_container_client.py
--rw-r--r--   0        0        0     2051 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/clients/base_file_client.py
--rw-r--r--   0        0        0     1902 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/factories.py
--rw-r--r--   0        0        0      239 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/managers/__init__.py
--rw-r--r--   0        0        0     3763 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/managers/azure_blob_manager.py
--rw-r--r--   0        0        0      727 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/managers/base_manager.py
--rw-r--r--   0        0        0      266 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/providers/__init__.py
--rw-r--r--   0        0        0     6387 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/providers/azure.py
--rw-r--r--   0        0        0      444 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/object_storage/providers/enum.py
--rw-r--r--   0        0        0     1181 2023-06-28 20:49:00.693702 pilot_platform_object_storage-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.3.0/setup.py
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3493 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/README.md
+-rw-r--r--   0        0        0      120 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/__init__.py
+-rw-r--r--   0        0        0      324 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/__init__.py
+-rw-r--r--   0        0        0     6885 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/azure_blob_client.py
+-rw-r--r--   0        0        0     8332 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/azure_container_client.py
+-rw-r--r--   0        0        0     2649 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/base_container_client.py
+-rw-r--r--   0        0        0     2190 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/base_file_client.py
+-rw-r--r--   0        0        0     1902 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/factories.py
+-rw-r--r--   0        0        0      239 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/managers/__init__.py
+-rw-r--r--   0        0        0     4530 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/managers/azure_blob_manager.py
+-rw-r--r--   0        0        0     1134 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/managers/base_manager.py
+-rw-r--r--   0        0        0      266 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/providers/__init__.py
+-rw-r--r--   0        0        0     7186 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/providers/azure.py
+-rw-r--r--   0        0        0      444 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/providers/enum.py
+-rw-r--r--   0        0        0     1181 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.4.0/setup.py
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.4.0/PKG-INFO
```

### Comparing `pilot_platform_object_storage-1.3.0/README.md` & `pilot_platform_object_storage-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/clients/azure_blob_client.py` & `pilot_platform_object_storage-1.4.0/object_storage/clients/azure_blob_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,33 +34,47 @@
     def __init__(
         self,
         blob_sas_url: str,
     ):
         self.blob_sas_url = blob_sas_url
 
     def _get_blob_name_from_sas(self) -> str:
+        """Returns blob's key from sas URL."""
+
         try:
             url, _ = self.blob_sas_url.split('?')
             return url[url.rfind('/') + 1 :]
         except ValueError as exc:
             exc_msg = 'Missing sas token in `blob_sas_url`'
             logger.exception(exc_msg)
             raise ValueError(exc_msg) from exc
 
+    async def is_exists(
+        self,
+    ) -> bool:
+        """Checks if blob in the context exists."""
+
+        try:
+            async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
+                return await blob_client.exists()
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
     async def upload_file(
         self,
         file_path: str,
-        chunk_size: Optional[int] = 4 * 1024 * 1024,
+        chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to a blob in the specified container."""
+
         key = self._get_blob_name_from_sas()
         try:
             async with BlobClient.from_blob_url(blob_url=self.blob_sas_url, max_block_size=chunk_size) as blob_client:
-                return await self._upload(blob_client, file_path, key, progress_callback)
+                return await self._upload(blob_client, file_path, key, progress_callback, chunk_size=chunk_size)
         except Exception as exc:
             raise self._handle_exception(exc)
 
     async def resume_upload(
         self,
         file_path: str,
         chunk_size: int = 4 * 1024 * 1024,
@@ -78,14 +92,15 @@
 
     async def download_file_to_bytes(
         self,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Download a file from the specified container."""
+
         key = self._get_blob_name_from_sas()
         try:
             async with BlobClient.from_blob_url(
                 blob_url=self.blob_sas_url, max_chunk_get_size=chunk_size
             ) as blob_client:
                 return await self._download_bytes(blob_client, key, progress_callback=progress_callback)
         except Exception as exc:
@@ -94,14 +109,15 @@
     async def download_file(
         self,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download a file from the specified container."""
+
         key = self._get_blob_name_from_sas()
 
         await self._create_parent_dir(file_path)
 
         try:
             async with BlobClient.from_blob_url(
                 blob_url=self.blob_sas_url, max_chunk_get_size=chunk_size
@@ -111,32 +127,35 @@
             raise self._handle_exception(exc)
 
     async def copy_file_from_url(
         self,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
+
         try:
             async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
                 return await self._copy_from_url(blob_client, source_url)
         except Exception as exc:
             raise self._handle_exception(exc)
 
     async def delete_file(self) -> None:
         """Delete a file with all snapshots in a specific container."""
+
         try:
             async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
                 return await self._delete(blob_client)
         except Exception as exc:
             raise self._handle_exception(exc)
 
     async def get_file_url(
         self,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
+
         try:
             async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
                 return blob_client.url
         except Exception as exc:
             raise self._handle_exception(exc)
 
     async def get_file_properties(
```

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/clients/azure_container_client.py` & `pilot_platform_object_storage-1.4.0/object_storage/clients/azure_container_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,28 +33,56 @@
 
     def __init__(
         self,
         container_sas_url: str,
     ):
         self.container_sas_url = container_sas_url
 
+    async def is_exists(self) -> bool:
+        """Checks if container in the context exists."""
+
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                return await container_client.exists()
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
+    async def is_file_exists(self, key: str) -> bool:
+        """Checks if container in the context exists."""
+
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return await blob_client.exists()
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
+    async def delete(self) -> Dict[str, Any]:
+        """Deletes the specific container in the context from the Storage."""
+
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                return await container_client.delete_container()
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
     async def upload_file(
         self,
         key: str,
         file_path: str,
-        chunk_size: Optional[int] = 4 * 1024 * 1024,
+        chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to a blob in the specified container."""
         try:
             async with ContainerClient.from_container_url(
                 container_url=self.container_sas_url, max_block_size=chunk_size
             ) as container_client:
                 blob_client = container_client.get_blob_client(key)
-                return await self._upload(blob_client, file_path, key, progress_callback)
+                return await self._upload(blob_client, file_path, key, progress_callback, chunk_size=chunk_size)
         except Exception as exc:
             raise self._handle_exception(exc)
 
     async def resume_upload(
         self,
         key: str,
         file_path: str,
```

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/clients/base_container_client.py` & `pilot_platform_object_storage-1.4.0/object_storage/clients/base_file_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,72 +7,72 @@
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 
 
-class BaseContainerClient(ABC):
+class BaseFileClient(ABC):
     """Abstract base class for object storage clients."""
 
     @abstractmethod
     async def upload_file(
         self,
-        key: str,
         file_path: str,
-        chunk_size: Optional[int] = 4 * 1024 * 1024,
+        chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file_to_bytes(
         self,
-        key: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Returns content in bytes of the specific file from the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file(
         self,
-        key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download the specific file from the specified bucket to file_path."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def copy_file_from_url(
         self,
-        key: str,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def delete_file(
         self,
-        key: str,
     ) -> None:
-        """Delete a file in the specified container."""
+        """Copies a file from a URL to a blob in the specified container."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def get_file_url(
         self,
-        key: str,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
 
         raise NotImplementedError()
+
+    @abstractmethod
+    async def is_exists(self) -> bool:
+        """Checks if file in the context exists."""
+
+        raise NotImplementedError()
```

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/clients/base_file_client.py` & `pilot_platform_object_storage-1.4.0/object_storage/clients/base_container_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,66 +7,90 @@
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 
 
-class BaseFileClient(ABC):
+class BaseContainerClient(ABC):
     """Abstract base class for object storage clients."""
 
     @abstractmethod
+    async def is_exists(self) -> bool:
+        """Checks if container in the context exists."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
+    async def is_file_exists(self, key: str) -> bool:
+        """Checks if file with specific key exists in container."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
+    async def delete(self) -> Dict[str, Any]:
+        """Deletes the specific container in the context from the Storage."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
     async def upload_file(
         self,
+        key: str,
         file_path: str,
-        chunk_size: Optional[int] = 4 * 1024 * 1024,
+        chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file_to_bytes(
         self,
+        key: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Returns content in bytes of the specific file from the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file(
         self,
+        key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download the specific file from the specified bucket to file_path."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def copy_file_from_url(
         self,
+        key: str,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def delete_file(
         self,
+        key: str,
     ) -> None:
-        """Copies a file from a URL to a blob in the specified container."""
+        """Delete a file in the specified container."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def get_file_url(
         self,
+        key: str,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
 
         raise NotImplementedError()
```

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/factories.py` & `pilot_platform_object_storage-1.4.0/object_storage/factories.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/managers/azure_blob_manager.py` & `pilot_platform_object_storage-1.4.0/object_storage/managers/azure_blob_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,24 +38,39 @@
         """Creates a new container with the specified name."""
 
         async with BlobServiceClient.from_connection_string(self.connection_string) as service:
             container_client = service.get_container_client(container_name)
             resp = await container_client.create_container()
             return resp
 
+    async def delete_container(self, container_name: str) -> Dict[str, Any]:
+        """Deletes container with the specified name."""
+
+        async with BlobServiceClient.from_connection_string(self.connection_string) as service:
+            container_client = service.get_container_client(container_name)
+            resp = await container_client.delete_container()
+            return resp
+
     async def list_objects(self, container_name: str) -> List[BlobProperties]:
         """Lists blobs in the specified container."""
 
         async with BlobServiceClient.from_connection_string(self.connection_string) as service:
             container_client = service.get_container_client(container_name)
             blobs = []
             async for blob in container_client.list_blobs(results_per_page=10):
                 blobs.append(blob)
             return blobs
 
+    async def is_container_exists(self, container_name: str) -> bool:
+        """Checks if container with `container_name` exists in the Storage."""
+
+        async with BlobServiceClient.from_connection_string(self.connection_string) as service:
+            container_client = service.get_container_client(container_name)
+            return await container_client.exists()
+
     async def get_blob_sas(self, container: str, key: str, read: bool = False, write: bool = False) -> str:
         """Generates a URL for a blob with a SAS token that allows read and write access."""
 
         async with BlobServiceClient.from_connection_string(self.connection_string) as service:
             sas_token = generate_blob_sas(
                 account_name=service.account_name,
                 account_key=service.credential.account_key,
```

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/managers/base_manager.py` & `pilot_platform_object_storage-1.4.0/object_storage/managers/base_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,11 +15,23 @@
     @abstractmethod
     async def create_container(self, container_name: str) -> Dict[str, Any]:
         """Creates a container in the object storage service."""
 
         raise NotImplementedError()
 
     @abstractmethod
+    async def delete_container(self, container_name: str) -> Dict[str, Any]:
+        """Deletes container from the object storage service."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
     async def list_objects(self, container_name: str) -> List[str]:
         """Lists all objects in the specified container."""
 
         raise NotImplementedError()
+
+    @abstractmethod
+    async def is_container_exists(self, container_name: str) -> bool:
+        """Checks if container with `container_name` exists in the Storage."""
+
+        raise NotImplementedError()
```

### Comparing `pilot_platform_object_storage-1.3.0/object_storage/providers/azure.py` & `pilot_platform_object_storage-1.4.0/object_storage/providers/azure.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 import logging
 from pathlib import Path
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Tuple
 from uuid import uuid4
 
 import aiofiles
 import aiofiles.os
 from aiofiles.os import makedirs
+from aiofiles.threadpool.binary import AsyncBufferedReader
 from azure.core.exceptions import ClientAuthenticationError
 from azure.core.exceptions import HttpResponseError
 from azure.core.exceptions import ResourceNotFoundError
 from azure.storage.blob import BlobBlock
 from azure.storage.blob.aio import BlobClient
 
 logger = logging.getLogger('pilot.object-storage')
@@ -49,36 +51,65 @@
 
     async def _upload(
         self,
         client: BlobClient,
         file_path: str,
         key: str,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
+        chunk_size: int = 4 * 1024 * 1024,
     ) -> Dict[str, Any]:
-        async def progress_hook(current: int, total: int) -> None:
-            if progress_callback:
-                await progress_callback(key, current, total)
+        """Upload a file to sas URL."""
 
-        stat_res = await aiofiles.os.stat(file_path)
         async with aiofiles.open(file_path, mode='rb') as f:
-            resp = await client.upload_blob(
-                f,
-                length=stat_res.st_size,
-                max_concurrency=4,
-                progress_hook=progress_hook,
-            )
-        return resp
+            uploaded_blocks = await self._upload_chunks(client, file_path, key, f, chunk_size, progress_callback)
+            return await self._commit_blob(client, uploaded_blocks)
+
+    async def _upload_chunks(
+        self,
+        client: BlobClient,
+        file_path: str,
+        key: str,
+        file_obj: AsyncBufferedReader,  # has to be checked the correct type
+        chunk_size: int = 4 * 1024 * 1024,
+        progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
+        current: int = 0,
+    ) -> List[BlobBlock]:
+        """Upload the file by cutting into chunks.
+
+        If there is progress callback, will upload the chunk from the current point.
+        """
+        uploaded_blocks = []
+        file_length = (await aiofiles.os.stat(file_path)).st_size
+
+        while True:
+            chunk = await file_obj.read(chunk_size)
+            if not chunk:
+                break
+            block_id = str(uuid4())
+            await client.stage_block(block_id=block_id, data=chunk)
+            if progress_callback:
+                current = min(current + chunk_size, file_length)
+                await progress_callback(key, current, file_length)
+            uploaded_blocks.append(BlobBlock(block_id=block_id))
+        return uploaded_blocks
+
+    async def _commit_blob(self, client: BlobClient, block_list: Optional[List[BlobBlock]] = None) -> Dict[str, Any]:
+        """Commits the uncommitted blocks of a blob, making them a part of the blob's content."""
+        if block_list:
+            return await client.commit_block_list(block_list)
+        _, block_list = await client.get_block_list('uncommitted')
+        return await client.commit_block_list(block_list)
 
     async def _download_bytes(
         self,
         client: BlobClient,
         key: str,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
-        """Download a file from the specified container."""
+        """Download a file bytes from the specified container."""
 
         stream = await client.download_blob(max_concurrency=4)
         chunk_list = []
         current = 0
         async for chunk in stream.chunks():
             current += len(chunk)
             if progress_callback:
@@ -128,49 +159,32 @@
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Uploads a file to an Azure Blob Storage container, resuming an interrupted upload if there is an uncommitted
         block list."""
 
         uploaded_blocks = []
         offset = 0
-        current = 0
 
         _, block_list = await client.get_block_list('uncommitted')
         for block in block_list:
             offset += block.size
             uploaded_blocks.append(block.id)
 
         current = offset
         file_length = (await aiofiles.os.stat(file_path)).st_size
         file_renaming_length = file_length - offset
 
         if file_renaming_length:
             async with aiofiles.open(file_path, mode='rb') as f:
                 await f.seek(offset)
-                while True:
-                    chunk = await f.read(chunk_size)
-                    if not chunk:
-                        break
-                    block_id = str(uuid4())
-                    await client.stage_block(block_id=block_id, data=chunk)
-                    current += chunk_size
-                    if progress_callback:
-                        await progress_callback(key, current, file_length)
-                    uploaded_blocks.append(BlobBlock(block_id=block_id))
+                uploaded_blocks += await self._upload_chunks(
+                    client, file_path, key, f, chunk_size, progress_callback, current
+                )
 
-        await client.commit_block_list(uploaded_blocks)
-
-    async def _commit_blob(
-        self,
-        client: BlobClient,
-    ) -> None:
-        """Commits the uncommitted blocks of a blob, making them a part of the blob's content."""
-
-        _, block_list = await client.get_block_list('uncommitted')
-        await client.commit_block_list(block_list)
+        await self._commit_blob(client, uploaded_blocks)
 
     async def _get_blob_chunks(
         self,
         client: BlobClient,
     ) -> Tuple[list[BlobBlock], list[BlobBlock]]:
         """Returns a list of committeed and uncommitted the info of blob chunks."""
```

### Comparing `pilot_platform_object_storage-1.3.0/pyproject.toml` & `pilot_platform_object_storage-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pilot-platform-object-storage"
-version = "1.3.0"
+version = "1.4.0"
 description = "Python library for interacting with multiple object storage APIs."
 authors = ["Indoc Research"]
 readme = "README.md"
 packages = [{include = "object_storage"}]
 license = "Proprietary"
 documentation = "https://pilotdataplatform.github.io/object-storage/"
```

### Comparing `pilot_platform_object_storage-1.3.0/setup.py` & `pilot_platform_object_storage-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'azure-storage-blob>=12.16.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'pilot-platform-object-storage',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'Python library for interacting with multiple object storage APIs.',
     'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_container_sas(\'test\'))\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_file_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_file_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_container_client = get_container_client(\'azure\', container_sas_url)\nasyncio.run(azr_container_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Documentation\n\nAPI Reference and User Guide available at [pilotdataplatform.github.io/object-storage](https://pilotdataplatform.github.io/object-storage/)\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
     'author': 'Indoc Research',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pilot_platform_object_storage-1.3.0/PKG-INFO` & `pilot_platform_object_storage-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-object-storage
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python library for interacting with multiple object storage APIs.
 License: Proprietary
 Author: Indoc Research
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

