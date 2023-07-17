# Comparing `tmp/sqlalchemy_crud-0.1.2.tar.gz` & `tmp/sqlalchemy_crud-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_crud-0.1.2.tar", max compression
+gzip compressed data, was "sqlalchemy_crud-0.2.0.tar", max compression
```

## Comparing `sqlalchemy_crud-0.1.2.tar` & `sqlalchemy_crud-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/LICENSE
--rw-r--r--   0        0        0      627 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      221 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/sqlalchemy_crud/__init__.py
--rw-r--r--   0        0        0     2945 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/sqlalchemy_crud/crud.py
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3959 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/README.md
+-rw-r--r--   0        0        0      657 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/sqlalchemy_crud/__init__.py
+-rw-r--r--   0        0        0     3542 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/sqlalchemy_crud/crud.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.2.0/PKG-INFO
```

### Comparing `sqlalchemy_crud-0.1.2/LICENSE` & `sqlalchemy_crud-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud-0.1.2/sqlalchemy_crud/crud.py` & `sqlalchemy_crud-0.2.0/sqlalchemy_crud/crud.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import List
+from typing import List, Type
 
+import sqlalchemy
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session
 
 Base = declarative_base()
 
 
 def get_models(
@@ -62,14 +63,38 @@
     for key, value in schema.items():
         if hasattr(db_model, key):
             setattr(db_model, key, value)
         else:
             raise AttributeError
 
     db.commit()
+    db.refresh(db_model)
+    return db_model
+
+
+def update_model_by_attribute(
+    db: Session,
+    model: Type[sqlalchemy.orm.decl_api.DeclarativeMeta],
+    lookup_attribute: str,
+    lookup_attribute_value,
+    schema: dict,
+):
+    db_model = get_model_by_attribute(
+        db=db,
+        model=model,
+        attribute=lookup_attribute,
+        attribute_value=lookup_attribute_value,
+    )
+    for key, value in schema.items():
+        if hasattr(db_model, key):
+            setattr(db_model, key, value)
+        else:
+            raise AttributeError
+
+    db.commit()
     db.refresh(db_model)
     return db_model
 
 
 def delete_model(db: Session, model: Base, model_id: int) -> None:
     db_model = get_model(db=db, model=model, model_id=model_id)
     db.delete(db_model)
```

