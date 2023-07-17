# Comparing `tmp/ephysiopy-1.9.24.tar.gz` & `tmp/ephysiopy-1.9.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.24.tar", last modified: Tue Jul 11 11:21:04 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.25.tar", last modified: Mon Jul 17 14:34:41 2023, max compression
```

## Comparing `ephysiopy-1.9.24.tar` & `ephysiopy-1.9.25.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.481640 ephysiopy-1.9.24/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.481640 ephysiopy-1.9.24/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.481640 ephysiopy-1.9.24/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-11 11:20:56.000000 ephysiopy-1.9.24/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32382 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:21:04.481640 ephysiopy-1.9.24/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-11 11:21:04.000000 ephysiopy-1.9.24/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-11 11:21:04.000000 ephysiopy-1.9.24/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:21:04.000000 ephysiopy-1.9.24/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 11:21:04.000000 ephysiopy-1.9.24/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 11:21:04.000000 ephysiopy-1.9.24/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 11:21:04.485640 ephysiopy-1.9.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-11 11:20:57.000000 ephysiopy-1.9.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/cluster_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/setup.py
```

### Comparing `ephysiopy-1.9.24/LICENSE` & `ephysiopy-1.9.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/PKG-INFO` & `ephysiopy-1.9.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.24
+Version: 1.9.25
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.24/README.md` & `ephysiopy-1.9.25/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.25/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.25/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.25/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.25/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/binning.py` & `ephysiopy-1.9.25/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.25/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.25/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.25/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.25/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.25/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.25/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.25/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.25/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/common/utils.py` & `ephysiopy-1.9.25/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.25/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.25/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/io/recording.py` & `ephysiopy-1.9.25/ephysiopy/io/recording.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def memmapBinaryFile(path2file: str, n_channels=384, **kwargs) -> np.ndarray:
     """
     Returns a numpy memmap of the int16 data in the
     file path2file, if present
     """
     import os
 
-    if("data_type" in kwargs.keys()):
+    if "data_type" in kwargs.keys():
         data_type = kwargs["data_type"]
     else:
         data_type = np.int16
 
     if os.path.exists(path2file):
         # make sure n_channels is int as could be str
         n_channels = int(n_channels)
@@ -103,15 +103,16 @@
     ACQUISITIONBOARD = 3
     NWB = 4
 
 
 Xml2RecordingKind = {
     "Acquisition Board": RecordingKind.ACQUISITIONBOARD,
     "Neuropix-PXI": RecordingKind.NEUROPIXELS,
-    "Rhythm FPGA": RecordingKind.FPGA}
+    "Rhythm FPGA": RecordingKind.FPGA,
+}
 
 
 class TrackingKind(Enum):
     POSTRACKER = 1
     TRACKINGPLUGIN = 2
 
 
@@ -277,19 +278,15 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def load_ttl(self, *args, **kwargs):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def get_spike_times(self,
-                        cluster: int,
-                        tetrode: int = None,
-                        *args,
-                        **kwargs):
+    def get_spike_times(self, cluster: int, tetrode: int, *args, **kwargs):
         """Returns the times of an individual cluster"""
         raise NotImplementedError
 
 
 class AxonaTrial(TrialInterface):
     def __init__(self, pname: Path, **kwargs) -> None:
         super().__init__(pname, **kwargs)
@@ -308,14 +305,15 @@
 
     @settings.setter
     def settings(self, value) -> None:
         self.__settings = value
 
     def load_lfp(self, pname: Path, *args, **kwargs):
         from ephysiopy.axona.axonaIO import EEG
+
         if "egf" in args:
             lfp = EEG(self.pname, egf=1)
         else:
             lfp = EEG(self.pname)
         if lfp is not None:
             self.EEGCalcs = EEGCalcsGeneric(lfp.sig, lfp.sample_rate)
 
@@ -324,62 +322,67 @@
 
     def load_cluster_data(self, *args, **kwargs):
         pass
 
     def load_settings(self, *args, **kwargs):
         return self.settings
 
-    def load_pos_data(self, pname: Path,
-                      ppm: int = 300, jumpmax: int = 100,
-                      *args, **kwargs) -> None:
+    def load_pos_data(
+        self, pname: Path, ppm: int = 300, jumpmax: int = 100, *args, **kwargs
+    ) -> None:
         try:
             AxonaPos = Pos(Path(pname))
             P = PosCalcsGeneric(
                 AxonaPos.led_pos[:, 0],
                 AxonaPos.led_pos[:, 1],
                 cm=True,
                 ppm=ppm,
-                jumpmax=jumpmax
+                jumpmax=jumpmax,
             )
             P.xyTS = AxonaPos.ts
-            P.sample_rate = AxonaPos.getHeaderVal(
-                AxonaPos.header, "sample_rate")
+            P.sample_rate = AxonaPos.getHeaderVal(AxonaPos.header, "sample_rate")
             P.postprocesspos()
             print("Loaded pos data")
             self.PosCalcs = P
         except IOError:
             print("Couldn't load the pos data")
 
     def load_ttl(self, *args, **kwargs):
         from ephysiopy.axona.axonaIO import Stim
+
         self.ttl_data = Stim(self.pname)
 
-    def get_spike_times(self, cluster: int, tetrode: int = None,
-                        *args, **kwargs):
+    def get_spike_times(self, cluster: int, tetrode: int = None, *args, **kwargs):
         if tetrode is not None:
             return self.TETRODE.get_spike_samples(tetrode, cluster)
 
 
 class OpenEphysBase(TrialInterface):
     def __init__(self, pname: Path, **kwargs) -> None:
         super().__init__(pname, **kwargs)
         setattr(self, "sync_message_file", None)
         self.load_settings()
-        # The numbers after the strings in this list are the node id's 
+        # The numbers after the strings in this list are the node id's
         # in openephys
-        record_methods = ["Acquisition Board [0-9][0-9][0-9]",
-                          "Neuropix-PXI [0-9][0-9][0-9]",
-                          "Sources/Neuropix-PXI [0-9][0-9][0-9]",
-                          "Rhythm FPGA [0-9][0-9][0-9]",
-                          "Sources/Rhythm FPGA [0-9][0-9][0-9]"]
-        rec_method = [re.search(m,k).string for k in self.settings.processors.keys() 
-                       for m in record_methods if re.search(m,k) is not None][0]
-        if 'Sources/' in rec_method:
-            rec_method = rec_method.lstrip('Sources/')
-        
+        record_methods = [
+            "Acquisition Board [0-9][0-9][0-9]",
+            "Neuropix-PXI [0-9][0-9][0-9]",
+            "Sources/Neuropix-PXI [0-9][0-9][0-9]",
+            "Rhythm FPGA [0-9][0-9][0-9]",
+            "Sources/Rhythm FPGA [0-9][0-9][0-9]",
+        ]
+        rec_method = [
+            re.search(m, k).string
+            for k in self.settings.processors.keys()
+            for m in record_methods
+            if re.search(m, k) is not None
+        ][0]
+        if "Sources/" in rec_method:
+            rec_method = rec_method.lstrip("Sources/")
+
         self.rec_kind = Xml2RecordingKind[rec_method.rpartition(" ")[0]]
 
         # Attempt to find the files contained in the parent directory
         # related to the recording with the default experiment and
         # recording name
         self.find_files(pname)
         self.sample_rate = None
@@ -391,43 +394,62 @@
             self.sample_rate = float(self.sample_rate)
         self.channel_count = self.settings.processors[rec_method].channel_count
         if self.channel_count is None:
             if self.rec_kind == RecordingKind.NEUROPIXELS:
                 self.channel_count = 384
         self.kilodata = None
 
