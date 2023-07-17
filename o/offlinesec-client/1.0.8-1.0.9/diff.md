# Comparing `tmp/offlinesec_client-1.0.8.tar.gz` & `tmp/offlinesec_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinesec_client-1.0.8.tar", last modified: Fri Jul  7 20:31:10 2023, max compression
+gzip compressed data, was "offlinesec_client-1.0.9.tar", last modified: Sat Jul  8 08:52:31 2023, max compression
```

## Comparing `offlinesec_client-1.0.8.tar` & `offlinesec_client-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 20:31:10.526014 offlinesec_client-1.0.8/
--rw-rw-rw-   0        0        0     2382 2023-07-07 20:31:10.525012 offlinesec_client-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2137 2023-07-02 14:04:21.000000 offlinesec_client-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 20:31:10.516991 offlinesec_client-1.0.8/offlinesec_client/
--rw-rw-rw-   0        0        0       23 2023-07-07 16:49:27.000000 offlinesec_client-1.0.8/offlinesec_client/__init__.py
--rw-rw-rw-   0        0        0       81 2023-07-02 10:37:26.000000 offlinesec_client-1.0.8/offlinesec_client/__main__.py
--rw-rw-rw-   0        0        0     2892 2023-07-07 16:49:27.000000 offlinesec_client-1.0.8/offlinesec_client/config.py
--rw-rw-rw-   0        0        0      219 2023-06-28 20:09:51.000000 offlinesec_client-1.0.8/offlinesec_client/const.py
--rw-rw-rw-   0        0        0     1045 2023-07-07 15:40:58.000000 offlinesec_client-1.0.8/offlinesec_client/func.py
--rw-rw-rw-   0        0        0     3189 2023-07-07 15:46:18.000000 offlinesec_client-1.0.8/offlinesec_client/get_reports.py
--rw-rw-rw-   0        0        0     2414 2023-07-07 15:46:18.000000 offlinesec_client-1.0.8/offlinesec_client/req_notes_report.py
-drwxrwxrwx   0        0        0        0 2023-07-07 20:31:10.524010 offlinesec_client-1.0.8/offlinesec_client.egg-info/
--rw-rw-rw-   0        0        0     2382 2023-07-07 20:31:10.000000 offlinesec_client-1.0.8/offlinesec_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-07-07 20:31:10.000000 offlinesec_client-1.0.8/offlinesec_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 20:31:10.000000 offlinesec_client-1.0.8/offlinesec_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-07-07 20:31:10.000000 offlinesec_client-1.0.8/offlinesec_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-07 20:31:10.000000 offlinesec_client-1.0.8/offlinesec_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-07 20:31:10.000000 offlinesec_client-1.0.8/offlinesec_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 20:31:10.526014 offlinesec_client-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      896 2023-07-02 10:22:37.000000 offlinesec_client-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:52:31.432901 offlinesec_client-1.0.9/
+-rw-rw-rw-   0        0        0     3418 2023-07-08 08:52:31.431899 offlinesec_client-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3173 2023-07-08 07:35:59.000000 offlinesec_client-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 08:52:31.424879 offlinesec_client-1.0.9/offlinesec_client/
+-rw-rw-rw-   0        0        0       23 2023-07-08 07:39:01.000000 offlinesec_client-1.0.9/offlinesec_client/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-07-02 10:37:26.000000 offlinesec_client-1.0.9/offlinesec_client/__main__.py
+-rw-rw-rw-   0        0        0     2892 2023-07-07 16:49:27.000000 offlinesec_client-1.0.9/offlinesec_client/config.py
+-rw-rw-rw-   0        0        0      219 2023-06-28 20:09:51.000000 offlinesec_client-1.0.9/offlinesec_client/const.py
+-rw-rw-rw-   0        0        0     1045 2023-07-07 15:40:58.000000 offlinesec_client-1.0.9/offlinesec_client/func.py
+-rw-rw-rw-   0        0        0     3189 2023-07-07 15:46:18.000000 offlinesec_client-1.0.9/offlinesec_client/get_reports.py
+-rw-rw-rw-   0        0        0     2414 2023-07-07 15:46:18.000000 offlinesec_client-1.0.9/offlinesec_client/req_notes_report.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:52:31.430894 offlinesec_client-1.0.9/offlinesec_client.egg-info/
+-rw-rw-rw-   0        0        0     3418 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 08:52:31.432901 offlinesec_client-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      896 2023-07-02 10:22:37.000000 offlinesec_client-1.0.9/setup.py
```

### Comparing `offlinesec_client-1.0.8/README.md` & `offlinesec_client-1.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-#Offline Security Client
+# Offline Security Client
 
