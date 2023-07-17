# Comparing `tmp/PyQtGuiLib-PySide-1.0.tar.gz` & `tmp/PyQtGuiLib-PySide-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtGuiLib-PySide-1.0.tar", last modified: Mon Jul 17 04:08:35 2023, max compression
+gzip compressed data, was "PyQtGuiLib-PySide-1.1.tar", last modified: Mon Jul 17 04:58:21 2023, max compression
```

## Comparing `PyQtGuiLib-PySide-1.0.tar` & `PyQtGuiLib-PySide-1.1.tar`

### file list

```diff
@@ -1,76 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.811868 PyQtGuiLib-PySide-1.0/
--rw-rw-rw-   0        0        0     7815 2023-07-17 03:38:31.000000 PyQtGuiLib-PySide-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      790 2023-07-17 04:08:35.810870 PyQtGuiLib-PySide-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.747437 PyQtGuiLib-PySide-1.0/PyQtGuiLib/
--rw-rw-rw-   0        0        0        0 2023-07-17 01:41:56.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.750428 PyQtGuiLib-PySide-1.0/PyQtGuiLib/animation/
--rw-rw-rw-   0        0        0     6797 2023-05-08 00:28:14.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/animation/PropertyAnimation.py
--rw-rw-rw-   0        0        0      124 2023-07-17 01:45:28.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/animation/__init__.py
--rw-rw-rw-   0        0        0     7157 2023-07-17 02:01:21.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/animation/animation.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.751426 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/
--rw-rw-rw-   0        0        0        0 2023-07-17 02:04:14.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.754020 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/layout/
--rw-rw-rw-   0        0        0       56 2023-07-17 02:07:35.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/layout/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-07-17 02:08:04.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/layout/flowLayout.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.757014 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/progressBar/
--rw-rw-rw-   0        0        0       63 2023-07-17 02:12:13.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/progressBar/__init__.py
--rw-rw-rw-   0        0        0     3833 2023-07-17 02:14:16.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/progressBar/gradientBar.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.759009 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/switchButtons/
--rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/switchButtons/__init__.py
--rw-rw-rw-   0        0        0     4988 2023-07-17 02:05:45.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/switchButtons/swButton.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.763996 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.783942 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/__init__.py
--rw-rw-rw-   0        0        0     7313 2023-07-17 02:59:39.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qt.py
--rw-rw-rw-   0        0        0      198 2023-07-17 03:15:39.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtBluetooth.py
--rw-rw-rw-   0        0        0      192 2023-07-17 03:11:57.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtCharts.py
--rw-rw-rw-   0        0        0      200 2023-07-17 03:11:57.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtConcurrent.py
--rw-rw-rw-   0        0        0      304 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtCore.py
--rw-rw-rw-   0        0        0      214 2023-07-17 03:12:48.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtDataVisualization.py
--rw-rw-rw-   0        0        0      316 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtGui.py
--rw-rw-rw-   0        0        0      188 2023-07-17 03:13:24.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtHelp.py
--rw-rw-rw-   0        0        0      200 2023-07-17 03:13:54.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtMultimedia.py
--rw-rw-rw-   0        0        0      214 2023-07-17 03:07:26.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtMultimediaWidgets.py
--rw-rw-rw-   0        0        0      194 2023-07-17 03:14:21.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtNetwork.py
--rw-rw-rw-   0        0        0      202 2023-07-17 03:14:55.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtNetworkAuth.py
--rw-rw-rw-   0        0        0      274 2023-07-17 03:08:44.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtSip.py
--rw-rw-rw-   0        0        0      186 2023-07-17 03:10:27.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtSvg.py
--rw-rw-rw-   0        0        0      290 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtUic.py
--rw-rw-rw-   0        0        0      263 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qtWidgets.py
--rw-rw-rw-   0        0        0      813 2023-07-17 03:41:58.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/__init__.py
--rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/error.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.785937 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/py/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/py/__init__.py
--rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/py/common.py
--rw-rw-rw-   0        0        0     2758 2023-07-17 01:38:38.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/utility.py
--rw-rw-rw-   0        0        0      375 2023-07-17 01:33:20.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/versions.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.788929 PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/
--rw-rw-rw-   0        0        0      130 2023-07-17 01:44:41.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/__init__.py
--rw-rw-rw-   0        0        0     8588 2023-07-17 02:02:43.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/styleAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.790924 PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/superPainter/
--rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/superPainter/__init__.py
--rw-rw-rw-   0        0        0    15654 2023-07-17 03:29:46.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/superPainter/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.795910 PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/
--rw-rw-rw-   0        0        0      790 2023-07-17 04:08:35.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1862 2023-07-17 04:08:35.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 04:08:35.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 04:08:35.000000 PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-07-17 03:45:29.000000 PyQtGuiLib-PySide-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 04:08:35.811868 PyQtGuiLib-PySide-1.0/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-07-17 04:08:24.000000 PyQtGuiLib-PySide-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.799900 PyQtGuiLib-PySide-1.0/test/
--rw-rw-rw-   0        0        0      106 2023-07-17 01:33:20.000000 PyQtGuiLib-PySide-1.0/test/__init__.py
--rw-rw-rw-   0        0        0      527 2023-07-17 01:38:52.000000 PyQtGuiLib-PySide-1.0/test/test1.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.804887 PyQtGuiLib-PySide-1.0/test/test_Animation/
--rw-rw-rw-   0        0        0     1990 2023-06-14 07:54:17.000000 PyQtGuiLib-PySide-1.0/test/test_Animation/1.py
--rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-PySide-1.0/test/test_Animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.807878 PyQtGuiLib-PySide-1.0/test/test_Animation/test_ani/
--rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-PySide-1.0/test/test_Animation/test_ani/1.py
--rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-PySide-1.0/test/test_Animation/test_ani/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-07-17 03:43:13.000000 PyQtGuiLib-PySide-1.0/test/test_Animation/test_animation.py
--rw-rw-rw-   0        0        0     1728 2023-06-25 10:32:05.000000 PyQtGuiLib-PySide-1.0/test/test_Animation/test_p_ani.py
--rw-rw-rw-   0        0        0     1779 2023-07-17 02:12:13.000000 PyQtGuiLib-PySide-1.0/test/test_gradientBar.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:08:35.809873 PyQtGuiLib-PySide-1.0/test/test_styleAnalysis/
--rw-rw-rw-   0        0        0      106 2023-07-17 01:42:51.000000 PyQtGuiLib-PySide-1.0/test/test_styleAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2364 2023-07-17 02:59:39.000000 PyQtGuiLib-PySide-1.0/test/test_styleAnalysis/test1.py
--rw-rw-rw-   0        0        0     1054 2023-07-17 02:08:36.000000 PyQtGuiLib-PySide-1.0/test/test_switchButton.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.200841 PyQtGuiLib-PySide-1.1/
+-rw-rw-rw-   0        0        0     7815 2023-07-17 03:38:31.000000 PyQtGuiLib-PySide-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      790 2023-07-17 04:58:21.199844 PyQtGuiLib-PySide-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.103101 PyQtGuiLib-PySide-1.1/PyQtGuiLib/
+-rw-rw-rw-   0        0        0        0 2023-07-17 01:41:56.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.107091 PyQtGuiLib-PySide-1.1/PyQtGuiLib/animation/
+-rw-rw-rw-   0        0        0     6797 2023-05-08 00:28:14.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/animation/PropertyAnimation.py
+-rw-rw-rw-   0        0        0      124 2023-07-17 01:45:28.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/animation/__init__.py
+-rw-rw-rw-   0        0        0     7157 2023-07-17 02:01:21.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/animation/animation.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.111081 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/
+-rw-rw-rw-   0        0        0      126 2023-07-17 04:54:16.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.115070 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/layout/
+-rw-rw-rw-   0        0        0       56 2023-07-17 02:07:35.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/layout/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-07-17 02:08:04.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/layout/flowLayout.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.123048 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/
+-rw-rw-rw-   0        0        0        0 2023-05-27 07:16:04.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/__init__.py
+-rw-rw-rw-   0        0        0    10022 2023-05-11 04:23:31.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/colorHsv.py
+-rw-rw-rw-   0        0        0     6492 2023-05-09 09:37:23.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/paletteFrame.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.130029 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/paletteTools/
+-rw-rw-rw-   0        0        0      107 2023-05-27 07:33:06.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/paletteTools/__init__.py
+-rw-rw-rw-   0        0        0    40079 2023-07-17 04:56:14.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/paletteTools/area.py
+-rw-rw-rw-   0        0        0    16131 2023-05-31 09:28:26.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/paletteTools/paletteToolUI.py
+-rw-rw-rw-   0        0        0     4959 2023-05-31 09:45:57.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/paletteTools/palettetools.py
+-rw-rw-rw-   0        0        0    63735 2023-07-04 02:05:16.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/palettes/palettetools.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.134019 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/progressBar/
+-rw-rw-rw-   0        0        0       63 2023-07-17 02:12:13.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/progressBar/__init__.py
+-rw-rw-rw-   0        0        0     3833 2023-07-17 02:14:16.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/progressBar/gradientBar.py
+-rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/slideShow.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.136012 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/switchButtons/
+-rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/switchButtons/__init__.py
+-rw-rw-rw-   0        0        0     4988 2023-07-17 02:05:45.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/switchButtons/swButton.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.141000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.168926 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/__init__.py
+-rw-rw-rw-   0        0        0     7313 2023-07-17 02:59:39.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qt.py
+-rw-rw-rw-   0        0        0      198 2023-07-17 03:15:39.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtBluetooth.py
+-rw-rw-rw-   0        0        0      192 2023-07-17 03:11:57.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtCharts.py
+-rw-rw-rw-   0        0        0      200 2023-07-17 03:11:57.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtConcurrent.py
+-rw-rw-rw-   0        0        0      304 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtCore.py
+-rw-rw-rw-   0        0        0      214 2023-07-17 03:12:48.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtDataVisualization.py
+-rw-rw-rw-   0        0        0      316 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtGui.py
+-rw-rw-rw-   0        0        0      188 2023-07-17 03:13:24.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtHelp.py
+-rw-rw-rw-   0        0        0      200 2023-07-17 03:13:54.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtMultimedia.py
+-rw-rw-rw-   0        0        0      214 2023-07-17 03:07:26.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtMultimediaWidgets.py
+-rw-rw-rw-   0        0        0      194 2023-07-17 03:14:21.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtNetwork.py
+-rw-rw-rw-   0        0        0      202 2023-07-17 03:14:55.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtNetworkAuth.py
+-rw-rw-rw-   0        0        0      274 2023-07-17 03:08:44.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtSip.py
+-rw-rw-rw-   0        0        0      186 2023-07-17 03:10:27.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtSvg.py
+-rw-rw-rw-   0        0        0      290 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtUic.py
+-rw-rw-rw-   0        0        0      263 2023-07-17 02:19:24.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qtWidgets.py
+-rw-rw-rw-   0        0        0      813 2023-07-17 03:41:58.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/error.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.170920 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/py/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/py/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/py/common.py
+-rw-rw-rw-   0        0        0     2758 2023-07-17 01:38:38.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/utility.py
+-rw-rw-rw-   0        0        0      375 2023-07-17 01:33:20.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/versions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.172915 PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/
+-rw-rw-rw-   0        0        0      130 2023-07-17 01:44:41.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/__init__.py
+-rw-rw-rw-   0        0        0     8588 2023-07-17 02:02:43.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/styleAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.175906 PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/superPainter/
+-rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/superPainter/__init__.py
+-rw-rw-rw-   0        0        0    15654 2023-07-17 03:29:46.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/superPainter/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.181892 PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/
+-rw-rw-rw-   0        0        0      790 2023-07-17 04:58:21.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2278 2023-07-17 04:58:21.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 04:58:21.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 04:58:21.000000 PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-17 03:45:29.000000 PyQtGuiLib-PySide-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 04:58:21.200841 PyQtGuiLib-PySide-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-07-17 04:58:08.000000 PyQtGuiLib-PySide-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.188872 PyQtGuiLib-PySide-1.1/test/
+-rw-rw-rw-   0        0        0      106 2023-07-17 01:33:20.000000 PyQtGuiLib-PySide-1.1/test/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-07-17 01:38:52.000000 PyQtGuiLib-PySide-1.1/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.192861 PyQtGuiLib-PySide-1.1/test/test_Animation/
+-rw-rw-rw-   0        0        0     1990 2023-06-14 07:54:17.000000 PyQtGuiLib-PySide-1.1/test/test_Animation/1.py
+-rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-PySide-1.1/test/test_Animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.195854 PyQtGuiLib-PySide-1.1/test/test_Animation/test_ani/
+-rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-PySide-1.1/test/test_Animation/test_ani/1.py
+-rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-PySide-1.1/test/test_Animation/test_ani/__init__.py
+-rw-rw-rw-   0        0        0     1388 2023-07-17 03:43:13.000000 PyQtGuiLib-PySide-1.1/test/test_Animation/test_animation.py
+-rw-rw-rw-   0        0        0     1728 2023-06-25 10:32:05.000000 PyQtGuiLib-PySide-1.1/test/test_Animation/test_p_ani.py
+-rw-rw-rw-   0        0        0     1898 2023-05-31 09:45:31.000000 PyQtGuiLib-PySide-1.1/test/test_PaletteTools.py
+-rw-rw-rw-   0        0        0     1779 2023-07-17 02:12:13.000000 PyQtGuiLib-PySide-1.1/test/test_gradientBar.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:58:21.198845 PyQtGuiLib-PySide-1.1/test/test_styleAnalysis/
+-rw-rw-rw-   0        0        0      106 2023-07-17 01:42:51.000000 PyQtGuiLib-PySide-1.1/test/test_styleAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2364 2023-07-17 02:59:39.000000 PyQtGuiLib-PySide-1.1/test/test_styleAnalysis/test1.py
+-rw-rw-rw-   0        0        0     1054 2023-07-17 02:08:36.000000 PyQtGuiLib-PySide-1.1/test/test_switchButton.py
```

### Comparing `PyQtGuiLib-PySide-1.0/LICENSE.txt` & `PyQtGuiLib-PySide-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PKG-INFO` & `PyQtGuiLib-PySide-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib-PySide
-Version: 1.0
+Version: 1.1
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib-PySide
 Author: LX
 Author-email: lx984608061@163.com
 License: GPL
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/animation/PropertyAnimation.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/animation/PropertyAnimation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/animation/animation.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/layout/flowLayout.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/layout/flowLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/progressBar/gradientBar.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/progressBar/gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/core/switchButtons/swButton.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/core/switchButtons/swButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/Qt/qt.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/Qt/qt.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/__init__.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/header/utility.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/header/utility.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/styleAnalysis.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/styleAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib/styles/superPainter/superPainter.py` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib/styles/superPainter/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/PKG-INFO` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib-PySide
-Version: 1.0
+Version: 1.1
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib-PySide
 Author: LX
 Author-email: lx984608061@163.com
 License: GPL
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PyQtGuiLib-PySide-1.0/PyQtGuiLib_PySide.egg-info/SOURCES.txt` & `PyQtGuiLib-PySide-1.1/PyQtGuiLib_PySide.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,25 @@
 README.md
 setup.py
 PyQtGuiLib/__init__.py
 PyQtGuiLib/animation/PropertyAnimation.py
 PyQtGuiLib/animation/__init__.py
 PyQtGuiLib/animation/animation.py
 PyQtGuiLib/core/__init__.py