-    def get_spike_times(self, cluster: int, tetrode: int = None,
-                        *args, **kwargs):
+    def _get_recording_start_time(self) -> float:
+        """
+        Get the recording start time from the sync_messages.txt file
+        """
+        recording_start_time = 0.0
+        if self.sync_message_file is not None:
+            with open(self.sync_message_file, "r") as f:
+                sync_strs = f.read()
+            sync_lines = sync_strs.split("\n")
+            for line in sync_lines:
+                if "Start Time" in line:
+                    tokens = line.split(":")
+                    start_time = int(tokens[-1])
+                    sample_rate = int(tokens[0].split("@")[-1].strip().split()[0])
+                    recording_start_time = start_time / float(sample_rate)
+        return recording_start_time
+
+    def get_spike_times(self, cluster: int, tetrode: int = None, *args, **kwargs):
         ts = self.clusterData.spk_times
         if cluster in self.clusterData.spk_clusters:
             times = ts[self.clusterData.spk_clusters == cluster]
             return times.astype(np.int64) / self.sample_rate
         else:
             warnings.warn("Cluster not present")
 
     def load_lfp(self, pname: Path, *args, **kwargs):
-        '''
+        """
         Valid kwargs are:
         'target_sample_rate' - int
             the sample rate to downsample to from the original
-        '''
+        """
         from scipy import signal
+
         if self.path2LFPdata is not None:
             lfp = memmapBinaryFile(
                 os.path.join(self.path2LFPdata, "continuous.dat"),
-                n_channels=self.channel_count)
+                n_channels=self.channel_count,
+            )
             channel = 0
             if "channel" in kwargs.keys():
                 channel = kwargs["channel"]
             target_sample_rate = 500
             if "target_sample_rate" in kwargs.keys():
                 target_sample_rate = kwargs["target_sample_rate"]
             n_samples = np.shape(lfp[channel, :])[0]
-            sig = signal.resample(lfp[channel, :], int(
-                n_samples / self.sample_rate) * target_sample_rate)
+            sig = signal.resample(
+                lfp[channel, :], int(n_samples / self.sample_rate) * target_sample_rate
+            )
             self.EEGCalcs = EEGCalcsGeneric(sig, target_sample_rate)
 
     def load_neural_data(self, pname: Path, *args, **kwargs) -> None:
         pass
 
     def load_settings(self, *args, **kwargs):
         if self._settings is None:
@@ -445,69 +467,68 @@
                     try:
                         clusterData.removeKSNoiseClusters()
                         print("Removed noise clusters")
                     except Exception:
                         pass
         self.clusterData = clusterData
 
-    def load_pos_data(self, ppm: int = 300, jumpmax: int = 100,
-                      *args, **kwargs) -> None:
+    def load_pos_data(
+        self, ppm: int = 300, jumpmax: int = 100, *args, **kwargs
+    ) -> None:
         # Only sub-class that doesn't use this is OpenEphysNWB
         # which needs updating
         # TODO: Update / overhaul OpenEphysNWB
         # Load the start time from the sync_messages file
         if "cm" in kwargs:
             cm = kwargs["cm"]
         else:
             cm = True
-        recording_start_time = 0
-        if self.sync_message_file is not None:
-            with open(self.sync_message_file, "r") as f:
-                sync_strs = f.read()
-            sync_lines = sync_strs.split("\n")
-            for line in sync_lines:
-                if "Start Time" in line:
-                    tokens = line.split(":")
-                    start_time = int(tokens[-1])
-                    sample_rate = int(tokens[0].split("@")
-                                      [-1].strip().split()[0])
-                    recording_start_time = start_time / sample_rate
+
+        recording_start_time = self._get_recording_start_time()
+
         if self.path2PosData is not None:
-            pos_method = ["Pos Tracker [0-9][0-9][0-9]",
-                          "PosTracker [0-9][0-9][0-9]",
-                          "TrackMe [0-9][0-9][0-9]"]
-            pos_kind = [re.search(m,k).string for k in self.settings.processors.keys() 
-                       for m in pos_method if re.search(m,k) is not None][0]
-            if 'Sources/' in pos_method:
-                pos_method = pos_method.lstrip('Sources/')
+            pos_method = [
+                "Pos Tracker [0-9][0-9][0-9]",
+                "PosTracker [0-9][0-9][0-9]",
+                "TrackMe [0-9][0-9][0-9]",
+                "TrackingPlugin [0-9][0-9][0-9]",
+            ]
+            pos_plugin_name = [
+                re.search(m, k).string
+                for k in self.settings.processors.keys()
+                for m in pos_method
+                if re.search(m, k) is not None
+            ][0]
+            if "Sources/" in pos_plugin_name:
+                pos_plugin_name = pos_plugin_name.lstrip("Sources/")
 
             pos_data_type = getattr(self, "pos_data_type", "PosTracker")
             if pos_data_type == "PosTracker" or pos_data_type == "Pos Tracker":
                 print("Loading PosTracker data...")
-                pos_data = np.load(os.path.join(
-                    self.path2PosData, "data_array.npy"))
+                pos_data = np.load(os.path.join(self.path2PosData, "data_array.npy"))
             if pos_data_type == "TrackingPlugin":
                 print("Loading Tracking Plugin data...")
                 pos_data = loadTrackingPluginData(
                     os.path.join(self.path2PosData, "data_array.npy")
                 )
             pos_ts = np.load(os.path.join(self.path2PosData, "timestamps.npy"))
             # pos_ts in seconds
             pos_ts = np.ravel(pos_ts)
             if pos_data_type == "TrackMe":
                 print("Loading TrackMe data...")
                 n_pos_chans = int(
-                    self.settings.processors[pos_kind].channel_count)
+                    self.settings.processors[pos_plugin_name].channel_count
+                )
                 pos_data = loadTrackMePluginData(
                     Path(os.path.join(self.path2PosData, "continuous.dat")),
-                    n_channels=n_pos_chans)
-                pos_ts = loadTrackMeTTLTimestamps(
-                    Path(self.path2EventsData))
-                pos_ts = pos_ts[0:len(pos_data)]
-            sample_rate = self.settings.processors[pos_kind].sample_rate
+                    n_channels=n_pos_chans,
+                )
+                pos_ts = loadTrackMeTTLTimestamps(Path(self.path2EventsData))
+                pos_ts = pos_ts[0 : len(pos_data)]
+            sample_rate = self.settings.processors[pos_plugin_name].sample_rate
             sample_rate = float(sample_rate)
             if pos_data_type != "TrackMe":
                 xyTS = pos_ts - recording_start_time
             else:
                 xyTS = pos_ts
             if self.sync_message_file is not None:
                 recording_start_time = xyTS[0]
@@ -529,37 +550,38 @@
                 "Could not find the pos data. \
                 Make sure there is a pos_data folder with data_array.npy \
                 and timestamps.npy in"
             )
         self.recording_start_time = recording_start_time
 
     def load_ttl(self, *args, **kwargs):
-        '''
+        """
         Valid kwargs are:
         StimControl_id: str
             This is the string "StimControl [0-9][0-9][0-9]" where the numbers
             are the node id in the openephys signal chain
         TTL_channel_number: int
-            The integer value in the "states.npy" file that corresponds to the 
-            identity of the TTL input on the Digital I/O board on the 
+            The integer value in the "states.npy" file that corresponds to the
+            identity of the TTL input on the Digital I/O board on the
             openephys recording system. i.e. if there is input to BNC port 3 on
             the digital I/O board then values of 3 in the states.npy file are high
             TTL values on this input and -3 are low TTL values (I think)