-Offline Security is 
+Offline Security is new IT Security Project like no other. It based on client-server model. You collect yourself all the necessary data for analysis, send it to server and get the report.
+Analysis is performed on the server side.<br />
+We don't require any client-specific information (email, company, ip address). That's why we can't link the analysis results with particular company or particular SAP system. The Analysis performed fully anonymously! <br />
+All sensitive information like SAPSIDs, ip addresses, server names, role names, and so on will be masked. That's why we need client software.
 
 ## Table of contents
 
 * [Installation](#installation)
 * [Quick Start](#quick-start)
 * [Use Cases](#use-cases)
 * [Important Notes](#important-notes)
@@ -13,48 +16,61 @@
 
 ### Python installation
 Install last version of Python [from here](https://www.python.org/downloads/)
 
 ### Published version installation (recommended)
 ```sh
 pip install offlinesec_client
+or
+python -m pip install offlinesec_client
 ```
 
-### Installation from repository on [github.com](https://github.com/offlinesec/offlinesec-client)
+### Installation last version from repository on [github.com](https://github.com/offlinesec/offlinesec-client)
 ```sh
 git clone git@github.com:offlinesec/offlinesec-client.git
 python -m pip install --upgrade pip
 pip install setuptools wheel
 python setup.py bdist_wheel
-python3 -m pip install dist\offlinesec_client-1.0.1-py3-none-any.whl
+python3 -m pip install dist\offlinesec_client-1.0.8-py3-none-any.whl
+```
+The Version could be different! Please verify generated wheel name. 
+
+### Upgrade to last published version
+```sh
+pip install --upgrade offlinesec_client
 ```
-The Version could be different. Please verify generated wheel name. 
 
 ## Quick Start
 
-To check your SAP system against SAP Security Notes:
-1. Prepare text file with installed software component versions ([details](./docs/how_to_prepare_sap_softs.md))
+How to discovery missed SAP Security Notes:
+1. Prepare text file with installed SAP software component versions ([details](./docs/how_to_prepare_sap_softs.md))
 2. Send prepared file to server (optional you can set SAP system name):
 ```sh
 offlinesec_sap_notes -f "software_components.txt" -s "Demo System"
 ```
 3. Wait aprox 5 minutes (Depends on server load)
-4. Download report:
+4. Download your report:
 ```sh
 offlinesec_get_reports
 ```
-5. Find your report in Downloads folder. Enjoy.
+5. Find your downloaded report in Downloads folder. Enjoy.
 
 ## Use Cases
-
 1. SAP Security Notes Analysis (Vulnerabilities Check)
 * [How to prepare data and request report](./docs/how_to_prepare_sap_softs.md)
 * [Report example](./docs/sap_security_notes_report.md)
-* Our knowledge base is constantly updated. You can find the date of last loaded SAP Security Note in your report.
+* Our knowledge base is constantly updated and contain all SAP security notes released in 2015-2023. You can find the date of last loaded SAP Security Note in your report.
+
+2. Profile Parameters/Compliance Analysis
+* Will be available in next releases
+
+3. Role/Privilege Analysis
+* Will be available in next releases
 
 ## Important Notes:
-1. We don't collect any client identity like email address, SAP SIDs, ip addresses. All Checks are performed fully anonymously.
+1. We don't collect any client identity like email address, SAP SIDs, company, ip addresses. All Checks are performed fully anonymously.
 2. The reports aren't stored on server side. Once you have downloaded the report it's deleted.
-3. The report could download only the person who has token (Random String generated on first start).
-4. You can download reports within 10 days after it was requested.
+3. All data transferred to server are encrypted with HTTPS protocol. 
+4. The report could download only the person who has token (Random String generated on first start).
+5. You can download reports within 10 days after it was requested.
 
-Additional information is available [here](./docs/README.md)
+Additional documentation is available [here](./docs/README.md)
```

### Comparing `offlinesec_client-1.0.8/offlinesec_client/config.py` & `offlinesec_client-1.0.9/offlinesec_client/config.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.0.8/offlinesec_client/func.py` & `offlinesec_client-1.0.9/offlinesec_client/func.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.0.8/offlinesec_client/get_reports.py` & `offlinesec_client-1.0.9/offlinesec_client/get_reports.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.0.8/offlinesec_client/req_notes_report.py` & `offlinesec_client-1.0.9/offlinesec_client/req_notes_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.0.8/setup.py` & `offlinesec_client-1.0.9/setup.py`

 * *Files identical despite different names*

