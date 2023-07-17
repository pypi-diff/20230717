# Comparing `tmp/open-cravat-2.4.0.tar.gz` & `tmp/open-cravat-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-cravat-2.4.0.tar", last modified: Thu Jul  6 17:45:27 2023, max compression
+gzip compressed data, was "open-cravat-2.4.1.tar", last modified: Mon Jul 17 19:49:54 2023, max compression
```

## Comparing `open-cravat-2.4.0.tar` & `open-cravat-2.4.1.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.258769 open-cravat-2.4.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1067 2023-07-06 17:45:27.000000 open-cravat-2.4.0/LICENSE
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-07-06 17:45:27.258769 open-cravat-2.4.0/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)      769 2023-07-06 17:45:27.000000 open-cravat-2.4.0/README.rst
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.228769 open-cravat-2.4.0/cravat/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6364 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    60556 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/admin_util.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19600 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/aggregator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2990 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/annotator_options.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.228769 open-cravat-2.4.0/cravat/annotator_template/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      178 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/annotator_template/annotator_template.md
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2326 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/annotator_template/annotator_template.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1460 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/annotator_template/annotator_template.yml
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.228769 open-cravat-2.4.0/cravat/annotator_template/data/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/annotator_template/data/annotator_template.sqlite
--rw-r--r--   0 kyle      (1000) kyle      (1000)    28521 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/base_annotator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2074 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/base_commonmodule.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1259 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/base_converter.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16953 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/base_mapper.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12209 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/base_postaggregator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20758 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/base_summarizer.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5266 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/config_loader.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12114 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/constants.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      475 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat-system.template.yml
--rw-r--r--   0 kyle      (1000) kyle      (1000)       80 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat.yml
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32368 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_admin.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    85512 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_class.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    31453 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_convert.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    38094 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_filter.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6424 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_metrics.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1969 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_pack.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    51336 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_report.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32133 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_test.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    56209 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_util.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20271 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/cravat_web.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9036 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/example_input
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1245 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/exceptions.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19368 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/inout.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.229769 open-cravat-2.4.0/cravat/liftover/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   931825 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/liftover/hg18ToHg38.over.chain
--rw-r--r--   0 kyle      (1000) kyle      (1000)   606773 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/liftover/hg19ToHg38.over.chain
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2992 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/mp_runners.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/oc.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      295 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/runcravat.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10553 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/store_utils.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10935 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/util.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.230769 open-cravat-2.4.0/cravat/webresult/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16774 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/cravat_view.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.230769 open-cravat-2.4.0/cravat/webresult/css/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2389 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/css/pqselect.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/favicon.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.231769 open-cravat-2.4.0/cravat/webresult/fonts/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26456 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19508 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25692 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/roboto-light-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18980 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/roboto-light-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26312 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19416 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    33072 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25740 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.237769 open-cravat-2.4.0/cravat/webresult/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      350 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-90deg-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      326 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-down-right-circle-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      379 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-down-right-circle.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-down-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      311 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-left.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      312 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      815 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-spinner-static.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6792 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-spinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrow-up.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      706 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/arrows-move.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12538 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/back_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)   264317 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/bigSpinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2302 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/camera.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2140 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/camera.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      291 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/caret-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/caret-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      916 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/close-button.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3125 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/close.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2390 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/close.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1160 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/close_icon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      722 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/download-material-black.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7432 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/download-material-blue.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      263 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/download.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2066 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/download.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      378 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/download12.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      485 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/grip-vertical.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/help_16x16.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/help_icon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32137 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/loading-gif-animation.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2056 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/mail.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1211 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/menu.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      200 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/minus.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1568 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/openNewTab.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5131 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/package.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1703 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/pencil.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      805 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/pin-2.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      698 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/pin.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2219 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/pin.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2243 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/plus-circle-dotted.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/plus-circle-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      217 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/plus.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3324 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13026 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/resize.jpg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3498 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/save.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1408 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/save_new.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25171 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/search.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4645 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/sorry.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    55605 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/spinCircle.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25333 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/spinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1106 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/triangle-down.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1112 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/triangle-right.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      733 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/upload-material-black.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7573 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/upload-material-blue.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/x-lg.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      332 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/images/x.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5924 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/index.html
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.239769 open-cravat-2.4.0/cravat/webresult/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   398184 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/Chart.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9279 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/dom-to-image.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6000 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/download.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)   954164 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/graphics.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86659 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-3.2.1.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.241769 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12660 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1817 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.221769 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.241769 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   293430 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.242769 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6992 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6988 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6999 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6299 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32588 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    35997 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   520714 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    30747 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   253668 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18705 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    15548 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17342 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13847 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1340 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13171 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery.tools.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5451 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/jquery.url.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    84772 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/packery.pkgd.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.243769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11951 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)   103213 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.244769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      230 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      210 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      771 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1668 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       76 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)      216 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      201 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.245769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1169 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    76985 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.246769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      755 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      774 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      794 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      826 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      837 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      830 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      661 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      796 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      808 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      847 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      797 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      700 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1153 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      613 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)      541 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2973 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    27759 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2383 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12585 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2408 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2034 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16186 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   481365 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12765 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   242939 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1646 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1286 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)      587 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/readme.txt
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.222769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/brown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.247769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/gray/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/office/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/purple/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/red/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/tan/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.248769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/violet/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.249769 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1071 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1190 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2677 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3716 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1847 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12591 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/pqselect.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    92225 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/js/raphael-min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1530 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/jsonreporter.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.249769 open-cravat-2.4.0/cravat/webresult/nocache/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.249769 open-cravat-2.4.0/cravat/webresult/nocache/css/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1714 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/css/singlevariantpage.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20968 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/css/style.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2920 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/css/widget.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.250769 open-cravat-2.4.0/cravat/webresult/nocache/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26685 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/filter.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12851 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/infomgr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    44175 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/main.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    99662 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/setup.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7986 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/showvariant.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    35998 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/singlevariantpage.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    31708 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/util.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1688 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/variables.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20474 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/js/widgethelper.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5535 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/nocache/variant.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    30111 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/webresult.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      173 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webresult/webviewer.yml
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.251769 open-cravat-2.4.0/cravat/webstore/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1365 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/cravat_store.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/favicon.ico
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.253769 open-cravat-2.4.0/cravat/webstore/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      446 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/chat-dots-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      740 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/chat-dots.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      396 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/chat-left-text-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      545 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/chat-left-text.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    22268 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/done.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2226 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/empty.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1763 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/folder.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    38197 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/genericmodulelogo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4766 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/hamburger.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1194 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/left_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    67804 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3524 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/new.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1214 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/right_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/images/x-lg.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/jquery-3.3.1.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.254769 open-cravat-2.4.0/cravat/webstore/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    75673 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/js/showdown-1.9.1.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    91924 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/js/showdown.min.js.map
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.254769 open-cravat-2.4.0/cravat/webstore/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    15017 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/nocache/webstore.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    95532 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/nocache/webstore.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2342 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/sse.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1700 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/store_handlers.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16522 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/webstore.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      283 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/ws.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)      720 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/webstore/ws.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.256769 open-cravat-2.4.0/cravat/websubmit/
--rw-r--r--   0 kyle      (1000) kyle      (1000)       11 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/.gitignore
--rw-r--r--   0 kyle      (1000) kyle      (1000)   210024 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/Chart.bundle.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      719 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2291 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/down.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      108 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/googleAnalytics.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1052 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/help.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.257769 open-cravat-2.4.0/cravat/websubmit/input-examples/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      527 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/input-examples/cravat.hg18.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/input-examples/cravat.hg19.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/input-examples/cravat.hg38.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/input-examples/vcf.hg18.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/input-examples/vcf.hg19.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/input-examples/vcf.hg38.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/jquery-3.3.1.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    53784 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    56098 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/logo_transparent.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      225 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/menu.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.257769 open-cravat-2.4.0/cravat/websubmit/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13800 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/nocache/broken_wheel.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18796 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/nocache/index.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17372 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/nocache/websubmit.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    83472 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/nocache/websubmit.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11488 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/nointernet.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    27869 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/pqselect.dev.customforsubmit.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2167 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/refresh.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/threedots.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    48552 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/websubmit/websubmit.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3724 2023-07-06 17:45:27.000000 open-cravat-2.4.0/cravat/wincravat.pyw
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.258769 open-cravat-2.4.0/open_cravat.egg-info/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-07-06 17:45:27.000000 open-cravat-2.4.0/open_cravat.egg-info/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12287 2023-07-06 17:45:27.000000 open-cravat-2.4.0/open_cravat.egg-info/SOURCES.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2023-07-06 17:45:27.000000 open-cravat-2.4.0/open_cravat.egg-info/dependency_links.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-07-06 17:45:27.000000 open-cravat-2.4.0/open_cravat.egg-info/entry_points.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      184 2023-07-06 17:45:27.000000 open-cravat-2.4.0/open_cravat.egg-info/requires.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        7 2023-07-06 17:45:27.000000 open-cravat-2.4.0/open_cravat.egg-info/top_level.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-07-06 17:45:27.258769 open-cravat-2.4.0/setup.cfg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2877 2023-07-06 17:45:27.000000 open-cravat-2.4.0/setup.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-06 17:45:27.258769 open-cravat-2.4.0/tests/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6183 2023-07-06 17:45:27.000000 open-cravat-2.4.0/tests/test_admin_util.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.373078 open-cravat-2.4.1/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1067 2023-07-17 19:49:54.000000 open-cravat-2.4.1/LICENSE
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-07-17 19:49:54.373078 open-cravat-2.4.1/PKG-INFO
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      769 2023-07-17 19:49:54.000000 open-cravat-2.4.1/README.rst
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.350079 open-cravat-2.4.1/cravat/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6364 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    60556 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/admin_util.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19600 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/aggregator.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2990 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/annotator_options.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.350079 open-cravat-2.4.1/cravat/annotator_template/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      178 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/annotator_template/annotator_template.md
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2326 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/annotator_template/annotator_template.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1460 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/annotator_template/annotator_template.yml
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.350079 open-cravat-2.4.1/cravat/annotator_template/data/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/annotator_template/data/annotator_template.sqlite
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    28521 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/base_annotator.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2074 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/base_commonmodule.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1259 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/base_converter.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    17199 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/base_mapper.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12209 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/base_postaggregator.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20758 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/base_summarizer.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5266 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/config_loader.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12114 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/constants.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      475 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat-system.template.yml
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       80 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat.yml
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32368 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_admin.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    85512 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_class.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    31453 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_convert.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    38094 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_filter.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6424 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_metrics.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1969 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_pack.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    51336 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_report.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32133 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_test.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    56209 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_util.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20271 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/cravat_web.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     9036 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/example_input
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1245 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/exceptions.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19368 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/inout.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.351079 open-cravat-2.4.1/cravat/liftover/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   931825 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/liftover/hg18ToHg38.over.chain
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   606773 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/liftover/hg19ToHg38.over.chain
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2992 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/mp_runners.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/oc.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      295 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/runcravat.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10553 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/store_utils.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10935 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/util.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.352079 open-cravat-2.4.1/cravat/webresult/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16774 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/cravat_view.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.352079 open-cravat-2.4.1/cravat/webresult/css/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2389 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/css/pqselect.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/email.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/favicon.ico
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/favicon.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.352079 open-cravat-2.4.1/cravat/webresult/fonts/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    26456 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19508 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25692 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/roboto-light-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    18980 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/roboto-light-webfont.woff2
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    26312 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19416 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    33072 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25740 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.357079 open-cravat-2.4.1/cravat/webresult/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      350 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-90deg-down.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      326 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      379 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-down-right-circle.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-down-right.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-down.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      311 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-left.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      312 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-right.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      815 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-spinner-static.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6792 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-spinner.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrow-up.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      706 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/arrows-move.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12538 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/back_arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   264317 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/bigSpinner.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2302 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/camera.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2140 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/camera.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      291 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/caret-down.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/caret-right.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      916 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/close-button.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3125 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/close.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2390 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/close.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1160 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/close_icon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      722 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/download-material-black.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7432 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/download-material-blue.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      263 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/download.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2066 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/download.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      378 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/download12.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      485 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/grip-vertical.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/help_16x16.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/help_icon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32137 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/loading-gif-animation.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2056 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/mail.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1211 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/menu.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      200 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/minus.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1568 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/openNewTab.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5131 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/package.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1703 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/pencil.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      805 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/pin-2.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      698 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/pin.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2219 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/pin.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2243 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/plus-circle-dotted.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/plus-circle-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      217 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/plus.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3324 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13026 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/resize.jpg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3498 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/save.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1408 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/save_new.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25171 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/search.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4645 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/sorry.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    55605 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/spinCircle.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25333 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/spinner.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1106 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/triangle-down.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1112 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/triangle-right.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      733 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/upload-material-black.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7573 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/upload-material-blue.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/x-lg.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      332 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/images/x.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5924 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/index.html
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.358079 open-cravat-2.4.1/cravat/webresult/js/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   398184 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/Chart.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     9279 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/dom-to-image.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6000 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/download.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   954164 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/graphics.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    86659 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-3.2.1.min.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.360078 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12660 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1817 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.345079 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.360078 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   293430 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.360078 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6992 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6988 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6999 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6299 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32588 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    35997 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   520714 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    30747 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   253668 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    18705 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    15548 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    17342 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13847 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1340 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13171 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery.tools.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5451 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/jquery.url.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    84772 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/packery.pkgd.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.362079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    11951 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   103213 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/EULA.pdf
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.362079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      230 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      210 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      771 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/loading.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1668 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/sprite.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       76 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      216 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      201 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.363078 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1169 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    76985 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.364079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      755 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      774 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      794 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      826 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      837 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      830 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      661 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      796 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      808 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      847 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      797 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      700 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.364079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1153 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      613 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      541 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2973 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    27759 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2383 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12585 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2408 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2034 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16186 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   481365 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12765 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   242939 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1646 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1286 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      587 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/readme.txt
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.346079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.364079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.364079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/brown/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.364079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.364079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/gray/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/office/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/purple/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/red/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/tan/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.365079 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/violet/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.366078 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1071 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1190 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2677 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3716 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1847 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12591 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/pqselect.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    92225 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/js/raphael-min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1530 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/jsonreporter.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.366078 open-cravat-2.4.1/cravat/webresult/nocache/
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.366078 open-cravat-2.4.1/cravat/webresult/nocache/css/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1714 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/css/singlevariantpage.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20968 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/css/style.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2920 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/css/widget.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.367078 open-cravat-2.4.1/cravat/webresult/nocache/js/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    26685 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/filter.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12851 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/infomgr.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    44175 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/main.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    99662 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/setup.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7986 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/showvariant.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    35998 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/singlevariantpage.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    31708 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/util.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1688 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/variables.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20474 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/js/widgethelper.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5535 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/nocache/variant.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    30111 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/webresult.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      173 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webresult/webviewer.yml
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.368079 open-cravat-2.4.1/cravat/webstore/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1365 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/cravat_store.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/favicon.ico
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.369078 open-cravat-2.4.1/cravat/webstore/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      446 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/chat-dots-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      740 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/chat-dots.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      396 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/chat-left-text-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      545 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/chat-left-text.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    22268 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/done.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/email.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2226 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/empty.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/favicon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1763 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/folder.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    38197 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/genericmodulelogo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4766 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/hamburger.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1194 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/left_arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    67804 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/logo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3524 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/new.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1214 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/right_arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/images/x-lg.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/jquery-3.3.1.min.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.369078 open-cravat-2.4.1/cravat/webstore/js/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    75673 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/js/showdown-1.9.1.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    91924 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/js/showdown.min.js.map
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.369078 open-cravat-2.4.1/cravat/webstore/nocache/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    15017 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/nocache/webstore.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    95532 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/nocache/webstore.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2342 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/sse.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1700 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/store_handlers.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16522 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/webstore.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      283 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/ws.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      720 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/webstore/ws.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.371078 open-cravat-2.4.1/cravat/websubmit/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       11 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/.gitignore
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   210024 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/Chart.bundle.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      719 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2291 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/down.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/email.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/favicon.ico
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/favicon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      108 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/googleAnalytics.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1052 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/help.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.372079 open-cravat-2.4.1/cravat/websubmit/input-examples/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      527 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/input-examples/cravat.hg18.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/input-examples/cravat.hg19.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/input-examples/cravat.hg38.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/input-examples/vcf.hg18.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/input-examples/vcf.hg19.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/input-examples/vcf.hg38.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/jquery-3.3.1.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    53784 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/logo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    56098 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/logo_transparent.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      225 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/menu.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.372079 open-cravat-2.4.1/cravat/websubmit/nocache/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13800 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/nocache/broken_wheel.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    18796 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/nocache/index.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    17372 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/nocache/websubmit.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    83472 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/nocache/websubmit.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    11488 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/nointernet.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    27869 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/pqselect.dev.customforsubmit.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2167 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/refresh.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/threedots.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    48552 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/websubmit/websubmit.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3724 2023-07-17 19:49:54.000000 open-cravat-2.4.1/cravat/wincravat.pyw
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.372079 open-cravat-2.4.1/open_cravat.egg-info/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-07-17 19:49:54.000000 open-cravat-2.4.1/open_cravat.egg-info/PKG-INFO
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12287 2023-07-17 19:49:54.000000 open-cravat-2.4.1/open_cravat.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2023-07-17 19:49:54.000000 open-cravat-2.4.1/open_cravat.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-07-17 19:49:54.000000 open-cravat-2.4.1/open_cravat.egg-info/entry_points.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      184 2023-07-17 19:49:54.000000 open-cravat-2.4.1/open_cravat.egg-info/requires.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        7 2023-07-17 19:49:54.000000 open-cravat-2.4.1/open_cravat.egg-info/top_level.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-07-17 19:49:54.373078 open-cravat-2.4.1/setup.cfg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2877 2023-07-17 19:49:54.000000 open-cravat-2.4.1/setup.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-07-17 19:49:54.373078 open-cravat-2.4.1/tests/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6183 2023-07-17 19:49:54.000000 open-cravat-2.4.1/tests/test_admin_util.py
```

### Comparing `open-cravat-2.4.0/LICENSE` & `open-cravat-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/PKG-INFO` & `open-cravat-2.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.4.0
+Version: 2.4.1
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: RyangGuk Kim, Kyle Moad, Mike Ryan, and Rachel Karchin
 Author-email: support@opencravat.org
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `open-cravat-2.4.0/README.rst` & `open-cravat-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/__init__.py` & `open-cravat-2.4.1/cravat/__init__.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/admin_util.py` & `open-cravat-2.4.1/cravat/admin_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/aggregator.py` & `open-cravat-2.4.1/cravat/aggregator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/annotator_options.py` & `open-cravat-2.4.1/cravat/annotator_options.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/annotator_template/annotator_template.py` & `open-cravat-2.4.1/cravat/annotator_template/annotator_template.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/annotator_template/annotator_template.yml` & `open-cravat-2.4.1/cravat/annotator_template/annotator_template.yml`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/base_annotator.py` & `open-cravat-2.4.1/cravat/base_annotator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/base_commonmodule.py` & `open-cravat-2.4.1/cravat/base_commonmodule.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/base_converter.py` & `open-cravat-2.4.1/cravat/base_converter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/base_mapper.py` & `open-cravat-2.4.1/cravat/base_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,21 @@
             tmp = []
             for col in cols:
                 if col == 'base__note_variant':
                     tmp.append('base__note')
                     continue
                 tmp.append(col)
             cols = tmp
