# Comparing `tmp/degiroasync-0.18.1.tar.gz` & `tmp/degiroasync-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiroasync-0.18.1.tar", last modified: Sun Jul  9 09:11:35 2023, max compression
+gzip compressed data, was "degiroasync-0.19.0.tar", last modified: Mon Jul 17 18:16:16 2023, max compression
```

## Comparing `degiroasync-0.18.1.tar` & `degiroasync-0.19.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2023-07-08 16:07:32.000000 degiroasync-0.18.1/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-09 09:11:35.489396 degiroasync-0.18.1/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4352 2023-07-08 16:07:32.000000 degiroasync-0.18.1/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.485396 degiroasync-0.18.1/degiroasync/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/__init__.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/degiroasync/api/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4330 2023-07-09 09:11:20.000000 degiroasync-0.18.1/degiroasync/api/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/api/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    31824 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/api/product.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8975 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/api/session.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/degiroasync/core/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6556 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/constants.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    14273 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/exceptions.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    16476 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/helpers.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/degiroasync/webapi/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-09 09:11:20.000000 degiroasync-0.18.1/degiroasync/webapi/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5780 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/webapi/login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/webapi/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    28777 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/webapi/product.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.485396 degiroasync-0.18.1/degiroasync.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      723 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      293 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2023-07-08 16:07:32.000000 degiroasync-0.18.1/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-09 09:11:35.489396 degiroasync-0.18.1/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2209 2023-07-09 09:11:20.000000 degiroasync-0.18.1/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/integration_login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/test_core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    36370 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/test_degiroapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    19359 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/test_degirowebapi.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.624474 degiroasync-0.19.0/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.19.0/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-17 18:16:16.624474 degiroasync-0.19.0/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4347 2023-07-08 15:05:00.000000 degiroasync-0.19.0/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.19.0/degiroasync/__init__.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/api/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4330 2023-07-08 14:01:28.000000 degiroasync-0.19.0/degiroasync/api/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.19.0/degiroasync/api/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    35297 2023-07-13 13:06:08.000000 degiroasync-0.19.0/degiroasync/api/product.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     9298 2023-07-09 15:27:14.000000 degiroasync-0.19.0/degiroasync/api/session.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/core/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.19.0/degiroasync/core/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6565 2023-07-13 13:09:23.000000 degiroasync-0.19.0/degiroasync/core/constants.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14341 2023-07-10 07:20:34.000000 degiroasync-0.19.0/degiroasync/core/core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.19.0/degiroasync/core/exceptions.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    16450 2023-07-09 14:06:23.000000 degiroasync-0.19.0/degiroasync/core/helpers.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/webapi/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-08 14:01:46.000000 degiroasync-0.19.0/degiroasync/webapi/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5967 2023-07-09 14:59:10.000000 degiroasync-0.19.0/degiroasync/webapi/login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.19.0/degiroasync/webapi/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    29327 2023-07-10 07:36:11.000000 degiroasync-0.19.0/degiroasync/webapi/product.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      270 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.19.0/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-17 18:16:16.624474 degiroasync-0.19.0/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2167 2023-07-09 16:49:30.000000 degiroasync-0.19.0/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.624474 degiroasync-0.19.0/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.19.0/tests/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.19.0/tests/integration_login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.19.0/tests/test_core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    37483 2023-07-09 16:16:22.000000 degiroasync-0.19.0/tests/test_degiroapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    18422 2023-07-09 16:53:26.000000 degiroasync-0.19.0/tests/test_degirowebapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.19.0/tests/test_setup.py
```

### Comparing `degiroasync-0.18.1/LICENSE` & `degiroasync-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/PKG-INFO` & `degiroasync-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.18.1
+Version: 0.19.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # DegiroAsync
 
 ## Documentation
 
