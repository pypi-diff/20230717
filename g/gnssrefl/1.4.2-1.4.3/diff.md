# Comparing `tmp/gnssrefl-1.4.2.tar.gz` & `tmp/gnssrefl-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.4.2.tar", last modified: Mon Jul 10 09:17:36 2023, max compression
+gzip compressed data, was "gnssrefl-1.4.3.tar", last modified: Mon Jul 17 14:04:19 2023, max compression
```

## Comparing `gnssrefl-1.4.2.tar` & `gnssrefl-1.4.3.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.364844 gnssrefl-1.4.2/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.364844 gnssrefl-1.4.2/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33744 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   183016 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nyquist_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.364844 gnssrefl-1.4.2/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:18.982496 gnssrefl-1.4.3/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:18.982496 gnssrefl-1.4.3/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33744 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   183142 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nyquist_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:18.982496 gnssrefl-1.4.3/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.4.2/LICENSE` & `gnssrefl-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/PKG-INFO` & `gnssrefl-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.2
+Version: 1.4.3
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
 I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
 using the newarcs option in the last month, you need to rerun gnssir and any 
 downstream codes (subdaily, daily_avg etc). This bug has
```

### Comparing `gnssrefl-1.4.2/README.md` & `gnssrefl-1.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.4.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
 I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
 using the newarcs option in the last month, you need to rerun gnssir and any 
 downstream codes (subdaily, daily_avg etc). This bug has
```

### Comparing `gnssrefl-1.4.2/gnssrefl/EGM96.py` & `gnssrefl-1.4.3/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/check_rinex_file.py` & `gnssrefl-1.4.3/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/computemp1mp2.py` & `gnssrefl-1.4.3/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/daily_avg.py` & `gnssrefl-1.4.3/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.4.3/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.4.3/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/decipher_argt.py` & `gnssrefl-1.4.3/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_ioc.py` & `gnssrefl-1.4.3/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_noaa.py` & `gnssrefl-1.4.3/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_orbits.py` & `gnssrefl-1.4.3/gnssrefl/download_orbits.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     orbit : string
         value options:
 
             gps (default) : uses GPS broadcast orbit
 
             gps+glo : will use JAXA orbits which have GPS and Glonass (usually available in 48 hours)
 
-            gnss : will use GFZ orbits, which is multi-GNSS (available in 3-4 days)
+            gnss : will use GFZ orbits, which is multi-GNSS (available in 3-4 days). but taken from CDDIS archive
 
             nav : GPS broadcast, adequate for reflectometry. Searches various places
 
             nav-sopac : GPS broadcast file from SOPAC, adequate for reflectometry. 
 
             nav-esa : GPS broadcast file from ESA, adequate for reflectometry. 
 
@@ -116,20 +116,17 @@
         print(orbit_list)
         sys.exit()
 
     # if generic names used, we direct people to these orbit types
     if pCtr == 'gps':
         pCtr = 'nav'
 
-    # try to avoid CDDIS. after 2022, just go to rapid. before that, more nuanced ....
+    # send to CDDIS to get final GFZ orbits
     if pCtr == 'gnss':
-        if year >= 2022:
-            pCtr = 'gfr'
-        else:
-            pCtr = 'gnss3'
+        pCtr = 'gbm'
 
     if pCtr == 'gps+glo':
         pCtr = 'jax'
 
     # using gfz multi-gnss for rapid
     if pCtr == 'rapid':
         pCtr = 'gfr'
```

### Comparing `gnssrefl-1.4.2/gnssrefl/download_psmsl.py` & `gnssrefl-1.4.3/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_rinex.py` & `gnssrefl-1.4.3/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_teqc.py` & `gnssrefl-1.4.3/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_tides.py` & `gnssrefl-1.4.3/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_unr.py` & `gnssrefl-1.4.3/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/download_wsv.py` & `gnssrefl-1.4.3/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/filesizes.py` & `gnssrefl-1.4.3/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gnssir.py` & `gnssrefl-1.4.3/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gnssir_cl.py` & `gnssrefl-1.4.3/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gnssir_input.py` & `gnssrefl-1.4.3/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gnssir_v2.py` & `gnssrefl-1.4.3/gnssrefl/gnssir_v2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gnsssnr.f` & `gnssrefl-1.4.3/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.4.3/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gps.py` & `gnssrefl-1.4.3/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,14 +702,15 @@
     """
     screenstats = False # for now
     foundit = False
     # this returns sp3 orbit product name
     month, day, doy, cyyyy, cyy, cdoy = ymd2ch(year,month,day)
 
     name, fdir = sp3_name(year,month,day,pCtr) 
+    print('sp3 filename ',name)
     gps_week = name[3:7]
     igps_week = int(gps_week)
     # unfortunately the CDDIS archive was at one point computing the GPS week wrong
     igps_week_at_cddis = 1 + int(gps_week)
     #print('GPS week', gps_week,igps_week)
     file1 = name + '.Z'
 
@@ -3449,19 +3450,19 @@
     snrexe : str 
         location of SNR executable. only relevant for fortran users
 
     """
     #default values
     # if they ask for gnss or gnss3, always use rapid.
     # at least for years 2022 and after