-        '''
+        """
         ttl_ts = np.load(os.path.join(self.path2EventsData, "timestamps.npy"))
         states = np.load(os.path.join(self.path2EventsData, "states.npy"))
+        recording_start_time = self._get_recording_start_time()
         if "StimControl_id" in kwargs.keys():
-            stim_id = kwargs['StimControl_id']
+            stim_id = kwargs["StimControl_id"]
             duration = getattr(self.settings.processors[stim_id], "Duration")
             setattr(self, "stim_duration", int(duration))
         if "TTL_channel_number" in kwargs.keys():
             chan = kwargs["TTL_channel_number"]
-            high_ttl = ttl_ts[states==chan]
+            high_ttl = ttl_ts[states == chan]
             # get into ms
-            high_ttl = high_ttl * 1000.
+            high_ttl = (high_ttl * 1000.0) - recording_start_time
             setattr(self, "ttl_timestamps", high_ttl)
 
     def find_files(
         self,
         pname_root: str,
         experiment_name: str = "experiment1",
         rec_name: str = "recording1",
@@ -568,51 +590,53 @@
         PosTracker_match = (
             exp_name / rec_name / "events" / "*Pos_Tracker*/BINARY_group*"
         )
         TrackingPlugin_match = (
             exp_name / rec_name / "events" / "*Tracking_Port*/BINARY_group*"
         )
         TrackMe_match = (
-            exp_name / rec_name /
-            "continuous" / "TrackMe-[0-9][0-9][0-9].TrackingNode"
+            exp_name / rec_name / "continuous" / "TrackMe-[0-9][0-9][0-9].TrackingNode"
         )
         sync_file_match = exp_name / rec_name
         acq_method = ""
         if self.rec_kind == RecordingKind.NEUROPIXELS:
             # the old OE NPX plugins saved two forms of the data,
             # one for AP @30kHz and one for LFP @??Hz
             # the newer plugin saves only the 30kHz data. Also, the
             # 2.0 probes are saved with Probe[A-Z] appended to the end
             # of the folder
             # the older way:
             acq_method = "Neuropix-PXI-[0-9][0-9][0-9]."
-            APdata_match = (exp_name / rec_name /
-                            "continuous" / (acq_method + "0"))
-            LFPdata_match = (exp_name / rec_name /
-                             "continuous" / (acq_method + "1"))
+            APdata_match = exp_name / rec_name / "continuous" / (acq_method + "0")
+            LFPdata_match = exp_name / rec_name / "continuous" / (acq_method + "1")
             # the new way:
-            Rawdata_match = (exp_name / rec_name /
-                             "continuous" / (acq_method + "Probe[A-Z]"))
+            Rawdata_match = (
+                exp_name / rec_name / "continuous" / (acq_method + "Probe[A-Z]")
+            )
         elif self.rec_kind == RecordingKind.FPGA:
             acq_method = "Rhythm_FPGA-[0-9][0-9][0-9]."
-            APdata_match = (exp_name / rec_name /
-                            "continuous" / (acq_method + "0"))
-            LFPdata_match = (exp_name / rec_name /
-                             "continuous" / (acq_method + "1"))
-            Rawdata_match = (exp_name / rec_name /
-                             "continuous" / (acq_method + "Probe[A-Z]"))
+            APdata_match = exp_name / rec_name / "continuous" / (acq_method + "0")
+            LFPdata_match = exp_name / rec_name / "continuous" / (acq_method + "1")
+            Rawdata_match = (
+                exp_name / rec_name / "continuous" / (acq_method + "Probe[A-Z]")
+            )
         else:
             acq_method = "Acquisition_Board-[0-9][0-9][0-9].*"
             APdata_match = exp_name / rec_name / "continuous" / acq_method
             LFPdata_match = exp_name / rec_name / "continuous" / acq_method
-            Rawdata_match = (exp_name / rec_name /
-                             "continuous" / (acq_method + "Probe[A-Z]"))
+            Rawdata_match = (
+                exp_name / rec_name / "continuous" / (acq_method + "Probe[A-Z]")
+            )
         Events_match = (
             # only dealing with a single TTL channel at the moment
-            exp_name / rec_name / "events" / acq_method / "TTL"
+            exp_name
+            / rec_name
+            / "events"
+            / acq_method
+            / "TTL"
         )
 
         if pname_root is None:
             pname_root = self.pname_root
 
         for d, c, f in os.walk(pname_root):
             for ff in f:
@@ -627,17 +651,15 @@
                         if PurePath(d).match("*pos_data*"):
                             if self.path2PosData is None:
                                 self.path2PosData = os.path.join(d)
                                 print(f"Pos data at: {self.path2PosData}")
                         if PurePath(d).match(str(TrackingPlugin_match)):
                             if self.path2PosData is None:
                                 self.path2PosData = os.path.join(d)
-                                setattr(self,
-                                        "pos_data_type",
-                                        "TrackingPlugin")
+                                setattr(self, "pos_data_type", "TrackingPlugin")
                                 print(f"Pos data at: {self.path2PosData}")
                     if "continuous.dat" in ff:
                         if PurePath(d).match(str(APdata_match)):
                             self.path2APdata = os.path.join(d)
                             print(f"Continuous AP data at: {self.path2APdata}")
                             self.path2APOEBin = Path(d).parents[1]
                         if PurePath(d).match(str(LFPdata_match)):
@@ -674,27 +696,22 @@
 
     def load_neural_data(self, pname: Path, *args, **kwargs) -> None:
         pass
 
     def load_settings(self, *args, **kwargs):
         return super().load_settings()
 
-    def load_pos_data(self, ppm: int = 300, jumpmax: int = 100,
-                      *args, **kwargs) -> None:
+    def load_pos_data(
+        self, ppm: int = 300, jumpmax: int = 100, *args, **kwargs
+    ) -> None:
         with h5py.File(os.path.join(self.path2NWBData), mode="r") as nwbData:
             xy = np.array(nwbData[self.path2PosData + "/data"])
             xy = xy[:, 0:2]
             ts = np.array(nwbData[self.path2PosData]["timestamps"])
-            P = PosCalcsGeneric(
-                xy[0, :],
-                xy[1, :],
-                cm=True,
-                ppm=ppm,
-                jumpmax=jumpmax
-            )
+            P = PosCalcsGeneric(xy[0, :], xy[1, :], cm=True, ppm=ppm, jumpmax=jumpmax)
             P.xyTS = ts
             P.sample_rate = 1.0 / np.mean(np.diff(ts))
             P.postprocesspos()
             print("Loaded pos data")
             self.PosCalcs = P
 
     def find_files(
```

### Comparing `ephysiopy-1.9.24/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.25/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.25/ephysiopy/openephys2py/OESettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,29 +359,14 @@
         import os
 
         for d, _, f in os.walk(pname):
             for ff in f:
                 if "settings.xml" in ff:
                     self.filename = os.path.join(d, "settings.xml")
         self.tree = None
-        """
-        It's not uncommon to have > 1 of the same type of processor, i.e.
-        2 x bandpass filter to look at LFP and APs. This deals with that...
-        """
-        self.possible_processors = OrderedDict([
-            ("Pos Tracker", PosTracker()),
-            ("PosTracker", PosTracker()),
-            ("Rhythm FPGA", RhythmFPGA()),
-            ("Neuropix-PXI", NeuropixPXI()),
-            ("Acquisition Board", AcquisitionBoard()),
-            ("Spike Sorter", SpikeSorter()),
-            ("TrackMe", TrackMe()),
-            ("Record Node", RecordNode()),
-            ("StimControl", StimControl())
-        ])
         self.processors = OrderedDict()
         self.record_nodes = OrderedDict()
         self.tracker_params = {}
         self.stimcontrol_params = {}
         self.load()
         self.parse()
```

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.25/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.25/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.24/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.25/ephysiopy/visualise/plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,34 +17,36 @@
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         ax = func(*args, **kwargs)
         plt.setp(ax.get_xticklabels(), visible=False)
         plt.setp(ax.get_yticklabels(), visible=False)
         ax.axes.get_xaxis().set_visible(False)
         ax.axes.get_yaxis().set_visible(False)
-        if 'polar' in ax.name:
+        if "polar" in ax.name:
             ax.set_rticks([])
         else:
-            ax.spines['right'].set_visible(False)
-            ax.spines['top'].set_visible(False)
-            ax.spines['bottom'].set_visible(False)
-            ax.spines['left'].set_visible(False)
+            ax.spines["right"].set_visible(False)
+            ax.spines["top"].set_visible(False)
+            ax.spines["bottom"].set_visible(False)
+            ax.spines["left"].set_visible(False)
         return ax
+
     return wrapper
 
 
 jet_cmap = matplotlib.cm.get_cmap("jet")
 grey_cmap = matplotlib.cm.get_cmap("gray_r")
 
 
 class FigureMaker(object):
-    '''
+    """
     A mixin class for TrialInterface that deals solely with
     producing graphical output
-    '''
+    """
+
     def __init__(self):
         self.PosCalcs = None
 
     def initialise(self):
         xy = getattr(self.PosCalcs, "xy")
         hdir = getattr(self.PosCalcs, "dir")
         speed = getattr(self.PosCalcs, "speed")
