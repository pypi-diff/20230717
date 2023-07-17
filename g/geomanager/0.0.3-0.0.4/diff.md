# Comparing `tmp/geomanager-0.0.3.tar.gz` & `tmp/geomanager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomanager-0.0.3.tar", last modified: Thu Jul  6 14:08:10 2023, max compression
+gzip compressed data, was "geomanager-0.0.4.tar", last modified: Mon Jul 17 09:20:17 2023, max compression
```

## Comparing `geomanager-0.0.3.tar` & `geomanager-0.0.4.tar`

### file list

```diff
@@ -1,123 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.886046 geomanager-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 14:07:56.000000 geomanager-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-06 14:08:10.886046 geomanager-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-06 14:07:56.000000 geomanager-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.874046 geomanager-0.0.3/geomanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    50516 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/migrations/0004_alter_dataset_can_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/migrations/0005_delete_countryboundary_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/models/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/models/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/samples/basemaps/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/samples/basemaps/basemaps.json
--rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/samples/basemaps/style.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/serializers/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/static/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/static/django_large_image/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/static/django_large_image/js/geojs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/static/django_large_image/js/geojs/1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/static/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/static/geomanager/css/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/css/preview-map.css
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/css/upload.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/static/geomanager/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/css/vendor/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.878046 geomanager-0.0.3/geomanager/static/geomanager/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/images/geomapviewer-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/static/geomanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/add-multiple.js
--rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/colorbrewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/mbt_source_extra.js
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/raster-preview.js
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/raster_style_extra.js
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/vector-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/static/geomanager/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/vendor/d3-format.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   745424 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/vendor/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (123)   542509 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/vendor/ol.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/static/geomanager/js/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/widgets/icon_chooser.js
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/widgets/raster_style_widget.js
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/static/geomanager/js/wms-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.874046 geomanager-0.0.3/geomanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.870046 geomanager-0.0.3/geomanager/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.874046 geomanager-0.0.3/geomanager/templates/admin/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/templates/admin/geomanager/layerrasterfile/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/templates/django_nextjs/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/django_nextjs/mapviewer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/templates/geomanager/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/raster_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/raster_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/raster_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/vector_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/vector_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/vector_upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.882046 geomanager-0.0.3/geomanager/templates/geomanager/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/widgets/raster_style_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/geomanager/wms_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.886046 geomanager-0.0.3/geomanager/templates/modeladmin/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/templates/modeladmin/index_without_custom_create.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.886046 geomanager-0.0.3/geomanager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/utils/raster_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/utils/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/utils/vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.886046 geomanager-0.0.3/geomanager/views/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/nextjs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    20493 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/views/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.886046 geomanager-0.0.3/geomanager/viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/viewsets/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/viewsets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/viewsets/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/viewsets/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    23126 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-06 14:07:56.000000 geomanager-0.0.3/geomanager/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:08:10.874046 geomanager-0.0.3/geomanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-06 14:08:10.000000 geomanager-0.0.3/geomanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-06 14:08:10.000000 geomanager-0.0.3/geomanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:08:10.000000 geomanager-0.0.3/geomanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-06 14:08:10.000000 geomanager-0.0.3/geomanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 14:08:10.000000 geomanager-0.0.3/geomanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 14:07:56.000000 geomanager-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-06 14:08:10.886046 geomanager-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.344429 geomanager-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 09:19:56.000000 geomanager-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-17 09:20:17.344429 geomanager-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-17 09:19:56.000000 geomanager-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.328428 geomanager-0.0.4/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    50516 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0004_alter_dataset_can_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0005_delete_countryboundary_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0006_stationsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0008_stationsettings_name_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0009_stationsettings_popup_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0010_remove_stationsettings_popup_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/samples/basemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/samples/basemaps/basemaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/samples/basemaps/style.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/django_large_image/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/django_large_image/js/geojs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/static/django_large_image/js/geojs/1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/static/geomanager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/css/preview-map.css
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/css/upload.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/static/geomanager/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/css/vendor/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.336428 geomanager-0.0.4/geomanager/static/geomanager/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/images/geomapviewer-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.336428 geomanager-0.0.4/geomanager/static/geomanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/add-multiple.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/colorbrewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/mbt_source_extra.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/raster-preview.js
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/raster_style_extra.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vector-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.336428 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/d3-format.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   745424 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)   542509 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/ol.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/static/geomanager/js/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/widgets/icon_chooser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/widgets/raster_style_widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/wms-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/templates/admin/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/admin/geomanager/layerrasterfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/django_nextjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/django_nextjs/mapviewer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/raster_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/raster_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/raster_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/stations_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/stations_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/vector_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/vector_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/vector_upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/geomanager/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/widgets/raster_style_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/wms_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/modeladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/modeladmin/index_without_custom_create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templatetags/geomanager_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/raster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.344429 geomanager-0.0.4/geomanager/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/nextjs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.344429 geomanager-0.0.4/geomanager/viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.328428 geomanager-0.0.4/geomanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 09:19:56.000000 geomanager-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 09:20:17.344429 geomanager-0.0.4/setup.cfg
```

### Comparing `geomanager-0.0.3/PKG-INFO` & `geomanager-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wagtail based Geospatial Data Manager
 Home-page: https://github.com/wmo-raf/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `geomanager-0.0.3/README.md` & `geomanager-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/apps.py` & `geomanager-0.0.4/geomanager/apps.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/blocks.py` & `geomanager-0.0.4/geomanager/blocks.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/constants.py` & `geomanager-0.0.4/geomanager/constants.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/errors.py` & `geomanager-0.0.4/geomanager/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,7 +70,15 @@
 
 class GeostoreNotFound(Error):
     pass
 
 
 class QueryParamRequired(Error):
     pass
