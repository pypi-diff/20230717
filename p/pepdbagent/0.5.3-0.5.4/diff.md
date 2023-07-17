# Comparing `tmp/pepdbagent-0.5.3.tar.gz` & `tmp/pepdbagent-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.5.3.tar", last modified: Fri Jul 14 00:39:13 2023, max compression
+gzip compressed data, was "pepdbagent-0.5.4.tar", last modified: Mon Jul 17 14:55:18 2023, max compression
```

## Comparing `pepdbagent-0.5.3.tar` & `pepdbagent-0.5.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.349764 pepdbagent-0.5.3/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-14 00:39:02.000000 pepdbagent-0.5.3/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-17 14:55:18.000000 pepdbagent-0.5.4/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 14:55:18.000000 pepdbagent-0.5.4/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:55:18.000000 pepdbagent-0.5.4/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 14:55:18.000000 pepdbagent-0.5.4/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 14:55:18.000000 pepdbagent-0.5.4/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:18.973821 pepdbagent-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-07-17 14:55:04.000000 pepdbagent-0.5.4/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.5.3/LICENSE.txt` & `pepdbagent-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/PKG-INFO` & `pepdbagent-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.3/README.md` & `pepdbagent-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/pepdbagent/db_utils.py` & `pepdbagent-0.5.4/pepdbagent/db_utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/pepdbagent/exceptions.py` & `pepdbagent-0.5.4/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/pepdbagent/models.py` & `pepdbagent-0.5.4/pepdbagent/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,7 +126,26 @@
         if "?" in v:
             return ValueError("Question mark (?) is prohibited in name and tag.")
         return v
 
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
+
+
+class NamespaceInfo(BaseModel):
+    """
+    Model with information about namespace
+    """
+
+    namespace: str
+    number_of_projects: int
+
+
+class ListOfNamespaceInfo(BaseModel):
+    """
+    Namespace information response model
+    """
+
+    number_of_namespaces: int
+    limit: int
+    results: List[NamespaceInfo]
```

### Comparing `pepdbagent-0.5.3/pepdbagent/modules/annotation.py` & `pepdbagent-0.5.4/pepdbagent/modules/annotation.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/pepdbagent/modules/namespace.py` & `pepdbagent-0.5.4/pepdbagent/modules/namespace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from typing import List, Union
 
-from sqlalchemy import distinct, func, or_, select
+from sqlalchemy import distinct, func, or_, select, text
 from sqlalchemy.sql.selectable import Select
 from sqlalchemy.orm import Session
 
-from pepdbagent.const import DEFAULT_LIMIT, DEFAULT_OFFSET, PKG_NAME
+from pepdbagent.const import DEFAULT_LIMIT, DEFAULT_OFFSET, PKG_NAME, DEFAULT_LIMIT_INFO
 from pepdbagent.db_utils import Projects, BaseEngine
-from pepdbagent.models import Namespace, NamespaceList
+from pepdbagent.models import Namespace, NamespaceList, NamespaceInfo, ListOfNamespaceInfo
 from pepdbagent.utils import tuple_converter
 
 _LOGGER = logging.getLogger(PKG_NAME)
 
 
 class PEPDatabaseNamespace:
     """
@@ -67,14 +67,15 @@
         search_str: str,
         admin_nsp: tuple = None,
         limit: int = DEFAULT_LIMIT,
         offset: int = DEFAULT_OFFSET,
     ) -> List[Namespace]:
         """
         Search for namespace by providing search string.
+
         :param search_str: string of symbols, words, keywords to search in the
             namespace name.
         :param admin_nsp: tuple of namespaces where project can be retrieved if they are privet
         :param limit: limit of return results
         :param offset: number of results off set (that were already showed)
         :return: list of dict with structure {
                 namespace,
@@ -110,17 +111,18 @@
                     namespace=res.namespace,
                     number_of_projects=res.number_of_projects,
                     number_of_samples=res.number_of_samples,
                 )
             )
         return results_list
 