+        if au.compare_version(dbver, '2.4.0') <= 0:
+            tmp = []
+            for col in cols:
+                if col in ('base__exonno','base__gposend'):
+                    continue
+                tmp.append(col)
+            cols = tmp
         data = {}
         t = time.time()
         rows = await cf.exec_db(cf.get_variant_data_for_cols, cols)
         rows_by_hugo = {}
         t = time.time()
         for row in rows:
             hugo = row[-1]
```

### Comparing `open-cravat-2.4.0/cravat/base_postaggregator.py` & `open-cravat-2.4.1/cravat/base_postaggregator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/base_summarizer.py` & `open-cravat-2.4.1/cravat/base_summarizer.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/config_loader.py` & `open-cravat-2.4.1/cravat/config_loader.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/constants.py` & `open-cravat-2.4.1/cravat/constants.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_admin.py` & `open-cravat-2.4.1/cravat/cravat_admin.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_class.py` & `open-cravat-2.4.1/cravat/cravat_class.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_convert.py` & `open-cravat-2.4.1/cravat/cravat_convert.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_filter.py` & `open-cravat-2.4.1/cravat/cravat_filter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_metrics.py` & `open-cravat-2.4.1/cravat/cravat_metrics.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_pack.py` & `open-cravat-2.4.1/cravat/cravat_pack.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_report.py` & `open-cravat-2.4.1/cravat/cravat_report.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_test.py` & `open-cravat-2.4.1/cravat/cravat_test.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_util.py` & `open-cravat-2.4.1/cravat/cravat_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/cravat_web.py` & `open-cravat-2.4.1/cravat/cravat_web.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/example_input` & `open-cravat-2.4.1/cravat/example_input`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/exceptions.py` & `open-cravat-2.4.1/cravat/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/inout.py` & `open-cravat-2.4.1/cravat/inout.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/liftover/hg18ToHg38.over.chain` & `open-cravat-2.4.1/cravat/liftover/hg18ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/liftover/hg19ToHg38.over.chain` & `open-cravat-2.4.1/cravat/liftover/hg19ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/mp_runners.py` & `open-cravat-2.4.1/cravat/mp_runners.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/oc.py` & `open-cravat-2.4.1/cravat/oc.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/store_utils.py` & `open-cravat-2.4.1/cravat/store_utils.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/util.py` & `open-cravat-2.4.1/cravat/util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/cravat_view.py` & `open-cravat-2.4.1/cravat/webresult/cravat_view.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/css/pqselect.min.css` & `open-cravat-2.4.1/cravat/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/email.png` & `open-cravat-2.4.1/cravat/webresult/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/favicon.ico` & `open-cravat-2.4.1/cravat/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/favicon.png` & `open-cravat-2.4.1/cravat/webresult/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/roboto-bold-webfont.woff` & `open-cravat-2.4.1/cravat/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/roboto-bold-webfont.woff2` & `open-cravat-2.4.1/cravat/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/roboto-light-webfont.woff` & `open-cravat-2.4.1/cravat/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/roboto-light-webfont.woff2` & `open-cravat-2.4.1/cravat/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/roboto-medium-webfont.woff` & `open-cravat-2.4.1/cravat/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/roboto-medium-webfont.woff2` & `open-cravat-2.4.1/cravat/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff` & `open-cravat-2.4.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `open-cravat-2.4.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/arrow-spinner-static.gif` & `open-cravat-2.4.1/cravat/webresult/images/arrow-spinner-static.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/arrow-spinner.gif` & `open-cravat-2.4.1/cravat/webresult/images/arrow-spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/arrows-move.svg` & `open-cravat-2.4.1/cravat/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/back_arrow.png` & `open-cravat-2.4.1/cravat/webresult/images/back_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/bigSpinner.gif` & `open-cravat-2.4.1/cravat/webresult/images/bigSpinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/camera.png` & `open-cravat-2.4.1/cravat/webresult/images/camera.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/camera.svg` & `open-cravat-2.4.1/cravat/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/close-button.png` & `open-cravat-2.4.1/cravat/webresult/images/close-button.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/close.png` & `open-cravat-2.4.1/cravat/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/close.svg` & `open-cravat-2.4.1/cravat/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/close_icon.png` & `open-cravat-2.4.1/cravat/webresult/images/close_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/download-material-black.png` & `open-cravat-2.4.1/cravat/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/download-material-blue.png` & `open-cravat-2.4.1/cravat/webresult/images/download-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/download.svg` & `open-cravat-2.4.1/cravat/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/help_16x16.gif` & `open-cravat-2.4.1/cravat/webresult/images/help_16x16.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/help_icon.png` & `open-cravat-2.4.1/cravat/webresult/images/help_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/loading-gif-animation.gif` & `open-cravat-2.4.1/cravat/webresult/images/loading-gif-animation.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/mail.png` & `open-cravat-2.4.1/cravat/webresult/images/mail.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/menu.png` & `open-cravat-2.4.1/cravat/webresult/images/menu.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/openNewTab.png` & `open-cravat-2.4.1/cravat/webresult/images/openNewTab.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/package.png` & `open-cravat-2.4.1/cravat/webresult/images/package.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/pencil.png` & `open-cravat-2.4.1/cravat/webresult/images/pencil.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/pin-2.png` & `open-cravat-2.4.1/cravat/webresult/images/pin-2.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/pin.png` & `open-cravat-2.4.1/cravat/webresult/images/pin.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/pin.svg` & `open-cravat-2.4.1/cravat/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/plus-circle-dotted.svg` & `open-cravat-2.4.1/cravat/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/question.png` & `open-cravat-2.4.1/cravat/webresult/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/resize.jpg` & `open-cravat-2.4.1/cravat/webresult/images/resize.jpg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/save.png` & `open-cravat-2.4.1/cravat/webresult/images/save.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/save_new.png` & `open-cravat-2.4.1/cravat/webresult/images/save_new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/search.png` & `open-cravat-2.4.1/cravat/webresult/images/search.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/sorry.png` & `open-cravat-2.4.1/cravat/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/spinCircle.gif` & `open-cravat-2.4.1/cravat/webresult/images/spinCircle.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/spinner.gif` & `open-cravat-2.4.1/cravat/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/triangle-down.png` & `open-cravat-2.4.1/cravat/webresult/images/triangle-down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/triangle-right.png` & `open-cravat-2.4.1/cravat/webresult/images/triangle-right.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/upload-material-black.png` & `open-cravat-2.4.1/cravat/webresult/images/upload-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/images/upload-material-blue.png` & `open-cravat-2.4.1/cravat/webresult/images/upload-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/index.html` & `open-cravat-2.4.1/cravat/webresult/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/Chart.js` & `open-cravat-2.4.1/cravat/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/dom-to-image.min.js` & `open-cravat-2.4.1/cravat/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/download.js` & `open-cravat-2.4.1/cravat/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/graphics.js` & `open-cravat-2.4.1/cravat/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-3.2.1.min.js` & `open-cravat-2.4.1/cravat/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json` & `open-cravat-2.4.1/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery.tools.min.js` & `open-cravat-2.4.1/cravat/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/jquery.url.js` & `open-cravat-2.4.1/cravat/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/packery.pkgd.js` & `open-cravat-2.4.1/cravat/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/readme.txt` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `open-cravat-2.4.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/pqselect.min.js` & `open-cravat-2.4.1/cravat/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/js/raphael-min.js` & `open-cravat-2.4.1/cravat/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/jsonreporter.py` & `open-cravat-2.4.1/cravat/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/css/singlevariantpage.css` & `open-cravat-2.4.1/cravat/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/css/style.css` & `open-cravat-2.4.1/cravat/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/css/widget.css` & `open-cravat-2.4.1/cravat/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/filter.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/infomgr.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/main.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/main.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/setup.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/showvariant.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/singlevariantpage.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/util.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/variables.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/js/widgethelper.js` & `open-cravat-2.4.1/cravat/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/nocache/variant.html` & `open-cravat-2.4.1/cravat/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/question.png` & `open-cravat-2.4.1/cravat/webresult/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webresult/webresult.py` & `open-cravat-2.4.1/cravat/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/cravat_store.css` & `open-cravat-2.4.1/cravat/webstore/cravat_store.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/favicon.ico` & `open-cravat-2.4.1/cravat/webstore/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/chat-dots.svg` & `open-cravat-2.4.1/cravat/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/chat-left-text.svg` & `open-cravat-2.4.1/cravat/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/done.png` & `open-cravat-2.4.1/cravat/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/email.png` & `open-cravat-2.4.1/cravat/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/empty.png` & `open-cravat-2.4.1/cravat/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/favicon.png` & `open-cravat-2.4.1/cravat/webstore/images/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/folder.png` & `open-cravat-2.4.1/cravat/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/genericmodulelogo.png` & `open-cravat-2.4.1/cravat/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/hamburger.png` & `open-cravat-2.4.1/cravat/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/left_arrow.png` & `open-cravat-2.4.1/cravat/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/logo.png` & `open-cravat-2.4.1/cravat/webstore/images/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/new.png` & `open-cravat-2.4.1/cravat/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/question.png` & `open-cravat-2.4.1/cravat/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/images/right_arrow.png` & `open-cravat-2.4.1/cravat/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/jquery-3.3.1.min.js` & `open-cravat-2.4.1/cravat/webstore/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/js/showdown-1.9.1.min.js` & `open-cravat-2.4.1/cravat/webstore/js/showdown-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/js/showdown.min.js.map` & `open-cravat-2.4.1/cravat/webstore/js/showdown.min.js.map`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/nocache/webstore.css` & `open-cravat-2.4.1/cravat/webstore/nocache/webstore.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/nocache/webstore.js` & `open-cravat-2.4.1/cravat/webstore/nocache/webstore.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/sse.py` & `open-cravat-2.4.1/cravat/webstore/sse.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/store_handlers.py` & `open-cravat-2.4.1/cravat/webstore/store_handlers.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/webstore.py` & `open-cravat-2.4.1/cravat/webstore/webstore.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/webstore/ws.js` & `open-cravat-2.4.1/cravat/webstore/ws.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/Chart.bundle.min.js` & `open-cravat-2.4.1/cravat/websubmit/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/arrow.png` & `open-cravat-2.4.1/cravat/websubmit/arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/down.png` & `open-cravat-2.4.1/cravat/websubmit/down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/email.png` & `open-cravat-2.4.1/cravat/websubmit/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/favicon.ico` & `open-cravat-2.4.1/cravat/websubmit/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/favicon.png` & `open-cravat-2.4.1/cravat/websubmit/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/help.png` & `open-cravat-2.4.1/cravat/websubmit/help.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/input-examples/cravat.hg18.txt` & `open-cravat-2.4.1/cravat/websubmit/input-examples/cravat.hg18.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/input-examples/cravat.hg19.txt` & `open-cravat-2.4.1/cravat/websubmit/input-examples/cravat.hg19.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/input-examples/cravat.hg38.txt` & `open-cravat-2.4.1/cravat/websubmit/input-examples/cravat.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/input-examples/vcf.hg18.txt` & `open-cravat-2.4.1/cravat/websubmit/input-examples/vcf.hg18.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/input-examples/vcf.hg19.txt` & `open-cravat-2.4.1/cravat/websubmit/input-examples/vcf.hg19.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/input-examples/vcf.hg38.txt` & `open-cravat-2.4.1/cravat/websubmit/input-examples/vcf.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/jquery-3.3.1.min.js` & `open-cravat-2.4.1/cravat/websubmit/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/logo.png` & `open-cravat-2.4.1/cravat/websubmit/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/logo_transparent.png` & `open-cravat-2.4.1/cravat/websubmit/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/nocache/broken_wheel.gif` & `open-cravat-2.4.1/cravat/websubmit/nocache/broken_wheel.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/nocache/index.html` & `open-cravat-2.4.1/cravat/websubmit/nocache/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/nocache/websubmit.css` & `open-cravat-2.4.1/cravat/websubmit/nocache/websubmit.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/nocache/websubmit.js` & `open-cravat-2.4.1/cravat/websubmit/nocache/websubmit.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/nointernet.png` & `open-cravat-2.4.1/cravat/websubmit/nointernet.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/pqselect.dev.customforsubmit.js` & `open-cravat-2.4.1/cravat/websubmit/pqselect.dev.customforsubmit.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/question.png` & `open-cravat-2.4.1/cravat/websubmit/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/refresh.png` & `open-cravat-2.4.1/cravat/websubmit/refresh.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/websubmit/websubmit.py` & `open-cravat-2.4.1/cravat/websubmit/websubmit.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/cravat/wincravat.pyw` & `open-cravat-2.4.1/cravat/wincravat.pyw`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/open_cravat.egg-info/PKG-INFO` & `open-cravat-2.4.1/open_cravat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.4.0
+Version: 2.4.1
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: RyangGuk Kim, Kyle Moad, Mike Ryan, and Rachel Karchin
 Author-email: support@opencravat.org
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `open-cravat-2.4.0/open_cravat.egg-info/SOURCES.txt` & `open-cravat-2.4.1/open_cravat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.4.0/setup.py` & `open-cravat-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 for root, dirs, files in os.walk(os.path.join('cravat', 'websubmit')):
     root_files = [os.path.join('..', root, f) for f in files]
     data_files.extend(root_files)
 
 setup(
     name='open-cravat',
     packages=['cravat'],
-    version='2.4.0',
+    version='2.4.1',
     description='OpenCRAVAT - variant analysis toolkit',
     long_description=readme(),
     author='RyangGuk Kim, Kyle Moad, Mike Ryan, and Rachel Karchin',
     author_email='support@opencravat.org',
     url='https://www.opencravat.org',
     license='',
     package_data={
```

### Comparing `open-cravat-2.4.0/tests/test_admin_util.py` & `open-cravat-2.4.1/tests/test_admin_util.py`

 * *Files identical despite different names*

