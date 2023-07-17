# Comparing `tmp/podaac-data-subscriber-1.9.0.tar.gz` & `tmp/podaac-data-subscriber-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podaac-data-subscriber-1.9.0.tar", last modified: Thu Apr 28 16:50:50 2022, max compression
+gzip compressed data, was "podaac-data-subscriber-1.9.1.tar", max compression
```

## Comparing `podaac-data-subscriber-1.9.0.tar` & `podaac-data-subscriber-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 16:50:50.140699 podaac-data-subscriber-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11336 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5666 2022-04-28 16:50:50.140699 podaac-data-subscriber-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 16:50:50.140699 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5666 2022-04-28 16:50:49.000000 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-04-28 16:50:50.000000 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 16:50:49.000000 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-28 16:50:49.000000 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 16:50:48.000000 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-28 16:50:50.000000 podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-28 16:50:50.140699 podaac-data-subscriber-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 16:50:50.140699 podaac-data-subscriber-1.9.0/subscriber/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15214 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/subscriber/podaac_access.py
--rw-r--r--   0 runner    (1001) docker     (121)    13300 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/subscriber/podaac_data_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15592 2022-04-28 16:50:36.000000 podaac-data-subscriber-1.9.0/subscriber/podaac_data_subscriber.py
+-rw-r--r--   0        0        0    11336 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/LICENSE
+-rw-r--r--   0        0        0     5177 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/README.md
+-rw-r--r--   0        0        0      903 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/subscriber/__init__.py
+-rw-r--r--   0        0        0    15453 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/subscriber/podaac_access.py
+-rw-r--r--   0        0        0    13300 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/subscriber/podaac_data_downloader.py
+-rwxr-xr-x   0        0        0    15592 2022-05-19 17:27:52.365823 podaac-data-subscriber-1.9.1/subscriber/podaac_data_subscriber.py
+-rw-r--r--   0        0        0     6168 2022-05-19 17:28:14.518971 podaac-data-subscriber-1.9.1/setup.py
+-rw-r--r--   0        0        0     5787 2022-05-19 17:28:14.519612 podaac-data-subscriber-1.9.1/PKG-INFO
```

### Comparing `podaac-data-subscriber-1.9.0/LICENSE` & `podaac-data-subscriber-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podaac-data-subscriber-1.9.0/PKG-INFO` & `podaac-data-subscriber-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: podaac-data-subscriber
-Version: 1.9.0
-Summary: PO.DAAC Data Susbcriber Command Line Tool
+Version: 1.9.1
+Summary: PO.DAAC Data Subscriber Command Line Tool
 Home-page: https://github.com/podaac/data-subscriber
+License: Apache-2.0
 Author: PO.DAAC
 Author-email: podaac@podaac.jpl.nasa.gov
