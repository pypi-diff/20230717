# Comparing `tmp/linkplay-cli-0.0.3.tar.gz` & `tmp/linkplay-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkplay-cli-0.0.3.tar", last modified: Sun Jun  4 17:53:54 2023, max compression
+gzip compressed data, was "linkplay-cli-0.0.4.tar", last modified: Mon Jul 17 17:29:39 2023, max compression
```

## Comparing `linkplay-cli-0.0.3.tar` & `linkplay-cli-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:53:54.468422 linkplay-cli-0.0.3/
--rw-rw-rw-   0        0        0     1211 2023-05-26 14:29:31.000000 linkplay-cli-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1161 2023-06-04 17:53:54.467421 linkplay-cli-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      804 2023-05-28 21:18:52.000000 linkplay-cli-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 17:53:54.417421 linkplay-cli-0.0.3/linkplay_cli/
--rw-rw-rw-   0        0        0        1 2023-05-29 21:05:26.000000 linkplay-cli-0.0.3/linkplay_cli/__init__.py
--rw-rw-rw-   0        0        0    10334 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/cli.py
--rw-rw-rw-   0        0        0      217 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/config.py
--rw-rw-rw-   0        0        0     2423 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/discovery.py
--rw-rw-rw-   0        0        0     2300 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/firmware_update.py
--rw-rw-rw-   0        0        0      739 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:53:54.464419 linkplay-cli-0.0.3/linkplay_cli.egg-info/
--rw-rw-rw-   0        0        0     1161 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:53:54.469422 linkplay-cli-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-06-04 17:53:06.000000 linkplay-cli-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/linkplay_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21069 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/firmware_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/linkplay_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/setup.py
```

### Comparing `linkplay-cli-0.0.3/LICENSE` & `linkplay-cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.3/PKG-INFO` & `linkplay-cli-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-Metadata-Version: 2.1
-Name: linkplay-cli
-Version: 0.0.3
-Summary: Control Linkplay devices from the comfort of your shell
-Home-page: https://github.com/ramikg/linkplay-cli
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Linkplay CLI
-
-Control audio devices supporting the Linkplay API, from the comfort of your shell.  
-Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
-
-![Screenshot](resources/screenshot.png)
-
-# Installation
-```bash
-pip install linkplay-cli
-```
-
-After installing, run `linkplay-cli -h` to get started.
-
-## FAQ
-
-### I'm getting the error `command not found: linkplay-cli` 
-
-The installed script is probably not in your `PATH`.  
-Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
-
-### Some commands have no effect
-
-This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
-For example, most commands won't work when the audio source is YouTube playing from your browser.
-
-
+Metadata-Version: 2.1
+Name: linkplay-cli
+Version: 0.0.4
+Summary: Control Linkplay devices from the comfort of your shell
+Home-page: https://github.com/ramikg/linkplay-cli
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Linkplay CLI
+
+Control audio devices supporting the Linkplay API, from the comfort of your shell.  
+Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
+
+![Screenshot](resources/screenshot.png)
+
+# Installation
+```bash
+pip install linkplay-cli
+```
+
+After installing, run `linkplay-cli -h` to get started.
+
+_(Requirement: Python 3.6+)_
+
+## FAQ
+
+### I'm getting the error `command not found: linkplay-cli` 
+
+The installed script is probably not in your `PATH`.  
+Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
+
+### Some commands have no effect
+
+This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
+For example, most commands won't work when the audio source is YouTube playing from your browser.
```

### Comparing `linkplay-cli-0.0.3/README.md` & `linkplay-cli-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # Installation
 ```bash
 pip install linkplay-cli
 ```
 
 After installing, run `linkplay-cli -h` to get started.
 
+_(Requirement: Python 3.6+)_
+
 ## FAQ
 
 ### I'm getting the error `command not found: linkplay-cli` 
 
 The installed script is probably not in your `PATH`.  
 Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
```

### Comparing `linkplay-cli-0.0.3/linkplay_cli/discovery.py` & `linkplay-cli-0.0.4/linkplay_cli/discovery.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import ipaddress
 
 from async_upnp_client.search import async_search
-import requests
 
 from linkplay_cli import config
 from linkplay_cli.utils import perform_get_request, LinkplayCliGetRequestFailedException
 
 
 class LinkplayCliDeviceNotFoundException(Exception):
     pass
@@ -18,29 +17,29 @@
 def _is_linkplay_ip_address(ip_address):
     if ip_address is None:
         return False
 
     try:
         perform_get_request(f'http://{ip_address}/httpapi.asp?command=setPlayerCmd', verbose=False)
         return True
-    except (requests.exceptions.RequestException, LinkplayCliGetRequestFailedException):
+    except LinkplayCliGetRequestFailedException:
         return False
 
 
 def discover_linkplay_address(verbose):
     try:
         if config.cache_file_path.exists():
             cached_ip_address = ipaddress.IPv4Address(config.cache_file_path.read_text())
             if _is_linkplay_ip_address(cached_ip_address):
                 if verbose:
                     print(f'Using cached IP address {cached_ip_address}')
                 return cached_ip_address
     except ipaddress.AddressValueError:
         print('Cached IP address is corrupted. Rediscovering.')
