# Comparing `tmp/pyngeso-0.3.3.tar.gz` & `tmp/pyngeso-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyngeso-0.3.3.tar", max compression
+gzip compressed data, was "pyngeso-0.3.4.tar", max compression
```

## Comparing `pyngeso-0.3.3.tar` & `pyngeso-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2022-04-08 15:15:01.390564 pyngeso-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0     1243 2022-08-23 09:21:13.955327 pyngeso-0.3.3/README.md
--rw-r--r--   0        0        0       50 2023-01-04 14:14:16.785879 pyngeso-0.3.3/pyngeso/__init__.py
--rwxr-xr-x   0        0        0      500 2022-04-08 15:15:01.391437 pyngeso-0.3.3/pyngeso/configure_logging.py
--rw-r--r--   0        0        0       47 2022-04-08 15:15:01.391533 pyngeso-0.3.3/pyngeso/exceptions.py
--rw-r--r--   0        0        0     6885 2022-08-23 09:21:13.955678 pyngeso-0.3.3/pyngeso/pyngeso.py
--rw-r--r--   0        0        0     9015 2023-01-04 14:12:51.131393 pyngeso-0.3.3/pyngeso/resources.py
--rw-r--r--   0        0        0     1439 2023-01-04 14:13:07.406113 pyngeso-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1973 2023-01-04 14:30:25.564521 pyngeso-0.3.3/setup.py
--rw-r--r--   0        0        0     2144 2023-01-04 14:30:25.564712 pyngeso-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-08-23 07:06:37.475514 pyngeso-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0     1347 2023-07-17 10:53:01.250035 pyngeso-0.3.4/README.md
+-rw-r--r--   0        0        0       50 2023-07-17 09:49:24.628549 pyngeso-0.3.4/pyngeso/__init__.py
+-rwxr-xr-x   0        0        0      500 2022-08-23 07:06:37.476423 pyngeso-0.3.4/pyngeso/configure_logging.py
+-rw-r--r--   0        0        0       47 2022-08-23 07:06:37.476508 pyngeso-0.3.4/pyngeso/exceptions.py
+-rw-r--r--   0        0        0     6876 2023-07-17 10:53:01.250726 pyngeso-0.3.4/pyngeso/pyngeso.py
+-rw-r--r--   0        0        0     9720 2023-07-17 10:53:01.251152 pyngeso-0.3.4/pyngeso/resources.py
+-rw-r--r--   0        0        0     1439 2023-07-17 10:53:01.251499 pyngeso-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 pyngeso-0.3.4/setup.py
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 pyngeso-0.3.4/PKG-INFO
```

### Comparing `pyngeso-0.3.3/LICENSE.txt` & `pyngeso-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyngeso-0.3.3/README.md` & `pyngeso-0.3.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -26,17 +26,20 @@
 ## Tested reports
 
 ### Queryable via NG's api
 * `historic-day-ahead-demand-forecast`
 * `day-ahead-demand-forecast`
 * `historic-2day-ahead-demand-forecast`
 * `2day-ahead-demand-forecast`
+* `historic-2-14-days-ahead-demand-forecast`
 * `historic-day-ahead-wind-forecast`
 * `day-ahead-wind-forecast`
+* `14-days-ahead-wind-forecast`
 * `demand-data-update`
 * `dc-results-summary`
+* `dc-dr-dm-linear-orders`
 * `historic-demand-data-{year}` [2009-2022]
 * `historic-frequency-data` [Jan21-Jan22]
 * `transmission-entry-capacity-tec-register`
 
 ### Download of files
 * `historic-generation-mix`
```

### Comparing `pyngeso-0.3.3/pyngeso/pyngeso.py` & `pyngeso-0.3.4/pyngeso/pyngeso.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import logging
-from typing import Optional, List, Literal, Union
-from datetime import datetime, date
 import json
+import logging
+from datetime import date, datetime
+from typing import List, Literal, Optional, Union
 
 import requests
 
 from .configure_logging import setup_logger
-from .resources import api_resource_ids, file_resource_ids
 from .exceptions import UnsuccessfulRequest
+from .resources import api_resource_ids, file_resource_ids
 
 logger = setup_logger(logging.getLogger("PyNgEso"))
 
 date_fmt = "%Y-%m-%d"
 datetime_fmt = "%Y-%m-%dT%H:%M:%S"
 
 
@@ -49,15 +49,15 @@
         date_col: Optional[str] = None,
         start_date: Optional[Union[date, datetime]] = None,
         end_date: Optional[Union[date, datetime]] = None,
         filters: Optional[List[str]] = None,
         limit: Optional[int] = None,
     ) -> bytes:
 
-        url = f"https://data.nationalgrideso.com/api/3/action/datastore_search_sql"
+        url = "https://data.nationalgrideso.com/api/3/action/datastore_search_sql"
         sql = self.construct_sql(fields, date_col, start_date, end_date, filters, limit)
         params = {"sql": sql}
 
         logger.debug(f"Querying {self.resource}: {sql}")
         r = requests.get(url, params=params)
         self._check_for_errors(r)
         self._missing_data(r)