@@ -53,144 +55,158 @@
         pos_weights = None
         if hdir is not None:
             if np.ma.is_masked(hdir):
                 pos_weights = np.array(~hdir.mask).astype(int)
             else:
                 pos_weights = np.ones_like(hdir)
         self.RateMap = RateMap(
-            xy=xy, hdir=hdir, speed=speed, pos_weights=pos_weights, ppm=ppm,
-            xyInCms=True)
-        self.RateMap.x_lims = getattr(self, 'x_lims', None)  # 2-tuple
-        self.RateMap.y_lims = getattr(self, 'y_lims', None)
+            xy=xy,
+            hdir=hdir,
+            speed=speed,
+            pos_weights=pos_weights,
+            ppm=ppm,
+            xyInCms=True,
+        )
+        self.RateMap.x_lims = getattr(self, "x_lims", None)  # 2-tuple
+        self.RateMap.y_lims = getattr(self, "y_lims", None)
 
     def getSpikePosIndices(self, spk_times: np.ndarray):
-        pos_times = getattr(self.PosCalcs, 'xyTS')
+        pos_times = getattr(self.PosCalcs, "xyTS")
         idx = np.searchsorted(pos_times, spk_times)
         idx[idx == len(pos_times)] = idx[idx == len(pos_times)] - 1
         return idx
 
     def makeSummaryPlot(self, spk_times: np.ndarray):
         fig = plt.figure()
         ax = plt.subplot(221)
         self.makeSpikePathPlot(spk_times, ax=ax, markersize=2)
         ax = plt.subplot(222)
         self.makeRateMap(spk_times, ax=ax)
-        ax = plt.subplot(223, projection='polar')
+        ax = plt.subplot(223, projection="polar")
         self.makeHDPlot(spk_times, ax=ax)
         ax = plt.subplot(224)
         try:
             self.makeSAC(spk_times, ax=ax)
         except IndexError:
             pass
         return fig
 
     @stripAxes
-    def makeRateMap(self, spk_times: np.ndarray,
-                    ax: matplotlib.axes = None) -> matplotlib.axes:
+    def makeRateMap(
+        self, spk_times: np.ndarray, ax: matplotlib.axes = None
+    ) -> matplotlib.axes:
         if not self.RateMap:
             self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
-        spk_weights = np.bincount(
-            spk_times_in_pos_samples, minlength=self.npos)
+        spk_weights = np.bincount(spk_times_in_pos_samples, minlength=self.npos)
         rmap = self.RateMap.getMap(spk_weights)
         ratemap = np.ma.MaskedArray(rmap[0], np.isnan(rmap[0]), copy=True)
         x, y = np.meshgrid(rmap[1][1][0:-1].data, rmap[1][0][0:-1].data)
         vmax = np.nanmax(np.ravel(ratemap))
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax.pcolormesh(
-            x, y, ratemap, cmap=jet_cmap, edgecolors='face',
-            vmax=vmax, shading='auto')
-        ax.set_aspect('equal')
+            x, y, ratemap, cmap=jet_cmap, edgecolors="face", vmax=vmax, shading="auto"
+        )
+        ax.set_aspect("equal")
         return ax
 
     @stripAxes
-    def makeSpikePathPlot(self, spk_times: np.ndarray = None,
-                          ax: matplotlib.axes = None,
-                          **kwargs) -> matplotlib.axes:
+    def makeSpikePathPlot(
+        self, spk_times: np.ndarray = None, ax: matplotlib.axes = None, **kwargs
+    ) -> matplotlib.axes:
         if not self.RateMap:
             self.initialise()
-        if 'c' in kwargs:
-            col = kwargs.pop('c')
+        if "c" in kwargs:
+            col = kwargs.pop("c")
         else:
             col = tcols.colours[1]
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
-        ax.plot(self.PosCalcs.xy[0, :],
-                self.PosCalcs.xy[1, :], c=tcols.colours[0], zorder=1)
-        ax.set_aspect('equal')
+        ax.plot(
+            self.PosCalcs.xy[0, :], self.PosCalcs.xy[1, :], c=tcols.colours[0], zorder=1
+        )
+        ax.set_aspect("equal")
         if spk_times is not None:
             idx = self.getSpikePosIndices(spk_times)
-            ax.plot(self.PosCalcs.xy[0, idx],
-                    self.PosCalcs.xy[1, idx], 's', c=col, **kwargs)
+            ax.plot(
+                self.PosCalcs.xy[0, idx], self.PosCalcs.xy[1, idx], "s", c=col, **kwargs
+            )
         return ax
 
     @stripAxes
