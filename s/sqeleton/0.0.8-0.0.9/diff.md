# Comparing `tmp/sqeleton-0.0.8.tar.gz` & `tmp/sqeleton-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqeleton-0.0.8.tar", max compression
+gzip compressed data, was "sqeleton-0.0.9.tar", max compression
```

## Comparing `sqeleton-0.0.8.tar` & `sqeleton-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1065 2023-02-10 14:52:28.608775 sqeleton-0.0.8/LICENSE
--rw-r--r--   0        0        0     3002 2023-02-10 14:52:28.608901 sqeleton-0.0.8/README.md
--rw-r--r--   0        0        0     2212 2023-04-03 10:05:57.858760 sqeleton-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       76 2023-02-10 14:52:28.614033 sqeleton-0.0.8/sqeleton/__init__.py
--rw-r--r--   0        0        0      584 2023-02-10 14:52:28.614157 sqeleton-0.0.8/sqeleton/__main__.py
--rw-r--r--   0        0        0      254 2023-02-10 14:52:28.614324 sqeleton-0.0.8/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-02-10 14:52:28.614446 sqeleton-0.0.8/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    10339 2023-03-10 11:29:18.850790 sqeleton-0.0.8/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     5909 2023-03-01 12:11:42.264799 sqeleton-0.0.8/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-02-10 14:52:28.614858 sqeleton-0.0.8/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0     8937 2023-02-10 14:52:28.614997 sqeleton-0.0.8/sqeleton/conn_editor.py
--rw-r--r--   0        0        0      554 2023-02-10 14:52:28.615210 sqeleton-0.0.8/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9111 2023-02-10 14:52:28.615350 sqeleton-0.0.8/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    19909 2023-04-02 20:21:45.070584 sqeleton-0.0.8/sqeleton/databases/base.py
--rw-r--r--   0        0        0     7140 2023-02-10 14:52:28.615703 sqeleton-0.0.8/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-02-10 14:52:28.615855 sqeleton-0.0.8/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-02-10 14:52:28.615995 sqeleton-0.0.8/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-03-01 12:11:42.265963 sqeleton-0.0.8/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-02-10 14:52:28.616262 sqeleton-0.0.8/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-03-01 12:11:42.266508 sqeleton-0.0.8/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6523 2023-03-01 12:11:42.267017 sqeleton-0.0.8/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5401 2023-03-10 11:29:18.853225 sqeleton-0.0.8/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6183 2023-03-10 11:29:18.853848 sqeleton-0.0.8/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     4844 2023-03-10 11:29:18.854139 sqeleton-0.0.8/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7732 2023-03-31 23:35:15.884422 sqeleton-0.0.8/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-02-10 14:52:28.617268 sqeleton-0.0.8/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-02-10 14:52:28.617498 sqeleton-0.0.8/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-02-10 14:52:28.617733 sqeleton-0.0.8/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-02 20:21:45.072025 sqeleton-0.0.8/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30646 2023-04-02 20:21:45.073157 sqeleton-0.0.8/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-02-10 14:52:28.618325 sqeleton-0.0.8/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-02-10 14:52:28.618458 sqeleton-0.0.8/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-02-10 14:52:28.618579 sqeleton-0.0.8/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1384 2023-02-10 14:52:28.618703 sqeleton-0.0.8/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-03-01 12:11:42.268414 sqeleton-0.0.8/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-02-10 14:52:28.619136 sqeleton-0.0.8/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-02 20:21:45.073750 sqeleton-0.0.8/sqeleton/utils.py
--rw-r--r--   0        0        0     5208 1970-01-01 00:00:00.000000 sqeleton-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1118 2023-04-20 22:14:47.343750 sqeleton-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2430 2023-07-17 08:33:47.571898 sqeleton-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5985 2023-05-21 15:25:37.554368 sqeleton-0.0.9/README.md
+-rw-r--r--   0        0        0      103 2023-07-17 08:33:56.534088 sqeleton-0.0.9/sqeleton/__init__.py
+-rw-r--r--   0        0        0      612 2023-05-12 07:53:31.094088 sqeleton-0.0.9/sqeleton/__main__.py
+-rw-r--r--   0        0        0      268 2023-04-20 22:12:19.910000 sqeleton-0.0.9/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      424 2023-06-08 09:42:16.319189 sqeleton-0.0.9/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    10846 2023-07-17 08:07:35.367651 sqeleton-0.0.9/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     6078 2023-05-08 12:16:59.177932 sqeleton-0.0.9/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2214 2023-05-08 12:16:59.178928 sqeleton-0.0.9/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0     9149 2023-05-08 12:16:59.178928 sqeleton-0.0.9/sqeleton/conn_editor.py
+-rw-r--r--   0        0        0      580 2023-07-17 08:07:35.367651 sqeleton-0.0.9/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9382 2023-04-20 22:12:19.914011 sqeleton-0.0.9/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    22160 2023-07-17 08:07:35.368650 sqeleton-0.0.9/sqeleton/databases/base.py
+-rw-r--r--   0        0        0     7353 2023-04-20 22:12:19.915003 sqeleton-0.0.9/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6838 2023-04-20 22:12:19.915003 sqeleton-0.0.9/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     7158 2023-04-20 22:12:19.915003 sqeleton-0.0.9/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6307 2023-07-17 08:07:35.369654 sqeleton-0.0.9/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      935 2023-04-20 22:12:19.916002 sqeleton-0.0.9/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4657 2023-07-17 08:07:35.370652 sqeleton-0.0.9/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6669 2023-05-08 12:16:59.179930 sqeleton-0.0.9/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5874 2023-07-17 08:07:35.371652 sqeleton-0.0.9/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     7034 2023-07-17 08:07:35.371652 sqeleton-0.0.9/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     4972 2023-04-20 22:12:19.918002 sqeleton-0.0.9/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7960 2023-04-20 22:12:19.918002 sqeleton-0.0.9/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1366 2023-07-17 08:07:35.372650 sqeleton-0.0.9/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5607 2023-04-20 22:12:19.919001 sqeleton-0.0.9/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      530 2023-07-17 08:07:35.373649 sqeleton-0.0.9/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5669 2023-07-17 08:07:35.374650 sqeleton-0.0.9/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    42859 2023-07-17 08:07:35.375649 sqeleton-0.0.9/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      451 2023-07-17 08:07:35.376653 sqeleton-0.0.9/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     5216 2023-07-17 08:07:35.377651 sqeleton-0.0.9/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     2047 2023-04-20 22:12:19.922002 sqeleton-0.0.9/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1438 2023-04-20 22:12:19.922002 sqeleton-0.0.9/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     6511 2023-07-17 08:07:35.378652 sqeleton-0.0.9/sqeleton/repl.py
+-rw-r--r--   0        0        0     2218 2023-07-17 08:07:35.379651 sqeleton-0.0.9/sqeleton/schema.py
+-rw-r--r--   0        0        0     9415 2023-07-17 08:07:35.380650 sqeleton-0.0.9/sqeleton/utils.py
+-rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 sqeleton-0.0.9/setup.py
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 sqeleton-0.0.9/PKG-INFO
```

### Comparing `sqeleton-0.0.8/LICENSE` & `sqeleton-0.0.9/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-MIT License
-
-Copyright (c) 2022 Datafold
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Datafold
+Copyright (c) 2023 Erez Shinan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sqeleton-0.0.8/pyproject.toml` & `sqeleton-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,81 @@
-[tool.poetry]
-name = "sqeleton"
-version = "0.0.8"
-description = "Python library for querying SQL databases"
-authors = ["Erez Shinan <erezshin@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-repository = "https://github.com/datafold/sqeleton"
-documentation = ""
-classifiers = [
-    "Intended Audience :: Developers",
-    "Intended Audience :: Information Technology",
-    "Intended Audience :: System Administrators",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Development Status :: 2 - Pre-Alpha",
-    "Environment :: Console",
-    "Topic :: Database :: Database Engines/Servers",
-    "Typing :: Typed"
-]
-packages = [{ include = "sqeleton" }]
-
-[tool.poetry.dependencies]
-python = "^3.7"
-runtype = "^0.2.6"
-dsnparse = "*"
-click = "^8.1"
-rich = "*"
-toml = "^0.10.2"
-mysql-connector-python = {version="8.0.29", optional=true}
-psycopg2 = {version="*", optional=true}
-snowflake-connector-python = {version="^2.7.2", optional=true}
-cryptography = {version="*", optional=true}
-trino = {version="^0.314.0", optional=true}
-presto-python-client = {version="*", optional=true}
-clickhouse-driver = {version="*", optional=true}
-duckdb = {version="^0.7.0", optional=true}
-textual = {version="^0.9.1", optional=true}
-textual-select = {version="*", optional=true}
-
-[tool.poetry.dev-dependencies]
-parameterized = "*"
-unittest-parallel = "*"
-
-duckdb = "^0.7.0"
-mysql-connector-python = "*"
-psycopg2 = "*"
-snowflake-connector-python = "^2.7.2"
-cryptography = "*"
-trino = "^0.314.0"
-presto-python-client = "*"
-clickhouse-driver = "*"
-vertica-python = "*"
-
-[tool.poetry.extras]
-mysql = ["mysql-connector-python"]
-postgresql = ["psycopg2"]
-snowflake = ["snowflake-connector-python", "cryptography"]
-presto = ["presto-python-client"]
-oracle = ["cx_Oracle"]
-# databricks = ["databricks-sql-connector"]
-trino = ["trino"]
-clickhouse = ["clickhouse-driver"]
-vertica = ["vertica-python"]
-duckdb = ["duckdb"]
-tui = ["textual", "textual-select"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.scripts]
-sqeleton = 'sqeleton.__main__:main'
+[tool.poetry]
+name = "sqeleton"
+version = "0.0.9"
+description = "Python library for querying SQL databases"
+authors = ["Erez Shinan <erezshin@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+repository = "https://github.com/erezsh/sqeleton"
+documentation = ""
+classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: System Administrators",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Development Status :: 2 - Pre-Alpha",
+    "Environment :: Console",
+    "Topic :: Database :: Database Engines/Servers",
+    "Typing :: Typed"
+]
+packages = [{ include = "sqeleton" }]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+runtype = "^0.3.5"
+dsnparse = "*"
+click = "^8.1"
+rich = "*"
+toml = "^0.10.2"
+mysql-connector-python = {version="8.0.29", optional=true}
+psycopg2 = {version="*", optional=true}
+snowflake-connector-python = {version="^2.7.2", optional=true}
+cryptography = {version="*", optional=true}
+trino = {version="^0.314.0", optional=true}
+presto-python-client = {version="*", optional=true}
+clickhouse-driver = {version="*", optional=true}
+duckdb = {version="^0.7.0", optional=true}
+textual = {version="^0.9.1", optional=true}
+textual-select = {version="*", optional=true}
+pygments = {version="^2.13.0", optional=true}
+prompt-toolkit = {version="^3.0.36", optional=true}
+
+[tool.poetry.dev-dependencies]
+parameterized = "*"
+unittest-parallel = "*"
+
+duckdb = "^0.7.0"
+mysql-connector-python = "*"
+psycopg2 = "*"
+snowflake-connector-python = "^2.7.2"
+cryptography = "*"
+trino = "^0.314.0"
+presto-python-client = "*"
+clickhouse-driver = "*"
+vertica-python = "*"
+
+[tool.poetry.extras]
+mysql = ["mysql-connector-python"]
+postgresql = ["psycopg2"]
+snowflake = ["snowflake-connector-python", "cryptography"]
+presto = ["presto-python-client"]
+oracle = ["cx_Oracle"]
+# databricks = ["databricks-sql-connector"]
+trino = ["trino"]
+clickhouse = ["clickhouse-driver"]
+vertica = ["vertica-python"]
+duckdb = ["duckdb"]
+tui = ["textual", "textual-select", "pygments", "prompt-toolkit"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+sqeleton = 'sqeleton.__main__:main'
+
+[tool.ruff]
+line-length = 120
+target-version = "py38"
+
```

### Comparing `sqeleton-0.0.8/sqeleton/abcs/database_types.py` & `sqeleton-0.0.9/sqeleton/abcs/database_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,384 +1,388 @@
-import decimal
-from abc import ABC, abstractmethod
-from typing import Sequence, Optional, Tuple, Union, Dict, List
-from datetime import datetime
-
-from runtype import dataclass
-
-from ..utils import ArithAlphanumeric, ArithUUID, Self, Unknown
-
-
-DbPath = Tuple[str, ...]
-DbKey = Union[int, str, bytes, ArithUUID, ArithAlphanumeric]
-DbTime = datetime
-
-
-class ColType:
-    supported = True
-
-
-@dataclass
-class PrecisionType(ColType):
-    precision: int
-    rounds: Union[bool, Unknown] = Unknown
-
-
-class Boolean(ColType):
-    precision = 0
-
-
-class TemporalType(PrecisionType):
-    pass
-
-
-class Timestamp(TemporalType):
-    pass
-
-
-class TimestampTZ(TemporalType):
-    pass
-
-
-class Datetime(TemporalType):
-    pass
-
-
-class Date(TemporalType):
-    pass
-
-
-@dataclass
-class NumericType(ColType):
-    # 'precision' signifies how many fractional digits (after the dot) we want to compare
-    precision: int
-
-
-class FractionalType(NumericType):
-    pass
-
-
-class Float(FractionalType):
-    python_type = float
-
-
-class IKey(ABC):
-    "Interface for ColType, for using a column as a key in table."
-
-    @property
-    @abstractmethod
-    def python_type(self) -> type:
-        "Return the equivalent Python type of the key"
-
-    def make_value(self, value):
-        return self.python_type(value)
-
-
-class Decimal(FractionalType, IKey):  # Snowflake may use Decimal as a key
-    @property
-    def python_type(self) -> type:
-        if self.precision == 0:
-            return int
-        return decimal.Decimal
-
-
-@dataclass
-class StringType(ColType):
-    python_type = str
-
-
-class ColType_UUID(ColType, IKey):
-    python_type = ArithUUID
-
-
-class ColType_Alphanum(ColType, IKey):
-    python_type = ArithAlphanumeric
-
-
-class Native_UUID(ColType_UUID):
-    pass
-
-
-class String_UUID(ColType_UUID, StringType):
-    pass
-
-
-class String_Alphanum(ColType_Alphanum, StringType):
-    @staticmethod
-    def test_value(value: str) -> bool:
-        try:
-            ArithAlphanumeric(value)
-            return True
-        except ValueError:
-            return False
-
-    def make_value(self, value):
-        return self.python_type(value)
-
-
-class String_VaryingAlphanum(String_Alphanum):
-    pass
-
-
-@dataclass
-class String_FixedAlphanum(String_Alphanum):
-    length: int
-
-    def make_value(self, value):
-        if len(value) != self.length:
-            raise ValueError(f"Expected alphanumeric value of length {self.length}, but got '{value}'.")
-        return self.python_type(value, max_len=self.length)
-
-
-@dataclass
-class Text(StringType):
-    supported = False
-
-
-@dataclass
-class Integer(NumericType, IKey):
-    precision: int = 0
-    python_type: type = int
-
-    def __post_init__(self):
-        assert self.precision == 0
-
-
-@dataclass
-class UnknownColType(ColType):
-    text: str
-
-    supported = False
-
-
-class AbstractDialect(ABC):
-    """Dialect-dependent query expressions"""
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        "Name of the dialect"
-
-    @classmethod
-    @abstractmethod
-    def load_mixins(cls, *abstract_mixins) -> Self:
-        "Load a list of mixins that implement the given abstract mixins"
-
-    @property
-    @abstractmethod
-    def ROUNDS_ON_PREC_LOSS(self) -> bool:
-        "True if db rounds real values when losing precision, False if it truncates."
-
-    @abstractmethod
-    def quote(self, s: str):
-        "Quote SQL name"
-
-    @abstractmethod
-    def concat(self, items: List[str]) -> str:
-        "Provide SQL for concatenating a bunch of columns into a string"
-
-    @abstractmethod
-    def is_distinct_from(self, a: str, b: str) -> str:
-        "Provide SQL for a comparison where NULL = NULL is true"
-
-    @abstractmethod
-    def to_string(self, s: str) -> str:
-        # TODO rewrite using cast_to(x, str)
-        "Provide SQL for casting a column to string"
-
-    @abstractmethod
-    def random(self) -> str:
-        "Provide SQL for generating a random number betweein 0..1"
-
-    @abstractmethod
-    def current_timestamp(self) -> str:
-        "Provide SQL for returning the current timestamp, aka now"
-
-    @abstractmethod
-    def offset_limit(self, offset: Optional[int] = None, limit: Optional[int] = None):
-        "Provide SQL fragment for limit and offset inside a select"
-
-    @abstractmethod
-    def explain_as_text(self, query: str) -> str:
-        "Provide SQL for explaining a query, returned as table(varchar)"
-
-    @abstractmethod
-    def timestamp_value(self, t: datetime) -> str:
-        "Provide SQL for the given timestamp value"
-
-    @abstractmethod
-    def set_timezone_to_utc(self) -> str:
-        "Provide SQL for setting the session timezone to UTC"
-
-    @abstractmethod
-    def parse_type(
-        self,
-        table_path: DbPath,
-        col_name: str,
-        type_repr: str,
-        datetime_precision: int = None,
-        numeric_precision: int = None,
-        numeric_scale: int = None,
-    ) -> ColType:
-        "Parse type info as returned by the database"
-
-
-from typing import TypeVar, Generic
-
-T_Dialect = TypeVar("T_Dialect", bound=AbstractDialect)
-
-
-class AbstractDatabase(Generic[T_Dialect]):
-    @property
-    @abstractmethod
-    def dialect(self) -> T_Dialect:
-        "The dialect of the database. Used internally by Database, and also available publicly."
-
-    @classmethod
-    @abstractmethod
-    def load_mixins(cls, *abstract_mixins) -> type:
-        "Extend the dialect with a list of mixins that implement the given abstract mixins."
-
-    @property
-    @abstractmethod
-    def CONNECT_URI_HELP(self) -> str:
-        "Example URI to show the user in help and error messages"
-
-    @property
-    @abstractmethod
-    def CONNECT_URI_PARAMS(self) -> List[str]:
-        "List of parameters given in the path of the URI"
-
-    @abstractmethod
-    def _query(self, sql_code: str) -> list:
-        "Send query to database and return result"
-
-    @abstractmethod
-    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
-        """Query the table for its schema for table in 'path', and return {column: tuple}
-        where the tuple is (table_name, col_name, type_repr, datetime_precision?, numeric_precision?, numeric_scale?)
-
-        Note: This method exists instead of select_table_schema(), just because not all databases support
-              accessing the schema using a SQL query.
-        """
-
-    @abstractmethod
-    def select_table_unique_columns(self, path: DbPath) -> str:
-        "Provide SQL for selecting the names of unique columns in the table"
-
-    @abstractmethod
-    def query_table_unique_columns(self, path: DbPath) -> List[str]:
-        """Query the table for its unique columns for table in 'path', and return {column}"""
-
-    @abstractmethod
-    def _process_table_schema(
-        self, path: DbPath, raw_schema: Dict[str, tuple], filter_columns: Sequence[str], where: str = None
-    ):
-        """Process the result of query_table_schema().
-
-        Done in a separate step, to minimize the amount of processed columns.
-        Needed because processing each column may:
-        * throw errors and warnings
-        * query the database to sample values
-
-        """
-
-    @abstractmethod
-    def parse_table_name(self, name: str) -> DbPath:
-        "Parse the given table name into a DbPath"
-
-    @abstractmethod
-    def close(self):
-        "Close connection(s) to the database instance. Querying will stop functioning."
-
-    @property
-    @abstractmethod
-    def is_autocommit(self) -> bool:
-        "Return whether the database autocommits changes. When false, COMMIT statements are skipped."
-
-
-class AbstractTable(ABC):
-    @abstractmethod
-    def select(self, *exprs, distinct=False, **named_exprs) -> "AbstractTable":
-        """Choose new columns, based on the old ones. (aka Projection)
-
-        Parameters:
-            exprs: List of expressions to constitute the columns of the new table.
-                    If not provided, returns all columns in source table (i.e. ``select *``)
-            distinct: 'select' or 'select distinct'
-            named_exprs: More expressions to constitute the columns of the new table, aliased to keyword name.
-
-        """
-        # XXX distinct=SKIP
-
-    @abstractmethod
-    def where(self, *exprs) -> "AbstractTable":
-        """Filter the rows, based on the given predicates. (aka Selection)"""
-
-    @abstractmethod
-    def order_by(self, *exprs) -> "AbstractTable":
-        """Order the rows lexicographically, according to the given expressions."""
-
-    @abstractmethod
-    def limit(self, limit: int) -> "AbstractTable":
-        """Stop yielding rows after the given limit. i.e. take the first 'n=limit' rows"""
-
-    @abstractmethod
-    def join(self, target) -> "AbstractTable":
-        """Join the current table with the target table, returning a new table containing both side-by-side.
-
-        When joining, it's recommended to use explicit tables names, instead of `this`, in order to avoid potential name collisions.
-
-        Example:
-            ::
-
-                person = table('person')
-                city = table('city')
-
-                name_and_city = (
-                    person
-                    .join(city)
-                    .on(person['city_id'] == city['id'])
-                    .select(person['id'], city['name'])
-                )
-        """
-
-    @abstractmethod
-    def group_by(self, *keys):
-        """Behaves like in SQL, except for a small change in syntax:
-
-        A call to `.agg()` must follow every call to `.group_by()`.
-
-        Example:
-            ::
-
-                # SELECT a, sum(b) FROM tmp GROUP BY 1
-                table('tmp').group_by(this.a).agg(this.b.sum())
-
-                # SELECT a, sum(b) FROM a GROUP BY 1 HAVING (b > 10)
-                (table('tmp')
-                    .group_by(this.a)
-                    .agg(this.b.sum())
-                    .having(this.b > 10)
-                )
-
-        """
-
-    @abstractmethod
-    def count(self) -> int:
-        """SELECT count() FROM self"""
-
-    @abstractmethod
-    def union(self, other: "ITable"):
-        """SELECT * FROM self UNION other"""
-
-    @abstractmethod
-    def union_all(self, other: "ITable"):
-        """SELECT * FROM self UNION ALL other"""
-
-    @abstractmethod
-    def minus(self, other: "ITable"):
-        """SELECT * FROM self EXCEPT other"""
-
-    @abstractmethod
-    def intersect(self, other: "ITable"):
-        """SELECT * FROM self INTERSECT other"""
+import decimal
+from abc import ABC, abstractmethod
+from typing import Sequence, Optional, Tuple, Union, Dict, List, TypeVar, Generic, Any
+from datetime import datetime
+
+from runtype import dataclass
+
+from ..utils import ArithAlphanumeric, ArithUUID, Self, Unknown
+
+
+DbPath = Tuple[str, ...]
+DbKey = Union[int, str, bytes, ArithUUID, ArithAlphanumeric]
+DbTime = datetime
+
+
+class ColType:
+    supported = True
+
+
+@dataclass
+class PrecisionType(ColType):
+    precision: int
+    rounds: Union[bool, Unknown] = Unknown
+
+
+class Boolean(ColType):
+    precision = 0
+
+
+class TemporalType(PrecisionType):
+    pass
+
+
+class Timestamp(TemporalType):
+    pass
+
+
+class TimestampTZ(TemporalType):
+    pass
+
+
+class Datetime(TemporalType):
+    pass
+
+
+class Date(TemporalType):
+    pass
+
+
+@dataclass
+class NumericType(ColType):
+    # 'precision' signifies how many fractional digits (after the dot) we want to compare
+    precision: int
+
+
+class FractionalType(NumericType):
+    pass
+
+
+class Float(FractionalType):
+    python_type = float
+
+
+class IKey(ABC):
+    "Interface for ColType, for using a column as a key in table."
+
+    @property
+    @abstractmethod
+    def python_type(self) -> type:
+        "Return the equivalent Python type of the key"
+
+    def make_value(self, value):
+        return self.python_type(value)
+
+
+class Decimal(FractionalType, IKey):  # Snowflake may use Decimal as a key
+    @property
+    def python_type(self) -> type:
+        if self.precision == 0:
+            return int
+        return decimal.Decimal
+
+
+@dataclass
+class StringType(ColType):
+    python_type = str
+
+
+class ColType_UUID(ColType, IKey):
+    python_type = ArithUUID
+
+
+class ColType_Alphanum(ColType, IKey):
+    python_type = ArithAlphanumeric
+
+
+class Native_UUID(ColType_UUID):
+    pass
+
+
+class String_UUID(ColType_UUID, StringType):
+    pass
+
+
+class String_Alphanum(ColType_Alphanum, StringType):
+    @staticmethod
+    def test_value(value: str) -> bool:
+        try:
+            ArithAlphanumeric(value)
+            return True
+        except ValueError:
+            return False
+
+    def make_value(self, value):
+        return self.python_type(value)
+
+
+class String_VaryingAlphanum(String_Alphanum):
+    pass
+
+
+@dataclass
+class String_FixedAlphanum(String_Alphanum):
+    length: int
+
+    def make_value(self, value):
+        if len(value) != self.length:
+            raise ValueError(f"Expected alphanumeric value of length {self.length}, but got '{value}'.")
+        return self.python_type(value, max_len=self.length)
+
+
+@dataclass
+class Text(StringType):
+    supported = False
+
+
+@dataclass
+class Integer(NumericType, IKey):
+    precision: int = 0
+    python_type: type = int
+
+    def __post_init__(self):
+        assert self.precision == 0
+
+
+@dataclass
+class UnknownColType(ColType):
+    text: str
+
+    supported = False
+
+
+class AbstractDialect(ABC):
+    """Dialect-dependent query expressions"""
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        "Name of the dialect"
+
+    @classmethod
+    @abstractmethod
+    def load_mixins(cls, *abstract_mixins) -> Self:
+        "Load a list of mixins that implement the given abstract mixins"
+
+    @property
+    @abstractmethod
+    def ROUNDS_ON_PREC_LOSS(self) -> bool:
+        "True if db rounds real values when losing precision, False if it truncates."
+
+    @abstractmethod
+    def quote(self, s: str):
+        "Quote SQL name"
+
+    @abstractmethod
+    def concat(self, items: List[str]) -> str:
+        "Provide SQL for concatenating a bunch of columns into a string"
+
+    @abstractmethod
+    def is_distinct_from(self, a: str, b: str) -> str:
+        "Provide SQL for a comparison where NULL = NULL is true"
+
+    @abstractmethod
+    def to_string(self, s: str) -> str:
+        # TODO rewrite using cast_to(x, str)
+        "Provide SQL for casting a column to string"
+
+    @abstractmethod
+    def random(self) -> str:
+        "Provide SQL for generating a random number betweein 0..1"
+
+    @abstractmethod
+    def current_timestamp(self) -> str:
+        "Provide SQL for returning the current timestamp, aka now"
+
+    @abstractmethod
+    def offset_limit(self, offset: Optional[int] = None, limit: Optional[int] = None):
+        "Provide SQL fragment for limit and offset inside a select"
+
+    @abstractmethod
+    def explain_as_text(self, query: str) -> str:
+        "Provide SQL for explaining a query, returned as table(varchar)"
+
+    @abstractmethod
+    def timestamp_value(self, t: datetime) -> str:
+        "Provide SQL for the given timestamp value"
+
+    @abstractmethod
+    def set_timezone_to_utc(self) -> str:
+        "Provide SQL for setting the session timezone to UTC"
+
+    @abstractmethod
+    def parse_type(
+        self,
+        table_path: DbPath,
+        col_name: str,
+        type_repr: str,
+        datetime_precision: int = None,
+        numeric_precision: int = None,
+        numeric_scale: int = None,
+    ) -> ColType:
+        "Parse type info as returned by the database"
+
+
+T_Dialect = TypeVar("T_Dialect", bound=AbstractDialect)
+
+
+class AbstractDatabase(Generic[T_Dialect]):
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        "The name of the database"
+
+    @property
+    @abstractmethod
+    def dialect(self) -> T_Dialect:
+        "The dialect of the database. Used internally by Database, and also available publicly."
+
+    @classmethod
+    @abstractmethod
+    def load_mixins(cls, *abstract_mixins) -> type:
+        "Extend the dialect with a list of mixins that implement the given abstract mixins."
+
+    @property
+    @abstractmethod
+    def CONNECT_URI_HELP(self) -> str:
+        "Example URI to show the user in help and error messages"
+
+    @property
+    @abstractmethod
+    def CONNECT_URI_PARAMS(self) -> List[str]:
+        "List of parameters given in the path of the URI"
+
+    @abstractmethod
+    def _query(self, sql_code: Any) -> list:
+        "Send query to database and return result"
+
+    @abstractmethod
+    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
+        """Query the table for its schema for table in 'path', and return {column: tuple}
+        where the tuple is (table_name, col_name, type_repr, datetime_precision?, numeric_precision?, numeric_scale?)
+
+        Note: This method exists instead of select_table_schema(), just because not all databases support
+              accessing the schema using a SQL query.
+        """
+
+    @abstractmethod
+    def select_table_unique_columns(self, path: DbPath) -> str:
+        "Provide SQL for selecting the names of unique columns in the table"
+
+    @abstractmethod
+    def query_table_unique_columns(self, path: DbPath) -> List[str]:
+        """Query the table for its unique columns for table in 'path', and return {column}"""
+
+    @abstractmethod
+    def _process_table_schema(
+        self, path: DbPath, raw_schema: Dict[str, tuple], filter_columns: Sequence[str], where: str = None
+    ):
+        """Process the result of query_table_schema().
+
+        Done in a separate step, to minimize the amount of processed columns.
+        Needed because processing each column may:
+        * throw errors and warnings
+        * query the database to sample values
+
+        """
+
+    @abstractmethod
+    def parse_table_name(self, name: str) -> DbPath:
+        "Parse the given table name into a DbPath"
+
+    @abstractmethod
+    def close(self):
+        "Close connection(s) to the database instance. Querying will stop functioning."
+
+    @property
+    @abstractmethod
+    def is_autocommit(self) -> bool:
+        "Return whether the database autocommits changes. When false, COMMIT statements are skipped."
+
+
+class AbstractTable(ABC):
+    @abstractmethod
+    def select(self, *exprs, distinct=False, **named_exprs) -> "AbstractTable":
+        """Choose new columns, based on the old ones. (aka Projection)
+
+        Parameters:
+            exprs: List of expressions to constitute the columns of the new table.
+                    If not provided, returns all columns in source table (i.e. ``select *``)
+            distinct: 'select' or 'select distinct'
+            named_exprs: More expressions to constitute the columns of the new table, aliased to keyword name.
+
+        """
+        # XXX distinct=SKIP
+
+    @abstractmethod
+    def where(self, *exprs) -> "AbstractTable":
+        """Filter the rows, based on the given predicates. (aka Selection)"""
+
+    @abstractmethod
+    def order_by(self, *exprs) -> "AbstractTable":
+        """Order the rows lexicographically, according to the given expressions."""
+
+    @abstractmethod
+    def limit(self, limit: int) -> "AbstractTable":
+        """Stop yielding rows after the given limit. i.e. take the first 'n=limit' rows"""
+
+    @abstractmethod
+    def join(self, target) -> "AbstractTable":
+        """Join the current table with the target table, returning a new table containing both side-by-side.
+
+        When joining, it's recommended to use explicit tables names, instead of `this`,
+        in order to avoid potential name collisions.
+
+        Example:
+            ::
+
+                person = table('person')
+                city = table('city')
+
+                name_and_city = (
+                    person
+                    .join(city)
+                    .on(person['city_id'] == city['id'])
+                    .select(person['id'], city['name'])
+                )
+        """
+
+    @abstractmethod
+    def group_by(self, *keys):
+        """Behaves like in SQL, except for a small change in syntax:
+
+        A call to `.agg()` must follow every call to `.group_by()`.
+
+        Example:
+            ::
+
+                # SELECT a, sum(b) FROM tmp GROUP BY 1
+                table('tmp').group_by(this.a).agg(this.b.sum())
+
+                # SELECT a, sum(b) FROM a GROUP BY 1 HAVING (b > 10)
+                (table('tmp')
+                    .group_by(this.a)
+                    .agg(this.b.sum())
+                    .having(this.b > 10)
+                )
+
+        """
+
+    @abstractmethod
+    def count(self) -> int:
+        """SELECT count() FROM self"""
+
+    @abstractmethod
+    def union(self, other: "AbstractTable"):
+        """SELECT * FROM self UNION other"""
+
+    @abstractmethod
+    def union_all(self, other: "AbstractTable"):
+        """SELECT * FROM self UNION ALL other"""
+
+    @abstractmethod
+    def minus(self, other: "AbstractTable"):
+        """SELECT * FROM self EXCEPT other"""
+
+    @abstractmethod
+    def intersect(self, other: "AbstractTable"):
+        """SELECT * FROM self INTERSECT other"""
```

### Comparing `sqeleton-0.0.8/sqeleton/abcs/mixins.py` & `sqeleton-0.0.9/sqeleton/abcs/mixins.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,158 @@
-from abc import ABC, abstractmethod
-from .database_types import TemporalType, FractionalType, ColType_UUID, Boolean, ColType, String_UUID
-from .compiler import Compilable
-
-
-class AbstractMixin(ABC):
-    "A mixin for a database dialect"
-
-
-class AbstractMixin_NormalizeValue(AbstractMixin):
-    @abstractmethod
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        """Creates an SQL expression, that converts 'value' to a normalized timestamp.
-
-        The returned expression must accept any SQL datetime/timestamp, and return a string.
-
-        Date format: ``YYYY-MM-DD HH:mm:SS.FFFFFF``
-
-        Precision of dates should be rounded up/down according to coltype.rounds
-        """
-
-    @abstractmethod
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        """Creates an SQL expression, that converts 'value' to a normalized number.
-
-        The returned expression must accept any SQL int/numeric/float, and return a string.
-
-        Floats/Decimals are expected in the format
-        "I.P"
-
-        Where I is the integer part of the number (as many digits as necessary),
-        and must be at least one digit (0).
-        P is the fractional digits, the amount of which is specified with
-        coltype.precision. Trailing zeroes may be necessary.
-        If P is 0, the dot is omitted.
-
-        Note: We use 'precision' differently than most databases. For decimals,
-        it's the same as ``numeric_scale``, and for floats, who use binary precision,
-        it can be calculated as ``log10(2**numeric_precision)``.
-        """
-
-    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
-        """Creates an SQL expression, that converts 'value' to either '0' or '1'."""
-        return self.to_string(value)
-
-    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
-        """Creates an SQL expression, that strips uuids of artifacts like whitespace."""
-        if isinstance(coltype, String_UUID):
-            return f"TRIM({value})"
-        return self.to_string(value)
-
-    def normalize_value_by_type(self, value: str, coltype: ColType) -> str:
-        """Creates an SQL expression, that converts 'value' to a normalized representation.
-
-        The returned expression must accept any SQL value, and return a string.
-
-        The default implementation dispatches to a method according to `coltype`:
-
-        ::
-
-            TemporalType    -> normalize_timestamp()
-            FractionalType  -> normalize_number()
-            *else*          -> to_string()
-
-            (`Integer` falls in the *else* category)
-
-        """
-        if isinstance(coltype, TemporalType):
-            return self.normalize_timestamp(value, coltype)
-        elif isinstance(coltype, FractionalType):
-            return self.normalize_number(value, coltype)
-        elif isinstance(coltype, ColType_UUID):
-            return self.normalize_uuid(value, coltype)
-        elif isinstance(coltype, Boolean):
-            return self.normalize_boolean(value, coltype)
-        return self.to_string(value)
-
-
-class AbstractMixin_MD5(AbstractMixin):
-    """Methods for calculating an MD6 hash as an integer."""
-
-    @abstractmethod
-    def md5_as_int(self, s: str) -> str:
-        "Provide SQL for computing md5 and returning an int"
-
-
-class AbstractMixin_Schema(AbstractMixin):
-    """Methods for querying the database schema
-
-    TODO: Move AbstractDatabase.query_table_schema() and friends over here
-    """
-
-    def table_information(self) -> Compilable:
-        "Query to return a table of schema information about existing tables"
-        raise NotImplementedError()
-
-    @abstractmethod
-    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
-        """Query to select the list of tables in the schema. (query return type: table[str])
-
-        If 'like' is specified, the value is applied to the table name, using the 'like' operator.
-        """
-
-
-class AbstractMixin_Regex(AbstractMixin):
-    @abstractmethod
-    def test_regex(self, string: Compilable, pattern: Compilable) -> Compilable:
-        """Tests whether the regex pattern matches the string. Returns a bool expression."""
-
-
-class AbstractMixin_RandomSample(AbstractMixin):
-    @abstractmethod
-    def random_sample_n(self, tbl: str, size: int) -> str:
-        """Take a random sample of the given size, i.e. return 'size' amount of rows"""
-
-    @abstractmethod
-    def random_sample_ratio_approx(self, tbl: str, ratio: float) -> str:
-        """Take a random sample of the approximate size determined by the ratio (0..1), where 0 means no rows, and 1 means all rows
-
-        i.e. the actual mount of rows returned may vary by standard deviation.
-        """
-
-    # def random_sample_ratio(self, table: AbstractTable, ratio: float):
-    #     """Take a random sample of the size determined by the ratio (0..1), where 0 means no rows, and 1 means all rows
-    #     """
-
-
-class AbstractMixin_TimeTravel(AbstractMixin):
-    @abstractmethod
-    def time_travel(
-        self,
-        table: Compilable,
-        before: bool = False,
-        timestamp: Compilable = None,
-        offset: Compilable = None,
-        statement: Compilable = None,
-    ) -> Compilable:
-        """Selects historical data from a table
-
-        Parameters:
-            table - The name of the table whose history we're querying
-            timestamp - A constant timestamp
-            offset - the time 'offset' seconds before now
-            statement - identifier for statement, e.g. query ID
-
-        Must specify exactly one of `timestamp`, `offset` or `statement`.
-        """
-
-
-class AbstractMixin_OptimizerHints(AbstractMixin):
-    @abstractmethod
-    def optimizer_hints(self, optimizer_hints: str) -> str:
-        """Creates a compatible optimizer_hints string
-
-        Parameters:
-            optimizer_hints - string of optimizer hints
-        """
+from abc import ABC, abstractmethod
+from .database_types import TemporalType, FractionalType, ColType_UUID, Boolean, ColType, String_UUID
+from .compiler import Compilable
+
+
+class AbstractMixin(ABC):
+    "A mixin for a database dialect"
+
+
+class AbstractMixin_NormalizeValue(AbstractMixin):
+    @abstractmethod
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        """Creates an SQL expression, that converts 'value' to a normalized timestamp.
+
+        The returned expression must accept any SQL datetime/timestamp, and return a string.
+
+        Date format: ``YYYY-MM-DD HH:mm:SS.FFFFFF``
+
+        Precision of dates should be rounded up/down according to coltype.rounds
+        """
+
+    @abstractmethod
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        """Creates an SQL expression, that converts 'value' to a normalized number.
+
+        The returned expression must accept any SQL int/numeric/float, and return a string.
+
+        Floats/Decimals are expected in the format
+        "I.P"
+
+        Where I is the integer part of the number (as many digits as necessary),
+        and must be at least one digit (0).
+        P is the fractional digits, the amount of which is specified with
+        coltype.precision. Trailing zeroes may be necessary.
+        If P is 0, the dot is omitted.
+
+        Note: We use 'precision' differently than most databases. For decimals,
+        it's the same as ``numeric_scale``, and for floats, who use binary precision,
+        it can be calculated as ``log10(2**numeric_precision)``.
+        """
+
+    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
+        """Creates an SQL expression, that converts 'value' to either '0' or '1'."""
+        return self.to_string(value)
+
+    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
+        """Creates an SQL expression, that strips uuids of artifacts like whitespace."""
+        if isinstance(coltype, String_UUID):
+            return f"TRIM({value})"
+        return self.to_string(value)
+
+    def normalize_value_by_type(self, value: str, coltype: ColType) -> str:
+        """Creates an SQL expression, that converts 'value' to a normalized representation.
+
+        The returned expression must accept any SQL value, and return a string.
+
+        The default implementation dispatches to a method according to `coltype`:
+
+        ::
+
+            TemporalType    -> normalize_timestamp()
+            FractionalType  -> normalize_number()
+            *else*          -> to_string()
+
+            (`Integer` falls in the *else* category)
+
+        """
+        if isinstance(coltype, TemporalType):
+            return self.normalize_timestamp(value, coltype)
+        elif isinstance(coltype, FractionalType):
+            return self.normalize_number(value, coltype)
+        elif isinstance(coltype, ColType_UUID):
+            return self.normalize_uuid(value, coltype)
+        elif isinstance(coltype, Boolean):
+            return self.normalize_boolean(value, coltype)
+        return self.to_string(value)
+
+
+class AbstractMixin_MD5(AbstractMixin):
+    """Methods for calculating an MD6 hash as an integer."""
+
+    @abstractmethod
+    def md5_as_int(self, s: str) -> str:
+        "Provide SQL for computing md5 and returning an int"
+
+
+class AbstractMixin_Schema(AbstractMixin):
+    """Methods for querying the database schema
+
+    TODO: Move AbstractDatabase.query_table_schema() and friends over here
+    """
+
+    def table_information(self) -> Compilable:
+        "Query to return a table of schema information about existing tables"
+        raise NotImplementedError()
+
+    @abstractmethod
+    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
+        """Query to select the list of tables in the schema. (query return type: table[str])
+
+        If 'like' is specified, the value is applied to the table name, using the 'like' operator.
+        """
+
+
+class AbstractMixin_Regex(AbstractMixin):
+    @abstractmethod
+    def test_regex(self, string: Compilable, pattern: Compilable) -> Compilable:
+        """Tests whether the regex pattern matches the string. Returns a bool expression."""
+
+
+class AbstractMixin_RandomSample(AbstractMixin):
+    @abstractmethod
+    def random_sample_n(self, tbl: str, size: int) -> str:
+        """Take a random sample of the given size, i.e. return 'size' amount of rows"""
+
+    @abstractmethod
+    def random_sample_ratio_approx(self, tbl: str, ratio: float) -> str:
+        """Take a random sample of the approximate size determined by the ratio (0..1),
+        ratio of 0 means no rows, and 1 means all rows
+
+        i.e. the actual mount of rows returned may vary by standard deviation.
+        """
+
+    # def random_sample_ratio(self, table: AbstractTable, ratio: float):
+    #     """Take a random sample of the size determined by the ratio (0..1), where 0 means no rows, and 1 means all rows
+    #     """
+
+
+class AbstractMixin_TimeTravel(AbstractMixin):
+    @abstractmethod
+    def time_travel(
+        self,
+        table: Compilable,
+        before: bool = False,
+        timestamp: Compilable = None,
+        offset: Compilable = None,
+        statement: Compilable = None,
+    ) -> Compilable:
+        """Selects historical data from a table
+
+        Parameters:
+            table - The name of the table whose history we're querying
+            timestamp - A constant timestamp
+            offset - the time 'offset' seconds before now
+            statement - identifier for statement, e.g. query ID
+
+        Must specify exactly one of `timestamp`, `offset` or `statement`.
+        """
+
+
+class AbstractMixin_OptimizerHints(AbstractMixin):
+    @abstractmethod
+    def optimizer_hints(self, optimizer_hints: str) -> str:
+        """Creates a compatible optimizer_hints string
+
+        Parameters:
+            optimizer_hints - string of optimizer hints
+        """
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/__init__.py` & `sqeleton-0.0.9/sqeleton/databases/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .base import MD5_HEXDIGITS, CHECKSUM_HEXDIGITS, QueryError, ConnectError, BaseDialect, Database
-from ..abcs import DbPath, DbKey, DbTime
-from ._connect import Connect
-
-from .postgresql import PostgreSQL
-from .mysql import MySQL
-from .oracle import Oracle
-from .snowflake import Snowflake
-from .bigquery import BigQuery
-from .redshift import Redshift
-from .presto import Presto
-from .databricks import Databricks
-from .trino import Trino
-from .clickhouse import Clickhouse
-from .vertica import Vertica
-from .duckdb import DuckDB
-
-connect = Connect()
+from .base import MD5_HEXDIGITS, CHECKSUM_HEXDIGITS, QueryError, ConnectError, BaseDialect, Database, logger
+from ..abcs import DbPath, DbKey, DbTime
+from ._connect import Connect
+
+from .postgresql import PostgreSQL
+from .mysql import MySQL
+from .oracle import Oracle
+from .snowflake import Snowflake
+from .bigquery import BigQuery
+from .redshift import Redshift
+from .presto import Presto
+from .databricks import Databricks
+from .trino import Trino
+from .clickhouse import Clickhouse
+from .vertica import Vertica
+from .duckdb import DuckDB
+
+connect = Connect()
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/base.py` & `sqeleton-0.0.9/sqeleton/databases/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,596 +1,646 @@
-from datetime import datetime
-import math
-import sys
-import logging
-from typing import Any, Callable, Dict, Generator, Tuple, Optional, Sequence, Type, List, Union, TypeVar, TYPE_CHECKING
-from functools import partial, wraps
-from concurrent.futures import ThreadPoolExecutor
-import threading
-from abc import abstractmethod
-from uuid import UUID
-import decimal
-
-from runtype import dataclass
-
-from ..utils import is_uuid, safezip, Self
-from ..queries import Expr, Compiler, table, Select, SKIP, Explain, Code, this
-from ..queries.ast_classes import Random
-from ..abcs.database_types import (
-    AbstractDatabase,
-    T_Dialect,
-    AbstractDialect,
-    AbstractTable,
-    ColType,
-    Integer,
-    Decimal,
-    Float,
-    Native_UUID,
-    String_UUID,
-    String_Alphanum,
-    String_VaryingAlphanum,
-    TemporalType,
-    UnknownColType,
-    TimestampTZ,
-    Text,
-    DbTime,
-    DbPath,
-    Boolean,
-)
-from ..abcs.mixins import Compilable
-from ..abcs.mixins import (
-    AbstractMixin_Schema,
-    AbstractMixin_RandomSample,
-    AbstractMixin_NormalizeValue,
-    AbstractMixin_OptimizerHints,
-)
-from ..bound_exprs import bound_table
-
-logger = logging.getLogger("database")
-
-
-def parse_table_name(t):
-    return tuple(t.split("."))
-
-
-def import_helper(package: str = None, text=""):
-    def dec(f):
-        @wraps(f)
-        def _inner():
-            try:
-                return f()
-            except ModuleNotFoundError as e:
-                s = text
-                if package:
-                    s += f"You can install it using 'pip install sqeleton[{package}]'."
-                raise ModuleNotFoundError(f"{e}\n\n{s}\n")
-
-        return _inner
-
-    return dec
-
-
-class ConnectError(Exception):
-    pass
-
-
-class QueryError(Exception):
-    pass
-
-
-def _one(seq):
-    (x,) = seq
-    return x
-
-
-class ThreadLocalInterpreter:
-    """An interpeter used to execute a sequence of queries within the same thread and cursor.
-
-    Useful for cursor-sensitive operations, such as creating a temporary table.
-    """
-
-    def __init__(self, compiler: Compiler, gen: Generator):
-        self.gen = gen
-        self.compiler = compiler
-
-    def apply_queries(self, callback: Callable[[str], Any]):
-        q: Expr = next(self.gen)
-        while True:
-            sql = self.compiler.compile(q)
-            logger.debug("Running SQL (%s-TL): %s", self.compiler.database.name, sql)
-            try:
-                try:
-                    res = callback(sql) if sql is not SKIP else SKIP
-                except Exception as e:
-                    q = self.gen.throw(type(e), e)
-                else:
-                    q = self.gen.send(res)
-            except StopIteration:
-                break
-
-
-def apply_query(callback: Callable[[str], Any], sql_code: Union[str, ThreadLocalInterpreter]) -> list:
-    if isinstance(sql_code, ThreadLocalInterpreter):
-        return sql_code.apply_queries(callback)
-    else:
-        return callback(sql_code)
-
-
-class Mixin_Schema(AbstractMixin_Schema):
-    def table_information(self) -> Compilable:
-        return table("information_schema", "tables")
-
-    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
-        return (
-            self.table_information()
-            .where(
-                this.table_schema == table_schema,
-                this.table_name.like(like) if like is not None else SKIP,
-                this.table_type == "BASE TABLE",
-            )
-            .select(this.table_name)
-        )
-
-
-class Mixin_RandomSample(AbstractMixin_RandomSample):
-    def random_sample_n(self, tbl: AbstractTable, size: int) -> AbstractTable:
-        # TODO use a more efficient algorithm, when the table count is known
-        return tbl.order_by(Random()).limit(size)
-
-    def random_sample_ratio_approx(self, tbl: AbstractTable, ratio: float) -> AbstractTable:
-        return tbl.where(Random() < ratio)
-
-
-class Mixin_OptimizerHints(AbstractMixin_OptimizerHints):
-    def optimizer_hints(self, hints: str) -> str:
-        return f"/*+ {hints} */ "
-
-
-class BaseDialect(AbstractDialect):
-    SUPPORTS_PRIMARY_KEY = False
-    SUPPORTS_INDEXES = False
-    TYPE_CLASSES: Dict[str, type] = {}
-    MIXINS = frozenset()
-
-    PLACEHOLDER_TABLE = None  # Used for Oracle
-
-    def offset_limit(self, offset: Optional[int] = None, limit: Optional[int] = None):
-        if offset:
-            raise NotImplementedError("No support for OFFSET in query")
-
-        return f"LIMIT {limit}"
-
-    def concat(self, items: List[str]) -> str:
-        assert len(items) > 1
-        joined_exprs = ", ".join(items)
-        return f"concat({joined_exprs})"
-
-    def is_distinct_from(self, a: str, b: str) -> str:
-        return f"{a} is distinct from {b}"
-
-    def timestamp_value(self, t: DbTime) -> str:
-        return f"'{t.isoformat()}'"
-
-    def random(self) -> str:
-        return "random()"
-
-    def current_timestamp(self) -> str:
-        return "current_timestamp()"
-
-    def explain_as_text(self, query: str) -> str:
-        return f"EXPLAIN {query}"
-
-    def _constant_value(self, v):
-        if v is None:
-            return "NULL"
-        elif isinstance(v, str):
-            return f"'{v}'"
-        elif isinstance(v, datetime):
-            return self.timestamp_value(v)
-        elif isinstance(v, UUID):
-            return f"'{v}'"
-        elif isinstance(v, decimal.Decimal):
-            return str(v)
-        elif isinstance(v, bytearray):
-            return f"'{v.decode()}'"
-        elif isinstance(v, Code):
-            return v.code
-        return repr(v)
-
-    def constant_values(self, rows) -> str:
-        values = ", ".join("(%s)" % ", ".join(self._constant_value(v) for v in row) for row in rows)
-        return f"VALUES {values}"
-
-    def type_repr(self, t) -> str:
-        if isinstance(t, str):
-            return t
-        elif isinstance(t, TimestampTZ):
-            return f"TIMESTAMP({min(t.precision, DEFAULT_DATETIME_PRECISION)})"
-        return {
-            int: "INT",
-            str: "VARCHAR",
-            bool: "BOOLEAN",
-            float: "FLOAT",
-            datetime: "TIMESTAMP",
-        }[t]
-
-    def _parse_type_repr(self, type_repr: str) -> Optional[Type[ColType]]:
-        return self.TYPE_CLASSES.get(type_repr)
-
-    def parse_type(
-        self,
-        table_path: DbPath,
-        col_name: str,
-        type_repr: str,
-        datetime_precision: int = None,
-        numeric_precision: int = None,
-        numeric_scale: int = None,
-    ) -> ColType:
-        """ """
-
-        cls = self._parse_type_repr(type_repr)
-        if not cls:
-            return UnknownColType(type_repr)
-
-        if issubclass(cls, TemporalType):
-            return cls(
-                precision=datetime_precision if datetime_precision is not None else DEFAULT_DATETIME_PRECISION,
-                rounds=self.ROUNDS_ON_PREC_LOSS,
-            )
-
-        elif issubclass(cls, Integer):
-            return cls()
-
-        elif issubclass(cls, Boolean):
-            return cls()
-
-        elif issubclass(cls, Decimal):
-            if numeric_scale is None:
-                numeric_scale = 0  # Needed for Oracle.
-            return cls(precision=numeric_scale)
-
-        elif issubclass(cls, Float):
-            # assert numeric_scale is None
-            return cls(
-                precision=self._convert_db_precision_to_digits(
-                    numeric_precision if numeric_precision is not None else DEFAULT_NUMERIC_PRECISION
-                )
-            )
-
-        elif issubclass(cls, (Text, Native_UUID)):
-            return cls()
-
-        raise TypeError(f"Parsing {type_repr} returned an unknown type '{cls}'.")
-
-    def _convert_db_precision_to_digits(self, p: int) -> int:
-        """Convert from binary precision, used by floats, to decimal precision."""
-        # See: https://en.wikipedia.org/wiki/Single-precision_floating-point_format
-        return math.floor(math.log(2**p, 10))
-
-    @classmethod
-    def load_mixins(cls, *abstract_mixins) -> "Self":
-        mixins = {m for m in cls.MIXINS if issubclass(m, abstract_mixins)}
-
-        class _DialectWithMixins(cls, *mixins, *abstract_mixins):
-            pass
-
-        _DialectWithMixins.__name__ = cls.__name__
-        return _DialectWithMixins()
-
-
-T = TypeVar("T", bound=BaseDialect)
-
-
-@dataclass
-class QueryResult:
-    rows: list
-    columns: list = None
-
-    def __iter__(self):
-        return iter(self.rows)
-
-    def __len__(self):
-        return len(self.rows)
-
-    def __getitem__(self, i):
-        return self.rows[i]
-
-
-class Database(AbstractDatabase[T]):
-    """Base abstract class for databases.
-
-    Used for providing connection code and implementation specific SQL utilities.
-
-    Instanciated using :meth:`~sqeleton.connect`
-    """
-
-    default_schema: str = None
-    SUPPORTS_ALPHANUMS = True
-    SUPPORTS_UNIQUE_CONSTAINT = False
-
-    CONNECT_URI_KWPARAMS = []
-
-    _interactive = False
-    is_closed = False
-
-    @property
-    def name(self):
-        return type(self).__name__
-
-    def compile(self, sql_ast):
-        compiler = Compiler(self)
-        return compiler.compile(sql_ast)
-
-    def query(self, sql_ast: Union[Expr, Generator], res_type: type = None):
-        """Query the given SQL code/AST, and attempt to convert the result to type 'res_type'
-
-        If given a generator, it will execute all the yielded sql queries with the same thread and cursor.
-        The results of the queries a returned by the `yield` stmt (using the .send() mechanism).
-        It's a cleaner approach than exposing cursors, but may not be enough in all cases.
-        """
-
-        compiler = Compiler(self)
-        if isinstance(sql_ast, Generator):
-            sql_code = ThreadLocalInterpreter(compiler, sql_ast)
-        elif isinstance(sql_ast, list):
-            for i in sql_ast[:-1]:
-                self.query(i)
-            return self.query(sql_ast[-1], res_type)
-        else:
-            if isinstance(sql_ast, str):
-                sql_code = sql_ast
-            else:
-                if res_type is None:
-                    res_type = sql_ast.type
-                sql_code = compiler.compile(sql_ast)
-                if sql_code is SKIP:
-                    return SKIP
-
-            logger.debug("Running SQL (%s): %s", self.name, sql_code)
-
-        if self._interactive and isinstance(sql_ast, Select):
-            explained_sql = compiler.compile(Explain(sql_ast))
-            explain = self._query(explained_sql)
-            for row in explain:
-                # Most returned a 1-tuple. Presto returns a string
-                if isinstance(row, tuple):
-                    (row,) = row
-                logger.debug("EXPLAIN: %s", row)
-            answer = input("Continue? [y/n] ")
-            if answer.lower() not in ["y", "yes"]:
-                sys.exit(1)
-
-        res = self._query(sql_code)
-        if res_type is list:
-            return list(res)
-        elif res_type is int:
-            if not res:
-                raise ValueError("Query returned 0 rows, expected 1")
-            row = _one(res)
-            if not row:
-                raise ValueError("Row is empty, expected 1 column")
-            res = _one(row)
-            if res is None:  # May happen due to sum() of 0 items
-                return None
-            return int(res)
-        elif res_type is datetime:
-            res = _one(_one(res))
-            if isinstance(res, str):
-                res = datetime.fromisoformat(res[:23])  # TODO use a better parsing method
-            return res
-        elif res_type is tuple:
-            assert len(res) == 1, (sql_code, res)
-            return res[0]
-        elif getattr(res_type, "__origin__", None) is list and len(res_type.__args__) == 1:
-            if res_type.__args__ in ((int,), (str,)):
-                return [_one(row) for row in res]
-            elif res_type.__args__ in [(Tuple,), (tuple,)]:
-                return [tuple(row) for row in res]
-            elif res_type.__args__ == (dict,):
-                return [dict(safezip(res.columns, row)) for row in res]
-            else:
-                raise ValueError(res_type)
-        return res
-
-    def enable_interactive(self):
-        self._interactive = True
-
-    def select_table_schema(self, path: DbPath) -> str:
-        """Provide SQL for selecting the table schema as (name, type, date_prec, num_prec)"""
-        schema, name = self._normalize_table_path(path)
-
-        return (
-            "SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale "
-            "FROM information_schema.columns "
-            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
-        )
-
-    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
-        rows = self.query(self.select_table_schema(path), list)
-        if not rows:
-            raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
-
-        d = {r[0]: r for r in rows}
-        assert len(d) == len(rows)
-        return d
-
-    def select_table_unique_columns(self, path: DbPath) -> str:
-        schema, name = self._normalize_table_path(path)
-
-        return (
-            "SELECT column_name "
-            "FROM information_schema.key_column_usage "
-            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
-        )
-
-    def query_table_unique_columns(self, path: DbPath) -> List[str]:
-        if not self.SUPPORTS_UNIQUE_CONSTAINT:
-            raise NotImplementedError("This database doesn't support 'unique' constraints")
-        res = self.query(self.select_table_unique_columns(path), List[str])
-        return list(res)
-
-    def _process_table_schema(
-        self, path: DbPath, raw_schema: Dict[str, tuple], filter_columns: Sequence[str] = None, where: str = None
-    ):
-        if filter_columns is None:
-            filtered_schema = raw_schema
-        else:
-            accept = {i.lower() for i in filter_columns}
-            filtered_schema = {name: row for name, row in raw_schema.items() if name.lower() in accept}
-
-        col_dict = {row[0]: self.dialect.parse_type(path, *row) for _name, row in filtered_schema.items()}
-
-        self._refine_coltypes(path, col_dict, where)
-
-        # Return a dict of form {name: type} after normalization
-        return col_dict
-
-    def _refine_coltypes(self, table_path: DbPath, col_dict: Dict[str, ColType], where: str = None, sample_size=64):
-        """Refine the types in the column dict, by querying the database for a sample of their values
-
-        'where' restricts the rows to be sampled.
-        """
-
-        text_columns = [k for k, v in col_dict.items() if isinstance(v, Text)]
-        if not text_columns:
-            return
-
-        if isinstance(self.dialect, AbstractMixin_NormalizeValue):
-            fields = [Code(self.dialect.normalize_uuid(self.dialect.quote(c), String_UUID())) for c in text_columns]
-        else:
-            fields = this[text_columns]
-
-        samples_by_row = self.query(
-            table(*table_path).select(*fields).where(Code(where) if where else SKIP).limit(sample_size), list
-        )
-        if not samples_by_row:
-            raise ValueError(f"Table {table_path} is empty.")
-
-        samples_by_col = list(zip(*samples_by_row))
-
-        for col_name, samples in safezip(text_columns, samples_by_col):
-            uuid_samples = [s for s in samples if s and is_uuid(s)]
-
-            if uuid_samples:
-                if len(uuid_samples) != len(samples):
-                    logger.warning(
-                        f"Mixed UUID/Non-UUID values detected in column {'.'.join(table_path)}.{col_name}, disabling UUID support."
-                    )
-                else:
-                    assert col_name in col_dict
-                    col_dict[col_name] = String_UUID()
-                    continue
-
-            if self.SUPPORTS_ALPHANUMS:  # Anything but MySQL (so far)
-                alphanum_samples = [s for s in samples if String_Alphanum.test_value(s)]
-                if alphanum_samples:
-                    if len(alphanum_samples) != len(samples):
-                        logger.debug(
-                            f"Mixed Alphanum/Non-Alphanum values detected in column {'.'.join(table_path)}.{col_name}. It cannot be used as a key."
-                        )
-                    else:
-                        assert col_name in col_dict
-                        col_dict[col_name] = String_VaryingAlphanum()
-
-    # @lru_cache()
-    # def get_table_schema(self, path: DbPath) -> Dict[str, ColType]:
-    #     return self.query_table_schema(path)
-
-    def _normalize_table_path(self, path: DbPath) -> DbPath:
-        if len(path) == 1:
-            return self.default_schema, path[0]
-        elif len(path) == 2:
-            return path
-
-        raise ValueError(f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected form: schema.table")
-
-    def parse_table_name(self, name: str) -> DbPath:
-        return parse_table_name(name)
-
-    def _query_cursor(self, c, sql_code: str) -> QueryResult:
-        assert isinstance(sql_code, str), sql_code
-        try:
-            c.execute(sql_code)
-            if sql_code.lower().startswith(("select", "explain", "show")):
-                columns = [col[0] for col in c.description]
-                return QueryResult(c.fetchall(), columns)
-        except Exception as _e:
-            # logger.exception(e)
-            # logger.error(f'Caused by SQL: {sql_code}')
-            raise
-
-    def _query_conn(self, conn, sql_code: Union[str, ThreadLocalInterpreter]) -> QueryResult:
-        c = conn.cursor()
-        callback = partial(self._query_cursor, c)
-        return apply_query(callback, sql_code)
-
-    def close(self):
-        self.is_closed = True
-        return super().close()
-
-    def list_tables(self, tables_like, schema=None):
-        return self.query(self.dialect.list_tables(schema or self.default_schema, tables_like))
-
-    def table(self, *path, **kw):
-        return bound_table(self, path, **kw)
-
-    @classmethod
-    def load_mixins(cls, *abstract_mixins) -> type:
-        class _DatabaseWithMixins(cls):
-            dialect = cls.dialect.load_mixins(*abstract_mixins)
-
-        _DatabaseWithMixins.__name__ = cls.__name__
-        return _DatabaseWithMixins
-
-
-class ThreadedDatabase(Database):
-    """Access the database through singleton threads.
-
-    Used for database connectors that do not support sharing their connection between different threads.
-    """
-
-    def __init__(self, thread_count=1):
-        self._init_error = None
-        self._queue = ThreadPoolExecutor(thread_count, initializer=self.set_conn)
-        self.thread_local = threading.local()
-        logger.info(f"[{self.name}] Starting a threadpool, size={thread_count}.")
-
-    def set_conn(self):
-        assert not hasattr(self.thread_local, "conn")
-        try:
-            self.thread_local.conn = self.create_connection()
-        except Exception as e:
-            self._init_error = e
-
-    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]) -> QueryResult:
-        r = self._queue.submit(self._query_in_worker, sql_code)
-        return r.result()
-
-    def _query_in_worker(self, sql_code: Union[str, ThreadLocalInterpreter]):
-        "This method runs in a worker thread"
-        if self._init_error:
-            raise self._init_error
-        return self._query_conn(self.thread_local.conn, sql_code)
-
-    @abstractmethod
-    def create_connection(self):
-        "Return a connection instance, that supports the .cursor() method."
-
-    def close(self):
-        super().close()
-        self._queue.shutdown()
-
-    @property
-    def is_autocommit(self) -> bool:
-        return False
-
-
-CHECKSUM_HEXDIGITS = 15  # Must be 15 or lower, otherwise SUM() overflows
-MD5_HEXDIGITS = 32
-
-_CHECKSUM_BITSIZE = CHECKSUM_HEXDIGITS << 2
-CHECKSUM_MASK = (2**_CHECKSUM_BITSIZE) - 1
-
-DEFAULT_DATETIME_PRECISION = 6
-DEFAULT_NUMERIC_PRECISION = 24
-
-TIMESTAMP_PRECISION_POS = 20  # len("2022-06-03 12:24:35.") == 20
+from datetime import datetime
+import math
+import sys
+import logging
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    Tuple,
+    Optional,
+    Sequence,
+    List,
+    Union,
+    TypeVar,
+    Type,
+    overload
+)
+from functools import partial, wraps
+from concurrent.futures import ThreadPoolExecutor
+import threading
+from abc import abstractmethod
+
+from runtype import dataclass
+
+from sqeleton.queries.compiler import CompiledCode
+
+from ..utils import is_uuid, safezip, Self
+from ..queries import ExprNode, Compiler, table, Select, SKIP, T_SKIP, Explain, Code, this, commit
+from ..queries.ast_classes import ForeignKey, Random, CompilableNode, TablePath
+from ..abcs.database_types import (
+    AbstractDatabase,
+    AbstractDialect,
+    AbstractTable,
+    ColType,
+    Integer,
+    Decimal,
+    Float,
+    Native_UUID,
+    String_UUID,
+    String_Alphanum,
+    String_VaryingAlphanum,
+    TemporalType,
+    UnknownColType,
+    TimestampTZ,
+    Text,
+    DbTime,
+    DbPath,
+    Boolean,
+)
+from ..schema import Options
+from ..abcs.mixins import Compilable
+from ..abcs.mixins import (
+    AbstractMixin_Schema,
+    AbstractMixin_RandomSample,
+    AbstractMixin_NormalizeValue,
+    AbstractMixin_OptimizerHints,
+)
+from ..bound_exprs import bound_table
+
+logger = logging.getLogger("database")
+
+
+def parse_table_name(t):
+    return tuple(t.split("."))
+
+
+def import_helper(package: str = None, text=""):
+    def dec(f):
+        @wraps(f)
+        def _inner():
+            try:
+                return f()
+            except ModuleNotFoundError as e:
+                s = text
+                if package:
+                    s += f"You can install it using 'pip install sqeleton[{package}]'."
+                raise ModuleNotFoundError(f"{e}\n\n{s}\n")
+
+        return _inner
+
+    return dec
+
+
+class ConnectError(Exception):
+    pass
+
+
+class QueryError(Exception):
+    pass
+
+
+def _one(seq):
+    (x,) = seq
+    return x
+
+
+@dataclass
+class QueryResult:
+    rows: list
+    columns: list = None
+
+    def __iter__(self):
+        return iter(self.rows)
+
+    def __len__(self):
+        return len(self.rows)
+
+    def __getitem__(self, i):
+        return self.rows[i]
+
+
+class ThreadLocalInterpreter:
+    """An interpeter used to execute a sequence of queries within the same thread and cursor.
+
+    Useful for cursor-sensitive operations, such as creating a temporary table.
+    """
+
+    def __init__(self, compiler: Compiler, gen: Generator):
+        self.gen = gen
+        self.compiler = compiler
+
+    def apply_queries(self, callback: Callable[[CompiledCode], Any]) -> None:
+        q: ExprNode = next(self.gen)
+        while True:
+            sql = self.compiler.compile_with_args(q)
+            try:
+                try:
+                    res = callback(sql) if sql is not SKIP else SKIP
+                except Exception as e:
+                    q = self.gen.throw(type(e), e)
+                else:
+                    q = self.gen.send(res)
+            except StopIteration:
+                break
+
+SqlCode = Union[str, CompiledCode, ThreadLocalInterpreter]
+
+
+def apply_query(
+    callback: Callable[[CompiledCode], Any], sql_code: SqlCode
+) -> Optional[QueryResult]:
+    if isinstance(sql_code, ThreadLocalInterpreter):
+        return sql_code.apply_queries(callback)
+    elif isinstance(sql_code, str):
+        sql_code = CompiledCode(sql_code, [], None) # Unknown type. #TODO: Should we guess?
+
+    return callback(sql_code)
+
+
+class Mixin_Schema(AbstractMixin_Schema):
+    def table_information(self) -> TablePath:
+        return table("information_schema", "tables")
+
+    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
+        return (
+            self.table_information()
+            .where(
+                this.table_schema == table_schema,
+                this.table_name.like(like) if like is not None else SKIP,
+                this.table_type == "BASE TABLE",
+            )
+            .select(this.table_name)
+        )
+
+
+class Mixin_RandomSample(AbstractMixin_RandomSample):
+    def random_sample_n(self, tbl: AbstractTable, size: int) -> AbstractTable:
+        # TODO use a more efficient algorithm, when the table count is known
+        return tbl.order_by(Random()).limit(size)
+
+    def random_sample_ratio_approx(self, tbl: AbstractTable, ratio: float) -> AbstractTable:
+        return tbl.where(Random() < ratio)
+
+
+class Mixin_OptimizerHints(AbstractMixin_OptimizerHints):
+    def optimizer_hints(self, hints: str) -> str:
+        return f"/*+ {hints} */ "
+
+
+class BaseDialect(AbstractDialect):
+    SUPPORTS_PRIMARY_KEY = False
+    SUPPORTS_INDEXES = False
+    TYPE_CLASSES: Dict[str, type] = {}
+    MIXINS = frozenset()
+    ARG_SYMBOL = "%s"
+    PLACEHOLDER_TABLE = None  # Used for Oracle
+
+    def offset_limit(self, offset: Optional[int] = None, limit: Optional[int] = None):
+        if offset:
+            raise NotImplementedError("No support for OFFSET in query")
+
+        return f"LIMIT {limit}"
+
+    def concat(self, items: List[str]) -> str:
+        assert len(items) > 1
+        joined_exprs = ", ".join(items)
+        return f"concat({joined_exprs})"
+
+    def is_distinct_from(self, a: str, b: str) -> str:
+        return f"{a} is distinct from {b}"
+
+    def timestamp_value(self, t: DbTime) -> str:
+        return f"'{t.isoformat()}'"
+
+    def random(self) -> str:
+        return "random()"
+
+    def current_timestamp(self) -> str:
+        return "current_timestamp()"
+
+    def explain_as_text(self, query: str) -> str:
+        return f"EXPLAIN {query}"
+
+    def immediate_values(self, rows) -> str:
+        values = ", ".join("(%s)" % ", ".join(row) for row in rows)
+        return f"VALUES {values}"
+
+    def type_repr(self, t) -> str:
+        if isinstance(t, str):
+            return t
+        elif isinstance(t, TimestampTZ):
+            return f"TIMESTAMP({min(t.precision, DEFAULT_DATETIME_PRECISION)})"
+        elif isinstance(t, ForeignKey):
+            return self.type_repr(t.type)
+        return {
+            int: "INT",
+            str: "VARCHAR",
+            bytes: "BYTEA",
+            bool: "BOOLEAN",
+            float: "FLOAT",
+            datetime: "TIMESTAMP",
+        }[t]
+
+    # def decl_repr(self, name, type_):
+    #     if isinstance(type_, ForeignKey):
+    #         return f"FOREIGN KEY ({name}) REFERENCES Persons(PersonID)"
+
+    def _parse_type_repr(self, type_repr: str) -> Optional[Type[ColType]]:
+        return self.TYPE_CLASSES.get(type_repr)
+
+    def parse_type(
+        self,
+        table_path: DbPath,
+        col_name: str,
+        type_repr: str,
+        datetime_precision: int = None,
+        numeric_precision: int = None,
+        numeric_scale: int = None,
+    ) -> ColType:
+        """ """
+
+        cls = self._parse_type_repr(type_repr)
+        if not cls:
+            return UnknownColType(type_repr)
+
+        if issubclass(cls, TemporalType):
+            return cls(
+                precision=datetime_precision if datetime_precision is not None else DEFAULT_DATETIME_PRECISION,
+                rounds=self.ROUNDS_ON_PREC_LOSS,
+            )
+
+        elif issubclass(cls, Integer):
+            return cls()
+
+        elif issubclass(cls, Boolean):
+            return cls()
+
+        elif issubclass(cls, Decimal):
+            if numeric_scale is None:
+                numeric_scale = 0  # Needed for Oracle.
+            return cls(precision=numeric_scale)
+
+        elif issubclass(cls, Float):
+            # assert numeric_scale is None
+            return cls(
+                precision=self._convert_db_precision_to_digits(
+                    numeric_precision if numeric_precision is not None else DEFAULT_NUMERIC_PRECISION
+                )
+            )
+
+        elif issubclass(cls, (Text, Native_UUID)):
+            return cls()
+
+        raise TypeError(f"Parsing {type_repr} returned an unknown type '{cls}'.")
+
+    def _convert_db_precision_to_digits(self, p: int) -> int:
+        """Convert from binary precision, used by floats, to decimal precision."""
+        # See: https://en.wikipedia.org/wiki/Single-precision_floating-point_format
+        return math.floor(math.log(2**p, 10))
+
+    @classmethod
+    def load_mixins(cls, *abstract_mixins) -> "Self":
+        mixins = {m for m in cls.MIXINS if issubclass(m, abstract_mixins)}
+
+        class _DialectWithMixins(cls, *mixins, *abstract_mixins):
+            pass
+
+        _DialectWithMixins.__name__ = cls.__name__
+        return _DialectWithMixins()
+
+
+T = TypeVar("T", bound=BaseDialect)
+TRes = TypeVar("TRes")
+
+
+QueryInputItem = Union[CompilableNode, T_SKIP]
+QueryInput = Union[str, QueryInputItem, Generator, List[QueryInputItem]]
+
+class Database(AbstractDatabase[T]):
+    """Base abstract class for databases.
+
+    Used for providing connection code and implementation specific SQL utilities.
+
+    Instanciated using :meth:`~sqeleton.connect`
+    """
+
+    default_schema: str = None
+    SUPPORTS_ALPHANUMS = True
+    SUPPORTS_UNIQUE_CONSTAINT = False
+
+    CONNECT_URI_KWPARAMS = []
+
+    _interactive = False
+    is_closed = False
+
+    @property
+    def name(self):
+        return type(self).__name__
+
+    def compile(self, sql_ast):
+        compiler = Compiler(self)
+        return compiler.compile(sql_ast)
+
+    # def set_logger_level(self, level: Union[str, int]):
+    #     if isinstance(level, str):
+    #         level = getattr(logging, level)
+
+    #     logger.setLevel(level)
+
+    @overload
+    def query(self, query_input: QueryInput) -> Any:
+        ...
+
+    @overload
+    def query(self, query_input: QueryInput, res_type: None) -> Any:
+        ...
+
+    @overload
+    def query(self, query_input: QueryInput, res_type: Type[TRes]) -> TRes:
+        ...
+
+    def query(self, query_input, res_type = None):
+        """Query the given SQL code/AST, and attempt to convert the result to type 'res_type'
+
+        If given a generator:
+            It will execute all the yielded sql queries with the same thread and cursor.
+            The results of the queries are returned by the `yield` stmt (using the .send() mechanism).
+            It's a cleaner approach than exposing cursors, but may not be enough in all cases.
+        """
+        if query_input is SKIP:
+            return
+
+        compiler = Compiler(self)
+        if isinstance(query_input, Generator):
+            sql_code = ThreadLocalInterpreter(compiler, query_input)
+        elif isinstance(query_input, list):
+            for i in query_input[:-1]:
+                self.query(i)
+            return self.query(query_input[-1], res_type)
+        else:
+            if isinstance(query_input, str):
+                sql_code = query_input
+            else:
+                if res_type is None:
+                    res_type = query_input.type
+                sql_code = compiler.compile_with_args(query_input)
+                if sql_code is SKIP:
+                    return SKIP
+
+        if self._interactive and isinstance(query_input, Select):
+            explained_sql = compiler.compile_with_args(Explain(query_input))
+            explain = self._query(explained_sql)
+            for row in explain:
+                # Most returned a 1-tuple. Presto returns a string
+                if isinstance(row, tuple):
+                    (row,) = row
+                logger.debug("EXPLAIN: %s", row)
+            answer = input("Continue? [y/n] ")
+            if answer.lower() not in ["y", "yes"]:
+                sys.exit(1)
+
+        res = self._query(sql_code)
+        if res_type == None:
+            pass    # Do no casting
+        elif res is None:
+            assert res_type is not None
+            raise ValueError(f"Query returned NULL, but query() is expecting type {res_type}")
+        elif res_type is list:
+            return list(res)
+        elif res_type in (int, str):
+            if not res:
+                raise ValueError("Query returned 0 rows, expected 1")
+            row = _one(res)
+            if not row:
+                raise ValueError("Row is empty, expected 1 column")
+            res = _one(row)
+            if res is None:  # May happen due to sum() of 0 items
+                return None
+            return res_type(res)
+        elif res_type is datetime:
+            res = _one(_one(res))
+            if isinstance(res, str):
+                res = datetime.fromisoformat(res[:23])  # TODO use a better parsing method
+            return res
+        elif res_type is tuple:
+            assert len(res) == 1, (sql_code, res)
+            return res[0]
+        elif getattr(res_type, "__origin__", None) is list and len(res_type.__args__) == 1:
+            if res_type.__args__ in ((int,), (str,), (bytes,), (float,)):
+                return [_one(row) for row in res]
+            elif res_type.__args__ in [(Tuple,), (tuple,)]:
+                return [tuple(row) for row in res]
+            elif res_type.__args__ == (dict,):
+                return [dict(safezip(res.columns, row)) for row in res]
+            else:
+                (elem_type,) = res_type.__args__
+                return [elem_type(**dict(safezip(res.columns, row))) for row in res]
+                # raise ValueError(res_type)
+        else:
+            if len(res) == 0:
+                return None     # TODO: Only allow if res_type is Optional
+            assert len(res) == 1, len(res)
+            d = dict(safezip(res.columns, res[0]))
+            return res_type(**d)
+        return res
+
+    def enable_interactive(self):
+        self._interactive = True
+
+    def select_table_schema(self, path: DbPath) -> str:
+        """Provide SQL for selecting the table schema as (name, type, date_prec, num_prec)"""
+        schema, name = self._normalize_table_path(path)
+
+        return (
+            "SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale "
+            "FROM information_schema.columns "
+            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
+        )
+
+    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
+        rows = self.query(self.select_table_schema(path), list)
+        if not rows:
+            raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
+
+        d = {r[0]: r for r in rows}
+        assert len(d) == len(rows)
+        return d
+
+    def select_table_unique_columns(self, path: DbPath) -> str:
+        schema, name = self._normalize_table_path(path)
+
+        return (
+            "SELECT column_name "
+            "FROM information_schema.key_column_usage "
+            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
+        )
+
+    def query_table_unique_columns(self, path: DbPath) -> List[str]:
+        if not self.SUPPORTS_UNIQUE_CONSTAINT:
+            raise NotImplementedError("This database doesn't support 'unique' constraints")
+        res = self.query(self.select_table_unique_columns(path), List[str])
+        return list(res)
+
+    def _process_table_schema(
+        self, path: DbPath, raw_schema: Dict[str, tuple], filter_columns: Sequence[str] = None, where: str = None
+    ):
+        if filter_columns is None:
+            filtered_schema = raw_schema
+        else:
+            accept = {i.lower() for i in filter_columns}
+            filtered_schema = {name: row for name, row in raw_schema.items() if name.lower() in accept}
+
+        col_dict = {row[0]: self.dialect.parse_type(path, *row) for _name, row in filtered_schema.items()}
+
+        self._refine_coltypes(path, col_dict, where)
+
+        # Return a dict of form {name: type} after normalization
+        return col_dict
+
+    def _refine_coltypes(self, table_path: DbPath, col_dict: Dict[str, ColType], where: str = None, sample_size=64):
+        """Refine the types in the column dict, by querying the database for a sample of their values
+
+        'where' restricts the rows to be sampled.
+        """
+
+        text_columns = [k for k, v in col_dict.items() if isinstance(v, Text)]
+        if not text_columns:
+            return
+
+        if isinstance(self.dialect, AbstractMixin_NormalizeValue):
+            fields = [Code(self.dialect.normalize_uuid(self.dialect.quote(c), String_UUID())) for c in text_columns]
+        else:
+            fields = this[text_columns]
+
+        samples_by_row = self.query(
+            table(*table_path).select(*fields).where(Code(where) if where else SKIP).limit(sample_size), list
+        )
+        if not samples_by_row:
+            raise ValueError(f"Table {table_path} is empty.")
+
+        samples_by_col = list(zip(*samples_by_row))
+
+        for col_name, samples in safezip(text_columns, samples_by_col):
+            uuid_samples = [s for s in samples if s and is_uuid(s)]
+
+            if uuid_samples:
+                if len(uuid_samples) != len(samples):
+                    logger.warning(
+                        f"Mixed UUID/Non-UUID values detected in column {'.'.join(table_path)}.{col_name}, disabling UUID support."
+                    )
+                else:
+                    assert col_name in col_dict
+                    col_dict[col_name] = String_UUID()
+                    continue
+
+            if self.SUPPORTS_ALPHANUMS:  # Anything but MySQL (so far)
+                alphanum_samples = [s for s in samples if String_Alphanum.test_value(s)]
+                if alphanum_samples:
+                    if len(alphanum_samples) != len(samples):
+                        logger.debug(
+                            f"Mixed Alphanum/Non-Alphanum values detected in column {'.'.join(table_path)}.{col_name}. It cannot be used as a key."
+                        )
+                    else:
+                        assert col_name in col_dict
+                        col_dict[col_name] = String_VaryingAlphanum()
+
+    # @lru_cache()
+    # def get_table_schema(self, path: DbPath) -> Dict[str, ColType]:
+    #     return self.query_table_schema(path)
+
+    def _normalize_table_path(self, path: DbPath) -> DbPath:
+        if len(path) == 1:
+            return self.default_schema, path[0]
+        elif len(path) == 2:
+            return path
+
+        raise ValueError(f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected form: schema.table")
+
+    def parse_table_name(self, name: str) -> DbPath:
+        return parse_table_name(name)
+
+    def _query_cursor(self, c, sql_code: CompiledCode) -> Optional[QueryResult]:
+        assert isinstance(sql_code, CompiledCode), sql_code
+        try:
+            logger.debug(f"{self.name} Executing SQL: {sql_code.code} || {sql_code.args}")
+            c.execute(sql_code.code, sql_code.args)
+            # insert, delete and update may return values if they have the "returning" clause.
+            if sql_code.type is not None or sql_code.code.lstrip().lower().startswith(("select", "explain", "show", "with")):
+                columns = c.description and [col[0] for col in c.description]
+                return QueryResult(c.fetchall(), columns)
+        except Exception as _e:
+            # logger.exception(e)
+            # logger.error(f'Caused by SQL: {sql_code}')
+            raise
+
+    def _query_conn(self, conn, sql_code: SqlCode) -> Optional[QueryResult]:
+        c = conn.cursor()
+        callback = partial(self._query_cursor, c)
+        return apply_query(callback, sql_code)
+
+    def close(self):
+        self.is_closed = True
+        return super().close()
+
+    def list_tables(self, tables_like, schema=None):
+        self.dialect: Mixin_Schema
+        return self.query(self.dialect.list_tables(schema or self.default_schema, tables_like))
+
+    def table(self, *path, **kw):
+        return bound_table(self, path, **kw)
+
+    @classmethod
+    def load_mixins(cls, *abstract_mixins) -> type:
+        class _DatabaseWithMixins(cls):
+            dialect = cls.dialect.load_mixins(*abstract_mixins)
+
+        _DatabaseWithMixins.__name__ = cls.__name__
+        return _DatabaseWithMixins
+
+    def commit(self):
+        return self.query(commit)
+
+
+class ThreadedDatabase(Database):
+    """Access the database through singleton threads.
+
+    Used for database connectors that do not support sharing their connection between different threads.
+    """
+
+    def __init__(self, thread_count=1):
+        self._init_error = None
+        self._queue = ThreadPoolExecutor(thread_count, initializer=self.set_conn)
+        self.thread_local = threading.local()
+        logger.info(f"[{self.name}] Starting a threadpool, size={thread_count}.")
+
+    def set_conn(self):
+        assert not hasattr(self.thread_local, "conn")
+        try:
+            self.thread_local.conn = self.create_connection()
+        except Exception as e:
+            self._init_error = e
+
+    def _query(self, sql_code: SqlCode) -> QueryResult:
+        r = self._queue.submit(self._query_in_worker, sql_code)
+        return r.result()
+
+    def _query_in_worker(self, sql_code: SqlCode):
+        "This method runs in a worker thread"
+        if self._init_error:
+            raise self._init_error
+        return self._query_conn(self.thread_local.conn, sql_code)
+
+    @abstractmethod
+    def create_connection(self):
+        "Return a connection instance, that supports the .cursor() method."
+
+    def close(self):
+        super().close()
+        self._queue.shutdown()
+
+    @property
+    def is_autocommit(self) -> bool:
+        return False
+
+
+CHECKSUM_HEXDIGITS = 15  # Must be 15 or lower, otherwise SUM() overflows
+MD5_HEXDIGITS = 32
+
+_CHECKSUM_BITSIZE = CHECKSUM_HEXDIGITS << 2
+CHECKSUM_MASK = (2**_CHECKSUM_BITSIZE) - 1
+
+DEFAULT_DATETIME_PRECISION = 6
+DEFAULT_NUMERIC_PRECISION = 24
+
+TIMESTAMP_PRECISION_POS = 20  # len("2022-06-03 12:24:35.") == 20
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/clickhouse.py` & `sqeleton-0.0.9/sqeleton/databases/clickhouse.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-from typing import Optional, Type
-
-from .base import (
-    MD5_HEXDIGITS,
-    CHECKSUM_HEXDIGITS,
-    TIMESTAMP_PRECISION_POS,
-    BaseDialect,
-    ThreadedDatabase,
-    import_helper,
-    ConnectError,
-    Mixin_RandomSample,
-)
-from ..abcs.database_types import (
-    ColType,
-    Decimal,
-    Float,
-    Integer,
-    FractionalType,
-    Native_UUID,
-    TemporalType,
-    Text,
-    Timestamp,
-    Boolean,
-)
-from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue
-
-# https://clickhouse.com/docs/en/operations/server-configuration-parameters/settings/#default-database
-DEFAULT_DATABASE = "default"
-
-
-@import_helper("clickhouse")
-def import_clickhouse():
-    import clickhouse_driver
-
-    return clickhouse_driver
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        substr_idx = 1 + MD5_HEXDIGITS - CHECKSUM_HEXDIGITS
-        return f"reinterpretAsUInt128(reverse(unhex(lowerUTF8(substr(hex(MD5({s})), {substr_idx})))))"
-
-
-class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        # If a decimal value has trailing zeros in a fractional part, when casting to string they are dropped.
-        # For example:
-        #   select toString(toDecimal128(1.10, 2));  -- the result is 1.1
-        #   select toString(toDecimal128(1.00, 2)); -- the result is 1
-        # So, we should use some custom approach to save these trailing zeros.
-        # To avoid it, we can add a small value like 0.000001 to prevent dropping of zeros from the end when casting.
-        # For examples above it looks like:
-        #   select toString(toDecimal128(1.10, 2 + 1) + toDecimal128(0.001, 3)); -- the result is 1.101
-        # After that, cut an extra symbol from the string, i.e. 1.101 -> 1.10
-        # So, the algorithm is:
-        # 1. Cast to decimal with precision + 1
-        # 2. Add a small value 10^(-precision-1)
-        # 3. Cast the result to string
-        # 4. Drop the extra digit from the string. To do that, we need to slice the string
-        #    with length = digits in an integer part + 1 (symbol of ".") + precision
-
-        if coltype.precision == 0:
-            return self.to_string(f"round({value})")
-
-        precision = coltype.precision
-        # TODO: too complex, is there better performance way?
-        value = f"""
-            if({value} >= 0, '', '-') || left(
-                toString(
-                    toDecimal128(
-                        round(abs({value}), {precision}),
-                        {precision} + 1
-                    )
-                    +
-                    toDecimal128(
-                        exp10(-{precision + 1}),
-                        {precision} + 1
-                    )
-                ),
-                toUInt8(
-                    greatest(
-                        floor(log10(abs({value}))) + 1,
-                        1
-                    )
-                ) + 1 + {precision}
-            )
-        """
-        return value
-
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        prec = coltype.precision
-        if coltype.rounds:
-            timestamp = f"toDateTime64(round(toUnixTimestamp64Micro(toDateTime64({value}, 6)) / 1000000, {prec}), 6)"
-            return self.to_string(timestamp)
-
-        fractional = f"toUnixTimestamp64Micro(toDateTime64({value}, {prec})) % 1000000"
-        fractional = f"lpad({self.to_string(fractional)}, 6, '0')"
-        value = f"formatDateTime({value}, '%Y-%m-%d %H:%M:%S') || '.' || {self.to_string(fractional)}"
-        return f"rpad({value}, {TIMESTAMP_PRECISION_POS + 6}, '0')"
-
-
-class Dialect(BaseDialect):
-    name = "Clickhouse"
-    ROUNDS_ON_PREC_LOSS = False
-    TYPE_CLASSES = {
-        "Int8": Integer,
-        "Int16": Integer,
-        "Int32": Integer,
-        "Int64": Integer,
-        "Int128": Integer,
-        "Int256": Integer,
-        "UInt8": Integer,
-        "UInt16": Integer,
-        "UInt32": Integer,
-        "UInt64": Integer,
-        "UInt128": Integer,
-        "UInt256": Integer,
-        "Float32": Float,
-        "Float64": Float,
-        "Decimal": Decimal,
-        "UUID": Native_UUID,
-        "String": Text,
-        "FixedString": Text,
-        "DateTime": Timestamp,
-        "DateTime64": Timestamp,
-        "Bool": Boolean,
-    }
-    MIXINS = {Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
-
-    def quote(self, s: str) -> str:
-        return f'"{s}"'
-
-    def to_string(self, s: str) -> str:
-        return f"toString({s})"
-
-    def _convert_db_precision_to_digits(self, p: int) -> int:
-        # Done the same as for PostgreSQL but need to rewrite in another way
-        # because it does not help for float with a big integer part.
-        return super()._convert_db_precision_to_digits(p) - 2
-
-    def _parse_type_repr(self, type_repr: str) -> Optional[Type[ColType]]:
-        nullable_prefix = "Nullable("
-        if type_repr.startswith(nullable_prefix):
-            type_repr = type_repr[len(nullable_prefix) :].rstrip(")")
-
-        if type_repr.startswith("Decimal"):
-            type_repr = "Decimal"
-        elif type_repr.startswith("FixedString"):
-            type_repr = "FixedString"
-        elif type_repr.startswith("DateTime64"):
-            type_repr = "DateTime64"
-
-        return self.TYPE_CLASSES.get(type_repr)
-
-    # def timestamp_value(self, t: DbTime) -> str:
-    #     # return f"'{t}'"
-    #     return f"'{str(t)[:19]}'"
-
-    def set_timezone_to_utc(self) -> str:
-        raise NotImplementedError()
-
-    def current_timestamp(self) -> str:
-        return "now()"
-
-
-class Clickhouse(ThreadedDatabase):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "clickhouse://<user>:<password>@<host>/<database>"
-    CONNECT_URI_PARAMS = ["database?"]
-
-    def __init__(self, *, thread_count: int, **kw):
-        super().__init__(thread_count=thread_count)
-
-        self._args = kw
-        # In Clickhouse database and schema are the same
-        self.default_schema = kw.get("database", DEFAULT_DATABASE)
-
-    def create_connection(self):
-        clickhouse = import_clickhouse()
-
-        class SingleConnection(clickhouse.dbapi.connection.Connection):
-            """Not thread-safe connection to Clickhouse"""
-
-            def cursor(self, cursor_factory=None):
-                if not len(self.cursors):
-                    _ = super().cursor()
-                return self.cursors[0]
-
-        try:
-            return SingleConnection(**self._args)
-        except clickhouse.OperationError as e:
-            raise ConnectError(*e.args) from e
-
-    @property
-    def is_autocommit(self) -> bool:
-        return True
+from typing import Optional, Type
+
+from .base import (
+    MD5_HEXDIGITS,
+    CHECKSUM_HEXDIGITS,
+    TIMESTAMP_PRECISION_POS,
+    BaseDialect,
+    ThreadedDatabase,
+    import_helper,
+    ConnectError,
+    Mixin_RandomSample,
+)
+from ..abcs.database_types import (
+    ColType,
+    Decimal,
+    Float,
+    Integer,
+    FractionalType,
+    Native_UUID,
+    TemporalType,
+    Text,
+    Timestamp,
+    Boolean,
+)
+from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue
+
+# https://clickhouse.com/docs/en/operations/server-configuration-parameters/settings/#default-database
+DEFAULT_DATABASE = "default"
+
+
+@import_helper("clickhouse")
+def import_clickhouse():
+    import clickhouse_driver
+
+    return clickhouse_driver
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        substr_idx = 1 + MD5_HEXDIGITS - CHECKSUM_HEXDIGITS
+        return f"reinterpretAsUInt128(reverse(unhex(lowerUTF8(substr(hex(MD5({s})), {substr_idx})))))"
+
+
+class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        # If a decimal value has trailing zeros in a fractional part, when casting to string they are dropped.
+        # For example:
+        #   select toString(toDecimal128(1.10, 2));  -- the result is 1.1
+        #   select toString(toDecimal128(1.00, 2)); -- the result is 1
+        # So, we should use some custom approach to save these trailing zeros.
+        # To avoid it, we can add a small value like 0.000001 to prevent dropping of zeros from the end when casting.
+        # For examples above it looks like:
+        #   select toString(toDecimal128(1.10, 2 + 1) + toDecimal128(0.001, 3)); -- the result is 1.101
+        # After that, cut an extra symbol from the string, i.e. 1.101 -> 1.10
+        # So, the algorithm is:
+        # 1. Cast to decimal with precision + 1
+        # 2. Add a small value 10^(-precision-1)
+        # 3. Cast the result to string
+        # 4. Drop the extra digit from the string. To do that, we need to slice the string
+        #    with length = digits in an integer part + 1 (symbol of ".") + precision
+
+        if coltype.precision == 0:
+            return self.to_string(f"round({value})")
+
+        precision = coltype.precision
+        # TODO: too complex, is there better performance way?
+        value = f"""
+            if({value} >= 0, '', '-') || left(
+                toString(
+                    toDecimal128(
+                        round(abs({value}), {precision}),
+                        {precision} + 1
+                    )
+                    +
+                    toDecimal128(
+                        exp10(-{precision + 1}),
+                        {precision} + 1
+                    )
+                ),
+                toUInt8(
+                    greatest(
+                        floor(log10(abs({value}))) + 1,
+                        1
+                    )
+                ) + 1 + {precision}
+            )
+        """
+        return value
+
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        prec = coltype.precision
+        if coltype.rounds:
+            timestamp = f"toDateTime64(round(toUnixTimestamp64Micro(toDateTime64({value}, 6)) / 1000000, {prec}), 6)"
+            return self.to_string(timestamp)
+
+        fractional = f"toUnixTimestamp64Micro(toDateTime64({value}, {prec})) % 1000000"
+        fractional = f"lpad({self.to_string(fractional)}, 6, '0')"
+        value = f"formatDateTime({value}, '%Y-%m-%d %H:%M:%S') || '.' || {self.to_string(fractional)}"
+        return f"rpad({value}, {TIMESTAMP_PRECISION_POS + 6}, '0')"
+
+
+class Dialect(BaseDialect):
+    name = "Clickhouse"
+    ROUNDS_ON_PREC_LOSS = False
+    TYPE_CLASSES = {
+        "Int8": Integer,
+        "Int16": Integer,
+        "Int32": Integer,
+        "Int64": Integer,
+        "Int128": Integer,
+        "Int256": Integer,
+        "UInt8": Integer,
+        "UInt16": Integer,
+        "UInt32": Integer,
+        "UInt64": Integer,
+        "UInt128": Integer,
+        "UInt256": Integer,
+        "Float32": Float,
+        "Float64": Float,
+        "Decimal": Decimal,
+        "UUID": Native_UUID,
+        "String": Text,
+        "FixedString": Text,
+        "DateTime": Timestamp,
+        "DateTime64": Timestamp,
+        "Bool": Boolean,
+    }
+    MIXINS = {Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
+
+    def quote(self, s: str) -> str:
+        return f'"{s}"'
+
+    def to_string(self, s: str) -> str:
+        return f"toString({s})"
+
+    def _convert_db_precision_to_digits(self, p: int) -> int:
+        # Done the same as for PostgreSQL but need to rewrite in another way
+        # because it does not help for float with a big integer part.
+        return super()._convert_db_precision_to_digits(p) - 2
+
+    def _parse_type_repr(self, type_repr: str) -> Optional[Type[ColType]]:
+        nullable_prefix = "Nullable("
+        if type_repr.startswith(nullable_prefix):
+            type_repr = type_repr[len(nullable_prefix) :].rstrip(")")
+
+        if type_repr.startswith("Decimal"):
+            type_repr = "Decimal"
+        elif type_repr.startswith("FixedString"):
+            type_repr = "FixedString"
+        elif type_repr.startswith("DateTime64"):
+            type_repr = "DateTime64"
+
+        return self.TYPE_CLASSES.get(type_repr)
+
+    # def timestamp_value(self, t: DbTime) -> str:
+    #     # return f"'{t}'"
+    #     return f"'{str(t)[:19]}'"
+
+    def set_timezone_to_utc(self) -> str:
+        raise NotImplementedError()
+
+    def current_timestamp(self) -> str:
+        return "now()"
+
+
+class Clickhouse(ThreadedDatabase):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "clickhouse://<user>:<password>@<host>/<database>"
+    CONNECT_URI_PARAMS = ["database?"]
+
+    def __init__(self, *, thread_count: int, **kw):
+        super().__init__(thread_count=thread_count)
+
+        self._args = kw
+        # In Clickhouse database and schema are the same
+        self.default_schema = kw.get("database", DEFAULT_DATABASE)
+
+    def create_connection(self):
+        clickhouse = import_clickhouse()
+
+        class SingleConnection(clickhouse.dbapi.connection.Connection):
+            """Not thread-safe connection to Clickhouse"""
+
+            def cursor(self, cursor_factory=None):
+                if not len(self.cursors):
+                    _ = super().cursor()
+                return self.cursors[0]
+
+        try:
+            return SingleConnection(**self._args)
+        except clickhouse.OperationError as e:
+            raise ConnectError(*e.args) from e
+
+    @property
+    def is_autocommit(self) -> bool:
+        return True
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/databricks.py` & `sqeleton-0.0.9/sqeleton/databases/databricks.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-import math
-from typing import Dict, Sequence
-import logging
-
-from ..abcs.database_types import (
-    Integer,
-    Float,
-    Decimal,
-    Timestamp,
-    Text,
-    TemporalType,
-    NumericType,
-    DbPath,
-    ColType,
-    UnknownColType,
-    Boolean,
-)
-from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue
-from .base import (
-    MD5_HEXDIGITS,
-    CHECKSUM_HEXDIGITS,
-    BaseDialect,
-    ThreadedDatabase,
-    import_helper,
-    parse_table_name,
-    Mixin_RandomSample,
-)
-
-
-@import_helper(text="You can install it using 'pip install databricks-sql-connector'")
-def import_databricks():
-    import databricks.sql
-
-    return databricks
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        return f"cast(conv(substr(md5({s}), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS}), 16, 10) as decimal(38, 0))"
-
-
-class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        """Databricks timestamp contains no more than 6 digits in precision"""
-
-        if coltype.rounds:
-            timestamp = f"cast(round(unix_micros({value}) / 1000000, {coltype.precision}) * 1000000 as bigint)"
-            return f"date_format(timestamp_micros({timestamp}), 'yyyy-MM-dd HH:mm:ss.SSSSSS')"
-
-        precision_format = "S" * coltype.precision + "0" * (6 - coltype.precision)
-        return f"date_format({value}, 'yyyy-MM-dd HH:mm:ss.{precision_format}')"
-
-    def normalize_number(self, value: str, coltype: NumericType) -> str:
-        value = f"cast({value} as decimal(38, {coltype.precision}))"
-        if coltype.precision > 0:
-            value = f"format_number({value}, {coltype.precision})"
-        return f"replace({self.to_string(value)}, ',', '')"
-
-    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
-        return self.to_string(f"cast ({value} as int)")
-
-
-class Dialect(BaseDialect):
-    name = "Databricks"
-    ROUNDS_ON_PREC_LOSS = True
-    TYPE_CLASSES = {
-        # Numbers
-        "INT": Integer,
-        "SMALLINT": Integer,
-        "TINYINT": Integer,
-        "BIGINT": Integer,
-        "FLOAT": Float,
-        "DOUBLE": Float,
-        "DECIMAL": Decimal,
-        # Timestamps
-        "TIMESTAMP": Timestamp,
-        # Text
-        "STRING": Text,
-        # Boolean
-        "BOOLEAN": Boolean,
-    }
-    MIXINS = {Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
-
-    def quote(self, s: str):
-        return f"`{s}`"
-
-    def to_string(self, s: str) -> str:
-        return f"cast({s} as string)"
-
-    def _convert_db_precision_to_digits(self, p: int) -> int:
-        # Subtracting 2 due to wierd precision issues
-        return max(super()._convert_db_precision_to_digits(p) - 2, 0)
-
-    def set_timezone_to_utc(self) -> str:
-        return "SET TIME ZONE 'UTC'"
-
-
-class Databricks(ThreadedDatabase):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "databricks://:<access_token>@<server_hostname>/<http_path>"
-    CONNECT_URI_PARAMS = ["catalog", "schema"]
-
-    def __init__(self, *, thread_count, **kw):
-        logging.getLogger("databricks.sql").setLevel(logging.WARNING)
-
-        self._args = kw
-        self.default_schema = kw.get("schema", "default")
-        self.catalog = self._args.get("catalog", "hive_metastore")
-        super().__init__(thread_count=thread_count)
-
-    def create_connection(self):
-        databricks = import_databricks()
-
-        try:
-            return databricks.sql.connect(
-                server_hostname=self._args["server_hostname"],
-                http_path=self._args["http_path"],
-                access_token=self._args["access_token"],
-                catalog=self.catalog,
-            )
-        except databricks.sql.exc.Error as e:
-            raise ConnectionError(*e.args) from e
-
-    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
-        # Databricks has INFORMATION_SCHEMA only for Databricks Runtime, not for Databricks SQL.
-        # https://docs.databricks.com/spark/latest/spark-sql/language-manual/information-schema/columns.html
-        # So, to obtain information about schema, we should use another approach.
-
-        conn = self.create_connection()
-
-        catalog, schema, table = self._normalize_table_path(path)
-        with conn.cursor() as cursor:
-            cursor.columns(catalog_name=catalog, schema_name=schema, table_name=table)
-            try:
-                rows = cursor.fetchall()
-            finally:
-                conn.close()
-            if not rows:
-                raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
-
-            d = {r.COLUMN_NAME: (r.COLUMN_NAME, r.TYPE_NAME, r.DECIMAL_DIGITS, None, None) for r in rows}
-            assert len(d) == len(rows)
-            return d
-
-    def _process_table_schema(
-        self, path: DbPath, raw_schema: Dict[str, tuple], filter_columns: Sequence[str], where: str = None
-    ):
-        accept = {i.lower() for i in filter_columns}
-        rows = [row for name, row in raw_schema.items() if name.lower() in accept]
-
-        resulted_rows = []
-        for row in rows:
-            row_type = "DECIMAL" if row[1].startswith("DECIMAL") else row[1]
-            type_cls = self.dialect.TYPE_CLASSES.get(row_type, UnknownColType)
-
-            if issubclass(type_cls, Integer):
-                row = (row[0], row_type, None, None, 0)
-
-            elif issubclass(type_cls, Float):
-                numeric_precision = math.ceil(row[2] / math.log(2, 10))
-                row = (row[0], row_type, None, numeric_precision, None)
-
-            elif issubclass(type_cls, Decimal):
-                items = row[1][8:].rstrip(")").split(",")
-                numeric_precision, numeric_scale = int(items[0]), int(items[1])
-                row = (row[0], row_type, None, numeric_precision, numeric_scale)
-
-            elif issubclass(type_cls, Timestamp):
-                row = (row[0], row_type, row[2], None, None)
-
-            else:
-                row = (row[0], row_type, None, None, None)
-
-            resulted_rows.append(row)
-
-        col_dict: Dict[str, ColType] = {row[0]: self.dialect.parse_type(path, *row) for row in resulted_rows}
-
-        self._refine_coltypes(path, col_dict, where)
-        return col_dict
-
-    def parse_table_name(self, name: str) -> DbPath:
-        path = parse_table_name(name)
-        return tuple(i for i in self._normalize_table_path(path) if i is not None)
-
-    @property
-    def is_autocommit(self) -> bool:
-        return True
-
-    def _normalize_table_path(self, path: DbPath) -> DbPath:
-        if len(path) == 1:
-            return self.catalog, self.default_schema, path[0]
-        elif len(path) == 2:
-            return self.catalog, path[0], path[1]
-        elif len(path) == 3:
-            return path
-
-        raise ValueError(
-            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or catalog.schema.table"
-        )
+import math
+from typing import Dict, Sequence
+import logging
+
+from ..abcs.database_types import (
+    Integer,
+    Float,
+    Decimal,
+    Timestamp,
+    Text,
+    TemporalType,
+    NumericType,
+    DbPath,
+    ColType,
+    UnknownColType,
+    Boolean,
+)
+from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue
+from .base import (
+    MD5_HEXDIGITS,
+    CHECKSUM_HEXDIGITS,
+    BaseDialect,
+    ThreadedDatabase,
+    import_helper,
+    parse_table_name,
+    Mixin_RandomSample,
+)
+
+
+@import_helper(text="You can install it using 'pip install databricks-sql-connector'")
+def import_databricks():
+    import databricks.sql
+
+    return databricks
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        return f"cast(conv(substr(md5({s}), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS}), 16, 10) as decimal(38, 0))"
+
+
+class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        """Databricks timestamp contains no more than 6 digits in precision"""
+
+        if coltype.rounds:
+            timestamp = f"cast(round(unix_micros({value}) / 1000000, {coltype.precision}) * 1000000 as bigint)"
+            return f"date_format(timestamp_micros({timestamp}), 'yyyy-MM-dd HH:mm:ss.SSSSSS')"
+
+        precision_format = "S" * coltype.precision + "0" * (6 - coltype.precision)
+        return f"date_format({value}, 'yyyy-MM-dd HH:mm:ss.{precision_format}')"
+
+    def normalize_number(self, value: str, coltype: NumericType) -> str:
+        value = f"cast({value} as decimal(38, {coltype.precision}))"
+        if coltype.precision > 0:
+            value = f"format_number({value}, {coltype.precision})"
+        return f"replace({self.to_string(value)}, ',', '')"
+
+    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
+        return self.to_string(f"cast ({value} as int)")
+
+
+class Dialect(BaseDialect):
+    name = "Databricks"
+    ROUNDS_ON_PREC_LOSS = True
+    TYPE_CLASSES = {
+        # Numbers
+        "INT": Integer,
+        "SMALLINT": Integer,
+        "TINYINT": Integer,
+        "BIGINT": Integer,
+        "FLOAT": Float,
+        "DOUBLE": Float,
+        "DECIMAL": Decimal,
+        # Timestamps
+        "TIMESTAMP": Timestamp,
+        # Text
+        "STRING": Text,
+        # Boolean
+        "BOOLEAN": Boolean,
+    }
+    MIXINS = {Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
+
+    def quote(self, s: str):
+        return f"`{s}`"
+
+    def to_string(self, s: str) -> str:
+        return f"cast({s} as string)"
+
+    def _convert_db_precision_to_digits(self, p: int) -> int:
+        # Subtracting 2 due to wierd precision issues
+        return max(super()._convert_db_precision_to_digits(p) - 2, 0)
+
+    def set_timezone_to_utc(self) -> str:
+        return "SET TIME ZONE 'UTC'"
+
+
+class Databricks(ThreadedDatabase):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "databricks://:<access_token>@<server_hostname>/<http_path>"
+    CONNECT_URI_PARAMS = ["catalog", "schema"]
+
+    def __init__(self, *, thread_count, **kw):
+        logging.getLogger("databricks.sql").setLevel(logging.WARNING)
+
+        self._args = kw
+        self.default_schema = kw.get("schema", "default")
+        self.catalog = self._args.get("catalog", "hive_metastore")
+        super().__init__(thread_count=thread_count)
+
+    def create_connection(self):
+        databricks = import_databricks()
+
+        try:
+            return databricks.sql.connect(
+                server_hostname=self._args["server_hostname"],
+                http_path=self._args["http_path"],
+                access_token=self._args["access_token"],
+                catalog=self.catalog,
+            )
+        except databricks.sql.exc.Error as e:
+            raise ConnectionError(*e.args) from e
+
+    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
+        # Databricks has INFORMATION_SCHEMA only for Databricks Runtime, not for Databricks SQL.
+        # https://docs.databricks.com/spark/latest/spark-sql/language-manual/information-schema/columns.html
+        # So, to obtain information about schema, we should use another approach.
+
+        conn = self.create_connection()
+
+        catalog, schema, table = self._normalize_table_path(path)
+        with conn.cursor() as cursor:
+            cursor.columns(catalog_name=catalog, schema_name=schema, table_name=table)
+            try:
+                rows = cursor.fetchall()
+            finally:
+                conn.close()
+            if not rows:
+                raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
+
+            d = {r.COLUMN_NAME: (r.COLUMN_NAME, r.TYPE_NAME, r.DECIMAL_DIGITS, None, None) for r in rows}
+            assert len(d) == len(rows)
+            return d
+
+    def _process_table_schema(
+        self, path: DbPath, raw_schema: Dict[str, tuple], filter_columns: Sequence[str], where: str = None
+    ):
+        accept = {i.lower() for i in filter_columns}
+        rows = [row for name, row in raw_schema.items() if name.lower() in accept]
+
+        resulted_rows = []
+        for row in rows:
+            row_type = "DECIMAL" if row[1].startswith("DECIMAL") else row[1]
+            type_cls = self.dialect.TYPE_CLASSES.get(row_type, UnknownColType)
+
+            if issubclass(type_cls, Integer):
+                row = (row[0], row_type, None, None, 0)
+
+            elif issubclass(type_cls, Float):
+                numeric_precision = math.ceil(row[2] / math.log(2, 10))
+                row = (row[0], row_type, None, numeric_precision, None)
+
+            elif issubclass(type_cls, Decimal):
+                items = row[1][8:].rstrip(")").split(",")
+                numeric_precision, numeric_scale = int(items[0]), int(items[1])
+                row = (row[0], row_type, None, numeric_precision, numeric_scale)
+
+            elif issubclass(type_cls, Timestamp):
+                row = (row[0], row_type, row[2], None, None)
+
+            else:
+                row = (row[0], row_type, None, None, None)
+
+            resulted_rows.append(row)
+
+        col_dict: Dict[str, ColType] = {row[0]: self.dialect.parse_type(path, *row) for row in resulted_rows}
+
+        self._refine_coltypes(path, col_dict, where)
+        return col_dict
+
+    def parse_table_name(self, name: str) -> DbPath:
+        path = parse_table_name(name)
+        return tuple(i for i in self._normalize_table_path(path) if i is not None)
+
+    @property
+    def is_autocommit(self) -> bool:
+        return True
+
+    def _normalize_table_path(self, path: DbPath) -> DbPath:
+        if len(path) == 1:
+            return self.catalog, self.default_schema, path[0]
+        elif len(path) == 2:
+            return self.catalog, path[0], path[1]
+        elif len(path) == 3:
+            return path
+
+        raise ValueError(
+            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or catalog.schema.table"
+        )
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/duckdb.py` & `sqeleton-0.0.9/sqeleton/databases/duckdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,193 @@
-from typing import Union
-
-from ..utils import match_regexps
-from ..abcs.database_types import (
-    Timestamp,
-    TimestampTZ,
-    DbPath,
-    ColType,
-    Float,
-    Decimal,
-    Integer,
-    TemporalType,
-    Native_UUID,
-    Text,
-    FractionalType,
-    Boolean,
-    AbstractTable,
-)
-from ..abcs.mixins import (
-    AbstractMixin_MD5,
-    AbstractMixin_NormalizeValue,
-    AbstractMixin_RandomSample,
-    AbstractMixin_Regex,
-)
-from .base import (
-    Database,
-    BaseDialect,
-    import_helper,
-    ConnectError,
-    ThreadLocalInterpreter,
-    TIMESTAMP_PRECISION_POS,
-)
-from .base import MD5_HEXDIGITS, CHECKSUM_HEXDIGITS, Mixin_Schema
-from ..queries.ast_classes import Func, Compilable
-from ..queries.api import code
-
-
-@import_helper("duckdb")
-def import_duckdb():
-    import duckdb
-
-    return duckdb
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        return f"('0x' || SUBSTRING(md5({s}), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS},{CHECKSUM_HEXDIGITS}))::BIGINT"
-
-
-class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        # It's precision 6 by default. If precision is less than 6 -> we remove the trailing numbers.
-        if coltype.rounds and coltype.precision > 0:
-            return f"CONCAT(SUBSTRING(STRFTIME({value}::TIMESTAMP, '%Y-%m-%d %H:%M:%S.'),1,23), LPAD(((ROUND(strftime({value}::timestamp, '%f')::DECIMAL(15,7)/100000,{coltype.precision-1})*100000)::INT)::VARCHAR,6,'0'))"
-
-        return f"rpad(substring(strftime({value}::timestamp, '%Y-%m-%d %H:%M:%S.%f'),1,{TIMESTAMP_PRECISION_POS+coltype.precision}),26,'0')"
-
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        return self.to_string(f"{value}::DECIMAL(38, {coltype.precision})")
-
-    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
-        return self.to_string(f"{value}::INTEGER")
-
-
-class Mixin_RandomSample(AbstractMixin_RandomSample):
-    def random_sample_n(self, tbl: AbstractTable, size: int) -> AbstractTable:
-        return code("SELECT * FROM ({tbl}) USING SAMPLE {size};", tbl=tbl, size=size)
-
-    def random_sample_ratio_approx(self, tbl: AbstractTable, ratio: float) -> AbstractTable:
-        return code("SELECT * FROM ({tbl}) USING SAMPLE {percent}%;", tbl=tbl, percent=int(100 * ratio))
-
-
-class Mixin_Regex(AbstractMixin_Regex):
-    def test_regex(self, string: Compilable, pattern: Compilable) -> Compilable:
-        return Func("regexp_matches", [string, pattern])
-
-
-class Dialect(BaseDialect, Mixin_Schema):
-    name = "DuckDB"
-    ROUNDS_ON_PREC_LOSS = False
-    SUPPORTS_PRIMARY_KEY = True
-    SUPPORTS_INDEXES = True
-    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
-
-    TYPE_CLASSES = {
-        # Timestamps
-        "TIMESTAMP WITH TIME ZONE": TimestampTZ,
-        "TIMESTAMP": Timestamp,
-        # Numbers
-        "DOUBLE": Float,
-        "FLOAT": Float,
-        "DECIMAL": Decimal,
-        "INTEGER": Integer,
-        "BIGINT": Integer,
-        # Text
-        "VARCHAR": Text,
-        "TEXT": Text,
-        # UUID
-        "UUID": Native_UUID,
-        # Bool
-        "BOOLEAN": Boolean,
-    }
-
-    def quote(self, s: str):
-        return f'"{s}"'
-
-    def to_string(self, s: str):
-        return f"{s}::VARCHAR"
-
-    def _convert_db_precision_to_digits(self, p: int) -> int:
-        # Subtracting 2 due to wierd precision issues in PostgreSQL
-        return super()._convert_db_precision_to_digits(p) - 2
-
-    def parse_type(
-        self,
-        table_path: DbPath,
-        col_name: str,
-        type_repr: str,
-        datetime_precision: int = None,
-        numeric_precision: int = None,
-        numeric_scale: int = None,
-    ) -> ColType:
-        regexps = {
-            r"DECIMAL\((\d+),(\d+)\)": Decimal,
-        }
-
-        for m, t_cls in match_regexps(regexps, type_repr):
-            precision = int(m.group(2))
-            return t_cls(precision=precision)
-
-        return super().parse_type(table_path, col_name, type_repr, datetime_precision, numeric_precision, numeric_scale)
-
-    def set_timezone_to_utc(self) -> str:
-        return "SET GLOBAL TimeZone='UTC'"
-
-    def current_timestamp(self) -> str:
-        return "current_timestamp"
-
-
-class DuckDB(Database):
-    dialect = Dialect()
-    SUPPORTS_UNIQUE_CONSTAINT = False  # Temporary, until we implement it
-    default_schema = "main"
-    CONNECT_URI_HELP = "duckdb://<dbname>@<filepath>"
-    CONNECT_URI_PARAMS = ["database", "dbpath"]
-
-    def __init__(self, **kw):
-        self._args = kw
-        self._conn = self.create_connection()
-
-    @property
-    def is_autocommit(self) -> bool:
-        return True
-
-    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]):
-        "Uses the standard SQL cursor interface"
-        return self._query_conn(self._conn, sql_code)
-
-    def close(self):
-        super().close()
-        self._conn.close()
-
-    def create_connection(self):
-        ddb = import_duckdb()
-        try:
-            return ddb.connect(self._args["filepath"])
-        except ddb.OperationalError as e:
-            raise ConnectError(*e.args) from e
-
-    def select_table_schema(self, path: DbPath) -> str:
-        database, schema, table = self._normalize_table_path(path)
-
-        info_schema_path = ["information_schema", "columns"]
-        if database:
-            info_schema_path.insert(0, database)
-
-        return (
-            f"SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale FROM {'.'.join(info_schema_path)} "
-            f"WHERE table_name = '{table}' AND table_schema = '{schema}'"
-        )
-
-    def _normalize_table_path(self, path: DbPath) -> DbPath:
-        if len(path) == 1:
-            return None, self.default_schema, path[0]
-        elif len(path) == 2:
-            return None, path[0], path[1]
-        elif len(path) == 3:
-            return path
-
-        raise ValueError(
-            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
-        )
+from typing import Union
+
+from ..utils import match_regexps
+from ..abcs.database_types import (
+    Timestamp,
+    TimestampTZ,
+    DbPath,
+    ColType,
+    Float,
+    Decimal,
+    Integer,
+    TemporalType,
+    Native_UUID,
+    Text,
+    FractionalType,
+    Boolean,
+    AbstractTable,
+)
+from ..abcs.mixins import (
+    AbstractMixin_MD5,
+    AbstractMixin_NormalizeValue,
+    AbstractMixin_RandomSample,
+    AbstractMixin_Regex,
+)
+from .base import (
+    Database,
+    BaseDialect,
+    import_helper,
+    ConnectError,
+    ThreadLocalInterpreter,
+    TIMESTAMP_PRECISION_POS,
+)
+from .base import MD5_HEXDIGITS, CHECKSUM_HEXDIGITS, Mixin_Schema
+from ..queries.ast_classes import Func, Compilable
+from ..queries.api import code
+
+
+@import_helper("duckdb")
+def import_duckdb():
+    import duckdb
+
+    return duckdb
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        return f"('0x' || SUBSTRING(md5({s}), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS},{CHECKSUM_HEXDIGITS}))::BIGINT"
+
+
+class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        # It's precision 6 by default. If precision is less than 6 -> we remove the trailing numbers.
+        if coltype.rounds and coltype.precision > 0:
+            return f"CONCAT(SUBSTRING(STRFTIME({value}::TIMESTAMP, '%Y-%m-%d %H:%M:%S.'),1,23), LPAD(((ROUND(strftime({value}::timestamp, '%f')::DECIMAL(15,7)/100000,{coltype.precision-1})*100000)::INT)::VARCHAR,6,'0'))"
+
+        return f"rpad(substring(strftime({value}::timestamp, '%Y-%m-%d %H:%M:%S.%f'),1,{TIMESTAMP_PRECISION_POS+coltype.precision}),26,'0')"
+
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        return self.to_string(f"{value}::DECIMAL(38, {coltype.precision})")
+
+    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
+        return self.to_string(f"{value}::INTEGER")
+
+
+class Mixin_RandomSample(AbstractMixin_RandomSample):
+    def random_sample_n(self, tbl: AbstractTable, size: int) -> AbstractTable:
+        return code("SELECT * FROM ({tbl}) USING SAMPLE {size};", tbl=tbl, size=size)
+
+    def random_sample_ratio_approx(self, tbl: AbstractTable, ratio: float) -> AbstractTable:
+        return code("SELECT * FROM ({tbl}) USING SAMPLE {percent}%;", tbl=tbl, percent=int(100 * ratio))
+
+
+class Mixin_Regex(AbstractMixin_Regex):
+    def test_regex(self, string: Compilable, pattern: Compilable) -> Compilable:
+        return Func("regexp_matches", [string, pattern])
+
+
+class Dialect(BaseDialect, Mixin_Schema):
+    name = "DuckDB"
+    ROUNDS_ON_PREC_LOSS = False
+    SUPPORTS_PRIMARY_KEY = True
+    SUPPORTS_INDEXES = True
+    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
+    ARG_SYMBOL = "?"
+
+    TYPE_CLASSES = {
+        # Timestamps
+        "TIMESTAMP WITH TIME ZONE": TimestampTZ,
+        "TIMESTAMP": Timestamp,
+        # Numbers
+        "DOUBLE": Float,
+        "FLOAT": Float,
+        "DECIMAL": Decimal,
+        "INTEGER": Integer,
+        "BIGINT": Integer,
+        # Text
+        "VARCHAR": Text,
+        "TEXT": Text,
+        # UUID
+        "UUID": Native_UUID,
+        # Bool
+        "BOOLEAN": Boolean,
+    }
+
+    def quote(self, s: str):
+        return f'"{s}"'
+
+    def to_string(self, s: str):
+        return f"{s}::VARCHAR"
+
+    def _convert_db_precision_to_digits(self, p: int) -> int:
+        # Subtracting 2 due to wierd precision issues in PostgreSQL
+        return super()._convert_db_precision_to_digits(p) - 2
+
+    def parse_type(
+        self,
+        table_path: DbPath,
+        col_name: str,
+        type_repr: str,
+        datetime_precision: int = None,
+        numeric_precision: int = None,
+        numeric_scale: int = None,
+    ) -> ColType:
+        regexps = {
+            r"DECIMAL\((\d+),(\d+)\)": Decimal,
+        }
+
+        for m, t_cls in match_regexps(regexps, type_repr):
+            precision = int(m.group(2))
+            return t_cls(precision=precision)
+
+        return super().parse_type(table_path, col_name, type_repr, datetime_precision, numeric_precision, numeric_scale)
+
+    def set_timezone_to_utc(self) -> str:
+        return "SET GLOBAL TimeZone='UTC'"
+
+    def current_timestamp(self) -> str:
+        return "current_timestamp"
+
+
+class DuckDB(Database):
+    dialect = Dialect()
+    SUPPORTS_UNIQUE_CONSTAINT = False  # Temporary, until we implement it
+    default_schema = "main"
+    CONNECT_URI_HELP = "duckdb://<dbname>@<filepath>"
+    CONNECT_URI_PARAMS = ["database", "dbpath"]
+
+    def __init__(self, **kw):
+        self._args = kw
+        self._conn = self.create_connection()
+
+    @property
+    def is_autocommit(self) -> bool:
+        return True
+
+    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]):
+        "Uses the standard SQL cursor interface"
+        return self._query_conn(self._conn, sql_code)
+
+    def close(self):
+        super().close()
+        self._conn.close()
+
+    def create_connection(self):
+        ddb = import_duckdb()
+        try:
+            return ddb.connect(self._args["filepath"])
+        except ddb.OperationalError as e:
+            raise ConnectError(*e.args) from e
+
+    def select_table_schema(self, path: DbPath) -> str:
+        database, schema, table = self._normalize_table_path(path)
+
+        info_schema_path = ["information_schema", "columns"]
+        if database:
+            info_schema_path.insert(0, database)
+
+        return (
+            f"SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale FROM {'.'.join(info_schema_path)} "
+            f"WHERE table_name = '{table}' AND table_schema = '{schema}'"
+        )
+
+    def _normalize_table_path(self, path: DbPath) -> DbPath:
+        if len(path) == 1:
+            return None, self.default_schema, path[0]
+        elif len(path) == 2:
+            return None, path[0], path[1]
+        elif len(path) == 3:
+            return path
+
+        raise ValueError(
+            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
+        )
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/oracle.py` & `sqeleton-0.0.9/sqeleton/databases/oracle.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,203 +1,201 @@
-from typing import Dict, List, Optional
-
-from ..utils import match_regexps
-from ..abcs.database_types import (
-    Decimal,
-    Float,
-    Text,
-    DbPath,
-    TemporalType,
-    ColType,
-    DbTime,
-    ColType_UUID,
-    Timestamp,
-    TimestampTZ,
-    FractionalType,
-)
-from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue, AbstractMixin_Schema
-from ..abcs import Compilable
-from ..queries import this, table, SKIP
-from .base import (
-    BaseDialect,
-    Mixin_OptimizerHints,
-    ThreadedDatabase,
-    import_helper,
-    ConnectError,
-    QueryError,
-    Mixin_RandomSample,
-)
-from .base import TIMESTAMP_PRECISION_POS
-
-SESSION_TIME_ZONE = None  # Changed by the tests
-
-
-@import_helper("oracle")
-def import_oracle():
-    import cx_Oracle
-
-    return cx_Oracle
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        # standard_hash is faster than DBMS_CRYPTO.Hash
-        # TODO: Find a way to use UTL_RAW.CAST_TO_BINARY_INTEGER ?
-        return f"to_number(substr(standard_hash({s}, 'MD5'), 18), 'xxxxxxxxxxxxxxx')"
-
-
-class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
-        # Cast is necessary for correct MD5 (trimming not enough)
-        return f"CAST(TRIM({value}) AS VARCHAR(36))"
-
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        if coltype.rounds:
-            return f"to_char(cast({value} as timestamp({coltype.precision})), 'YYYY-MM-DD HH24:MI:SS.FF6')"
-
-        if coltype.precision > 0:
-            truncated = f"to_char({value}, 'YYYY-MM-DD HH24:MI:SS.FF{coltype.precision}')"
-        else:
-            truncated = f"to_char({value}, 'YYYY-MM-DD HH24:MI:SS.')"
-        return f"RPAD({truncated}, {TIMESTAMP_PRECISION_POS+6}, '0')"
-
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        # FM999.9990
-        format_str = "FM" + "9" * (38 - coltype.precision)
-        if coltype.precision:
-            format_str += "0." + "9" * (coltype.precision - 1) + "0"
-        return f"to_char({value}, '{format_str}')"
-
-
-class Mixin_Schema(AbstractMixin_Schema):
-    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
-        return (
-            table("ALL_TABLES")
-            .where(
-                this.OWNER == table_schema,
-                this.TABLE_NAME.like(like) if like is not None else SKIP,
-            )
-            .select(table_name=this.TABLE_NAME)
-        )
-
-
-class Dialect(BaseDialect, Mixin_Schema, Mixin_OptimizerHints):
-    name = "Oracle"
-    SUPPORTS_PRIMARY_KEY = True
-    SUPPORTS_INDEXES = True
-    TYPE_CLASSES: Dict[str, type] = {
-        "NUMBER": Decimal,
-        "FLOAT": Float,
-        # Text
-        "CHAR": Text,
-        "NCHAR": Text,
-        "NVARCHAR2": Text,
-        "VARCHAR2": Text,
-    }
-    ROUNDS_ON_PREC_LOSS = True
-    PLACEHOLDER_TABLE = "DUAL"
-    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
-
-    def quote(self, s: str):
-        return f'"{s}"'
-
-    def to_string(self, s: str):
-        return f"cast({s} as varchar(1024))"
-
-    def offset_limit(self, offset: Optional[int] = None, limit: Optional[int] = None):
-        if offset:
-            raise NotImplementedError("No support for OFFSET in query")
-
-        return f"FETCH NEXT {limit} ROWS ONLY"
-
-    def concat(self, items: List[str]) -> str:
-        joined_exprs = " || ".join(items)
-        return f"({joined_exprs})"
-
-    def timestamp_value(self, t: DbTime) -> str:
-        return "timestamp '%s'" % t.isoformat(" ")
-
-    def random(self) -> str:
-        return "dbms_random.value"
-
-    def is_distinct_from(self, a: str, b: str) -> str:
-        return f"DECODE({a}, {b}, 1, 0) = 0"
-
-    def type_repr(self, t) -> str:
-        try:
-            return {
-                str: "VARCHAR(1024)",
-            }[t]
-        except KeyError:
-            return super().type_repr(t)
-
-    def constant_values(self, rows) -> str:
-        return " UNION ALL ".join(
-            "SELECT %s FROM DUAL" % ", ".join(self._constant_value(v) for v in row) for row in rows
-        )
-
-    def explain_as_text(self, query: str) -> str:
-        raise NotImplementedError("Explain not yet implemented in Oracle")
-
-    def parse_type(
-        self,
-        table_path: DbPath,
-        col_name: str,
-        type_repr: str,
-        datetime_precision: int = None,
-        numeric_precision: int = None,
-        numeric_scale: int = None,
-    ) -> ColType:
-        regexps = {
-            r"TIMESTAMP\((\d)\) WITH LOCAL TIME ZONE": Timestamp,
-            r"TIMESTAMP\((\d)\) WITH TIME ZONE": TimestampTZ,
-            r"TIMESTAMP\((\d)\)": Timestamp,
-        }
-
-        for m, t_cls in match_regexps(regexps, type_repr):
-            precision = int(m.group(1))
-            return t_cls(precision=precision, rounds=self.ROUNDS_ON_PREC_LOSS)
-
-        return super().parse_type(table_path, col_name, type_repr, datetime_precision, numeric_precision, numeric_scale)
-
-    def set_timezone_to_utc(self) -> str:
-        return "ALTER SESSION SET TIME_ZONE = 'UTC'"
-
-    def current_timestamp(self) -> str:
-        return "LOCALTIMESTAMP"
-
-
-class Oracle(ThreadedDatabase):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "oracle://<user>:<password>@<host>/<database>"
-    CONNECT_URI_PARAMS = ["database?"]
-
-    def __init__(self, *, host, database, thread_count, **kw):
-        self.kwargs = dict(dsn=f"{host}/{database}" if database else host, **kw)
-
-        self.default_schema = kw.get("user").upper()
-
-        super().__init__(thread_count=thread_count)
-
-    def create_connection(self):
-        self._oracle = import_oracle()
-        try:
-            c = self._oracle.connect(**self.kwargs)
-            if SESSION_TIME_ZONE:
-                c.cursor().execute(f"ALTER SESSION SET TIME_ZONE = '{SESSION_TIME_ZONE}'")
-            return c
-        except Exception as e:
-            raise ConnectError(*e.args) from e
-
-    def _query_cursor(self, c, sql_code: str):
-        try:
-            return super()._query_cursor(c, sql_code)
-        except self._oracle.DatabaseError as e:
-            raise QueryError(e)
-
-    def select_table_schema(self, path: DbPath) -> str:
-        schema, name = self._normalize_table_path(path)
-
-        return (
-            f"SELECT column_name, data_type, 6 as datetime_precision, data_precision as numeric_precision, data_scale as numeric_scale"
-            f" FROM ALL_TAB_COLUMNS WHERE table_name = '{name}' AND owner = '{schema}'"
-        )
+from typing import Dict, List, Optional
+
+from ..utils import match_regexps
+from ..abcs.database_types import (
+    Decimal,
+    Float,
+    Text,
+    DbPath,
+    TemporalType,
+    ColType,
+    DbTime,
+    ColType_UUID,
+    Timestamp,
+    TimestampTZ,
+    FractionalType,
+)
+from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue, AbstractMixin_Schema
+from ..abcs import Compilable
+from ..queries import this, table, SKIP
+from .base import (
+    BaseDialect,
+    Mixin_OptimizerHints,
+    ThreadedDatabase,
+    import_helper,
+    ConnectError,
+    QueryError,
+    Mixin_RandomSample,
+)
+from .base import TIMESTAMP_PRECISION_POS
+
+SESSION_TIME_ZONE = None  # Changed by the tests
+
+
+@import_helper("oracle")
+def import_oracle():
+    import cx_Oracle
+
+    return cx_Oracle
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        # standard_hash is faster than DBMS_CRYPTO.Hash
+        # TODO: Find a way to use UTL_RAW.CAST_TO_BINARY_INTEGER ?
+        return f"to_number(substr(standard_hash({s}, 'MD5'), 18), 'xxxxxxxxxxxxxxx')"
+
+
+class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
+    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
+        # Cast is necessary for correct MD5 (trimming not enough)
+        return f"CAST(TRIM({value}) AS VARCHAR(36))"
+
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        if coltype.rounds:
+            return f"to_char(cast({value} as timestamp({coltype.precision})), 'YYYY-MM-DD HH24:MI:SS.FF6')"
+
+        if coltype.precision > 0:
+            truncated = f"to_char({value}, 'YYYY-MM-DD HH24:MI:SS.FF{coltype.precision}')"
+        else:
+            truncated = f"to_char({value}, 'YYYY-MM-DD HH24:MI:SS.')"
+        return f"RPAD({truncated}, {TIMESTAMP_PRECISION_POS+6}, '0')"
+
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        # FM999.9990
+        format_str = "FM" + "9" * (38 - coltype.precision)
+        if coltype.precision:
+            format_str += "0." + "9" * (coltype.precision - 1) + "0"
+        return f"to_char({value}, '{format_str}')"
+
+
+class Mixin_Schema(AbstractMixin_Schema):
+    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
+        return (
+            table("ALL_TABLES")
+            .where(
+                this.OWNER == table_schema,
+                this.TABLE_NAME.like(like) if like is not None else SKIP,
+            )
+            .select(table_name=this.TABLE_NAME)
+        )
+
+
+class Dialect(BaseDialect, Mixin_Schema, Mixin_OptimizerHints):
+    name = "Oracle"
+    SUPPORTS_PRIMARY_KEY = True
+    SUPPORTS_INDEXES = True
+    TYPE_CLASSES: Dict[str, type] = {
+        "NUMBER": Decimal,
+        "FLOAT": Float,
+        # Text
+        "CHAR": Text,
+        "NCHAR": Text,
+        "NVARCHAR2": Text,
+        "VARCHAR2": Text,
+    }
+    ROUNDS_ON_PREC_LOSS = True
+    PLACEHOLDER_TABLE = "DUAL"
+    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
+
+    def quote(self, s: str):
+        return f'"{s}"'
+
+    def to_string(self, s: str):
+        return f"cast({s} as varchar(1024))"
+
+    def offset_limit(self, offset: Optional[int] = None, limit: Optional[int] = None):
+        if offset:
+            raise NotImplementedError("No support for OFFSET in query")
+
+        return f"FETCH NEXT {limit} ROWS ONLY"
+
+    def concat(self, items: List[str]) -> str:
+        joined_exprs = " || ".join(items)
+        return f"({joined_exprs})"
+
+    def timestamp_value(self, t: DbTime) -> str:
+        return "timestamp '%s'" % t.isoformat(" ")
+
+    def random(self) -> str:
+        return "dbms_random.value"
+
+    def is_distinct_from(self, a: str, b: str) -> str:
+        return f"DECODE({a}, {b}, 1, 0) = 0"
+
+    def type_repr(self, t) -> str:
+        try:
+            return {
+                str: "VARCHAR(1024)",
+            }[t]
+        except KeyError:
+            return super().type_repr(t)
+
+    def constant_values(self, rows) -> str:
+        return " UNION ALL ".join("SELECT %s FROM DUAL" % ", ".join(row) for row in rows)
+
+    def explain_as_text(self, query: str) -> str:
+        raise NotImplementedError("Explain not yet implemented in Oracle")
+
+    def parse_type(
+        self,
+        table_path: DbPath,
+        col_name: str,
+        type_repr: str,
+        datetime_precision: int = None,
+        numeric_precision: int = None,
+        numeric_scale: int = None,
+    ) -> ColType:
+        regexps = {
+            r"TIMESTAMP\((\d)\) WITH LOCAL TIME ZONE": Timestamp,
+            r"TIMESTAMP\((\d)\) WITH TIME ZONE": TimestampTZ,
+            r"TIMESTAMP\((\d)\)": Timestamp,
+        }
+
+        for m, t_cls in match_regexps(regexps, type_repr):
+            precision = int(m.group(1))
+            return t_cls(precision=precision, rounds=self.ROUNDS_ON_PREC_LOSS)
+
+        return super().parse_type(table_path, col_name, type_repr, datetime_precision, numeric_precision, numeric_scale)
+
+    def set_timezone_to_utc(self) -> str:
+        return "ALTER SESSION SET TIME_ZONE = 'UTC'"
+
+    def current_timestamp(self) -> str:
+        return "LOCALTIMESTAMP"
+
+
+class Oracle(ThreadedDatabase):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "oracle://<user>:<password>@<host>/<database>"
+    CONNECT_URI_PARAMS = ["database?"]
+
+    def __init__(self, *, host, database, thread_count, **kw):
+        self.kwargs = dict(dsn=f"{host}/{database}" if database else host, **kw)
+
+        self.default_schema = kw.get("user").upper()
+
+        super().__init__(thread_count=thread_count)
+
+    def create_connection(self):
+        self._oracle = import_oracle()
+        try:
+            c = self._oracle.connect(**self.kwargs)
+            if SESSION_TIME_ZONE:
+                c.cursor().execute(f"ALTER SESSION SET TIME_ZONE = '{SESSION_TIME_ZONE}'")
+            return c
+        except Exception as e:
+            raise ConnectError(*e.args) from e
+
+    def _query_cursor(self, c, sql_code: str):
+        try:
+            return super()._query_cursor(c, sql_code)
+        except self._oracle.DatabaseError as e:
+            raise QueryError(e)
+
+    def select_table_schema(self, path: DbPath) -> str:
+        schema, name = self._normalize_table_path(path)
+
+        return (
+            f"SELECT column_name, data_type, 6 as datetime_precision, data_precision as numeric_precision, data_scale as numeric_scale"
+            f" FROM ALL_TAB_COLUMNS WHERE table_name = '{name}' AND owner = '{schema}'"
+        )
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/presto.py` & `sqeleton-0.0.9/sqeleton/databases/vertica.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,197 +1,181 @@
-from functools import partial
-import re
-
-from ..utils import match_regexps
-
-from ..abcs.database_types import (
-    Timestamp,
-    TimestampTZ,
-    Integer,
-    Float,
-    Text,
-    FractionalType,
-    DbPath,
-    DbTime,
-    Decimal,
-    ColType,
-    ColType_UUID,
-    TemporalType,
-    Boolean,
-)
-from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue
-from .base import BaseDialect, Database, import_helper, ThreadLocalInterpreter, Mixin_Schema, Mixin_RandomSample
-from .base import (
-    MD5_HEXDIGITS,
-    CHECKSUM_HEXDIGITS,
-    TIMESTAMP_PRECISION_POS,
-)
-
-
-def query_cursor(c, sql_code):
-    c.execute(sql_code)
-    if sql_code.lower().startswith("select"):
-        return c.fetchall()
-    # Required for the query to actually run 🤯
-    if re.match(r"(insert|create|truncate|drop|explain)", sql_code, re.IGNORECASE):
-        return c.fetchone()
-
-
-@import_helper("presto")
-def import_presto():
-    import prestodb
-
-    return prestodb
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        return f"cast(from_base(substr(to_hex(md5(to_utf8({s}))), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS}), 16) as decimal(38, 0))"
-
-
-class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
-        # Trim doesn't work on CHAR type
-        return f"TRIM(CAST({value} AS VARCHAR))"
-
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        # TODO rounds
-        if coltype.rounds:
-            s = f"date_format(cast({value} as timestamp(6)), '%Y-%m-%d %H:%i:%S.%f')"
-        else:
-            s = f"date_format(cast({value} as timestamp(6)), '%Y-%m-%d %H:%i:%S.%f')"
-
-        return f"RPAD(RPAD({s}, {TIMESTAMP_PRECISION_POS+coltype.precision}, '.'), {TIMESTAMP_PRECISION_POS+6}, '0')"
-
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        return self.to_string(f"cast({value} as decimal(38,{coltype.precision}))")
-
-    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
-        return self.to_string(f"cast ({value} as int)")
-
-
-class Dialect(BaseDialect, Mixin_Schema):
-    name = "Presto"
-    ROUNDS_ON_PREC_LOSS = True
-    TYPE_CLASSES = {
-        # Timestamps
-        "timestamp with time zone": TimestampTZ,
-        "timestamp without time zone": Timestamp,
-        "timestamp": Timestamp,
-        # Numbers
-        "integer": Integer,
-        "bigint": Integer,
-        "real": Float,
-        "double": Float,
-        # Text
-        "varchar": Text,
-        # Boolean
-        "boolean": Boolean,
-    }
-    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
-
-    def explain_as_text(self, query: str) -> str:
-        return f"EXPLAIN (FORMAT TEXT) {query}"
-
-    def type_repr(self, t) -> str:
-        try:
-            return {float: "REAL"}[t]
-        except KeyError:
-            return super().type_repr(t)
-
-    def timestamp_value(self, t: DbTime) -> str:
-        return f"timestamp '{t.isoformat(' ')}'"
-
-    def quote(self, s: str):
-        return f'"{s}"'
-
-    def to_string(self, s: str):
-        return f"cast({s} as varchar)"
-
-    def parse_type(
-        self,
-        table_path: DbPath,
-        col_name: str,
-        type_repr: str,
-        datetime_precision: int = None,
-        numeric_precision: int = None,
-        _numeric_scale: int = None,
-    ) -> ColType:
-        timestamp_regexps = {
-            r"timestamp\((\d)\)": Timestamp,
-            r"timestamp\((\d)\) with time zone": TimestampTZ,
-        }
-        for m, t_cls in match_regexps(timestamp_regexps, type_repr):
-            precision = int(m.group(1))
-            return t_cls(precision=precision, rounds=self.ROUNDS_ON_PREC_LOSS)
-
-        number_regexps = {r"decimal\((\d+),(\d+)\)": Decimal}
-        for m, n_cls in match_regexps(number_regexps, type_repr):
-            _prec, scale = map(int, m.groups())
-            return n_cls(scale)
-
-        string_regexps = {r"varchar\((\d+)\)": Text, r"char\((\d+)\)": Text}
-        for m, n_cls in match_regexps(string_regexps, type_repr):
-            return n_cls()
-
-        return super().parse_type(table_path, col_name, type_repr, datetime_precision, numeric_precision)
-
-    def set_timezone_to_utc(self) -> str:
-        return "SET TIME ZONE '+00:00'"
-
-    def current_timestamp(self) -> str:
-        return "current_timestamp"
-
-    def type_repr(self, t) -> str:
-        if isinstance(t, TimestampTZ):
-            return f"timestamp with time zone"
-        return super().type_repr(t)
-
-
-class Presto(Database):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "presto://<user>@<host>/<catalog>/<schema>"
-    CONNECT_URI_PARAMS = ["catalog", "schema"]
-
-    default_schema = "public"
-
-    def __init__(self, **kw):
-        prestodb = import_presto()
-
-        if kw.get("schema"):
-            self.default_schema = kw.get("schema")
-
-        if kw.get("auth") == "basic":  # if auth=basic, add basic authenticator for Presto
-            kw["auth"] = prestodb.auth.BasicAuthentication(kw.pop("user"), kw.pop("password"))
-
-        if "cert" in kw:  # if a certificate was specified in URI, verify session with cert
-            cert = kw.pop("cert")
-            self._conn = prestodb.dbapi.connect(**kw)
-            self._conn._http_session.verify = cert
-        else:
-            self._conn = prestodb.dbapi.connect(**kw)
-
-    def _query(self, sql_code: str) -> list:
-        "Uses the standard SQL cursor interface"
-        c = self._conn.cursor()
-
-        if isinstance(sql_code, ThreadLocalInterpreter):
-            return sql_code.apply_queries(partial(query_cursor, c))
-
-        return query_cursor(c, sql_code)
-
-    def close(self):
-        super().close()
-        self._conn.close()
-
-    def select_table_schema(self, path: DbPath) -> str:
-        schema, table = self._normalize_table_path(path)
-
-        return (
-            "SELECT column_name, data_type, 3 as datetime_precision, 3 as numeric_precision, NULL as numeric_scale "
-            "FROM INFORMATION_SCHEMA.COLUMNS "
-            f"WHERE table_name = '{table}' AND table_schema = '{schema}'"
-        )
-
-    @property
-    def is_autocommit(self) -> bool:
-        return False
+from typing import List
+
+from ..utils import match_regexps
+from .base import (
+    CHECKSUM_HEXDIGITS,
+    MD5_HEXDIGITS,
+    TIMESTAMP_PRECISION_POS,
+    BaseDialect,
+    ConnectError,
+    DbPath,
+    ColType,
+    ThreadedDatabase,
+    import_helper,
+    Mixin_RandomSample,
+)
+from ..abcs.database_types import (
+    Decimal,
+    Float,
+    FractionalType,
+    Integer,
+    TemporalType,
+    Text,
+    Timestamp,
+    TimestampTZ,
+    Boolean,
+    ColType_UUID,
+)
+from ..abcs.mixins import AbstractMixin_MD5, AbstractMixin_NormalizeValue, AbstractMixin_Schema
+from ..abcs import Compilable
+from ..queries import table, this, SKIP
+
+
+@import_helper("vertica")
+def import_vertica():
+    import vertica_python
+
+    return vertica_python
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        return f"CAST(HEX_TO_INTEGER(SUBSTRING(MD5({s}), {1 + MD5_HEXDIGITS - CHECKSUM_HEXDIGITS})) AS NUMERIC(38, 0))"
+
+
+class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        if coltype.rounds:
+            return f"TO_CHAR({value}::TIMESTAMP({coltype.precision}), 'YYYY-MM-DD HH24:MI:SS.US')"
+
+        timestamp6 = f"TO_CHAR({value}::TIMESTAMP(6), 'YYYY-MM-DD HH24:MI:SS.US')"
+        return (
+            f"RPAD(LEFT({timestamp6}, {TIMESTAMP_PRECISION_POS+coltype.precision}), {TIMESTAMP_PRECISION_POS+6}, '0')"
+        )
+
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        return self.to_string(f"CAST({value} AS NUMERIC(38, {coltype.precision}))")
+
+    def normalize_uuid(self, value: str, _coltype: ColType_UUID) -> str:
+        # Trim doesn't work on CHAR type
+        return f"TRIM(CAST({value} AS VARCHAR))"
+
+    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
+        return self.to_string(f"cast ({value} as int)")
+
+
+class Mixin_Schema(AbstractMixin_Schema):
+    def table_information(self) -> Compilable:
+        return table("v_catalog", "tables")
+
+    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
+        return (
+            self.table_information()
+            .where(
+                this.table_schema == table_schema,
+                this.table_name.like(like) if like is not None else SKIP,
+            )
+            .select(this.table_name)
+        )
+
+
+class Dialect(BaseDialect, Mixin_Schema):
+    name = "Vertica"
+    ROUNDS_ON_PREC_LOSS = True
+
+    TYPE_CLASSES = {
+        # Timestamps
+        "timestamp": Timestamp,
+        "timestamptz": TimestampTZ,
+        # Numbers
+        "numeric": Decimal,
+        "int": Integer,
+        "float": Float,
+        # Text
+        "char": Text,
+        "varchar": Text,
+        # Boolean
+        "boolean": Boolean,
+    }
+    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
+
+    def quote(self, s: str):
+        return f'"{s}"'
+
+    def concat(self, items: List[str]) -> str:
+        return " || ".join(items)
+
+    def to_string(self, s: str) -> str:
+        return f"CAST({s} AS VARCHAR)"
+
+    def is_distinct_from(self, a: str, b: str) -> str:
+        return f"not ({a} <=> {b})"
+
+    def parse_type(
+        self,
+        table_path: DbPath,
+        col_name: str,
+        type_repr: str,
+        datetime_precision: int = None,
+        numeric_precision: int = None,
+        numeric_scale: int = None,
+    ) -> ColType:
+        timestamp_regexps = {
+            r"timestamp\(?(\d?)\)?": Timestamp,
+            r"timestamptz\(?(\d?)\)?": TimestampTZ,
+        }
+        for m, t_cls in match_regexps(timestamp_regexps, type_repr):
+            precision = int(m.group(1)) if m.group(1) else 6
+            return t_cls(precision=precision, rounds=self.ROUNDS_ON_PREC_LOSS)
+
+        number_regexps = {
+            r"numeric\((\d+),(\d+)\)": Decimal,
+        }
+        for m, n_cls in match_regexps(number_regexps, type_repr):
+            _prec, scale = map(int, m.groups())
+            return n_cls(scale)
+
+        string_regexps = {
+            r"varchar\((\d+)\)": Text,
+            r"char\((\d+)\)": Text,
+        }
+        for m, n_cls in match_regexps(string_regexps, type_repr):
+            return n_cls()
+
+        return super().parse_type(table_path, col_name, type_repr, datetime_precision, numeric_precision)
+
+    def set_timezone_to_utc(self) -> str:
+        return "SET TIME ZONE TO 'UTC'"
+
+    def current_timestamp(self) -> str:
+        return "current_timestamp(6)"
+
+
+class Vertica(ThreadedDatabase):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "vertica://<user>:<password>@<host>/<database>"
+    CONNECT_URI_PARAMS = ["database?"]
+
+    default_schema = "public"
+
+    def __init__(self, *, thread_count, **kw):
+        self._args = kw
+        self._args["AUTOCOMMIT"] = False
+
+        super().__init__(thread_count=thread_count)
+
+    def create_connection(self):
+        vertica = import_vertica()
+        try:
+            c = vertica.connect(**self._args)
+            return c
+        except vertica.errors.ConnectionError as e:
+            raise ConnectError(*e.args) from e
+
+    def select_table_schema(self, path: DbPath) -> str:
+        schema, name = self._normalize_table_path(path)
+
+        return (
+            "SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale "
+            "FROM V_CATALOG.COLUMNS "
+            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/redshift.py` & `sqeleton-0.0.9/sqeleton/databases/redshift.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from typing import List, Dict
-from ..abcs.database_types import Float, TemporalType, FractionalType, DbPath, TimestampTZ
-from ..abcs.mixins import AbstractMixin_MD5
-from .postgresql import (
-    PostgreSQL,
-    MD5_HEXDIGITS,
-    CHECKSUM_HEXDIGITS,
-    TIMESTAMP_PRECISION_POS,
-    PostgresqlDialect,
-    Mixin_NormalizeValue,
-)
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        return f"strtol(substring(md5({s}), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS}), 16)::decimal(38)"
-
-
-class Mixin_NormalizeValue(Mixin_NormalizeValue):
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        if coltype.rounds:
-            timestamp = f"{value}::timestamp(6)"
-            # Get seconds since epoch. Redshift doesn't support milli- or micro-seconds.
-            secs = f"timestamp 'epoch' + round(extract(epoch from {timestamp})::decimal(38)"
-            # Get the milliseconds from timestamp.
-            ms = f"extract(ms from {timestamp})"
-            # Get the microseconds from timestamp, without the milliseconds!
-            us = f"extract(us from {timestamp})"
-            # epoch = Total time since epoch in microseconds.
-            epoch = f"{secs}*1000000 + {ms}*1000 + {us}"
-            timestamp6 = (
-                f"to_char({epoch}, -6+{coltype.precision}) * interval '0.000001 seconds', 'YYYY-mm-dd HH24:MI:SS.US')"
-            )
-        else:
-            timestamp6 = f"to_char({value}::timestamp(6), 'YYYY-mm-dd HH24:MI:SS.US')"
-        return (
-            f"RPAD(LEFT({timestamp6}, {TIMESTAMP_PRECISION_POS+coltype.precision}), {TIMESTAMP_PRECISION_POS+6}, '0')"
-        )
-
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        return self.to_string(f"{value}::decimal(38,{coltype.precision})")
-
-
-class Dialect(PostgresqlDialect):
-    name = "Redshift"
-    TYPE_CLASSES = {
-        **PostgresqlDialect.TYPE_CLASSES,
-        "double": Float,
-        "real": Float,
-    }
-    SUPPORTS_INDEXES = False
-
-    def concat(self, items: List[str]) -> str:
-        joined_exprs = " || ".join(items)
-        return f"({joined_exprs})"
-
-    def is_distinct_from(self, a: str, b: str) -> str:
-        return f"({a} IS NULL != {b} IS NULL) OR ({a}!={b})"
-
-    def type_repr(self, t) -> str:
-        if isinstance(t, TimestampTZ):
-            return f"timestamptz"
-        return super().type_repr(t)
-
-
-class Redshift(PostgreSQL):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "redshift://<user>:<password>@<host>/<database>"
-    CONNECT_URI_PARAMS = ["database?"]
-
-    def select_table_schema(self, path: DbPath) -> str:
-        database, schema, table = self._normalize_table_path(path)
-
-        info_schema_path = ["information_schema", "columns"]
-        if database:
-            info_schema_path.insert(0, database)
-
-        return (
-            f"SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale FROM {'.'.join(info_schema_path)} "
-            f"WHERE table_name = '{table.lower()}' AND table_schema = '{schema.lower()}'"
-        )
-
-    def select_external_table_schema(self, path: DbPath) -> str:
-        database, schema, table = self._normalize_table_path(path)
-
-        db_clause = ""
-        if database:
-            db_clause = f" AND redshift_database_name = '{database.lower()}'"
-
-        return (
-            f"""SELECT
-                columnname AS column_name
-                , CASE WHEN external_type = 'string' THEN 'varchar' ELSE external_type END AS data_type
-                , NULL AS datetime_precision
-                , NULL AS numeric_precision
-                , NULL AS numeric_scale
-            FROM svv_external_columns
-                WHERE tablename = '{table.lower()}' AND schemaname = '{schema.lower()}'
-            """
-            + db_clause
-        )
-
-    def query_external_table_schema(self, path: DbPath) -> Dict[str, tuple]:
-        rows = self.query(self.select_external_table_schema(path), list)
-        if not rows:
-            raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
-
-        d = {r[0]: r for r in rows}
-        assert len(d) == len(rows)
-        return d
-
-    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
-        try:
-            return super().query_table_schema(path)
-        except RuntimeError:
-            return self.query_external_table_schema(path)
-
-    def _normalize_table_path(self, path: DbPath) -> DbPath:
-        if len(path) == 1:
-            return None, self.default_schema, path[0]
-        elif len(path) == 2:
-            return None, path[0], path[1]
-        elif len(path) == 3:
-            return path
-
-        raise ValueError(
-            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
-        )
+from typing import List, Dict
+from ..abcs.database_types import Float, TemporalType, FractionalType, DbPath, TimestampTZ
+from ..abcs.mixins import AbstractMixin_MD5
+from .postgresql import (
+    PostgreSQL,
+    MD5_HEXDIGITS,
+    CHECKSUM_HEXDIGITS,
+    TIMESTAMP_PRECISION_POS,
+    PostgresqlDialect,
+    Mixin_NormalizeValue,
+)
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        return f"strtol(substring(md5({s}), {1+MD5_HEXDIGITS-CHECKSUM_HEXDIGITS}), 16)::decimal(38)"
+
+
+class Mixin_NormalizeValue(Mixin_NormalizeValue):
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        if coltype.rounds:
+            timestamp = f"{value}::timestamp(6)"
+            # Get seconds since epoch. Redshift doesn't support milli- or micro-seconds.
+            secs = f"timestamp 'epoch' + round(extract(epoch from {timestamp})::decimal(38)"
+            # Get the milliseconds from timestamp.
+            ms = f"extract(ms from {timestamp})"
+            # Get the microseconds from timestamp, without the milliseconds!
+            us = f"extract(us from {timestamp})"
+            # epoch = Total time since epoch in microseconds.
+            epoch = f"{secs}*1000000 + {ms}*1000 + {us}"
+            timestamp6 = (
+                f"to_char({epoch}, -6+{coltype.precision}) * interval '0.000001 seconds', 'YYYY-mm-dd HH24:MI:SS.US')"
+            )
+        else:
+            timestamp6 = f"to_char({value}::timestamp(6), 'YYYY-mm-dd HH24:MI:SS.US')"
+        return (
+            f"RPAD(LEFT({timestamp6}, {TIMESTAMP_PRECISION_POS+coltype.precision}), {TIMESTAMP_PRECISION_POS+6}, '0')"
+        )
+
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        return self.to_string(f"{value}::decimal(38,{coltype.precision})")
+
+
+class Dialect(PostgresqlDialect):
+    name = "Redshift"
+    TYPE_CLASSES = {
+        **PostgresqlDialect.TYPE_CLASSES,
+        "double": Float,
+        "real": Float,
+    }
+    SUPPORTS_INDEXES = False
+
+    def concat(self, items: List[str]) -> str:
+        joined_exprs = " || ".join(items)
+        return f"({joined_exprs})"
+
+    def is_distinct_from(self, a: str, b: str) -> str:
+        return f"({a} IS NULL != {b} IS NULL) OR ({a}!={b})"
+
+    def type_repr(self, t) -> str:
+        if isinstance(t, TimestampTZ):
+            return f"timestamptz"
+        return super().type_repr(t)
+
+
+class Redshift(PostgreSQL):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "redshift://<user>:<password>@<host>/<database>"
+    CONNECT_URI_PARAMS = ["database?"]
+
+    def select_table_schema(self, path: DbPath) -> str:
+        database, schema, table = self._normalize_table_path(path)
+
+        info_schema_path = ["information_schema", "columns"]
+        if database:
+            info_schema_path.insert(0, database)
+
+        return (
+            f"SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale FROM {'.'.join(info_schema_path)} "
+            f"WHERE table_name = '{table.lower()}' AND table_schema = '{schema.lower()}'"
+        )
+
+    def select_external_table_schema(self, path: DbPath) -> str:
+        database, schema, table = self._normalize_table_path(path)
+
+        db_clause = ""
+        if database:
+            db_clause = f" AND redshift_database_name = '{database.lower()}'"
+
+        return (
+            f"""SELECT
+                columnname AS column_name
+                , CASE WHEN external_type = 'string' THEN 'varchar' ELSE external_type END AS data_type
+                , NULL AS datetime_precision
+                , NULL AS numeric_precision
+                , NULL AS numeric_scale
+            FROM svv_external_columns
+                WHERE tablename = '{table.lower()}' AND schemaname = '{schema.lower()}'
+            """
+            + db_clause
+        )
+
+    def query_external_table_schema(self, path: DbPath) -> Dict[str, tuple]:
+        rows = self.query(self.select_external_table_schema(path), list)
+        if not rows:
+            raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
+
+        d = {r[0]: r for r in rows}
+        assert len(d) == len(rows)
+        return d
+
+    def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
+        try:
+            return super().query_table_schema(path)
+        except RuntimeError:
+            return self.query_external_table_schema(path)
+
+    def _normalize_table_path(self, path: DbPath) -> DbPath:
+        if len(path) == 1:
+            return None, self.default_schema, path[0]
+        elif len(path) == 2:
+            return None, path[0], path[1]
+        elif len(path) == 3:
+            return path
+
+        raise ValueError(
+            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
+        )
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/snowflake.py` & `sqeleton-0.0.9/sqeleton/databases/snowflake.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-from typing import Union, List
-import logging
-
-from ..abcs.database_types import (
-    Timestamp,
-    TimestampTZ,
-    Decimal,
-    Float,
-    Text,
-    FractionalType,
-    TemporalType,
-    DbPath,
-    Boolean,
-    Date,
-)
-from ..abcs.mixins import (
-    AbstractMixin_MD5,
-    AbstractMixin_NormalizeValue,
-    AbstractMixin_Schema,
-    AbstractMixin_TimeTravel,
-)
-from ..abcs import Compilable
-from sqeleton.queries import table, this, SKIP, code
-from .base import (
-    BaseDialect,
-    ConnectError,
-    Database,
-    import_helper,
-    CHECKSUM_MASK,
-    ThreadLocalInterpreter,
-    Mixin_RandomSample,
-)
-
-
-@import_helper("snowflake")
-def import_snowflake():
-    import snowflake.connector
-    from cryptography.hazmat.primitives import serialization
-    from cryptography.hazmat.backends import default_backend
-
-    return snowflake, serialization, default_backend
-
-
-class Mixin_MD5(AbstractMixin_MD5):
-    def md5_as_int(self, s: str) -> str:
-        return f"BITAND(md5_number_lower64({s}), {CHECKSUM_MASK})"
-
-
-class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        if coltype.rounds:
-            timestamp = f"to_timestamp(round(date_part(epoch_nanosecond, convert_timezone('UTC', {value})::timestamp(9))/1000000000, {coltype.precision}))"
-        else:
-            timestamp = f"cast(convert_timezone('UTC', {value}) as timestamp({coltype.precision}))"
-
-        return f"to_char({timestamp}, 'YYYY-MM-DD HH24:MI:SS.FF6')"
-
-    def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        return self.to_string(f"cast({value} as decimal(38, {coltype.precision}))")
-
-    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
-        return self.to_string(f"{value}::int")
-
-
-class Mixin_Schema(AbstractMixin_Schema):
-    def table_information(self) -> Compilable:
-        return table("INFORMATION_SCHEMA", "TABLES")
-
-    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
-        return (
-            self.table_information()
-            .where(
-                this.TABLE_SCHEMA == table_schema,
-                this.TABLE_NAME.like(like) if like is not None else SKIP,
-                this.TABLE_TYPE == "BASE TABLE",
-            )
-            .select(table_name=this.TABLE_NAME)
-        )
-
-
-class Mixin_TimeTravel(AbstractMixin_TimeTravel):
-    def time_travel(
-        self,
-        table: Compilable,
-        before: bool = False,
-        timestamp: Compilable = None,
-        offset: Compilable = None,
-        statement: Compilable = None,
-    ) -> Compilable:
-        at_or_before = "AT" if before else "BEFORE"
-        if timestamp is not None:
-            assert offset is None and statement is None
-            key = "timestamp"
-            value = timestamp
-        elif offset is not None:
-            assert statement is None
-            key = "offset"
-            value = offset
-        else:
-            assert statement is not None
-            key = "statement"
-            value = statement
-
-        return code(f"{{table}} {at_or_before}({key} => {{value}})", table=table, value=value)
-
-
-class Dialect(BaseDialect, Mixin_Schema):
-    name = "Snowflake"
-    ROUNDS_ON_PREC_LOSS = False
-    TYPE_CLASSES = {
-        # Timestamps
-        "TIMESTAMP_NTZ": Timestamp,
-        "TIMESTAMP_LTZ": Timestamp,
-        "TIMESTAMP_TZ": TimestampTZ,
-        "DATE": Date,
-        # Numbers
-        "NUMBER": Decimal,
-        "FLOAT": Float,
-        # Text
-        "TEXT": Text,
-        # Boolean
-        "BOOLEAN": Boolean,
-    }
-    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_TimeTravel, Mixin_RandomSample}
-
-    def explain_as_text(self, query: str) -> str:
-        return f"EXPLAIN USING TEXT {query}"
-
-    def quote(self, s: str):
-        return f'"{s}"'
-
-    def to_string(self, s: str):
-        return f"cast({s} as string)"
-
-    def table_information(self) -> Compilable:
-        return table("INFORMATION_SCHEMA", "TABLES")
-
-    def set_timezone_to_utc(self) -> str:
-        return "ALTER SESSION SET TIMEZONE = 'UTC'"
-
-    def optimizer_hints(self, hints: str) -> str:
-        raise NotImplementedError("Optimizer hints not yet implemented in snowflake")
-
-    def type_repr(self, t) -> str:
-        if isinstance(t, TimestampTZ):
-            return f"timestamp_tz({t.precision})"
-        return super().type_repr(t)
-
-
-class Snowflake(Database):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "snowflake://<user>:<password>@<account>/<database>/<SCHEMA>?warehouse=<WAREHOUSE>"
-    CONNECT_URI_PARAMS = ["database", "schema"]
-    CONNECT_URI_KWPARAMS = ["warehouse"]
-
-    def __init__(self, *, schema: str, **kw):
-        snowflake, serialization, default_backend = import_snowflake()
-        logging.getLogger("snowflake.connector").setLevel(logging.WARNING)
-
-        # Ignore the error: snowflake.connector.network.RetryRequest: could not find io module state
-        # It's a known issue: https://github.com/snowflakedb/snowflake-connector-python/issues/145
-        logging.getLogger("snowflake.connector.network").disabled = True
-
-        assert '"' not in schema, "Schema name should not contain quotes!"
-        # If a private key is used, read it from the specified path and pass it as "private_key" to the connector.
-        if "key" in kw:
-            with open(kw.get("key"), "rb") as key:
-                if "password" in kw:
-                    raise ConnectError("Cannot use password and key at the same time")
-                if kw.get("private_key_passphrase"):
-                    encoded_passphrase = kw.get("private_key_passphrase").encode()
-                else:
-                    encoded_passphrase = None
-                p_key = serialization.load_pem_private_key(
-                    key.read(),
-                    password=encoded_passphrase,
-                    backend=default_backend(),
-                )
-
-            kw["private_key"] = p_key.private_bytes(
-                encoding=serialization.Encoding.DER,
-                format=serialization.PrivateFormat.PKCS8,
-                encryption_algorithm=serialization.NoEncryption(),
-            )
-
-        self._conn = snowflake.connector.connect(schema=f'"{schema}"', **kw)
-
-        self.default_schema = schema
-
-    def close(self):
-        super().close()
-        self._conn.close()
-
-    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]):
-        "Uses the standard SQL cursor interface"
-        return self._query_conn(self._conn, sql_code)
-
-    def select_table_schema(self, path: DbPath) -> str:
-        """Provide SQL for selecting the table schema as (name, type, date_prec, num_prec)"""
-        database, schema, name = self._normalize_table_path(path)
-        info_schema_path = ["information_schema", "columns"]
-        if database:
-            info_schema_path.insert(0, database)
-
-        return (
-            "SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale "
-            f"FROM {'.'.join(info_schema_path)} "
-            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
-        )
-
-    def _normalize_table_path(self, path: DbPath) -> DbPath:
-        if len(path) == 1:
-            return None, self.default_schema, path[0]
-        elif len(path) == 2:
-            return None, path[0], path[1]
-        elif len(path) == 3:
-            return path
-
-        raise ValueError(
-            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
-        )
-
-    @property
-    def is_autocommit(self) -> bool:
-        return True
-
-    def query_table_unique_columns(self, path: DbPath) -> List[str]:
-        return []
+from typing import Union, List
+import logging
+
+from ..abcs.database_types import (
+    Timestamp,
+    TimestampTZ,
+    Decimal,
+    Float,
+    Text,
+    FractionalType,
+    TemporalType,
+    DbPath,
+    Boolean,
+    Date,
+)
+from ..abcs.mixins import (
+    AbstractMixin_MD5,
+    AbstractMixin_NormalizeValue,
+    AbstractMixin_Schema,
+    AbstractMixin_TimeTravel,
+)
+from ..abcs import Compilable
+from sqeleton.queries import table, this, SKIP, code
+from .base import (
+    BaseDialect,
+    ConnectError,
+    Database,
+    import_helper,
+    CHECKSUM_MASK,
+    ThreadLocalInterpreter,
+    Mixin_RandomSample,
+)
+
+
+@import_helper("snowflake")
+def import_snowflake():
+    import snowflake.connector
+    from cryptography.hazmat.primitives import serialization
+    from cryptography.hazmat.backends import default_backend
+
+    return snowflake, serialization, default_backend
+
+
+class Mixin_MD5(AbstractMixin_MD5):
+    def md5_as_int(self, s: str) -> str:
+        return f"BITAND(md5_number_lower64({s}), {CHECKSUM_MASK})"
+
+
+class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        if coltype.rounds:
+            timestamp = f"to_timestamp(round(date_part(epoch_nanosecond, convert_timezone('UTC', {value})::timestamp(9))/1000000000, {coltype.precision}))"
+        else:
+            timestamp = f"cast(convert_timezone('UTC', {value}) as timestamp({coltype.precision}))"
+
+        return f"to_char({timestamp}, 'YYYY-MM-DD HH24:MI:SS.FF6')"
+
+    def normalize_number(self, value: str, coltype: FractionalType) -> str:
+        return self.to_string(f"cast({value} as decimal(38, {coltype.precision}))")
+
+    def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
+        return self.to_string(f"{value}::int")
+
+
+class Mixin_Schema(AbstractMixin_Schema):
+    def table_information(self) -> Compilable:
+        return table("INFORMATION_SCHEMA", "TABLES")
+
+    def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
+        return (
+            self.table_information()
+            .where(
+                this.TABLE_SCHEMA == table_schema,
+                this.TABLE_NAME.like(like) if like is not None else SKIP,
+                this.TABLE_TYPE == "BASE TABLE",
+            )
+            .select(table_name=this.TABLE_NAME)
+        )
+
+
+class Mixin_TimeTravel(AbstractMixin_TimeTravel):
+    def time_travel(
+        self,
+        table: Compilable,
+        before: bool = False,
+        timestamp: Compilable = None,
+        offset: Compilable = None,
+        statement: Compilable = None,
+    ) -> Compilable:
+        at_or_before = "AT" if before else "BEFORE"
+        if timestamp is not None:
+            assert offset is None and statement is None
+            key = "timestamp"
+            value = timestamp
+        elif offset is not None:
+            assert statement is None
+            key = "offset"
+            value = offset
+        else:
+            assert statement is not None
+            key = "statement"
+            value = statement
+
+        return code(f"{{table}} {at_or_before}({key} => {{value}})", table=table, value=value)
+
+
+class Dialect(BaseDialect, Mixin_Schema):
+    name = "Snowflake"
+    ROUNDS_ON_PREC_LOSS = False
+    TYPE_CLASSES = {
+        # Timestamps
+        "TIMESTAMP_NTZ": Timestamp,
+        "TIMESTAMP_LTZ": Timestamp,
+        "TIMESTAMP_TZ": TimestampTZ,
+        "DATE": Date,
+        # Numbers
+        "NUMBER": Decimal,
+        "FLOAT": Float,
+        # Text
+        "TEXT": Text,
+        # Boolean
+        "BOOLEAN": Boolean,
+    }
+    MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_TimeTravel, Mixin_RandomSample}
+
+    def explain_as_text(self, query: str) -> str:
+        return f"EXPLAIN USING TEXT {query}"
+
+    def quote(self, s: str):
+        return f'"{s}"'
+
+    def to_string(self, s: str):
+        return f"cast({s} as string)"
+
+    def table_information(self) -> Compilable:
+        return table("INFORMATION_SCHEMA", "TABLES")
+
+    def set_timezone_to_utc(self) -> str:
+        return "ALTER SESSION SET TIMEZONE = 'UTC'"
+
+    def optimizer_hints(self, hints: str) -> str:
+        raise NotImplementedError("Optimizer hints not yet implemented in snowflake")
+
+    def type_repr(self, t) -> str:
+        if isinstance(t, TimestampTZ):
+            return f"timestamp_tz({t.precision})"
+        return super().type_repr(t)
+
+
+class Snowflake(Database):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "snowflake://<user>:<password>@<account>/<database>/<SCHEMA>?warehouse=<WAREHOUSE>"
+    CONNECT_URI_PARAMS = ["database", "schema"]
+    CONNECT_URI_KWPARAMS = ["warehouse"]
+
+    def __init__(self, *, schema: str, **kw):
+        snowflake, serialization, default_backend = import_snowflake()
+        logging.getLogger("snowflake.connector").setLevel(logging.WARNING)
+
+        # Ignore the error: snowflake.connector.network.RetryRequest: could not find io module state
+        # It's a known issue: https://github.com/snowflakedb/snowflake-connector-python/issues/145
+        logging.getLogger("snowflake.connector.network").disabled = True
+
+        assert '"' not in schema, "Schema name should not contain quotes!"
+        # If a private key is used, read it from the specified path and pass it as "private_key" to the connector.
+        if "key" in kw:
+            with open(kw.get("key"), "rb") as key:
+                if "password" in kw:
+                    raise ConnectError("Cannot use password and key at the same time")
+                if kw.get("private_key_passphrase"):
+                    encoded_passphrase = kw.get("private_key_passphrase").encode()
+                else:
+                    encoded_passphrase = None
+                p_key = serialization.load_pem_private_key(
+                    key.read(),
+                    password=encoded_passphrase,
+                    backend=default_backend(),
+                )
+
+            kw["private_key"] = p_key.private_bytes(
+                encoding=serialization.Encoding.DER,
+                format=serialization.PrivateFormat.PKCS8,
+                encryption_algorithm=serialization.NoEncryption(),
+            )
+
+        self._conn = snowflake.connector.connect(schema=f'"{schema}"', **kw)
+
+        self.default_schema = schema
+
+    def close(self):
+        super().close()
+        self._conn.close()
+
+    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]):
+        "Uses the standard SQL cursor interface"
+        return self._query_conn(self._conn, sql_code)
+
+    def select_table_schema(self, path: DbPath) -> str:
+        """Provide SQL for selecting the table schema as (name, type, date_prec, num_prec)"""
+        database, schema, name = self._normalize_table_path(path)
+        info_schema_path = ["information_schema", "columns"]
+        if database:
+            info_schema_path.insert(0, database)
+
+        return (
+            "SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale "
+            f"FROM {'.'.join(info_schema_path)} "
+            f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
+        )
+
+    def _normalize_table_path(self, path: DbPath) -> DbPath:
+        if len(path) == 1:
+            return None, self.default_schema, path[0]
+        elif len(path) == 2:
+            return None, path[0], path[1]
+        elif len(path) == 3:
+            return path
+
+        raise ValueError(
+            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
+        )
+
+    @property
+    def is_autocommit(self) -> bool:
+        return True
+
+    def query_table_unique_columns(self, path: DbPath) -> List[str]:
+        return []
```

### Comparing `sqeleton-0.0.8/sqeleton/databases/trino.py` & `sqeleton-0.0.9/sqeleton/databases/trino.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-from ..abcs.database_types import TemporalType, ColType_UUID
-from . import presto
-from .base import import_helper
-from .base import TIMESTAMP_PRECISION_POS
-
-
-@import_helper("trino")
-def import_trino():
-    import trino
-
-    return trino
-
-
-Mixin_MD5 = presto.Mixin_MD5
-
-
-class Mixin_NormalizeValue(presto.Mixin_NormalizeValue):
-    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
-        if coltype.rounds:
-            s = f"date_format(cast({value} as timestamp({coltype.precision})), '%Y-%m-%d %H:%i:%S.%f')"
-        else:
-            s = f"date_format(cast({value} as timestamp(6)), '%Y-%m-%d %H:%i:%S.%f')"
-
-        return (
-            f"RPAD(RPAD({s}, {TIMESTAMP_PRECISION_POS + coltype.precision}, '.'), {TIMESTAMP_PRECISION_POS + 6}, '0')"
-        )
-
-    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
-        return f"TRIM({value})"
-
-
-class Dialect(presto.Dialect):
-    name = "Trino"
-
-
-class Trino(presto.Presto):
-    dialect = Dialect()
-    CONNECT_URI_HELP = "trino://<user>@<host>/<catalog>/<schema>"
-    CONNECT_URI_PARAMS = ["catalog", "schema"]
-
-    def __init__(self, **kw):
-        trino = import_trino()
-
-        if kw.get("schema"):
-            self.default_schema = kw.get("schema")
-
-        self._conn = trino.dbapi.connect(**kw)
+from ..abcs.database_types import TemporalType, ColType_UUID
+from . import presto
+from .base import import_helper
+from .base import TIMESTAMP_PRECISION_POS
+
+
+@import_helper("trino")
+def import_trino():
+    import trino
+
+    return trino
+
+
+Mixin_MD5 = presto.Mixin_MD5
+
+
+class Mixin_NormalizeValue(presto.Mixin_NormalizeValue):
+    def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
+        if coltype.rounds:
+            s = f"date_format(cast({value} as timestamp({coltype.precision})), '%Y-%m-%d %H:%i:%S.%f')"
+        else:
+            s = f"date_format(cast({value} as timestamp(6)), '%Y-%m-%d %H:%i:%S.%f')"
+
+        return (
+            f"RPAD(RPAD({s}, {TIMESTAMP_PRECISION_POS + coltype.precision}, '.'), {TIMESTAMP_PRECISION_POS + 6}, '0')"
+        )
+
+    def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
+        return f"TRIM({value})"
+
+
+class Dialect(presto.Dialect):
+    name = "Trino"
+    ARG_SYMBOL = "?"
+
+
+class Trino(presto.Presto):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "trino://<user>@<host>/<catalog>/<schema>"
+    CONNECT_URI_PARAMS = ["catalog", "schema"]
+
+    def __init__(self, **kw):
+        trino = import_trino()
+
+        if kw.get("schema"):
+            self.default_schema = kw.get("schema")
+
+        self._conn = trino.dbapi.connect(**kw)
```

### Comparing `sqeleton-0.0.8/sqeleton/queries/ast_classes.py` & `sqeleton-0.0.9/sqeleton/queries/ast_classes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1028 +1,1393 @@
-from dataclasses import field
-from datetime import datetime
-from typing import Any, Generator, List, Optional, Sequence, Union, Dict
-
-from runtype import dataclass
-
-from ..utils import join_iter, ArithString
-from ..abcs import Compilable
-from ..abcs.database_types import AbstractTable
-from ..abcs.mixins import AbstractMixin_Regex, AbstractMixin_TimeTravel
-from ..schema import Schema
-
-from .compiler import Compiler, cv_params, Root, CompileError
-from .base import SKIP, DbPath, args_as_tuple, SqeletonError
-
-
-class QueryBuilderError(SqeletonError):
-    pass
-
-
-class QB_TypeError(QueryBuilderError):
-    pass
-
-
-class ExprNode(Compilable):
-    "Base class for query expression nodes"
-
-    type: Any = None
-
-    def _dfs_values(self):
-        yield self
-        for k, vs in dict(self).items():  # __dict__ provided by runtype.dataclass
-            if k == "source_table":
-                # Skip data-sources, we're only interested in data-parameters
-                continue
-            if not isinstance(vs, (list, tuple)):
-                vs = [vs]
-            for v in vs:
-                if isinstance(v, ExprNode):
-                    yield from v._dfs_values()
-
-    def cast_to(self, to):
-        return Cast(self, to)
-
-
-# Query expressions can only interact with objects that are an instance of 'Expr'
-Expr = Union[ExprNode, str, bool, int, float, datetime, ArithString, None]
-
-
-@dataclass
-class Code(ExprNode, Root):
-    code: str
-    args: Dict[str, Expr] = None
-
-    def compile(self, c: Compiler) -> str:
-        if not self.args:
-            return self.code
-
-        args = {k: c.compile(v) for k, v in self.args.items()}
-        return self.code.format(**args)
-
-
-def _expr_type(e: Expr) -> type:
-    if isinstance(e, ExprNode):
-        return e.type
-    return type(e)
-
-
-@dataclass
-class Alias(ExprNode):
-    expr: Expr
-    name: str
-
-    def compile(self, c: Compiler) -> str:
-        return f"{c.compile(self.expr)} AS {c.quote(self.name)}"
-
-    @property
-    def type(self):
-        return _expr_type(self.expr)
-
-
-def _drop_skips(exprs):
-    return [e for e in exprs if e is not SKIP]
-
-
-def _drop_skips_dict(exprs_dict):
-    return {k: v for k, v in exprs_dict.items() if v is not SKIP}
-
-
-class ITable(AbstractTable):
-    source_table: Any
-    schema: Schema = None
-
-    def select(self, *exprs, distinct=SKIP, optimizer_hints=SKIP, **named_exprs) -> "ITable":
-        """Create a new table with the specified fields"""
-        exprs = args_as_tuple(exprs)
-        exprs = _drop_skips(exprs)
-        named_exprs = _drop_skips_dict(named_exprs)
-        exprs += _named_exprs_as_aliases(named_exprs)
-        resolve_names(self.source_table, exprs)
-        return Select.make(self, columns=exprs, distinct=distinct, optimizer_hints=optimizer_hints)
-
-    def where(self, *exprs):
-        exprs = args_as_tuple(exprs)
-        exprs = _drop_skips(exprs)
-        if not exprs:
-            return self
-
-        resolve_names(self.source_table, exprs)
-        return Select.make(self, where_exprs=exprs)
-
-    def order_by(self, *exprs):
-        exprs = _drop_skips(exprs)
-        if not exprs:
-            return self
-
-        resolve_names(self.source_table, exprs)
-        return Select.make(self, order_by_exprs=exprs)
-
-    def limit(self, limit: int):
-        if limit is SKIP:
-            return self
-
-        return Select.make(self, limit_expr=limit)
-
-    def join(self, target: "ITable"):
-        """Join this table with the target table."""
-        return Join([self, target])
-
-    def group_by(self, *keys) -> "GroupBy":
-        """Group according to the given keys.
-
-        Must be followed by a call to :ref:``GroupBy.agg()``
-        """
-        keys = _drop_skips(keys)
-        resolve_names(self.source_table, keys)
-
-        return GroupBy(self, keys)
-
-    def _get_column(self, name: str):
-        if self.schema:
-            name = self.schema.get_key(name)  # Get the actual name. Might be case-insensitive.
-        return Column(self, name)
-
-    # def __getattr__(self, column):
-    #     return self._get_column(column)
-
-    def __getitem__(self, column):
-        if not isinstance(column, str):
-            raise TypeError()
-        return self._get_column(column)
-
-    def count(self):
-        return Select(self, [Count()])
-
-    def union(self, other: "ITable"):
-        """SELECT * FROM self UNION other"""
-        return TableOp("UNION", self, other)
-
-    def union_all(self, other: "ITable"):
-        """SELECT * FROM self UNION ALL other"""
-        return TableOp("UNION ALL", self, other)
-
-    def minus(self, other: "ITable"):
-        """SELECT * FROM self EXCEPT other"""
-        # aka
-        return TableOp("EXCEPT", self, other)
-
-    def intersect(self, other: "ITable"):
-        """SELECT * FROM self INTERSECT other"""
-        return TableOp("INTERSECT", self, other)
-
-
-@dataclass
-class Concat(ExprNode):
-    exprs: list
-    sep: str = None
-
-    def compile(self, c: Compiler) -> str:
-        # We coalesce because on some DBs (e.g. MySQL) concat('a', NULL) is NULL
-        items = [f"coalesce({c.compile(Code(c.dialect.to_string(c.compile(expr))))}, '<null>')" for expr in self.exprs]
-        assert items
-        if len(items) == 1:
-            return items[0]
-
-        if self.sep:
-            items = list(join_iter(f"'{self.sep}'", items))
-        return c.dialect.concat(items)
-
-
-@dataclass
-class Count(ExprNode):
-    expr: Expr = None
-    distinct: bool = False
-
-    type = int
-
-    def compile(self, c: Compiler) -> str:
-        expr = c.compile(self.expr) if self.expr else "*"
-        if self.distinct:
-            return f"count(distinct {expr})"
-
-        return f"count({expr})"
-
-
-class LazyOps:
-    def __add__(self, other):
-        return BinOp("+", [self, other])
-
-    def __sub__(self, other):
-        return BinOp("-", [self, other])
-
-    def __neg__(self):
-        return UnaryOp("-", self)
-
-    def __gt__(self, other):
-        return BinBoolOp(">", [self, other])
-
-    def __ge__(self, other):
-        return BinBoolOp(">=", [self, other])
-
-    def __eq__(self, other):
-        if other is None:
-            return BinBoolOp("IS", [self, None])
-        return BinBoolOp("=", [self, other])
-
-    def __lt__(self, other):
-        return BinBoolOp("<", [self, other])
-
-    def __le__(self, other):
-        return BinBoolOp("<=", [self, other])
-
-    def __or__(self, other):
-        return BinBoolOp("OR", [self, other])
-
-    def __and__(self, other):
-        return BinBoolOp("AND", [self, other])
-
-    def is_distinct_from(self, other):
-        return IsDistinctFrom(self, other)
-
-    def like(self, other):
-        return BinBoolOp("LIKE", [self, other])
-
-    def test_regex(self, other):
-        return TestRegex(self, other)
-
-    def sum(self):
-        return Func("SUM", [self])
-
-    def max(self):
-        return Func("MAX", [self])
-
-    def min(self):
-        return Func("MIN", [self])
-
-
-@dataclass
-class TestRegex(ExprNode, LazyOps):
-    string: Expr
-    pattern: Expr
-
-    def compile(self, c: Compiler) -> str:
-        if not isinstance(c.dialect, AbstractMixin_Regex):
-            raise NotImplementedError(f"No regex implementation for database '{c.database}'")
-        regex = c.dialect.test_regex(self.string, self.pattern)
-        return c.compile(regex)
-
-
-@dataclass(eq=False)
-class Func(ExprNode, LazyOps):
-    name: str
-    args: Sequence[Expr]
-
-    def compile(self, c: Compiler) -> str:
-        args = ", ".join(c.compile(e) for e in self.args)
-        return f"{self.name}({args})"
-
-
-@dataclass
-class WhenThen(ExprNode):
-    when: Expr
-    then: Expr
-
-    def compile(self, c: Compiler) -> str:
-        return f"WHEN {c.compile(self.when)} THEN {c.compile(self.then)}"
-
-
-@dataclass
-class CaseWhen(ExprNode):
-    cases: Sequence[WhenThen]
-    else_expr: Expr = None
-
-    def compile(self, c: Compiler) -> str:
-        assert self.cases
-        when_thens = " ".join(c.compile(case) for case in self.cases)
-        else_expr = (" ELSE " + c.compile(self.else_expr)) if self.else_expr is not None else ""
-        return f"CASE {when_thens}{else_expr} END"
-
-    @property
-    def type(self):
-        then_types = {_expr_type(case.then) for case in self.cases}
-        if self.else_expr:
-            then_types |= _expr_type(self.else_expr)
-        if len(then_types) > 1:
-            raise QB_TypeError(f"Non-matching types in when: {then_types}")
-        (t,) = then_types
-        return t
-
-    def when(self, *whens: Expr) -> "QB_When":
-        """Add a new 'when' clause to the case expression
-
-        Must be followed by a call to `.then()`
-        """
-        whens = args_as_tuple(whens)
-        whens = _drop_skips(whens)
-        if not whens:
-            raise QueryBuilderError("Expected valid whens")
-
-        # XXX reimplementing api.and_()
-        if len(whens) == 1:
-            return QB_When(self, whens[0])
-        return QB_When(self, BinBoolOp("AND", whens))
-
-    def else_(self, then: Expr):
-        """Add an 'else' clause to the case expression.
-
-        Can only be called once!
-        """
-        if self.else_expr is not None:
-            raise QueryBuilderError(f"Else clause already specified in {self}")
-
-        return self.replace(else_expr=then)
-
-
-@dataclass
-class QB_When:
-    "Partial case-when, used for query-building"
-    casewhen: CaseWhen
-    when: Expr
-
-    def then(self, then: Expr) -> CaseWhen:
-        """Add a 'then' clause after a 'when' was added."""
-        case = WhenThen(self.when, then)
-        return self.casewhen.replace(cases=self.casewhen.cases + [case])
-
-
-@dataclass(eq=False, order=False)
-class IsDistinctFrom(ExprNode, LazyOps):
-    a: Expr
-    b: Expr
-    type = bool
-
-    def compile(self, c: Compiler) -> str:
-        return c.dialect.is_distinct_from(c.compile(self.a), c.compile(self.b))
-
-
-@dataclass(eq=False, order=False)
-class BinOp(ExprNode, LazyOps):
-    op: str
-    args: Sequence[Expr]
-
-    def compile(self, c: Compiler) -> str:
-        expr = f" {self.op} ".join(c.compile(a) for a in self.args)
-        return f"({expr})"
-
-    @property
-    def type(self):
-        types = {_expr_type(i) for i in self.args}
-        if len(types) > 1:
-            raise TypeError(f"Expected all args to have the same type, got {types}")
-        (t,) = types
-        return t
-
-
-@dataclass
-class UnaryOp(ExprNode, LazyOps):
-    op: str
-    expr: Expr
-
-    def compile(self, c: Compiler) -> str:
-        return f"({self.op}{c.compile(self.expr)})"
-
-
-class BinBoolOp(BinOp):
-    type = bool
-
-
-@dataclass(eq=False, order=False)
-class Column(ExprNode, LazyOps):
-    source_table: ITable
-    name: str
-
-    @property
-    def type(self):
-        if self.source_table.schema is None:
-            raise QueryBuilderError(f"Schema required for table {self.source_table}")
-        return self.source_table.schema[self.name]
-
-    def compile(self, c: Compiler) -> str:
-        if c._table_context:
-            if len(c._table_context) > 1:
-                aliases = [
-                    t for t in c._table_context if isinstance(t, TableAlias) and t.source_table is self.source_table
-                ]
-                if not aliases:
-                    return c.quote(self.name)
-                elif len(aliases) > 1:
-                    raise CompileError(f"Too many aliases for column {self.name}")
-                (alias,) = aliases
-
-                return f"{c.quote(alias.name)}.{c.quote(self.name)}"
-
-        return c.quote(self.name)
-
-
-@dataclass
-class TablePath(ExprNode, ITable):
-    path: DbPath
-    schema: Optional[Schema] = field(default=None, repr=False)
-
-    @property
-    def source_table(self):
-        return self
-
-    def compile(self, c: Compiler) -> str:
-        path = self.path  # c.database._normalize_table_path(self.name)
-        return ".".join(map(c.quote, path))
-
-    # Statement shorthands
-    def create(self, source_table: ITable = None, *, if_not_exists: bool = False, primary_keys: List[str] = None):
-        """Returns a query expression to create a new table.
-
-        Parameters:
-            source_table: a table expression to use for initializing the table.
-                          If not provided, the table must have a schema specified.
-            if_not_exists: Add a 'if not exists' clause or not. (note: not all dbs support it!)
-            primary_keys: List of column names which define the primary key
-        """
-
-        if source_table is None and not self.schema:
-            raise ValueError("Either schema or source table needed to create table")
-        if isinstance(source_table, TablePath):
-            source_table = source_table.select()
-        return CreateTable(self, source_table, if_not_exists=if_not_exists, primary_keys=primary_keys)
-
-    def drop(self, if_exists=False):
-        """Returns a query expression to delete the table.
-
-        Parameters:
-            if_not_exists: Add a 'if not exists' clause or not. (note: not all dbs support it!)
-        """
-        return DropTable(self, if_exists=if_exists)
-
-    def truncate(self):
-        """Returns a query expression to truncate the table. (remove all rows)"""
-        return TruncateTable(self)
-
-    def insert_rows(self, rows: Sequence, *, columns: List[str] = None):
-        """Returns a query expression to insert rows to the table, given as Python values.
-
-        Parameters:
-            rows: A list of tuples. Must all have the same width.
-            columns: Names of columns being populated. If specified, must have the same length as the tuples.
-        """
-        rows = list(rows)
-        return InsertToTable(self, ConstantTable(rows), columns=columns)
-
-    def insert_row(self, *values, columns: List[str] = None):
-        """Returns a query expression to insert a single row to the table, given as Python values.
-
-        Parameters:
-            columns: Names of columns being populated. If specified, must have the same length as 'values'
-        """
-        return InsertToTable(self, ConstantTable([values]), columns=columns)
-
-    def insert_expr(self, expr: Expr):
-        """Returns a query expression to insert rows to the table, given as a query expression.
-
-        Parameters:
-            expr: query expression to from which to read the rows
-        """
-        if isinstance(expr, TablePath):
-            expr = expr.select()
-        return InsertToTable(self, expr)
-
-    def time_travel(
-        self, *, before: bool = False, timestamp: datetime = None, offset: int = None, statement: str = None
-    ) -> Compilable:
-        """Selects historical data from the table
-
-        Parameters:
-            before: If false, inclusive of the specified point in time.
-                     If True, only return the time before it. (at/before)
-            timestamp: A constant timestamp
-            offset: the time 'offset' seconds before now
-            statement: identifier for statement, e.g. query ID
-
-        Must specify exactly one of `timestamp`, `offset` or `statement`.
-        """
-        if sum(int(i is not None) for i in (timestamp, offset, statement)) != 1:
-            raise ValueError("Must specify exactly one of `timestamp`, `offset` or `statement`.")
-
-        if timestamp is not None:
-            assert offset is None and statement is None
-
-
-@dataclass
-class TableAlias(ExprNode, ITable):
-    source_table: ITable
-    name: str
-
-    def compile(self, c: Compiler) -> str:
-        return f"{c.compile(self.source_table)} {c.quote(self.name)}"
-
-
-@dataclass
-class Join(ExprNode, ITable, Root):
-    source_tables: Sequence[ITable]
-    op: str = None
-    on_exprs: Sequence[Expr] = None
-    columns: Sequence[Expr] = None
-
-    @property
-    def source_table(self):
-        return self
-
-    @property
-    def schema(self):
-        assert self.columns  # TODO Implement SELECT *
-        s = self.source_tables[0].schema  # TODO validate types match between both tables
-        return type(s)({c.name: c.type for c in self.columns})
-
-    def on(self, *exprs) -> "Join":
-        """Add an ON clause, for filtering the result of the cartesian product (i.e. the JOIN)"""
-        if len(exprs) == 1:
-            (e,) = exprs
-            if isinstance(e, Generator):
-                exprs = tuple(e)
-
-        exprs = _drop_skips(exprs)
-        if not exprs:
-            return self
-
-        return self.replace(on_exprs=(self.on_exprs or []) + exprs)
-
-    def select(self, *exprs, **named_exprs) -> ITable:
-        """Select fields to return from the JOIN operation
-
-        See Also: ``ITable.select()``
-        """
-        if self.columns is not None:
-            # join-select already applied
-            return super().select(*exprs, **named_exprs)
-
-        exprs = _drop_skips(exprs)
-        named_exprs = _drop_skips_dict(named_exprs)
-        exprs += _named_exprs_as_aliases(named_exprs)
-        resolve_names(self.source_table, exprs)
-        # TODO Ensure exprs <= self.columns ?
-        return self.replace(columns=exprs)
-
-    def compile(self, parent_c: Compiler) -> str:
-        tables = [
-            t if isinstance(t, TableAlias) else TableAlias(t, parent_c.new_unique_name()) for t in self.source_tables
-        ]
-        c = parent_c.add_table_context(*tables, in_join=True, in_select=False)
-        op = " JOIN " if self.op is None else f" {self.op} JOIN "
-        joined = op.join(c.compile(t) for t in tables)
-
-        if self.on_exprs:
-            on = " AND ".join(c.compile(e) for e in self.on_exprs)
-            res = f"{joined} ON {on}"
-        else:
-            res = joined
-
-        columns = "*" if self.columns is None else ", ".join(map(c.compile, self.columns))
-        select = f"SELECT {columns} FROM {res}"
-
-        if parent_c.in_select:
-            select = f"({select}) {c.new_unique_name()}"
-        elif parent_c.in_join:
-            select = f"({select})"
-        return select
-
-
-@dataclass
-class GroupBy(ExprNode, ITable, Root):
-    table: ITable
-    keys: Sequence[Expr] = None  # IKey?
-    values: Sequence[Expr] = None
-    having_exprs: Sequence[Expr] = None
-
-    @property
-    def source_table(self):
-        return self
-
-    def __post_init__(self):
-        assert self.keys or self.values
-
-    def having(self, *exprs):
-        """Add a 'HAVING' clause to the group-by"""
-        exprs = args_as_tuple(exprs)
-        exprs = _drop_skips(exprs)
-        if not exprs:
-            return self
-
-        resolve_names(self.table, exprs)
-        return self.replace(having_exprs=(self.having_exprs or []) + exprs)
-
-    def agg(self, *exprs):
-        """Select aggregated fields for the group-by."""
-        exprs = args_as_tuple(exprs)
-        exprs = _drop_skips(exprs)
-        resolve_names(self.table, exprs)
-        return self.replace(values=(self.values or []) + exprs)
-
-    def compile(self, c: Compiler) -> str:
-        if self.values is None:
-            raise CompileError(".group_by() must be followed by a call to .agg()")
-
-        keys = [str(i + 1) for i in range(len(self.keys))]
-        columns = (self.keys or []) + (self.values or [])
-        if isinstance(self.table, Select) and self.table.columns is None and self.table.group_by_exprs is None:
-            return c.compile(
-                self.table.replace(
-                    columns=columns,
-                    group_by_exprs=[Code(k) for k in keys],
-                    having_exprs=self.having_exprs,
-                )
-            )
-
-        keys_str = ", ".join(keys)
-        columns_str = ", ".join(c.compile(x) for x in columns)
-        having_str = (
-            " HAVING " + " AND ".join(map(c.compile, self.having_exprs)) if self.having_exprs is not None else ""
-        )
-        select = (
-            f"SELECT {columns_str} FROM {c.replace(in_select=True).compile(self.table)} GROUP BY {keys_str}{having_str}"
-        )
-
-        if c.in_select:
-            select = f"({select}) {c.new_unique_name()}"
-        elif c.in_join:
-            select = f"({select})"
-        return select
-
-
-@dataclass
-class TableOp(ExprNode, ITable, Root):
-    op: str
-    table1: ITable
-    table2: ITable
-
-    @property
-    def source_table(self):
-        return self
-
-    @property
-    def type(self):
-        # TODO ensure types of both tables are compatible
-        return self.table1.type
-
-    @property
-    def schema(self):
-        s1 = self.table1.schema
-        s2 = self.table2.schema
-        assert len(s1) == len(s2)
-        return s1
-
-    def compile(self, parent_c: Compiler) -> str:
-        c = parent_c.replace(in_select=False)
-        table_expr = f"{c.compile(self.table1)} {self.op} {c.compile(self.table2)}"
-        if parent_c.in_select:
-            table_expr = f"({table_expr}) {c.new_unique_name()}"
-        elif parent_c.in_join:
-            table_expr = f"({table_expr})"
-        return table_expr
-
-
-@dataclass
-class Select(ExprNode, ITable, Root):
-    table: Expr = None
-    columns: Sequence[Expr] = None
-    where_exprs: Sequence[Expr] = None
-    order_by_exprs: Sequence[Expr] = None
-    group_by_exprs: Sequence[Expr] = None
-    having_exprs: Sequence[Expr] = None
-    limit_expr: int = None
-    distinct: bool = False
-    optimizer_hints: Sequence[Expr] = None
-
-    @property
-    def schema(self):
-        s = self.table.schema
-        if s is None or self.columns is None:
-            return s
-        return type(s)({c.name: c.type for c in self.columns})
-
-    @property
-    def source_table(self):
-        return self
-
-    def compile(self, parent_c: Compiler) -> str:
-        c = parent_c.replace(in_select=True)  # .add_table_context(self.table)
-
-        columns = ", ".join(map(c.compile, self.columns)) if self.columns else "*"
-        distinct = "DISTINCT " if self.distinct else ""
-        optimizer_hints = c.dialect.optimizer_hints(self.optimizer_hints) if self.optimizer_hints else ""
-        select = f"SELECT {optimizer_hints}{distinct}{columns}"
-
-        if self.table:
-            select += " FROM " + c.compile(self.table)
-        elif c.dialect.PLACEHOLDER_TABLE:
-            select += f" FROM {c.dialect.PLACEHOLDER_TABLE}"
-
-        if self.where_exprs:
-            select += " WHERE " + " AND ".join(map(c.compile, self.where_exprs))
-
-        if self.group_by_exprs:
-            select += " GROUP BY " + ", ".join(map(c.compile, self.group_by_exprs))
-
-        if self.having_exprs:
-            assert self.group_by_exprs
-            select += " HAVING " + " AND ".join(map(c.compile, self.having_exprs))
-
-        if self.order_by_exprs:
-            select += " ORDER BY " + ", ".join(map(c.compile, self.order_by_exprs))
-
-        if self.limit_expr is not None:
-            select += " " + c.dialect.offset_limit(0, self.limit_expr)
-
-        if parent_c.in_select:
-            select = f"({select}) {c.new_unique_name()}"
-        elif parent_c.in_join:
-            select = f"({select})"
-        return select
-
-    @classmethod
-    def make(cls, table: ITable, distinct: bool = SKIP, optimizer_hints: str = SKIP, **kwargs):
-        assert "table" not in kwargs
-
-        if not isinstance(table, cls):  # If not Select
-            if distinct is not SKIP:
-                kwargs["distinct"] = distinct
-            if optimizer_hints is not SKIP:
-                kwargs["optimizer_hints"] = optimizer_hints
-            return cls(table, **kwargs)
-
-        # We can safely assume isinstance(table, Select)
-        if optimizer_hints is not SKIP:
-            kwargs["optimizer_hints"] = optimizer_hints
-
-        if distinct is not SKIP:
-            if distinct == False and table.distinct:
-                return cls(table, **kwargs)
-            kwargs["distinct"] = distinct
-
-        if table.limit_expr or table.group_by_exprs:
-            return cls(table, **kwargs)
-
-        # Fill in missing attributes, instead of nesting instances
-        for k, v in kwargs.items():
-            if getattr(table, k) is not None:
-                if k == "where_exprs":  # Additive attribute
-                    kwargs[k] = getattr(table, k) + v
-                elif k in ["distinct", "optimizer_hints"]:
-                    pass
-                else:
-                    raise ValueError(k)
-
-        return table.replace(**kwargs)
-
-
-@dataclass
-class Cte(ExprNode, ITable):
-    source_table: Expr
-    name: str = None
-    params: Sequence[str] = None
-
-    def compile(self, parent_c: Compiler) -> str:
-        c = parent_c.replace(_table_context=[], in_select=False)
-        compiled = c.compile(self.source_table)
-
-        name = self.name or parent_c.new_unique_name()
-        name_params = f"{name}({', '.join(self.params)})" if self.params else name
-        parent_c._subqueries[name_params] = compiled
-
-        return name
-
-    @property
-    def schema(self):
-        # TODO add cte to schema
-        return self.source_table.schema
-
-
-def _named_exprs_as_aliases(named_exprs):
-    return [Alias(expr, name) for name, expr in named_exprs.items()]
-
-
-def resolve_names(source_table, exprs):
-    i = 0
-    for expr in exprs:
-        # Iterate recursively and update _ResolveColumn instances with the right expression
-        if isinstance(expr, ExprNode):
-            for v in expr._dfs_values():
-                if isinstance(v, _ResolveColumn):
-                    v.resolve(source_table._get_column(v.resolve_name))
-                    i += 1
-
-
-@dataclass(frozen=False, eq=False, order=False)
-class _ResolveColumn(ExprNode, LazyOps):
-    resolve_name: str
-    resolved: Expr = None
-
-    def resolve(self, expr: Expr):
-        if self.resolved is not None:
-            raise QueryBuilderError("Already resolved!")
-        self.resolved = expr
-
-    def _get_resolved(self) -> Expr:
-        if self.resolved is None:
-            raise QueryBuilderError(f"Column not resolved: {self.resolve_name}")
-        return self.resolved
-
-    def compile(self, c: Compiler) -> str:
-        return self._get_resolved().compile(c)
-
-    @property
-    def type(self):
-        return self._get_resolved().type
-
-    @property
-    def name(self):
-        return self._get_resolved().name
-
-
-class This:
-    """Builder object for accessing table attributes.
-
-    Automatically evaluates to the the 'top-most' table during compilation.
-    """
-
-    def __getattr__(self, name):
-        return _ResolveColumn(name)
-
-    def __getitem__(self, name):
-        if isinstance(name, (list, tuple)):
-            return [_ResolveColumn(n) for n in name]
-        return _ResolveColumn(name)
-
-
-@dataclass
-class In(ExprNode):
-    expr: Expr
-    list: Sequence[Expr]
-
-    type = bool
-
-    def compile(self, c: Compiler):
-        elems = ", ".join(map(c.compile, self.list))
-        return f"({c.compile(self.expr)} IN ({elems}))"
-
-
-@dataclass
-class Cast(ExprNode):
-    expr: Expr
-    target_type: Expr
-
-    def compile(self, c: Compiler) -> str:
-        return f"cast({c.compile(self.expr)} as {c.compile(self.target_type)})"
-
-
-@dataclass
-class Random(ExprNode, LazyOps):
-    type = float
-
-    def compile(self, c: Compiler) -> str:
-        return c.dialect.random()
-
-
-@dataclass
-class ConstantTable(ExprNode):
-    rows: Sequence[Sequence]
-
-    def compile(self, c: Compiler) -> str:
-        raise NotImplementedError()
-
-    def compile_for_insert(self, c: Compiler):
-        return c.dialect.constant_values(self.rows)
-
-
-@dataclass
-class Explain(ExprNode, Root):
-    select: Select
-
-    type = str
-
-    def compile(self, c: Compiler) -> str:
-        return c.dialect.explain_as_text(c.compile(self.select))
-
-
-class CurrentTimestamp(ExprNode):
-    type = datetime
-
-    def compile(self, c: Compiler) -> str:
-        return c.dialect.current_timestamp()
-
-
-@dataclass
-class TimeTravel(ITable):
-    table: TablePath
-    before: bool = False
-    timestamp: datetime = None
-    offset: int = None
-    statement: str = None
-
-    def compile(self, c: Compiler) -> str:
-        assert isinstance(c, AbstractMixin_TimeTravel)
-        return c.compile(
-            c.time_travel(
-                self.table, before=self.before, timestamp=self.timestamp, offset=self.offset, statement=self.statement
-            )
-        )
-
-
-# DDL
-
-
-class Statement(Compilable, Root):
-    type = None
-
-
-@dataclass
-class CreateTable(Statement):
-    path: TablePath
-    source_table: Expr = None
-    if_not_exists: bool = False
-    primary_keys: List[str] = None
-
-    def compile(self, c: Compiler) -> str:
-        ne = "IF NOT EXISTS " if self.if_not_exists else ""
-        if self.source_table:
-            return f"CREATE TABLE {ne}{c.compile(self.path)} AS {c.compile(self.source_table)}"
-
-        schema = ", ".join(f"{c.dialect.quote(k)} {c.dialect.type_repr(v)}" for k, v in self.path.schema.items())
-        pks = (
-            ", PRIMARY KEY (%s)" % ", ".join(self.primary_keys)
-            if self.primary_keys and c.dialect.SUPPORTS_PRIMARY_KEY
-            else ""
-        )
-        return f"CREATE TABLE {ne}{c.compile(self.path)}({schema}{pks})"
-
-
-@dataclass
-class DropTable(Statement):
-    path: TablePath
-    if_exists: bool = False
-
-    def compile(self, c: Compiler) -> str:
-        ie = "IF EXISTS " if self.if_exists else ""
-        return f"DROP TABLE {ie}{c.compile(self.path)}"
-
-
-@dataclass
-class TruncateTable(Statement):
-    path: TablePath
-
-    def compile(self, c: Compiler) -> str:
-        return f"TRUNCATE TABLE {c.compile(self.path)}"
-
-
-@dataclass
-class InsertToTable(Statement):
-    path: TablePath
-    expr: Expr
-    columns: List[str] = None
-    returning_exprs: List[str] = None
-
-    def compile(self, c: Compiler) -> str:
-        if isinstance(self.expr, ConstantTable):
-            expr = self.expr.compile_for_insert(c)
-        else:
-            expr = c.compile(self.expr)
-
-        columns = "(%s)" % ", ".join(map(c.quote, self.columns)) if self.columns is not None else ""
-
-        return f"INSERT INTO {c.compile(self.path)}{columns} {expr}"
-
-    def returning(self, *exprs):
-        """Add a 'RETURNING' clause to the insert expression.
-
-        Note: Not all databases support this feature!
-        """
-        if self.returning_exprs:
-            raise ValueError("A returning clause is already specified")
-
-        exprs = args_as_tuple(exprs)
-        exprs = _drop_skips(exprs)
-        if not exprs:
-            return self
-
-        resolve_names(self.path, exprs)
-        return self.replace(returning_exprs=exprs)
-
-
-@dataclass
-class Commit(Statement):
-    """Generate a COMMIT statement, if we're in the middle of a transaction, or in auto-commit. Otherwise SKIP."""
-
-    def compile(self, c: Compiler) -> str:
-        return "COMMIT" if not c.database.is_autocommit else SKIP
-
-
-@dataclass
-class Param(ExprNode, ITable):
-    """A value placeholder, to be specified at compilation time using the `cv_params` context variable."""
-
-    name: str
-
-    @property
-    def source_table(self):
-        return self
-
-    def compile(self, c: Compiler) -> str:
-        params = cv_params.get()
-        return c._compile(params[self.name])
+from dataclasses import field
+from datetime import datetime
+from typing import Any, Generator, List, Optional, Sequence, Union, Dict, Literal, overload
+from collections import ChainMap
+from functools import lru_cache
+
+from runtype import dataclass as _dataclass, cv_type_checking, isa
+
+from ..utils import join_iter, ArithString
+from ..abcs import AbstractCompiler, Compilable
+from ..abcs.database_types import AbstractTable, AbstractDialect
+from ..abcs.mixins import AbstractMixin_Regex, AbstractMixin_TimeTravel
+from ..schema import Schema, TableType, Options, _Field
+
+from .compiler import Compiler, cv_params, Root, CompileError
+from .base import SKIP, DbPath, args_as_tuple, SqeletonError
+
+
+class QueryBuilderError(SqeletonError):
+    pass
+
+
+class QB_TypeError(QueryBuilderError):
+    pass
+
+
+dataclass = _dataclass(eq=False, order=False)
+
+ellipsis = type(Ellipsis)
+
+
+def cache(user_function, /):
+    'Simple lightweight unbounded cache.  Sometimes called "memoize".'
+    # Taken from https://github.com/python/cpython/blob/3.11/Lib/functools.py
+    return lru_cache(maxsize=None)(user_function)
+
+
+class CompilableNode(Compilable):
+    "Base class for query expression nodes"
+
+    type: Any = None
+
+    def _dfs_values(self):
+        yield self
+        for k, vs in dict(self).items():  # __dict__ provided by runtype.dataclass
+            if k == "source_table":
+                # Skip data-sources, we're only interested in data-parameters
+                continue
+            if not isinstance(vs, (list, tuple)):
+                vs = [vs]
+            for v in vs:
+                if isinstance(v, CompilableNode):
+                    yield from v._dfs_values()
+
+
+class ExprNode(CompilableNode):
+    "Base class for query expression nodes"
+
+    def cast_to(self, to):
+        return Cast(self, to)
+
+
+# Query expressions can only interact with objects that are an instance of 'Expr'
+Expr = Union[ExprNode, str, bytes, bool, int, float, datetime, ArithString, None, dict, list]
+
+
+@dataclass
+class Code(ExprNode, Root):
+    code: str
+    args: Dict[str, Expr] = None
+
+    def compile(self, c: Compiler) -> str:
+        if not self.args:
+            return self.code
+
+        args = {k: c.compile(v) for k, v in self.args.items()}
+        return self.code.format(**args)
+
+
+def _expr_type(e: Expr) -> type:
+    if isinstance(e, ExprNode):
+        return e.type
+    return type(e)
+
+
+@dataclass
+class Alias(ExprNode):
+    expr: Expr
+    name: str
+
+    def compile(self, c: Compiler) -> str:
+        return f"{c.compile(self.expr)} AS {c.quote(self.name)}"
+
+    @property
+    def type(self):
+        return _expr_type(self.expr)
+
+
+def _drop_skips(exprs):
+    return [e for e in exprs if e is not SKIP]
+
+
+def _drop_skips_dict(exprs_dict):
+    return {k: v for k, v in exprs_dict.items() if v is not SKIP}
+
+
+class ITable(AbstractTable):
+    source_table: Any
+    schema: Schema = None
+
+    def select(self, *exprs: Expr, distinct: bool=SKIP, optimizer_hints=SKIP, **named_exprs) -> "Select":
+        """Create a new table with the specified fields"""
+        exprs = args_as_tuple(exprs)
+        exprs = _drop_skips(exprs)
+        named_exprs = _drop_skips_dict(named_exprs)
+        exprs += _named_exprs_as_aliases(named_exprs)
+        resolve_names(self.source_table, exprs)
+        return Select.make(self, columns=exprs, distinct=distinct, optimizer_hints=optimizer_hints)
+
+    def where(self, *exprs) -> "Select":
+        exprs = args_as_tuple(exprs)
+        exprs = _drop_skips(exprs)
+        if not exprs:
+            return self
+
+        resolve_names(self.source_table, exprs)
+        return Select.make(self, where_exprs=exprs)
+
+    def order_by(self, *exprs):
+        exprs = _drop_skips(exprs)
+        if not exprs:
+            return self
+
+        resolve_names(self.source_table, exprs)
+        return Select.make(self, order_by_exprs=exprs)
+
+    def limit(self, limit: int):
+        if limit is SKIP:
+            return self
+
+        return Select.make(self, limit_expr=limit)
+
+    def join(self, target: "ITable"):
+        """Join this table with the target table."""
+        return Join([self, target])
+
+    def group_by(self, *keys) -> "GroupBy":
+        """Group according to the given keys.
+
+        Must be followed by a call to :ref:``GroupBy.agg()``
+        """
+        keys = _drop_skips(keys)
+        resolve_names(self.source_table, keys)
+
+        return GroupBy(self, keys)
+
+    def _get_column(self, name: str):
+        if self.schema:
+            name = self.schema.get_key(name)  # Get the actual name. Might be case-insensitive.
+        return Column(self, name)
+
+    # def __getattr__(self, column):
+    #     return self._get_column(column)
+
+    def __getitem__(self, column):
+        if isinstance(column, (list, tuple)):
+            return [self[c] for c in column]
+        elif column is ...:
+            assert self.schema
+            return [self[k] for k in self.schema]
+        if not isinstance(column, str):
+            raise TypeError(column)
+        return self._get_column(column)
+
+    def count(self):
+        return Select(self, [Count()])
+
+    def union(self, other: "ITable"):
+        """SELECT * FROM self UNION other"""
+        return TableOp("UNION", self, other)
+
+    def union_all(self, other: "ITable"):
+        """SELECT * FROM self UNION ALL other"""
+        return TableOp("UNION ALL", self, other)
+
+    def minus(self, other: "ITable"):
+        """SELECT * FROM self EXCEPT other"""
+        # aka
+        return TableOp("EXCEPT", self, other)
+
+    def intersect(self, other: "ITable"):
+        """SELECT * FROM self INTERSECT other"""
+        return TableOp("INTERSECT", self, other)
+
+    def alias(self, name):
+        if isinstance(self, TableAlias):
+            return self.replace(name=name)
+        return TableAlias(self, name)
+
+
+@dataclass
+class Concat(ExprNode):
+    exprs: list
+    sep: str = None
+
+    def compile(self, c: Compiler) -> str:
+        # We coalesce because on some DBs (e.g. MySQL) concat('a', NULL) is NULL
+        items = [f"coalesce({c.compile(Code(c.dialect.to_string(c.compile(expr))))}, '<null>')" for expr in self.exprs]
+        assert items
+        if len(items) == 1:
+            return items[0]
+
+        if self.sep:
+            items = list(join_iter(f"'{self.sep}'", items))
+        return c.dialect.concat(items)
+
+
+@dataclass
+class Count(ExprNode):
+    expr: Expr = None
+    distinct: bool = False
+
+    type = int
+
+    def compile(self, c: Compiler) -> str:
+        expr = c.compile(self.expr) if self.expr else "*"
+        if self.distinct:
+            return f"count(distinct {expr})"
+
+        return f"count({expr})"
+
+
+class LazyOps:
+    def __add__(self, other):
+        return BinOp("+", [self, other])
+
+    def __sub__(self, other):
+        return BinOp("-", [self, other])
+
+    def __rsub__(self, other):
+        return BinOp("-", [other, self])
+
+    def __mul__(self, other):
+        return BinOp("*", [self, other])
+
+    __radd__ = __add__
+    __rmul__ = __mul__
+
+    def __truediv__(self, other):
+        return BinOp("/", [self, other])
+
+    def __neg__(self):
+        return UnaryOp("-", self)
+
+    def not_(self):
+        return UnaryOp("NOT ", self)
+
+    def __gt__(self, other):
+        return BinBoolOp(">", [self, other])
+
+    def __ge__(self, other):
+        return BinBoolOp(">=", [self, other])
+
+    def __eq__(self, other):
+        if cv_type_checking.get():
+            return super().__eq__(other)
+
+        if other is None:
+            return BinBoolOp("IS", [self, None])
+
+        return BinBoolOp("=", [self, other])
+
+    def __ne__(self, other):
+        if cv_type_checking.get():
+            return super().__ne__(other)
+
+        if other is None:
+            return BinBoolOp("IS NOT", [self, None])
+
+        return BinBoolOp("<>", [self, other])
+
+    def __lt__(self, other):
+        return BinBoolOp("<", [self, other])
+
+    def __le__(self, other):
+        return BinBoolOp("<=", [self, other])
+
+    def __or__(self, other):
+        return BinBoolOp("OR", [self, other])
+
+    def __and__(self, other):
+        return BinBoolOp("AND", [self, other])
+
+    def is_distinct_from(self, other):
+        return IsDistinctFrom(self, other)
+
+    def like(self, other):
+        return BinBoolOp("LIKE", [self, other])
+
+    def ilike(self, other):
+        return BinBoolOp("ILIKE", [self, other])
+
+    def in_(self, *others):
+        others = args_as_tuple(others)
+        assert isinstance(others, tuple), f"Only lists of constants are supported for now, not {others}"
+        if len(others) == 0:
+            return False  # SQL value
+        elif len(others) == 1 and isinstance(others[0], ExprTable):
+            return InTable(self, others[0])
+        return In(self, others)
+
+    def test_regex(self, other):
+        return TestRegex(self, other)
+
+    def sum(self):
+        return Func("SUM", [self])
+
+    def count(self, distinct=False):
+        # return Func("COUNT", [self])
+        return Count(self, distinct=distinct)
+
+    def max(self):
+        return Func("MAX", [self])
+
+    def min(self):
+        return Func("MIN", [self])
+
+
+@dataclass
+class TestRegex(ExprNode, LazyOps):
+    string: Expr
+    pattern: Expr
+
+    def compile(self, c: Compiler) -> str:
+        if not isinstance(c.dialect, AbstractMixin_Regex):
+            raise NotImplementedError(f"No regex implementation for database '{c.database}'")
+        regex = c.dialect.test_regex(self.string, self.pattern)
+        return c.compile(regex)
+
+
+@dataclass
+class Func(ExprNode, LazyOps):
+    name: str
+    args: Sequence[Expr]
+    ret_type: type = None
+
+    def compile(self, c: Compiler) -> str:
+        args = ", ".join(c.compile(e) for e in self.args)
+        return f"{self.name}({args})"
+
+
+@dataclass
+class WhenThen(ExprNode):
+    when: Expr
+    then: Expr
+
+    def compile(self, c: Compiler) -> str:
+        return f"WHEN {c.compile(self.when)} THEN {c.compile(self.then)}"
+
+
+@dataclass
+class CaseWhen(ExprNode, LazyOps):
+    cases: Sequence[WhenThen]
+    else_expr: Expr = None
+
+    def compile(self, c: Compiler) -> str:
+        assert self.cases
+        when_thens = " ".join(c.compile(case) for case in self.cases)
+        else_expr = (" ELSE " + c.compile(self.else_expr)) if self.else_expr is not None else ""
+        return f"CASE {when_thens}{else_expr} END"
+
+    @property
+    def type(self):
+        then_types = {_expr_type(case.then) for case in self.cases}
+        if self.else_expr:
+            then_types.add(_expr_type(self.else_expr))
+        if len(then_types) > 1:
+            raise QB_TypeError(f"Non-matching types in when: {then_types}")
+        (t,) = then_types
+        return t
+
+    def when(self, *whens: Expr) -> "QB_When":
+        """Add a new 'when' clause to the case expression
+
+        Must be followed by a call to `.then()`
+        """
+        whens = args_as_tuple(whens)
+        whens = _drop_skips(whens)
+        if not whens:
+            raise QueryBuilderError("Expected valid whens")
+
+        # XXX reimplementing api.and_()
+        if len(whens) == 1:
+            return QB_When(self, whens[0])
+        return QB_When(self, BinBoolOp("AND", whens))
+
+    def else_(self, then: Expr):
+        """Add an 'else' clause to the case expression.
+
+        Can only be called once!
+        """
+        if self.else_expr is not None:
+            raise QueryBuilderError(f"Else clause already specified in {self}")
+
+        return self.replace(else_expr=then)
+
+
+@dataclass
+class QB_When:
+    "Partial case-when, used for query-building"
+    casewhen: CaseWhen
+    when: Expr
+
+    def then(self, then: Expr) -> CaseWhen:
+        """Add a 'then' clause after a 'when' was added."""
+        case = WhenThen(self.when, then)
+        return self.casewhen.replace(cases=self.casewhen.cases + [case])
+
+
+@_dataclass(eq=False, order=False)
+class IsDistinctFrom(ExprNode, LazyOps):
+    a: Expr
+    b: Expr
+    type = bool
+
+    def compile(self, c: Compiler) -> str:
+        return c.dialect.is_distinct_from(c.compile(self.a), c.compile(self.b))
+
+
+@_dataclass(eq=False, order=False)
+class BinOp(ExprNode, LazyOps):
+    op: str
+    args: Sequence[Expr]
+
+    def compile(self, c: Compiler) -> str:
+        expr = f" {self.op} ".join(c.compile(a) for a in self.args)
+        return f"({expr})"
+
+    @property
+    def type(self):
+        types = {_expr_type(i) for i in self.args}
+        if len(types) > 1:
+            # raise TypeError(f"Expected all args to have the same type, got {types}")
+            return Union[tuple(types)]
+        (t,) = types
+        return t
+
+
+@dataclass
+class UnaryOp(ExprNode, LazyOps):
+    op: str
+    expr: Expr
+
+    def compile(self, c: Compiler) -> str:
+        return f"({self.op}{c.compile(self.expr)})"
+
+    @property
+    def type(self):
+        return self.expr.type
+
+
+class BinBoolOp(BinOp):
+    type = bool
+
+
+@_dataclass(eq=False, order=False)
+class Column(ExprNode, LazyOps):
+    source_table: ITable    # TODO: TablePath
+    name: str
+
+    @property
+    def type(self):
+        if self.source_table.schema is None:
+            raise QueryBuilderError(f"Schema required for table {self.source_table}")
+        return self.source_table.schema[self.name]
+
+    def compile(self, c: Compiler) -> str:
+        if c._table_context:
+            if len(c._table_context) > 1:
+                possible_owners = [t for t in c._table_context if t.schema is None or self.name in t.schema]
+                if len(possible_owners) > 1:
+                    owners = [t for t in possible_owners if t is self.source_table]
+                    if owners:
+                        owner ,= owners
+                        if isinstance(owner, TablePath):
+                            return f"{c.compile(owner)}.{c.quote(self.name)}"
+                        elif isinstance(owner, TableAlias):
+                            return f"{c.quote(owner.name)}.{c.quote(self.name)}"
+
+                aliases = [
+                    t
+                    for t in c._table_context
+                    if isinstance(t, TableAlias) and (t.source_table is self.source_table or t is self.source_table)
+                ]
+                if not aliases:
+                    return c.quote(self.name)
+                elif len(aliases) > 1:
+                    names = [a.name for a in aliases]
+                    raise CompileError(f"Too many aliases for column {self.name} between tables: {names}")
+                (alias,) = aliases
+
+                return f"{c.quote(alias.name)}.{c.quote(self.name)}"
+
+        return c.quote(self.name)
+
+
+class ExprTable(ExprNode, ITable):
+    pass
+
+
+@_dataclass
+class TablePath(ExprTable):
+    path: DbPath
+    schema: Optional[Schema] = field(default=None, repr=False)
+
+    @property
+    def source_table(self):
+        return self
+
+    @property
+    def name(self):
+        return self.path[-1]
+
+    def to_string(self, dialect: AbstractDialect):
+        return ".".join(map(dialect.quote, self.path))
+
+    def compile(self, c: Compiler) -> str:
+        # path = self.path  # c.database._normalize_table_path(self.name)
+        # return ".".join(map(c.quote, path))
+        return self.to_string(c.dialect)
+
+    def __repr__(self) -> str:
+        if self.schema:
+            return f"TablePath({self.path!r}, schema=<{len(self.schema)} cols>)"
+        return f"TablePath({self.path!r})"
+
+    # Statement shorthands
+    def create(self, source_table: ITable = None, *, if_not_exists: bool = False, primary_keys: List[str] = None):
+        """Returns a query expression to create a new table.
+
+        Parameters:
+            source_table: a table expression to use for initializing the table.
+                          If not provided, the table must have a schema specified.
+            if_not_exists: Add a 'if not exists' clause or not. (note: not all dbs support it!)
+            primary_keys: List of column names which define the primary key
+        """
+
+        if source_table is None and not self.schema:
+            raise ValueError("Either schema or source table needed to create table")
+        if isinstance(source_table, TablePath):
+            source_table = source_table.select()
+        return CreateTable(self, source_table, if_not_exists=if_not_exists, primary_keys=primary_keys)
+
+    def drop(self, if_exists=False):
+        """Returns a query expression to delete the table.
+
+        Parameters:
+            if_not_exists: Add a 'if not exists' clause or not. (note: not all dbs support it!)
+        """
+        return DropTable(self, if_exists=if_exists)
+
+    def truncate(self):
+        """Returns a query expression to truncate the table. (remove all rows)"""
+        return TruncateTable(self)
+
+    def delete_rows(self, *where_exprs: Union[Expr, Literal[SKIP]]):
+        where_exprs = args_as_tuple(where_exprs)
+        where_exprs = _drop_skips(where_exprs)
+        if not where_exprs:
+            return self.truncate()
+
+        resolve_names(self.source_table, where_exprs)
+        return DeleteFromTable(self, where_exprs)
+
+    def update_fields(self, *where_exprs: Expr, **kv):
+        where_exprs = args_as_tuple(where_exprs)
+        where_exprs = _drop_skips(where_exprs)
+        resolve_names(self.source_table, where_exprs)
+        resolve_names(self.source_table, kv.values())
+        return UpdateTable(self, kv, where_exprs)
+
+    def insert_rows(self, rows: Sequence, *, columns: List[str] = None):
+        """Returns a query expression to insert rows to the table, given as Python values.
+
+        Parameters:
+            rows: A list of tuples. Must all have the same width.
+            columns: Names of columns being populated. If specified, must have the same length as the tuples.
+        """
+        # TODO support expressions (now, random, etc.)
+        rows = list(rows)
+        if not rows:
+            return SKIP
+
+        if isinstance(rows[0], dict):
+            # TODO: Validate all rows are the same?
+            keys = list(rows[0].keys())
+            if not columns:
+                columns = keys
+            elif not (set(columns) <= set(rows[0].keys())):
+                raise ValueError("Keys in dictionary are not a subset of 'columns'")
+            rows = [[row.get(k) for k in columns] for row in rows]
+
+        return InsertToTable(self, ConstantTable(rows), columns=columns)
+
+    def insert_row(self, *values, columns: List[str] = None, **kw):
+        """Returns a query expression to insert a single row to the table, given as Python values.
+
+        Parameters:
+            columns: Names of columns being populated. If specified, must have the same length as 'values'
+        """
+        if (not values) == (not kw):
+            raise ValueError("Must provide either positional arguments or keyword arguments, but not a mix of both.")
+        if values:
+            if len(values) == 1 and isinstance(values[0], TableType):
+                assert columns is None
+                kw = {k:v.default if isinstance(v, Options) else v
+                      for k, v in values[0]
+                      if not (isinstance(v, Options) and v.auto)
+                      }
+            else:
+                return InsertToTable(self, ConstantTable([values]), columns=columns)
+
+        assert kw
+        assert not columns
+        return InsertToTable(self, ConstantTable([list(kw.values())]), columns=list(kw.keys()))
+
+    def insert_expr(self, expr: Expr):
+        """Returns a query expression to insert rows to the table, given as a query expression.
+
+        Parameters:
+            expr: query expression to from which to read the rows
+        """
+        if isinstance(expr, TablePath):
+            expr = expr.select()
+        return InsertToTable(self, expr)
+
+    def time_travel(
+        self, *, before: bool = False, timestamp: datetime = None, offset: int = None, statement: str = None
+    ) -> Compilable:
+        """Selects historical data from the table
+
+        Parameters:
+            before: If false, inclusive of the specified point in time.
+                     If True, only return the time before it. (at/before)
+            timestamp: A constant timestamp
+            offset: the time 'offset' seconds before now
+            statement: identifier for statement, e.g. query ID
+
+        Must specify exactly one of `timestamp`, `offset` or `statement`.
+        """
+        if sum(int(i is not None) for i in (timestamp, offset, statement)) != 1:
+            raise ValueError("Must specify exactly one of `timestamp`, `offset` or `statement`.")
+
+        if timestamp is not None:
+            assert offset is None and statement is None
+
+
+@_dataclass
+class ForeignKey:
+    table: TablePath
+    field: str
+
+    @property
+    def type(self):
+        return self.table.schema[self.field]
+
+
+@dataclass
+class TableAlias(ExprTable):
+    source_table: ITable
+    name: str
+
+    def compile(self, c: Compiler) -> str:
+        return f"{c.compile(self.source_table)} {c.quote(self.name)}"
+
+    @property
+    def schema(self):
+        return self.source_table.schema
+
+@dataclass
+class Exists(ExprNode, LazyOps):
+    expr: ITable
+
+    type = bool
+
+    def compile(self, c: Compiler) -> str:
+        c = c.replace(in_select=False)
+        return f"EXISTS ({c.compile(self.expr)})"
+
+SelectColumns = Sequence[Union[Expr, ellipsis]]
+
+
+def _expand_ellipsis(schema: dict, columns: SelectColumns):
+    for c in columns:
+        if c is ...:
+            # select all, i.e. *
+            yield from schema.items()
+        else:
+            yield c.name, c.type
+
+
+def _union_dicts(*ds):
+    unioned = {}
+    for d in ds:
+        unioned.update(d)
+    return unioned
+
+
+@dataclass
+class Join(ExprNode, ITable, Root):
+    source_tables: Sequence[ITable]
+    op: str = None
+    on_exprs: Sequence[Expr] = None
+    columns: SelectColumns = None
+
+    @property
+    def source_table(self):
+        return self
+
+    @property
+    @cache
+    def schema(self):
+        if not self.columns:
+            schemas = [t.schema for t in self.source_tables if t.schema]
+            assert schemas and all(schemas)
+            return type(schemas[0])(ChainMap(*schemas))  # TODO merge dictionaries in compliance with SQL dialect!
+
+        # TODO validate types match between both tables
+        schemas = [s.schema for s in self.source_tables]
+        d = _union_dicts(*schemas)
+        return type(schemas[0])(dict(_expand_ellipsis(d, self.columns)))
+
+    def on(self, *exprs) -> "Join":
+        """Add an ON clause, for filtering the result of the cartesian product (i.e. the JOIN)"""
+        if len(exprs) == 1:
+            (e,) = exprs
+            if isinstance(e, Generator):
+                exprs = tuple(e)
+
+        exprs = _drop_skips(exprs)
+        if not exprs:
+            return self
+
+        exprs = [BinBoolOp('=', [t[e] for t in self.source_tables])
+                 if isinstance(e, str)
+                 else e
+                 for e in exprs]
+
+        return self.replace(on_exprs=(self.on_exprs or []) + exprs)
+
+    def select(self, *exprs: Expr, **named_exprs) -> "Join":
+        """Select fields to return from the JOIN operation
+
+        See Also: ``ITable.select()``
+        """
+        for e in exprs:
+            if not isa(e, Expr):
+                raise TypeError(e)
+
+        if self.columns is not None:
+            # join-select already applied
+            return ITable.select(self, *exprs, **named_exprs)
+
+        exprs = _drop_skips(exprs)
+        named_exprs = _drop_skips_dict(named_exprs)
+        exprs += _named_exprs_as_aliases(named_exprs)
+        resolve_names(self.source_table, exprs)
+        # TODO Ensure exprs <= self.columns ?
+        return self.replace(columns=exprs)
+
+    def compile(self, parent_c: Compiler) -> str:
+        tables = [
+            t if isinstance(t, TableAlias) else TableAlias(t, parent_c.new_unique_name()) for t in self.source_tables
+        ]
+        c = parent_c.replace(in_select=True)
+        op = " JOIN " if self.op is None else f" {self.op} JOIN "
+        joined = op.join(c.compile(t) for t in tables)
+        c = parent_c.add_table_context(*tables, in_select=True)
+
+        if self.on_exprs:
+            on = " AND ".join(c.compile(e) for e in self.on_exprs)
+            res = f"{joined} ON {on}"
+        else:
+            res = joined
+
+        columns = "*" if not self.columns else ", ".join(map(c.compile, self.columns))
+        select = f"SELECT {columns} FROM {res}"
+
+        # TODO work with TableAlias
+        if parent_c.in_select:
+            select = f"({select})"
+        return select
+
+
+@dataclass
+class GroupBy(ExprNode, ITable, Root):
+    table: ITable
+    keys_: Sequence[Expr] = None  # IKey?
+    values_: Sequence[Expr] = None
+    having_exprs: Sequence[Expr] = None
+
+    @property
+    def source_table(self):
+        return self
+
+    @property
+    @cache
+    def schema(self):
+        s = self.table.schema
+        if s is None:
+            return None
+        return type(s)({c.name: c.type for c in self.keys_ + self.values_})
+
+    def __post_init__(self):
+        assert self.keys_ or self.values_
+
+    def having(self, *exprs):
+        """Add a 'HAVING' clause to the group-by"""
+        exprs = args_as_tuple(exprs)
+        exprs = _drop_skips(exprs)
+        if not exprs:
+            return self
+
+        resolve_names(self.table, exprs)
+        return self.replace(having_exprs=(self.having_exprs or []) + exprs)
+
+    def agg(self, *exprs, **named_exprs):
+        """Select aggregated fields for the group-by."""
+        exprs = args_as_tuple(exprs)
+        exprs = _drop_skips(exprs)
+
+        named_exprs = _drop_skips_dict(named_exprs)
+        exprs += _named_exprs_as_aliases(named_exprs)
+
+        resolve_names(self.table, exprs)
+        return self.replace(values_=(self.values_ or []) + exprs)
+
+    def compile(self, c: Compiler) -> str:
+        if self.values_ is None:
+            raise CompileError(".group_by() must be followed by a call to .agg()")
+
+        keys = [str(i + 1) for i in range(len(self.keys_))]
+        columns = (self.keys_ or []) + (self.values_ or [])
+        if isinstance(self.table, Select) and not self.table.columns and self.table.group_by_exprs is None:
+            return c.compile(
+                self.table.replace(
+                    columns=columns,
+                    group_by_exprs=[Code(k) for k in keys],
+                    having_exprs=self.having_exprs,
+                )
+            )
+
+        keys_str = ", ".join(keys)
+        columns_str = ", ".join(c.compile(x) for x in columns)
+        having_str = (
+            " HAVING " + " AND ".join(map(c.compile, self.having_exprs)) if self.having_exprs is not None else ""
+        )
+        select = f"SELECT {columns_str} FROM {SelectCompiler(c).compile(self.table)} GROUP BY {keys_str}{having_str}"
+
+        if c.in_select:
+            select = f"({select})"
+        return select
+
+
+@dataclass
+class TableOp(ExprNode, ITable, Root):
+    op: str
+    table1: ITable
+    table2: ITable
+
+    @property
+    def source_table(self):
+        return self
+
+    @property
+    def type(self):
+        # TODO ensure types of both tables are compatible
+        return self.table1.type
+
+    @property
+    def schema(self):
+        s1 = self.table1.schema
+        s2 = self.table2.schema
+        assert len(s1) == len(s2)
+        return s1
+
+    def compile(self, parent_c: Compiler) -> str:
+        c = parent_c.replace(in_select=False)
+        table_expr = f"{c.compile(self.table1)} {self.op} {c.compile(self.table2)}"
+        if parent_c.in_select:
+            table_expr = f"({table_expr})"
+        return table_expr
+
+
+@dataclass
+class SelectCompiler(AbstractCompiler):
+    c: Compiler
+
+    def compile(self, elem: Any, params: Dict[str, Any] = None) -> str:
+        if isinstance(elem, (Select, TableOp, GroupBy, Join)):
+            elem = TableAlias(elem, self.c.new_unique_name())
+        c = self.c.replace(in_select=True)
+        return c.compile(elem, params)
+
+    @property
+    def dialect(self):
+        return self.c.dialect
+
+    def add_table_context(self, *tables: Sequence, **kw):
+        return SelectCompiler(self.c.add_table_context(*tables, **kw))
+
+
+@dataclass
+class Desc(ExprNode):
+    expr: ExprNode
+
+    def compile(self, c: Compiler) -> str:
+        e = c.compile(expr)
+        return f"{e} DESC"
+
+
+@dataclass
+class Select(ExprTable, Root):
+    table: Expr = None
+    columns: SelectColumns = None
+    where_exprs: Sequence[Expr] = None
+    order_by_exprs: Sequence[Expr] = None
+    group_by_exprs: Sequence[Expr] = None
+    having_exprs: Sequence[Expr] = None
+    limit_expr: int = None
+    distinct: bool = False
+    optimizer_hints: Sequence[Expr] = None
+    postfix: str = None
+
+    @property
+    @cache
+    def schema(self):
+        s = self.table.schema
+        if s is None or not self.columns:
+            return s
+        return type(s)(dict(_expand_ellipsis(s, self.columns)))
+
+    @property
+    def source_table(self):
+        return self
+
+    def compile(self, parent_c: Compiler) -> str:
+        c = SelectCompiler(parent_c)
+
+        if isinstance(self.table, (TablePath,)):
+            c = c.add_table_context(self.table)
+
+        columns = ", ".join(map(c.compile, self.columns)) if self.columns else "*"
+        distinct = "DISTINCT " if self.distinct else ""
+        optimizer_hints = c.dialect.optimizer_hints(self.optimizer_hints) if self.optimizer_hints else ""
+        select = f"SELECT {optimizer_hints}{distinct}{columns}"
+
+        if self.table:
+            select += " FROM " + c.compile(self.table)
+        elif c.dialect.PLACEHOLDER_TABLE:
+            select += f" FROM {c.dialect.PLACEHOLDER_TABLE}"
+
+        if self.where_exprs:
+            select += " WHERE " + " AND ".join(map(c.compile, self.where_exprs))
+
+        if self.group_by_exprs:
+            select += " GROUP BY " + ", ".join(map(c.compile, self.group_by_exprs))
+
+        if self.having_exprs:
+            assert self.group_by_exprs
+            select += " HAVING " + " AND ".join(map(c.compile, self.having_exprs))
+
+        if self.order_by_exprs:
+            select += " ORDER BY " + ", ".join(map(c.compile, self.order_by_exprs))
+
+        if self.limit_expr is not None:
+            select += " " + c.dialect.offset_limit(0, self.limit_expr)
+        
+        if self.postfix:
+            select += self.postfix
+
+        if parent_c.in_select:
+            select = f"({select})"
+        return select
+
+    @classmethod
+    def make(cls, table: ITable, distinct: bool = SKIP, optimizer_hints: str = SKIP, **kwargs):
+        assert "table" not in kwargs
+
+        if optimizer_hints is not SKIP:
+            kwargs["optimizer_hints"] = optimizer_hints
+        if distinct is not SKIP:
+            kwargs["distinct"] = distinct
+
+        # If table is not a select, return a new Select instance
+        if not isinstance(table, cls):
+            return cls(table, **kwargs)
+        
+        if 'columns' in kwargs and table.columns is not None:
+            return cls(table, **kwargs)
+
+        # We can safely assume isinstance(table, Select)
+        # We will try to merge them, instead of creating nested instances
+        if distinct is False and table.distinct:
+            # Cannot merge the selects
+            return cls(table, **kwargs)
+
+        if table.limit_expr or table.group_by_exprs:
+            # Cannot merge the selects
+            return cls(table, **kwargs)
+
+        # Fill in missing attributes
+        for k, v in kwargs.items():
+            if getattr(table, k) is not None:
+                if k == "where_exprs":  # Additive attribute
+                    kwargs[k] = getattr(table, k) + v
+                elif k in ["distinct", "optimizer_hints"]:
+                    pass
+                else:
+                    raise ValueError(k)
+
+        return table.replace(**kwargs)
+
+
+@dataclass
+class Cte(ExprNode, ITable):
+    source_table: Expr
+    name: str = None
+    params: Sequence[str] = None
+
+    def compile(self, parent_c: Compiler) -> str:
+        c = parent_c.replace(_table_context=[], in_select=False)
+        compiled = c.compile(self.source_table)
+
+        name = self.name or parent_c.new_unique_name()
+        name_params = f"{name}({', '.join(self.params)})" if self.params else name
+        parent_c._subqueries[name_params] = compiled
+
+        return name
+
+    @property
+    def schema(self):
+        # TODO add cte to schema
+        return self.source_table.schema
+
+
+def _named_exprs_as_aliases(named_exprs):
+    return [Alias(expr, name) for name, expr in named_exprs.items()]
+
+
+def resolve_names(source_table, exprs):
+    i = 0
+    for expr in exprs:
+        # Iterate recursively and update _ResolveColumn instances with the right expression
+        if isinstance(expr, ExprNode):
+            for v in expr._dfs_values():
+                if isinstance(v, _ResolveColumn):
+                    v.resolve(source_table._get_column(v.resolve_name))
+                    i += 1
+
+
+@_dataclass(frozen=False, eq=False, order=False)
+class _ResolveColumn(ExprNode, LazyOps):
+    resolve_name: str
+    resolved: Expr = None
+
+    def resolve(self, expr: Expr):
+        if self.resolved is not None:
+            raise QueryBuilderError(f"Column '{self.resolve_name}' Already resolved! To value: {self.resolved}")
+        self.resolved = expr
+
+    def _get_resolved(self) -> Expr:
+        if self.resolved is None:
+            breakpoint()
+            raise QueryBuilderError(f"Column not resolved: {self.resolve_name}")
+        return self.resolved
+
+    def compile(self, c: Compiler) -> str:
+        return self._get_resolved().compile(c)
+
+    @property
+    def type(self):
+        return self._get_resolved().type
+
+    @property
+    def name(self):
+        return self._get_resolved().name
+
+    def __rsub__(self, other):
+        if other is ...:
+            # return Wildcard()
+            pass
+
+        # return super().__rsub__(other)    XXX why does it fail?
+        return LazyOps.__rsub__(self, other)
+
+
+
+
+
+@dataclass
+class Wildcard:
+    exclude: List[str]
+
+
+class This:
+    """Builder object for accessing table attributes.
+
+    Automatically evaluates to the the 'top-most' table during compilation.
+    """
+
+    def __getattr__(self, name):
+        return _ResolveColumn(name)
+
+    @overload
+    def __getitem__(self, name: str) -> 'This': ...
+    @overload
+    def __getitem__(self, name: (list, tuple)) -> List['This']:
+        ...
+
+    def __getitem__(self, name):
+        if isinstance(name, (list, tuple)):
+            return [_ResolveColumn(n) for n in name]
+        return _ResolveColumn(name)
+
+
+@dataclass
+class In(ExprNode):
+    expr: Expr
+    list: Sequence[Expr]
+
+    type = bool
+
+    def compile(self, c: Compiler):
+        elems = ", ".join(map(c.compile, self.list))
+        return f"({c.compile(self.expr)} IN ({elems}))"
+
+
+@dataclass
+class InTable(ExprNode):
+    expr: Expr
+    source_table: ExprTable
+
+    type = bool
+
+    def compile(self, c: Compiler):
+        return f"({c.compile(self.expr)} IN ({self.source_table.compile(c.replace(in_select=False))}))"
+
+
+@dataclass
+class Cast(ExprNode):
+    expr: Expr
+    target_type: Expr
+
+    def compile(self, c: Compiler) -> str:
+        return f"cast({c.compile(self.expr)} as {c.compile(self.target_type)})"
+
+
+@dataclass
+class Random(ExprNode, LazyOps):
+    type = float
+
+    def compile(self, c: Compiler) -> str:
+        return c.dialect.random()
+
+
+@dataclass
+class ConstantTable(ExprNode):
+    rows: Sequence[Sequence]
+
+    def compile(self, c: Compiler) -> str:
+        raise NotImplementedError()
+
+    def compile_for_insert(self, c: Compiler):
+        compiled_rows = [[c.compile(v) for v in r] for r in self.rows]
+        return c.dialect.immediate_values(compiled_rows)
+
+
+@dataclass
+class Explain(ExprNode, Root):
+    select: Select
+
+    type = str
+
+    def compile(self, c: Compiler) -> str:
+        return c.dialect.explain_as_text(c.compile(self.select))
+
+
+@dataclass
+class CurrentTimestamp(ExprNode, LazyOps):
+    type = datetime
+
+    def compile(self, c: Compiler) -> str:
+        return c.dialect.current_timestamp()
+
+
+@dataclass
+class TimeTravel(ITable):
+    table: TablePath
+    before: bool = False
+    timestamp: datetime = None
+    offset: int = None
+    statement: str = None
+
+    def compile(self, c: Compiler) -> str:
+        assert isinstance(c, AbstractMixin_TimeTravel)
+        return c.compile(
+            c.time_travel(
+                self.table, before=self.before, timestamp=self.timestamp, offset=self.offset, statement=self.statement
+            )
+        )
+
+
+# DDL
+
+
+class Statement(CompilableNode, Root):
+    type = None
+
+
+@dataclass
+class CreateTable(Statement):
+    path: TablePath
+    source_table: Expr = None
+    if_not_exists: bool = False
+    primary_keys: List[str] = None
+
+    def compile(self, c: Compiler) -> str:
+        ne = "IF NOT EXISTS " if self.if_not_exists else ""
+        if self.source_table:
+            return f"CREATE TABLE {ne}{c.compile(self.path)} AS {c.compile(self.source_table)}"
+
+        primary_keys = [k for k, v in self.path.schema.items() if isinstance(v, _Field) and v.options.primary_key]
+
+        if self.primary_keys is not None:
+            if primary_keys:
+                assert self.primary_keys == primary_keys
+            else:
+                primary_keys = self.primary_keys
+
+        if primary_keys and c.dialect.SUPPORTS_PRIMARY_KEY:
+            pks = ", PRIMARY KEY (%s)" % ", ".join(primary_keys)
+        else:
+            pks = ""
+
+        schema = ", ".join(f"{c.dialect.quote(k)} {c.dialect.type_repr(v)}" for k, v in self.path.schema.items())
+        return f"CREATE TABLE {ne}{c.compile(self.path)}({schema}{pks})"
+
+
+@dataclass
+class DropTable(Statement):
+    path: TablePath
+    if_exists: bool = False
+
+    def compile(self, c: Compiler) -> str:
+        ie = "IF EXISTS " if self.if_exists else ""
+        return f"DROP TABLE {ie}{c.compile(self.path)}"
+
+
+@dataclass
+class TruncateTable(Statement):
+    path: TablePath
+
+    def compile(self, c: Compiler) -> str:
+        return f"TRUNCATE TABLE {c.compile(self.path)}"
+
+
+class ReturningStatement(Statement):
+    returning_exprs: SelectColumns = None
+
+    @property
+    def type(self):
+        return None if self.returning_exprs is None else ITable
+
+    def returning(self, *exprs):
+        """Add a 'RETURNING' clause to the insert expression.
+
+        Note: Not all databases support this feature!
+        """
+        if self.returning_exprs:
+            raise ValueError("A returning clause is already specified")
+
+        exprs = args_as_tuple(exprs)
+        exprs = _drop_skips(exprs)
+        if not exprs:
+            return self
+
+        resolve_names(self.path, exprs)
+        return self.replace(returning_exprs=exprs)
+
+    def _compile_returning(self, c: Compiler):
+        if not self.returning_exprs:
+            return ""
+
+        columns = ", ".join(map(c.compile, self.returning_exprs))
+        return " RETURNING " + columns
+
+@dataclass
+class DeleteFromTable(ReturningStatement):
+    path: TablePath
+    where_exprs: Sequence[Expr] = None
+    returning_exprs: SelectColumns = None
+
+    def compile(self, c: Compiler) -> str:
+        delete = f"DELETE FROM {c.compile(self.path)}"
+        if self.where_exprs:
+            delete += " WHERE " + " AND ".join(map(c.compile, self.where_exprs))
+
+        delete += self._compile_returning(c)
+        return delete
+
+
+@dataclass
+class UpdateTable(ReturningStatement):
+    path: TablePath
+    updates: Dict[str, Expr]
+    where_exprs: Sequence[Expr] = None
+    returning_exprs: SelectColumns = None
+
+    def compile(self, c: Compiler) -> str:
+        updates = [f"{k} = {c.compile(v)}" for k, v in self.updates.items()]
+        update = f"UPDATE {c.compile(self.path)} SET " + ", ".join(updates)
+
+        if self.where_exprs:
+            update += " WHERE " + " AND ".join(map(c.compile, self.where_exprs))
+        update += self._compile_returning(c)
+        return update
+
+
+@dataclass
+class InsertToTable(ReturningStatement):
+    path: TablePath
+    expr: Expr
+    columns: List[str] = None
+    returning_exprs: SelectColumns = None
+
+    @property
+    def type(self):
+        if self.returning_exprs:
+            return ITable
+        return None
+
+    def compile(self, c: Compiler) -> str:
+        if isinstance(self.expr, ConstantTable):
+            expr = self.expr.compile_for_insert(c)
+        else:
+            expr = c.compile(self.expr)
+
+        columns = "(%s)" % ", ".join(map(c.quote, self.columns)) if self.columns is not None else ""
+
+        q = f"INSERT INTO {c.compile(self.path)}{columns} {expr}"
+
+        q += self._compile_returning(c)
+        return q
+
+    def returning(self, *exprs):
+        """Add a 'RETURNING' clause to the insert expression.
+
+        Note: Not all databases support this feature!
+        """
+        if self.returning_exprs:
+            raise ValueError("A returning clause is already specified")
+
+        exprs = args_as_tuple(exprs)
+        exprs = _drop_skips(exprs)
+        if not exprs:
+            return self
+
+        resolve_names(self.path, exprs)
+        return self.replace(returning_exprs=exprs)
+
+
+@dataclass
+class Commit(Statement):
+    """Generate a COMMIT statement, if we're in the middle of a transaction, or in auto-commit. Otherwise SKIP."""
+
+    def compile(self, c: Compiler) -> str:
+        return "COMMIT" if not c.database.is_autocommit else SKIP
+
+
+@dataclass
+class Param(ExprNode, ITable):
+    """A value placeholder, to be specified at compilation time using the `cv_params` context variable."""
+
+    name: str
+
+    @property
+    def source_table(self):
+        return self
+
+    def compile(self, c: Compiler) -> str:
+        params = cv_params.get()
+        return c._compile(params[self.name])
```

### Comparing `sqeleton-0.0.8/sqeleton/query_utils.py` & `sqeleton-0.0.9/sqeleton/query_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"Module for query utilities that didn't make it into the query-builder (yet)"
-
-from contextlib import suppress
-
-from sqeleton.databases import DbPath, QueryError, Oracle
-from sqeleton.queries import table, commit, Expr
-
-
-def _drop_table_oracle(name: DbPath):
-    t = table(name)
-    # Experience shows double drop is necessary
-    with suppress(QueryError):
-        yield t.drop()
-        yield t.drop()
-    yield commit
-
-
-def _drop_table(name: DbPath):
-    t = table(name)
-    yield t.drop(if_exists=True)
-    yield commit
-
-
-def drop_table(db, tbl):
-    if isinstance(db, Oracle):
-        db.query(_drop_table_oracle(tbl))
-    else:
-        db.query(_drop_table(tbl))
-
-
-def _append_to_table_oracle(path: DbPath, expr: Expr):
-    """See append_to_table"""
-    assert expr.schema, expr
-    t = table(path, schema=expr.schema)
-    with suppress(QueryError):
-        yield t.create()  # uses expr.schema
-        yield commit
-    yield t.insert_expr(expr)
-    yield commit
-
-
-def _append_to_table(path: DbPath, expr: Expr):
-    """Append to table"""
-    assert expr.schema, expr
-    t = table(path, schema=expr.schema)
-    yield t.create(if_not_exists=True)  # uses expr.schema
-    yield commit
-    yield t.insert_expr(expr)
-    yield commit
-
-
-def append_to_table(db, path, expr):
-    f = _append_to_table_oracle if isinstance(db, Oracle) else _append_to_table
-    db.query(f(path, expr))
+"Module for query utilities that didn't make it into the query-builder (yet)"
+
+from contextlib import suppress
+
+from sqeleton.databases import DbPath, QueryError, Oracle
+from sqeleton.queries import table, commit, Expr
+
+
+def _drop_table_oracle(name: DbPath):
+    t = table(name)
+    # Experience shows double drop is necessary
+    with suppress(QueryError):
+        yield t.drop()
+        yield t.drop()
+    yield commit
+
+
+def _drop_table(name: DbPath):
+    t = table(name)
+    yield t.drop(if_exists=True)
+    yield commit
+
+
+def drop_table(db, tbl):
+    if isinstance(db, Oracle):
+        db.query(_drop_table_oracle(tbl))
+    else:
+        db.query(_drop_table(tbl))
+
+
+def _append_to_table_oracle(path: DbPath, expr: Expr):
+    """See append_to_table"""
+    assert expr.schema, expr
+    t = table(path, schema=expr.schema)
+    with suppress(QueryError):
+        yield t.create()  # uses expr.schema
+        yield commit
+    yield t.insert_expr(expr)
+    yield commit
+
+
+def _append_to_table(path: DbPath, expr: Expr):
+    """Append to table"""
+    assert expr.schema, expr
+    t = table(path, schema=expr.schema)
+    yield t.create(if_not_exists=True)  # uses expr.schema
+    yield commit
+    yield t.insert_expr(expr)
+    yield commit
+
+
+def append_to_table(db, path, expr):
+    f = _append_to_table_oracle if isinstance(db, Oracle) else _append_to_table
+    db.query(f(path, expr))
```

### Comparing `sqeleton-0.0.8/sqeleton/utils.py` & `sqeleton-0.0.9/sqeleton/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,341 +1,349 @@
-from typing import (
-    Iterable,
-    Iterator,
-    MutableMapping,
-    Union,
-    Any,
-    Sequence,
-    Dict,
-    Hashable,
-    TypeVar,
-    TYPE_CHECKING,
-    List,
-)
-from abc import abstractmethod
-from weakref import ref
-import math
-import string
-import re
-from uuid import UUID
-from urllib.parse import urlparse
-
-# -- Common --
-
-try:
-    from typing import Self
-except ImportError:
-    Self = Any
-
-
-class WeakCache:
-    def __init__(self):
-        self._cache = {}
-
-    def _hashable_key(self, k: Union[dict, Hashable]) -> Hashable:
-        if isinstance(k, dict):
-            return tuple(k.items())
-        return k
-
-    def add(self, key: Union[dict, Hashable], value: Any):
-        key = self._hashable_key(key)
-        self._cache[key] = ref(value)
-
-    def get(self, key: Union[dict, Hashable]) -> Any:
-        key = self._hashable_key(key)
-
-        value = self._cache[key]()
-        if value is None:
-            del self._cache[key]
-            raise KeyError(f"Key {key} not found, or no longer a valid reference")
-
-        return value
-
-
-def join_iter(joiner: Any, iterable: Iterable) -> Iterable:
-    it = iter(iterable)
-    try:
-        yield next(it)
-    except StopIteration:
-        return
-    for i in it:
-        yield joiner
-        yield i
-
-
-def safezip(*args):
-    "zip but makes sure all sequences are the same length"
-    lens = list(map(len, args))
-    if len(set(lens)) != 1:
-        raise ValueError(f"Mismatching lengths in arguments to safezip: {lens}")
-    return zip(*args)
-
-
-def is_uuid(u):
-    try:
-        UUID(u)
-    except ValueError:
-        return False
-    return True
-
-
-def match_regexps(regexps: Dict[str, Any], s: str) -> Sequence[tuple]:
-    for regexp, v in regexps.items():
-        m = re.match(regexp + "$", s)
-        if m:
-            yield m, v
-
-
-# -- Schema --
-
-V = TypeVar("V")
-
-
-class CaseAwareMapping(MutableMapping[str, V]):
-    @abstractmethod
-    def get_key(self, key: str) -> str:
-        ...
-
-    def new(self, initial=()):
-        return type(self)(initial)
-
-
-class CaseInsensitiveDict(CaseAwareMapping):
-    def __init__(self, initial):
-        self._dict = {k.lower(): (k, v) for k, v in dict(initial).items()}
-
-    def __getitem__(self, key: str) -> V:
-        return self._dict[key.lower()][1]
-
-    def __iter__(self) -> Iterator[V]:
-        return iter(self._dict)
-
-    def __len__(self) -> int:
-        return len(self._dict)
-
-    def __setitem__(self, key: str, value):
-        k = key.lower()
-        if k in self._dict:
-            key = self._dict[k][0]
-        self._dict[k] = key, value
-
-    def __delitem__(self, key: str):
-        del self._dict[key.lower()]
-
-    def get_key(self, key: str) -> str:
-        return self._dict[key.lower()][0]
-
-    def __repr__(self) -> str:
-        return repr(dict(self.items()))
-
-
-class CaseSensitiveDict(dict, CaseAwareMapping):
-    def get_key(self, key):
-        self[key]  # Throw KeyError if key doesn't exist
-        return key
-
-    def as_insensitive(self):
-        return CaseInsensitiveDict(self)
-
-
-# -- Alphanumerics --
-
-alphanums = " -" + string.digits + string.ascii_uppercase + "_" + string.ascii_lowercase
-
-
-class ArithString:
-    @classmethod
-    def new(cls, *args, **kw):
-        return cls(*args, **kw)
-
-    def range(self, other: "ArithString", count: int):
-        assert isinstance(other, ArithString)
-        checkpoints = split_space(self.int, other.int, count)
-        return [self.new(int=i) for i in checkpoints]
-
-
-class ArithUUID(UUID, ArithString):
-    "A UUID that supports basic arithmetic (add, sub)"
-
-    def __int__(self):
-        return self.int
-
-    def __add__(self, other: int):
-        if isinstance(other, int):
-            return self.new(int=self.int + other)
-        return NotImplemented
-
-    def __sub__(self, other: Union[UUID, int]):
-        if isinstance(other, int):
-            return self.new(int=self.int - other)
-        elif isinstance(other, UUID):
-            return self.int - other.int
-        return NotImplemented
-
-
-def numberToAlphanum(num: int, base: str = alphanums) -> str:
-    digits = []
-    while num > 0:
-        num, remainder = divmod(num, len(base))
-        digits.append(remainder)
-    return "".join(base[i] for i in digits[::-1])
-
-
-def alphanumToNumber(alphanum: str, base: str = alphanums) -> int:
-    num = 0
-    for c in alphanum:
-        num = num * len(base) + base.index(c)
-    return num
-
-
-def justify_alphanums(s1: str, s2: str):
-    max_len = max(len(s1), len(s2))
-    s1 = s1.ljust(max_len)
-    s2 = s2.ljust(max_len)
-    return s1, s2
-
-
-def alphanums_to_numbers(s1: str, s2: str):
-    s1, s2 = justify_alphanums(s1, s2)
-    n1 = alphanumToNumber(s1)
-    n2 = alphanumToNumber(s2)
-    return n1, n2
-
-
-class ArithAlphanumeric(ArithString):
-    def __init__(self, s: str, max_len=None):
-        if s is None:
-            raise ValueError("Alphanum string cannot be None")
-        if max_len and len(s) > max_len:
-            raise ValueError(f"Length of alphanum value '{str}' is longer than the expected {max_len}")
-
-        for ch in s:
-            if ch not in alphanums:
-                raise ValueError(f"Unexpected character {ch} in alphanum string")
-
-        self._str = s
-        self._max_len = max_len
-
-    # @property
-    # def int(self):
-    #     return alphanumToNumber(self._str, alphanums)
-
-    def __str__(self):
-        s = self._str
-        if self._max_len:
-            s = s.rjust(self._max_len, alphanums[0])
-        return s
-
-    def __len__(self):
-        return len(self._str)
-
-    def __repr__(self):
-        return f'alphanum"{self._str}"'
-
-    def __add__(self, other: "Union[ArithAlphanumeric, int]") -> "ArithAlphanumeric":
-        if isinstance(other, int):
-            if other != 1:
-                raise NotImplementedError("not implemented for arbitrary numbers")
-            num = alphanumToNumber(self._str)
-            return self.new(numberToAlphanum(num + 1))
-
-        return NotImplemented
-
-    def range(self, other: "ArithAlphanumeric", count: int):
-        assert isinstance(other, ArithAlphanumeric)
-        n1, n2 = alphanums_to_numbers(self._str, other._str)
-        split = split_space(n1, n2, count)
-        return [self.new(numberToAlphanum(s)) for s in split]
-
-    def __sub__(self, other: "Union[ArithAlphanumeric, int]") -> float:
-        if isinstance(other, ArithAlphanumeric):
-            n1, n2 = alphanums_to_numbers(self._str, other._str)
-            return n1 - n2
-
-        return NotImplemented
-
-    def __ge__(self, other):
-        if not isinstance(other, type(self)):
-            return NotImplemented
-        return self._str >= other._str
-
-    def __lt__(self, other):
-        if not isinstance(other, type(self)):
-            return NotImplemented
-        return self._str < other._str
-
-    def __eq__(self, other):
-        if not isinstance(other, type(self)):
-            return NotImplemented
-        return self._str == other._str
-
-    def new(self, *args, **kw):
-        return type(self)(*args, **kw, max_len=self._max_len)
-
-
-def number_to_human(n):
-    millnames = ["", "k", "m", "b"]
-    n = float(n)
-    millidx = max(
-        0,
-        min(len(millnames) - 1, int(math.floor(0 if n == 0 else math.log10(abs(n)) / 3))),
-    )
-
-    return "{:.0f}{}".format(n / 10 ** (3 * millidx), millnames[millidx])
-
-
-def split_space(start, end, count) -> List[int]:
-    size = end - start
-    assert count <= size, (count, size)
-    return list(range(start, end, (size + 1) // (count + 1)))[1 : count + 1]
-
-
-def remove_passwords_in_dict(d: dict, replace_with: str = "***"):
-    for k, v in d.items():
-        if k == "password":
-            d[k] = replace_with
-        elif isinstance(v, dict):
-            remove_passwords_in_dict(v, replace_with)
-        elif k.startswith("database"):
-            d[k] = remove_password_from_url(v, replace_with)
-
-
-def _join_if_any(sym, args):
-    args = list(args)
-    if not args:
-        return ""
-    return sym.join(str(a) for a in args if a)
-
-
-def remove_password_from_url(url: str, replace_with: str = "***") -> str:
-    parsed = urlparse(url)
-    account = parsed.username or ""
-    if parsed.password:
-        account += ":" + replace_with
-    host = _join_if_any(":", filter(None, [parsed.hostname, parsed.port]))
-    netloc = _join_if_any("@", filter(None, [account, host]))
-    replaced = parsed._replace(netloc=netloc)
-    return replaced.geturl()
-
-
-def match_like(pattern: str, strs: Sequence[str]) -> Iterable[str]:
-    reo = re.compile(pattern.replace("%", ".*").replace("?", ".") + "$")
-    for s in strs:
-        if reo.match(s):
-            yield s
-
-
-
-class UnknownMeta(type):
-    def __instancecheck__(self, instance):
-        return instance is Unknown
-
-    def __repr__(self):
-        return "Unknown"
-
-
-class Unknown(metaclass=UnknownMeta):
-    def __nonzero__(self):
-        raise TypeError()
-
-    def __new__(class_, *args, **kwargs):
-        raise RuntimeError("Unknown is a singleton")
+from typing import (
+    Iterable,
+    Iterator,
+    MutableMapping,
+    Union,
+    Any,
+    Sequence,
+    Dict,
+    Hashable,
+    TypeVar,
+    Generator,
+    List,
+)
+from abc import ABC, abstractmethod
+from weakref import ref
+import math
+import string
+import re
+from uuid import UUID
+from urllib.parse import urlparse
+
+# -- Common --
+
+try:
+    from typing import Self
+except ImportError:
+    Self = Any
+
+
+class WeakCache:
+    def __init__(self):
+        self._cache = {}
+
+    def _hashable_key(self, k: Union[dict, Hashable]) -> Hashable:
+        if isinstance(k, dict):
+            return tuple(k.items())
+        return k
+
+    def add(self, key: Union[dict, Hashable], value: Any):
+        key = self._hashable_key(key)
+        self._cache[key] = ref(value)
+
+    def get(self, key: Union[dict, Hashable]) -> Any:
+        key = self._hashable_key(key)
+
+        value = self._cache[key]()
+        if value is None:
+            del self._cache[key]
+            raise KeyError(f"Key {key} not found, or no longer a valid reference")
+
+        return value
+
+
+def join_iter(joiner: Any, iterable: Iterable) -> Iterable:
+    it = iter(iterable)
+    try:
+        yield next(it)
+    except StopIteration:
+        return
+    for i in it:
+        yield joiner
+        yield i
+
+
+def safezip(*args):
+    "zip but makes sure all sequences are the same length"
+    lens = list(map(len, args))
+    if len(set(lens)) != 1:
+        raise ValueError(f"Mismatching lengths in arguments to safezip: {lens}")
+    return zip(*args)
+
+
+def is_uuid(u):
+    try:
+        UUID(u)
+    except ValueError:
+        return False
+    return True
+
+
+def match_regexps(regexps: Dict[str, Any], s: str) -> Generator[tuple, None, None]:
+    for regexp, v in regexps.items():
+        m = re.match(regexp + "$", s)
+        if m:
+            yield m, v
+
+
+# -- Schema --
+
+V = TypeVar("V")
+
+
+class CaseAwareMapping(MutableMapping[str, V]):
+    @abstractmethod
+    def get_key(self, key: str) -> str:
+        ...
+
+    @abstractmethod
+    def __init__(self, initial):
+        ...
+
+    def new(self, initial=()):
+        return type(self)(initial)
+
+
+class CaseInsensitiveDict(CaseAwareMapping[V]):
+    def __init__(self, initial):
+        self._dict = {k.lower(): (k, v) for k, v in dict(initial).items()}
+
+    def __getitem__(self, key: str) -> V:
+        return self._dict[key.lower()][1]
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self._dict)
+
+    def __len__(self) -> int:
+        return len(self._dict)
+
+    def __setitem__(self, key: str, value):
+        k = key.lower()
+        if k in self._dict:
+            key = self._dict[k][0]
+        self._dict[k] = key, value
+
+    def __delitem__(self, key: str):
+        del self._dict[key.lower()]
+
+    def get_key(self, key: str) -> str:
+        return self._dict[key.lower()][0]
+
+    def __repr__(self) -> str:
+        return repr(dict(self.items()))
+
+
+class CaseSensitiveDict(dict, CaseAwareMapping):
+    def get_key(self, key) -> str:
+        self[key]  # Throw KeyError if key doesn't exist
+        return key
+
+    def as_insensitive(self):
+        return CaseInsensitiveDict(self)
+
+
+# -- Alphanumerics --
+
+alphanums = " -" + string.digits + string.ascii_uppercase + "_" + string.ascii_lowercase
+
+
+class ArithString(ABC):
+    @classmethod
+    def new(cls, *args, **kw):
+        return cls(*args, **kw)
+
+    def range(self, other: "ArithString", count: int):
+        assert isinstance(other, ArithString)
+        checkpoints = split_space(self.int, other.int, count)
+        return [self.new(int=i) for i in checkpoints]
+
+    @property
+    @abstractmethod
+    def int(self):
+        ...
+
+
+class ArithUUID(UUID, ArithString):
+    "A UUID that supports basic arithmetic (add, sub)"
+
+    def __int__(self):
+        return self.int
+
+    def __add__(self, other: int):
+        if isinstance(other, int):
+            return self.new(int=self.int + other)
+        return NotImplemented
+
+    def __sub__(self, other: Union[UUID, int]):
+        if isinstance(other, int):
+            return self.new(int=self.int - other)
+        elif isinstance(other, UUID):
+            return self.int - other.int
+        return NotImplemented
+
+
+def numberToAlphanum(num: int, base: str = alphanums) -> str:
+    digits = []
+    while num > 0:
+        num, remainder = divmod(num, len(base))
+        digits.append(remainder)
+    return "".join(base[i] for i in digits[::-1])
+
+
+def alphanumToNumber(alphanum: str, base: str = alphanums) -> int:
+    num = 0
+    for c in alphanum:
+        num = num * len(base) + base.index(c)
+    return num
+
+
+def justify_alphanums(s1: str, s2: str):
+    max_len = max(len(s1), len(s2))
+    s1 = s1.ljust(max_len)
+    s2 = s2.ljust(max_len)
+    return s1, s2
+
+
+def alphanums_to_numbers(s1: str, s2: str):
+    s1, s2 = justify_alphanums(s1, s2)
+    n1 = alphanumToNumber(s1)
+    n2 = alphanumToNumber(s2)
+    return n1, n2
+
+
+class ArithAlphanumeric(ArithString):
+    def __init__(self, s: str, max_len=None):
+        if s is None:
+            raise ValueError("Alphanum string cannot be None")
+        if max_len and len(s) > max_len:
+            raise ValueError(f"Length of alphanum value '{str}' is longer than the expected {max_len}")
+
+        for ch in s:
+            if ch not in alphanums:
+                raise ValueError(f"Unexpected character {ch} in alphanum string")
+
+        self._str = s
+        self._max_len = max_len
+
+    # @property
+    # def int(self):
+    #     return alphanumToNumber(self._str, alphanums)
+
+    def __str__(self):
+        s = self._str
+        if self._max_len:
+            s = s.rjust(self._max_len, alphanums[0])
+        return s
+
+    def __len__(self):
+        return len(self._str)
+
+    def __repr__(self):
+        return f'alphanum"{self._str}"'
+
+    def __add__(self, other: "Union[ArithAlphanumeric, int]") -> "ArithAlphanumeric":
+        if isinstance(other, int):
+            if other != 1:
+                raise NotImplementedError("not implemented for arbitrary numbers")
+            num = alphanumToNumber(self._str)
+            return self.new(numberToAlphanum(num + 1))
+
+        return NotImplemented
+
+    def range(self, other: "ArithAlphanumeric", count: int):
+        assert isinstance(other, ArithAlphanumeric)
+        n1, n2 = alphanums_to_numbers(self._str, other._str)
+        split = split_space(n1, n2, count)
+        return [self.new(numberToAlphanum(s)) for s in split]
+
+    def __sub__(self, other: "Union[ArithAlphanumeric, int]") -> float:
+        if isinstance(other, ArithAlphanumeric):
+            n1, n2 = alphanums_to_numbers(self._str, other._str)
+            return n1 - n2
+
+        return NotImplemented
+
+    def __ge__(self, other):
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self._str >= other._str
+
+    def __lt__(self, other):
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self._str < other._str
+
+    def __eq__(self, other):
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self._str == other._str
+
+    def new(self, *args, **kw):
+        return type(self)(*args, **kw, max_len=self._max_len)
+
+
+def number_to_human(n):
+    millnames = ["", "k", "m", "b"]
+    n = float(n)
+    millidx = max(
+        0,
+        min(len(millnames) - 1, int(math.floor(0 if n == 0 else math.log10(abs(n)) / 3))),
+    )
+
+    return "{:.0f}{}".format(n / 10 ** (3 * millidx), millnames[millidx])
+
+
+def split_space(start, end, count) -> List[int]:
+    size = end - start
+    assert count <= size, (count, size)
+    return list(range(start, end, (size + 1) // (count + 1)))[1 : count + 1]
+
+
+def remove_passwords_in_dict(d: dict, replace_with: str = "***"):
+    for k, v in d.items():
+        if k == "password":
+            d[k] = replace_with
+        elif isinstance(v, dict):
+            remove_passwords_in_dict(v, replace_with)
+        elif k.startswith("database"):
+            d[k] = remove_password_from_url(v, replace_with)
+
+
+def _join_if_any(sym, args):
+    args = list(args)
+    if not args:
+        return ""
+    return sym.join(str(a) for a in args if a)
+
+
+def remove_password_from_url(url: str, replace_with: str = "***") -> str:
+    parsed = urlparse(url)
+    account = parsed.username or ""
+    if parsed.password:
+        account += ":" + replace_with
+    host = _join_if_any(":", filter(None, [parsed.hostname, parsed.port]))
+    netloc = _join_if_any("@", filter(None, [account, host]))
+    replaced = parsed._replace(netloc=netloc)
+    return replaced.geturl()
+
+
+def match_like(pattern: str, strs: Sequence[str]) -> Iterable[str]:
+    reo = re.compile(pattern.replace("%", ".*").replace("?", ".") + "$")
+    for s in strs:
+        if reo.match(s):
+            yield s
+
+
+class UnknownMeta(type):
+    def __instancecheck__(self, instance):
+        return instance is Unknown
+
+    def __repr__(self):
+        return "Unknown"
+
+
+class Unknown(metaclass=UnknownMeta):
+    def __nonzero__(self):
+        raise TypeError()
+
+    def __new__(cls, *args, **kwargs):
+        raise RuntimeError("Unknown is a singleton")
```

