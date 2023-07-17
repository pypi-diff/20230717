# Comparing `tmp/cmo_nnect-0.0.2.tar.gz` & `tmp/cmo_nnect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cmo_nnect-0.0.2.tar", last modified: Wed Jun 14 13:02:44 2023, max compression
+gzip compressed data, was "dist\cmo_nnect-0.1.0.tar", last modified: Mon Jul 17 13:44:28 2023, max compression
```

## Comparing `cmo_nnect-0.0.2.tar` & `cmo_nnect-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/
--rw-rw-rw-   0        0        0    35129 2023-06-14 13:01:56.000000 cmo_nnect-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4383 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3405 2023-06-14 13:01:56.000000 cmo_nnect-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect/
--rw-rw-rw-   0        0        0       82 2023-06-14 13:01:58.000000 cmo_nnect-0.0.2/cmo_nnect/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-06-14 13:01:58.000000 cmo_nnect-0.0.2/cmo_nnect/afasprofit.py
--rw-rw-rw-   0        0        0     2065 2023-06-14 13:01:58.000000 cmo_nnect-0.0.2/cmo_nnect/nmbrs.py
--rw-rw-rw-   0        0        0     1569 2023-06-14 13:01:58.000000 cmo_nnect-0.0.2/cmo_nnect/test_afasprofit.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect.egg-info/
--rw-rw-rw-   0        0        0     4383 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/cmo_nnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 13:02:44.000000 cmo_nnect-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-06-14 13:01:57.000000 cmo_nnect-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/
+-rw-rw-rw-   0        0        0    35129 2023-07-17 13:43:51.000000 cmo_nnect-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5627 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4457 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect/
+-rw-rw-rw-   0        0        0      146 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/afasprofit.py
+-rw-rw-rw-   0        0        0     7788 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/businesscentral.py
+-rw-rw-rw-   0        0        0     4002 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/mautic.py
+-rw-rw-rw-   0        0        0     2065 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/nmbrs.py
+-rw-rw-rw-   0        0        0     1569 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/test_afasprofit.py
+-rw-rw-rw-   0        0        0     2455 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/test_businesscentral.py
+-rw-rw-rw-   0        0        0     2600 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/cmo_nnect/test_mautic.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect.egg-info/
+-rw-rw-rw-   0        0        0     5627 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/cmo_nnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:44:28.000000 cmo_nnect-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-07-17 13:43:52.000000 cmo_nnect-0.1.0/setup.py
```

### Comparing `cmo_nnect-0.0.2/LICENSE` & `cmo_nnect-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.0.2/PKG-INFO` & `cmo_nnect-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,98 @@
-Metadata-Version: 2.1
-Name: cmo_nnect
-Version: 0.0.2
-Summary: Connect with a variety of API's with ease.
-Home-page: https://dev.azure.com/Cmotions/Packages/_git/cmo_nnect
-Author: Thijs van der Velden, Koen Leijsten
-Author-email: service@cmotions.nl
-License: UNKNOWN
-Description: # Cmotions Nnect
-        cmo_nnect is a Python library created by [Cmotions](https://cmotions.nl/). This library aims to ease the interaction with different API's of software packages. Examples include Microsoft Dynamics, Exact Online, AFAS Profit etc. You only need the right authentication credentials, and the target endpoints of the source/destination API to start interacting!
-        
-        From our experience with integrating data from a variety of software packages we decided to publish our connectors to ease the use of the API's with Python. We encourage collaboration to increase the number of connectors and improvements of existing connectors!
-        
-        The library always returns a Pandas dataframe by default.
-        
-        ## Installation
-        Install cmo_nnect using pip
-        ```bash
-        pip install cmo-nnect
-        ```
-        
-        ## Usage
-        Choose the [connector](#Available-connectors) from the list, and import the connector by using the reference name. For example for AFAS Profit the reference name is afasprofit:
-        ```bash
-        from cmo_nnect import afasprofit
-        ```
-        From the [connector usage documentation](#Connector-usage) determine the authentication requirements, for example for AFAS Profit we need a token, a company-id, and an optional environment name. We can then initialize a client:
-        ```bash
-        # define authentication credentials
-        token = "<token><version>1</version><data>54740093832496081845474abcdefghijklmnopq740093832496081841234127</data></token>"
-        company_id = 12345
-        environment = "development"
-        
-        # set up a client to ease interaction
-        client = afasprofit(token,company_id)
-        ```
-        We are now able to start interacting with the API. To extract data you can use the format client.get_data(). In the documentation of the specific connector you can see what is expected for the specific method. For example for AFAS Profit we need to provide a get_connector name, and optional parameters:
-        ```bash
-        # define parameters
-        params = {"skip": "-1", "take": "-1"}
-        
-        # extract data from the software package
-        contacts = client.get_data("get_contacts", params)
-        ```
-        ## Available connectors
-        - [AFAS Profit](https://help.afas.nl/help/NL/SE/App_Cnr_Rest_Api.htm) (afasprofit)
-        - [Nmbrs](https://support.nmbrs.nl/hc/nl/articles/205903718-Visma-Nmbrs-API-for-developers-) (nmbrs)
-        
-        ## Connector usage
-        ### AFAS Profit
-        **Authentication**<br>
-        To authenticate with AFAS Profit you need:
-        - A profit token (e.g. "<token><version>1</version><data>54740093832496081845474abcdefghijklmnopq740093832496081841234127</data></token>")
-        - A company ID (e.g. 12345)
-        Optionally:
-        - An environment, defaults to production (e.g. "test")
-        
-        **Interaction**<br>
-        For each interaction you can provide optional parameters in a dictionary (e.g. {"skip": "-1", "take": "-1"}).
-        
-        **Extracting data**<br>
-        To get data, you need:
-        - A get_connector name of a get connector which is [set-up in AFAS profit](https://help.afas.nl/help/NL/SE/App_Apps_Custom_Add.htm) (e.g. "get_contacts")
-        
-        **Inserting data**<br>
-        T.B.A.
-        
-        **Updating data**<br>
-        T.B.A.
-        
-        **Deleting data**<br>
-        T.B.A.
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
-        
-        ## License
-        [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
-        
-        ## Contributors
-        Thijs van der Velden, Koen Leijsten<br>
-        [Contact us](mailto:info@cmotions.nl)
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+# Cmotions Nnect
+cmo_nnect is a Python library created by [Cmotions](https://cmotions.nl/). This library aims to ease the interaction with different API's of software packages. Examples include Microsoft Dynamics, Exact Online, AFAS Profit etc. You only need the right authentication credentials, and the target endpoints of the source/destination API to start interacting!
+
+From our experience with integrating data from a variety of software packages we decided to publish our connectors to ease the use of the API's with Python. We encourage collaboration to increase the number of connectors and improvements of existing connectors!
+
+The library always returns a Pandas dataframe by default.
+
+## Installation
+Install cmo_nnect using pip
+```bash
+pip install cmo-nnect
+```
+
+## Usage
+Choose the [connector](#Available-connectors) from the list, and import the connector by using the reference name. For example for AFAS Profit the reference name is afasprofit:
+```bash
+from cmo_nnect import afasprofit
+```
+From the [connector usage documentation](#Connector-usage) determine the authentication requirements, for example for AFAS Profit we need a token, a company-id, and an optional environment name. We can then initialize a client:
+```bash
+# define authentication credentials
+token = "<token><version>1</version><data>54740093832496081845474abcdefghijklmnopq740093832496081841234127</data></token>"
+company_id = 12345
+environment = "development"
+
+# set up a client to ease interaction
+client = afasprofit(token,company_id)
+```
+We are now able to start interacting with the API. To extract data you can use the format client.get_data(). In the documentation of the specific connector you can see what is expected for the specific method. For example for AFAS Profit we need to provide a get_connector name, and optional parameters:
+```bash
+# define parameters
+params = {"skip": "-1", "take": "-1"}
+
+# extract data from the software package
+contacts = client.get_data("get_contacts", params)
+```
+## Available connectors
+- [AFAS Profit](https://help.afas.nl/help/NL/SE/App_Cnr_Rest_Api.htm) (afasprofit)
+- [Nmbrs](https://support.nmbrs.nl/hc/nl/articles/205903718-Visma-Nmbrs-API-for-developers-) (nmbrs)
+- [Mautic](https://developer.mautic.org/#rest-api) (mautic)
+
+## Connector usage
+### AFAS Profit
+**Authentication**<br>
+To authenticate with AFAS Profit you need:
+- A profit token (e.g. "<token><version>1</version><data>54740093832496081845474abcdefghijklmnopq740093832496081841234127</data></token>")
+- A company ID (e.g. 12345)
+Optionally:
+- An environment, defaults to production (e.g. "test")
+
+**Interaction**<br>
+For each interaction you can provide optional parameters in a dictionary (e.g. {"skip": "-1", "take": "-1"}).
+
+**Extracting data**<br>
+To get data, you need:
+- A get_connector name of a get connector which is [set-up in AFAS profit](https://help.afas.nl/help/NL/SE/App_Apps_Custom_Add.htm) (e.g. "get_contacts")
+
+**Inserting data**<br>
+T.B.A.
+
+**Updating data**<br>
+T.B.A.
+
+**Deleting data**<br>
+T.B.A.
+
+### Mautic
+**Authentication**<br>
+To authenticate with Mautic you need:
+- A company name, you can find the company name in the url of your mautic instance (e.g. cmotions)
+- A client id, the client id will be generated when the mautic administrator enables the API. Check the [Mautic documentation](https://developer.mautic.org/#authorization) for setting this up.
+- A client secret, the client secret will be generated when the mautic administrator enables the API. Check the [Mautic documentation](https://developer.mautic.org/#authorization) for setting this up.
+
+**Interaction**<br>
+For each interaction you can provide optional parameters in a dictionary (e.g. "limit=10&minimal=true").
+
+**Extracting data**<br>
+To get data, you need:
+- A entity name, check the [Mautic documentation](https://developer.mautic.org/#endpoints) for the available entities (e.g. "campaigns")
+
+**Inserting data**<br>
+T.B.A.
+
+**Updating data**<br>
+T.B.A.
+
+**Deleting data**<br>
+T.B.A.
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
+
+## License
+[GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
+
+## Contributors
+Thijs van der Velden, Koen Leijsten<br>
+[Contact us](mailto:info@cmotions.nl)
```

### Comparing `cmo_nnect-0.0.2/cmo_nnect/afasprofit.py` & `cmo_nnect-0.1.0/cmo_nnect/afasprofit.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.0.2/cmo_nnect/nmbrs.py` & `cmo_nnect-0.1.0/cmo_nnect/nmbrs.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.0.2/cmo_nnect/test_afasprofit.py` & `cmo_nnect-0.1.0/cmo_nnect/test_afasprofit.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.0.2/cmo_nnect.egg-info/PKG-INFO` & `cmo_nnect-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmo-nnect
-Version: 0.0.2
+Name: cmo_nnect
+Version: 0.1.0
 Summary: Connect with a variety of API's with ease.
 Home-page: https://dev.azure.com/Cmotions/Packages/_git/cmo_nnect
 Author: Thijs van der Velden, Koen Leijsten
 Author-email: service@cmotions.nl
 License: UNKNOWN
 Description: # Cmotions Nnect
         cmo_nnect is a Python library created by [Cmotions](https://cmotions.nl/). This library aims to ease the interaction with different API's of software packages. Examples include Microsoft Dynamics, Exact Online, AFAS Profit etc. You only need the right authentication credentials, and the target endpoints of the source/destination API to start interacting!
@@ -41,14 +41,15 @@
         
         # extract data from the software package
         contacts = client.get_data("get_contacts", params)
         ```
         ## Available connectors
         - [AFAS Profit](https://help.afas.nl/help/NL/SE/App_Cnr_Rest_Api.htm) (afasprofit)
         - [Nmbrs](https://support.nmbrs.nl/hc/nl/articles/205903718-Visma-Nmbrs-API-for-developers-) (nmbrs)
+        - [Mautic](https://developer.mautic.org/#rest-api) (mautic)
         
         ## Connector usage
         ### AFAS Profit
         **Authentication**<br>
         To authenticate with AFAS Profit you need:
         - A profit token (e.g. "<token><version>1</version><data>54740093832496081845474abcdefghijklmnopq740093832496081841234127</data></token>")
         - A company ID (e.g. 12345)
@@ -64,14 +65,37 @@
         
         **Inserting data**<br>
         T.B.A.
         
         **Updating data**<br>
         T.B.A.
         
+        **Deleting data**<br>
+        T.B.A.
+        
+        ### Mautic
+        **Authentication**<br>
+        To authenticate with Mautic you need:
+        - A company name, you can find the company name in the url of your mautic instance (e.g. cmotions)
+        - A client id, the client id will be generated when the mautic administrator enables the API. Check the [Mautic documentation](https://developer.mautic.org/#authorization) for setting this up.
+        - A client secret, the client secret will be generated when the mautic administrator enables the API. Check the [Mautic documentation](https://developer.mautic.org/#authorization) for setting this up.
+        
+        **Interaction**<br>
+        For each interaction you can provide optional parameters in a dictionary (e.g. "limit=10&minimal=true").
+        
+        **Extracting data**<br>
+        To get data, you need:
+        - A entity name, check the [Mautic documentation](https://developer.mautic.org/#endpoints) for the available entities (e.g. "campaigns")
+        
+        **Inserting data**<br>
+        T.B.A.
+        
+        **Updating data**<br>
+        T.B.A.
+        
         **Deleting data**<br>
         T.B.A.
         
         ## Contributing
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
         
         ## License
```

### Comparing `cmo_nnect-0.0.2/setup.py` & `cmo_nnect-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="cmo_nnect",
-    version="0.0.2",
+    version="0.1.0",
     python_requires=">=3.8",
     description="Connect with a variety of API's with ease.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Thijs van der Velden, Koen Leijsten",
     author_email="service@cmotions.nl",
-    keyword = ['API', 'Connector', 'Connectors', 'Dynamics', 'AFAS Profit', 'Profit', 'Nmbrs'],
+    keyword = ['API', 'Connector', 'Connectors', 'Dynamics', 'AFAS Profit', 'Profit', 'Nmbrs', 'Mautic'],
     url="https://dev.azure.com/Cmotions/Packages/_git/cmo_nnect",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "requests",
         "zeep",
     ],
```

