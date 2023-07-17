# Comparing `tmp/github-secret-syncer-0.0.8.tar.gz` & `tmp/github-secret-syncer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-secret-syncer-0.0.8.tar", last modified: Tue Jul 11 00:53:57 2023, max compression
+gzip compressed data, was "github-secret-syncer-0.0.9.tar", last modified: Mon Jul 17 21:23:48 2023, max compression
```

## Comparing `github-secret-syncer-0.0.8.tar` & `github-secret-syncer-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:53:57.122787 github-secret-syncer-0.0.8/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.8/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-11 00:53:57.122617 github-secret-syncer-0.0.8/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      734 2023-07-08 09:44:30.000000 github-secret-syncer-0.0.8/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:53:57.121587 github-secret-syncer-0.0.8/github_secret_syncer/
--rw-r--r--   0 j3ymac     (501) staff       (20)     4525 2023-07-08 09:29:14.000000 github-secret-syncer-0.0.8/github_secret_syncer/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:53:57.122418 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      278 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       14 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/requires.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-11 00:53:57.122832 github-secret-syncer-0.0.8/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      788 2023-07-11 00:52:16.000000 github-secret-syncer-0.0.8/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-17 21:23:48.606400 github-secret-syncer-0.0.9/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.9/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-17 21:23:48.606248 github-secret-syncer-0.0.9/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      734 2023-07-08 09:44:30.000000 github-secret-syncer-0.0.9/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-17 21:23:48.605443 github-secret-syncer-0.0.9/github_secret_syncer/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     4703 2023-07-17 21:23:29.000000 github-secret-syncer-0.0.9/github_secret_syncer/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-17 21:23:48.605997 github-secret-syncer-0.0.9/github_secret_syncer.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-17 21:23:48.000000 github-secret-syncer-0.0.9/github_secret_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      278 2023-07-17 21:23:48.000000 github-secret-syncer-0.0.9/github_secret_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-17 21:23:48.000000 github-secret-syncer-0.0.9/github_secret_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       14 2023-07-17 21:23:48.000000 github-secret-syncer-0.0.9/github_secret_syncer.egg-info/requires.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-17 21:23:48.000000 github-secret-syncer-0.0.9/github_secret_syncer.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-17 21:23:48.606442 github-secret-syncer-0.0.9/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      788 2023-07-17 21:16:27.000000 github-secret-syncer-0.0.9/setup.py
```

### Comparing `github-secret-syncer-0.0.8/LICENSE` & `github-secret-syncer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.8/PKG-INFO` & `github-secret-syncer-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-secret-syncer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Github Secret Syncer.
 Home-page: https://github.com/thejimmylin/github-secret-syncer
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `github-secret-syncer-0.0.8/README.md` & `github-secret-syncer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.8/github_secret_syncer/__init__.py` & `github-secret-syncer-0.0.9/github_secret_syncer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import logging
 from base64 import b64encode
 from pathlib import Path
 from typing import Any, TypedDict, cast
 
 import dotenv
 import requests
-from loguru import logger
 from nacl import encoding, public
 
+logger = logging.getLogger(__name__)
+
 __all__ = ["GithubSecretManager", "sync_secrets"]
 
 
 class PublicKey(TypedDict):
     key: str
     key_id: str
 
@@ -89,20 +91,24 @@
 def sync_secrets(
     dotenv_path: Path,
     owner: str,
     repo: str,
     pat: str,
     delete_missing: bool = True,
     api_version: str = "2022-11-28",
+    show_info=False,
 ) -> None:
     """Sync secrets from dotenv to Github Actions
 
     This function can be seen as an example of how to use GithubSecretManager.
     Feel free to copy and modify it to fit your needs.
     """
+    if show_info:
+        logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+
     secret_manager = GithubSecretManager(owner, repo, pat, api_version)
     secrets = secret_manager.list_repo_secrets()
     _dotenv_secrets = dotenv.dotenv_values(dotenv_path)
 
     # Ignore secrets like `foo` (without `=`)
     # This will not ignore secrets like `bar=` (it's value will be `""`)
     dotenv_secrets: dict[str, str] = {}
```

### Comparing `github-secret-syncer-0.0.8/github_secret_syncer.egg-info/PKG-INFO` & `github-secret-syncer-0.0.9/github_secret_syncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-secret-syncer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Github Secret Syncer.
 Home-page: https://github.com/thejimmylin/github-secret-syncer
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `github-secret-syncer-0.0.8/setup.py` & `github-secret-syncer-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="github-secret-syncer",
-    version="0.0.8",
+    version="0.0.9",
     install_requires=[
         "PyNaCl==1.5.0",
     ],
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="Github Secret Syncer.",
     long_description=long_description,
```

