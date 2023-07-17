# Comparing `tmp/shapelets-platform-2.0.87.tar.gz` & `tmp/shapelets-platform-2.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.87.tar", last modified: Thu Jul 13 12:29:39 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.88.tar", last modified: Mon Jul 17 08:29:50 2023, max compression
```

## Comparing `shapelets-platform-2.0.87.tar` & `shapelets-platform-2.0.88.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.087065 shapelets-platform-2.0.87/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-13 12:29:39.087065 shapelets-platform-2.0.87/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     3069 2023-07-13 12:29:39.087065 shapelets-platform-2.0.87/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.971064 shapelets-platform-2.0.87/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.979064 shapelets-platform-2.0.87/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    51403 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-07-13 12:29:35.000000 shapelets-platform-2.0.87/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.983064 shapelets-platform-2.0.87/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    68871 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.983064 shapelets-platform-2.0.87/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.991064 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19053 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.991064 shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.003064 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1996 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4503 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7578 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8196 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/gauge.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5978 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/metric.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9880 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.003064 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/ring.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14789 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.007064 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6057 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5683 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26073 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/iris.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.015064 shapelets-platform-2.0.87/src/shapelets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/altair.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/capsule.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/collection.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/function_description.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/function_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/group.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/metadata_item.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/ndarray.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/replicated_param.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/sequence.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/sequence_axis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/user.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/model/view_match.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.015064 shapelets-platform-2.0.87/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.019064 shapelets-platform-2.0.87/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.019064 shapelets-platform-2.0.87/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.027064 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.031064 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9536 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2407 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.031064 shapelets-platform-2.0.87/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.035065 shapelets-platform-2.0.87/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v4.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.039065 shapelets-platform-2.0.87/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.039065 shapelets-platform-2.0.87/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4392 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4951 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.043064 shapelets-platform-2.0.87/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.051065 shapelets-platform-2.0.87/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.051065 shapelets-platform-2.0.87/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.059065 shapelets-platform-2.0.87/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.059065 shapelets-platform-2.0.87/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.063065 shapelets-platform-2.0.87/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.067065 shapelets-platform-2.0.87/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.067065 shapelets-platform-2.0.87/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/custom_sample.js
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:38.971064 shapelets-platform-2.0.87/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.067065 shapelets-platform-2.0.87/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.079065 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-07-13 12:29:34.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-07-13 12:29:34.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.083065 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-07-13 12:29:33.000000 shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-07-13 12:07:59.000000 shapelets-platform-2.0.87/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 12:29:39.087065 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-13 12:29:35.000000 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11445 2023-07-13 12:29:38.000000 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-13 12:29:35.000000 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-07-13 12:29:35.000000 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1306 2023-07-13 12:29:35.000000 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-07-13 12:29:35.000000 shapelets-platform-2.0.87/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.683736 shapelets-platform-2.0.88/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-17 08:29:50.683736 shapelets-platform-2.0.88/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     3069 2023-07-17 08:29:50.683736 shapelets-platform-2.0.88/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.583734 shapelets-platform-2.0.88/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.587734 shapelets-platform-2.0.88/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    51403 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-07-17 08:29:47.000000 shapelets-platform-2.0.88/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.591734 shapelets-platform-2.0.88/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    68871 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.591734 shapelets-platform-2.0.88/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.595734 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19053 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.599734 shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.607734 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1996 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4503 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7578 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8196 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/gauge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5978 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/metric.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9880 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.607734 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/ring.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14789 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.607734 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6057 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5683 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/iris.csv
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.615734 shapelets-platform-2.0.88/src/shapelets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/altair.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/capsule.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/function_description.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/function_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/group.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/metadata_item.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/ndarray.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/replicated_param.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/sequence.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/sequence_axis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/user.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/model/view_match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.619735 shapelets-platform-2.0.88/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.619735 shapelets-platform-2.0.88/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.619735 shapelets-platform-2.0.88/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.623735 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.627735 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9536 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2407 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.635735 shapelets-platform-2.0.88/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.635735 shapelets-platform-2.0.88/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v4.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.635735 shapelets-platform-2.0.88/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.639735 shapelets-platform-2.0.88/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4392 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4951 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.639735 shapelets-platform-2.0.88/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.647735 shapelets-platform-2.0.88/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.647735 shapelets-platform-2.0.88/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.655735 shapelets-platform-2.0.88/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.655735 shapelets-platform-2.0.88/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.659736 shapelets-platform-2.0.88/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.659736 shapelets-platform-2.0.88/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.663735 shapelets-platform-2.0.88/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/custom_sample.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.583734 shapelets-platform-2.0.88/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.663735 shapelets-platform-2.0.88/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.671736 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-07-17 08:29:46.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.679736 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-07-17 08:29:41.000000 shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-07-17 08:11:48.000000 shapelets-platform-2.0.88/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 08:29:50.683736 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-17 08:29:47.000000 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11445 2023-07-17 08:29:50.000000 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-17 08:29:47.000000 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-07-17 08:29:47.000000 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1306 2023-07-17 08:29:47.000000 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-07-17 08:29:47.000000 shapelets-platform-2.0.88/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.87/LICENSE.md` & `shapelets-platform-2.0.88/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/PKG-INFO` & `shapelets-platform-2.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.87
+Version: 2.0.88
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.87/README.md` & `shapelets-platform-2.0.88/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/noxfile.py` & `shapelets-platform-2.0.88/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/pyproject.toml` & `shapelets-platform-2.0.88/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/setup.cfg` & `shapelets-platform-2.0.88/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 	pyarrow >=12.0.0
 	py-cpuinfo>=9.0.0
 	pydantic == 1.10.11
 	pygeohash >= 1.2.0
 	PyNaCl >= 1.5.0
 	requests >= 2.28.1
 	setuptools-scm >= 7.1.0