-    if year >= 2022:
-        if (orbtype == 'gnss') or (orbtype == 'gnss3'):
-            orbtype = 'rapid'
-        if orbtype == 'gbm':
-            orbtype = 'rapid'
+    #if year >= 2022:
+    #    if (orbtype == 'gnss') or (orbtype == 'gnss3'):
+    #        orbtype = 'rapid'
+        #if orbtype == 'gbm':
+        #    orbtype = 'rapid'
 
     foundit = False
     f=''; orbdir=''
     # define directory for the conversion executables
     exedir = os.environ['EXE']
     if (orbtype == 'grg'):
         # French multi gnss, but there are no Beidou results
@@ -5283,14 +5284,16 @@
         lat = 58.455146633; lon  = -135.888483766 ; ht = 12.559;  
     elif (station == 'ugar'):
         lat = -9.50477824; lon = 143.54686680 ; ht =  81.2
     elif (station == 'whla'):
         lat = -33.01640186 ; lon = 137.59157111 ; ht = 7.856
     elif (station == 'kubn'):
         lat =-10.23608303 ; lon =142.21446068; ht = 78.2
+    elif (station == 'smm4'):
+        lat =72.57369139 ; lon =-38.470709199 ; ht = 3262
 
     if (not_in_database) and (lat == 0):
         print('Did not find station coordinates :', station)
 
     return lat,lon,ht
 
 def rinex3_nav(year,month,day):