-License: apache-2
-Platform: UNKNOWN
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Project-URL: Repository, https://github.com/podaac/data-subscriber
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![Python Build](https://github.com/podaac/data-subscriber/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/podaac/data-subscriber/actions/workflows/python-app.yml)
 [![PyPi release](https://github.com/podaac/data-subscriber/actions/workflows/release.yml/badge.svg)](https://github.com/podaac/data-subscriber/actions/workflows/release.yml)
 
 
 # Scripted Access to PODAAC data
 
@@ -31,25 +38,20 @@
 
 The Downloader is useful if you need to download PO.DAAC data once in a while or prefer to do it "on-demand". The subscriber makes no assumptions about the last time run or what is new in the archive, it simply uses the provided requests and downloads all matching data.
 
 **Subscriber** - [Documentation](Subscriber.md)
 
 The subscriber is useful for users who need to continuously pull the latest data from the PO.DAAC archive. If you feed data into a model or real time process, the subscriber allows you to repeatedly run the script and only download the latest data.
 
-## Dependencies
-
-Aside from **python 3**, the only dependency is the python 'requests' module, which can be installed via pip. Pip is the `package installer for python`. you don't need to know much of anything about python or pip, as long as you have it installed on the machine you're using.
-
-```
-python -m pip install requests
-```
 
 ## Installation
 
-The subscriber and downloader scripes are available in the [pypi python repository](https://pypi.org/project/podaac-data-subscriber/), it can be installed via pip:
+Both subscriber and download require Python >= 3.8.
+
+The subscriber and downloader scripts are available in the [pypi python repository](https://pypi.org/project/podaac-data-subscriber/), it can be installed via pip:
 
 ```
 pip install podaac-data-subscriber
 ```
 
 you should now have access to the downloader and subscriber Command line interfaces:
 
@@ -131,8 +133,7 @@
 
 
 ### In need of Help?
 The PO.DAAC User Services Office is the primary point of contact for answering your questions concerning data and information held by the PO.DAAC. User Services staff members are knowledgeable about both the data ordering system and the data products themselves. We answer questions about data, route requests to other DAACs, and direct questions we cannot answer to the appropriate information source.
 
 Please contact us via email at podaac@podaac.jpl.nasa.gov
 
-
```

### Comparing `podaac-data-subscriber-1.9.0/README.md` & `podaac-data-subscriber-1.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,20 @@
 
 The Downloader is useful if you need to download PO.DAAC data once in a while or prefer to do it "on-demand". The subscriber makes no assumptions about the last time run or what is new in the archive, it simply uses the provided requests and downloads all matching data.
 
 **Subscriber** - [Documentation](Subscriber.md)
 
 The subscriber is useful for users who need to continuously pull the latest data from the PO.DAAC archive. If you feed data into a model or real time process, the subscriber allows you to repeatedly run the script and only download the latest data.
 
-## Dependencies
-
-Aside from **python 3**, the only dependency is the python 'requests' module, which can be installed via pip. Pip is the `package installer for python`. you don't need to know much of anything about python or pip, as long as you have it installed on the machine you're using.
-
-```
-python -m pip install requests
-```
 
 ## Installation
 
-The subscriber and downloader scripes are available in the [pypi python repository](https://pypi.org/project/podaac-data-subscriber/), it can be installed via pip:
+Both subscriber and download require Python >= 3.8.
+
+The subscriber and downloader scripts are available in the [pypi python repository](https://pypi.org/project/podaac-data-subscriber/), it can be installed via pip:
 
 ```
 pip install podaac-data-subscriber
 ```
 
 you should now have access to the downloader and subscriber Command line interfaces:
```

### Comparing `podaac-data-subscriber-1.9.0/podaac_data_subscriber.egg-info/PKG-INFO` & `podaac-data-subscriber-1.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,37 @@
-Metadata-Version: 2.1
-Name: podaac-data-subscriber
-Version: 1.9.0
-Summary: PO.DAAC Data Susbcriber Command Line Tool
-Home-page: https://github.com/podaac/data-subscriber
-Author: PO.DAAC
-Author-email: podaac@podaac.jpl.nasa.gov
-License: apache-2
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-[![Python Build](https://github.com/podaac/data-subscriber/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/podaac/data-subscriber/actions/workflows/python-app.yml)
-[![PyPi release](https://github.com/podaac/data-subscriber/actions/workflows/release.yml/badge.svg)](https://github.com/podaac/data-subscriber/actions/workflows/release.yml)
+packages = \
+['subscriber']
 
+package_data = \
+{'': ['*']}
 
-# Scripted Access to PODAAC data
-
- ----
-
-![N|Solid](https://podaac.jpl.nasa.gov/sites/default/files/image/custom_thumbs/podaac_logo.png)
-
-
-## Subscriber or Bulk Download?
-
-There are 2 tools in this repository, the data subscriber and the data downloader. Which you use depends on your use case. If you're not sure, we'd recommend starting with the downloader.
-
-![Download or Subscribe?](/img/PO.DAAC%20Tools.png)
-
-**Downloader** - [Documentation](Downloader.md)
-
-The Downloader is useful if you need to download PO.DAAC data once in a while or prefer to do it "on-demand". The subscriber makes no assumptions about the last time run or what is new in the archive, it simply uses the provided requests and downloads all matching data.
-
-**Subscriber** - [Documentation](Subscriber.md)
-
-The subscriber is useful for users who need to continuously pull the latest data from the PO.DAAC archive. If you feed data into a model or real time process, the subscriber allows you to repeatedly run the script and only download the latest data.
-
-## Dependencies
-
-Aside from **python 3**, the only dependency is the python 'requests' module, which can be installed via pip. Pip is the `package installer for python`. you don't need to know much of anything about python or pip, as long as you have it installed on the machine you're using.
-
-```
-python -m pip install requests
-```
-
-## Installation
-
-The subscriber and downloader scripes are available in the [pypi python repository](https://pypi.org/project/podaac-data-subscriber/), it can be installed via pip:
-
-```
-pip install podaac-data-subscriber
-```
-
-you should now have access to the downloader and subscriber Command line interfaces:
-
-```
-$> podaac-data-subscriber -h
-usage: podaac_data_subscriber.py [-h] -c COLLECTION -d OUTPUTDIRECTORY [-sd STARTDATE] [-ed ENDDATE] [-b BBOX] [-dc] [-dydoy] [-dymd] [-dy] [--offset OFFSET] [-m MINUTES]
-                                 [-e EXTENSIONS] [--process PROCESS_CMD] [--version] [--verbose] [-p PROVIDER]
-
-...
-```
-
-```
-$> podaac-data-downloader -h
-usage: PO.DAAC bulk-data downloader [-h] -c COLLECTION -d OUTPUTDIRECTORY [--cycle SEARCH_CYCLES] [-sd STARTDATE] [-ed ENDDATE] [-b BBOX] [-dc] [-dydoy] [-dymd] [-dy] [--offset OFFSET] [-e EXTENSIONS] [--process PROCESS_CMD] [--version] [--verbose] [-p PROVIDER] [--limit LIMIT]
-
-...
-```
-
-## Step 1:  Get Earthdata Login     
-This step is needed only if you dont have an Earthdata login already.
-https://urs.earthdata.nasa.gov/
-> The Earthdata Login provides a single mechanism for user registration and profile  management for all EOSDIS system components (DAACs, Tools, Services). Your Earthdata login   also helps the EOSDIS program better understand the usage of EOSDIS services to improve  user experience through customization of tools and improvement of services. EOSDIS data are  openly available to all and free of charge except where governed by international  agreements.
-
-For setting up your authentication, see the notes on the `netrc` file below.
-
-## Step 2: Setup your Earthdata Login
-The netrc used within the script  will allow Python scripts to log into any Earthdata Login without being prompted for
-credentials every time you run. The netrc file should be placed in your HOME directory.
-To find the location of your HOME directory
-
-On UNIX you can use
-```
-echo $HOME
-```
-On Windows you can use
-```
-echo %HOMEDRIVE%%HOMEPATH%
-```
-
-The output location from the command above should be the location of the `.netrc` (`_netrc` on Windows) file.
-
-The format of the `netrc` file is as follows:
-
-```
-machine urs.earthdata.nasa.gov
-    login <your username>
-    password <your password>
-```
-for example:
-
-```
-machine urs.earthdata.nasa.gov
-    login podaacUser
-    password podaacIsAwesome
-```
-
-**If the script cannot find the netrc file, you will be prompted to enter the username and password and the script wont be able to generate the CMR token**
-
-
-## Advanced Usage
-
-### Request data from another DAAC...
-
-Use the 'provider' flag to point at a non-PO.DAAC provider. Be aware, the default data types (--extensions) may need to be specified if the desired data are not in the defaults.
-
-```
-podaac-data-subscriber -c SENTINEL-1A_SLC -d myData  -p ASF -sd 2014-06-01T00:46:02Z
-```
-
-### Logging
-
-For error troubleshooting, one can set an environment variable to gain more insight into errors:
-
-```
-export PODAAC_LOGLEVEL=DEBUG
-```
-
-And then run the script. This should give you more verbose output on URL requests to CMR, tokens, etc.
-
-
-### In need of Help?
-The PO.DAAC User Services Office is the primary point of contact for answering your questions concerning data and information held by the PO.DAAC. User Services staff members are knowledgeable about both the data ordering system and the data products themselves. We answer questions about data, route requests to other DAACs, and direct questions we cannot answer to the appropriate information source.
-
-Please contact us via email at podaac@podaac.jpl.nasa.gov
+install_requires = \
+['requests>=2.27.1,<3.0.0', 'tenacity>=8.0.1,<9.0.0']
+
+entry_points = \
+{'console_scripts': ['podaac-data-downloader = '
+                     'subscriber.podaac_data_downloader:main',
+                     'podaac-data-subscriber = '
+                     'subscriber.podaac_data_subscriber:main']}
+
+setup_kwargs = {
+    'name': 'podaac-data-subscriber',
+    'version': '1.9.1',
+    'description': 'PO.DAAC Data Subscriber Command Line Tool',
+    'long_description': '[![Python Build](https://github.com/podaac/data-subscriber/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/podaac/data-subscriber/actions/workflows/python-app.yml)\n[![PyPi release](https://github.com/podaac/data-subscriber/actions/workflows/release.yml/badge.svg)](https://github.com/podaac/data-subscriber/actions/workflows/release.yml)\n\n\n# Scripted Access to PODAAC data\n\n ----\n\n![N|Solid](https://podaac.jpl.nasa.gov/sites/default/files/image/custom_thumbs/podaac_logo.png)\n\n\n## Subscriber or Bulk Download?\n\nThere are 2 tools in this repository, the data subscriber and the data downloader. Which you use depends on your use case. If you\'re not sure, we\'d recommend starting with the downloader.\n\n![Download or Subscribe?](/img/PO.DAAC%20Tools.png)\n\n**Downloader** - [Documentation](Downloader.md)\n\nThe Downloader is useful if you need to download PO.DAAC data once in a while or prefer to do it "on-demand". The subscriber makes no assumptions about the last time run or what is new in the archive, it simply uses the provided requests and downloads all matching data.\n\n**Subscriber** - [Documentation](Subscriber.md)\n\nThe subscriber is useful for users who need to continuously pull the latest data from the PO.DAAC archive. If you feed data into a model or real time process, the subscriber allows you to repeatedly run the script and only download the latest data.\n\n\n## Installation\n\nBoth subscriber and download require Python >= 3.8.\n\nThe subscriber and downloader scripts are available in the [pypi python repository](https://pypi.org/project/podaac-data-subscriber/), it can be installed via pip:\n\n```\npip install podaac-data-subscriber\n```\n\nyou should now have access to the downloader and subscriber Command line interfaces:\n\n```\n$> podaac-data-subscriber -h\nusage: podaac_data_subscriber.py [-h] -c COLLECTION -d OUTPUTDIRECTORY [-sd STARTDATE] [-ed ENDDATE] [-b BBOX] [-dc] [-dydoy] [-dymd] [-dy] [--offset OFFSET] [-m MINUTES]\n                                 [-e EXTENSIONS] [--process PROCESS_CMD] [--version] [--verbose] [-p PROVIDER]\n\n...\n```\n\n```\n$> podaac-data-downloader -h\nusage: PO.DAAC bulk-data downloader [-h] -c COLLECTION -d OUTPUTDIRECTORY [--cycle SEARCH_CYCLES] [-sd STARTDATE] [-ed ENDDATE] [-b BBOX] [-dc] [-dydoy] [-dymd] [-dy] [--offset OFFSET] [-e EXTENSIONS] [--process PROCESS_CMD] [--version] [--verbose] [-p PROVIDER] [--limit LIMIT]\n\n...\n```\n\n## Step 1:  Get Earthdata Login     \nThis step is needed only if you dont have an Earthdata login already.\nhttps://urs.earthdata.nasa.gov/\n> The Earthdata Login provides a single mechanism for user registration and profile  management for all EOSDIS system components (DAACs, Tools, Services). Your Earthdata login   also helps the EOSDIS program better understand the usage of EOSDIS services to improve  user experience through customization of tools and improvement of services. EOSDIS data are  openly available to all and free of charge except where governed by international  agreements.\n\nFor setting up your authentication, see the notes on the `netrc` file below.\n\n## Step 2: Setup your Earthdata Login\nThe netrc used within the script  will allow Python scripts to log into any Earthdata Login without being prompted for\ncredentials every time you run. The netrc file should be placed in your HOME directory.\nTo find the location of your HOME directory\n\nOn UNIX you can use\n```\necho $HOME\n```\nOn Windows you can use\n```\necho %HOMEDRIVE%%HOMEPATH%\n```\n\nThe output location from the command above should be the location of the `.netrc` (`_netrc` on Windows) file.\n\nThe format of the `netrc` file is as follows:\n\n```\nmachine urs.earthdata.nasa.gov\n    login <your username>\n    password <your password>\n```\nfor example:\n\n```\nmachine urs.earthdata.nasa.gov\n    login podaacUser\n    password podaacIsAwesome\n```\n\n**If the script cannot find the netrc file, you will be prompted to enter the username and password and the script wont be able to generate the CMR token**\n\n\n## Advanced Usage\n\n### Request data from another DAAC...\n\nUse the \'provider\' flag to point at a non-PO.DAAC provider. Be aware, the default data types (--extensions) may need to be specified if the desired data are not in the defaults.\n\n```\npodaac-data-subscriber -c SENTINEL-1A_SLC -d myData  -p ASF -sd 2014-06-01T00:46:02Z\n```\n\n### Logging\n\nFor error troubleshooting, one can set an environment variable to gain more insight into errors:\n\n```\nexport PODAAC_LOGLEVEL=DEBUG\n```\n\nAnd then run the script. This should give you more verbose output on URL requests to CMR, tokens, etc.\n\n\n### In need of Help?\nThe PO.DAAC User Services Office is the primary point of contact for answering your questions concerning data and information held by the PO.DAAC. User Services staff members are knowledgeable about both the data ordering system and the data products themselves. We answer questions about data, route requests to other DAACs, and direct questions we cannot answer to the appropriate information source.\n\nPlease contact us via email at podaac@podaac.jpl.nasa.gov\n',
+    'author': 'PO.DAAC',
+    'author_email': 'podaac@podaac.jpl.nasa.gov',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': 'https://github.com/podaac/data-subscriber',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
+    'python_requires': '>=3.8,<4.0',
+}
 
 
+setup(**setup_kwargs)
```

### Comparing `podaac-data-subscriber-1.9.0/subscriber/podaac_access.py` & `podaac-data-subscriber-1.9.1/subscriber/podaac_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import requests
 
 import requests
 import tenacity
 from datetime import datetime
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 extensions = [".nc", ".h5", ".zip", ".tar.gz"]
 edl = "urs.earthdata.nasa.gov"
 cmr = "cmr.earthdata.nasa.gov"
 token_url = "https://" + cmr + "/legacy-services/rest/tokens"
 
 IPAddr = "127.0.0.1"  # socket.gethostbyname(hostname)
 
@@ -347,15 +347,14 @@
     except KeyError:
         raise ValueError('No cycles found within collection granules. '
                          'Specify an output directory or '
                          'choose another output directory flag other than -dc.')  # noqa E501
     return cycles
 
 
-
 def extract_checksums(granule_results):
     """
     Create a dictionary containing checksum information from files.
 
     Parameters
     ----------
     granule_results : dict
@@ -411,22 +410,27 @@
     True - if the file's checksum matches a checksum in the checksum dict
     False - if the file doesn't have a checksum, or if the checksum doesn't match
     """
     filename = basename(file_path)
     checksum = checksums.get(filename)
     if not checksum:
         return False
-    return make_checksum(file_path, checksum["Algorithm"]) == checksum["Value"]
+
+    computed_checksum = make_checksum(file_path, checksum["Algorithm"])
+    checksums_match = computed_checksum == checksum["Value"]
+    if not checksums_match:
+        logging.warning(f'Computed checksum {computed_checksum} does not match expected checksum {checksum["Value"]}')
+    return checksums_match
 
 
 def make_checksum(file_path, algorithm):
     """
     Create checksum of file using the specified algorithm
     """
     # Based on https://stackoverflow.com/questions/3431825/generating-an-md5-checksum-of-a-file#answer-3431838
     # with modification to handle multiple algorithms
-    hash = getattr(hashlib, algorithm.lower())()
+    hash_alg = getattr(hashlib, algorithm.lower())()
 
     with open(file_path, 'rb') as f:
         for chunk in iter(lambda: f.read(4096), b""):
-            hash.update(chunk)
-    return hash.hexdigest()
+            hash_alg.update(chunk)
+    return hash_alg.hexdigest()
```

### Comparing `podaac-data-subscriber-1.9.0/subscriber/podaac_data_downloader.py` & `podaac-data-subscriber-1.9.1/subscriber/podaac_data_downloader.py`

 * *Files identical despite different names*

### Comparing `podaac-data-subscriber-1.9.0/subscriber/podaac_data_subscriber.py` & `podaac-data-subscriber-1.9.1/subscriber/podaac_data_subscriber.py`

 * *Files identical despite different names*