+
+
+class InvalidGeomType(Error):
+    pass
+
+
+class GeomValidationNotImplemented(Error):
+    pass
```

### Comparing `geomanager-0.0.3/geomanager/fields.py` & `geomanager-0.0.4/geomanager/fields.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/forms.py` & `geomanager-0.0.4/geomanager/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -128,7 +128,32 @@
         fields = "__all__"
 
 
 class AoiForm(ModelForm):
     class Meta:
         model = AreaOfInterest
         fields = "__all__"
+
+
+class StationsUploadForm(forms.Form):
+    shp_zip = forms.FileField(required=True, label=_("Stations Shapefile ZIP"),
+                              widget=forms.FileInput(attrs={'accept': '.zip'}))
+
+
+class StationColumnsForm(forms.Form):
+    columns = forms.JSONField(required=False, widget=forms.HiddenInput)
+    name_column = forms.ChoiceField(required=False, label=_("Station name field"))
+
+    def __init__(self, *args, **kwargs):
+        column_choices = None
+        if "column_choices" in kwargs:
+            column_choices = kwargs.get("column_choices")
+            kwargs.pop("column_choices")
+
+        super().__init__(*args, **kwargs)
+
+        if column_choices:
+            choices = [("", "--------")]
+            choices.extend(column_choices)
+            self.fields['name_column'].choices = choices
+        else:
+            self.fields['name_column'].widget = forms.HiddenInput()
```

### Comparing `geomanager-0.0.3/geomanager/helpers.py` & `geomanager-0.0.4/geomanager/helpers.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/migrations/0001_initial.py` & `geomanager-0.0.4/geomanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/migrations/0002_geomanagersettings_logo_and_more.py` & `geomanager-0.0.4/geomanager/migrations/0002_geomanagersettings_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py` & `geomanager-0.0.4/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/migrations/0004_alter_dataset_can_clip.py` & `geomanager-0.0.4/geomanager/migrations/0004_alter_dataset_can_clip.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/migrations/0005_delete_countryboundary_and_more.py` & `geomanager-0.0.4/geomanager/migrations/0005_delete_countryboundary_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/models/__init__.py` & `geomanager-0.0.4/geomanager/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .core import *
 from .raster import *
 from .tile_gl import *
 from .vector import *
 from .profile import *
 from .aoi import *
+from .stations import *
 
 logger = logging.getLogger(__name__)
 
 
 # clear wagtail cache on saving the following models
 @receiver(post_save, sender=Category)
 @receiver(post_save, sender=SubCategory)
