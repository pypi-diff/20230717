# Comparing `tmp/ckanext-versioned-tiledmap-2.2.0.tar.gz` & `tmp/ckanext-versioned-tiledmap-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-versioned-tiledmap-2.2.0.tar", last modified: Tue May  9 09:40:15 2023, max compression
+gzip compressed data, was "ckanext-versioned-tiledmap-2.2.1.tar", last modified: Mon Jul 17 08:29:11 2023, max compression
```

## Comparing `ckanext-versioned-tiledmap-2.2.0.tar` & `ckanext-versioned-tiledmap-2.2.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/lib/validators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/routes/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/less/maps.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/map_view.js
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/maptype_control.js
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/minimap_control.js
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.885640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.885640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/backbone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    59498 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.885640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)   248138 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)    93869 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/
--rw-r--r--   0 runner    (1001) docker     (123)   215378 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)   125495 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/
--rw-r--r--   0 runner    (1001) docker     (123)    71140 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.885640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/mustache/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/terraformer/
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    39926 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.885640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/underscore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.893640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/data/
--rw-r--r--   0 runner    (1001) docker     (123)   551530 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/data/countries.geojson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/toggle.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/map_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/map_view.html
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/point_detail.mustache
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/point_detail_hover.dwc.mustache
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/point_detail_hover.mustache
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 09:40:15.000000 ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.889640 ckanext-versioned-tiledmap-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:15.897640 ckanext-versioned-tiledmap-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/tests/test_route_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-09 09:40:04.000000 ckanext-versioned-tiledmap-2.2.0/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.455300 ckanext-versioned-tiledmap-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-17 08:29:11.455300 ckanext-versioned-tiledmap-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.435299 ckanext-versioned-tiledmap-2.2.1/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.435299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.435299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/lib/validators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.435299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/routes/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.439299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.439299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/less/maps.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.439299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/map_view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/maptype_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/minimap_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.427299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/backbone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.439299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    59498 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.427299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.443300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   248138 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    93869 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.443300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/
+-rw-r--r--   0 runner    (1001) docker     (123)   215378 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)   125495 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.443300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/
+-rw-r--r--   0 runner    (1001) docker     (123)    71140 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.443300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.443300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/mustache/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.447300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.447300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/terraformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39926 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/underscore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.447300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.447300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   551530 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/data/countries.geojson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.447300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.447300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.451300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/toggle.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.451300 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/map_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/map_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/point_detail.mustache
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/point_detail_hover.dwc.mustache
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/point_detail_hover.mustache
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.451300 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:29:11.000000 ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.431299 ckanext-versioned-tiledmap-2.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.451300 ckanext-versioned-tiledmap-2.2.1/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:29:11.455300 ckanext-versioned-tiledmap-2.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:11.455300 ckanext-versioned-tiledmap-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/tests/test_route_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-17 08:28:58.000000 ckanext-versioned-tiledmap-2.2.1/tests/test_validators.py
```

### Comparing `ckanext-versioned-tiledmap-2.2.0/LICENSE` & `ckanext-versioned-tiledmap-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/PKG-INFO` & `ckanext-versioned-tiledmap-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-tiledmap
-Version: 2.2.0
+Version: 2.2.1
 Summary: A CKAN extension with a map view for versioned-datastore backed resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_tiledmap
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-versioned-tiledmap
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-versioned-tiledmap/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-versioned-tiledmap/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-versioned-tiledmap)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-versioned-tiledmap-2.2.0/README.md` & `ckanext-versioned-tiledmap-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-versioned-tiledmap
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-versioned-tiledmap/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-versioned-tiledmap/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-versioned-tiledmap)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/config.py` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/lib/validators.py` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/lib/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/plugin.py` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/routes/_helpers.py` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/routes/_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/routes/map.py` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/routes/map.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/less/maps.less` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/less/maps.less`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/map_view.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/map_view.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/maptype_control.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/maptype_control.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/minimap_control.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/minimap_control.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/assets/webassets.yml` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/assets/webassets.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/data/countries.geojson` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/data/countries.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/map_form.html` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/map_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext/tiledmap/theme/templates/point_detail.mustache` & `ckanext-versioned-tiledmap-2.2.1/ckanext/tiledmap/theme/templates/point_detail.mustache`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/PKG-INFO` & `ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-tiledmap
-Version: 2.2.0
+Version: 2.2.1
 Summary: A CKAN extension with a map view for versioned-datastore backed resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_tiledmap
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-versioned-tiledmap
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-versioned-tiledmap/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-versioned-tiledmap/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-versioned-tiledmap)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-versioned-tiledmap-2.2.0/ckanext_versioned_tiledmap.egg-info/SOURCES.txt` & `ckanext-versioned-tiledmap-2.2.1/ckanext_versioned_tiledmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/docs/_scripts/gen_api_pages.py` & `ckanext-versioned-tiledmap-2.2.1/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/pyproject.toml` & `ckanext-versioned-tiledmap-2.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-versioned-tiledmap"
-version = "2.2.0"
+version = "2.2.1"
 description = "A CKAN extension with a map view for versioned-datastore backed resources."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.tiledmap.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.0"
+version = "2.2.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-versioned-tiledmap-2.2.0/tests/test_route_helpers.py` & `ckanext-versioned-tiledmap-2.2.1/tests/test_route_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/tests/test_utils.py` & `ckanext-versioned-tiledmap-2.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.2.0/tests/test_validators.py` & `ckanext-versioned-tiledmap-2.2.1/tests/test_validators.py`

 * *Files identical despite different names*