+PyQtGuiLib/core/slideShow.py
 PyQtGuiLib/core/layout/__init__.py
 PyQtGuiLib/core/layout/flowLayout.py
+PyQtGuiLib/core/palettes/__init__.py
+PyQtGuiLib/core/palettes/colorHsv.py
+PyQtGuiLib/core/palettes/paletteFrame.py
+PyQtGuiLib/core/palettes/palettetools.py
+PyQtGuiLib/core/palettes/paletteTools/__init__.py
+PyQtGuiLib/core/palettes/paletteTools/area.py
+PyQtGuiLib/core/palettes/paletteTools/paletteToolUI.py
+PyQtGuiLib/core/palettes/paletteTools/palettetools.py
 PyQtGuiLib/core/progressBar/__init__.py
 PyQtGuiLib/core/progressBar/gradientBar.py
 PyQtGuiLib/core/switchButtons/__init__.py
 PyQtGuiLib/core/switchButtons/swButton.py
 PyQtGuiLib/header/__init__.py
 PyQtGuiLib/header/error.py
 PyQtGuiLib/header/utility.py
@@ -41,14 +50,15 @@
 PyQtGuiLib/styles/superPainter/superPainter.py
 PyQtGuiLib_PySide.egg-info/PKG-INFO
 PyQtGuiLib_PySide.egg-info/SOURCES.txt
 PyQtGuiLib_PySide.egg-info/dependency_links.txt
 PyQtGuiLib_PySide.egg-info/top_level.txt
 test/__init__.py
 test/test1.py