-    def makeSAC(self, spk_times: np.array = None,
-                ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
+    def makeSAC(
+        self, spk_times: np.array = None, ax: matplotlib.axes = None, **kwargs
+    ) -> matplotlib.axes:
         if not self.RateMap:
             self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
-        spk_weights = np.bincount(
-            spk_times_in_pos_samples, minlength=self.npos)
+        spk_weights = np.bincount(spk_times_in_pos_samples, minlength=self.npos)
         rmap = self.RateMap.getMap(spk_weights)
         nodwell = ~np.isfinite(rmap[0])
         sac = self.RateMap.autoCorr2D(rmap[0], nodwell)
         from ephysiopy.common.gridcell import SAC
+
         S = SAC()
         measures = S.getMeasures(sac)
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax = self.show_SAC(sac, measures, ax)
         return ax
 
     @stripAxes
-    def makeHDPlot(self, spk_times: np.array = None,
-                   ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
+    def makeHDPlot(
+        self, spk_times: np.array = None, ax: matplotlib.axes = None, **kwargs
+    ) -> matplotlib.axes:
         if not self.RateMap:
             self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
-        spk_weights = np.bincount(
-            spk_times_in_pos_samples, minlength=self.npos)
+        spk_weights = np.bincount(spk_times_in_pos_samples, minlength=self.npos)
         rmap = self.RateMap.getMap(spk_weights, varType=VariableToBin.DIR)
         if ax is None:
             fig = plt.figure()
-            ax = fig.add_subplot(111, projection='polar')
+            ax = fig.add_subplot(111, projection="polar")
         # need to deal with the case where the axis is supplied but
         # is not polar. deal with polar first
         theta = np.deg2rad(rmap[1][0])
         ax.clear()
         r = rmap[0]  # in samples so * pos sample_rate
         r = np.insert(r, -1, r[0])
-        if 'polar' in ax.name:
+        if "polar" in ax.name:
             ax.plot(theta, r)
-            if 'fill' in kwargs:
+            if "fill" in kwargs:
                 ax.fill(theta, r, alpha=0.5)
-            ax.set_aspect('equal')
+            ax.set_aspect("equal")
         else:
             pass
 
         # See if we should add the mean resultant vector (mrv)
-        if 'add_mrv' in kwargs:
+        if "add_mrv" in kwargs:
             from ephysiopy.common.statscalcs import mean_resultant_vector
+
             angles = self.PosCalcs.dir[spk_times_in_pos_samples]
             r, th = mean_resultant_vector(np.deg2rad(angles))
-            ax.plot([th, th], [0, r*np.max(rmap[0])], 'r')
-        if 'polar' in ax.name:
+            ax.plot([th, th], [0, r * np.max(rmap[0])], "r")
+        if "polar" in ax.name:
             ax.set_thetagrids([0, 90, 180, 270])
         return ax
 
     # @stripAxes
     def makeSpeedVsRatePlot(
-            self, spk_times: np.array, minSpeed: float = 0.0,
-            maxSpeed: float = 40.0, sigma: float = 3.0,
-            ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
+        self,
+        spk_times: np.array,
+        minSpeed: float = 0.0,
+        maxSpeed: float = 40.0,
+        sigma: float = 3.0,
+        ax: matplotlib.axes = None,
+        **kwargs
+    ) -> matplotlib.axes:
         """
         Plots the instantaneous firing rate of a cell against running speed
         Also outputs a couple of measures as with Kropff et al., 2015; the
         Pearsons correlation and the depth of modulation (dom) - see below for
         details
         """
         self.initialise()
@@ -204,134 +220,163 @@
         speed_filt = np.ma.MaskedArray(speed)
         speed_filt = np.ma.masked_where(speed_filt < minSpeed, speed_filt)
         speed_filt = np.ma.masked_where(speed_filt > maxSpeed, speed_filt)
         from ephysiopy.common.spikecalcs import SpikeCalcsGeneric
 
         x1 = spk_times_in_pos_samples
         S = SpikeCalcsGeneric(x1)
-        spk_sm = S.smoothSpikePosCount(
-            x1, self.PosCalcs.xyTS.shape[0], sigma, None)
+        spk_sm = S.smoothSpikePosCount(x1, self.PosCalcs.xyTS.shape[0], sigma, None)
         spk_sm = np.ma.MaskedArray(spk_sm, mask=np.ma.getmask(speed_filt))
         spd_dig = np.digitize(speed_filt, spd_bins, right=True)
-        mn_rate = np.array([np.ma.mean(
-            spk_sm[spd_dig == i]) for i in range(0, len(spd_bins))])
-        var = np.array([np.ma.std(
-            spk_sm[spd_dig == i]) for i in range(0, len(spd_bins))])
-        np.array([np.ma.sum(
-            spk_sm[spd_dig == i]) for i in range(0, len(spd_bins))])
+        mn_rate = np.array(
+            [np.ma.mean(spk_sm[spd_dig == i]) for i in range(0, len(spd_bins))]
+        )
+        var = np.array(
+            [np.ma.std(spk_sm[spd_dig == i]) for i in range(0, len(spd_bins))]
+        )
+        np.array([np.ma.sum(spk_sm[spd_dig == i]) for i in range(0, len(spd_bins))])
         fig = plt.figure()
         ax = fig.add_subplot(111)
-        ax.errorbar(
-            spd_bins, mn_rate * self.PosCalcs.sample_rate,
-            yerr=var, color='k')
+        ax.errorbar(spd_bins, mn_rate * self.PosCalcs.sample_rate, yerr=var, color="k")
         ax.set_xlim(spd_bins[0], spd_bins[-1])
-        plt.xticks([spd_bins[0], spd_bins[-1]], ['0', '{:.2g}'.format(
-            spd_bins[-1])], fontweight='normal', size=6)
-        plt.yticks([0, np.nanmax(
-            mn_rate)*self.PosCalcs.sample_rate], ['0', '{:.2f}'.format(
-                np.nanmax(mn_rate))], fontweight='normal', size=6)
+        plt.xticks(
+            [spd_bins[0], spd_bins[-1]],
+            ["0", "{:.2g}".format(spd_bins[-1])],
+            fontweight="normal",
+            size=6,
+        )
+        plt.yticks(
+            [0, np.nanmax(mn_rate) * self.PosCalcs.sample_rate],
+            ["0", "{:.2f}".format(np.nanmax(mn_rate))],
+            fontweight="normal",
+            size=6,
+        )
         return ax
 
     # @stripAxes
-    def makeSpeedVsHeadDirectionPlot(self, spk_times: np.array,
-                                     ax: matplotlib.axes = None,
-                                     **kwargs) -> matplotlib.axes:
+    def makeSpeedVsHeadDirectionPlot(
+        self, spk_times: np.array, ax: matplotlib.axes = None, **kwargs
+    ) -> matplotlib.axes:
         self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
         idx = np.array(spk_times_in_pos_samples, dtype=int)
         if np.ma.is_masked(self.PosCalcs.speed):
             w = self.speed.mask
             w = np.array(~w, dtype=int)
         else:
             w = np.bincount(idx, minlength=self.PosCalcs.speed.shape[0])
         dir_bins = np.arange(0, 360, 6)
         spd_bins = np.arange(0, 30, 1)
-        h = np.histogram2d(self.PosCalcs.dir,
-                           self.PosCalcs.speed,
-                           [dir_bins, spd_bins], weights=w)
+        h = np.histogram2d(
+            self.PosCalcs.dir, self.PosCalcs.speed, [dir_bins, spd_bins], weights=w
+        )
         from ephysiopy.common.utils import blurImage
-        im = blurImage(h[0], 5, ftype='gaussian')
+
+        im = blurImage(h[0], 5, ftype="gaussian")
         im = np.ma.MaskedArray(im)
         # mask low rates...
         im = np.ma.masked_where(im <= 1, im)
         # ... and where less than 0.5% of data is accounted for
         x, y = np.meshgrid(dir_bins, spd_bins)
         vmax = np.max(np.ravel(im))
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
-        ax.pcolormesh(x, y, im.T, cmap=jet_cmap,
-                      edgecolors='face',
-                      vmax=vmax, shading='auto')
-        plt.xticks([90, 180, 270], fontweight='normal', size=6)
-        plt.yticks([10, 20], fontweight='normal', size=6)
-        plt.xlabel("Heading", fontweight='normal', size=6)
+        ax.pcolormesh(
+            x, y, im.T, cmap=jet_cmap, edgecolors="face", vmax=vmax, shading="auto"
+        )
+        plt.xticks([90, 180, 270], fontweight="normal", size=6)
+        plt.yticks([10, 20], fontweight="normal", size=6)
+        plt.xlabel("Heading", fontweight="normal", size=6)
         return ax
 
     def makePowerSpectrum(
-            self, freqs: np.array, power: np.array, sm_power: np.array,
-            band_max_power: float, freq_at_band_max_power: float,
-            max_freq: int = 50, theta_range: tuple = [6, 12],
-            ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
+        self,
+        freqs: np.array,
+        power: np.array,
+        sm_power: np.array,
+        band_max_power: float,
+        freq_at_band_max_power: float,
+        max_freq: int = 50,
+        theta_range: tuple = [6, 12],
+        ax: matplotlib.axes = None,
+        **kwargs
+    ) -> matplotlib.axes:
         # downsample frequencies and power
         freqs = freqs[0::50]
         power = power[0::50]
         sm_power = sm_power[0::50]
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax.plot(freqs, power, alpha=0.5, color=[0.8627, 0.8627, 0.8627])
         ax.plot(freqs, sm_power)
         ax.set_xlim(0, max_freq)
         ylim = [0, band_max_power / 0.8]
-        if 'ylim' in kwargs:
-            ylim = kwargs['ylim']
+        if "ylim" in kwargs:
+            ylim = kwargs["ylim"]
         ax.set_ylim(ylim)
-        ax.set_ylabel('Power')
-        ax.set_xlabel('Frequency')
+        ax.set_ylabel("Power")
+        ax.set_xlabel("Frequency")
         ax.text(
-            x=theta_range[1] / 0.9, y=band_max_power,
-            s=str(freq_at_band_max_power)[0:4], fontsize=20)
+            x=theta_range[1] / 0.9,
+            y=band_max_power,
+            s=str(freq_at_band_max_power)[0:4],
+            fontsize=20,
+        )
         from matplotlib.patches import Rectangle
-        r = Rectangle((
-            theta_range[0], 0), width=np.diff(theta_range)[0],
-            height=np.diff(ax.get_ylim())[0], alpha=0.25, color='r', ec='none')
+
+        r = Rectangle(
+            (theta_range[0], 0),
+            width=np.diff(theta_range)[0],
+            height=np.diff(ax.get_ylim())[0],
+            alpha=0.25,
+            color="r",
+            ec="none",
+        )
         ax.add_patch(r)
         return ax
 
-    def makeXCorr(self, spk_times: np.array, ax: matplotlib.axes = None,
-                  **kwargs) -> matplotlib.axes:
+    def makeXCorr(
+        self, spk_times: np.array, ax: matplotlib.axes = None, **kwargs
+    ) -> matplotlib.axes:
         # spk_times in samples provided in seconds but convert to
         # ms for a more display friendly scale
-        spk_times = spk_times / 3e4 * 1000.
+        spk_times = spk_times / 3e4 * 1000.0
         S = SpikeCalcsGeneric(spk_times)
         y = S.xcorr(spk_times)
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax.hist(
-                y[y != 0], bins=201, range=[-500, 500],
-                color='k', histtype='stepfilled')
+            y[y != 0], bins=201, range=[-500, 500], color="k", histtype="stepfilled"
+        )
         ax.set_xlim(-500, 500)
         ax.set_xticks((-500, 0, 500))