```

### Comparing `geomanager-0.0.3/geomanager/models/aoi.py` & `geomanager-0.0.4/geomanager/models/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/models/core.py` & `geomanager-0.0.4/geomanager/models/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/models/profile.py` & `geomanager-0.0.4/geomanager/models/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/models/raster.py` & `geomanager-0.0.4/geomanager/models/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/models/tile_gl.py` & `geomanager-0.0.4/geomanager/models/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/models/vector.py` & `geomanager-0.0.4/geomanager/models/vector.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/samples/basemaps/basemaps.json` & `geomanager-0.0.4/geomanager/samples/basemaps/basemaps.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/samples/basemaps/style.json` & `geomanager-0.0.4/geomanager/samples/basemaps/style.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/serializers/aoi.py` & `geomanager-0.0.4/geomanager/serializers/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/serializers/auth.py` & `geomanager-0.0.4/geomanager/serializers/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/serializers/core.py` & `geomanager-0.0.4/geomanager/serializers/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/serializers/profile.py` & `geomanager-0.0.4/geomanager/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/serializers/raster.py` & `geomanager-0.0.4/geomanager/serializers/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/serializers/vector.py` & `geomanager-0.0.4/geomanager/serializers/vector.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/css/vendor/maplibre-gl.css` & `geomanager-0.0.4/geomanager/static/geomanager/css/vendor/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/images/geomapviewer-logo.png` & `geomanager-0.0.4/geomanager/static/geomanager/images/geomapviewer-logo.png`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/add-multiple.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/colorbrewer.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/colorbrewer.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/mbt_source_extra.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/mbt_source_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/raster-preview.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/raster-preview.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -165,19 +165,17 @@
                 style = {
                     "bands": [{
                         "band": 1,
                         "palette": selectedColorScale
                     }]
                 }
                 style = JSON.stringify(style)
-                console.log(style)
-
             }
             const params = {
-                style: JSON.stringify(style)
+                style: style
             }
             updateSourceTileUrl(map, sourceId, params)
         }
     };
 
     const setColorMaps = async () => {
         const colorMaps = await fetchColorMaps()
```

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/raster_style_extra.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/raster_style_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/vector-preview.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/vector-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/vendor/d3-format.min.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/vendor/d3-format.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/vendor/maplibre-gl.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/vendor/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/vendor/ol.min.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/vendor/ol.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/widgets/icon_chooser.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/widgets/icon_chooser.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/widgets/raster_style_widget.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/widgets/raster_style_widget.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/static/geomanager/js/wms-preview.js` & `geomanager-0.0.4/geomanager/static/geomanager/js/wms-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/django_nextjs/mapviewer.html` & `geomanager-0.0.4/geomanager/templates/django_nextjs/mapviewer.html`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
         .navbar-logo {
             height: 100%;
             max-width: 300px;
             min-width: 200px;
         }
 
+        .navbar-brand {
+            height: 100%;
+            width: 100%;
+        }
+
         .navbar-item {
             padding: 0 10px;
             margin: 0 5px;
             cursor: pointer;
             color: rgb(85, 85, 85);
             font-size: 14px;
             text-transform: uppercase;
```

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/raster_edit_form.html` & `geomanager-0.0.4/geomanager/templates/geomanager/raster_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/raster_preview.html` & `geomanager-0.0.4/geomanager/templates/geomanager/raster_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/raster_upload.html` & `geomanager-0.0.4/geomanager/templates/geomanager/raster_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/vector_edit_form.html` & `geomanager-0.0.4/geomanager/templates/geomanager/vector_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/vector_preview.html` & `geomanager-0.0.4/geomanager/templates/geomanager/vector_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/vector_upload.html` & `geomanager-0.0.4/geomanager/templates/geomanager/vector_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/widgets/raster_style_widget.html` & `geomanager-0.0.4/geomanager/templates/geomanager/widgets/raster_style_widget.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/geomanager/wms_preview.html` & `geomanager-0.0.4/geomanager/templates/geomanager/wms_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/templates/modeladmin/index_without_custom_create.html` & `geomanager-0.0.4/geomanager/templates/modeladmin/index_without_custom_create.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/urls.py` & `geomanager-0.0.4/geomanager/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.urls import include, path
-from django.views.decorators.cache import cache_page
 from rest_framework.routers import SimpleRouter
 from rest_framework_simplejwt.views import (
     TokenRefreshView, )
 
 from geomanager.views import (
     RasterTileView,
     VectorTileView,
@@ -26,14 +25,15 @@
 )
 from geomanager.views.raster import (
     RasterDataPixelView,
     RasterDataPixelTimeseriesView,
     RasterDataGeostoreView,
     RasterDataGeostoreTimeseriesView
 )