-    def _count_namespace(self, search_str: str = None, admin_nsp: tuple = None) -> int:
+    def _count_namespace(self, search_str: str = None, admin_nsp: tuple = tuple()) -> int:
         """
         Get number of found namespace. [This function is related to _get_namespaces]
+
         :param search_str: string of symbols, words, keywords to search in the
             namespace name.
         :param admin_nsp: tuple of namespaces where project can be retrieved if they are privet
         :return: number of found namespaces
         """
         statement = select(
             func.count(distinct(Projects.namespace)).label("number_of_namespaces")
@@ -156,7 +158,49 @@
                     Projects.namespace.ilike(sql_search_str),
                 )
             )
         statement = statement.where(
             or_(Projects.private.is_(False), Projects.namespace.in_(admin_list))
         )
         return statement
+
+    def info(self, limit: int = DEFAULT_LIMIT_INFO) -> ListOfNamespaceInfo:
+        """
+        Get list of top n namespaces in the database
+
+        :param limit: limit of results (top namespace )
+        :return: number_of_namespaces: int
+                 limit: int
+                 results: { namespace: str
+                            number_of_projects: int
+                            }
+        """
+        total_number_of_namespaces = self._count_namespace()
+
+        statement = (
+            select(
+                func.count(Projects.namespace).label("number_of_projects"),
+                Projects.namespace,
+            )
+            .select_from(Projects)
+            .where(Projects.private.is_(False))
+            .limit(limit)
+            .order_by(text("number_of_projects desc"))
+            .group_by(Projects.namespace)
+        )
+
+        with Session(self._sa_engine) as session:
+            query_results = session.execute(statement).all()
+
+        list_of_results = []
+        for result in query_results:
+            list_of_results.append(
+                NamespaceInfo(
+                    namespace=result.namespace,
+                    number_of_projects=result.number_of_projects,
+                )
+            )
+        return ListOfNamespaceInfo(
+            number_of_namespaces=total_number_of_namespaces,
+            limit=limit,
+            results=list_of_results,
+        )
```

### Comparing `pepdbagent-0.5.3/pepdbagent/modules/project.py` & `pepdbagent-0.5.4/pepdbagent/modules/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,19 +346,20 @@
 
                     found_prj.digest = project_digest
                     found_prj.number_of_samples = number_of_samples
                     found_prj.private = private
                     found_prj.pep_schema = pep_schema
                     found_prj.config = project_dict[CONFIG_KEY]
                     found_prj.description = description
+                    found_prj.last_update_date = datetime.datetime.now(datetime.timezone.utc)
 
                     # Deleting old samples and subsamples
                     if found_prj.samples_mapping:
                         for sample in found_prj.samples_mapping:
-                            _LOGGER.info(f"deleting samples: {str(sample)}")
+                            _LOGGER.debug(f"deleting samples: {str(sample)}")
                             session.delete(sample)
 
                     if found_prj.subsamples_mapping:
                         for subsample in found_prj.subsamples_mapping:
                             _LOGGER.debug(f"deleting subsamples: {str(subsample)}")
                             session.delete(subsample)
```

### Comparing `pepdbagent-0.5.3/pepdbagent/pepdbagent.py` & `pepdbagent-0.5.4/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/pepdbagent/utils.py` & `pepdbagent-0.5.4/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.5.4/pepdbagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.3/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.5.4/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/setup.py` & `pepdbagent-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/tests/conftest.py` & `pepdbagent-0.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.3/tests/test_pepagent.py` & `pepdbagent-0.5.4/tests/test_pepagent.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,7 +406,18 @@
     def test_annotation(self, initiate_pepdb_con):
         result = initiate_pepdb_con.namespace.get()
         assert len(result.results) == 3
 
     def test_annotation_private(self, initiate_pepdb_con):
         result = initiate_pepdb_con.namespace.get(admin="private_test")
         assert len(result.results) == 4
+
+    def test_namespace_info(self, initiate_pepdb_con):
+        initiate_pepdb_con.project.update(
+            namespace="private_test",
+            name="derive",
+            tag="default",
+            update_dict={"is_private": False},
+        )
+        result = initiate_pepdb_con.namespace.info()
+        assert len(result.results) == 4
+        assert result.results[3].number_of_projects == 1
```