-        ax.set_xticklabels('')
+        ax.set_xticklabels("")
         ax.tick_params(
-            axis='both', which='both', left=False, right=False,
-            bottom=False, top=False)
-        ax.set_yticklabels('')
-        ax.spines['right'].set_visible(False)
-        ax.spines['top'].set_visible(False)
-        ax.spines['left'].set_visible(False)
-        ax.xaxis.set_ticks_position('bottom')
+            axis="both", which="both", left=False, right=False, bottom=False, top=False
+        )
+        ax.set_yticklabels("")
+        ax.spines["right"].set_visible(False)
+        ax.spines["top"].set_visible(False)
+        ax.spines["left"].set_visible(False)
+        ax.xaxis.set_ticks_position("bottom")
         return ax
 
-    def makeRaster(self, spk_times: np.array, dt=(-50, 100),
-                   prc_max: float = 0.5, ax: matplotlib.axes = None,
-                   ms_per_bin: int = 1, histtype: str = 'count',
-                   **kwargs) -> matplotlib.axes:
+    def makeRaster(
+        self,
+        spk_times: np.array,
+        dt=(-50, 100),
+        prc_max: float = 0.5,
+        ax: matplotlib.axes = None,
+        ms_per_bin: int = 1,
+        histtype: str = "count",
+        **kwargs
+    ) -> matplotlib.axes:
         """
         Plots a raster plot for a specified tetrode/ cluster
 
         Parameters
         ----------
         spk_times: np.array
             The spike times in samples
@@ -346,93 +391,112 @@
         ms_per_bin : int
             The number of milliseconds in each bin of the raster plot
         histtype : str
             either 'count' or 'rate' - the resulting histogram plotted above
             the raster plot will consist of either the counts of spikes in
             ms_per_bin or the mean rate in ms_per_bin
         """
-        x1 = spk_times / 3e4 * 1000.  # get into ms
+        x1 = spk_times / 3e4 * 1000.0  # get into ms
         x1.sort()
-        on_good = getattr(self, 'ttl_timestamps')
+        on_good = getattr(self, "ttl_timestamps")
         dt = np.array(dt)
         irange = on_good[:, np.newaxis] + dt[np.newaxis, :]
         dts = np.searchsorted(x1, irange)
         y = []
         x = []
         for i, t in enumerate(dts):
-            tmp = x1[t[0]:t[1]] - on_good[i]
+            tmp = x1[t[0] : t[1]] - on_good[i]
             x.extend(tmp)
             y.extend(np.repeat(i, len(tmp)))
         if ax is None:
             fig = plt.figure(figsize=(4.0, 7.0))
             axScatter = fig.add_subplot(111)
         else:
             axScatter = ax
-        axScatter.scatter(x, y, marker='.', s=2, rasterized=False)
+        axScatter.scatter(x, y, marker=".", s=2, rasterized=False)
         divider = make_axes_locatable(axScatter)
         axScatter.set_xticks((dt[0], 0, dt[1]))
-        axScatter.set_xticklabels((str(dt[0]), '0', str(dt[1])))
-        axHistx = divider.append_axes("top", 0.95, pad=0.2, sharex=axScatter,
-                                      transform=axScatter.transAxes)
-        scattTrans = transforms.blended_transform_factory(axScatter.transData,
-                                                          axScatter.transAxes)
+        axScatter.set_xticklabels((str(dt[0]), "0", str(dt[1])))
+        axHistx = divider.append_axes(
+            "top", 0.95, pad=0.2, sharex=axScatter, transform=axScatter.transAxes
+        )
+        scattTrans = transforms.blended_transform_factory(
+            axScatter.transData, axScatter.transAxes
+        )
         stim_pwidth = getattr(self, "stim_duration", None)
         if stim_pwidth is None:
             raise ValueError("stim duration is None")
 
         axScatter.add_patch(
             Rectangle(
-                (0, 0), width=stim_pwidth, height=1,
+                (0, 0),
+                width=stim_pwidth,
+                height=1,
                 transform=scattTrans,
-                color=[0, 0, 1], alpha=0.5))
-        histTrans = transforms.blended_transform_factory(axHistx.transData,
-                                                         axHistx.transAxes)
-        axHistx.add_patch(Rectangle((0, 0), width=stim_pwidth, height=1,
-                          transform=histTrans,
-                          color=[0, 0, 1], alpha=0.5))
-        axScatter.set_ylabel('Laser stimulation events', labelpad=-18.5)
-        axScatter.set_xlabel('Time to stimulus onset(ms)')
+                color=[0, 0, 1],
+                alpha=0.5,
+            )
+        )
+        histTrans = transforms.blended_transform_factory(
+            axHistx.transData, axHistx.transAxes
+        )
+        axHistx.add_patch(
+            Rectangle(
+                (0, 0),
+                width=stim_pwidth,
+                height=1,
+                transform=histTrans,
+                color=[0, 0, 1],
+                alpha=0.5,
+            )
+        )
+        axScatter.set_ylabel("Laser stimulation events", labelpad=-18.5)
+        axScatter.set_xlabel("Time to stimulus onset(ms)")
         nStms = len(on_good)
         axScatter.set_ylim(0, nStms)
         # Label only the min and max of the y-axis
         ylabels = axScatter.get_yticklabels()
-        for i in range(1, len(ylabels)-1):
+        for i in range(1, len(ylabels) - 1):
             ylabels[i].set_visible(False)
         yticks = axScatter.get_yticklines()
-        for i in range(1, len(yticks)-1):
+        for i in range(1, len(yticks) - 1):
             yticks[i].set_visible(False)
 