+from geomanager.views.stations import StationsTileView
 from geomanager.viewsets import (
     FileImageLayerRasterFileDetailViewSet,
     VectorTableFileDetailViewSet,
     DatasetListViewSet,
     GeostoreViewSet,
     AdminBoundaryViewSet,
     MetadataViewSet
@@ -98,28 +98,28 @@
                        name="get_by_gid1"),
                   path(r'api/geostore/admin/<str:gid_0>/<str:gid_1>/<str:gid_2>',
                        GeostoreViewSet.as_view({"get": "get_by_admin"}),
                        name="get_by_gid2"),
 
                   # Tiles
                   path(r'api/raster-tiles/<int:z>/<int:x>/<int:y>', RasterTileView.as_view(), name="raster_tiles"),
-                  path(r'api/vector-tiles/<int:z>/<int:x>/<int:y>', cache_page(3600)(VectorTileView.as_view()),
-                       name="vector_tiles"),
+                  path(r'api/vector-tiles/<int:z>/<int:x>/<int:y>', VectorTileView.as_view(), name="vector_tiles"),
+                  path(r'api/station-tiles/<int:z>/<int:x>/<int:y>', StationsTileView.as_view(), name="station_tiles"),
 
                   # Data
                   path(r'api/raster-data/pixel', RasterDataPixelView.as_view(), name="raster_data_pixel"),
                   path(r'api/raster-data/pixel/timeseries', RasterDataPixelTimeseriesView.as_view(),
                        name="raster_data_pixel_timeseries"),
 
                   path(r'api/raster-data/geostore', RasterDataGeostoreView.as_view(), name="raster_data_geostore"),
                   path(r'api/raster-data/geostore/timeseries', RasterDataGeostoreTimeseriesView.as_view(),
                        name="raster_data_geostore_timeseries"),
 
                   # FeatureServ
-                  path(r'api/feature-serv/<str:table_name>.geojson', cache_page(3600)(GeoJSONPgTableView.as_view()),
+                  path(r'api/feature-serv/<str:table_name>.geojson', GeoJSONPgTableView.as_view(),
                        name="feature_serv"),
 
                   # Tiles GL
                   path(r'api/tile-gl/tile/<str:source_slug>/<int:z>/<int:x>/<int:y>.pbf', tile_gl, name="tile_gl"),
                   path(r'api/tile-gl/tile-json/<str:source_slug>.json', tile_json_gl, name="tile_json_gl"),
                   path(r'api/tile-gl/style/<str:source_slug>.json', style_json_gl, name="style_json_gl"),
```

### Comparing `geomanager-0.0.3/geomanager/utils/raster_utils.py` & `geomanager-0.0.4/geomanager/utils/raster_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,14 @@
 
             # delete 'NETCDF_*' attributes
             for nc_attr in netcdf_attrs:
                 rds.attrs.pop(nc_attr)
 
             rds.rio.to_raster(out_file_path, driver="COG", compress="DEFLATE")
         except Exception as e:
-            print(e)
             raise e
         finally:
             rds.close()
 
         return True
 
     # handle geotiff
```

### Comparing `geomanager-0.0.3/geomanager/utils/tile_gl.py` & `geomanager-0.0.4/geomanager/utils/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/views/__init__.py` & `geomanager-0.0.4/geomanager/views/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,7 +17,9 @@
     upload_vector_file,
     publish_vector,
     delete_vector_upload,
     preview_vector_layers,
     VectorTileView,
     GeoJSONPgTableView
 )
