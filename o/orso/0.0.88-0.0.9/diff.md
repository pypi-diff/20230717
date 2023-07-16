# Comparing `tmp/orso-0.0.88.tar.gz` & `tmp/orso-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orso-0.0.88.tar", last modified: Sun Jul 16 22:42:36 2023, max compression
+gzip compressed data, was "orso-0.0.9.tar", last modified: Sun Mar 12 02:47:11 2023, max compression
```

## Comparing `orso-0.0.88.tar` & `orso-0.0.9.tar`

### file list

```diff
@@ -1,62 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.439409 orso-0.0.88/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-16 22:42:23.000000 orso-0.0.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-16 22:42:36.439409 orso-0.0.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-16 22:42:23.000000 orso-0.0.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.431409 orso-0.0.88/orso/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-16 22:42:23.000000 orso-0.0.88/orso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso/bitarray/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 22:42:23.000000 orso-0.0.88/orso/bitarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   232514 2023-07-16 22:42:23.000000 orso-0.0.88/orso/bitarray/cbitarray.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso/cityhash/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 22:42:23.000000 orso-0.0.88/orso/cityhash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-07-16 22:42:23.000000 orso-0.0.88/orso/cityhash/city.cc
--rw-r--r--   0 runner    (1001) docker     (123)   237362 2023-07-16 22:42:23.000000 orso-0.0.88/orso/cityhash/cityhash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-16 22:42:23.000000 orso-0.0.88/orso/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-07-16 22:42:23.000000 orso-0.0.88/orso/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-16 22:42:23.000000 orso-0.0.88/orso/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-16 22:42:23.000000 orso-0.0.88/orso/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 22:42:23.000000 orso-0.0.88/orso/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 22:42:23.000000 orso-0.0.88/orso/filters/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-16 22:42:23.000000 orso-0.0.88/orso/filters/cuckoo_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-16 22:42:23.000000 orso-0.0.88/orso/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-16 22:42:23.000000 orso-0.0.88/orso/logging/add_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-16 22:42:23.000000 orso-0.0.88/orso/logging/create_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-16 22:42:23.000000 orso-0.0.88/orso/logging/google_cloud_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-16 22:42:23.000000 orso-0.0.88/orso/logging/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 22:42:23.000000 orso-0.0.88/orso/logging/log_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-16 22:42:23.000000 orso-0.0.88/orso/profiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso/profiler/distogram/
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-07-16 22:42:23.000000 orso-0.0.88/orso/profiler/distogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-16 22:42:23.000000 orso-0.0.88/orso/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-16 22:42:23.000000 orso-0.0.88/orso/row.py
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-07-16 22:42:23.000000 orso-0.0.88/orso/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-16 22:42:23.000000 orso-0.0.88/orso/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-16 22:42:23.000000 orso-0.0.88/orso/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 22:42:23.000000 orso-0.0.88/orso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.435409 orso-0.0.88/orso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-16 22:42:36.000000 orso-0.0.88/orso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-16 22:42:36.000000 orso-0.0.88/orso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:42:36.000000 orso-0.0.88/orso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 22:42:36.000000 orso-0.0.88/orso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 22:42:36.000000 orso-0.0.88/orso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-16 22:42:23.000000 orso-0.0.88/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 22:42:36.439409 orso-0.0.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-16 22:42:23.000000 orso-0.0.88/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:42:36.439409 orso-0.0.88/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_cityhash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_converters_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_converters_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_converters_polars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_filter_bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_filter_cuckoo_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_schema_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-16 22:42:23.000000 orso-0.0.88/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.041472 orso-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-03-12 02:46:53.000000 orso-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-12 02:47:11.041472 orso-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-12 02:46:53.000000 orso-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.037472 orso-0.0.9/orso/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-12 02:46:53.000000 orso-0.0.9/orso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-12 02:46:53.000000 orso-0.0.9/orso/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-03-12 02:46:53.000000 orso-0.0.9/orso/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-03-12 02:46:53.000000 orso-0.0.9/orso/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-12 02:46:53.000000 orso-0.0.9/orso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-12 02:46:53.000000 orso-0.0.9/orso/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-12 02:46:53.000000 orso-0.0.9/orso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.037472 orso-0.0.9/orso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-12 02:46:53.000000 orso-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 02:47:11.041472 orso-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-12 02:46:53.000000 orso-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.041472 orso-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_converters_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_load_from_pyarrow.py
```

### Comparing `orso-0.0.88/LICENSE` & `orso-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orso-0.0.88/PKG-INFO` & `orso-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.88
-Summary: 🐻 DataFrame Library
+Version: 0.0.9
+Summary: 🐻 Dataframe Library
 Home-page: https://github.com/mabel-dev/orso/
