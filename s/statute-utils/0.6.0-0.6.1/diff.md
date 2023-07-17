# Comparing `tmp/statute_utils-0.6.0.tar.gz` & `tmp/statute_utils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.6.0.tar", max compression
+gzip compressed data, was "statute_utils-0.6.1.tar", max compression
```

## Comparing `statute_utils-0.6.0.tar` & `statute_utils-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.0/LICENSE
--rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.0/README.md
--rw-r--r--   0        0        0     1357 2023-07-16 05:42:45.235534 statute_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      817 2023-07-16 07:43:47.611153 statute_utils-0.6.0/statute_utils/__init__.py
--rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.0/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     5976 2023-07-16 05:09:00.421516 statute_utils-0.6.0/statute_utils/components/branch.py
--rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.0/statute_utils/components/builder.py
--rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.6.0/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.0/statute_utils/components/short.py
--rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.0/statute_utils/components/utils.py
--rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.6.0/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.6.0/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.0/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.0/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.0/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.0/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.0/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.0/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.0/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6537 2023-07-16 06:04:54.216686 statute_utils-0.6.0/statute_utils/statute.py
--rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.0/statute_utils/templater.py
--rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.0/statute_utils/templates/crumbs.html
--rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.0/statute_utils/templates/paragraph.html
--rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.0/statute_utils/templates/subtree.html
--rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.0/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.0/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.1/README.md
+-rw-r--r--   0        0        0     1357 2023-07-17 01:45:55.216080 statute_utils-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      858 2023-07-17 01:59:03.643591 statute_utils-0.6.1/statute_utils/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.1/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     5976 2023-07-16 05:09:00.421516 statute_utils-0.6.1/statute_utils/components/branch.py
+-rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.1/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.6.1/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.1/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.1/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.1/statute_utils/config.py
+-rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.1/statute_utils/main.py
+-rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.1/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.1/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.1/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.1/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.1/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.1/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.1/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.1/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6640 2023-07-17 01:48:41.595692 statute_utils-0.6.1/statute_utils/statute.py
+-rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.1/statute_utils/templater.py
+-rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.1/statute_utils/templates/crumbs.html
+-rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.1/statute_utils/templates/paragraph.html
+-rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.1/statute_utils/templates/subtree.html
+-rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.1/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.1/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.1/PKG-INFO
```

### Comparing `statute_utils-0.6.0/LICENSE` & `statute_utils-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/README.md` & `statute_utils-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/pyproject.toml` & `statute_utils-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.6.0"
+version = "0.6.1"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.6.0/statute_utils/__init__.py` & `statute_utils-0.6.1/statute_utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,25 @@
     is_par,
     ltr,
     make_branch,
     make_branch_json_array,
     set_mp_slug,
     try_short,
 )
+from .config import get_local_statute_db, setup_local_statute_db
 from .main import (
     CountedStatute,
     extract_named_rules,
     extract_rule,
     extract_rules,
     extract_serial_rules,
 )
-from .models import Rule, create_db
+from .models import Rule
 from .models_names import STYLES_NAMED, NamedPattern
 from .models_serials import STYLES_SERIAL, SerialPattern
-from .statute import STATUTE_DIR, Statute
+from .statute import Statute
 from .templater import (
     html_crumbs_from_hierarchy,
     html_paragraph_from_hierarchy,
     html_tree_from_hierarchy,
     render_units,
 )
```

### Comparing `statute_utils-0.6.0/statute_utils/components/__init__.py` & `statute_utils-0.6.1/statute_utils/components/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/components/branch.py` & `statute_utils-0.6.1/statute_utils/components/branch.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/components/builder.py` & `statute_utils-0.6.1/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/components/category.py` & `statute_utils-0.6.1/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/components/short.py` & `statute_utils-0.6.1/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/components/utils.py` & `statute_utils-0.6.1/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/main.py` & `statute_utils-0.6.1/statute_utils/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,21 +126,14 @@
     and [named][named-pattern] rules (_the Civil Code of the Philippines_),
     extract the [`Rules`][rule-model] into their canonical serial variants.
 
     Examples:
         >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
         >>> list(extract_rules(text)) # get all rules
         [<Rule: ra 386>, <Rule: ra 386>, <Rule: spain civil>]
-        >>> ambiguous_text = "The Civil Code"
-        >>> doc_date1 = datetime.date(year=1940, month=1, day=1)
-        >>> list(extract_rules(ambiguous_text, doc_date1))
-        [<Rule: spain civil>]
-        >>> doc_date2 = datetime.date(year=1960, month=1, day=1)
-        >>> list(extract_rules(ambiguous_text, doc_date2))
-        [<Rule: ra 386>]
 
     Args:
         text (str): Text to search for statute patterns.
         document_date (datetime.date | None, optional): When present, makes a naive dated extraction of _named_ ambiguous rules. Defaults to None.
         context (str | None, optional): Helps provide error message, if provided. Defaults to None.
 
     Yields:
```

### Comparing `statute_utils-0.6.0/statute_utils/models.py` & `statute_utils-0.6.1/statute_utils/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,20 @@
 import datetime
 import re
 from collections.abc import Iterator
 from dataclasses import dataclass
 from functools import cached_property