+
+from .stations import load_stations, preview_stations
```

### Comparing `geomanager-0.0.3/geomanager/views/auth.py` & `geomanager-0.0.4/geomanager/views/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/views/core.py` & `geomanager-0.0.4/geomanager/views/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/views/nextjs.py` & `geomanager-0.0.4/geomanager/views/nextjs.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/views/profile.py` & `geomanager-0.0.4/geomanager/views/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/views/raster.py` & `geomanager-0.0.4/geomanager/views/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,16 @@
 
         if style:
             # explict request to use layer defined style. Mostly used for admin previews
             if style == "layer-style":
                 layer_style = raster_file.layer.style
                 if layer_style:
                     style = layer_style.get_style_as_json()
+                else:
+                    style = None
             else:
                 # try validating style
                 # TODO: do more thorough validation
                 try:
                     style = json.loads(style)
                 except Exception:
                     style = None
```

### Comparing `geomanager-0.0.3/geomanager/views/tile_gl.py` & `geomanager-0.0.4/geomanager/views/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/views/vector.py` & `geomanager-0.0.4/geomanager/views/vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,17 @@
             tile = cursor.fetchone()[0]
             if not len(tile):
                 raise Http404()
 
         return HttpResponse(tile, content_type="application/x-protobuf")
 
 
+
+
+
 @method_decorator(cache_page, name='get')
 class GeoJSONPgTableView(View):
     def get(self, request, table_name):
         try:
             vector_table = PgVectorTable.objects.get(table_name=table_name)
         except ObjectDoesNotExist:
             return JsonResponse({"message": f"Table with name: '{table_name}' does not exist"}, status=404)
```

### Comparing `geomanager-0.0.3/geomanager/viewsets/aoi.py` & `geomanager-0.0.4/geomanager/viewsets/aoi.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 
     def create(self, request, *args, **kwargs):
         request.data.update({"user": request.user.id})
 
         return super().create(request, *args, **kwargs)
 
     def update(self, request, *args, **kwargs):
-        print(kwargs)
         return super().update(request, *args, **kwargs)
```

### Comparing `geomanager-0.0.3/geomanager/viewsets/core.py` & `geomanager-0.0.4/geomanager/viewsets/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/viewsets/raster.py` & `geomanager-0.0.4/geomanager/viewsets/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/viewsets/vector.py` & `geomanager-0.0.4/geomanager/viewsets/vector.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/geomanager/wagtail_hooks.py` & `geomanager-0.0.4/geomanager/wagtail_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     publish_raster,
     delete_raster_upload,
     preview_raster_layers,
     upload_vector_file,
     publish_vector,
     delete_vector_upload,
     preview_vector_layers,
-    preview_wms_layers
+    preview_wms_layers,
+    load_stations,
+    preview_stations
 )
 
 
 @hooks.register('register_admin_urls')
 def urlconf_geomanager():
     return [
         path('upload-rasters/', upload_raster_file, name='geomanager_upload_rasters'),
@@ -63,14 +65,17 @@
         path('preview-vector-layers/<uuid:dataset_id>/<uuid:layer_id>/', preview_vector_layers,
              name='geomanager_preview_vector_layer'),
 
         path('preview-wms-layers/<uuid:dataset_id>/', preview_wms_layers,
              name='geomanager_preview_wms_dataset'),
         path('preview-wms-layers/<uuid:dataset_id>/<uuid:layer_id>/', preview_wms_layers,
              name='geomanager_preview_wms_layer'),
+
+        path('load-stations/', load_stations, name='geomanager_load_stations'),
+        path('preview-stations/', preview_stations, name='geomanager_preview_stations'),
     ]
 
 
 class ModelAdminCanHide(ModelAdmin):
     hidden = False
 
 
@@ -602,14 +607,18 @@
         except Exception:
             pass
 
         boundary_loader = MenuItem(label=_("Boundary Data"), url=reverse("adminboundarymanager_preview_boundary"),
                                    icon_name="map")
         menu_items.append(boundary_loader)
 
+        stations_data = MenuItem(label=_("Stations Data"), url=reverse("geomanager_preview_stations"),
+                                 icon_name="map")
+        menu_items.append(stations_data)
+
         try:
             settings_url = reverse(
                 "wagtailsettings:edit",
                 args=[GeomanagerSettings._meta.app_label, GeomanagerSettings._meta.model_name, ],
             )
             gm_settings_menu = MenuItem(label=_("Settings"), url=settings_url, icon_name="cog")
             menu_items.append(gm_settings_menu)