@@ -142,19 +142,19 @@
         # if filtering by date "WHERE' clause is already added
         if date_filtering:
             return "and " + filters_sql
         return "where " + filters_sql
 
     @staticmethod
     def validate_date_range(
-            start_date: Union[date, datetime],
-            end_date: Union[date, datetime]
+        start_date: Union[date, datetime], end_date: Union[date, datetime]
     ) -> None:
-        assert type(start_date) == type(end_date), \
-            "start_date and end_date should either be both a date or a datetime object"
+        assert type(start_date) == type(
+            end_date
+        ), "start_date and end_date should either be both a date or a datetime object"
 
         assert (
             end_date >= start_date
         ), "end_date should be the same of greater than start_date"
 
     @staticmethod
     def datetime_to_str(datetime_obj: Optional[Union[date, datetime]]) -> Optional[str]:
```

### Comparing `pyngeso-0.3.3/pyngeso/resources.py` & `pyngeso-0.3.4/pyngeso/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,30 @@
         "id": "24abd271-5936-45c7-85f4-2a6b450ef6b7",
         "url": "https://data.nationalgrideso.com/demand/2-day-ahead-demand-forecast/r/historic_2_day_ahead_demand_forecasts",
     },
     "2day-ahead-demand-forecast": {
         "id": "cda26f27-4bb6-4632-9fb5-2d029ca605e1",
         "url": "https://data.nationalgrideso.com/demand/2-day-ahead-demand-forecast/r/2_day_ahead_demand_forecast",
     },
+    "historic-2-14-days-ahead-demand-forecast": {
+        "id": "4dd712a2-ee2c-455d-a9c0-9d3564c80fa0",
+        "url": "https://data.nationalgrideso.com/demand/2-14-days-ahead-national-demand-forecast/r/historic_2-14_day_ahead_demand_forecasts",
+    },
     "historic-day-ahead-wind-forecast": {
         "id": "7524ec65-f782-4258-aaf8-5b926c17b966",
         "url": "https://data.nationalgrideso.com/demand/day-ahead-wind-forecast/r/historic_day_ahead_wind_forecasts",
     },
     "day-ahead-wind-forecast": {
         "id": "b2f03146-f05d-4824-a663-3a4f36090c71",
         "url": "https://data.nationalgrideso.com/demand/day-ahead-wind-forecast/r/day_ahead_wind_forecast",
     },
+    "14-days-ahead-wind-forecast": {
+        "id": "93c3048e-1dab-4057-a2a9-417540583929",
+        "url": "https://data.nationalgrideso.com/demand/14-days-ahead-wind-forecasts/r/14_days_ahead_wind_forecast",
+    },
     "embedded-solar-and-wind": {
         "id": "db6c038f-98af-4570-ab60-24d71ebd0ae5",
         "url": "https://data.nationalgrideso.com/generation/embedded-wind-and-solar-forecasts/r/embedded_solar_and_wind_forecast",
     },
     "demand-data-update": {
         "id": "177f6fa4-ae49-4182-81ea-0c6b35f26ca6",
         "url": "https://data.nationalgrideso.com/demand/daily-demand-update",
@@ -97,14 +105,18 @@
         "id": "6fd8e042-be27-4c67-ad59-5acdd2a7b0fd",
         "url": "https://data.nationalgrideso.com/ancillary-services/dynamic-containment-data/r/dc,_dr_&_dm_block_orders_master_data_2021-2022",
     },
     "dc-volume-forecast": {
         "id": "d5c3b48a-a0a9-4d57-a02a-ac0af09a6298",
         "url": "https://data.nationalgrideso.com/ancillary-services/dynamic-containment-4-day-forecast/r/dynamic_containment_4_day_forecast_-_history",
     },