-Check out the online documentation [here](https://ohmajesticlama.github.io/degiroasync/index.html).
+Check out the [online documentation](https://ohmajesticlama.github.io/degiroasync/index.html).
 
 ## Introduction
 
 This project aims to provide an *unofficial* API for Degiro platform that works
 asynchronously.
```

### Comparing `degiroasync-0.18.1/README.md` & `degiroasync-0.19.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DegiroAsync
 
 ## Documentation
 
-Check out the online documentation [here](https://ohmajesticlama.github.io/degiroasync/index.html).
+Check out the [online documentation](https://ohmajesticlama.github.io/degiroasync/index.html).
 
 ## Introduction
 
 This project aims to provide an *unofficial* API for Degiro platform that works
 asynchronously.
```

### Comparing `degiroasync-0.18.1/degiroasync/__init__.py` & `degiroasync-0.19.0/degiroasync/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/api/__init__.py` & `degiroasync-0.19.0/degiroasync/api/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/api/orders.py` & `degiroasync-0.19.0/degiroasync/api/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/api/product.py` & `degiroasync-0.19.0/degiroasync/api/product.py`

 * *Files 7% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             for i in range(ind + 1, len(batches_awt)):
                 await batches_awt[i]
             raise
 
     @classmethod
     async def _create_batch(
             cls,
-            session: SessionCore,
+            session: Session,
             attributes_batch: Iterable[Dict[str, Any]]
     ) -> Iterable[ProductBase]:
         """
         Create Products and their common ProductsInfo.
         Returns an Iterable of Product instances.
         """
         attributes_batch1, attributes_batch2 = itertools.tee(attributes_batch)
@@ -230,15 +230,15 @@
                 LOGGER.debug("__products_from_attrs| product_info %s",
                              product_info)
                 try:
                     product_info['product_type_id'] = PRODUCT.TYPEID(
                         product_info['product_type_id']
                         )
                 except ValueError:
-                    # Let int live its life, it'll be a generic product.
+                    # Let int stay, it'll be a generic product.
                     pass
 
                 product_type_id = product_info['product_type_id']
                 # Get specialized class if there is one implemented
                 inst_cls = {
                     PRODUCT.TYPEID.CURRENCY: Currency,
                     PRODUCT.TYPEID.STOCK: Stock
@@ -246,14 +246,25 @@
                     product_type_id,
                     ProductGeneric
                 )
                 LOGGER.debug(
                         "api.ProductFactory.init_product| type_id %s class %s",
                         product_type_id, inst_cls)
                 product_info = camelcase_dict_to_snake(product_info)
+                #if inst_cls is Stock:
+                if (
+                        product_info.get('exchange_id')
+                        and issubclass(inst_cls, Stock)
+                        ):
+                    # WARNING: There could be exchange_id key, but empty value,
+                    # We don't want to set it here if that's the case
+                    product_info['exchange'] = (
+                            session.exchange_dictionary.exchange_by(
+                                id=product_info['exchange_id'])
+                            )
                 # 2022.04 JSONclass poor compatibility with mypy
                 info = inst_cls.Info(product_info)  # type: ignore
                 instance = inst_cls(force_init=True)
                 # 2022.04 JSONclass poor compatibility with mypy
                 instance.base = inst_cls.Base(product_base)  # type: ignore
                 instance.info = info
                 products_dict[product_id] = instance
@@ -275,14 +286,15 @@
 
 class Stock(ProductBase):
     class Info(ProductBase.Info):
         "Store Info calls return."
         isin: str
         symbol: str
         name: str
+        exchange: Exchange
         vwd_id: Optional[str] = None  # not set if non-tradable
         vwd_identifier_type: Optional[str] = None  # not set if non-tradable
         product_type: str
         product_type_id: PRODUCT.TYPEID
         tradable: bool
         category: str
         # feed_quality: str  # Not always available
@@ -750,134 +762,227 @@
             resolution=PRICE.RESOLUTION(resp_json['resolution']),
             currency=product.info.currency,
             series=series_d,
             )
     return prices_series
 
 
+async def _search_one(
+        session: Session,
+        *,
+        by_text: Optional[str] = None,
+        by_isin: Optional[str] = None,
+        by_symbol: Optional[str] = None,
+        country_id: Optional[str] = None,
+        exchange_id: Optional[Union[str, Exchange]] = None,
+        product_type_id: Optional[PRODUCT.TYPEID] = PRODUCT.TYPEID.STOCK,
+        offset: int = 0,
+        limit: int = 100,
+        ) -> (Sequence[ProductBase], int, int):
+    """
+    Returns
+    -------
+
+    products
+        Instantiated products found.
+
+    n_unfiltered
+        Number of products returned by the API before local filtering.
+
+    total
+        Total number of products that could be returned by API, before local
+        filtering.
+    """
+    def __custom_filter(p_json: Dict[str, Any]) -> bool:
+        "Return True if product match user parameters"
+
+        # Web API should already filter by typeId, recheck TypeID here to be
+        # sure we don't have garbage in.
+        for attr, key in ((product_type_id, 'productTypeId'),
+                          (by_isin, 'isin'),
+                          (by_symbol, 'symbol'),
+                          (exchange_id, 'exchangeId'),
+                          ):
+            if attr is not None and p_json.get(key) != attr:
+                return False
+        return True
+
+    resp_json = await webapi.search_product(
+        session,
+        by_text,
+        product_type_id=product_type_id,
+        country_id=country_id,
+        limit=limit,
+        offset=offset)
+    LOGGER.debug("api.search_product response| %s",
+                 pprint.pformat(resp_json))
+    # Calls with more than one page could be parallelized:
+    # First page is needed first to get the total answers, but
+    # further pages could be fetched several at a time.
+    total = resp_json['total']  # Total number of products returned
+    if 'products' in resp_json:
+        n_unfiltered = len(resp_json['products'])
+        products_json = resp_json['products']
+        LOGGER.debug("api.search_product n_products| %s",
+                     products_json)
+        batch_gen = ProductFactory.init_batch(
+                session,
+                filter(__custom_filter,
+                       products_json))
+        products = [p async for p in batch_gen]
+        # This could be optimized later on with a generator class to be
+        # able to yield data as soon as we receive it while still not
+        # blocking further calls to be launched, should it be needed.
+        LOGGER.debug("api.search_product (batch len, symbol)| (%s, %s)",
+                     len(products), by_symbol)
+        return products, n_unfiltered, total
+
+    else:
+        LOGGER.debug("No 'products' key in response. Stop.")
+        raise ResponseError(f"No 'products' key in response {resp_json} ")
+
+
 async def search_product(
         session: Session,
         *,
         by_text: Optional[str] = None,
         by_isin: Optional[str] = None,
         by_symbol: Optional[str] = None,
-        by_exchange: Union[str, Exchange, None] = None,
+        by_country: Optional[str] = None,
+        by_exchange: Optional[Union[str, Exchange]] = None,
         product_type_id: Optional[PRODUCT.TYPEID] = PRODUCT.TYPEID.STOCK,
-        max_iter: Union[int, None] = 1000
+        max_iter: Optional[int] = 1000
         ) -> List[ProductBase]:
     """
     Access `product_search` endpoint.
 
     Exactly one of `by_text`, `by_isin`, `by_symbol` be set.
-    This is done because endpoint API doesn't return expected results
-    with both text and ISIN search.
+    Note: API endpoint doesn't return expected results with both text and
+    ISIN search.
+
+    Parameters
+    ----------
+
+        by_text
+            As a search text in Degiro search field website.
+
+        by_isin
+            Will look-up products with provided ISIN identifier.
 
-    product_type_id
-        Restricts search to one type of products.
+        by_symbol
+            Product outputs will be filtered on their 'symbol'.
 
-    by_exchange
-        Restricts results to products in a exchange. Can be either an Exchange
-        instance or an `hiq_abbr` str (e.g. EPA for Paris, AEX for Amsterdam)
+        by_country
+            Products matching this argument, string must be ISO 3166-1 alpha-2
+            2 letters code.
+
+        product_type_id
+            Restricts search to one type of products.
+            See :class:`~degiroasync.core.PRODUCT.TYPEID`
+
+        by_exchange
+            Restricts results to products in a exchange. Can be either an
+            Exchange instance or an `hiq_abbr` str (e.g. EPA for Paris, AEX
+            for Amsterdam)
+
+        product_type_id
+            Restricts search to one type of products.
+
+        max_iter
+            Pull `max_iter` pages of results. If `None`, don't stop until end
+            is reached. Default value: 1000.
 
-    max_iter
-        Pull `max_iter` pages of results. If `None`, don't stop until end is
-        reached. Default value: 1000.
+    Returns
+    -------
 
-    Return a list of ProductBase objects returned by Degiro for `search_txt`
-    attribute.
+        Return a list of ProductBase objects returned by Degiro for
+        `search_txt` attribute.
     """
-    if sum(k is not None for k in (by_text, by_isin, by_symbol)) != 1:
+    if sum(k is not None for k in (by_text, by_isin, by_symbol)) > 1:
         raise AssertionError(
-            "Exactly one of by_text, by_isin, by_symbol must "
+            "Only one of by_text, by_isin, by_symbol can "
             "be not None.")
     # Degiro API doesn't support well 2 or more attribute in searchTxt:
     # e.g. we can't search for "AIRBUS NL0000235190" and get all the AIRBUS
     # named products with ISIN NL0000235190.
     if by_text is None:
         # We've checked above that we only have one not-None search parameter.
         if by_symbol is not None:
             by_text = by_symbol
         elif by_isin is not None:
             by_text = by_isin
+        elif by_country is not None:
+            pass  # Could also be set without text deal with it after
         else:
             raise AssertionError(
                     "by_text is None and no search parameters was set or "
                     "found. Have you set a search parameters to "
-                    "get_price_series?"
+                    "search_product?"
                     "\n If yes, this shouldn't be happening, please open a bug"
                     " report."
                     )
 
+    country_id = None
+    if by_country is not None:
+        country = session.exchange_dictionary.country_by(
+            name=by_country
+                )
+        country_id = country.id
+
     exchange_id = None
     if by_exchange is not None:
         if isinstance(by_exchange, Exchange):
             exchange_id = by_exchange.id
         elif isinstance(by_exchange, str):
             check_session_exchange_dictionary(session)
             exchange = session.exchange_dictionary.exchange_by(
                 hiq_abbr=by_exchange)
             exchange_id = exchange.id
         else:
             raise TypeError(
                 "Only Exchange or str types supported for 'by_exchange'.")
 
     limit = 100
-    offset = 0
     products = []
 
-    def __custom_filter(p_json: Dict[str, Any]) -> bool:
-        "Return True if product match user parameters"
+    # trigger first call to get total:
+    products, n_unfiltered, total = await _search_one(
+            session,
+            by_text=by_text,
+            by_isin=by_isin,
+            by_symbol=by_symbol,
+            country_id=country_id,
+            exchange_id=exchange_id,
+            offset=0,
+            limit=limit
+            )
 
-        # Web API should already filter by typeId, recheck TypeID here to be
-        # sure we don't have garbage in.
-        for attr, key in ((product_type_id, 'productTypeId'),
-                          (by_isin, 'isin'),
-                          (by_symbol, 'symbol'),
-                          (exchange_id, 'exchangeId')):
-            if attr is not None and p_json.get(key) != attr:
-                return False
-        return True
+    if n_unfiltered < total:
+        # Generate args
+        args = ({
+            'session': session,
+            'by_text': by_text,
+            'by_isin': by_isin,
+            'by_symbol': by_symbol,
+            'country_id': country_id,
+            'exchange_id': exchange_id,
+            'offset': offset,
+            'limit': limit,
+            } for offset in range(n_unfiltered, total, limit)
+            )
+        # The use of _search_one and gather improves performance over
+        # sequential queries in a while loop as before.
+        # 20230713 FR symbols query, throttling at 10 queries per 1 second:
+        #   - With gather+_search_one: 3.6s
+        #   - With legacy sequential calls: 6.9s
+        answers = await asyncio.gather(
+                    *[_search_one(**kwa) for kwa in args])
+        for prods, _, _ in answers:
+            products += prods
 
-    iter_n = 0
-    run_forever = max_iter is None
-    if max_iter is None:
-        max_iter = -1
-    while iter_n < max_iter or run_forever:
-        iter_n += 1
-        resp_json = await webapi.search_product(
-            session,
-            by_text,
-            product_type_id=product_type_id,
-            limit=limit,
-            offset=offset)
-        LOGGER.debug("api.search_product response| %s",
-                     pprint.pformat(resp_json))
-        if 'products' in resp_json:
-            products_json = resp_json['products']
-            LOGGER.debug("api.search_product n_products| %s",
-                         products_json)
-            batch_gen = ProductFactory.init_batch(
-                    session,
-                    filter(__custom_filter,
-                           products_json))
-            batch = [p async for p in batch_gen]
-            # This could be optimized later on with a generator class to be
-            # able to yield data as soon as we receive it while still not
-            # blocking further calls to be launched, should it be needed.
-            products += batch
-            LOGGER.debug("api.search_product (batch len, symbol)| (%s, %s)",
-                         len(batch), by_symbol)
-            if len(products_json) < limit:
-                break
-            else:
-                offset += len(products_json)
-        else:
-            LOGGER.debug("No 'products' key in response. Stop.")
-            break
-    # return a unique list
     return list(unique_everseen(products, lambda p: p.info.id))
 
 
 __all__ = [
     obj.__name__ for obj in (  # type: ignore
         # Login & setup
         Credentials,
```

### Comparing `degiroasync-0.18.1/degiroasync/api/session.py` & `degiroasync-0.19.0/degiroasync/api/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union, List, Dict, Any
 from typing import Set
+from typing import Optional
 import functools
 import logging
 import pprint
 import copy
 
 from jsonloader import JSONclass
 
@@ -26,27 +27,27 @@
     id: int
     name: str
 
 
 @JSONclass(annotations=True, annotations_type=True)
 class Country:
     id: str
-    name: str  # 2 letters country codename
+    name: str  # ISO 3166-1 alpha-2 country codename
     region: 'Region'
 
 
 @JSONclass(annotations=True, annotations_type=True)
 class Exchange:
     id: str
     name: str
-    city: Union[str, None] = None
-    code: Union[str, None] = None
+    city: Optional[str] = None
+    code: Optional[str] = None
     country_name: str  # renamed from 'country' as it is country name
     hiq_abbr: str
-    mic_code: Union[str, None] = None
+    mic_code: Optional[str] = None
 
 
 class ExchangeDictionary:
     """
     Usage:
 
     .. code-block:: python
@@ -110,20 +111,22 @@
     def regions(self):
         return self._regions.values()
 
     @functools.lru_cache(32)
     def exchange_by(
             self,
             *,
-            name: Union[str, None] = None,
-            id: Union[int, None] = None,
-            hiq_abbr: Union[str, None] = None,
-            mic_code: Union[str, None] = None) -> Exchange:
-        """Get Exchange by *either* name, hiqAbbr (e.g. EPA),
-        micCode (e.g. XPAR)."""
+            name: Optional[str] = None,
+            id: Optional[int] = None,
+            hiq_abbr: Optional[str] = None,
+            mic_code: Optional[str] = None) -> Exchange:
+        """
+        Get Exchange by *either* name, hiqAbbr (e.g. EPA),
+        micCode (e.g. XPAR).
+        """
         if sum(attr is not None for attr in (name,
                                              id,
                                              hiq_abbr,
                                              mic_code)) != 1:
             raise AssertionError(
                 "Exactly one of (name, id, hiqAbbr, micCode) "
                 "must be not None.")
@@ -144,14 +147,20 @@
             *,
             name: Union[str, None] = None,
             id: Union[int, None] = None) -> Country:
         if sum(attr is not None for attr in (name, id)) != 1:
             raise AssertionError(
                 "Exactly one of (name, id) must be not None.")
         if name is not None:
+            if name not in self._countries_name:
+                raise KeyError(
+                        "{} not found. List of available countries: {}".format(
+                            name,
+                            [c for c in self._countries_name]
+                            ))
             return self._countries_name[name]
         if id is not None:
             return self._countries_id[id]
 
 
 class Session(SessionCore):
     config: Config
@@ -200,14 +209,15 @@
         # cache.
         _LOGIN_FAILURE_HASH.discard(credentials)
         return True
     else:
         return False
 
 
+
 async def login(
         credentials: Credentials,
         session: Union[Session, None] = None,
         /,
         safeguard_incorrect_credentials: bool = True
         ) -> Session:
     """
```

### Comparing `degiroasync-0.18.1/degiroasync/core/__init__.py` & `degiroasync-0.19.0/degiroasync/core/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/core/constants.py` & `degiroasync-0.19.0/degiroasync/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,10 +289,10 @@
 
 class POSITION:
     class TYPE(StrEnum):
         PRODUCT = 'PRODUCT'
 
 
 # HTTP Requests global timeout, in seconds. DEGIRO endpoints are sometimes
-# a bit slow to answer, maybe due to throttling: this is necessary
+# a bit slow to answer, maybe due to endpoint throttling: this is necessary
 # to limit number of call failure.
-TIMEOUT: float = 20
+TIMEOUT: float = 30
```

### Comparing `degiroasync-0.18.1/degiroasync/core/core.py` & `degiroasync-0.19.0/degiroasync/core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import httpx
 from jsonloader import JSONclass
 
 from .helpers import join_url
 from .constants import LOGGER_NAME
 from .constants import PRODUCT
+from .constants import TIMEOUT
 from ..core.helpers import ThrottlingClient
 from .exceptions import ContextError
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 LOGGER.setLevel(logging.DEBUG)
 
 
@@ -207,15 +208,16 @@
     def __hash__(self):
         return hash(self.__dict__.values())
 
     async def __aenter__(self) -> ThrottlingClient:
         if self._http_client is None:
             self._http_client = ThrottlingClient(
                     max_requests=self._max_requests_default,
-                    period_seconds=self._period_seconds_default
+                    period_seconds=self._period_seconds_default,
+                    timeout=TIMEOUT
                     )
         return await self._http_client.__aenter__()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self._http_client.__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `degiroasync-0.18.1/degiroasync/core/exceptions.py` & `degiroasync-0.19.0/degiroasync/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/core/helpers.py` & `degiroasync-0.19.0/degiroasync/core/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         if self.wait:
             self.res = self.coro.__await__()
             self.wait = False
         return self.res
 
 
 def lru_cache_timed(
-        func: Union[Callable, None] = None,
+        func: Optional[Callable] = None,
         /,
         maxsize: int = 128,
         typed: bool = False,
-        seconds: Union[None, float] = None,
+        seconds: Optional[float] = None,
 ):
     """
     Time-sensitive LRU cache that works with async functions.
 
     >>> @lru_cache_timed(seconds=120)
     ... async def foo():
     ...     asyncio.sleep(1)
@@ -476,15 +476,14 @@
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         self._count_open -= 1
         if self._count_open <= 0:
             await self._async_client.__aexit__(exc_type, exc_val, exc_tb)
             self._async_client = None
             self._client_open = None
-        return self
 
     @_throttle
     @functools.wraps(httpx.AsyncClient.get)
     async def get(self, *args, **kwargs):
         return await self._client_open.get(*args, **kwargs)
 
     @_throttle
```

### Comparing `degiroasync-0.18.1/degiroasync/webapi/__init__.py` & `degiroasync-0.19.0/degiroasync/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/webapi/login.py` & `degiroasync-0.19.0/degiroasync/webapi/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-from typing import Union, Dict, Any
+from typing import Union, Dict, Any, Optional
 import logging
 import json
 import base64
 import struct
 import hmac
 import hashlib
 import time
 
-import httpx
-
 from ..core.constants import LOGGER_NAME
 from ..core.constants import LOGIN
 from ..core.constants import TIMEOUT
 from ..core import Credentials, SessionCore, URLs, Config, PAClient
 from ..core import check_session_config
 from ..core.helpers import check_response
 from ..core.helpers import camelcase_dict_to_snake
+from ..core.helpers import ThrottlingClient
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 
 
+# Dedicated Throttling client for login as it is much more restricted.
+_LOGIN_THROTTLE = ThrottlingClient(max_requests=1, period_seconds=2)
+
+
 async def login(
         credentials: Credentials,
-        session: Union[SessionCore, None] = None) -> SessionCore:
+        session: Optional[SessionCore] = None) -> SessionCore:
     """
     Authentify with Degiro API.
     `session` will be updated with required data for further connections.
     If no `session` is provided, create one.
     """
     url = URLs.LOGIN
     session = session or SessionCore()
     payload = {
         "username": credentials.username,
         "password": credentials.password,
         "isRedirectToMobile": False,
         "isPassCodeReset": '',
         "queryParams": {"reason": "session_expired"}
     }
-    async with session as client:
+    async with _LOGIN_THROTTLE as client:
         LOGGER.debug("login| url %s", url)
         response = await client.post(url, content=json.dumps(payload))
         LOGGER.debug("login| response %s", response.__dict__)
 
         response_load = response.json()
 
         if response_load['status'] == LOGIN.TOTP_NEEDED:
```

### Comparing `degiroasync-0.18.1/degiroasync/webapi/orders.py` & `degiroasync-0.19.0/degiroasync/webapi/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/degiroasync/webapi/product.py` & `degiroasync-0.19.0/degiroasync/webapi/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 from typing import Union, Any, List, Dict
-
-import httpx
+from typing import Optional
 
 from ..core import SessionCore, URLs
 from ..core import join_url
 from ..core import check_session_config
 from ..core import check_session_client
 from ..core.constants import LOGGER_NAME
 from ..core.constants import PRICE
 from ..core.constants import PRODUCT
-from ..core.constants import TIMEOUT
 from ..core.helpers import check_response
 
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 
 
 async def get_portfolio(session: SessionCore) -> Dict[str, Any]:
@@ -750,15 +748,17 @@
                         ]],
                 "id":"price:issueid:360114899",
                 "type":"time"}]
             }
     """
     # TODO: There may be an issue with the above JSON example, review.
     if vwdIdentifierType not in ('issueid', 'vwdkey'):
-        raise ValueError("vwdIdentifierType must be 'issueid' or 'vwdkey'")
+        raise ValueError(
+                f"vwdIdentifierType must be 'issueid' or 'vwdkey', "
+                f"not {vwdIdentifierType}")
 
     check_session_config(session)
     url = URLs.get_price_data_url(session)
     LOGGER.debug('get_price_series url| %s', url)
     params = {
         'requestid': 1,
         'resolution': str(resolution),
@@ -811,92 +811,103 @@
     check_response(response)
     LOGGER.debug("get_trading_update| %s", response.json())
     return response.json()
 
 
 async def search_product(
         session: SessionCore,
-        search_txt: str,
-        product_type_id: Union[PRODUCT.TYPEID, None] = None,
-        limit: int = 10,
+        search_txt: Optional[str] = None,
+        *,
+        product_type_id: Optional[PRODUCT.TYPEID] = None,
+        country_id: Optional[str] = None,
+        index_id: Optional[str] = None,
+        limit: int = 50,
         offset: int = 0) -> Dict[str, Any]:
     """
     Access `product_search` endpoint.
 