-from pathlib import Path
 from re import Pattern
 from typing import NamedTuple
 
 from slugify import slugify
 from sqlite_utils import Database
 
 from .components import StatuteSerialCategory, make_regex_readable
-
-STATUTE_DB = Database("statute_files.db", use_counts_table=True)
-
-
-def create_db(db: Database = STATUTE_DB):
-    rows = []
-    for item in STATUTE_DIR.glob("**/*.yml"):
-        cat, num, date, variant = item.parts[-4:]
-        v = variant.split(".")[0]
-        rows.append(
-            {
-                "id": "-".join([cat, num, date, v]),
-                "cat": cat,
-                "num": num,
-                "date": date,
-                "variant": variant.split(".")[0],
-                "size": item.stat().st_size,
-            }
-        )
-    db["statutes"].insert_all(rows, pk="id", ignore=True)  # type: ignore
-    db["statutes"].create_index(  # type: ignore
-        columns={"cat", "num"},
-        index_name="idx_statutes_cat_num",
-        if_not_exists=True,
-    )
-    db["statutes"].create_index(  # type: ignore
-        columns={"cat", "num", "date"},
-        index_name="idx_statutes_cat_num_date",
-        if_not_exists=True,
-    )
-
-
-STATUTE_DIR = Path().home().joinpath("code/corpus-statutes")
-if not STATUTE_DB["statutes"].exists():
-    create_db()
+from .config import get_local_statute_db
 
 
 @dataclass(frozen=True)
 class Rule:
     """A `Rule` is detected if it matches either a named pattern or a serial pattern.
     Each rule maps to a category and number.
     """  # noqa: E501
@@ -71,25 +36,28 @@
 
     @property
     def serial_title(self):
         return StatuteSerialCategory(self.cat.value).serialize(self.num)
 
     @cached_property
     def date(self) -> datetime.date | None:
+        """Useful only for local folder use when the `statute_files.db` is created
+        by `setup_local_statute_db()`"""
         try:
-            date_str = STATUTE_DB.execute_returning_dicts(
-                """--sql
-                    select min(s.date) min_date
-                    from statutes s
-                    where s.cat = :cat and s.num = :num
-                    group by s.cat, s.num;
-                    """,
-                params={"cat": self.cat.value.lower(), "num": self.num.lower()},
-            )[0]["min_date"]
-            return datetime.date.fromisoformat(date_str)
+            if db := get_local_statute_db():
+                date_str = db.execute_returning_dicts(
+                    """--sql
+                        select min(s.date) min_date
+                        from statutes s
+                        where s.cat = :cat and s.num = :num
+                        group by s.cat, s.num;
+                        """,
+                    params={"cat": self.cat.value.lower(), "num": self.num.lower()},
+                )[0]["min_date"]
+                return datetime.date.fromisoformat(date_str)
         except Exception:
             return None
 
 
 class NamedPattern(NamedTuple):
     name: str
     regex_base: str
```

### Comparing `statute_utils-0.6.0/statute_utils/models_names.py` & `statute_utils-0.6.1/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/models_serials.py` & `statute_utils-0.6.1/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/recipes/digits.py` & `statute_utils-0.6.1/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/recipes/spain.py` & `statute_utils-0.6.1/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/statute.py` & `statute_utils-0.6.1/statute_utils/statute.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     StatuteSerialCategory,
     StatuteTitle,
     create_fts_snippet_column,
     create_unit_heading,
     set_node_ids,
     walk,
 )
-from .models import STATUTE_DIR, Rule
+from .models import Rule
 from .templater import html_tree_from_hierarchy
 
 
 class Statute(NamedTuple):
     """A instance is dependent on a statute path from a fixed
-    `STATUTE_DIR`. The shape of the Python object will be different
+    directory. The shape of the Python object will be different
     from the shape of the dumpable `.yml` export."""
 
     titles: list[StatuteTitle]
     rule: Rule
     variant: int
     date: datetime.date
     units: list[dict]
@@ -103,19 +103,22 @@
                 "caption": unit.get("caption"),
                 "content": unit.get("content"),
                 "snippetable": create_fts_snippet_column(unit),  # enable searchability
             }
             if subunits := unit.get("units"):
                 yield from cls.flatten_units(statute_id, subunits, present_heading)
 
-    def to_file(self) -> Path:
+    def to_file(self, basepath: Path) -> Path:
         """Orders different key, value pairs for a yaml dump operation.
         Ensures each node in the tree is properly (rather than alphabetically) ordered.
         """
-        f = STATUTE_DIR.joinpath(self.__repr__())
+        if not basepath.exists():
+            raise Exception("Ensure a statute base path exists first.")
+
+        f = basepath.joinpath(self.__repr__())
         f.parent.mkdir(parents=True, exist_ok=True)
         data: dict = self._asdict()
         data["units"] = walk(data["units"])
         text = yaml.dump(data, width=60)  # see representer added in walk
         f.write_text(text)
         return f
```

### Comparing `statute_utils-0.6.0/statute_utils/templater.py` & `statute_utils-0.6.1/statute_utils/templater.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/templates/tree.css` & `statute_utils-0.6.1/statute_utils/templates/tree.css`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/statute_utils/templates/tree.html` & `statute_utils-0.6.1/statute_utils/templates/tree.html`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.0/PKG-INFO` & `statute_utils-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.6.0
+Version: 0.6.1
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