+Author: @joocer
 Author-email: justin.joyce@joocer.com
+Maintainer: @joocer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 ![Orso](https://raw.githubusercontent.com/mabel-dev/orso/main/orso.png)
 
-**Orso is a shared DataFrame library for [Opteryx](https://opteryx.dev/), [Mabel](https://github.com/mabel-dev/mabel) and [HadroDB](https://github.com/mabel-dev/hadrodb).**
+**Orso is a shared Dataframe library for Opteryx and HadroDB.**
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/orso.svg)](https://pypi.org/project/orso/)
 [![Downloads](https://static.pepy.tech/badge/orso)](https://pepy.tech/project/orso)
 [![codecov](https://codecov.io/gh/mabel-dev/orso/branch/main/graph/badge.svg?token=nl9JwOVdPs)](https://codecov.io/gh/mabel-dev/orso)
 [![Documentation](https://img.shields.io/badge/Documentation-018EF5?logo=ReadMe&logoColor=fff&style=flat)](https://opteryx.dev/latest/get-started/ecosystem/orso/)
 
 </div>
 
-Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite ~~bear~~ DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
-
-In Opteryx, Orso provides most of the database Cursor functionality.
-
-In Mabel, Orso provides the data schema and validation functionality.
-
-In HadroDB, Orso provides functionality for handling datasets.
+Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
 
 ## License
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mabel-dev/orso/blob/master/LICENSE)
 
 Orso is licensed under Apache 2.0 unless explicitly indicated otherwise.
 
 ## Status
 
-[![Status](https://img.shields.io/badge/Status-beta-orange)](https://github.com/mabel-dev/orso)
+[![Status](https://img.shields.io/badge/Status-alpha-orange)](https://github.com/mabel-dev/orso)
 
-Orso is in beta. Beta means different things to different people, to us, being beta means:
+Orso is in alpha. Alpha means different things to different people, to us, being alpha means:
 
-- Interfaces are generally stable but may still have breaking changes
-- Unit test are not reliable enough to capture breaks to functionality
-- Bugs are likely to exist in edge cases
-- Code may not be tuned for performance
+- Interfaces may be significantly changed
+- Expected functionality is missing
+- Things that worked yesterday, don't work today
+- The results of the system may be unreliable
 
-As such, we really don't recommend using Orso in critical applications.
+As such, we really don't recommend using Orso anywhere where your data matters.
```

### Comparing `orso-0.0.88/README.md` & `orso-0.0.9/orso.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
+Metadata-Version: 2.1
+Name: orso
+Version: 0.0.9
+Summary: 🐻 Dataframe Library
+Home-page: https://github.com/mabel-dev/orso/
+Author: @joocer
+Author-email: justin.joyce@joocer.com
+Maintainer: @joocer
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 ![Orso](https://raw.githubusercontent.com/mabel-dev/orso/main/orso.png)
 
-**Orso is a shared DataFrame library for [Opteryx](https://opteryx.dev/), [Mabel](https://github.com/mabel-dev/mabel) and [HadroDB](https://github.com/mabel-dev/hadrodb).**
+**Orso is a shared Dataframe library for Opteryx and HadroDB.**
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/orso.svg)](https://pypi.org/project/orso/)
 [![Downloads](https://static.pepy.tech/badge/orso)](https://pepy.tech/project/orso)
 [![codecov](https://codecov.io/gh/mabel-dev/orso/branch/main/graph/badge.svg?token=nl9JwOVdPs)](https://codecov.io/gh/mabel-dev/orso)
 [![Documentation](https://img.shields.io/badge/Documentation-018EF5?logo=ReadMe&logoColor=fff&style=flat)](https://opteryx.dev/latest/get-started/ecosystem/orso/)
 
 </div>
 
-Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite ~~bear~~ DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
-
-In Opteryx, Orso provides most of the database Cursor functionality.
-
-In Mabel, Orso provides the data schema and validation functionality.
-
-In HadroDB, Orso provides functionality for handling datasets.
+Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
 
 ## License
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mabel-dev/orso/blob/master/LICENSE)
 
 Orso is licensed under Apache 2.0 unless explicitly indicated otherwise.
 
 ## Status
 
-[![Status](https://img.shields.io/badge/Status-beta-orange)](https://github.com/mabel-dev/orso)
+[![Status](https://img.shields.io/badge/Status-alpha-orange)](https://github.com/mabel-dev/orso)
 
-Orso is in beta. Beta means different things to different people, to us, being beta means:
+Orso is in alpha. Alpha means different things to different people, to us, being alpha means:
 
-- Interfaces are generally stable but may still have breaking changes
-- Unit test are not reliable enough to capture breaks to functionality
-- Bugs are likely to exist in edge cases
-- Code may not be tuned for performance
+- Interfaces may be significantly changed
+- Expected functionality is missing
+- Things that worked yesterday, don't work today
+- The results of the system may be unreliable
 
-As such, we really don't recommend using Orso in critical applications.
+As such, we really don't recommend using Orso anywhere where your data matters.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orso-0.0.88/orso/converters.py` & `orso-0.0.9/orso/converters.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,112 +8,108 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import itertools
 import typing
-from decimal import Decimal
 
+from orso.dataframe import DataFrame
 from orso.exceptions import MissingDependencyError
 from orso.row import Row
-from orso.schema import FlatColumn
-from orso.schema import RelationSchema
-from orso.types import PYTHON_TO_ORSO_MAP
 
 
 def to_arrow(dataset, size=None):
     try:
         import pyarrow
     except ImportError as import_error:
         raise MissingDependencyError(import_error.name) from import_error
-
     # Create a list of PyArrow arrays from the rows
-    rows = dataset._rows
-    arrays = [
-        pyarrow.array(col) for col in zip(*(rows if size is None else itertools.islice(rows, size)))
-    ]
-
+    arrays = [pyarrow.array(col) for col in zip(*dataset._rows)]
+    # Limit the number of rows to 'size'
+    if size:
+        arrays = itertools.islice(arrays, size)
     # Create a PyArrow table from the arrays and schema
-    if arrays:
-        table = pyarrow.Table.from_arrays(arrays, dataset.column_names)
-    else:
-        table = pyarrow.Table.from_arrays([[]] * len(dataset.column_names), dataset.column_names)
+    table = pyarrow.Table.from_arrays(arrays, dataset.column_names)
 
     return table
 
 
 def from_arrow(tables, size=None):
-    """
-    Convert an Arrow table or an iterable of Arrow tables to a generator of
-    Python objects.
-    """
+    try:
+        import pyarrow.lib as lib
+    except ImportError as import_error:
+        raise MissingDependencyError(import_error.name) from import_error
+
+    def _type_convert(field_type):
+        if field_type.id == lib.Type_BOOL:
+            return bool
+        if field_type.id == lib.Type_STRING:
+            return str
+        if field_type.id in {
+            lib.Type_INT8,
+            lib.Type_INT16,
+            lib.Type_INT32,
+            lib.Type_INT64,
+            lib.Type_UINT8,
+            lib.Type_UINT16,
+            lib.Type_UINT32,
+            lib.Type_UINT64,
+        }:
+            return int
+        if field_type.id in {lib.Type_HALF_FLOAT, lib.Type_FLOAT, lib.Type_DOUBLE}:
+            return float
+
+    def _peek(iterable):
+        iter1, iter2 = itertools.tee(iterable)
+        try:
+            first = next(iter1)
+        except StopIteration:
+            return None, iter([])
+        else:
+            return first, iter2
+
     if not isinstance(tables, (typing.Generator, list, tuple)):
         tables = [tables]
 
     if isinstance(tables, (list, tuple)):
         tables = iter(tables)
 
-    # Extract schema information from the first table
-    first_table = next(tables, None)
-    if first_table is None:
-        return [], {}
-
-    arrow_schema = first_table.schema
-
-    orso_schema = RelationSchema(
-        name="arrow",
-        columns=[FlatColumn.from_arrow(field) for field in arrow_schema],
-    )
+    first_table, all_tables = _peek(tables)
+    schema = first_table.schema
+    fields = {
+        str(field.name): {"type": _type_convert(field.type), "nullable": field.nullable}
+        for field in schema
+    }
 
     # Create a generator of tuples from the columns
-    row_factory = Row.create_class(orso_schema)
-
-    BATCH_SIZE: int = 10000
-    if size:
-        BATCH_SIZE = min(size, BATCH_SIZE)
-
-    rows: typing.List[Row] = []
-    for table in [first_table] + list(tables):
-        batches = table.to_batches(max_chunksize=BATCH_SIZE)
-        for batch in batches:
-            column_data_dict = batch.to_pydict()
-            column_data = [column_data_dict[name] for name in arrow_schema.names]
-            new_rows: typing.Iterable = [tuple()] * batch.num_rows
-            for i, row_data in enumerate(zip(*column_data)):
-                new_rows[i] = row_factory(row_data)  # type:ignore
-            rows.extend(new_rows)
-            if size and len(rows) >= size:
-                break
+    row_factory = Row.create_class(fields)
+    rows = (
+        (row_factory(col[i].as_py() for col in [table.column(j) for j in schema.names]))
+        for table in all_tables
+        for i in range(table.num_rows)
+    )
 
     # Limit the number of rows to 'size'
     if size:
-        rows = itertools.islice(rows, size)  # type:ignore
+        rows = itertools.islice(rows, size)
 
-    return rows, orso_schema
+    return DataFrame(rows=rows, schema=fields)
 
 
-def to_pandas(dataset, size=None):
-    try:
-        import pandas
-    except ImportError as import_error:
-        raise MissingDependencyError(import_error.name) from import_error
-    return pandas.DataFrame(r.as_dict for r in dataset.slice(0, size))
+def to_pandas(dataset):
+    raise NotImplementedError()
 
 
 def from_pandas(pandas):
     raise NotImplementedError()
 
 
-def to_polars(dataset, size=None):
-    try:
-        import polars
-    except ImportError as import_error:
-        raise MissingDependencyError(import_error.name) from import_error
-    return polars.DataFrame(r.as_dict for r in dataset.slice(0, size))
+def to_polars(dataset):
+    raise NotImplementedError()
 
 
 def from_polars(polars):
     raise NotImplementedError()
 
 
 def to_csv(dataset):
```

### Comparing `orso-0.0.88/orso/version.py` & `orso-0.0.9/orso/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__: str = "0.0.88"
+__version__: str = "0.0.9"
 __author__: str = "@joocer"
```

### Comparing `orso-0.0.88/orso.egg-info/PKG-INFO` & `orso-0.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-Metadata-Version: 2.1
-Name: orso
-Version: 0.0.88
-Summary: 🐻 DataFrame Library
-Home-page: https://github.com/mabel-dev/orso/
-Author-email: justin.joyce@joocer.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 ![Orso](https://raw.githubusercontent.com/mabel-dev/orso/main/orso.png)
 
-**Orso is a shared DataFrame library for [Opteryx](https://opteryx.dev/), [Mabel](https://github.com/mabel-dev/mabel) and [HadroDB](https://github.com/mabel-dev/hadrodb).**
+**Orso is a shared Dataframe library for Opteryx and HadroDB.**
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/orso.svg)](https://pypi.org/project/orso/)
 [![Downloads](https://static.pepy.tech/badge/orso)](https://pepy.tech/project/orso)
 [![codecov](https://codecov.io/gh/mabel-dev/orso/branch/main/graph/badge.svg?token=nl9JwOVdPs)](https://codecov.io/gh/mabel-dev/orso)
 [![Documentation](https://img.shields.io/badge/Documentation-018EF5?logo=ReadMe&logoColor=fff&style=flat)](https://opteryx.dev/latest/get-started/ecosystem/orso/)
 
 </div>
 
-Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite ~~bear~~ DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
-
-In Opteryx, Orso provides most of the database Cursor functionality.
-
-In Mabel, Orso provides the data schema and validation functionality.
-
-In HadroDB, Orso provides functionality for handling datasets.
+Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
 
 ## License
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mabel-dev/orso/blob/master/LICENSE)
 
 Orso is licensed under Apache 2.0 unless explicitly indicated otherwise.
 
 ## Status
 
-[![Status](https://img.shields.io/badge/Status-beta-orange)](https://github.com/mabel-dev/orso)
+[![Status](https://img.shields.io/badge/Status-alpha-orange)](https://github.com/mabel-dev/orso)
 
-Orso is in beta. Beta means different things to different people, to us, being beta means:
+Orso is in alpha. Alpha means different things to different people, to us, being alpha means:
 
-- Interfaces are generally stable but may still have breaking changes
-- Unit test are not reliable enough to capture breaks to functionality
-- Bugs are likely to exist in edge cases
-- Code may not be tuned for performance
+- Interfaces may be significantly changed
+- Expected functionality is missing
+- Things that worked yesterday, don't work today
+- The results of the system may be unreliable
 
-As such, we really don't recommend using Orso in critical applications.
+As such, we really don't recommend using Orso anywhere where your data matters.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `orso-0.0.88/setup.py` & `orso-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from Cython.Build import cythonize
-from setuptools import Extension
 from setuptools import find_packages
 from setuptools import setup
 
 LIBRARY = "orso"
 
 
 __version__ = "notset"
@@ -17,35 +15,23 @@
 try:
     with open("requirements.txt", "r") as f:
         required = f.read().splitlines()
 except:
     with open(f"{LIBRARY}.egg-info/requires.txt", "r") as f:
         required = f.read().splitlines()
 
-extensions = [
-    Extension(
-        name="orso.cityhash.cityhash",
-        sources=[
-            "orso/cityhash/city.cc",
-            "orso/cityhash/cityhash.cpp",
-        ],
-    ),
-    Extension(
-        name="orso.bitarray.cbitarray",
-        sources=["orso/bitarray/cbitarray.pyx"],
-    ),
-]
 
 setup_config = {
     "name": LIBRARY,
     "version": __version__,
-    "description": "🐻 DataFrame Library",
+    "description": "🐻 Dataframe Library",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
+    "maintainer": "@joocer",
+    "author": "@joocer",
     "author_email": "justin.joyce@joocer.com",
     "packages": find_packages(include=[LIBRARY, f"{LIBRARY}.*"]),
     "url": "https://github.com/mabel-dev/orso/",
-    "ext_modules": cythonize(extensions),
     "install_requires": required,
 }
 
 setup(**setup_config)
```

### Comparing `orso-0.0.88/tests/test_fetching.py` & `orso-0.0.9/tests/test_fetching.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 
 from orso.dataframe import DataFrame
 
 
 def test_fetchall():
     dataframe = DataFrame(
         rows=[(1, "John"), (2, "Jane"), (3, "Bob")],
-        schema=["id", "name"],
+        schema={"id": {"type": int}, "name": {"type": str}},
     )
     result = dataframe.fetchall()
     expected = [(1, "John"), (2, "Jane"), (3, "Bob")]
     assert result == expected
-    assert dataframe.fetchall() == [], dataframe.fetchall()
 
 
 def test_fetchone():
     dataframe = DataFrame(
         rows=[(1, "John"), (2, "Jane"), (3, "Bob")],
-        schema=["id", "name"],
+        schema={"id": {"type": int}, "name": {"type": str}},
     )
     result1 = dataframe.fetchone()
     expected1 = (1, "John")
     assert result1 == expected1
 
     result2 = dataframe.fetchone()
     expected2 = (2, "Jane")
@@ -38,48 +37,27 @@
     expected4 = None
     assert result4 == expected4
 
 
 def test_fetchmany():
     dataframe = DataFrame(
         rows=[(1, "John"), (2, "Jane"), (3, "Bob")],
-        schema=["id", "name"],
+        schema={"id": {"type": int}, "name": {"type": str}},
     )
     result1 = dataframe.fetchmany(2)
     expected1 = [(1, "John"), (2, "Jane")]
     assert result1 == expected1, result1
 
     result2 = dataframe.fetchmany(2)
     expected2 = [(3, "Bob")]
     assert result2 == expected2, result2
 
     result3 = dataframe.fetchmany(2)
     expected3 = []
     assert result3 == expected3, result3
 
 
-def test_fetch_methods():
-    dataframe = DataFrame(
-        rows=[(1, "John"), (2, "Jane"), (3, "Bob")],
-        schema=["id", "name"],
-    )
-
-    # Test fetchone
-    result1 = dataframe.fetchone()
-    expected1 = (1, "John")
-    assert result1 == expected1
-
-    # Test fetchmany
-    result2 = dataframe.fetchmany(2)
-    expected2 = [(2, "Jane"), (3, "Bob")]
-    assert result2 == expected2
-
-    # Test fetchall
-    result3 = dataframe.fetchall()
-    expected3 = []
-    assert result3 == expected3
-
-
-if __name__ == "__main__":  # prgama: nocover
-    from tests import run_tests
-
-    run_tests()
+if __name__ == "__main__":  # pragma: no cover
+    test_fetchone()
+    test_fetchmany()
+    test_fetchall()
+    print("✅ okay")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