-    Example JSON response:
-    {
-        "offset": 0,
-        "products": [
-            {
-                "active": true,
-                "buyOrderTypes": [
-                    "LIMIT",
-                    "MARKET",
-                    "STOPLOSS",
-                    "STOPLIMIT"
-                ],
-                "category": "B",
-                "closePrice": 113.3,
-                "closePriceDate": "2022-02-02",
-                "contractSize": 1.0,
-                "currency": "EUR",
-                "exchangeId": "710",
-                "feedQuality": "R",
-                "feedQualitySecondary": "CX",
-                "id": "96008",
-                "isin": "NL0000235190",
-                "name": "AIRBUS",
-                "onlyEodPrices": false,
-                "orderBookDepth": 0,
-                "orderBookDepthSecondary": 0,
-                "orderTimeTypes": [
-                    "DAY",
-                    "GTC"
-                ],
-                "productBitTypes": [],
-                "productType": "STOCK",
-                "productTypeId": 1,
-                "qualitySwitchFree": false,
-                "qualitySwitchFreeSecondary": false,
-                "qualitySwitchable": false,
-                "qualitySwitchableSecondary": false,
-                "sellOrderTypes": [
-                    "LIMIT",
-                    "MARKET",
-                    "STOPLOSS",
-                    "STOPLIMIT"
-                ],
-                "strikePrice": -0.0001,
-                "symbol": "AIR",
-                "tradable": true,
-                "vwdId": "360114899",
-                "vwdIdSecondary": "955000256",
-                "vwdIdentifierType": "issueid",
-                "vwdIdentifierTypeSecondary": "issueid",
-                "vwdModuleId": 1,
-                "vwdModuleIdSecondary": 2
-            }
-        ]
-    }
+    Example response:
+
+    .. code-block:: python
+
+        {
+            "offset": 0,
+            "products": [
+                {
+                    "active": true,
+                    "buyOrderTypes": [
+                        "LIMIT",
+                        "MARKET",
+                        "STOPLOSS",
+                        "STOPLIMIT"
+                    ],
+                    "category": "B",
+                    "closePrice": 113.3,
+                    "closePriceDate": "2022-02-02",
+                    "contractSize": 1.0,
+                    "currency": "EUR",
+                    "exchangeId": "710",
+                    "feedQuality": "R",
+                    "feedQualitySecondary": "CX",
+                    "id": "96008",
+                    "isin": "NL0000235190",
+                    "name": "AIRBUS",
+                    "onlyEodPrices": false,
+                    "orderBookDepth": 0,
+                    "orderBookDepthSecondary": 0,
+                    "orderTimeTypes": [
+                        "DAY",
+                        "GTC"
+                    ],
+                    "productBitTypes": [],
+                    "productType": "STOCK",
+                    "productTypeId": 1,
+                    "qualitySwitchFree": false,
+                    "qualitySwitchFreeSecondary": false,
+                    "qualitySwitchable": false,
+                    "qualitySwitchableSecondary": false,
+                    "sellOrderTypes": [
+                        "LIMIT",
+                        "MARKET",
+                        "STOPLOSS",
+                        "STOPLIMIT"
+                    ],
+                    "strikePrice": -0.0001,
+                    "symbol": "AIR",
+                    "tradable": true,
+                    "vwdId": "360114899",
+                    "vwdIdSecondary": "955000256",
+                    "vwdIdentifierType": "issueid",
+                    "vwdIdentifierTypeSecondary": "issueid",
+                    "vwdModuleId": 1,
+                    "vwdModuleIdSecondary": 2
+                }
+            ]
+        }
 
     """
     check_session_config(session)
     url = URLs.get_product_search_url(session, product_type_id)
-    # TODO: Implement to target specialized URLs
     # Example query for stocks:
     # indexId=5&stockCountryId=886&requireTotal=true&offset=0&limit=100&sortColumns=name&sortTypes=asc&intAccount=123123123&sessionId=sdfasdfasdf
     params = dict(
         offset=offset,
         limit=limit,
-        searchText=search_txt,
         intAccount=session.client.int_account,
-        sessionId=session.config.session_id
+        sessionId=session.config.session_id,
+        requireTotal=True
     )
+    if search_txt is not None:
+        params['searchText'] = search_txt
     if product_type_id is not None:
         params['productTypeId'] = product_type_id
+    if country_id is not None:
+        params['stockCountryId'] = country_id
+    if index_id is not None:
+        params['indexId'] = index_id
     LOGGER.debug("webapi.search_product params| %s", params)
     async with session as client:
         response = await client.get(url,
                                     cookies=session._cookies,
                                     params=params)
     check_response(response)
     LOGGER.debug("webapi.search_product response| %s", response.json())
```

### Comparing `degiroasync-0.18.1/degiroasync.egg-info/PKG-INFO` & `degiroasync-0.19.0/degiroasync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.18.1
+Version: 0.19.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # DegiroAsync
 
 ## Documentation
 
-Check out the online documentation [here](https://ohmajesticlama.github.io/degiroasync/index.html).
+Check out the [online documentation](https://ohmajesticlama.github.io/degiroasync/index.html).
 
 ## Introduction
 
 This project aims to provide an *unofficial* API for Degiro platform that works
 asynchronously.
```

### Comparing `degiroasync-0.18.1/degiroasync.egg-info/SOURCES.txt` & `degiroasync-0.19.0/degiroasync.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 degiroasync/webapi/login.py
 degiroasync/webapi/orders.py
 degiroasync/webapi/product.py
 tests/__init__.py
 tests/integration_login.py
 tests/test_core.py
 tests/test_degiroapi.py
-tests/test_degirowebapi.py
+tests/test_degirowebapi.py
+tests/test_setup.py
```

### Comparing `degiroasync-0.18.1/setup.py` & `degiroasync-0.19.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,28 @@
     description = "A Python asynchronous library for Degiro trading service."
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiroasync",
-        version="0.18.1",
+        version="0.19.0",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiroasync",
         project_urls={
             'Documentation':
                 'https://ohmajesticlama.github.io/degiroasync/index.html'
             },
         packages=setuptools.find_packages(),
         install_requires=[
             'httpx >= 0.21.3, < 1.0',
             'jsonloader >= 0.8.1, < 1.0',
-            'typeguard >= 2.13.3, < 3.0',
             'asyncstdlib >= 3.10.3, < 4.0',
             'more_itertools >= 8.12.0, < 9'
             ],
         extras_require={
             'dev': [
                 # Tests
                 'pytest >= 7.0.1',
```

### Comparing `degiroasync-0.18.1/tests/integration_login.py` & `degiroasync-0.19.0/tests/integration_login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/tests/test_core.py` & `degiroasync-0.19.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.1/tests/test_degiroapi.py` & `degiroasync-0.19.0/tests/test_degiroapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,39 +282,42 @@
         self.assertEqual(country.region.name, 'Europe')
 
 
 class TestProduct(unittest.IsolatedAsyncioTestCase):
     """
     Local tests for Product.
     """
-    @unittest.mock.patch('degiroasync.api.ExchangeDictionary.exchange_by')
     @unittest.mock.patch('degiroasync.webapi.get_products_info')
-    async def test_product(self, wapi_prodinfo_m, exchange_by_m):
+    async def test_product(self, wapi_prodinfo_m):
         wapi_prodinfo_m.return_value = {'data': {
                 '123': {
                     'id': '123',
-                    'product_type_id': 99,
+                    'productTypeId': 99,
                     'name': 'foo',
                     'symbol': 'FOO',
                     'currency': 'EUR',
                     'exchangeId': 'exid',
                     'tradable': True,
                     'isin': 'isinexample',
                 }
             }
         }
-        exchange_by_m.return_value = Exchange(dict(
-            id='idex',
-            name='EuroNext',
-            country_name='France',
-            hiq_abbr='EPA'
+
+        session = MagicMock()  # Don't care
+        session.exchange_dictionary = MagicMock()
+        session.exchange_dictionary.exchange_by = MagicMock(
+                return_value=Exchange(dict(
+                    id='exid',
+                    name='EuroNext',
+                    country_name='France',
+                    hiq_abbr='EPA',
             )
         )
 
-        session = MagicMock()  # Don't care
+                )
 
         # Test that degiroasync.api returns properly initiated products
         products_gen = ProductFactory.init_batch(
                 session,
                 (
                     {
                         'id': '123',
@@ -340,18 +343,29 @@
                     'currency': 'EUR',
                     'exchangeId': 'exid',
                     'tradable': True,
                     'isin': 'isinexample',
                 }
             }
         }
+        session = MagicMock()  # Don't care
+        session.exchange_dictionary = MagicMock()
+        session.exchange_dictionary.exchange_by = MagicMock(
+                return_value=Exchange(dict(
+                    id='exid',
+                    name='EuroNext',
+                    country_name='France',
+                    hiq_abbr='EPA',
+                        )
+                    )
+            )
 
         # Test that degiroasync.api returns properly initiated products
         products_gen = ProductFactory.init_batch(
-                MagicMock(),  # Don't care about session here
+                session,  # Don't care about session here
                 [
                     {
                         'id': '123',
                         'additional': 123,
                     },
                 ],
                 size=1)
@@ -747,17 +761,14 @@
             session = await _IntegrationLogin._login()
             symbol = 'AIR'
             products = await degiroasync.api.search_product(session,
                                                             by_symbol=symbol)
             self.assertGreaterEqual(len(products), 1)
             for product in products:
                 self.assertEqual(symbol, product.info.symbol, product.info)
-                # We should only have airbus products here
-                #self.assertTrue('airbus' in product.info.name.lower(),
-                #               product.info)
 
         async def test_search_product_symbol_air(self):
             session = await _IntegrationLogin._login()
             symbol = 'AIR'  # GE symbol on EPA
             products = await degiroasync.api.search_product(session,
                                                             by_symbol=symbol,
                                                             by_exchange='EPA')
@@ -789,14 +800,32 @@
             # is to target one specific product. Raise an error if it doesn't
             # work.
             self.assertEqual(len(products), 1)
             for product in products:
                 # We should only have airbus products here
                 self.assertTrue('airbus' in product.info.name.lower())
 
+        async def test_search_product_country(self):
+            session = await _IntegrationLogin._login()
+            products = await degiroasync.api.search_product(
+                    session,
+                    by_country='FR',
+                    max_iter=1,  # We don't need every product for this test.
+                    )
+            # The point of implementing filtering on symbol and exchange
+            # is to target one specific product. Raise an error if it doesn't
+            # work.
+            self.assertGreaterEqual(len(products), 1)
+            for product in products:
+                self.assertEqual(
+                        session.exchange_dictionary.exchange_by(
+                            id=product.info.exchange_id).country_name,
+                        'FR'
+                        )
+
     class TestDegiroasyncIntegrationExchangeDictionary(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_product_dictionary_attributes(self):
             session = await _IntegrationLogin._login()
             dictionary = await degiroasync.api.ExchangeDictionary(session)
```

### Comparing `degiroasync-0.18.1/tests/test_degirowebapi.py` & `degiroasync-0.19.0/tests/test_degirowebapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from degiroasync.core import SessionCore
 from degiroasync.core.constants import PRODUCT
 from degiroasync.core.constants import PRICE
 from degiroasync.core.constants import ORDER
 from degiroasync.core.constants import LOGIN
 from degiroasync.core import ResponseError
 from degiroasync.core import BadCredentialsError
+from degiroasync.core.helpers import ThrottlingClient
 from degiroasync.webapi import get_config
 from degiroasync.webapi import get_products_info
 from degiroasync.webapi import get_company_profile
 from degiroasync.webapi import get_news_by_company
 
 
 LOGGER = logging.getLogger(degiroasync.core.LOGGER_NAME)
@@ -33,17 +34,24 @@
 RUN_INTEGRATION_TESTS = 0
 try:
     _env_var = os.environ.get('DEGIROASYNC_INTEGRATION')
     RUN_INTEGRATION_TESTS = int(_env_var)
 except (ValueError, TypeError):
     LOGGER.info('degiroasync integration tests will *not* run.')
 
+RUN_BAD_CREDENTIALS = 0
+try:
+    _env_var = os.environ.get('DEGIROASYNC_INTEGRATION_BAD_CREDENTIALS')
+    RUN_BAD_CREDENTIALS = int(_env_var)
+except (ValueError, TypeError):
+    LOGGER.info('degiroasync Bad Credentials integration test will *not* run.')
+
 
 class TestDegiroAsyncWebAPI(unittest.IsolatedAsyncioTestCase):
-    @unittest.mock.patch('httpx.AsyncClient.post')
+    @unittest.mock.patch('degiroasync.core.helpers.ThrottlingClient.post')
     async def test_login_bad_credentials(
             self,
             post_m
             ):
         """
         Verify that BadCredentialsError is raised when endpoint returns a bad
         credentials error.
