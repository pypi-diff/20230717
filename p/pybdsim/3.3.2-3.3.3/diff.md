# Comparing `tmp/pybdsim-3.3.2.tar.gz` & `tmp/pybdsim-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdsim-3.3.2.tar", last modified: Thu Jun 29 15:37:39 2023, max compression
+gzip compressed data, was "pybdsim-3.3.3.tar", last modified: Mon Jul 17 13:57:52 2023, max compression
```

## Comparing `pybdsim-3.3.2.tar` & `pybdsim-3.3.3.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.277667 pybdsim-3.3.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.3.2/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.3.2/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.3.2/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.3.2/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-06-29 15:37:39.277772 pybdsim-3.3.2/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      936 2023-05-08 16:07:40.000000 pybdsim-3.3.2/README.md
--rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.3.2/bitbucket-pipelines.yml
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.258870 pybdsim-3.3.2/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)  1200819 2023-06-29 15:29:59.000000 pybdsim-3.3.2/docs/pybdsim.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.261270 pybdsim-3.3.2/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      307 2023-05-08 16:07:51.000000 pybdsim-3.3.2/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.3.2/docs/source/builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.3.2/docs/source/classes.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.3.2/docs/source/compare.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-06-29 15:36:52.000000 pybdsim-3.3.2/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.3.2/docs/source/convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.3.2/docs/source/data.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.3.2/docs/source/data_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.3.2/docs/source/developer.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12893 2023-05-11 15:00:20.000000 pybdsim-3.3.2/docs/source/fieldmaps.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.262375 pybdsim-3.3.2/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/rebdsimFileHistograms.png
--rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/rebdsimFileHistogramsWrapped.png
--rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/rebdsimFileMembers.png
--rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/simpleHistogramPlot.png
--rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.3.2/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2198 2023-05-08 16:05:46.000000 pybdsim-3.3.2/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.3.2/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.3.2/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.3.2/docs/source/plotting.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/support.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12803 2023-06-29 15:06:32.000000 pybdsim-3.3.2/docs/source/version_history.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.262586 pybdsim-3.3.2/examples/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.263111 pybdsim-3.3.2/examples/1_builder/
--rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/1_builder/1_builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/1_builder/1_testmachine.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/1_builder/1_testmachine.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.265472 pybdsim-3.3.2/examples/2_convert/
--rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/1_madxtfs2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/1_madxtfs2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/2_convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/2_transport2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/2_transport2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/transport_example.dat
--rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/transport_example.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.tar.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.265608 pybdsim-3.3.2/examples/3_optics/
--rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.3.2/examples/3_optics/optics_validation.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.265717 pybdsim-3.3.2/examples/4_uproot/
--rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.3.2/examples/4_uproot/4_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.3.2/examples/examples.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1846 2023-05-15 09:07:01.000000 pybdsim-3.3.2/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      258 2023-06-29 15:37:39.278075 pybdsim-3.3.2/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.3.2/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.256625 pybdsim-3.3.2/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.267899 pybdsim-3.3.2/src/pybdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.3.2/src/pybdsim/Beam.py
--rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.3.2/src/pybdsim/Builder.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.269635 pybdsim-3.3.2/src/pybdsim/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.3.2/src/pybdsim/Compare/_BdsimBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    10613 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_ElegantBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    14712 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23099 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_MadxBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Compare/_MadxMadxComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48466 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_MultipleCodeComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Compare/_SadComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6438 2023-05-08 16:03:57.000000 pybdsim-3.3.2/src/pybdsim/Compare/_TransportBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      827 2023-05-08 16:04:54.000000 pybdsim-3.3.2/src/pybdsim/Compare/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.3.2/src/pybdsim/Constants.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.271161 pybdsim-3.3.2/src/pybdsim/Convert/
--rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.3.2/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.3.2/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
--rw-r--r--   0 lnevay     (501) staff       (20)    24017 2023-06-29 15:27:24.000000 pybdsim-3.3.2/src/pybdsim/Convert/_CPyMad2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_ElegantParamToStrength.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Rebdsim2Numpy.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_SadFlat2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     4483 2023-05-08 16:02:45.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Transport2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-05-08 15:59:37.000000 pybdsim-3.3.2/src/pybdsim/Convert/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Convert/collimator_analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)    83880 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.3.2/src/pybdsim/DataUproot.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.271594 pybdsim-3.3.2/src/pybdsim/Field/
--rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Field/FieldPlotter.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Field/FieldPlotterVtk.py
--rw-r--r--   0 lnevay     (501) staff       (20)    17734 2023-06-29 15:07:38.000000 pybdsim-3.3.2/src/pybdsim/Field/_Field.py
--rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.3.2/src/pybdsim/Field/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Geant4.py
--rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.3.2/src/pybdsim/Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Joinhistograms.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.3.2/src/pybdsim/ModelProcessing.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.256898 pybdsim-3.3.2/src/pybdsim/Obsolete/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.272736 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
--rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Event.py
--rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Model.py
--rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Plots.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Processed.py
--rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Root.py
--rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Run.py
--rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.3.2/src/pybdsim/Optics.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.3.2/src/pybdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)    76876 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.3.2/src/pybdsim/Run.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.273072 pybdsim-3.3.2/src/pybdsim/Testing/
--rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Testing/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.3.2/src/pybdsim/Testing/bdsimMadx.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Testing/trackingTester.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.3.2/src/pybdsim/Visualisation.py
--rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.3.2/src/pybdsim/Writer.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.3.2/src/pybdsim/XSecBias.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1586 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.3.2/src/pybdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.268517 pybdsim-3.3.2/src/pybdsim.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.3.2/src/pybdsim.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)      335 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.273175 pybdsim-3.3.2/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.3.2/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.274071 pybdsim-3.3.2/tests/test_input/
--rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
--rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/model-model-aper.tfs.gz
--rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/model-model-collsettings.dat
--rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/model-model.tfs.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.274334 pybdsim-3.3.2/tests/test_output/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_output/.gitkeep
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.275157 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.275751 pybdsim-3.3.2/tests/test_output/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.257395 pybdsim-3.3.2/tests/test_output2/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.276328 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.276882 pybdsim-3.3.2/tests/test_output2/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.277442 pybdsim-3.3.2/tests/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.3.2/tests/tests/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/tests/pybdsim_test_utils.py
--rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/tests/test_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.3.2/tests/tests/testratio.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.3.2/tests/tests/write_test_outputs.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.277562 pybdsim-3.3.2/tests/unit/
--rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/unit/test_Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.394880 pybdsim-3.3.3/
+-rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.3.3/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.3.3/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.3.3/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.3.3/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-07-17 13:57:52.394993 pybdsim-3.3.3/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      936 2023-05-08 16:07:40.000000 pybdsim-3.3.3/README.md
+-rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.3.3/bitbucket-pipelines.yml
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.355739 pybdsim-3.3.3/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)  1200819 2023-06-29 15:29:59.000000 pybdsim-3.3.3/docs/pybdsim.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.361813 pybdsim-3.3.3/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      307 2023-05-08 16:07:51.000000 pybdsim-3.3.3/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.3.3/docs/source/builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.3.3/docs/source/classes.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.3.3/docs/source/compare.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-06-29 15:36:52.000000 pybdsim-3.3.3/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.3.3/docs/source/convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.3.3/docs/source/data.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.3.3/docs/source/data_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.3.3/docs/source/developer.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12893 2023-05-11 15:00:20.000000 pybdsim-3.3.3/docs/source/fieldmaps.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.364617 pybdsim-3.3.3/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/source/figures/rebdsimFileHistograms.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/source/figures/rebdsimFileHistogramsWrapped.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/source/figures/rebdsimFileMembers.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/source/figures/simpleHistogramPlot.png
+-rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.3.3/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2198 2023-05-08 16:05:46.000000 pybdsim-3.3.3/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.3.3/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.3.3/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.3.3/docs/source/plotting.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.3.3/docs/source/support.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12923 2023-07-17 13:56:59.000000 pybdsim-3.3.3/docs/source/version_history.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.365079 pybdsim-3.3.3/examples/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.366320 pybdsim-3.3.3/examples/1_builder/
+-rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/1_builder/1_builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/1_builder/1_testmachine.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/1_builder/1_testmachine.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.369116 pybdsim-3.3.3/examples/2_convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/1_madxtfs2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/1_madxtfs2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/2_convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/2_transport2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/2_transport2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/transport_example.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/transport_example.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/twiss35tevb1_short.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.3.3/examples/2_convert/twiss35tevb1_short.tar.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.369294 pybdsim-3.3.3/examples/3_optics/
+-rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.3.3/examples/3_optics/optics_validation.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.369525 pybdsim-3.3.3/examples/4_uproot/
+-rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.3.3/examples/4_uproot/4_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.3.3/examples/examples.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1846 2023-05-15 09:07:01.000000 pybdsim-3.3.3/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      258 2023-07-17 13:57:52.395289 pybdsim-3.3.3/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.3.3/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.351302 pybdsim-3.3.3/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.375054 pybdsim-3.3.3/src/pybdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.3.3/src/pybdsim/Beam.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.3.3/src/pybdsim/Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.381300 pybdsim-3.3.3/src/pybdsim/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.3.3/src/pybdsim/Compare/_BdsimBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    10609 2023-07-17 13:55:48.000000 pybdsim-3.3.3/src/pybdsim/Compare/_ElegantBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    14708 2023-07-17 13:55:48.000000 pybdsim-3.3.3/src/pybdsim/Compare/_Mad8BdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    23095 2023-07-17 13:55:48.000000 pybdsim-3.3.3/src/pybdsim/Compare/_MadxBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Compare/_MadxMadxComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48466 2023-06-29 15:06:32.000000 pybdsim-3.3.3/src/pybdsim/Compare/_MultipleCodeComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Compare/_SadComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6438 2023-05-08 16:03:57.000000 pybdsim-3.3.3/src/pybdsim/Compare/_TransportBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      827 2023-05-08 16:04:54.000000 pybdsim-3.3.3/src/pybdsim/Compare/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.3.3/src/pybdsim/Constants.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.384660 pybdsim-3.3.3/src/pybdsim/Convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.3.3/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.3.3/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    24017 2023-06-29 15:27:24.000000 pybdsim-3.3.3/src/pybdsim/Convert/_CPyMad2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Convert/_ElegantParamToStrength.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Convert/_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Convert/_Rebdsim2Numpy.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Convert/_SadFlat2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     4483 2023-05-08 16:02:45.000000 pybdsim-3.3.3/src/pybdsim/Convert/_Transport2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-05-08 15:59:37.000000 pybdsim-3.3.3/src/pybdsim/Convert/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Convert/collimator_analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    83880 2023-06-29 15:06:32.000000 pybdsim-3.3.3/src/pybdsim/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.3.3/src/pybdsim/DataUproot.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.385675 pybdsim-3.3.3/src/pybdsim/Field/
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-06-29 15:06:32.000000 pybdsim-3.3.3/src/pybdsim/Field/FieldPlotter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Field/FieldPlotterVtk.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    17734 2023-06-29 15:07:38.000000 pybdsim-3.3.3/src/pybdsim/Field/_Field.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.3.3/src/pybdsim/Field/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.3.3/src/pybdsim/Geant4.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.3.3/src/pybdsim/Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Joinhistograms.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.3.3/src/pybdsim/ModelProcessing.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.351704 pybdsim-3.3.3/src/pybdsim/Obsolete/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.387785 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Event.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Model.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Plots.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Processed.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Root.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Run.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.3.3/src/pybdsim/Optics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.3.3/src/pybdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    76876 2023-06-29 15:06:32.000000 pybdsim-3.3.3/src/pybdsim/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.3.3/src/pybdsim/Run.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.388534 pybdsim-3.3.3/src/pybdsim/Testing/
+-rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Testing/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.3.3/src/pybdsim/Testing/bdsimMadx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.3.3/src/pybdsim/Testing/trackingTester.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.3.3/src/pybdsim/Visualisation.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.3.3/src/pybdsim/Writer.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.3.3/src/pybdsim/XSecBias.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1586 2023-06-29 15:06:32.000000 pybdsim-3.3.3/src/pybdsim/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.3.3/src/pybdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-07-17 13:57:52.000000 pybdsim-3.3.3/src/pybdsim/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.375827 pybdsim-3.3.3/src/pybdsim.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-07-17 13:57:52.000000 pybdsim-3.3.3/src/pybdsim.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-07-17 13:57:52.000000 pybdsim-3.3.3/src/pybdsim.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-07-17 13:57:52.000000 pybdsim-3.3.3/src/pybdsim.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.3.3/src/pybdsim.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      335 2023-07-17 13:57:52.000000 pybdsim-3.3.3/src/pybdsim.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-07-17 13:57:52.000000 pybdsim-3.3.3/src/pybdsim.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.388760 pybdsim-3.3.3/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.3.3/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.390257 pybdsim-3.3.3/tests/test_input/
+-rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.3.3/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.3.3/tests/test_input/model-model-aper.tfs.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.3.3/tests/test_input/model-model-collsettings.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.3.3/tests/test_input/model-model.tfs.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.390636 pybdsim-3.3.3/tests/test_output/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.3.3/tests/test_output/.gitkeep
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.391494 pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.392353 pybdsim-3.3.3/tests/test_output/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.352387 pybdsim-3.3.3/tests/test_output2/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.393121 pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.393879 pybdsim-3.3.3/tests/test_output2/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/test_output2/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.394622 pybdsim-3.3.3/tests/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.3.3/tests/tests/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/tests/pybdsim_test_utils.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.3.3/tests/tests/test_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.3.3/tests/tests/testratio.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.3.3/tests/tests/write_test_outputs.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-07-17 13:57:52.394755 pybdsim-3.3.3/tests/unit/
+-rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.3.3/tests/unit/test_Builder.py
```

### Comparing `pybdsim-3.3.2/COPYING.txt` & `pybdsim-3.3.3/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/LICENSE.txt` & `pybdsim-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/Makefile` & `pybdsim-3.3.3/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/PKG-INFO` & `pybdsim-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.3.2
+Version: 3.3.3
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.3.2/README.md` & `pybdsim-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/bitbucket-pipelines.yml` & `pybdsim-3.3.3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/Makefile` & `pybdsim-3.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/make.bat` & `pybdsim-3.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/pybdsim.pdf` & `pybdsim-3.3.3/docs/pybdsim.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/builder.rst` & `pybdsim-3.3.3/docs/source/builder.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/classes.rst` & `pybdsim-3.3.3/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/compare.rst` & `pybdsim-3.3.3/docs/source/compare.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/conf.py` & `pybdsim-3.3.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/convert.rst` & `pybdsim-3.3.3/docs/source/convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/data.rst` & `pybdsim-3.3.3/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/data_uproot.rst` & `pybdsim-3.3.3/docs/source/data_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/developer.rst` & `pybdsim-3.3.3/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/fieldmaps.rst` & `pybdsim-3.3.3/docs/source/fieldmaps.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/figures/rebdsimFileHistograms.png` & `pybdsim-3.3.3/docs/source/figures/rebdsimFileHistograms.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/figures/rebdsimFileHistogramsWrapped.png` & `pybdsim-3.3.3/docs/source/figures/rebdsimFileHistogramsWrapped.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/figures/rebdsimFileMembers.png` & `pybdsim-3.3.3/docs/source/figures/rebdsimFileMembers.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/figures/simpleHistogramPlot.png` & `pybdsim-3.3.3/docs/source/figures/simpleHistogramPlot.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/installation.rst` & `pybdsim-3.3.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/licence.rst` & `pybdsim-3.3.3/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/moduledocs.rst` & `pybdsim-3.3.3/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/plotting.rst` & `pybdsim-3.3.3/docs/source/plotting.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/support.rst` & `pybdsim-3.3.3/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/docs/source/version_history.rst` & `pybdsim-3.3.3/docs/source/version_history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ===============
 Version History
 ===============
 