-    except requests.exceptions.RequestException:
+    except LinkplayCliGetRequestFailedException:
         print('Connection failed. Rediscovering.')
 
     print('Starting device discovery...')
     linkplay_ip_addresses = []
 
     async def add_linkplay_device_to_list(upnp_device):
         device_ip_address = upnp_device.get('_host')
```

### Comparing `linkplay-cli-0.0.3/linkplay_cli/firmware_update.py` & `linkplay-cli-0.0.4/linkplay_cli/firmware_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bs4 import BeautifulSoup
-import requests
 
-from linkplay_cli.utils import perform_get_request
+from linkplay_cli.utils import perform_get_request, LinkplayCliGetRequestFailedException
 
 
 class LinkplayCliFirmwareUpdateNotFoundException(Exception):
     pass
 
 
 def _url_to_xml_soup(url):
@@ -41,21 +40,21 @@
     VERSION_FILE_VERSION_LINE = 0
     VERSION_FILE_RELEASE_DATE_LINE = 5
     HARDWARE_PREFIX = 'WiiMu-'
 
     try:
         version_file_url = _find_version_file_url(update_server_url, model, HARDWARE_PREFIX + hardware)
         version_file_lines = perform_get_request(version_file_url, verbose=verbose).splitlines()
-    except (AttributeError, requests.exceptions.RequestException, LinkplayCliFirmwareUpdateNotFoundException) as e:
+    except (AttributeError, LinkplayCliGetRequestFailedException, LinkplayCliFirmwareUpdateNotFoundException) as e:
         if verbose:
             print(f'Failed retrieving version file from server: {e}, {update_server_url}')
         return
 
     try:
         version = version_file_lines[VERSION_FILE_VERSION_LINE].split('.', maxsplit=1)[1]
         release_date = version_file_lines[VERSION_FILE_RELEASE_DATE_LINE]
-    except (AttributeError, IndexError, requests.exceptions.RequestException) as e:
+    except (AttributeError, IndexError, LinkplayCliGetRequestFailedException) as e:
         if verbose:
             print(f'Failed parsing version file: {e}, {version_file_lines}')
         return
 
     print(f'Latest firmware version: {version} (released {release_date})')
```

### Comparing `linkplay-cli-0.0.3/linkplay_cli.egg-info/PKG-INFO` & `linkplay-cli-0.0.4/linkplay_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-Metadata-Version: 2.1
-Name: linkplay-cli
-Version: 0.0.3
-Summary: Control Linkplay devices from the comfort of your shell
-Home-page: https://github.com/ramikg/linkplay-cli
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Linkplay CLI
-
-Control audio devices supporting the Linkplay API, from the comfort of your shell.  
-Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
-
-![Screenshot](resources/screenshot.png)
-
-# Installation
-```bash
-pip install linkplay-cli
-```
-
-After installing, run `linkplay-cli -h` to get started.
-
-## FAQ
-
-### I'm getting the error `command not found: linkplay-cli` 
-
-The installed script is probably not in your `PATH`.  
-Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
-
-### Some commands have no effect
-
-This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
-For example, most commands won't work when the audio source is YouTube playing from your browser.
-
-
+Metadata-Version: 2.1
+Name: linkplay-cli
+Version: 0.0.4
+Summary: Control Linkplay devices from the comfort of your shell
+Home-page: https://github.com/ramikg/linkplay-cli
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Linkplay CLI
+
+Control audio devices supporting the Linkplay API, from the comfort of your shell.  
+Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
+
+![Screenshot](resources/screenshot.png)
+
+# Installation
+```bash
+pip install linkplay-cli
+```
+
+After installing, run `linkplay-cli -h` to get started.
+
+_(Requirement: Python 3.6+)_
+
+## FAQ
+
+### I'm getting the error `command not found: linkplay-cli` 
+
+The installed script is probably not in your `PATH`.  
+Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
+
+### Some commands have no effect
+
+This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
+For example, most commands won't work when the audio source is YouTube playing from your browser.
```

### Comparing `linkplay-cli-0.0.3/setup.py` & `linkplay-cli-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,24 @@
     long_description = readme.read()
 
 setup(name='linkplay-cli',
       description='Control Linkplay devices from the comfort of your shell',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ramikg/linkplay-cli',
-      version='0.0.3',
+      version='0.0.4',
       packages=find_packages(),
       install_requires=[
           'async_upnp_client',
           'beautifulsoup4',
           'lxml',
+          'prettytable',
           'pycryptodome',
-          'requests'
+          'requests',
+          'urllib3'
       ],
       entry_points={
           'console_scripts': [
               'linkplay-cli = linkplay_cli.cli:main',
           ]
       },
       classifiers=[
```