@@ -627,7 +636,13 @@
     return icons + [
         'wagtailfontawesomesvg/solid/palette.svg',
         'wagtailfontawesomesvg/solid/database.svg',
         'wagtailfontawesomesvg/solid/layer-group.svg',
         'wagtailfontawesomesvg/solid/globe-africa.svg',
         'wagtailfontawesomesvg/solid/map.svg',
     ]
+
+
+@hooks.register('construct_settings_menu')
+def hide_settings_menu_item(request, menu_items):
+    hidden_settings = ["admin-boundary-settings", "geomanager-settings"]
+    menu_items[:] = [item for item in menu_items if item.name not in hidden_settings]
```

### Comparing `geomanager-0.0.3/geomanager.egg-info/PKG-INFO` & `geomanager-0.0.4/geomanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wagtail based Geospatial Data Manager
 Home-page: https://github.com/wmo-raf/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `geomanager-0.0.3/geomanager.egg-info/SOURCES.txt` & `geomanager-0.0.4/geomanager.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,20 +23,26 @@
 geomanager.egg-info/requires.txt
 geomanager.egg-info/top_level.txt
 geomanager/migrations/0001_initial.py
 geomanager/migrations/0002_geomanagersettings_logo_and_more.py
 geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
 geomanager/migrations/0004_alter_dataset_can_clip.py
 geomanager/migrations/0005_delete_countryboundary_and_more.py
+geomanager/migrations/0006_stationsettings.py
+geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
+geomanager/migrations/0008_stationsettings_name_column.py
+geomanager/migrations/0009_stationsettings_popup_props.py
+geomanager/migrations/0010_remove_stationsettings_popup_props.py
 geomanager/migrations/__init__.py
 geomanager/models/__init__.py
 geomanager/models/aoi.py
 geomanager/models/core.py
 geomanager/models/profile.py
 geomanager/models/raster.py
+geomanager/models/stations.py
 geomanager/models/tile_gl.py
 geomanager/models/vector.py
 geomanager/samples/basemaps/basemaps.json
 geomanager/samples/basemaps/style.json
 geomanager/serializers/__init__.py
 geomanager/serializers/aoi.py
 geomanager/serializers/auth.py
@@ -62,30 +68,35 @@
 geomanager/static/geomanager/js/widgets/icon_chooser.js
 geomanager/static/geomanager/js/widgets/raster_style_widget.js
 geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
 geomanager/templates/django_nextjs/mapviewer.html
 geomanager/templates/geomanager/raster_edit_form.html
 geomanager/templates/geomanager/raster_preview.html
 geomanager/templates/geomanager/raster_upload.html
+geomanager/templates/geomanager/stations_preview.html
+geomanager/templates/geomanager/stations_upload.html
 geomanager/templates/geomanager/vector_edit_form.html
 geomanager/templates/geomanager/vector_preview.html
 geomanager/templates/geomanager/vector_upload.html
 geomanager/templates/geomanager/wms_preview.html
 geomanager/templates/geomanager/widgets/raster_style_widget.html
 geomanager/templates/modeladmin/index_without_custom_create.html
+geomanager/templatetags/__init__.py
+geomanager/templatetags/geomanager_tags.py
 geomanager/utils/__init__.py
 geomanager/utils/raster_utils.py
 geomanager/utils/tile_gl.py
 geomanager/utils/vector_utils.py
 geomanager/views/__init__.py
 geomanager/views/auth.py
 geomanager/views/core.py
 geomanager/views/nextjs.py
 geomanager/views/profile.py
 geomanager/views/raster.py
+geomanager/views/stations.py
 geomanager/views/tile_gl.py
 geomanager/views/vector.py
 geomanager/viewsets/__init__.py
 geomanager/viewsets/aoi.py
 geomanager/viewsets/core.py
 geomanager/viewsets/raster.py
 geomanager/viewsets/vector.py
```

### Comparing `geomanager-0.0.3/geomanager.egg-info/requires.txt` & `geomanager-0.0.4/geomanager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.3/setup.cfg` & `geomanager-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geomanager
-version = 0.0.3
+version = 0.0.4
 description = Wagtail based Geospatial Data Manager
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/geomanager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