-	shapelets_native == 2.0.87
+	shapelets_native == 2.0.88
 	tabulate>=0.8.10
 	tomlkit >= 0.11.4
 	tqdm >= 4.64.1
 	typing_extensions >= 4.6.2
 	uvicorn >= 0.18.3
 	vega-datasets >= 0.9
 	websocket-client >= 1.5.2
```

### Comparing `shapelets-platform-2.0.87/setup.py` & `shapelets-platform-2.0.88/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/_api.py` & `shapelets-platform-2.0.88/src/shapelets/_api.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/_cli.py` & `shapelets-platform-2.0.88/src/shapelets/_cli.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/_relations.py` & `shapelets-platform-2.0.88/src/shapelets/_relations.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/_uom.py` & `shapelets-platform-2.0.88/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.88/src/shapelets/apps/data_app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.88/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/attribute_names.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/button.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/gauge.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/gauge.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/metric.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/metric.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/ring.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/ring.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/sequence_list.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/sequence_list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/table.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/table.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/panel.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/util.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.88/src/shapelets/apps/widgets/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import __main__
 import sys
 
 import os
 
 SH_DIR = os.path.expanduser('~/.shapelets')
 DATA_DIR = os.path.join(SH_DIR, 'data')
+if not os.path.exists(DATA_DIR):
+    os.makedirs(DATA_DIR)
 
 
 class Widget:
     """
     Units defined in Layout
     """
 
@@ -276,15 +278,16 @@
 
             # Function are saved  with a unique id, so the function won't be replaced when it is used multiple times.
             # This is because when a basic type is returned like str or int, the return value will only change the
             # value of the widget, but we want to keep the other widget attributes like the title.
             # If we don't use unique functions for each widget, we won't be able to keep the other attributes.
             fn_uid = str(uuid.uuid1())
             # Add to Widget Structure