+V3.3.3 - 2023 / 07 / 17
+=======================
+
+* Fix for missing functions due to recent refactor in `Data.General`.
+
 V3.3.2 - 2023 / 06 / 29
 =======================
 
 * Fix loading of new header variables with backwards compatibility.
 * Fix extra new lines and white space being written out in comments at the top
   of field maps.
 * New function to write a 3D scoring mesh out as ASCII for transfer to
```

### Comparing `pybdsim-3.3.2/examples/1_builder/1_testmachine.png` & `pybdsim-3.3.3/examples/1_builder/1_testmachine.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/1_madxtfs2gmad.png` & `pybdsim-3.3.3/examples/2_convert/1_madxtfs2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/2_convert.rst` & `pybdsim-3.3.3/examples/2_convert/2_convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/2_transport2gmad.png` & `pybdsim-3.3.3/examples/2_convert/2_transport2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/transport_example.dat` & `pybdsim-3.3.3/examples/2_convert/transport_example.dat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/transport_example.pdf` & `pybdsim-3.3.3/examples/2_convert/transport_example.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.pdf` & `pybdsim-3.3.3/examples/2_convert/twiss35tevb1_short.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.tar.gz` & `pybdsim-3.3.3/examples/2_convert/twiss35tevb1_short.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/3_optics/optics_validation.py` & `pybdsim-3.3.3/examples/3_optics/optics_validation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/examples/4_uproot/4_uproot.rst` & `pybdsim-3.3.3/examples/4_uproot/4_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/pyproject.toml` & `pybdsim-3.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Beam.py` & `pybdsim-3.3.3/src/pybdsim/Beam.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Builder.py` & `pybdsim-3.3.3/src/pybdsim/Builder.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_BdsimBdsimComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_BdsimBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_ElegantBdsimComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_ElegantBdsimComparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     | figsize         | Figure size for all figures - default is (12,5)         |
     +-----------------+---------------------------------------------------------+
     
     """
 
     _CheckFileExistsList(elegantTwiss, elegantSigma, elegantCentroid, bdsim)
 
-    fname = _pybdsim._General.GetFileName(bdsim) # cache file name
+    fname = _pybdsim.Data.GetFileName(bdsim) # cache file name
     if fname == "":
         fname = "optics_report"
 
     bdsData = _pybdsim.Data.Load(bdsim)
 
     bdsinst = _pybdsim.Data.CheckItsBDSAsciiData(bdsData, True)
     bdsopt  = _GetBDSIMOptics(bdsinst)
```

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_Mad8BdsimComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     """
 
     if not _isfile(twiss):
         raise IOError("File not found: ", twiss)
     if isinstance(bdsim, str) and not _isfile(bdsim):
         raise IOError("File not found: ", bdsim)
 