-        histColor = [192/255.0, 192/255.0, 192/255.0]
+        histColor = [192 / 255.0, 192 / 255.0, 192 / 255.0]
         axHistx.hist(
-            x, bins=np.arange(dt[0], dt[1] + ms_per_bin, ms_per_bin),
-            color=histColor, alpha=0.6, range=dt, rasterized=True,
-            histtype='stepfilled')
-        if 'rate' in histtype:
-            axHistx.set_ylabel('Rate')
+            x,
+            bins=np.arange(dt[0], dt[1] + ms_per_bin, ms_per_bin),
+            color=histColor,
+            alpha=0.6,
+            range=dt,
+            rasterized=True,
+            histtype="stepfilled",
+        )
+        if "rate" in histtype:
+            axHistx.set_ylabel("Rate")
             # mn_rate_pre_stim = np.mean(vals[bins[1:] < 0])
             # idx = np.logical_and(bins[1:] > 0, bins[1:] < 10).nonzero()[0]
             # mn_rate_post_stim = np.mean(vals[idx])
             # above_half_idx = idx[(
             # vals[idx] < mn_rate_pre_stim * prc_max).nonzero()[0]]
             # half_pre_rate_ms = bins[above_half_idx[0]]
             # print('\ntime to {0}% of pre-stimulus rate = {1}ms'.format(*(
             # prc_max * 100, half_pre_rate_ms)))
             # print('mean pre-laser rate = {0}Hz'.format(mn_rate_pre_stim))
             # print('mean 10ms post-laser rate = {0}'.format(
             # mn_rate_post_stim))
         else:
-            axHistx.set_ylabel('Spike count', labelpad=-2.5)
-        plt.setp(axHistx.get_xticklabels(),
-                 visible=False)
+            axHistx.set_ylabel("Spike count", labelpad=-2.5)
+        plt.setp(axHistx.get_xticklabels(), visible=False)
         # Label only the min and max of the y-axis
         ylabels = axHistx.get_yticklabels()
-        for i in range(1, len(ylabels)-1):
+        for i in range(1, len(ylabels) - 1):
             ylabels[i].set_visible(False)
         yticks = axHistx.get_yticklines()
-        for i in range(1, len(yticks)-1):
+        for i in range(1, len(yticks) - 1):
             yticks[i].set_visible(False)
         axHistx.set_xlim(dt)
         axScatter.set_xlim(dt)
         return axScatter
 
     '''
     def getRasterHist(
@@ -476,16 +540,17 @@
         else:
             return np.histogram(
                 x, bins=np.arange(
                     dt[0], dt[1]+1, 1), range=dt)[0]
     '''
 
     @stripAxes
-    def show_SAC(self, A: np.array, inDict: dict,
-                 ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
+    def show_SAC(
+        self, A: np.array, inDict: dict, ax: matplotlib.axes = None, **kwargs
+    ) -> matplotlib.axes:
         """
         Displays the result of performing a spatial autocorrelation (SAC)
         on a grid cell.
 
         Uses the dictionary containing measures of the grid cell SAC to
         make a pretty picture
 
@@ -508,63 +573,68 @@
         ephysiopy.common.binning.RateMap.autoCorr2D()
         ephysiopy.common.ephys_generic.FieldCalcs.getMeaures()
         """
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         Am = A.copy()
-        Am[~inDict['dist_to_centre']] = np.nan
+        Am[~inDict["dist_to_centre"]] = np.nan
         Am = np.ma.masked_invalid(np.atleast_2d(Am))
-        x, y = np.meshgrid(
-            np.arange(0, np.shape(A)[1]),
-            np.arange(0, np.shape(A)[0]))
+        x, y = np.meshgrid(np.arange(0, np.shape(A)[1]), np.arange(0, np.shape(A)[0]))
         vmax = np.nanmax(np.ravel(A))
         ax.pcolormesh(
-            x, y, A, cmap=grey_cmap,
-            edgecolors='face', vmax=vmax, shading='auto')
+            x, y, A, cmap=grey_cmap, edgecolors="face", vmax=vmax, shading="auto"
+        )
         import copy
+
         cmap = copy.copy(jet_cmap)
-        cmap.set_bad('w', 0)
-        ax.pcolormesh(
-            x, y, Am, cmap=cmap,
-            edgecolors='face', vmax=vmax, shading='auto')
+        cmap.set_bad("w", 0)
+        ax.pcolormesh(x, y, Am, cmap=cmap, edgecolors="face", vmax=vmax, shading="auto")
         # horizontal green line at 3 o'clock
-        _y = (np.shape(A)[0]/2, np.shape(A)[0]/2)
-        _x = (np.shape(A)[1]/2, np.shape(A)[0])
-        ax.plot(_x, _y, c='g')
-        mag = inDict['scale'] * 0.5
-        th = np.linspace(0, inDict['orientation'], 50)
+        _y = (np.shape(A)[0] / 2, np.shape(A)[0] / 2)
+        _x = (np.shape(A)[1] / 2, np.shape(A)[0])
+        ax.plot(_x, _y, c="g")
+        mag = inDict["scale"] * 0.5
+        th = np.linspace(0, inDict["orientation"], 50)
         from ephysiopy.common.utils import rect
+
         [x, y] = rect(mag, th, deg=1)
         # angle subtended by orientation
         ax.plot(
-            x + (inDict['dist_to_centre'].shape[1] / 2),
-                (inDict['dist_to_centre'].shape[0] / 2) - y, 'r', **kwargs)
+            x + (inDict["dist_to_centre"].shape[1] / 2),
+            (inDict["dist_to_centre"].shape[0] / 2) - y,
+            "r",
+            **kwargs
+        )
         # plot lines from centre to peaks above middle
-        for p in inDict['closest_peak_coords']:
-            if p[0] <= inDict['dist_to_centre'].shape[0] / 2:
+        for p in inDict["closest_peak_coords"]:
+            if p[0] <= inDict["dist_to_centre"].shape[0] / 2:
                 ax.plot(
-                    (inDict['dist_to_centre'].shape[1]/2, p[1]),
-                    (inDict['dist_to_centre'].shape[0] / 2, p[0]), 'k',
-                    **kwargs)
+                    (inDict["dist_to_centre"].shape[1] / 2, p[1]),
+                    (inDict["dist_to_centre"].shape[0] / 2, p[0]),
+                    "k",
+                    **kwargs
+                )
         ax.invert_yaxis()
         all_ax = ax.axes
-        all_ax.set_aspect('equal')
-        all_ax.set_xlim((0.5, inDict['dist_to_centre'].shape[1]-1.5))
-        all_ax.set_ylim((inDict['dist_to_centre'].shape[0]-.5, -.5))
+        all_ax.set_aspect("equal")
+        all_ax.set_xlim((0.5, inDict["dist_to_centre"].shape[1] - 1.5))
+        all_ax.set_ylim((inDict["dist_to_centre"].shape[0] - 0.5, -0.5))
         return ax
 
-    def plotSpectrogramByDepth(self,
-                               nchannels: int = 384,
-                               nseconds: int = 100,
-                               maxFreq: int = 125,
-                               channels: list = [],
-                               frequencies: list = [],
-                               frequencyIncrement: int = 1,
-                               **kwargs):
+    def plotSpectrogramByDepth(
+        self,
+        nchannels: int = 384,
+        nseconds: int = 100,
+        maxFreq: int = 125,
+        channels: list = [],
+        frequencies: list = [],
+        frequencyIncrement: int = 1,
+        **kwargs
+    ):
         """
         Plots a heat map spectrogram of the LFP for each channel.
         Line plots of power per frequency band and power on a subset of
         channels are also displayed to the right and above the main plot.
         Parameters
         ----------
         nchannels : int
@@ -592,114 +662,114 @@
         -----
         Should also allow kwargs to specify exactly which channels
         and / or frequency bands to do the line plots for
         """
         if not self.path2LFPdata:
             raise TypeError("Not a probe recording so not plotting")
         import os
-        lfp_file = os.path.join(self.path2LFPdata, 'continuous.dat')
+
+        lfp_file = os.path.join(self.path2LFPdata, "continuous.dat")
         status = os.stat(lfp_file)
         nsamples = int(status.st_size / 2 / nchannels)