-            self._add_bind_to_widget(fn=fn_uid, result=self._parent_class, parameters=references, triggers=on_changes_widgets)
+            self._add_bind_to_widget(fn=fn_uid, result=self._parent_class,
+                                     parameters=references, triggers=on_changes_widgets)
             # Serialize function and save it to file.
             ser_body = base64.b64encode(zlib.compress(dill.dumps(body, recurse=True))).decode('utf-8')
             with open(os.path.join(DATA_DIR, fn_uid), 'wt') as f:
                 f.write(ser_body)
             result = {
                 "body": fn_uid,
                 "parameters": entry_arguments,
```

### Comparing `shapelets-platform-2.0.87/src/shapelets/functions.py` & `shapelets-platform-2.0.88/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/iris.csv` & `shapelets-platform-2.0.88/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/model/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/altair.py` & `shapelets-platform-2.0.88/src/shapelets/model/altair.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/capsule.py` & `shapelets-platform-2.0.88/src/shapelets/model/capsule.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/collection.py` & `shapelets-platform-2.0.88/src/shapelets/model/collection.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/dataframe.py` & `shapelets-platform-2.0.88/src/shapelets/model/dataframe.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/function_description.py` & `shapelets-platform-2.0.88/src/shapelets/model/function_description.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/function_parameter.py` & `shapelets-platform-2.0.88/src/shapelets/model/function_parameter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/group.py` & `shapelets-platform-2.0.88/src/shapelets/model/group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/image.py` & `shapelets-platform-2.0.88/src/shapelets/model/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/metadata_item.py` & `shapelets-platform-2.0.88/src/shapelets/model/metadata_item.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/model.py` & `shapelets-platform-2.0.88/src/shapelets/model/model.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/ndarray.py` & `shapelets-platform-2.0.88/src/shapelets/model/ndarray.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/permissions.py` & `shapelets-platform-2.0.88/src/shapelets/model/permissions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/replicated_param.py` & `shapelets-platform-2.0.88/src/shapelets/model/replicated_param.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/sequence.py` & `shapelets-platform-2.0.88/src/shapelets/model/sequence.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/sequence_axis.py` & `shapelets-platform-2.0.88/src/shapelets/model/sequence_axis.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/user.py` & `shapelets-platform-2.0.88/src/shapelets/model/user.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/model/view_match.py` & `shapelets-platform-2.0.88/src/shapelets/model/view_match.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/app.py` & `shapelets-platform-2.0.88/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/authhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/authrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/authservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/iauthrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/authn/iauthservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.88/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataappshttp.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataappshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataappsrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/schema_v4.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/schema_v4.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.88/src/shapelets/svr/db/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.88/src/shapelets/svr/execution/executionhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/execution/executionservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/execution/executionservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.88/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/groups/groupservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.88/src/shapelets/svr/groups/groupshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/groups/groupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/groups/igroupsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.88/src/shapelets/svr/model/dataapps.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.88/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.88/src/shapelets/svr/model/users.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.88/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/server.py` & `shapelets-platform-2.0.88/src/shapelets/svr/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.88/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/iusersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/iusersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/usershttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/usersrepo.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/usersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/users/usersservice.py` & `shapelets-platform-2.0.88/src/shapelets/svr/users/usersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.88/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.88/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.88/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.88/src/shapelets/svr/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.88/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.88/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.88/src/shapelets/svr/www/index.html`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/2.379683b2.chunk.js` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/2.379683b2.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.88/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.88/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.87
+Version: 2.0.88
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.87/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.88/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.87/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.88/src/shapelets_platform.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pyarrow>=12.0.0
 py-cpuinfo>=9.0.0
 pydantic==1.10.11
 pygeohash>=1.2.0
 PyNaCl>=1.5.0
 requests>=2.28.1
 setuptools-scm>=7.1.0
-shapelets_native==2.0.87
+shapelets_native==2.0.88
 tabulate>=0.8.10
 tomlkit>=0.11.4
 tqdm>=4.64.1
 typing_extensions>=4.6.2
 uvicorn>=0.18.3
 vega-datasets>=0.9
 websocket-client>=1.5.2
```