-    fname = _pybdsim._General.GetFileName(bdsim)  # cache file name
+    fname = _pybdsim.Data.GetFileName(bdsim)  # cache file name
     if fname == "":
         fname = "optics_report"
 
     # load mad8 optics and bdsim optics
     mad8opt = _m8.Output(twiss)
     bdsinst = _pybdsim.Data.CheckItsBDSAsciiData(bdsim)
     bdsopt = _GetBDSIMOptics(bdsinst)
```

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_MadxBdsimComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_MadxBdsimComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     | figsize         | Figure size for all figures - default is (12,5)         |
     +-----------------+---------------------------------------------------------+
     
     """
 
     _CheckFilesExist(tfs, bdsim, survey)
 
-    fname = _pybdsim._General.GetFileName(bdsim) # cache file name
+    fname = _pybdsim.Data.GetFileName(bdsim) # cache file name
     if fname == "":
         fname = "optics_report"
 
     tfsinst = _pymadx.Data.CheckItsTfs(tfs)
     bdsinst = _pybdsim.Data.CheckItsBDSAsciiData(bdsim, True)
 
     tfsheader = tfsinst.header
```

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_MultipleCodeComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_MultipleCodeComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_SadComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_SadComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/_TransportBdsimComparison.py` & `pybdsim-3.3.3/src/pybdsim/Compare/_TransportBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Compare/__init__.py` & `pybdsim-3.3.3/src/pybdsim/Compare/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Constants.py` & `pybdsim-3.3.3/src/pybdsim/Constants.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_CPyMad2Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_CPyMad2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_ElegantParamToStrength.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_ElegantParamToStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Saveline2Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_Mad8Saveline2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_Mad8Twiss2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2GmadStrength.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_MadxTfs2GmadStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_Rebdsim2Numpy.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_Rebdsim2Numpy.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_SadFlat2Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_SadFlat2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/_Transport2Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Convert/_Transport2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/__init__.py` & `pybdsim-3.3.3/src/pybdsim/Convert/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Convert/collimator_analysis.py` & `pybdsim-3.3.3/src/pybdsim/Convert/collimator_analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Data.py` & `pybdsim-3.3.3/src/pybdsim/Data.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/DataUproot.py` & `pybdsim-3.3.3/src/pybdsim/DataUproot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Field/FieldPlotter.py` & `pybdsim-3.3.3/src/pybdsim/Field/FieldPlotter.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Field/FieldPlotterVtk.py` & `pybdsim-3.3.3/src/pybdsim/Field/FieldPlotterVtk.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Field/_Field.py` & `pybdsim-3.3.3/src/pybdsim/Field/_Field.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Field/__init__.py` & `pybdsim-3.3.3/src/pybdsim/Field/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Geant4.py` & `pybdsim-3.3.3/src/pybdsim/Geant4.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Gmad.py` & `pybdsim-3.3.3/src/pybdsim/Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Joinhistograms.py` & `pybdsim-3.3.3/src/pybdsim/Joinhistograms.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/ModelProcessing.py` & `pybdsim-3.3.3/src/pybdsim/ModelProcessing.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Analysis.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Event.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Event.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Processed.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Processed.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Root.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/Root.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/__init__.py` & `pybdsim-3.3.3/src/pybdsim/Obsolete/Rebdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Optics.py` & `pybdsim-3.3.3/src/pybdsim/Optics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Options.py` & `pybdsim-3.3.3/src/pybdsim/Options.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Plot.py` & `pybdsim-3.3.3/src/pybdsim/Plot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Run.py` & `pybdsim-3.3.3/src/pybdsim/Run.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Testing/bdsimMadx.py` & `pybdsim-3.3.3/src/pybdsim/Testing/bdsimMadx.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Testing/trackingTester.py` & `pybdsim-3.3.3/src/pybdsim/Testing/trackingTester.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Visualisation.py` & `pybdsim-3.3.3/src/pybdsim/Visualisation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/Writer.py` & `pybdsim-3.3.3/src/pybdsim/Writer.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/XSecBias.py` & `pybdsim-3.3.3/src/pybdsim/XSecBias.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/_General.py` & `pybdsim-3.3.3/src/pybdsim/_General.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim/__init__.py` & `pybdsim-3.3.3/src/pybdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/src/pybdsim.egg-info/PKG-INFO` & `pybdsim-3.3.3/src/pybdsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.3.2
+Version: 3.3.3
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.3.2/src/pybdsim.egg-info/SOURCES.txt` & `pybdsim-3.3.3/src/pybdsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz` & `pybdsim-3.3.3/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_input/model-model-aper.tfs.gz` & `pybdsim-3.3.3/tests/test_input/model-model-aper.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_input/model-model.tfs.gz` & `pybdsim-3.3.3/tests/test_input/model-model.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.3.3/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output/model-model/model_components.gmad` & `pybdsim-3.3.3/tests/test_output/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output/model-model/model_sequence.gmad` & `pybdsim-3.3.3/tests/test_output/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.3.3/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output2/model-model/model_components.gmad` & `pybdsim-3.3.3/tests/test_output2/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/test_output2/model-model/model_sequence.gmad` & `pybdsim-3.3.3/tests/test_output2/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/tests/pybdsim_test_utils.py` & `pybdsim-3.3.3/tests/tests/pybdsim_test_utils.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/tests/test_MadxTfs2Gmad.py` & `pybdsim-3.3.3/tests/tests/test_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/tests/testratio.py` & `pybdsim-3.3.3/tests/tests/testratio.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/tests/write_test_outputs.py` & `pybdsim-3.3.3/tests/tests/write_test_outputs.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.2/tests/unit/test_Builder.py` & `pybdsim-3.3.3/tests/unit/test_Builder.py`

 * *Files identical despite different names*