+test/test_PaletteTools.py
 test/test_gradientBar.py
 test/test_switchButton.py
 test/test_Animation/1.py
 test/test_Animation/__init__.py
 test/test_Animation/test_animation.py
 test/test_Animation/test_p_ani.py
 test/test_Animation/test_ani/1.py
```

### Comparing `PyQtGuiLib-PySide-1.0/setup.py` & `PyQtGuiLib-PySide-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name="PyQtGuiLib-PySide",
     packages =find_packages(),
-    version="1.0",
+    version="1.1",
     author="LX",
     author_email = "lx984608061@163.com",
     description = "Python version of the qt component library.",
     long_description=open('README.md', 'r',encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url = "https://github.com/LX-sys/PyQtGuiLib-PySide",
     license= "GPL",
```

### Comparing `PyQtGuiLib-PySide-1.0/test/test1.py` & `PyQtGuiLib-PySide-1.1/test/test1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_Animation/1.py` & `PyQtGuiLib-PySide-1.1/test/test_Animation/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_Animation/__init__.py` & `PyQtGuiLib-PySide-1.1/test/test_Animation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_Animation/test_ani/1.py` & `PyQtGuiLib-PySide-1.1/test/test_Animation/test_ani/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_Animation/test_animation.py` & `PyQtGuiLib-PySide-1.1/test/test_Animation/test_animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_Animation/test_p_ani.py` & `PyQtGuiLib-PySide-1.1/test/test_Animation/test_p_ani.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_gradientBar.py` & `PyQtGuiLib-PySide-1.1/test/test_gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_styleAnalysis/test1.py` & `PyQtGuiLib-PySide-1.1/test/test_styleAnalysis/test1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-PySide-1.0/test/test_switchButton.py` & `PyQtGuiLib-PySide-1.1/test/test_switchButton.py`

 * *Files identical despite different names*

