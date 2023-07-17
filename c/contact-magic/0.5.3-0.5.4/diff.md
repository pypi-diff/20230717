# Comparing `tmp/contact_magic-0.5.3.tar.gz` & `tmp/contact_magic-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.5.3.tar", max compression
+gzip compressed data, was "contact_magic-0.5.4.tar", max compression
```

## Comparing `contact_magic-0.5.3.tar` & `contact_magic-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.3/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.3/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.3/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.3/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5418 2023-07-13 11:03:11.215506 contact_magic-0.5.3/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.3/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     3716 2023-07-08 21:49:20.995044 contact_magic-0.5.3/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.3/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-13 10:14:40.612229 contact_magic-0.5.3/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1678 2023-07-08 23:06:56.717869 contact_magic-0.5.3/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.3/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.3/contact_magic/logger.py
--rw-r--r--   0        0        0    16259 2023-07-13 11:03:11.410196 contact_magic-0.5.3/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.3/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.3/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.3/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.3/contact_magic/scripts/default_scraper_options.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.3/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.3/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.3/contact_magic/scripts/sync_scraper_options_to_workersheets.py
--rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.3/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.3/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2023-07-13 11:03:28.052391 contact_magic-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.4/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.4/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.4/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.4/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5418 2023-07-13 11:03:11.215506 contact_magic-0.5.4/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.4/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3716 2023-07-08 21:49:20.995044 contact_magic-0.5.4/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.4/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-13 10:14:40.612229 contact_magic-0.5.4/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1678 2023-07-08 23:06:56.717869 contact_magic-0.5.4/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.4/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.4/contact_magic/logger.py
+-rw-r--r--   0        0        0    16761 2023-07-17 16:12:06.692037 contact_magic-0.5.4/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.4/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.4/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.4/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.4/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.4/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.4/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.4/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.4/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.4/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-07-17 15:36:24.862079 contact_magic-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.4/PKG-INFO
```

### Comparing `contact_magic-0.5.3/README.md` & `contact_magic-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/asyncio.py` & `contact_magic-0.5.4/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/conf/settings.py` & `contact_magic-0.5.4/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/dict_utils.py` & `contact_magic-0.5.4/contact_magic/dict_utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/helpers.py` & `contact_magic-0.5.4/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.4/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.4/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/integrations/sheets.py` & `contact_magic-0.5.4/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/models.py` & `contact_magic-0.5.4/contact_magic/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from contact_magic.integrations import (
     make_copyfactory_request,
     make_sales_scraper_request,
 )
 from contact_magic.logger import logger
 from contact_magic.utils import get_id_from_url, is_valid_premise_url
 
+SALES_SCRAPER_KEY_PREFIX_NAME = "sales_scrapers"
+
 
 class DataRow(BaseModel):
     """
     A class to hold a row of data and it's index number
     to sort by after. Converts set data to a dict.
     """
 
@@ -148,14 +150,22 @@
         )
         if scrape := await make_sales_scraper_request(self.scraper_name, data=data):
             for key, value in scrape.items():
                 if key in row.data and not overwrite:
                     continue
                 # Remove output schema since don't want
                 # to pass schema values to Copyfactory
+                # Scope scraper info to a prefixed keyname
+                # to not have conflict with other scraped values.
+                if key == "scraper_info":
+                    if isinstance(value, dict):
+                        value = {
+                            f"{SALES_SCRAPER_KEY_PREFIX_NAME}__{k}": v
+                            for k, v in value.items()
+                        }
                 value = delete_key_in_object(value, "output_schema")
                 unique_key = f"{col_prefix}__{self.scraper_name}__{key}"
                 row.data[unique_key] = value
                 self.added_key_names.add(unique_key)
             return row
         return row
 
@@ -197,15 +207,15 @@
             for key in keys_to_delete:
                 data = delete_key_in_object(data, key)
 
         if cf := await make_copyfactory_request(self.premise_id, variables=data):
             row.data[content_col_name] = cf["content"]
             source = row.data.get(
                 f"{content_col_name}__{self.scraper_name}__scraper_info", {}
-            ).get("data_source", "-")
+            ).get(f"{SALES_SCRAPER_KEY_PREFIX_NAME}__data_source", "-")
             row.data[source_col_name] = f"{self.scraper_name}, {source}"
             return row, True
         return row, False
 
     def run_processors(self, row) -> tuple[DataRow, bool]:
         """
         Iterate over field processors and break if any don't satisfy.
@@ -313,15 +323,15 @@
                 column_name=self.col_name,
                 status="STARTING",
             )
             row, did_succeed = await scraper.execute(
                 row,
                 self.col_name,
                 self.get_col_name_as_source,
-                keys_to_delete=keys_to_delete,
+                keys_to_delete=keys_to_delete | self.keys_added,
             )
             for key in scraper.added_key_names:
                 self.keys_added.add(key)
             if did_succeed:
                 if scraper.scraper_name != "FALLBACK":
                     self.successful_scraper_name = scraper.scraper_name
                 logger.info(
```

### Comparing `contact_magic-0.5.3/contact_magic/preprocessors.py` & `contact_magic-0.5.4/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/scripts/agency.py` & `contact_magic-0.5.4/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/scripts/default_scraper_options.py` & `contact_magic-0.5.4/contact_magic/scripts/default_scraper_options.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.4/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/scripts/sync_scraper_options_to_workersheets.py` & `contact_magic-0.5.4/contact_magic/scripts/sync_scraper_options_to_workersheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.4/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/contact_magic/utils.py` & `contact_magic-0.5.4/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.3/pyproject.toml` & `contact_magic-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.5.3"
+version = "0.5.4"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.5.3/PKG-INFO` & `contact_magic-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.5.3
+Version: 0.5.4
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