-        mmap = np.memmap(lfp_file,
-                         np.int16,
-                         'r',
-                         0,
-                         (nchannels, nsamples),
-                         order='F')
+        mmap = np.memmap(lfp_file, np.int16, "r", 0, (nchannels, nsamples), order="F")
         # Load the channel map NB assumes this is in the AP data
         # location and that kilosort was run there
         channel_map = np.squeeze(
-            np.load(os.path.join(self.path2APdata, 'channel_map.npy')))
+            np.load(os.path.join(self.path2APdata, "channel_map.npy"))
+        )
         lfp_sample_rate = 2500
-        data = np.array(mmap[channel_map, 0:nseconds*lfp_sample_rate])
+        data = np.array(mmap[channel_map, 0 : nseconds * lfp_sample_rate])
         from ephysiopy.common.ephys_generic import EEGCalcsGeneric
+
         E = EEGCalcsGeneric(data[0, :], lfp_sample_rate)
         E.calcEEGPowerSpectrum()
         spec_data = np.zeros(shape=(data.shape[0], len(E.sm_power[0::50])))
         for chan in range(data.shape[0]):
             E = EEGCalcsGeneric(data[chan, :], lfp_sample_rate)
             E.calcEEGPowerSpectrum()
             spec_data[chan, :] = E.sm_power[0::50]
 
         x, y = np.meshgrid(E.freqs[0::50], channel_map)
         import matplotlib.colors as colors
         from matplotlib.pyplot import cm
         from mpl_toolkits.axes_grid1 import make_axes_locatable
+
         _, spectoAx = plt.subplots()
-        spectoAx.pcolormesh(x,
-                            y,
-                            spec_data,
-                            edgecolors='face',
-                            cmap='bone',
-                            norm=colors.LogNorm())
+        spectoAx.pcolormesh(
+            x, y, spec_data, edgecolors="face", cmap="bone", norm=colors.LogNorm()
+        )
         spectoAx.set_xlim(0, maxFreq)
         spectoAx.set_ylim(channel_map[0], channel_map[-1])
-        spectoAx.set_xlabel('Frequency (Hz)')
-        spectoAx.set_ylabel('Channel')
+        spectoAx.set_xlabel("Frequency (Hz)")
+        spectoAx.set_ylabel("Channel")
         divider = make_axes_locatable(spectoAx)
-        channel_spectoAx = divider.append_axes("top",
-                                               1.2,
-                                               pad=0.1,
-                                               sharex=spectoAx)
-        meanfreq_powerAx = divider.append_axes("right",
-                                               1.2,
-                                               pad=0.1,
-                                               sharey=spectoAx)
-        plt.setp(channel_spectoAx.get_xticklabels() +
-                 meanfreq_powerAx.get_yticklabels(), visible=False)
+        channel_spectoAx = divider.append_axes("top", 1.2, pad=0.1, sharex=spectoAx)
+        meanfreq_powerAx = divider.append_axes("right", 1.2, pad=0.1, sharey=spectoAx)
+        plt.setp(
+            channel_spectoAx.get_xticklabels() + meanfreq_powerAx.get_yticklabels(),
+            visible=False,
+        )
 
         # plot mean power across some channels
         mn_power = np.mean(spec_data, 0)
         if not channels:
             channels = range(1, nchannels, 60)
         cols = iter(cm.rainbow(np.linspace(0, 1, len(channels))))
         for chan in channels:
             c = next(cols)
-            channel_spectoAx.plot(E.freqs[0::50],
-                                  10*np.log10(spec_data[chan, :]/mn_power),
-                                  c=c,
-                                  label=str(chan))
-
-        channel_spectoAx.set_ylabel('Channel power(dB)')
-        channel_spectoAx.legend(bbox_to_anchor=(0., 1.02, 1., .102),
-                                loc='lower left',
-                                mode='expand',
-                                fontsize='x-small',
-                                ncol=4)
+            channel_spectoAx.plot(
+                E.freqs[0::50],
+                10 * np.log10(spec_data[chan, :] / mn_power),
+                c=c,
+                label=str(chan),
+            )
+
+        channel_spectoAx.set_ylabel("Channel power(dB)")
+        channel_spectoAx.legend(
+            bbox_to_anchor=(0.0, 1.02, 1.0, 0.102),
+            loc="lower left",
+            mode="expand",
+            fontsize="x-small",
+            ncol=4,
+        )
 
         # plot mean frequencies across all channels
         if not frequencyIncrement:
             freq_inc = 6
         else:
             freq_inc = frequencyIncrement
         if not frequencies:
-            lower_freqs = np.arange(1, maxFreq-freq_inc, freq_inc)
+            lower_freqs = np.arange(1, maxFreq - freq_inc, freq_inc)
         else:
             lower_freqs = frequencies
         upper_freqs = [f + freq_inc for f in lower_freqs]
         cols = iter(cm.nipy_spectral(np.linspace(0, 1, len(upper_freqs))))
         mn_power = np.mean(spec_data, 1)
         for freqs in zip(lower_freqs, upper_freqs):
             freq_mask = np.logical_and(
-                E.freqs[0::50] > freqs[0], E.freqs[0::50] < freqs[1])
-            mean_power = 10*np.log10(
-                np.mean(spec_data[:, freq_mask], 1) / mn_power)
+                E.freqs[0::50] > freqs[0], E.freqs[0::50] < freqs[1]
+            )
+            mean_power = 10 * np.log10(np.mean(spec_data[:, freq_mask], 1) / mn_power)
             c = next(cols)
-            meanfreq_powerAx.plot(mean_power,
-                                  channel_map,
-                                  c=c,
-                                  label=str(freqs[0]) + " - " + str(freqs[1]))
-        meanfreq_powerAx.set_xlabel('Mean freq. band power(dB)')
-        meanfreq_powerAx.legend(bbox_to_anchor=(0., 1.02, 1., .102),
-                                loc='lower left',
-                                mode='expand',
-                                fontsize='x-small',
-                                ncol=1)
-        if 'saveas' in kwargs:
-            saveas = kwargs['saveas']
+            meanfreq_powerAx.plot(
+                mean_power,
+                channel_map,
+                c=c,
+                label=str(freqs[0]) + " - " + str(freqs[1]),
+            )
+        meanfreq_powerAx.set_xlabel("Mean freq. band power(dB)")
+        meanfreq_powerAx.legend(
+            bbox_to_anchor=(0.0, 1.02, 1.0, 0.102),
+            loc="lower left",
+            mode="expand",
+            fontsize="x-small",
+            ncol=1,
+        )
+        if "saveas" in kwargs:
+            saveas = kwargs["saveas"]
             plt.savefig(saveas)
         plt.show()
 
     '''
     def plotDirFilteredRmaps(self, tetrode, cluster, maptype='rmap', **kwargs):
         """
         Plots out directionally filtered ratemaps for the tetrode/ cluster
```

### Comparing `ephysiopy-1.9.24/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.25/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.24
+Version: 1.9.25
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.24/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.25/ephysiopy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ephysiopy/axona/__init__.py
 ephysiopy/axona/axonaIO.py
 ephysiopy/axona/file_headers.py
 ephysiopy/axona/tetrode_dict.py
 ephysiopy/axona/tintcolours.py
 ephysiopy/common/__init__.py
 ephysiopy/common/binning.py
+ephysiopy/common/cluster_old.py
 ephysiopy/common/ephys_generic.py
 ephysiopy/common/fieldcalcs.py
 ephysiopy/common/gridcell.py
 ephysiopy/common/mle_von_mises_vals.py
 ephysiopy/common/phasecoding.py
 ephysiopy/common/rhythmicity.py
 ephysiopy/common/spikecalcs.py
```

### Comparing `ephysiopy-1.9.24/setup.py` & `ephysiopy-1.9.25/setup.py`

 * *Files identical despite different names*

