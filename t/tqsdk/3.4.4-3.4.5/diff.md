# Comparing `tmp/tqsdk-3.4.4.tar.gz` & `tmp/tqsdk-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tqsdk-3.4.4.tar", last modified: Wed Jul 12 08:36:24 2023, max compression
+gzip compressed data, was "dist/tqsdk-3.4.5.tar", last modified: Mon Jul 17 05:20:37 2023, max compression
```

## Comparing `tqsdk-3.4.4.tar` & `tqsdk-3.4.5.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5268 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-07-12 08:35:35.000000 tqsdk-3.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-07-12 08:35:35.000000 tqsdk-3.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/
--rw-r--r--   0 runner    (1001) docker     (122)    20440 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/backtest/
--rw-r--r--   0 runner    (1001) docker     (122)     4816 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/backtest/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42162 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/backtest/backtest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6687 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/backtest/replay.py
--rw-r--r--   0 runner    (1001) docker     (122)     5400 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/baseApi.py
--rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/utils_symbols.py
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/stockprofit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/tradeable/
--rw-r--r--   0 runner    (1001) docker     (122)    15130 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/tradeable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/tradeable/otg/
--rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/otg/base_otg.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/otg/tqkq.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/otg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/otg/tqaccount.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/
--rw-r--r--   0 runner    (1001) docker     (122)    35956 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/trade_future.py
--rw-r--r--   0 runner    (1001) docker     (122)    10665 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/tqsim.py
--rw-r--r--   0 runner    (1001) docker     (122)     5083 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11943 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/trade_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8523 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/tqsim_stock.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18113 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/basesim.py
--rw-r--r--   0 runner    (1001) docker     (122)    27585 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tradeable/sim/trade_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/web/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/web/img/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/web/img/icons/
--rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/notes
--rw-r--r--   0 runner    (1001) docker     (122)    16757 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (122)     2890 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/ms-icon-70x70.png
--rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (122)     4557 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (122)     7785 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (122)     2628 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/icons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)   555353 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/img/ionicons.a2c4a261.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/web/css/
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/css/app.d72d8978.css
--rw-r--r--   0 runner    (1001) docker     (122)   279508 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/css/chunk-vendors.c93e9127.css
--rw-r--r--   0 runner    (1001) docker     (122)   246120 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/web/js/
--rw-r--r--   0 runner    (1001) docker     (122)    62759 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/js/app.2c843c86.js
--rw-r--r--   0 runner    (1001) docker     (122)  1787845 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/js/chunk-vendors.d7fceff6.js
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/web/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   197664 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/fonts/ionicons.d535a25a.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    82216 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   197740 2023-07-12 08:35:36.000000 tqsdk-3.4.4/tqsdk/web/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/service-worker.js
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/web/robots.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    91538 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/ta.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5865 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)     9392 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/trade_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)    15785 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/ins_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tools/dead_ins.lzma
--rw-r--r--   0 runner    (1001) docker     (122)    22148 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tools/downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3270 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/trading_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     4949 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/demo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/demo/example/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/doublema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4596 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/rbreaker.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/vwap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 08:35:38.000000 tqsdk-3.4.4/tqsdk/demo/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/dualthrust.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/momentum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/escalator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/fairy_four_price.py
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/gridtrading_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     7794 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/turtle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/gridtrading.py
--rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/rbreaker2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/example/aberration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t94.py
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t10.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t90.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t92.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/underlying_symbol.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t20.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t95.py
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t93.py
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t80.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t72.py
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t30.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t60.py
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t70.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t91.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 08:35:38.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t96.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/replay2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/backtest.py
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t41.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t40.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/replay.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/tutorial/t71.py
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/ta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/ta_option.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/download_orders.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 08:35:38.000000 tqsdk-3.4.4/tqsdk/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/multiaccount.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o20.py
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o10.py
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o41.py
--rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o74.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o40.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o72.py
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o71.py
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o60.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 08:35:38.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o30.py
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o70.py
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/demo/option_tutorial/o73.py
--rw-r--r--   0 runner    (1001) docker     (122)    12660 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/risk_rule.py
--rw-r--r--   0 runner    (1001) docker     (122)    52982 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tafunc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    19843 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/tqwebhelper.py
--rw-r--r--   0 runner    (1001) docker     (122)   208425 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/symbols.py
--rw-r--r--   0 runner    (1001) docker     (122)     6925 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/sm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1769 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/log.py
--rw-r--r--   0 runner    (1001) docker     (122)    10044 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/data_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/__pyinstaller/hook-tqsdk.py
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      603 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     9254 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/datetime_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    37146 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/objs.py
--rw-r--r--   0 runner    (1001) docker     (122)    23481 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/data_series.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/risk_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)    15935 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/algorithm/time_table_generater.py
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15605 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/algorithm/twap.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/baseModule.py
--rw-r--r--   0 runner    (1001) docker     (122)     4910 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/channel.py
--rw-r--r--   0 runner    (1001) docker     (122)   132245 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/expired_quotes.json.lzma
--rw-r--r--   0 runner    (1001) docker     (122)    20372 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/objs_not_entity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:36:24.000000 tqsdk-3.4.4/tqsdk/lib/
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/lib/notify.py
--rw-r--r--   0 runner    (1001) docker     (122)     4674 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/lib/target_pos_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)    38277 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/lib/target_pos_task.py
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21986 2023-07-12 08:35:35.000000 tqsdk-3.4.4/tqsdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-12 08:36:24.000000 tqsdk-3.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-07-12 08:35:35.000000 tqsdk-3.4.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-07-12 08:36:24.000000 tqsdk-3.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11335 2023-07-12 08:35:35.000000 tqsdk-3.4.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5268 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-07-17 05:19:58.000000 tqsdk-3.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-07-17 05:19:58.000000 tqsdk-3.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/
+-rw-r--r--   0 runner    (1001) docker     (122)    20440 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/backtest/
+-rw-r--r--   0 runner    (1001) docker     (122)     4816 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/backtest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42162 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/backtest/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6687 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/backtest/replay.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5400 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/baseApi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/utils_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/stockprofit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/tradeable/
+-rw-r--r--   0 runner    (1001) docker     (122)    15130 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/tradeable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/tradeable/otg/
+-rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/otg/base_otg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/otg/tqkq.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/otg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/otg/tqaccount.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/
+-rw-r--r--   0 runner    (1001) docker     (122)    35956 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/trade_future.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10665 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/tqsim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5083 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11943 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/trade_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8523 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/tqsim_stock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18113 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/basesim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27585 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tradeable/sim/trade_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/web/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/web/img/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/web/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/notes
+-rw-r--r--   0 runner    (1001) docker     (122)    16757 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2890 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/ms-icon-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4557 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7785 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2628 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/img/icons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)   555353 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/web/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/css/app.d72d8978.css
+-rw-r--r--   0 runner    (1001) docker     (122)   279508 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/css/chunk-vendors.c93e9127.css
+-rw-r--r--   0 runner    (1001) docker     (122)   246120 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/web/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    62759 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/js/app.2c843c86.js
+-rw-r--r--   0 runner    (1001) docker     (122)  1787845 2023-07-17 05:20:00.000000 tqsdk-3.4.5/tqsdk/web/js/chunk-vendors.d7fceff6.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/web/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   197664 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/fonts/ionicons.d535a25a.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    82216 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   197740 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/service-worker.js
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/web/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    91538 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/ta.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5865 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9392 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/trade_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15785 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/ins_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tools/dead_ins.lzma
+-rw-r--r--   0 runner    (1001) docker     (122)    22148 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tools/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3270 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/trading_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4949 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/demo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/demo/example/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/doublema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4596 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/rbreaker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/vwap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:01.000000 tqsdk-3.4.5/tqsdk/demo/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/dualthrust.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/escalator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/fairy_four_price.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/gridtrading_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7794 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/gridtrading.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/rbreaker2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/example/aberration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t94.py
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t10.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t90.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t92.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/underlying_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t95.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t93.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t80.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t72.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t30.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t60.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t70.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t91.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:01.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t96.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/replay2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t41.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t40.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/replay.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/tutorial/t71.py
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/ta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/ta_option.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/download_orders.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:01.000000 tqsdk-3.4.5/tqsdk/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/multiaccount.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o10.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o41.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o74.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o40.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o72.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o71.py
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o60.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:01.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o30.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o70.py
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/demo/option_tutorial/o73.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12660 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/risk_rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52982 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/tafunc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19843 2023-07-17 05:19:59.000000 tqsdk-3.4.5/tqsdk/tqwebhelper.py
+-rw-r--r--   0 runner    (1001) docker     (122)   208425 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6925 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/sm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1769 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10044 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/data_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/__pyinstaller/hook-tqsdk.py
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9254 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/datetime_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37146 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23481 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/risk_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)    15935 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/algorithm/time_table_generater.py
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15367 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/algorithm/twap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/baseModule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4910 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/channel.py
+-rw-r--r--   0 runner    (1001) docker     (122)   132245 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/expired_quotes.json.lzma
+-rw-r--r--   0 runner    (1001) docker     (122)    20372 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/objs_not_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 05:20:37.000000 tqsdk-3.4.5/tqsdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/lib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4674 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/lib/target_pos_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38039 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/lib/target_pos_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21986 2023-07-17 05:19:58.000000 tqsdk-3.4.5/tqsdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-17 05:20:37.000000 tqsdk-3.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-07-17 05:19:58.000000 tqsdk-3.4.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-07-17 05:20:37.000000 tqsdk-3.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11335 2023-07-17 05:19:58.000000 tqsdk-3.4.5/LICENSE
```

### Comparing `tqsdk-3.4.4/tqsdk.egg-info/PKG-INFO` & `tqsdk-3.4.5/tqsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.4.4
+Version: 3.4.5
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.4.4/tqsdk.egg-info/SOURCES.txt` & `tqsdk-3.4.5/tqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/README.md` & `tqsdk-3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/report.py` & `tqsdk-3.4.5/tqsdk/report.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/backtest/utils.py` & `tqsdk-3.4.5/tqsdk/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/backtest/backtest.py` & `tqsdk-3.4.5/tqsdk/backtest/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/backtest/replay.py` & `tqsdk-3.4.5/tqsdk/backtest/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/baseApi.py` & `tqsdk-3.4.5/tqsdk/baseApi.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/utils_symbols.py` & `tqsdk-3.4.5/tqsdk/utils_symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/stockprofit.py` & `tqsdk-3.4.5/tqsdk/stockprofit.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/mixin.py` & `tqsdk-3.4.5/tqsdk/tradeable/mixin.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/tradeable.py` & `tqsdk-3.4.5/tqsdk/tradeable/tradeable.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/otg/base_otg.py` & `tqsdk-3.4.5/tqsdk/tradeable/otg/base_otg.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/otg/tqkq.py` & `tqsdk-3.4.5/tqsdk/tradeable/otg/tqkq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/otg/tqaccount.py` & `tqsdk-3.4.5/tqsdk/tradeable/otg/tqaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/trade_future.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/trade_future.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/tqsim.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/tqsim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/utils.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/trade_base.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/trade_base.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/tqsim_stock.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/tqsim_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/basesim.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/basesim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tradeable/sim/trade_stock.py` & `tqsdk-3.4.5/tqsdk/tradeable/sim/trade_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/mstile-150x150.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/msapplication-icon-144x144.png.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/msapplication-icon-144x144.png.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/notes` & `tqsdk-3.4.5/tqsdk/web/img/icons/notes`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/ms-icon-310x310.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-36x36.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-76x76.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/favicon.ico` & `tqsdk-3.4.5/tqsdk/web/img/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/favicon-32x32.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-192x192.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-57x57.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/ms-icon-150x150.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-chrome-192x192.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-72x72.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/ms-icon-70x70.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-144x144.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-48x48.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-precomposed.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/android-icon-96x96.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-114x114.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-152x152.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/favicon-96x96.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-180x180.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-144x144.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-72x72.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-60x60.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/favicon-16x16.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/apple-touch-icon-120x120.png` & `tqsdk-3.4.5/tqsdk/web/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/icons/manifest.json` & `tqsdk-3.4.5/tqsdk/web/img/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/img/ionicons.a2c4a261.svg` & `tqsdk-3.4.5/tqsdk/web/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js` & `tqsdk-3.4.5/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/css/app.d72d8978.css` & `tqsdk-3.4.5/tqsdk/web/css/app.d72d8978.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/css/chunk-vendors.c93e9127.css` & `tqsdk-3.4.5/tqsdk/web/css/chunk-vendors.c93e9127.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/d3.min.js` & `tqsdk-3.4.5/tqsdk/web/d3.min.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/favicon.ico` & `tqsdk-3.4.5/tqsdk/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/js/app.2c843c86.js` & `tqsdk-3.4.5/tqsdk/web/js/app.2c843c86.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/js/chunk-vendors.d7fceff6.js` & `tqsdk-3.4.5/tqsdk/web/js/chunk-vendors.d7fceff6.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/index.html` & `tqsdk-3.4.5/tqsdk/web/index.html`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/fonts/ionicons.d535a25a.ttf` & `tqsdk-3.4.5/tqsdk/web/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/fonts/ionicons.143146fa.woff2` & `tqsdk-3.4.5/tqsdk/web/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/fonts/ionicons.99ac3308.woff` & `tqsdk-3.4.5/tqsdk/web/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/service-worker.js` & `tqsdk-3.4.5/tqsdk/web/service-worker.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/web/manifest.json` & `tqsdk-3.4.5/tqsdk/web/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/auth.py` & `tqsdk-3.4.5/tqsdk/auth.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/ta.py` & `tqsdk-3.4.5/tqsdk/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/utils.py` & `tqsdk-3.4.5/tqsdk/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/calendar.py` & `tqsdk-3.4.5/tqsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/trade_extension.py` & `tqsdk-3.4.5/tqsdk/trade_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/ins_schema.py` & `tqsdk-3.4.5/tqsdk/ins_schema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tools/dead_ins.lzma` & `tqsdk-3.4.5/tqsdk/tools/dead_ins.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tools/downloader.py` & `tqsdk-3.4.5/tqsdk/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/trading_status.py` & `tqsdk-3.4.5/tqsdk/trading_status.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/datetime.py` & `tqsdk-3.4.5/tqsdk/datetime.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/doublema.py` & `tqsdk-3.4.5/tqsdk/demo/example/doublema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/rbreaker.py` & `tqsdk-3.4.5/tqsdk/demo/example/rbreaker.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/vwap.py` & `tqsdk-3.4.5/tqsdk/demo/example/vwap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/random_forest.py` & `tqsdk-3.4.5/tqsdk/demo/example/random_forest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/dualthrust.py` & `tqsdk-3.4.5/tqsdk/demo/example/dualthrust.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/momentum.py` & `tqsdk-3.4.5/tqsdk/demo/example/momentum.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/escalator.py` & `tqsdk-3.4.5/tqsdk/demo/example/escalator.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/fairy_four_price.py` & `tqsdk-3.4.5/tqsdk/demo/example/fairy_four_price.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/gridtrading_async.py` & `tqsdk-3.4.5/tqsdk/demo/example/gridtrading_async.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/turtle.py` & `tqsdk-3.4.5/tqsdk/demo/example/turtle.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/gridtrading.py` & `tqsdk-3.4.5/tqsdk/demo/example/gridtrading.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/rbreaker2.py` & `tqsdk-3.4.5/tqsdk/demo/example/rbreaker2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/example/aberration.py` & `tqsdk-3.4.5/tqsdk/demo/example/aberration.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t94.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t94.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t90.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t90.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t92.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t92.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t20.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t95.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t95.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t93.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t93.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t80.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t80.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/downloader.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t72.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t30.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t60.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t70.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t91.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t91.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t96.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t96.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/replay2.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/replay2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/backtest.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t41.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t40.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/replay.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/tutorial/t71.py` & `tqsdk-3.4.5/tqsdk/demo/tutorial/t71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/ta.py` & `tqsdk-3.4.5/tqsdk/demo/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/ta_option.py` & `tqsdk-3.4.5/tqsdk/demo/ta_option.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/download_orders.py` & `tqsdk-3.4.5/tqsdk/demo/download_orders.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/multiaccount.py` & `tqsdk-3.4.5/tqsdk/demo/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o20.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o41.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o74.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o74.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o40.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o72.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o71.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o60.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o30.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o70.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/demo/option_tutorial/o73.py` & `tqsdk-3.4.5/tqsdk/demo/option_tutorial/o73.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/risk_rule.py` & `tqsdk-3.4.5/tqsdk/risk_rule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tafunc.py` & `tqsdk-3.4.5/tqsdk/tafunc.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/exceptions.py` & `tqsdk-3.4.5/tqsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/diff.py` & `tqsdk-3.4.5/tqsdk/diff.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/tqwebhelper.py` & `tqsdk-3.4.5/tqsdk/tqwebhelper.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/api.py` & `tqsdk-3.4.5/tqsdk/api.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/symbols.py` & `tqsdk-3.4.5/tqsdk/symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/sm.py` & `tqsdk-3.4.5/tqsdk/sm.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/log.py` & `tqsdk-3.4.5/tqsdk/log.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/data_extension.py` & `tqsdk-3.4.5/tqsdk/data_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/__init__.py` & `tqsdk-3.4.5/tqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/rangeset.py` & `tqsdk-3.4.5/tqsdk/rangeset.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/entity.py` & `tqsdk-3.4.5/tqsdk/entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/multiaccount.py` & `tqsdk-3.4.5/tqsdk/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/datetime_state.py` & `tqsdk-3.4.5/tqsdk/datetime_state.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/objs.py` & `tqsdk-3.4.5/tqsdk/objs.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/data_series.py` & `tqsdk-3.4.5/tqsdk/data_series.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/risk_manager.py` & `tqsdk-3.4.5/tqsdk/risk_manager.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/algorithm/time_table_generater.py` & `tqsdk-3.4.5/tqsdk/algorithm/time_table_generater.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/algorithm/twap.py` & `tqsdk-3.4.5/tqsdk/algorithm/twap.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,14 @@
                 break
 
           print("打印出 twap 全部成交以及成交均价")
           print(target_twap.trades)
           print(target_twap.average_trade_price)
           api.close()
         """
-        if symbol.startswith("CZCE.CJ"):
-            raise Exception("红枣期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 4 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.ZC"):
             raise Exception("动力煤期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 4 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.WH"):
             raise Exception("强麦期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 10 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.PM"):
             raise Exception("普麦期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 10 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.RI"):
```

### Comparing `tqsdk-3.4.4/tqsdk/baseModule.py` & `tqsdk-3.4.5/tqsdk/baseModule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/channel.py` & `tqsdk-3.4.5/tqsdk/channel.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/expired_quotes.json.lzma` & `tqsdk-3.4.5/tqsdk/expired_quotes.json.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/objs_not_entity.py` & `tqsdk-3.4.5/tqsdk/objs_not_entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/lib/notify.py` & `tqsdk-3.4.5/tqsdk/lib/notify.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/lib/utils.py` & `tqsdk-3.4.5/tqsdk/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/lib/target_pos_scheduler.py` & `tqsdk-3.4.5/tqsdk/lib/target_pos_scheduler.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/tqsdk/lib/target_pos_task.py` & `tqsdk-3.4.5/tqsdk/lib/target_pos_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,14 @@
             # 2021-03-15 11:29:48 -     INFO - 时间: 2021-03-15 11:29:47.522848, 合约: SHFE.rb2106, 开平: OPEN, 方向: BUY, 手数: 10, 价格: 4687.000,手续费: 47.05
             # 2021-03-15 11:29:48 -     INFO - 时间: 2021-03-15 11:29:47.525617, 合约: SHFE.rb2106, 开平: OPEN, 方向: BUY, 手数: 8, 价格: 4687.000,手续费: 37.64
             # 2021-03-15 11:29:48 -     INFO - 时间: 2021-03-15 11:29:47.528151, 合约: SHFE.rb2106, 开平: OPEN, 方向: BUY, 手数: 7, 价格: 4687.000,手续费: 32.94
             # 2021-03-15 11:29:48 -     INFO - 时间: 2021-03-15 11:29:47.530930, 合约: SHFE.rb2106, 开平: OPEN, 方向: BUY, 手数: 7, 价格: 4687.000,手续费: 32.94
             # 2021-03-15 11:29:48 -     INFO - 时间: 2021-03-15 11:29:47.533515, 合约: SHFE.rb2106, 开平: OPEN, 方向: BUY, 手数: 3, 价格: 4687.000,手续费: 14.12
 
         """
-        if symbol.startswith("CZCE.CJ"):
-            raise Exception("红枣期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 4 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.ZC"):
             raise Exception("动力煤期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 4 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.WH"):
             raise Exception("强麦期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 10 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.PM"):
             raise Exception("普麦期货不支持创建 targetpostask、twap、vwap 任务，交易所规定该品种最小开仓手数为大于等于 10 手，这些函数还未支持该规则!")
         if symbol.startswith("CZCE.RI"):
```

### Comparing `tqsdk-3.4.4/tqsdk/connect.py` & `tqsdk-3.4.5/tqsdk/connect.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.4.4/setup.py` & `tqsdk-3.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", mode="r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tqsdk',
-    version="3.4.4",
+    version="3.4.5",
     description='TianQin SDK',
     author='TianQin',
     author_email='tianqincn@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.shinnytech.com/tqsdk',
     packages=setuptools.find_packages(exclude=["tqsdk.test", "tqsdk.test.*"]),
```

### Comparing `tqsdk-3.4.4/PKG-INFO` & `tqsdk-3.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.4.4
+Version: 3.4.5
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.4.4/LICENSE` & `tqsdk-3.4.5/LICENSE`

 * *Files identical despite different names*