@@ -5732,15 +5735,15 @@
     filename : str
         name of the rinex file or orbit file
 
     directory : str
         where the file lives at CDDIS
 
     """
-    print('Original way of accessing CDDIS ')
+    #print('Original way of accessing CDDIS ')
 
     ftps = FTP_TLS(host = 'gdc.cddis.eosdis.nasa.gov')
     email = 'kristine.larson@colorado.edu'
     ftps.login(user='anonymous', passwd=email)
     ftps.prot_p()
     ftps.cwd(directory)
     ftps.retrbinary("RETR " + filename, open(filename, 'wb').write)
```

### Comparing `gnssrefl-1.4.2/gnssrefl/gpssnr.f` & `gnssrefl-1.4.3/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gpsweek.py` & `gnssrefl-1.4.3/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.4.3/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/highrate.py` & `gnssrefl-1.4.3/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/installexe_cl.py` & `gnssrefl-1.4.3/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/invsnr_cl.py` & `gnssrefl-1.4.3/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/invsnr_input.py` & `gnssrefl-1.4.3/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/karnak_libraries.py` & `gnssrefl-1.4.3/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/kelly.py` & `gnssrefl-1.4.3/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/llh2xyz.py` & `gnssrefl-1.4.3/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/make_json_input.py` & `gnssrefl-1.4.3/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/nmea2snr.py` & `gnssrefl-1.4.3/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.4.3/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/nyquist_cl.py` & `gnssrefl-1.4.3/gnssrefl/nyquist_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/nyquist_libs.py` & `gnssrefl-1.4.3/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/phase_functions.py` & `gnssrefl-1.4.3/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/prn2gps.py` & `gnssrefl-1.4.3/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/query_unr.py` & `gnssrefl-1.4.3/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/quickLook_cl.py` & `gnssrefl-1.4.3/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/quickLook_function.py` & `gnssrefl-1.4.3/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/quickLook_function2.py` & `gnssrefl-1.4.3/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/quickPhase.py` & `gnssrefl-1.4.3/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/quicklib.py` & `gnssrefl-1.4.3/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/quickplt.py` & `gnssrefl-1.4.3/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/read_snr_files.py` & `gnssrefl-1.4.3/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/refl_zones.py` & `gnssrefl-1.4.3/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.4.3/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/refraction.py` & `gnssrefl-1.4.3/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/rh_plot.py` & `gnssrefl-1.4.3/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/rinex2snr.py` & `gnssrefl-1.4.3/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.4.3/gnssrefl/rinex2snr_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,27 +128,27 @@
     orb : str, optional
         Which orbit files to download. Value options:
 
             gps (default) : will use GPS broadcast orbit
 
             gps+glos : will use JAXA orbits which have GPS and Glonass (usually available in 48 hours)
 
-            gnss : will use GFZ orbits, which is multi-GNSS (available in 3-4 days?)
+            gnss : use GFZ final orbits, which is multi-GNSS (available in 3-4 days?), but from CDDIS archive
 
-            gnss3 : test case for GFZ orbits downloaded from GFZ instead of CDDIS
+            gnss3 : GFZ orbits downloaded from GFZ instead of CDDIS, but do they include beidou?
 
             nav : GPS broadcast, perfectly adequate for reflectometry. Same as gps.
 
             igs : IGS precise, GPS only
 
             igr : IGS rapid, GPS only
 
             jax : JAXA, GPS + Glonass, within a few days, missing block III GPS satellites
 
-            gbm : GFZ Potsdam, multi-GNSS, not rapid
+            gbm : GFZ Potsdam, multi-GNSS, not rapid, via CDDIS 
 
             grg : French group, GPS, Galileo and Glonass, not rapid
 
             esa : ESA, multi-GNSS
 
             gfr : GFZ rapid, GPS, Galileo and Glonass, since May 17 2021
 
@@ -289,14 +289,15 @@
     if orb == 'rapid':
         orb = 'gfr'
 
     # if you choose GNSS, you get the GFZ sp3 file  (precise)
     # I think gbm should be changed to 'gnss3' though perhaps not here
     if orb == 'gnss':
         orb = 'gbm'
+        print('Using GBM orbit')
 
 
     # get orbit from IGS
     if orb == 'gnss2':
         # this code wants year month day....
         year, month, day = g.ydoy2ymd(year, doy)
         filename, fdir, foundit = g.avoid_cddis(year, month, day)
```

### Comparing `gnssrefl-1.4.2/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.4.3/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/rinex3_snr.py` & `gnssrefl-1.4.3/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/rinpy.py` & `gnssrefl-1.4.3/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.4.3/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/smoosh.py` & `gnssrefl-1.4.3/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/smoosh_snr.py` & `gnssrefl-1.4.3/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/snow_functions.py` & `gnssrefl-1.4.3/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.4.3/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/spline_functions.py` & `gnssrefl-1.4.3/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/subdaily.py` & `gnssrefl-1.4.3/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/subdaily_cl.py` & `gnssrefl-1.4.3/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/utils.py` & `gnssrefl-1.4.3/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/veg_multiyr.py` & `gnssrefl-1.4.3/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/vwc.py` & `gnssrefl-1.4.3/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/vwc_cl.py` & `gnssrefl-1.4.3/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/vwc_input.py` & `gnssrefl-1.4.3/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/xnmeasnr.f` & `gnssrefl-1.4.3/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/xyz2llh.py` & `gnssrefl-1.4.3/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/ydoy.py` & `gnssrefl-1.4.3/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl/ymd.py` & `gnssrefl-1.4.3/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.4.3/gnssrefl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.2
+Version: 1.4.3
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
 I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
 using the newarcs option in the last month, you need to rerun gnssir and any 
 downstream codes (subdaily, daily_avg etc). This bug has
```

### Comparing `gnssrefl-1.4.2/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.4.3/gnssrefl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 gnssrefl/installexe_cl.py
 gnssrefl/invsnr_cl.py
 gnssrefl/invsnr_input.py
 gnssrefl/karnak_libraries.py
 gnssrefl/kelly.py
 gnssrefl/llh2xyz.py
 gnssrefl/make_json_input.py
+gnssrefl/make_meta.py
 gnssrefl/nmea2snr.py
 gnssrefl/nmea2snr_cl.py
 gnssrefl/nyquist_cl.py
 gnssrefl/nyquist_libs.py
 gnssrefl/phase_functions.py
 gnssrefl/pickle_dilemma.py
 gnssrefl/prn2gps.py
```

### Comparing `gnssrefl-1.4.2/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.4.3/gnssrefl.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 gnssir = gnssrefl.gnssir_cl:main
 gnssir_input = gnssrefl.gnssir_input:main
 gpsweek = gnssrefl.gpsweek:main
 installexe = gnssrefl.installexe_cl:main
 invsnr = gnssrefl.invsnr_cl:main
 invsnr_input = gnssrefl.invsnr_input:main
 llh2xyz = gnssrefl.llh2xyz:main
+make_meta = gnssrefl.make_meta:main
 mp1mp2 = gnssrefl.computemp1mp2:main
 nmea2snr = gnssrefl.nmea2snr_cl:main
 nyquist = gnssrefl.nyquist_cl:main
 phase = gnssrefl.quickPhase:main
 pickle_dilemma = gnssrefl.pickle_dilemma:main
 prn2gps = gnssrefl.prn2gps:main
 query_unr = gnssrefl.query_unr:main
```

### Comparing `gnssrefl-1.4.2/pyproject.toml` & `gnssrefl-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.2/setup.py` & `gnssrefl-1.4.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,103 @@
 from setuptools import setup, find_packages
 from numpy.distutils.core import setup, Extension
 
 
-ext1 = Extension(name='gnssrefl.gpssnr', 
-        sources=['gnssrefl/gpssnr.f'], 
-        f2py_options=['--verbose'],
-        )
+ext1 = Extension(
+    name="gnssrefl.gpssnr",
+    sources=["gnssrefl/gpssnr.f"],
+    f2py_options=["--verbose"],
+)
 
-ext2 = Extension(name='gnssrefl.gnsssnr', 
-        sources=['gnssrefl/gnsssnr.f'], 
-        f2py_options=['--verbose'],
-        )
-ext3 = Extension(name='gnssrefl.gnsssnrbigger', 
-        sources=['gnssrefl/gnsssnrbigger.f'], 
-        f2py_options=['--verbose'],
-        )
-ext4 = Extension(name='gnssrefl.xnmeasnr', 
-        sources=['gnssrefl/xnmeasnr.f'], 
-        f2py_options=['--verbose'],
-        )
+ext2 = Extension(
+    name="gnssrefl.gnsssnr",
+    sources=["gnssrefl/gnsssnr.f"],
+    f2py_options=["--verbose"],
+)
+ext3 = Extension(
+    name="gnssrefl.gnsssnrbigger",
+    sources=["gnssrefl/gnsssnrbigger.f"],
+    f2py_options=["--verbose"],
+)
+ext4 = Extension(
+    name="gnssrefl.xnmeasnr",
+    sources=["gnssrefl/xnmeasnr.f"],
+    f2py_options=["--verbose"],
+)
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
-requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
+requirements = [
+    "numpy",
+    "wget",
+    "scipy",
+    "matplotlib",
+    "requests",
+    "progress",
+    "astropy",
+    "simplekml",
+    "earthscope-sdk",
+]
 setup(
     name="gnssrefl",
-    version="1.4.2",
+    version="1.4.3",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
     include_package_data=True,
-    entry_points ={ 
-        'console_scripts': [ 
-            'gnssir = gnssrefl.gnssir_cl:main',
-            'rinex2snr = gnssrefl.rinex2snr_cl:main',
-            'daily_avg = gnssrefl.daily_avg_cl:main',
-            'quickLook= gnssrefl.quickLook_cl:main',
-            'download_rinex = gnssrefl.download_rinex:main',
-            'download_orbits = gnssrefl.download_orbits:main',
-            'gnssir_input = gnssrefl.gnssir_input:main',
-            'ymd = gnssrefl.ymd:main',
-            'ydoy = gnssrefl.ydoy:main',
-            'xyz2llh = gnssrefl.xyz2llh:main',
-            'llh2xyz = gnssrefl.llh2xyz:main',
-            'prn2gps = gnssrefl.prn2gps:main',
-            'download_tides = gnssrefl.download_tides:main',
-            'subdaily= gnssrefl.subdaily_cl:main',
-            'gpsweek = gnssrefl.gpsweek:main',
-            'nmea2snr= gnssrefl.nmea2snr_cl:main',
-            'installexe= gnssrefl.installexe_cl:main',
-            'download_unr = gnssrefl.download_unr:main',
-            'query_unr= gnssrefl.query_unr:main',
-            'mp1mp2= gnssrefl.computemp1mp2:main',
-            'download_teqc = gnssrefl.download_teqc:main',
-            'rinex3_rinex2= gnssrefl.rinex3_rinex2:main',
-            'veg_multiyr= gnssrefl.veg_multiyr:main',
-            'check_rinex_file= gnssrefl.check_rinex_file:main',
-            'rinex3_snr= gnssrefl.rinex3_snr:main',
-            'rt_rinex3_snr= gnssrefl.rt_rinex3_snr:main',
-            'filesizes= gnssrefl.filesizes:main',
-            'invsnr= gnssrefl.invsnr_cl:main',
-            'invsnr_input= gnssrefl.invsnr_input:main',
-            'vwc_input= gnssrefl.vwc_input:main',
-            'phase= gnssrefl.quickPhase:main',
-            'refl_zones= gnssrefl.refl_zones_cl:main',
-            'vwc= gnssrefl.vwc_cl:main',
-            'smoosh= gnssrefl.smoosh:main',
-            'smoosh_snr= gnssrefl.smoosh_snr:main',
-            'quickplt= gnssrefl.quickplt:main',
-            'snowdepth= gnssrefl.snowdepth_cl:main',
-            'rh_plot= gnssrefl.rh_plot:main',
-            'nyquist= gnssrefl.nyquist_cl:main',
-            'pickle_dilemma= gnssrefl.pickle_dilemma:main',
-            ], 
-        },
+    entry_points={
+        "console_scripts": [
+            "gnssir = gnssrefl.gnssir_cl:main",
+            "rinex2snr = gnssrefl.rinex2snr_cl:main",
+            "daily_avg = gnssrefl.daily_avg_cl:main",
+            "quickLook= gnssrefl.quickLook_cl:main",
+            "download_rinex = gnssrefl.download_rinex:main",
+            "download_orbits = gnssrefl.download_orbits:main",
+            "gnssir_input = gnssrefl.gnssir_input:main",
+            "ymd = gnssrefl.ymd:main",
+            "ydoy = gnssrefl.ydoy:main",
+            "xyz2llh = gnssrefl.xyz2llh:main",
+            "llh2xyz = gnssrefl.llh2xyz:main",
+            "prn2gps = gnssrefl.prn2gps:main",
+            "download_tides = gnssrefl.download_tides:main",
+            "subdaily= gnssrefl.subdaily_cl:main",
+            "gpsweek = gnssrefl.gpsweek:main",
+            "nmea2snr= gnssrefl.nmea2snr_cl:main",
+            "installexe= gnssrefl.installexe_cl:main",
+            "download_unr = gnssrefl.download_unr:main",
+            "query_unr= gnssrefl.query_unr:main",
+            "mp1mp2= gnssrefl.computemp1mp2:main",
+            "download_teqc = gnssrefl.download_teqc:main",
+            "rinex3_rinex2= gnssrefl.rinex3_rinex2:main",
+            "veg_multiyr= gnssrefl.veg_multiyr:main",
+            "check_rinex_file= gnssrefl.check_rinex_file:main",
+            "rinex3_snr= gnssrefl.rinex3_snr:main",
+            "rt_rinex3_snr= gnssrefl.rt_rinex3_snr:main",
+            "filesizes= gnssrefl.filesizes:main",
+            "invsnr= gnssrefl.invsnr_cl:main",
+            "invsnr_input= gnssrefl.invsnr_input:main",
+            "vwc_input= gnssrefl.vwc_input:main",
+            "phase= gnssrefl.quickPhase:main",
+            "refl_zones= gnssrefl.refl_zones_cl:main",
+            "vwc= gnssrefl.vwc_cl:main",
+            "smoosh= gnssrefl.smoosh:main",
+            "smoosh_snr= gnssrefl.smoosh_snr:main",
+            "quickplt= gnssrefl.quickplt:main",
+            "snowdepth= gnssrefl.snowdepth_cl:main",
+            "rh_plot= gnssrefl.rh_plot:main",
+            "nyquist= gnssrefl.nyquist_cl:main",
+            "pickle_dilemma= gnssrefl.pickle_dilemma:main",
+            "make_meta= gnssrefl.make_meta:main",
+        ],
+    },
     install_requires=requirements,
-    ext_modules = [ext1,ext2,ext3,ext4],
+    ext_modules=[ext1, ext2, ext3, ext4],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

### Comparing `gnssrefl-1.4.2/test/test_gps.py` & `gnssrefl-1.4.3/test/test_gps.py`

 * *Files identical despite different names*