@@ -64,60 +72,31 @@
             await degiroasync.webapi.login(credentials)
 
 
 if RUN_INTEGRATION_TESTS:
     LOGGER.info('degiroasync.webapi integration tests will run.')
     from tests.integration_login import _IntegrationLogin
 
-    #class _IntegrationWebLogin:
-    #    """
-    #    Internal helper, can be inherited to make login for integration tests
-    #    easier.
-    #    """
-    #    async def asyncSetUp(self):
-    #        self._lock = asyncio.Lock()
-    #        _IntegrationLogin._login_attempted = False
-    #        self.session: Optional[SessionCore] = None
-
-    #    async def _login(self):
-    #        if self.session is not None:
-    #            return self.session
-    #        async with self._lock:
-    #            if not _IntegrationLogin._login_attempted and not self.session:
-    #                _IntegrationLogin._login_attempted = True
-    #                credentials = _get_credentials()
-    #                import degiroasync.api
-    #                # Use api.login here to benefit from wrong password check:
-    #                # if provided credentials are incorrect, don't try again
-    #                # This will block the degiro account.
-    #                self.session = await degiroasync.api.login(
-    #                        credentials)
-    #            else:
-    #                LOGGER.warning(
-    #                        "Log in already attempted without success, skip.")
-    #        if not self.session:
-    #            raise ResponseError("No session available.")
-    #        return self.session
-
     class TestDegiroAsyncWebAPIIntegration(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
 
         async def test_login(self):
             session = await _IntegrationLogin._login()
             self.assertTrue('JSESSIONID' in session.cookies,
                             "No JSESSIONID found.")
 
-        async def test_login_bad_credentials(self):
-            credentials = Credentials(
-                username='dummyaccount123456',
-                password='dummydummy'
-                    )
-            with self.assertRaises(BadCredentialsError):
-                await degiroasync.webapi.login(credentials)
+        if RUN_BAD_CREDENTIALS:
+            async def test_login_bad_credentials(self):
+                credentials = Credentials(
+                    username='dummyaccount123456',
+                    password='dummydummy'
+                        )
+                with self.assertRaises(BadCredentialsError):
+                    await degiroasync.webapi.login(credentials)
 
         async def test_config(self):
             session = await _IntegrationLogin._login()
             await get_config(session)
             LOGGER.debug('test_config| %s', session.config)
             self.assertTrue(
                     session.config.pa_url is not None,
```

