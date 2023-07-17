# Comparing `tmp/oarepo-model-builder-multilingual-3.0.7.tar.gz` & `tmp/oarepo-model-builder-multilingual-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-3.0.7.tar", last modified: Mon Jul 10 13:55:12 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-3.0.8.tar", last modified: Mon Jul 17 11:59:53 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-3.0.7.tar` & `oarepo-model-builder-multilingual-3.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.900027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.900027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.900027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-10 13:55:12.908027 oarepo-model-builder-multilingual-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.864162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.864162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.868162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/faker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:59:53.864162 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-17 11:59:53.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-17 11:59:53.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:59:53.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-17 11:59:53.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 11:59:53.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 11:59:53.000000 oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-17 11:59:53.872162 oarepo-model-builder-multilingual-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:59:17.000000 oarepo-model-builder-multilingual-3.0.8/setup.py
```

### Comparing `oarepo-model-builder-multilingual-3.0.7/LICENSE` & `oarepo-model-builder-multilingual-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.7
+Version: 3.0.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-3.0.7/README.md` & `oarepo-model-builder-multilingual-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/__init__.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from oarepo_model_builder.datatypes import DataType, Import, datatypes
 from oarepo_model_builder.datatypes.components import (
-    ObjectMarshmallowComponent,
-    RegularMarshmallowComponent,
+    UIMarshmallowComponent,
+    UIObjectMarshmallowComponent,
 )
 from oarepo_model_builder.datatypes.components.marshmallow import MarshmallowField
 from oarepo_model_builder.datatypes.components.marshmallow.graph import MarshmallowClass
 from oarepo_model_builder.utils.absolute_class import convert_to_absolute_class_name
 from oarepo_model_builder.utils.python_name import qualified_name
 
 from oarepo_model_builder_multilingual.datatypes import I18nDataType
@@ -68,36 +68,35 @@
                 imports=Import.from_config(marshmallow.get("imports", [])),
                 fields=fields,
                 strict=True,
             )
         )
 
 
-class I18nMarshmallowComponent(I18nMarshmallowMixin, ObjectMarshmallowComponent):
+class UII18nMarshmallowComponent(I18nMarshmallowMixin, UIObjectMarshmallowComponent):
     eligible_datatypes = [I18nDataType]
 
-    def marshmallow_field(
+    def ui_marshmallow_field(
         self, datatype: DataType, *, fields: List[MarshmallowField], **kwargs
     ):
         f = []
-
-        RegularMarshmallowComponent.marshmallow_field(self, datatype=datatype, fields=f)
-
+        UIMarshmallowComponent.ui_marshmallow_field(self, datatype=datatype, fields=f)
+        if not f:
+            return
         fld: MarshmallowField = f[0]
-
         fields.append(fld)
 
-    def marshmallow_build_class(self, *, datatype, classes, **kwargs):
+    def ui_marshmallow_build_class(self, *, datatype, classes, **kwargs):
         self._build_class(
             datatype,
-            datatype.section_marshmallow.config,
-            datatype.section_marshmallow.children,
-            "marshmallow_field",
+            datatype.section_ui.config.setdefault("marshmallow", {}),
+            datatype.section_ui.children,
+            "ui_marshmallow_field",
             classes,
         )
 
     def _marshmallow_field_arguments(self, datatype, section, marshmallow, field_name):
         return [
-            *RegularMarshmallowComponent._marshmallow_field_arguments(
+            *UIMarshmallowComponent._marshmallow_field_arguments(
                 self, datatype, section, marshmallow, field_name
             ),
         ]
```

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from oarepo_model_builder.datatypes import DataType, Import, datatypes
 from oarepo_model_builder.datatypes.components import (
-    UIMarshmallowComponent,
-    UIObjectMarshmallowComponent,
+    ObjectMarshmallowComponent,
+    RegularMarshmallowComponent,
 )
 from oarepo_model_builder.datatypes.components.marshmallow import MarshmallowField
 from oarepo_model_builder.datatypes.components.marshmallow.graph import MarshmallowClass
 from oarepo_model_builder.utils.absolute_class import convert_to_absolute_class_name
 from oarepo_model_builder.utils.python_name import qualified_name
 
 from oarepo_model_builder_multilingual.datatypes import I18nDataType
@@ -68,33 +68,38 @@
                 imports=Import.from_config(marshmallow.get("imports", [])),
                 fields=fields,
                 strict=True,
             )
         )
 
 
-class UII18nMarshmallowComponent(I18nMarshmallowMixin, UIObjectMarshmallowComponent):
+class I18nMarshmallowComponent(I18nMarshmallowMixin, ObjectMarshmallowComponent):
     eligible_datatypes = [I18nDataType]
 
-    def ui_marshmallow_field(
+    def marshmallow_field(
         self, datatype: DataType, *, fields: List[MarshmallowField], **kwargs
     ):
         f = []
-        UIMarshmallowComponent.ui_marshmallow_field(self, datatype=datatype, fields=f)
+
+        RegularMarshmallowComponent.marshmallow_field(self, datatype=datatype, fields=f)
+        if not f:
+            # the marshmallow field was not generated (read=False & write=False)
+            return
+
         fld: MarshmallowField = f[0]
         fields.append(fld)
 
-    def ui_marshmallow_build_class(self, *, datatype, classes, **kwargs):
+    def marshmallow_build_class(self, *, datatype, classes, **kwargs):
         self._build_class(
             datatype,
-            datatype.section_ui.config.setdefault("marshmallow", {}),
-            datatype.section_ui.children,
-            "ui_marshmallow_field",
+            datatype.section_marshmallow.config,
+            datatype.section_marshmallow.children,
+            "marshmallow_field",
             classes,
         )
 
     def _marshmallow_field_arguments(self, datatype, section, marshmallow, field_name):
         return [
-            *UIMarshmallowComponent._marshmallow_field_arguments(
+            *RegularMarshmallowComponent._marshmallow_field_arguments(
                 self, datatype, section, marshmallow, field_name
             ),
         ]
```

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/datatypes/multilings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/faker.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/faker.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/utils/supported_langs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/validation/__init__.py` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.7
+Version: 3.0.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-3.0.8/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.7/setup.cfg` & `oarepo-model-builder-multilingual-3.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-multilingual
-version = 3.0.7
+version = 3.0.8
 description = 
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