+    "dc-dr-dm-linear-orders": {
+        "id": "26aefbcc-fce0-403f-80e1-4a26af3fe84b",
+        "url": "https://data.nationalgrideso.com/ancillary-services/dynamic-containment-data/r/dc_dr_dm_linear_orders_master_data_2021-2023",
+    },
     "historic-frequency-data-jan22": {
         "id": "43000c20-1208-4ca7-a419-712c7a1d375c",
         "url": "https://data.nationalgrideso.com/system/system-frequency-data/r/january_2022_-_historic_frequency_data",
     },
     "historic-frequency-data-dec21": {
         "id": "afe9895c-5937-4e78-8949-f0f026643666",
         "url": "https://data.nationalgrideso.com/system/system-frequency-data/r/december_2021_-_historic_frequency_data",
@@ -155,16 +167,16 @@
     },
     "carbon-intensity-forecast": {
         "id": "0e5fde43-2de7-4fb4-833d-c7bca3b658b0",
         "url": "https://data.nationalgrideso.com/carbon-intensity1/national-carbon-intensity-forecast/r/national_carbon_intensity_forecast",
     },
     "transmission-entry-capacity-tec-register": {
         "id": "17becbab-e3e8-473f-b303-3806f43a6a10",
-        "url": "https://data.nationalgrideso.com/connection-registers/transmission-entry-capacity-tec-register/r/tec_register"
-    }
+        "url": "https://data.nationalgrideso.com/connection-registers/transmission-entry-capacity-tec-register/r/tec_register",
+    },
 }
 
 file_resource_ids: Dict[str, Dict[str, str]] = {
     "historic-generation-mix": {
         "dataset_id": "88313ae5-94e4-4ddc-a790-593554d8c6b9",
         "resource_id": "f93d1835-75bc-43e5-84ad-12472b180a98",
         "filename": "df_fuel_ckan.csv",
```

### Comparing `pyngeso-0.3.3/pyproject.toml` & `pyngeso-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyngeso"
-version = "0.3.3"
+version = "0.3.4"
 description = "Simple python wrapper for the National Grid ESO Portal"
 authors = [
     "atsangarides <andreas_tsangarides@hotmail.com>",
     "bethrice44 <bethrice44@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `pyngeso-0.3.3/setup.py` & `pyngeso-0.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyngeso',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'Simple python wrapper for the National Grid ESO Portal',
-    'long_description': '# pyngeso\n\nSimple python wrapper for the National Grid ESO Portal.\n\n[![](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/pyenv/pyenv)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n## Getting started\n\n\n* Example usage\n```python\nfrom pyngeso import NgEso\n\nresource = "historic-day-ahead-demand-forecast"\ndate_col = "TARGETDATE"\nstart_date = "2018-01-01"\nend_date = "2018-01-01"\n\nclient = NgEso(resource)\n# returns content of response\nr: bytes = client.query(date_col=date_col, start_date=start_date, end_date=end_date)\n```\n\n## Tested reports\n\n### Queryable via NG\'s api\n* `historic-day-ahead-demand-forecast`\n* `day-ahead-demand-forecast`\n* `historic-2day-ahead-demand-forecast`\n* `2day-ahead-demand-forecast`\n* `historic-day-ahead-wind-forecast`\n* `day-ahead-wind-forecast`\n* `demand-data-update`\n* `dc-results-summary`\n* `historic-demand-data-{year}` [2009-2022]\n* `historic-frequency-data` [Jan21-Jan22]\n* `transmission-entry-capacity-tec-register`\n\n### Download of files\n* `historic-generation-mix`\n',
+    'long_description': '# pyngeso\n\nSimple python wrapper for the National Grid ESO Portal.\n\n[![](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/pyenv/pyenv)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n## Getting started\n\n\n* Example usage\n```python\nfrom pyngeso import NgEso\n\nresource = "historic-day-ahead-demand-forecast"\ndate_col = "TARGETDATE"\nstart_date = "2018-01-01"\nend_date = "2018-01-01"\n\nclient = NgEso(resource)\n# returns content of response\nr: bytes = client.query(date_col=date_col, start_date=start_date, end_date=end_date)\n```\n\n## Tested reports\n\n### Queryable via NG\'s api\n* `historic-day-ahead-demand-forecast`\n* `day-ahead-demand-forecast`\n* `historic-2day-ahead-demand-forecast`\n* `2day-ahead-demand-forecast`\n* `historic-2-14-days-ahead-demand-forecast`\n* `historic-day-ahead-wind-forecast`\n* `day-ahead-wind-forecast`\n* `14-days-ahead-wind-forecast`\n* `demand-data-update`\n* `dc-results-summary`\n* `dc-dr-dm-linear-orders`\n* `historic-demand-data-{year}` [2009-2022]\n* `historic-frequency-data` [Jan21-Jan22]\n* `transmission-entry-capacity-tec-register`\n\n### Download of files\n* `historic-generation-mix`\n',
     'author': 'atsangarides',
     'author_email': 'andreas_tsangarides@hotmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/atsangarides/pyngeso',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `pyngeso-0.3.3/PKG-INFO` & `pyngeso-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pyngeso
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple python wrapper for the National Grid ESO Portal
 Home-page: https://github.com/atsangarides/pyngeso
 License: MIT
 Keywords: api,energy
 Author: atsangarides
 Author-email: andreas_tsangarides@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Repository, https://github.com/atsangarides/pyngeso
 Description-Content-Type: text/markdown
 
 # pyngeso
 
@@ -49,18 +50,21 @@
 ## Tested reports
 
 ### Queryable via NG's api
 * `historic-day-ahead-demand-forecast`
 * `day-ahead-demand-forecast`
 * `historic-2day-ahead-demand-forecast`
 * `2day-ahead-demand-forecast`
+* `historic-2-14-days-ahead-demand-forecast`
 * `historic-day-ahead-wind-forecast`
 * `day-ahead-wind-forecast`
+* `14-days-ahead-wind-forecast`
 * `demand-data-update`
 * `dc-results-summary`
+* `dc-dr-dm-linear-orders`
 * `historic-demand-data-{year}` [2009-2022]
 * `historic-frequency-data` [Jan21-Jan22]
 * `transmission-entry-capacity-tec-register`
 
 ### Download of files
 * `historic-generation-mix`
```

