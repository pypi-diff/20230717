# Comparing `tmp/d3blocks-1.2.9.tar.gz` & `tmp/d3blocks-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3blocks-1.2.9.tar", last modified: Fri Mar 10 13:13:17 2023, max compression
+gzip compressed data, was "d3blocks-1.3.0.tar", last modified: Mon Jul 17 11:34:42 2023, max compression
```

## Comparing `d3blocks-1.2.9.tar` & `d3blocks-1.3.0.tar`

### file list

```diff
@@ -1,105 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.576271 d3blocks-1.2.9/
--rw-rw-rw-   0        0        0    35837 2022-09-16 10:26:19.000000 d3blocks-1.2.9/LICENSE
--rw-rw-rw-   0        0        0      340 2023-01-18 18:48:46.000000 d3blocks-1.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     7585 2023-03-10 13:13:17.574932 d3blocks-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     7036 2023-03-10 13:03:50.000000 d3blocks-1.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.071745 d3blocks-1.2.9/d3blocks/
--rw-rw-rw-   0        0        0     1155 2023-03-10 13:05:39.000000 d3blocks-1.2.9/d3blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.116256 d3blocks-1.2.9/d3blocks/chord/
--rw-rw-rw-   0        0        0    12585 2023-01-19 15:36:50.000000 d3blocks-1.2.9/d3blocks/chord/Chord.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/chord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.136169 d3blocks-1.2.9/d3blocks/chord/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/chord/d3js/__init__.py
--rw-rw-rw-   0        0        0     1000 2022-10-16 08:41:27.000000 d3blocks-1.2.9/d3blocks/chord/d3js/chord.html.j2
--rw-rw-rw-   0        0        0    59483 2022-10-16 11:19:33.000000 d3blocks-1.2.9/d3blocks/chord/d3js/chord.js
--rw-rw-rw-   0        0        0   107446 2023-03-10 13:02:54.000000 d3blocks-1.2.9/d3blocks/d3blocks.py
--rw-rw-rw-   0        0        0    66693 2023-03-10 12:57:47.000000 d3blocks-1.2.9/d3blocks/examples.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.153285 d3blocks-1.2.9/d3blocks/heatmap/
--rw-rw-rw-   0        0        0     9977 2023-01-28 20:43:48.000000 d3blocks-1.2.9/d3blocks/heatmap/Heatmap.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/heatmap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.179088 d3blocks-1.2.9/d3blocks/heatmap/d3js/
--rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2023-01-18 19:37:38.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js
--rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.v4.js
--rw-rw-rw-   0        0        0   124409 2023-01-17 11:55:33.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/heatmap.html.j2
--rw-rw-rw-   0        0        0     4212 2023-01-18 11:20:35.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/matrix.html.j2
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.188025 d3blocks-1.2.9/d3blocks/imageslider/
--rw-rw-rw-   0        0        0     8308 2023-01-19 15:40:30.000000 d3blocks-1.2.9/d3blocks/imageslider/Imageslider.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/imageslider/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.267060 d3blocks-1.2.9/d3blocks/imageslider/d3js/
--rw-rw-rw-   0        0        0        0 2022-09-22 13:52:17.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/.keep
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/__init__.py
--rw-rw-rw-   0        0        0     1666 2022-09-18 11:05:56.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/imageslider.html.j2
--rw-rw-rw-   0        0        0   247351 2022-07-13 19:24:39.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/jquery-2.1.1.js
--rw-rw-rw-   0        0        0     5426 2022-07-13 19:24:39.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/main.js
--rw-rw-rw-   0        0        0    51351 2022-07-13 19:24:39.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/modernizr.js
--rw-rw-rw-   0        0        0      947 2022-07-13 21:41:56.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/reset.css
--rw-rw-rw-   0        0        0     4116 2022-07-13 21:41:49.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/style.css
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.270843 d3blocks-1.2.9/d3blocks/matrix/
--rw-rw-rw-   0        0        0     9064 2023-01-19 15:39:23.000000 d3blocks-1.2.9/d3blocks/matrix/Matrix.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/matrix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.299247 d3blocks-1.2.9/d3blocks/matrix/d3js/
--rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
--rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/d3.v4.js
--rw-rw-rw-   0        0        0     4122 2023-01-18 19:44:22.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2
--rw-rw-rw-   0        0        0     3982 2023-01-18 19:36:40.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2.new
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.316017 d3blocks-1.2.9/d3blocks/movingbubbles/
--rw-rw-rw-   0        0        0    24345 2023-01-20 17:00:37.000000 d3blocks-1.2.9/d3blocks/movingbubbles/Movingbubbles.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/movingbubbles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.353660 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/__init__.py
--rw-rw-rw-   0        0        0   151125 2022-04-02 10:57:29.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
--rw-rw-rw-   0        0        0    10475 2023-01-20 16:57:23.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/movingbubbles.html.j2
--rw-rw-rw-   0        0        0     1901 2022-04-24 13:58:40.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/style.css
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.361636 d3blocks-1.2.9/d3blocks/particles/
--rw-rw-rw-   0        0        0     2998 2023-01-19 15:40:03.000000 d3blocks-1.2.9/d3blocks/particles/Particles.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/particles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.386583 d3blocks-1.2.9/d3blocks/particles/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/particles/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2022-09-07 21:21:56.000000 d3blocks-1.2.9/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js
--rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.9/d3blocks/particles/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6558 2022-10-19 19:55:00.000000 d3blocks-1.2.9/d3blocks/particles/d3js/particles.html.j2
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.411167 d3blocks-1.2.9/d3blocks/sankey/
--rw-rw-rw-   0        0        0     9014 2023-01-19 15:40:47.000000 d3blocks-1.2.9/d3blocks/sankey/Sankey.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/sankey/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.433484 d3blocks-1.2.9/d3blocks/sankey/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/sankey/d3js/__init__.py
--rw-rw-rw-   0        0        0     3634 2023-01-19 20:24:54.000000 d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.html.j2
--rw-rw-rw-   0        0        0    73109 2022-08-27 15:02:46.000000 d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.js
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.449662 d3blocks-1.2.9/d3blocks/scatter/
--rw-rw-rw-   0        0        0    14847 2023-01-19 15:44:33.000000 d3blocks-1.2.9/d3blocks/scatter/Scatter.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/scatter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.470646 d3blocks-1.2.9/d3blocks/scatter/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/scatter/d3js/__init__.py
--rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.9/d3blocks/scatter/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6774 2022-10-19 19:55:06.000000 d3blocks-1.2.9/d3blocks/scatter/d3js/scatter.html.j2
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.478839 d3blocks-1.2.9/d3blocks/tests/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/tests/__init__.py
--rw-rw-rw-   0        0        0    17320 2023-01-19 15:53:44.000000 d3blocks-1.2.9/d3blocks/tests/test_d3blocks.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.494693 d3blocks-1.2.9/d3blocks/timeseries/
--rw-rw-rw-   0        0        0     9363 2023-01-19 15:41:31.000000 d3blocks-1.2.9/d3blocks/timeseries/Timeseries.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.543168 d3blocks-1.2.9/d3blocks/timeseries/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/__init__.py
--rw-rw-rw-   0        0        0   337945 2022-04-21 07:39:27.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/d3.v3.js
--rw-rw-rw-   0        0        0    15492 2022-09-13 20:40:47.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/script.js
--rw-rw-rw-   0        0        0      735 2022-04-24 13:58:40.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/style.css
--rw-rw-rw-   0        0        0      864 2022-09-18 11:17:26.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/timeseries.html.j2
--rw-rw-rw-   0        0        0    11203 2023-01-20 12:56:28.000000 d3blocks-1.2.9/d3blocks/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.547089 d3blocks-1.2.9/d3blocks/violin/
--rw-rw-rw-   0        0        0    11196 2023-03-10 12:54:49.000000 d3blocks-1.2.9/d3blocks/violin/Violin.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/violin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.571939 d3blocks-1.2.9/d3blocks/violin/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/violin/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2022-09-01 20:28:35.000000 d3blocks-1.2.9/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
--rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.9/d3blocks/violin/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6317 2023-03-10 12:45:47.000000 d3blocks-1.2.9/d3blocks/violin/d3js/violin.html.j2
-drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.104457 d3blocks-1.2.9/d3blocks.egg-info/
--rw-rw-rw-   0        0        0     7585 2023-03-10 13:13:15.000000 d3blocks-1.2.9/d3blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2600 2023-03-10 13:13:16.000000 d3blocks-1.2.9/d3blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 13:13:15.000000 d3blocks-1.2.9/d3blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-03-10 13:13:16.000000 d3blocks-1.2.9/d3blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-10 13:13:16.000000 d3blocks-1.2.9/d3blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 13:13:17.576271 d3blocks-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-01-28 20:41:18.000000 d3blocks-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.888180 d3blocks-1.3.0/
+-rw-rw-rw-   0        0        0    35837 2022-09-16 10:26:19.000000 d3blocks-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      373 2023-04-08 17:50:13.000000 d3blocks-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8052 2023-07-17 11:34:42.887183 d3blocks-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7544 2023-07-17 11:10:04.000000 d3blocks-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.716619 d3blocks-1.3.0/d3blocks/
+-rw-rw-rw-   0        0        0     1335 2023-07-17 11:26:35.000000 d3blocks-1.3.0/d3blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.729704 d3blocks-1.3.0/d3blocks/chord/
+-rw-rw-rw-   0        0        0    12624 2023-05-17 19:00:50.000000 d3blocks-1.3.0/d3blocks/chord/Chord.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/chord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.731560 d3blocks-1.3.0/d3blocks/chord/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/chord/d3js/__init__.py
+-rw-rw-rw-   0        0        0     1019 2023-05-17 19:00:47.000000 d3blocks-1.3.0/d3blocks/chord/d3js/chord.html.j2
+-rw-rw-rw-   0        0        0    59483 2022-10-16 11:19:33.000000 d3blocks-1.3.0/d3blocks/chord/d3js/chord.js
+-rw-rw-rw-   0        0        0   122892 2023-07-17 11:20:48.000000 d3blocks-1.3.0/d3blocks/d3blocks.py
+-rw-rw-rw-   0        0        0    73058 2023-07-17 10:18:13.000000 d3blocks-1.3.0/d3blocks/examples.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.733559 d3blocks-1.3.0/d3blocks/heatmap/
+-rw-rw-rw-   0        0        0    10036 2023-05-17 18:28:13.000000 d3blocks-1.3.0/d3blocks/heatmap/Heatmap.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/heatmap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.753934 d3blocks-1.3.0/d3blocks/heatmap/d3js/
+-rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.3.0/d3blocks/heatmap/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2023-01-18 19:37:38.000000 d3blocks-1.3.0/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.3.0/d3blocks/heatmap/d3js/d3.v4.js
+-rw-rw-rw-   0        0        0   124426 2023-05-17 18:28:00.000000 d3blocks-1.3.0/d3blocks/heatmap/d3js/heatmap.html.j2
+-rw-rw-rw-   0        0        0     4225 2023-05-17 18:27:45.000000 d3blocks-1.3.0/d3blocks/heatmap/d3js/matrix.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.758503 d3blocks-1.3.0/d3blocks/imageslider/
+-rw-rw-rw-   0        0        0     8308 2023-01-19 15:40:30.000000 d3blocks-1.3.0/d3blocks/imageslider/Imageslider.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/imageslider/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.789903 d3blocks-1.3.0/d3blocks/imageslider/d3js/
+-rw-rw-rw-   0        0        0        0 2022-09-22 13:52:17.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/.keep
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/__init__.py
+-rw-rw-rw-   0        0        0     1666 2022-09-18 11:05:56.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/imageslider.html.j2
+-rw-rw-rw-   0        0        0   247351 2022-07-13 19:24:39.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/jquery-2.1.1.js
+-rw-rw-rw-   0        0        0     5426 2022-07-13 19:24:39.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/main.js
+-rw-rw-rw-   0        0        0    51351 2022-07-13 19:24:39.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/modernizr.js
+-rw-rw-rw-   0        0        0      947 2022-07-13 21:41:56.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/reset.css
+-rw-rw-rw-   0        0        0     4116 2022-07-13 21:41:49.000000 d3blocks-1.3.0/d3blocks/imageslider/d3js/style.css
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.794358 d3blocks-1.3.0/d3blocks/matrix/
+-rw-rw-rw-   0        0        0     9121 2023-05-17 18:35:04.000000 d3blocks-1.3.0/d3blocks/matrix/Matrix.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/matrix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.807324 d3blocks-1.3.0/d3blocks/matrix/d3js/
+-rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.3.0/d3blocks/matrix/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2020-11-17 20:33:44.000000 d3blocks-1.3.0/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.3.0/d3blocks/matrix/d3js/d3.v4.js
+-rw-rw-rw-   0        0        0     4133 2023-05-17 18:33:29.000000 d3blocks-1.3.0/d3blocks/matrix/d3js/matrix.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.810317 d3blocks-1.3.0/d3blocks/movingbubbles/
+-rw-rw-rw-   0        0        0    24393 2023-06-05 22:22:24.000000 d3blocks-1.3.0/d3blocks/movingbubbles/Movingbubbles.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/movingbubbles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.818318 d3blocks-1.3.0/d3blocks/movingbubbles/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/movingbubbles/d3js/__init__.py
+-rw-rw-rw-   0        0        0   151125 2022-04-02 10:57:29.000000 d3blocks-1.3.0/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
+-rw-rw-rw-   0        0        0    10492 2023-05-17 19:00:38.000000 d3blocks-1.3.0/d3blocks/movingbubbles/d3js/movingbubbles.html.j2
+-rw-rw-rw-   0        0        0     1901 2022-04-24 13:58:40.000000 d3blocks-1.3.0/d3blocks/movingbubbles/d3js/style.css
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.821291 d3blocks-1.3.0/d3blocks/particles/
+-rw-rw-rw-   0        0        0     2415 2023-05-17 19:00:21.000000 d3blocks-1.3.0/d3blocks/particles/Particles.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/particles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.831258 d3blocks-1.3.0/d3blocks/particles/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/particles/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2022-09-07 21:21:56.000000 d3blocks-1.3.0/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.3.0/d3blocks/particles/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6579 2023-05-17 19:01:19.000000 d3blocks-1.3.0/d3blocks/particles/d3js/particles.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.833252 d3blocks-1.3.0/d3blocks/sankey/
+-rw-rw-rw-   0        0        0     9055 2023-05-17 19:03:20.000000 d3blocks-1.3.0/d3blocks/sankey/Sankey.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/sankey/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.836231 d3blocks-1.3.0/d3blocks/sankey/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/sankey/d3js/__init__.py
+-rw-rw-rw-   0        0        0     3657 2023-05-17 19:04:38.000000 d3blocks-1.3.0/d3blocks/sankey/d3js/sankey.html.j2
+-rw-rw-rw-   0        0        0    73109 2022-08-27 15:02:46.000000 d3blocks-1.3.0/d3blocks/sankey/d3js/sankey.js
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.838313 d3blocks-1.3.0/d3blocks/scatter/
+-rw-rw-rw-   0        0        0    16279 2023-05-28 19:52:43.000000 d3blocks-1.3.0/d3blocks/scatter/Scatter.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/scatter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.840624 d3blocks-1.3.0/d3blocks/scatter/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/scatter/d3js/__init__.py
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.3.0/d3blocks/scatter/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6797 2023-05-17 19:08:52.000000 d3blocks-1.3.0/d3blocks/scatter/d3js/scatter.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.842335 d3blocks-1.3.0/d3blocks/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/tests/__init__.py
+-rw-rw-rw-   0        0        0    20793 2023-07-17 11:26:04.000000 d3blocks-1.3.0/d3blocks/tests/test_d3blocks.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.846325 d3blocks-1.3.0/d3blocks/timeseries/
+-rw-rw-rw-   0        0        0     9402 2023-05-17 19:10:20.000000 d3blocks-1.3.0/d3blocks/timeseries/Timeseries.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/timeseries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.852468 d3blocks-1.3.0/d3blocks/timeseries/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/timeseries/d3js/__init__.py
+-rw-rw-rw-   0        0        0   337945 2022-04-21 07:39:27.000000 d3blocks-1.3.0/d3blocks/timeseries/d3js/d3.v3.js
+-rw-rw-rw-   0        0        0    15492 2022-09-13 20:40:47.000000 d3blocks-1.3.0/d3blocks/timeseries/d3js/script.js
+-rw-rw-rw-   0        0        0      735 2022-04-24 13:58:40.000000 d3blocks-1.3.0/d3blocks/timeseries/d3js/style.css
+-rw-rw-rw-   0        0        0      883 2023-05-17 19:13:10.000000 d3blocks-1.3.0/d3blocks/timeseries/d3js/timeseries.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.853534 d3blocks-1.3.0/d3blocks/tree/
+-rw-rw-rw-   0        0        0     5965 2023-07-17 11:04:29.000000 d3blocks-1.3.0/d3blocks/tree/Tree.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.856274 d3blocks-1.3.0/d3blocks/tree/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/tree/d3js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.868234 d3blocks-1.3.0/d3blocks/treemap/
+-rw-rw-rw-   0        0        0     5751 2023-07-16 22:03:25.000000 d3blocks-1.3.0/d3blocks/treemap/Treemap.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/treemap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.874217 d3blocks-1.3.0/d3blocks/treemap/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/treemap/d3js/__init__.py
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.3.0/d3blocks/treemap/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     3126 2023-05-17 19:13:05.000000 d3blocks-1.3.0/d3blocks/treemap/d3js/treemap.html.j2
+-rw-rw-rw-   0        0        0    20368 2023-07-17 11:20:59.000000 d3blocks-1.3.0/d3blocks/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.879252 d3blocks-1.3.0/d3blocks/violin/
+-rw-rw-rw-   0        0        0    11370 2023-05-17 19:12:44.000000 d3blocks-1.3.0/d3blocks/violin/Violin.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/violin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.886276 d3blocks-1.3.0/d3blocks/violin/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.3.0/d3blocks/violin/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2022-09-01 20:28:35.000000 d3blocks-1.3.0/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.3.0/d3blocks/violin/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6431 2023-05-17 19:13:00.000000 d3blocks-1.3.0/d3blocks/violin/d3js/violin.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-17 11:34:42.727535 d3blocks-1.3.0/d3blocks.egg-info/
+-rw-rw-rw-   0        0        0     8052 2023-07-17 11:34:42.000000 d3blocks-1.3.0/d3blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2803 2023-07-17 11:34:42.000000 d3blocks-1.3.0/d3blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:34:42.000000 d3blocks-1.3.0/d3blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-07-17 11:34:42.000000 d3blocks-1.3.0/d3blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 11:34:42.000000 d3blocks-1.3.0/d3blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:34:42.888180 d3blocks-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-05-17 20:48:28.000000 d3blocks-1.3.0/setup.py
```

### Comparing `d3blocks-1.2.9/LICENSE` & `d3blocks-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/PKG-INFO` & `d3blocks-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: d3blocks
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python package d3blocks
 Home-page: https://github.com/d3blocks/d3blocks
-Download-URL: https://github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz
+Download-URL: https://github.com/d3blocks/d3blocks/archive/1.3.0.tar.gz
 Author: Erdogan Taskesen, Oliver Verver
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -84,16 +82,16 @@
 | [Scatter](https://d3blocks.github.io/d3blocks/pages/html/Scatter.html)             | ``` d3.scatter()  ```        | [Scatter](https://towardsdatascience.com/get-the-most-out-of-your-scatterplot-by-making-it-interactive-using-d3js-19939e3b046)       |
 | [Heatmap](https://d3blocks.github.io/d3blocks/pages/html/Heatmap.html)             | ``` d3.heatmap()  ```        | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Chord diagram](https://d3blocks.github.io/d3blocks/pages/html/Chord.html)         | ``` d3.chord()  ```          | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Timeseries](https://d3blocks.github.io/d3blocks/pages/html/Timeseries.html)       | ``` d3.timeseries()  ```     | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Image slider](https://d3blocks.github.io/d3blocks/pages/html/Imageslider.html)    | ``` d3.imageslider()  ```    | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Violin plot](https://d3blocks.github.io/d3blocks/pages/html/Violin.html)          | ``` d3.violin()  ```         | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Particles](https://d3blocks.github.io/d3blocks/pages/html/Particles.html)         | ``` d3.particles()  ```      | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Treemap](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html)             | ``` d3.treemap()  ```        | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Tree](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html)                | ``` d3.tree()  ```           | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 |                                                                                    |                              |                                                                                                                                      |
 
 -------------------------------------------------------------------------
 
 #### References
 * [bl.ocks](https://bl.ocks.org/)
 * [observablehq](https://observablehq.com/top)
-
-
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: d3blocks Version: 1.2.9 Summary: Python package
+Metadata-Version: 2.1 Name: d3blocks Version: 1.3.0 Summary: Python package
 d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
-github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz Author: Erdogan Taskesen,
-Oliver Verver Author-email: erdogant@gmail.com License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved Classifier: Operating System :: OS Independent Requires-Python:
->=3 Description-Content-Type: text/markdown License-File: LICENSE
+github.com/d3blocks/d3blocks/archive/1.3.0.tar.gz Author: Erdogan Taskesen,
+Oliver Verver Author-email: erdogant@gmail.com Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved Classifier: Operating System
+:: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE
            [https://github.com/d3blocks/d3blocks/blob/main/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
 v/d3blocks)](https://pypi.org/project/d3blocks/) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-blue)](https://d3blocks.github.io/d3blocks/)
 [![LOC](https://sloc.xyz/github/d3blocks/d3blocks/?category=code)](https://
 github.com/d3blocks/d3blocks/) [![Downloads](https://static.pepy.tech/
@@ -79,10 +79,16 @@
 standalone-d3js-charts-3dda98ce97d4) | | [Violin plot](https://
 d3blocks.github.io/d3blocks/pages/html/Violin.html) | ``` d3.violin() ``` |
 [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-
 create-interactive-and-standalone-d3js-charts-3dda98ce97d4) | | [Particles]
 (https://d3blocks.github.io/d3blocks/pages/html/Particles.html) | ```
 d3.particles() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-
 python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
-| | | | -----------------------------------------------------------------------
--- #### References * [bl.ocks](https://bl.ocks.org/) * [observablehq](https://
+| [Treemap](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html) | ```
+d3.treemap() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-
+python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Tree](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html) | ```
+d3.tree() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-
+library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) | | | |
+| ------------------------------------------------------------------------
+- #### References * [bl.ocks](https://bl.ocks.org/) * [observablehq](https://
 observablehq.com/top)
```

### Comparing `d3blocks-1.2.9/README.md` & `d3blocks-1.3.0/d3blocks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: d3blocks
+Version: 1.3.0
+Summary: Python package d3blocks
+Home-page: https://github.com/d3blocks/d3blocks
+Download-URL: https://github.com/d3blocks/d3blocks/archive/1.3.0.tar.gz
+Author: Erdogan Taskesen, Oliver Verver
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <a href="https://d3blocks.github.io/d3blocks/pages/html/index.html">
   <img src="https://github.com/d3blocks/d3blocks/blob/main/logo.png" align="center" width="600" /> 
   </a>
 </p>
 
 
@@ -67,14 +82,16 @@
 | [Scatter](https://d3blocks.github.io/d3blocks/pages/html/Scatter.html)             | ``` d3.scatter()  ```        | [Scatter](https://towardsdatascience.com/get-the-most-out-of-your-scatterplot-by-making-it-interactive-using-d3js-19939e3b046)       |
 | [Heatmap](https://d3blocks.github.io/d3blocks/pages/html/Heatmap.html)             | ``` d3.heatmap()  ```        | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Chord diagram](https://d3blocks.github.io/d3blocks/pages/html/Chord.html)         | ``` d3.chord()  ```          | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Timeseries](https://d3blocks.github.io/d3blocks/pages/html/Timeseries.html)       | ``` d3.timeseries()  ```     | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Image slider](https://d3blocks.github.io/d3blocks/pages/html/Imageslider.html)    | ``` d3.imageslider()  ```    | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Violin plot](https://d3blocks.github.io/d3blocks/pages/html/Violin.html)          | ``` d3.violin()  ```         | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Particles](https://d3blocks.github.io/d3blocks/pages/html/Particles.html)         | ``` d3.particles()  ```      | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Treemap](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html)             | ``` d3.treemap()  ```        | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Tree](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html)                | ``` d3.tree()  ```           | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 |                                                                                    |                              |                                                                                                                                      |
 
 -------------------------------------------------------------------------
 
 #### References
 * [bl.ocks](https://bl.ocks.org/)
 * [observablehq](https://observablehq.com/top)
```

#### html2text {}

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1 Name: d3blocks Version: 1.3.0 Summary: Python package
+d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
+github.com/d3blocks/d3blocks/archive/1.3.0.tar.gz Author: Erdogan Taskesen,
+Oliver Verver Author-email: erdogant@gmail.com Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved Classifier: Operating System
+:: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE
            [https://github.com/d3blocks/d3blocks/blob/main/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
 v/d3blocks)](https://pypi.org/project/d3blocks/) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-blue)](https://d3blocks.github.io/d3blocks/)
 [![LOC](https://sloc.xyz/github/d3blocks/d3blocks/?category=code)](https://
 github.com/d3blocks/d3blocks/) [![Downloads](https://static.pepy.tech/
@@ -72,10 +79,16 @@
 standalone-d3js-charts-3dda98ce97d4) | | [Violin plot](https://
 d3blocks.github.io/d3blocks/pages/html/Violin.html) | ``` d3.violin() ``` |
 [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-
 create-interactive-and-standalone-d3js-charts-3dda98ce97d4) | | [Particles]
 (https://d3blocks.github.io/d3blocks/pages/html/Particles.html) | ```
 d3.particles() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-
 python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
-| | | | -----------------------------------------------------------------------
--- #### References * [bl.ocks](https://bl.ocks.org/) * [observablehq](https://
+| [Treemap](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html) | ```
+d3.treemap() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-
+python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Tree](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html) | ```
+d3.tree() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-
+library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) | | | |
+| ------------------------------------------------------------------------
+- #### References * [bl.ocks](https://bl.ocks.org/) * [observablehq](https://
 observablehq.com/top)
```

### Comparing `d3blocks-1.2.9/d3blocks/__init__.py` & `d3blocks-1.3.0/d3blocks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from d3blocks.d3blocks import D3Blocks
 
+from d3blocks.utils import (
+    normalize,
+    )
+
 __author__ = 'Erdogan Taskesen, Oliver Verver'
 __email__ = 'erdogant@gmail.com, mail@oliver3.nl'
-__version__ = '1.2.9'
+__version__ = '1.3.0'
 
 # module level doc-string
 __doc__ = """
 d3blocks
 =====================================================================
 
-Description
------------
 d3blocks is for the creation of stand-alone and interactive d3 graphs.
+Create interactive, stand-alone, and visually attractive charts that are built on the graphics of d3 javascript (d3js)
+but configurable with Python.
 
 References
 ----------
 * Github : https://github.com/d3blocks/d3blocks
 * Docs: https://d3blocks.github.io/d3blocks/
 * D3Blocks: https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4
 * D3Graph: https://towardsdatascience.com/creating-beautiful-stand-alone-interactive-d3-charts-with-python-804117cb95a7
```

### Comparing `d3blocks-1.2.9/d3blocks/chord/Chord.py` & `d3blocks-1.3.0/d3blocks/chord/Chord.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
     """
     content = {
         'json_data': X,
         'TITLE': config['title'],
         'WIDTH': config['figsize'][0],
         'HEIGHT': config['figsize'][1],
         'FONTSIZE': config['fontsize'],
+        'SUPPORT': config['support'],
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.chord', package_path='d3js'))
```

### Comparing `d3blocks-1.2.9/d3blocks/chord/d3js/chord.html.j2` & `d3blocks-1.3.0/d3blocks/chord/d3js/chord.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -36,9 +36,12 @@
             width: {{ WIDTH }},
             height: {{ HEIGHT }},
         });
     });
 
 </script>
 <div id="chart"></div>
+
+{{ SUPPORT }}
+
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1 +1,2 @@
 
+{{ SUPPORT }}
```

### Comparing `d3blocks-1.2.9/d3blocks/chord/d3js/chord.js` & `d3blocks-1.3.0/d3blocks/chord/d3js/chord.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/d3blocks.py` & `d3blocks-1.3.0/d3blocks/d3blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,44 +8,47 @@
 import logging
 import numpy as np
 import zipfile
 import webbrowser
 import random
 import time
 from typing import List, Union, Tuple
+from elasticgraph import Elasticgraph
+import d3graph as d3network
 
 import d3blocks.movingbubbles.Movingbubbles as Movingbubbles
 import d3blocks.timeseries.Timeseries as Timeseries
 import d3blocks.sankey.Sankey as Sankey
 import d3blocks.imageslider.Imageslider as Imageslider
 import d3blocks.chord.Chord as Chord
 import d3blocks.scatter.Scatter as Scatter
 import d3blocks.violin.Violin as Violin
 import d3blocks.particles.Particles as Particles
 import d3blocks.heatmap.Heatmap as Heatmap
 import d3blocks.matrix.Matrix as Matrix
+import d3blocks.treemap.Treemap as Treemap
+import d3blocks.tree.Tree as Tree
 import d3blocks.utils as utils
 
 # ###################### DEBUG ONLY ###################
 # import movingbubbles.Movingbubbles as Movingbubbles
 # import timeseries.Timeseries as Timeseries
 # import sankey.Sankey as Sankey
 # import imageslider.Imageslider as Imageslider
 # import chord.Chord as Chord
 # import scatter.Scatter as Scatter
 # import violin.Violin as Violin
 # import particles.Particles as Particles
 # import heatmap.Heatmap as Heatmap
 # import matrix.Matrix as Matrix
+# import treemap.Treemap as Treemap
+# import tree.Tree as Tree
 # import utils
 # #####################################################
 
-from elasticgraph import Elasticgraph
-import d3graph as d3network
-
 logger = logging.getLogger('')
 for handler in logger.handlers[:]:  # get rid of existing old handlers
     logger.removeHandler(handler)
 console = logging.StreamHandler()
 formatter = logging.Formatter('[d3blocks] >%(levelname)s> %(message)s')
 console.setFormatter(formatter)
 logger.addHandler(console)
@@ -58,14 +61,20 @@
     Parameters
     ----------
     frame : Bool, (default: True)
         True: Return in DataFrame.
         False: Return in dictionary.
     verbose : int, optional
         Verbose message. The default is 20.
+    support : String, (default: True)
+            This library is free of use and lets keep it this way! Support the project. It will cost you nothing.
+            * True: I support this project! It is even better when you occasionally click on the ethical add.
+            * 'text': I support this project with a text add.
+            * 'image': I support this project with an image add.
+            * False: I want to support in a different manner: https://d3blocks.github.io/d3blocks/pages/html/Documentation.html
 
     Returns
     -------
     None.
 
     References
     ----------
@@ -75,29 +84,30 @@
     * D3Graph: https://towardsdatascience.com/creating-beautiful-stand-alone-interactive-d3-charts-with-python-804117cb95a7
     * Scatter: https://towardsdatascience.com/get-the-most-out-of-your-scatterplot-by-making-it-interactive-using-d3js-19939e3b046
     * Sankey: https://towardsdatascience.com/hands-on-guide-to-create-beautiful-sankey-charts-in-d3js-with-python-8ddab43edb43
     * Movingbubbles: https://towardsdatascience.com/how-to-create-storytelling-moving-bubbles-charts-in-d3js-with-python-b31cec7b8226
 
     """
 
-    def __init__(self, chart: str = None, frame: bool = True, verbose: int = 20):
+    def __init__(self, chart: str = None, frame: bool = True, verbose: int = 20, support='text'):
         """Initialize d3blocks with user-defined parameters."""
         # Set the logger
         if chart is not None: chart = str.capitalize(chart)
         set_logger(verbose=verbose)
         # Clean
         self._clean(clean_config=True, logger=logger)
         # Get chart function
         self.chart = set_chart_func(chart=chart, logger=logger)
         # Set configurations for specific charts
         self.config = {}
         self.set_config()
         # Initialize empty config
         self.config['chart'] = chart
         self.config['frame'] = frame
+        self.config['support'] = utils.get_support(support)
         self.config['curpath'] = os.path.dirname(os.path.abspath(__file__))
 
     def particles(self,
                   text: str,
                   radius: int = 3,
                   collision: float = 0.05,
                   fontsize: int = 180,
@@ -175,15 +185,14 @@
                          filepath='D3Blocks.html',
                          collision=0.05,
                          spacing=7,
                          figsize=[750, 150],
                          fontsize=130,
                          cmap='Turbo',
                          color_background='#ffffff')
-        >>> #
 
         References
         ----------
         * https://d3blocks.github.io/d3blocks/pages/html/Particles.html
         * https://observablehq.com/@d3/color-schemes
 
         """
@@ -216,16 +225,17 @@
                y,
                size=5,
                color=None,
                x_order=None,
                opacity=0.6,
                stroke='#000000',
                tooltip=None,
-               cmap='inferno',
                fontsize=12,
+               fontsize_axis=12,
+               cmap='inferno',
                bins=50,
                ylim=[None, None],
                title='Violin - D3blocks',
                filepath='violin.html',
                figsize=[None, None],
                showfig=True,
                overwrite=True,
@@ -258,19 +268,21 @@
         opacity: float or list/array [0-1] (default: 0.6)
             Opacity of the dot. Shoud be same size as (x,y)
         stroke: list/array of hex colors with same size as (x,y)
             Edgecolor of dot in hex colors.
                 * '#000000' : Edge colors are all black.
         tooltip: list of labels with same size as (x,y)
             labels of the samples.
+        fontsize : int or list of labels with the same size as (x, y), optional (default: 12)
+            Text fontsize for the tooltip.
+        fontsize_axis : int, optional (default: 12)
+            Text fontsize for the x-axis and y-axis.
         cmap : String, (default: 'inferno')
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
-        fontsize : int, optional (default: 12)
-            Text fontsize.
+                * 'tab20c', 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
         bins : Int (default: 50)
             The bin size is the 'resolution' of the violin plot.
         ylim : tuple, (default: [None, None])
             Limit the width of the y-axis [min, max].
                 *  [None, None] : The width is determined based on the min-max value range.
         title : String, (default: None)
             Title of the figure.
@@ -360,15 +372,15 @@
 
         """
         # Cleaning
         self._clean(clean_config=reset_properties, logger=logger)
         # Store chart
         self.chart = set_chart_func('Violin', logger)
         # Store properties
-        self.config = self.chart.set_config(config=self.config, filepath=filepath, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, cmap=cmap, bins=bins, ylim=ylim, x_order=x_order, reset_properties=reset_properties, notebook=notebook, fontsize=fontsize, logger=logger)
+        self.config = self.chart.set_config(config=self.config, filepath=filepath, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, cmap=cmap, bins=bins, ylim=ylim, x_order=x_order, reset_properties=reset_properties, notebook=notebook, fontsize=fontsize, fontsize_axis=fontsize_axis, logger=logger)
         # Remvove quotes from source-target node_properties
         self.edge_properties = self.chart.set_edge_properties(x, y, config=self.config, color=color, size=size, stroke=stroke, opacity=opacity, tooltip=tooltip, cmap=self.config['cmap'], x_order=self.config['x_order'], fontsize=self.config['fontsize'], logger=logger)
         # Set default label properties
         if self.config['reset_properties'] or (not hasattr(self, 'node_properties')):
             self.set_node_properties(np.unique(self.edge_properties['x'].values), cmap=self.config['cmap'])
         # Create the plot
         return self.show()
@@ -376,17 +388,18 @@
     def scatter(self,
                 x,
                 y,
                 x1=None,
                 y1=None,
                 x2=None,
                 y2=None,
+                jitter=None,
                 size=3,
                 color='#002147',
-                c_gradient=None,
+                c_gradient='opaque',
                 opacity=0.8,
                 stroke='#ffffff',
                 tooltip=None,
                 cmap='tab20',
                 scale=False,
                 color_background='#ffffff',
                 label_radio=['(x, y)', '(x1, y1)', '(x2, y2)'],
@@ -418,34 +431,38 @@
             Second set of 1d coordinates x-axis.
         y1 : numpy array
             Second set of 1d coordinates y-axis.
         x2 : numpy array
             Third set of 1d coordinates x-axis.
         y2 : numpy array
             Third set of 1d coordinates y-axis.
+        jitter : float, default: None
+            Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
         size: list/array of with same size as (x,y).
             Size of the samples.
         color: list/array of hex colors with same size as (x,y)
                 * '#ffffff' : All dots are get the same hex color.
                 * None: The same color as for c is applied.
                 * ['#000000', '#ffffff',...]: list/array of hex colors with same size as (x,y)
         stroke: list/array of hex colors with same size as (x,y)
             Edgecolor of dotsize in hex colors.
                 * '#000000' : All dots are get the same hex color.
                 * ['#000000', '#ffffff',...]: list/array of hex colors with same size as (x,y)
-        c_gradient : String, (default: None)
-            Make a lineair gradient based on the density for the particular class label.
-                * '#FFFFFF'
+        c_gradient : String, (default: 'opaque')
+            Hex color to make a lineair gradient using the density.
+                * None: Do not use gradient.
+                * opaque: Towards the edges the points become more transparant. This will stress the dense areas and make scatter plot tidy.
+                * '#FFFFFF': Towards the edges it smooths into this color
         opacity: float or list/array [0-1]
             Opacity of the dot. Shoud be same size as (x,y)
         tooltip: list of labels with same size as (x,y)
             labels of the samples.
         cmap : String, (default: 'inferno')
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
+                * 'tab20c', 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
         scale: Bool, optional
             Scale datapoints. The default is False.
         label_radio: List ['(x, y)', '(x1, y1)', '(x2, y2)']
             The labels used for the radiobuttons.
         set_xlim : tuple, (default: [None, None])
             Width of the x-axis: The default is extracted from the data with 10% spacing.
         set_ylim : tuple, (default: [None, None])
@@ -591,21 +608,21 @@
 
         """
         # Cleaning
         self._clean(clean_config=reset_properties, logger=logger)
         # Store chart
         self.chart = set_chart_func('Scatter', logger)
         # Store properties
-        self.config = self.chart.set_config(config=self.config, filepath=filepath, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, cmap=cmap, scale=scale, ylim=ylim, xlim=xlim, label_radio=label_radio, color_background=color_background, reset_properties=reset_properties, notebook=notebook, logger=logger)
+        self.config = self.chart.set_config(config=self.config, filepath=filepath, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, cmap=cmap, scale=scale, ylim=ylim, xlim=xlim, label_radio=label_radio, color_background=color_background, reset_properties=reset_properties, notebook=notebook, jitter=jitter, logger=logger)
         # Check exceptions
         Scatter.check_exceptions(x, y, x1, y1, x2, y2, size, color, tooltip, logger)
         # Set node properties
         self.set_node_properties()
         # Set edge properties
-        self.set_edge_properties(x, y, x1=x1, y1=y1, x2=x2, y2=y2, color=color, size=size, tooltip=tooltip, opacity=opacity, c_gradient=c_gradient, stroke=stroke, cmap=self.config['cmap'], scale=self.config['scale'], logger=logger)
+        self.set_edge_properties(x, y, x1=x1, y1=y1, x2=x2, y2=y2, color=color, size=size, tooltip=tooltip, opacity=opacity, c_gradient=c_gradient, stroke=stroke, cmap=self.config['cmap'], scale=self.config['scale'], jitter=self.config['jitter'], logger=logger)
         # Create the plot
         return self.show()
 
     def chord(self,
               df,
               color='source',
               opacity='source',
@@ -647,15 +664,15 @@
                 * 'target': Opacity of edges/links similar to that of target-opacity node.
                 * 0.8: All links have the same opacity.
                 * [0.1, 0.75,...]: Set opacity per edge/link.
         fontsize : int, (default: 8)
             The Fontsize.
         cmap : String, (default: 'tab20')
             colormap is only used in case color=None. All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
+                * 'tab20c', 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
         title : String, (default: None)
             Title of the figure.
                 * 'Chord'
         filepath : String, (Default: user temp directory)
             File path to save the output.
                 * Temporarily path: 'd3blocks.html'
                 * Relative path: './d3blocks.html'
@@ -1102,15 +1119,15 @@
             The time notes will be shown between specific time points.
                 * time_notes = [{"start_minute": 1,
                                "stop_minute": 5,
                                "note": "Enter your note here and it is shown between 1 min and 5 min."}]
             time_notes.append[{"start_minute": 6, "stop_minute": 10, "note": "Enter your second note here and it is shown between 6 min and 10 min."}]
         cmap : String, (default: 'Set1')
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2'
+                * 'tab20c', 'Set1', 'Set2'
                 * 'rainbow', 'bwr', 'binary', 'seismic'
                 * 'Blues', 'Reds', 'Pastel1', 'Paired'
                 * 'twilight', 'hsv', 'inferno'
         title : String, (default: None)
             Title of the figure.
                 * 'Movingbubbles'
         filepath : String, (Default: user temp directory)
@@ -1259,15 +1276,15 @@
                 * False: Do not change the input order.
         whitelist : str, optional
             Keep only columns containing this (sub)string (case insensitive)
         fontsize : int, (default: 14)
             Fontsize of the fonts in the circle.
         cmap : String, (default: 'Set1')
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv', 'inferno'
+                * 'tab20c', 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv', 'inferno'
         title : String, (default: None)
             Title of the figure.
                 * 'Timeseries'
         filepath : String, (Default: user temp directory)
             File path to save the output.
                 * Temporarily path: 'd3blocks.html'
                 * Relative path: './d3blocks.html'
@@ -1407,15 +1424,15 @@
             Range of colors starting with maximum value. Increasing this value will color the cells more discrete.
                 * 1 : cells above value >1 are capped.
             None : cells are colored based on the maximum value in the input data.
         cluster_params : dict (defaults)
             Parameters for clustering the data and using the cluster labels to color the heatmap. See references for more information.
         cmap : String, (default: 'Set1')
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv', 'inferno'
+                * 'tab20c', 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv', 'inferno'
         title : String, (default: None)
             Title of the figure.
                 * 'Heatmap'
         filepath : String, (Default: user temp directory)
             File path to save the output.
                 * Temporarily path: 'd3blocks.html'
                 * Relative path: './d3blocks.html'
@@ -1628,14 +1645,15 @@
                 filepath='d3graph.html',
                 figsize=[1500, 800],
                 collision=0.5,
                 charge=400,
                 slider=[None, None],
                 notebook=False,
                 showfig=True,
+                support='text',
                 overwrite=True):
         """d3graph block.
 
         d3graph is integrated in d3blocks and is to create interactive and stand-alone D3 force-directed graphs.
         The input data is a dataframe containing source, target, and weight. In underneath example, we load the energy
         dataset which contains 68 relationships that are stored in a DataFrame with the columns source, target, and weight.
         The nodes are colored based on the Louvain heuristics which is the partition of highest modularity, i.e.
@@ -1756,39 +1774,39 @@
         self.config['notebook'] = notebook
 
         # Copy of data
         df = df.copy()
         # Remvove quotes from source-target labels
         df = utils.remove_quotes(df)
         # Initialize network graph
-        self.D3graph = d3network.d3graph(collision=collision, charge=charge, slider=slider)
+        self.D3graph = d3network.d3graph(collision=collision, charge=charge, slider=slider, support=support)
         # Convert vector to adjmat
         adjmat = d3network.vec2adjmat(df['source'], df['target'], weight=df['weight'])
         # Create default graph
         self.D3graph.graph(adjmat, color=color, size=size, scaler=scaler)
         # Open the webbrowser
         self.D3graph.show(figsize=figsize, title=title, filepath=filepath, showfig=showfig, overwrite=overwrite)
         # Display the chart
         # return self.display(html)
 
     def elasticgraph(self,
-                  df,
-                  scaler='zscore',
-                  group='cluster',
-                  title='Elasticgraph - D3blocks',
-                  filepath='Elasticgraph.html',
-                  figsize=[None, None],
-                  collision=0.5,
-                  charge=250,
-                  size=4,
-                  hull_offset=15,
-                  single_click_expand=False,
-                  notebook=False,
-                  showfig=False,
-                  overwrite=True):
+                     df,
+                     scaler='zscore',
+                     group='cluster',
+                     title='Elasticgraph - D3blocks',
+                     filepath='Elasticgraph.html',
+                     figsize=[None, None],
+                     collision=0.5,
+                     charge=250,
+                     size=4,
+                     hull_offset=15,
+                     single_click_expand=False,
+                     notebook=False,
+                     showfig=False,
+                     overwrite=True):
         """D3 Elasticgraph block.
 
         Elasticgraph is integrated in d3blocks to create interactive and stand-alone D3 force-directed graphs for which
         the groups are clustered. The original d3js is forked from Ger Hobbelts (see references). The input data is a
         dataframe containing source, target, and weight. This graph relies on the properties of d3graph and is also utilized
         in the d3blocks library.
         In underneath example, we load an example dataset which contains K relationships that are stored in a DataFrame
@@ -1914,14 +1932,308 @@
         # Create default graph
         self.Elasticgraph.graph(adjmat, group=group, scaler=scaler)
         # Open the webbrowser
         self.Elasticgraph.show(figsize=figsize, title=title, filepath=filepath, showfig=showfig, overwrite=overwrite)
         # Display the chart
         # return self.display(html)
 
+    def tree(self,
+             df,
+             hierarchy = [1, 2, 3, 4, 5, 6, 7, 8],
+             margin: dict = {"top": 20, "right": 60, "bottom": 20, "left": 44.05},
+             font: dict = {'size': 10},
+             title: str = 'Tree - D3blocks',
+             filepath: str = 'tree.html',
+             figsize: Tuple[int, int] = [960, 700],
+             showfig: bool = True,
+             overwrite: bool = True,
+             notebook: bool = False,
+             reset_properties: bool = True,
+             ):
+        """Tree block.
+
+        A Tree chart is a visualization to hierarchically show the data.
+        For demonstration purposes, the "energy" dataset can be used.
+        The javascript code is forked from Mike Bostock, inspired by R-Shiny and then Pythonized.
+
+        Parameters
+        ----------
+        df : pd.DataFrame()
+            Input data containing the following columns:
+                * 'source', 'target', 'weight'
+        hierarchy : list
+            Expand or substract the hierarchical structure. No information is lossed. The eight branches are shown by default.
+            * [1, 2, 3, 4, 5, 6, 7, 8]
+        margin : dict.
+            margin, in pixels.
+                * {"top": 40, "right": 10, "bottom": 10, "left": 10}
+        font : dict.
+            font properties.
+                * {'size': 10}
+        title : String, (default: None)
+            Title of the figure.
+                * 'Treemap'
+        filepath : String, (Default: user temp directory)
+                * File path to save the output.
+                * Temporarily path: 'd3blocks.html'
+                * Relative path: './d3blocks.html'
+                * Absolute path: 'c://temp//d3blocks.html'
+                * None: Return HTML
+        figsize : tuple
+            Size of the figure in the browser, [width, height].
+                * [1000, 600]
+                * [None, None]: Use the screen resolution.
+        showfig : bool, (default: True)
+                * True: Open browser-window.
+                * False: Do not open browser-window.
+        overwrite : bool, (default: True)
+                * True: Overwrite the html in the destination directory.
+                * False: Do not overwrite destination file but show warning instead.
+        notebook : bool
+                * True: Use IPython to show chart in notebook.
+                * False: Do not use IPython.
+        reset_properties : bool, (default: True)
+                * True: Reset the node_properties at each run.
+                * False: Use the d3.node_properties()
+
+        Returns
+        -------
+        d3.node_properties: DataFrame of dictionary
+             Contains properties of the unique input label/nodes/samples.
+
+        d3.edge_properties: DataFrame of dictionary
+             Contains properties of the unique input edges/links.
+
+        d3.config: dictionary
+             Contains configuration properties.
+
+        Examples
+        --------
+        >>> # Load d3blocks
+        >>> from d3blocks import D3Blocks
+        >>> #
+        >>> # Initialize
+        >>> d3 = D3Blocks()
+        >>> #
+        >>> # Load example data
+        >>> df = d3.import_example('energy')
+        >>> #
+        >>> # Plot
+        >>> d3.tree(df)
+        >>> #
+
+        Examples
+        --------
+        >>> # Load library
+        >>> from d3blocks import D3Blocks
+        >>>
+        >>> # Initialize
+        >>> d3 = D3Blocks(verbose='info', chart='tree', frame=False)
+        >>>
+        >>> # Import example
+        >>> df = d3.import_example('energy')
+        >>>
+        >>> # Set node properties
+        >>> d3.set_node_properties(df)
+        >>>
+        >>> # Set specific properties
+        >>> d3.node_properties.get('Bio-conversion')['size'] = 30
+        >>> d3.node_properties.get('Bio-conversion')['color'] = '#000000'
+        >>> d3.node_properties.get('Bio-conversion')['tooltip'] = 'Title: P Operations<br><img src="https://source.unsplash.com/collection/385548/150x100">'
+        >>> d3.node_properties.get('Bio-conversion')['edge_color'] = '#00FFFF'
+        >>> d3.node_properties.get('Bio-conversion')['edge_size'] = 5
+        >>> d3.node_properties.get('Bio-conversion')['opacity'] = 0.4
+        >>>
+        >>> # Set properties for Losses
+        >>> d3.node_properties.get('Losses')['color'] = '#FF0000'
+        >>> d3.node_properties.get('Losses')['size'] = 15
+        >>> d3.node_properties.get('Losses')['tooltip'] = ''
+        >>>
+        >>> # Set properties for Agriculture
+        >>> d3.node_properties.get('Agriculture')['color'] = '#00FFFF'
+        >>> d3.node_properties.get('Agriculture')['size'] = 5
+        >>> d3.node_properties.get('Agriculture')['edge_color'] = '#89CFF0'
+        >>> d3.node_properties.get('Agriculture')['edge_size'] = 3
+        >>> d3.node_properties.get('Agriculture')['opacity'] = 0.7
+        >>>
+        >>> # Set edge properties
+        >>> d3.set_edge_properties(df)
+        >>>
+        >>> # Show chart
+        >>> d3.show(hierarchy=[1, 2, 3, 4, 5, 6, 7, 8], filepath=r'c:\temp\tree.html')
+
+        Examples
+        --------
+        >>> # Load d3blocks
+        >>> from d3blocks import D3Blocks
+        >>> #
+        >>> # Initialize
+        >>> d3 = D3Blocks(chart='tree', frame=True)
+        >>> #
+        >>> # Import example
+        >>> df = d3.import_example('energy')
+        >>> #
+        >>> # Node properties
+        >>> d3.set_node_properties(df)
+        >>> print(d3.node_properties)
+        >>> #
+        >>> d3.set_edge_properties(df)
+        >>> print(d3.edge_properties)
+        >>> #
+        >>> # Show the chart
+        >>> d3.show()
+
+        References
+        ----------
+        * https://d3js.org/d3-hierarchy/tree
+        * https://d3blocks.github.io/d3blocks/pages/html/Tree.html
+
+        """
+        # Cleaning
+        self._clean(clean_config=reset_properties, logger=logger)
+        # Store chart
+        self.chart = set_chart_func('Tree', logger)
+        # Store properties
+        self.config = self.chart.set_config(config=self.config, filepath=filepath, font=font, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, margin=margin, reset_properties=reset_properties, notebook=notebook, hierarchy=hierarchy, logger=logger)
+        # Set default label properties
+        if self.config['reset_properties'] or (not hasattr(self, 'node_properties')):
+            self.set_node_properties(df, cmap=self.config['cmap'], labels=df.columns.values[:-1].astype(str))
+        # Set edge properties
+        self.set_edge_properties(df)
+        # Create the plot
+        return self.show()
+
+    def treemap(self,
+                df,
+                margin: dict = {"top": 40, "right": 10, "bottom": 10, "left": 10},
+                border: dict = {'type': 'solid', 'color': '#FFFFFF', 'width': 1},
+                font: dict = {'size': 10, 'type': 'sans-serif', 'position': 'absolute'},
+                title: str = 'Treemap - D3blocks',
+                filepath: str = 'treemap.html',
+                figsize: Tuple[int, int] = [1000, 600],
+                showfig: bool = True,
+                overwrite: bool = True,
+                notebook: bool = False,
+                reset_properties: bool = True,
+                ):
+        """Treemap block.
+
+        A Treemap chart is a visualization to hierarchically show the data as a set of nested rectangles.
+        For demonstration purposes, the "energy" and "stormofswords" dataset can be used.
+        The javascript code is forked from Mike Bostock and then Pythonized.
+
+        Parameters
+        ----------
+        df : pd.DataFrame()
+            Input data containing the following columns:
+                * 'source', 'target', 'weight'
+                * 'level0', 'level1', 'level2', 'weight'
+        margin : dict.
+            margin, in pixels.
+                * {"top": 40, "right": 10, "bottom": 10, "left": 10}
+        border : dict.
+            border properties.
+                * {'type': 'solid', 'color': '#FFFFFF', 'width': 1}
+        font : dict.
+            font properties.
+                * {'size': 10, 'type':'sans-serif', 'position': 'absolute'}
+        title : String, (default: None)
+            Title of the figure.
+                * 'Treemap'
+        filepath : String, (Default: user temp directory)
+                * File path to save the output.
+                * Temporarily path: 'd3blocks.html'
+                * Relative path: './d3blocks.html'
+                * Absolute path: 'c://temp//d3blocks.html'
+                * None: Return HTML
+        figsize : tuple
+            Size of the figure in the browser, [width, height].
+                * [1000, 600]
+                * [None, None]: Use the screen resolution.
+        showfig : bool, (default: True)
+                * True: Open browser-window.
+                * False: Do not open browser-window.
+        overwrite : bool, (default: True)
+                * True: Overwrite the html in the destination directory.
+                * False: Do not overwrite destination file but show warning instead.
+        notebook : bool
+                * True: Use IPython to show chart in notebook.
+                * False: Do not use IPython.
+        reset_properties : bool, (default: True)
+                * True: Reset the node_properties at each run.
+                * False: Use the d3.node_properties()
+
+        Returns
+        -------
+        d3.node_properties: DataFrame of dictionary
+             Contains properties of the unique input label/nodes/samples.
+
+        d3.edge_properties: DataFrame of dictionary
+             Contains properties of the unique input edges/links.
+
+        d3.config: dictionary
+             Contains configuration properties.
+
+        Examples
+        --------
+        >>> # Load d3blocks
+        >>> from d3blocks import D3Blocks
+        >>> #
+        >>> # Initialize
+        >>> d3 = D3Blocks()
+        >>> #
+        >>> # Load example data
+        >>> df = d3.import_example('energy')
+        >>> df = d3.import_example('animals')
+        >>> #
+        >>> # Plot
+        >>> d3.treemap(df)
+        >>> #
+
+        Examples
+        --------
+        >>> # Load d3blocks
+        >>> from d3blocks import D3Blocks
+        >>> #
+        >>> # Initialize
+        >>> d3 = D3Blocks(chart='Treemap', frame=True)
+        >>> #
+        >>> # Import example
+        >>> df = d3.import_example('energy')
+        >>> #
+        >>> # Node properties
+        >>> d3.set_node_properties(df)
+        >>> print(d3.node_properties)
+        >>> #
+        >>> d3.set_edge_properties(df)
+        >>> print(d3.edge_properties)
+        >>> #
+        >>> # Show the chart
+        >>> d3.show()
+
+        References
+        ----------
+        * Mike Bostock; http://bl.ocks.org/mbostock/4063582
+        * https://d3blocks.github.io/d3blocks/pages/html/Treemap.html
+
+        """
+        # Cleaning
+        self._clean(clean_config=reset_properties, logger=logger)
+        # Store chart
+        self.chart = set_chart_func('Treemap', logger)
+        # Store properties
+        self.config = self.chart.set_config(config=self.config, filepath=filepath, border=border, font=font, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, margin=margin, reset_properties=reset_properties, notebook=notebook, logger=logger)
+        # Set default label properties
+        if self.config['reset_properties'] or (not hasattr(self, 'node_properties')):
+            self.set_node_properties(df, cmap=self.config['cmap'], labels=df.columns.values[:-1].astype(str))
+        # Set edge properties
+        self.set_edge_properties(df)
+        # Create the plot
+        return self.show()
+
     def set_edge_properties(self, *args, **kwargs):
         """Set edge properties.
 
         The input for edge properties are the arguments that are inherited from the chart-function. As an example, the
         edge properties for the scatter chart are those described in the scatter function.
 
         Parameters
@@ -1946,15 +2258,15 @@
                 * 'source': Opacity of edges/links similar to that of source-opacity node.
                 * 'target': Opacity of edges/links similar to that of target-opacity node.
                 * 0.8: All links have the same opacity.
                 * [0.1, 0.75,...]: Set opacity per edge/link.
         cmap : String, (default: 'tab20')
             colormap is only used in case color=None.
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
-                * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
+                * 'tab20c', 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
 
         Returns
         -------
         None.
 
         """
         if self.config['chart'] is None:
@@ -2092,16 +2404,17 @@
         if logger is not None: logger.info('Cleaning edge_properties and config parameters..')
         if hasattr(self, 'G'): del self.G
         if hasattr(self, 'edge_properties'): del self.edge_properties
         if clean_config and hasattr(self, 'config'):
             # Remove all configurations except for the chart, frame and path
             chart = self.config.get('chart', None)
             frame = self.config.get('frame', True)
+            support = self.config.get('support', 'text')
             curpath = self.config.get('curpath', os.path.dirname(os.path.abspath(__file__)))
-            self.config = {'chart': chart, 'frame': frame, 'curpath': curpath, 'notebook': False}
+            self.config = {'chart': chart, 'frame': frame, 'curpath': curpath, 'notebook': False, 'support': support}
 
     @staticmethod
     def vec2adjmat(source, target, weight=None, symmetric=True, aggfunc='sum'):
         """Convert source and target into adjacency matrix.
 
         Parameters
         ----------
@@ -2188,14 +2501,15 @@
                 * "southern_nebula_internet"
                 * "cancer"
                 * "breast_cancer"
                 * "iris"
                 * "occupancy"
                 * "climate"
                 * "mnist"
+                * "animals"
         n : int, (default: 1000).
             Number of events (samples).
         c : int, (default: 100).
             Number of classes.
         date_start : str, (default: None)
             Start date.
                 * "17-12-1903 00:00:00" : start date
@@ -2233,14 +2547,15 @@
             * unsplash
             * cancer
             * breast_cancer
             * iris
             * occupancy
             * climate
             * "mnist"
+            * "animals"
     n : int, (default: 1000).
         Number of events (samples).
     c : int, (default: 100).
         Number of classes.
     date_start : str, (default: None)
         Start date.
             * "17-12-1903 00:00:00" : start date
@@ -2307,14 +2622,22 @@
         url='https://erdogant.github.io/datasets/UCI_Occupancy_Detection.zip'
         sep=','
     elif data=='climate':
         url='https://erdogant.github.io/datasets/kaggle_daily_delhi_climate_test.zip'
     elif data=='mnist':
         url='https://erdogant.github.io/datasets/mnist.zip'
         sep=';'
+    elif data=='animals':
+        # example data with three levels and a single value field
+        data = {'group1': ['Animal', 'Animal', 'Animal', 'Plant', 'Animal'],
+                'group2': ['Mammal', 'Mammal', 'Fish', 'Tree', 'Fish'],
+                'group3': ['Fox',    'Lion',   'Cod',  'Oak',  'Ape'],
+                'weight': [35000, 25000, 10000, 1500, 1750]}
+        df = pd.DataFrame.from_dict(data)
+        return df
 
     if url is None:
         logger.info('Nothing to download.')
         return None
 
     curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     filename = os.path.basename(urlparse(url).path)
@@ -2342,16 +2665,16 @@
         df = pd.read_csv(csvfile)
         df.rename(columns={'value': 'weight'}, inplace=True)
         df[['source', 'target']] = df[['source', 'target']].astype(str)
     elif data=='stormofswords':
         df = pd.read_csv(csvfile)
         # df.rename(columns={'weight':'value'}, inplace=True)
     elif data=='southern_nebula':
-        img_before = os.path.join(os.path.split(csvfile)[0], 'southern_nebula_before.jpg')
-        img_after = os.path.join(os.path.split(csvfile)[0], 'southern_nebula_after.jpg')
+        img_before = os.path.join(os.path.split(csvfile)[0], 'southern_nebula', 'southern_nebula_before.jpg')
+        img_after = os.path.join(os.path.split(csvfile)[0], 'southern_nebula', 'southern_nebula_after.jpg')
         return img_before, img_after
     elif data=='cancer':
         df = pd.read_csv(PATH_TO_DATA, sep=',')
         df.rename(columns={'tsneX': 'x', 'tsneY': 'y', 'labx': 'labels'}, inplace=True)
         df.set_index(df['labels'], inplace=True)
     else:
         df = pd.read_csv(PATH_TO_DATA, sep=sep)
@@ -2434,18 +2757,59 @@
     else:
         logger.warning('Input is not a zip file: [%s]', path_to_zip)
     # Return
     return getpath
 
 
 # %%
-def set_logger(verbose=20):
-    """Set the logger for verbosity messages."""
-    logger.setLevel(verbose)
+def set_logger(verbose: [str, int] = 'info'):
+    """Set the logger for verbosity messages.
 
+    Parameters
+    ----------
+    verbose : [str, int], default is 'info' or 20
+        Set the verbose messages using string or integer values.
+            * 0, 60, None, 'silent', 'off', 'no']: No message.
+            * 10, 'debug': Messages from debug level and higher.
+            * 20, 'info': Messages from info level and higher.
+            * 30, 'warning': Messages from warning level and higher.
+            * 50, 'critical': Messages from critical level and higher.
+
+    Returns
+    -------
+    None.
+
+    Examples
+    --------
+    >>> # Set the logger to warning
+    >>> set_logger(verbose='warning')
+    >>>
+    >>> # Test with different messages
+    >>> logger.debug("Hello debug")
+    >>> logger.info("Hello info")
+    >>> logger.warning("Hello warning")
+    >>> logger.critical("Hello critical")
+    >>>
+    """
+    # Set 0 and None as no messages.
+    if (verbose==0) or (verbose is None):
+        verbose=60
+    # Convert str to levels
+    if isinstance(verbose, str):
+        levels = {'silent': 60,
+                  'off': 60,
+                  'no': 60,
+                  'debug': 10,
+                  'info': 20,
+                  'warning': 30,
+                  'critical': 50}
+        verbose = levels[verbose]
+
+    # Show examples
+    logger.setLevel(verbose)
 
 # %%
 def disable_tqdm():
     """Set the logger for verbosity messages."""
     return (True if (logger.getEffectiveLevel()>=30) else False)
 
 
@@ -2458,14 +2822,14 @@
     chart function as Object.
 
     """
     # Check the presence of the chart name.
     if chart is not None:
         if logger is not None: logger.info('Initializing [%s]' %(chart))
         chart = str.capitalize(chart)
-        if np.isin(chart, ['Chord', 'Sankey', 'Timeseries', 'Violin', 'Movingbubbles', 'Scatter', 'Heatmap', 'Matrix']):
+        if np.isin(chart, ['Chord', 'Sankey', 'Timeseries', 'Violin', 'Movingbubbles', 'Scatter', 'Heatmap', 'Matrix', 'Treemap', 'Tree']):
             chart=eval(chart)
         else:
             if logger is not None: logger.info('%s is not yet implemented in such manner.' %(chart))
             chart = None
 
     return chart
```

### Comparing `d3blocks-1.2.9/d3blocks/examples.py` & `d3blocks-1.3.0/d3blocks/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,213 @@
 # %%
 # import d3blocks
 # print(dir(d3blocks))
 # print(d3blocks.__version__)
+# import pandas as pd
+# import numpy as np
+
+# df = d3.import_example('bigbang')
+# df1 = df.groupby(['source', 'target'])['weight'].sum()
+# df1 = df1.reset_index()
+
+# %% Tree with custom properties
+
+# Load library
+from d3blocks import D3Blocks
+# Initialize
+d3 = D3Blocks(verbose='info', chart='tree', frame=False)
+# Import example
+df = d3.import_example('energy')
+# Set node properties
+d3.set_node_properties(df)
+# d3.node_properties
+# Set specific properties
+d3.node_properties.get('Bio-conversion')['size'] = 30
+d3.node_properties.get('Bio-conversion')['color'] = '#000000'
+d3.node_properties.get('Bio-conversion')['tooltip'] = 'Title: P Operations<br><img src="https://source.unsplash.com/collection/385548/150x100">'
+d3.node_properties.get('Bio-conversion')['edge_color'] = '#00FFFF'
+d3.node_properties.get('Bio-conversion')['edge_size'] = 5
+d3.node_properties.get('Bio-conversion')['opacity'] = 0.4
+# Set properties for Losses
+d3.node_properties.get('Losses')['color'] = '#FF0000'
+d3.node_properties.get('Losses')['size'] = 15
+d3.node_properties.get('Losses')['tooltip'] = ''
+# Set properties for Agriculture
+d3.node_properties.get('Agriculture')['color'] = '#00FFFF'
+d3.node_properties.get('Agriculture')['size'] = 5
+d3.node_properties.get('Agriculture')['edge_color'] = '#89CFF0'
+d3.node_properties.get('Agriculture')['edge_size'] = 3
+d3.node_properties.get('Agriculture')['opacity'] = 0.7
+
+# Set edge properties
+d3.set_edge_properties(df)
+
+# Show chart
+d3.show(hierarchy=[1, 2, 3, 4, 5, 6, 7, 8], filepath=r'c:\temp\tree.html')
+
+# %% Tree with defaults
+# Import library
+from d3blocks import D3Blocks
+# Initialize
+d3 = D3Blocks(verbose='info', chart='tree')
+# Import example
+df = d3.import_example('energy')
+# Create tree
+html = d3.tree(df, filepath=r'c:\temp\tree.html', hierarchy=[1, 2, 3, 4, 5, 6, 7, 8])
+
+# %% Issue
+from d3blocks import D3Blocks
+
+# Initialize
+d3 = D3Blocks()
+
+df = d3.import_example(data='energy')
+
+d3.d3graph(df, filepath='d3graph.html', showfig=False)
+
+# Set edge properties
+d3.D3graph.set_edge_properties(minmax_distance=[50, 100])
+d3.D3graph.set_node_properties(color='cluster')
+
+# Plot
+d3.D3graph.show()
+
+# %%
+import pypickle
+import pandas as pd
+df = pypickle.load(r'D:/REPOS/aeroplus/aeroplus/data/maintenance.pkl')
+df.columns.values[0] = df.columns[0].replace('\xa0', ' ')
+df.rename(columns={'Date': 'datetime', 'Reported by': 'sample_id', 'Aircraft': 'state'}, inplace=True)
+
+df['state']
+df['number'] = df['state'].str.extract(r'^(\d+)')
+df['state'] = df['state'].str.replace(r'^\d+\s+', '', regex=True)
+df['datetime'] = pd.to_datetime(df['datetime'])
+
+df.drop(labels=['Note', '', 'number', 'Status'], axis=1, inplace=True)
+# print(df)
+
+
+from d3blocks import D3Blocks
+# Initialize
+d3 = D3Blocks(frame=False)
+# Import example
+# df = d3.import_example('random_time', n=1000, c=100, date_start="1-1-2000 00:10:05", date_stop="1-1-2000 23:59:59")
+
+# Show with size=5
+d3.movingbubbles(df, size=5, filepath='c://temp/movingbubbles.html')
+
+
+# %% d3graph
+import pandas as pd
+from d3blocks import D3Blocks
+
+# Initialize
+d3 = D3Blocks()
+
+# Load example data
+df = pd.read_csv(r'C:\temp\rules_sample_38.csv')
+df.rename(columns={'antecedents': 'source', 'consequents': 'target', 'lift': 'weight'}, inplace=True)
+
+# Set edge properties
+d3.D3graph.set_edge_properties(minmax_distance=[50, 100])
+
+# Plot
+d3.d3graph(df, filepath='c:/temp/d3graph.html')
+
+
+# %%
+# Scatter
+from d3blocks import D3Blocks
+d3 = D3Blocks()
+df = d3.import_example('cancer')
+html = d3.scatter(df['x'].values, df['y'].values, c_gradient='opaque', color=df['labels'].values, stroke='#000000')
+
+# %%
 import pandas as pd
 import numpy as np
+from d3blocks import D3Blocks
+
+# Initialize
+d3 = D3Blocks(verbose=10, support='text')
+
+# Import example
+df = d3.import_example('energy')
+html = d3.chord(df)
+
+# Import example
+df = d3.import_example('stormofswords')
+df = d3.vec2adjmat(df['source'], df['target'], weight=df['weight'], symmetric=True)
+d3.heatmap(df, classlabel='cluster', stroke='red', vmax=1)
+
+df = pd.DataFrame(np.random.randint(0, 10, size=(6, 20)))
+d3.matrix(df, cmap='interpolateGreens')
+
+df = d3.import_example('energy')
+html = d3.particles('D3blocks')
+
+df = d3.import_example(data='energy')
+d3.sankey(df, link={"color":"source-target"})
+
+df = d3.import_example('cancer')
+html = d3.scatter(df['x'].values, df['y'].values)
+
+df = d3.import_example('climate')
+html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S')
+
+df = d3.import_example('energy')
+html = d3.treemap(df)
+
+df = d3.import_example('cancer')
+html = d3.violin(x=df['labels'].values, y=df['age'].values)
+
+# %%
+# group by source and target, and count occurrences
+# counts = dfnew.groupby(['source', 'target']).count()
+# add weight column with count values
+# counts['weight'] = counts['weight']
+# reset index to make columns from groupby into columns of the dataframe
+# counts = counts.reset_index()
+
+
+# %% Treemap
+from d3blocks import D3Blocks
+# Initialize
+d3 = D3Blocks(verbose='info')
+# Import example
+# df = d3.import_example('animals')
+df = d3.import_example('energy')
+# df = d3.import_example('stormofswords')
+# df = d3.import_example('bigbang')
+# Create treemap
+html = d3.treemap(df, notebook=False, filepath=None)
+# html = d3.treemap(df, notebook=False, filepath=r'c:\temp\treemap.html', figsize=[1400, 800], font={'size':8}, border={'color': '#000000', 'width': 1})
+# html = d3.treemap(df, notebook=False, filepath=r'c:\temp\treemap.html', figsize=[None, None], font={'size':8}, border={'color': '#000000', 'width': 1})
+
+
+# %% Fontsize in violin map
+# Import example dataset
+from d3blocks import D3Blocks
+
+# Initialize
+d3 = D3Blocks()
+
+df = d3.import_example('cancer')
+
+# Create the chart
+d3.violin(x=df['labels'].values,
+          y=df['age'].values,
+          tooltip=df['labels'].values + ' <br /> Survival: ' + df['survival_months'].astype(str).values,
+          bins=50,
+          fontsize_axis=10,
+          fontsize=10,
+          size=df['survival_months'].values/10,
+          x_order=['acc','kich', 'brca','lgg','blca','coad','ov'],
+          filepath=r'c:\temp\violine.html', figsize=[900, None])
+
 
 # %% VIOLIN - EXAMPLE
 from d3blocks import D3Blocks
 
 # Initialize
 d3 = D3Blocks()
 
@@ -43,16 +243,14 @@
                         size=df['survival_months'].values/10,
                         x_order=['acc','kich', 'brca','lgg','blca','coad','ov'],
                         filepath='violine_demo.html')
 # d3.edge_properties
 d3.show(filepath='c://temp//violin1.html')
 
 
-
-
 # %%
 from d3blocks import D3Blocks
 
 # Initialize
 d3 = D3Blocks(verbose=10)
 # Import example
 df = d3.import_example('energy')
@@ -155,15 +353,15 @@
                  datetime='datetime',
                  state='state',
                  sample_id='sample_id',
                  size=size,
                  color=color,
                  color_method='node',
                  timedelta='minutes',
-                 speed={"slow": 1000, "medium": 200, "fast": 10},
+                 speed={"slow": 1000, "medium": 100, "fast": 10},
                  time_notes=time_notes,
                  filepath=r'c:\temp\movingbubbles.html',
                  cmap='Set2',
                  # standardize='minimum',
                   standardize='samplewise',
                  # standardize='relative',
                  )
@@ -285,14 +483,16 @@
 
 df1 = d3.edge_properties
 
 for i, _ in enumerate(df1.index):
     df1['sample_id'].iloc[i]
 
 # %% Matrix
+import pandas as pd
+import numpy as np
 from d3blocks import D3Blocks
 d3 = D3Blocks()
 df = pd.DataFrame(np.random.randint(0, 10, size=(6, 20)))
 d3.matrix(df, filepath='c:/temp/matrix/matrix.html', cmap='interpolateGreens')
 
 from d3blocks import D3Blocks
 d3 = D3Blocks()
@@ -303,29 +503,26 @@
 # %% Heatmap
 from d3blocks import D3Blocks
 
 # Initialize
 d3 = D3Blocks()
 # Import example
 # df = d3.import_example('bigbang')
-# df = d3.import_example('stormofswords')
-df = d3.import_example('energy')
+df = d3.import_example('stormofswords')
+# df = d3.import_example('energy')
 df = d3.vec2adjmat(df['source'], df['target'], weight=df['weight'], symmetric=True)
 
 # d3.heatmap(df, filepath='c:/temp/heatmap.html', classlabel=[1,1,1,2,2,2,3])
 d3.heatmap(df, filepath='c:/temp/heatmap.html', classlabel='cluster', stroke='red', vmax=1, figsize=(400, 400))
 html = d3.heatmap(df, filepath=None, notebook=False)
 d3.heatmap(df, notebook=True)
 
 
 # %% Notebook examples
 
-# d3graph
-# elasticgraph
-
 # Violin
 from d3blocks import D3Blocks
 d3 = D3Blocks()
 df = d3.import_example('cancer')
 html = d3.violin(x=df['labels'].values, y=df['age'].values, filepath=None, notebook=False)
 assert html is not None
 html = d3.violin(x=df['labels'].values, y=df['age'].values, filepath=None, notebook=True)
@@ -610,20 +807,22 @@
 # Initialize
 d3 = D3Blocks()
 
 # Load example data
 df = d3.import_example('energy')
 
 # Plot
-d3.d3graph(df, filepath='c:/temp/d3graph.html', showfig=True, charge=400)
+d3.d3graph(df, filepath='c:/temp/d3graph.html', showfig=True, charge=400, support=True)
 
 # Set clusters
 d3.D3graph.set_node_properties(color='cluster')
+d3.D3graph.edge_properties['UK_land_based_bioenergy', 'Bio-conversion']['label'] = 'test'
 d3.D3graph.show()
 
+
 d3.D3graph.set_node_properties(color='#000000')
 d3.D3graph.show()
 
 # %% CHORD - EXAMPLE
 from d3blocks import D3Blocks
 
 # Initialize
```

### Comparing `d3blocks-1.2.9/d3blocks/heatmap/Heatmap.py` & `d3blocks-1.3.0/d3blocks/heatmap/Heatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,16 @@
     html = html.replace('$DESCRIPTION$', str(config['description']))
     html = html.replace('$TITLE$', str(config['title']))
     html = html.replace('$WIDTH$', str(config['figsize'][0]))
     html = html.replace('$WIDTH_DROPDOWN$', str(int(config['figsize'][0] + 200)))
     html = html.replace('$HEIGHT$', str(config['figsize'][1]))
     html = html.replace('$STROKE$', str(config['stroke']))
     html = html.replace('$DATA_PATH$', filename)
+    html = html.replace('$SUPPORT$', config['support'])
+
     html = html.replace('$DATA_COMES_HERE$', json_data)
 
     # Write to html
     write_html_file(config, html, logger)
     # Return html
     return html
```

### Comparing `d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js` & `d3blocks-1.3.0/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.v4.js` & `d3blocks-1.3.0/d3blocks/heatmap/d3js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/heatmap/d3js/heatmap.html.j2` & `d3blocks-1.3.0/d3blocks/heatmap/d3js/heatmap.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <!--
     Thank you for inspecting this page! If you find some issues, let me know!
     Library     : pip install d3blocks
     Github      : https://d3blocks.github.io/d3blocks/pages/html/Heatmap.html
 	References  : d3-graph-gallery.com
  -->
 
+$SUPPORT$
+
 <!DOCTYPE html>
 <html class="d3heatmap">
 <meta charset="utf-8">
 <title>"$TITLE$"</title>
 <style>
 
 
@@ -411,7 +413,9 @@
   }, 5000);
 
 //});
 
 </script>
 
 <p>$DESCRIPTION$
+
+
```

### Comparing `d3blocks-1.2.9/d3blocks/heatmap/d3js/matrix.html.j2` & `d3blocks-1.3.0/d3blocks/heatmap/d3js/matrix.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     Library     : pip install d3blocks
     Author      : E.Taskesen
     Mail        : erdogant@gmail.com
     Github      : https://github.com/d3blocks/d3blocks
 	References  : d3-graph-gallery.com
  -->
 
+$SUPPORT$
+
+
 <!DOCTYPE html>
 <meta charset="utf-8">
 
 <!-- Load d3.js -->
 <script src="d3.v4.js"></script>
 <!-- {% include "d3.v4.js" %} -->
 
@@ -146,8 +149,8 @@
         .attr("text-anchor", "left")
         .style("font-size", "14px")
         .style("fill", "grey")
         .style("max-width", 400)
         .text("$DESCRIPTION$");
 
 
-</script>
+</script>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
+ $SUPPORT$
```

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/Imageslider.py` & `d3blocks-1.3.0/d3blocks/imageslider/Imageslider.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/d3js/imageslider.html.j2` & `d3blocks-1.3.0/d3blocks/imageslider/d3js/imageslider.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/d3js/jquery-2.1.1.js` & `d3blocks-1.3.0/d3blocks/imageslider/d3js/jquery-2.1.1.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/d3js/main.js` & `d3blocks-1.3.0/d3blocks/imageslider/d3js/main.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/d3js/modernizr.js` & `d3blocks-1.3.0/d3blocks/imageslider/d3js/modernizr.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/d3js/reset.css` & `d3blocks-1.3.0/d3blocks/imageslider/d3js/reset.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/imageslider/d3js/style.css` & `d3blocks-1.3.0/d3blocks/imageslider/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/matrix/Matrix.py` & `d3blocks-1.3.0/d3blocks/matrix/Matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,15 @@
     html = html.replace('$VMAX$', str(config['vmax']))
     html = html.replace('$FONTSIZE_X$', str(fontsize_x))
     html = html.replace('$FONTSIZE_Y$', str(fontsize_y))
     html = html.replace('$STROKE$', str(config['stroke']))
     html = html.replace('$CMAP$', str(config['cmap']))
     html = html.replace('$CMAP_TYPE$', str(config['cmap_type']))
     html = html.replace('$DATA_PATH$', filename)
+    html = html.replace('$SUPPORT$', config['support'])
     html = html.replace('$DATA_COMES_HERE$', json_data)
     # html = html.replace('src="d3.v4.js"', d3_library)
     # html = html.replace('src="d3.scale.chromatic.v1.min.js"', d3_chromatic)
 
     # content = {
     #     'DESCRIPTION': str(config['description']),
     #     'TITLE': str(config['title']),
```

### Comparing `d3blocks-1.2.9/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js` & `d3blocks-1.3.0/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/matrix/d3js/d3.v4.js` & `d3blocks-1.3.0/d3blocks/matrix/d3js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2` & `d3blocks-1.3.0/d3blocks/matrix/d3js/matrix.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
     Library     : pip install d3blocks
     Author      : E.Taskesen
     Mail        : erdogant@gmail.com
     Github      : https://github.com/d3blocks/d3blocks
 	References  : d3-graph-gallery.com
  -->
 
+$SUPPORT$
+
 <!DOCTYPE html>
 <meta charset="utf-8">
 
 <!-- Load d3.js -->
 <script src="d3.v4.js"></script>
 <!-- Load color palettes -->
 <script src="d3.scale.chromatic.v1.min.js"></script>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-
+ $SUPPORT$
```

### Comparing `d3blocks-1.2.9/d3blocks/movingbubbles/Movingbubbles.py` & `d3blocks-1.3.0/d3blocks/movingbubbles/Movingbubbles.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,14 +359,17 @@
         'SPEED': config['speed'],
         'DAMPER': config['damper'],
         'NOTE': config['note'],
         'TIME_NOTES': config['time_notes'],
         'COLOR_METHOD': config['color_method'],
         'START_HOUR_MIN': config['start_hour'] + (config['start_minute'] / 60),
         'START_TIME': zero_to_hour + str(config['start_hour']) + ":" + zero_to_min + str(config['start_minute']),
+
+        'SUPPORT': config['support'],
+
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.movingbubbles', package_path='d3js'))
 
@@ -406,15 +409,15 @@
     """
     # Use copy of dataframe
     df = df.copy()
     # Get unique
     uis = df[sample_id].unique()
 
     # Check datetime format
-    if not isinstance(df[datetime][0], dt.date):
+    if not isinstance(df[datetime].iloc[0], dt.date):
         if logger is not None: logger.info('Set datetime format to [%s]' %(dt_format))
         df[datetime] = pd.to_datetime(df[datetime], format=dt_format)
 
     # Initialize empty delta
     df['delta'] = df[datetime] - df[datetime]
     # Initialize empty datetime_norm
     # df['datetime_norm'] = df[datetime] - df[datetime]
```

### Comparing `d3blocks-1.2.9/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js` & `d3blocks-1.3.0/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/movingbubbles/d3js/movingbubbles.html.j2` & `d3blocks-1.3.0/d3blocks/movingbubbles/d3js/movingbubbles.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 Licensed    : GPL3
 -->
 
 <!DOCTYPE html>
 <head>
 <title>{{ TITLE }}</title>
 
+{{ SUPPORT }}
+
 <style>
 {% include "style.css" %}
     body { font-size: {{ FONTSIZE }}; }
 .node { stroke-width: 1.5px; }
 
 </style>
 </head>
@@ -50,15 +52,14 @@
     	  <option value="NODE" {{ COLOR_NODE_SELECTED }}>Sample id</option>
     </select>
     
     <div class="clr"></div>
     </div>
 
 
-
 <script>
 
     {% include "d3-3-5-5.min.js" %}
 
 var USER_SPEED = "slow";
 
 var width = {{ WIDTH }},
@@ -438,8 +439,8 @@
 //	
 //	return hh + ":" + mm + ampm
 //}
 
 			
 
 
-</script>
+</script>
```

### Comparing `d3blocks-1.2.9/d3blocks/movingbubbles/d3js/style.css` & `d3blocks-1.3.0/d3blocks/movingbubbles/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/particles/Particles.py` & `d3blocks-1.3.0/d3blocks/particles/Particles.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,33 +13,14 @@
 import time
 try:
     from .. utils import set_path, write_html_file
 except:
     from utils import set_path, write_html_file
 
 
-# %% Set configuration properties
-# def set_config(config, logger=None):
-#     """Set the general configuration setting."""
-#     config['chart'] ='Particles'
-#     config['title']='Particles - D3blocks'
-#     config['filepath']=set_path('particles.html')
-#     config['figsize']=[900, 200]
-#     config['showfig']=True
-#     config['overwrite']=True
-#     config['fontsize'] = '"' + str(180) + 'px"'
-#     config['radius']=3
-#     config['collision']=0.5
-#     config['spacing']=8
-#     config['cmap']='Turbo'
-#     config['background']='#000000'
-#     config['notebook'] = False
-#     return config
-
-
 def show(text, config, logger):
     """Build and show the graph.
 
     Parameters
     ----------
     text : string
         String to be visualized
@@ -78,14 +59,15 @@
         'HEIGHT': config['figsize'][1],
         'COLOR_BACKGROUND': config['color_background'],
         'RADIUS': config['radius'],
         'COLLISION': config['collision'],
         'FONTSIZE': config['fontsize'],
         'SPACING': config['spacing'],
         'CMAP': config['cmap'],
+        'SUPPORT': config['support'],
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.particles', package_path='d3js'))
```

### Comparing `d3blocks-1.2.9/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js` & `d3blocks-1.3.0/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/particles/d3js/d3.v4.min.js` & `d3blocks-1.3.0/d3blocks/particles/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/particles/d3js/particles.html.j2` & `d3blocks-1.3.0/d3blocks/particles/d3js/particles.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 <!doctype html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <title>{{ TITLE }}</title>
 
+    {{ SUPPORT }}
+
     <style>
       body { background: {{ COLOR_BACKGROUND }} }
       circle.mouse { fill: none; }
     </style>
 
 </head>
 <body>
```

### Comparing `d3blocks-1.2.9/d3blocks/sankey/Sankey.py` & `d3blocks-1.3.0/d3blocks/sankey/Sankey.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,16 @@
         'marginRight': config['margin']['right'],
         'marginBottom': config['margin']['bottom'],
         'marginLeft': config['margin']['left'],
         'node_align': config['node']['align'],
         'node_width': config['node']['width'],
         'node_padding': config['node']['padding'],
         'node_stroke_color': config['node']['color'],
+
+        'SUPPORT': config['support'],
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.sankey', package_path='d3js'))
```

### Comparing `d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.html.j2` & `d3blocks-1.3.0/d3blocks/sankey/d3js/sankey.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 -->
 
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <title>{{ TITLE }}</title>
+
+    {{ SUPPORT }}
+
 </head>
 <body>
 
     <form>
         <b>Link-color:</b>
     	<select id="linkColorOptions" onchange="link_color_changed(this.value)">
     	  <option value="source" {{ link_color_select_source }}>Source</option>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 
+{{ SUPPORT }}
 { link_color_select_source }}>Source
 { link_color_select_target }}>Target
 { link_color_select_source_target }}>Source-Target
 Static color
 { align_select_left }}>Left
 { align_select_right }}>Right
 { align_select_justify }}>Justify
```

### Comparing `d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.js` & `d3blocks-1.3.0/d3blocks/sankey/d3js/sankey.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/scatter/Scatter.py` & `d3blocks-1.3.0/d3blocks/scatter/Scatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import numpy as np
 from jinja2 import Environment, PackageLoader
 from pathlib import Path
 import os
 import time
 
 try:
-    from .. utils import set_colors, convert_dataframe_dict, set_path, update_config, write_html_file
+    from .. utils import set_colors, convert_dataframe_dict, set_path, update_config, write_html_file, jitter_func
 except:
-    from utils import set_colors, convert_dataframe_dict, set_path, update_config, write_html_file
+    from utils import set_colors, convert_dataframe_dict, set_path, update_config, write_html_file, jitter_func
 
 
 # %% Set configuration properties
 def set_config(config={}, **kwargs):
     """Set the default configuration setting."""
     logger = kwargs.get('logger', None)
     config['chart'] ='Scatter'
@@ -35,14 +35,15 @@
     config['scale'] = kwargs.get('scale', False)
     config['ylim'] = kwargs.get('ylim', [None, None])
     config['xlim'] = kwargs.get('xlim', [None, None])
     config['label_radio'] = kwargs.get('label_radio', ['(x, y)', '(x1, y1)', '(x2, y2)'])
     config['color_background'] = kwargs.get('color_background', '#ffffff')
     config['reset_properties'] = kwargs.get('reset_properties', True)
     config['notebook'] = kwargs.get('notebook', False)
+    config['jitter'] = kwargs.get('jitter', None)
     # Return
     return config
 
 
 # %% Preprocessing
 def check_exceptions(x, y, x1, y1, x2, y2, size, color, tooltip, logger):
     """Check Exceptions."""
@@ -123,14 +124,15 @@
 
     # Collect key-word arguments
     x1 = kwargs.get('x1', None)
     y1 = kwargs.get('y1', None)
     x2 = kwargs.get('x2', None)
     y2 = kwargs.get('y2', None)
 
+    jitter = kwargs.get('jitter', None)
     size = kwargs.get('size', 5)
     color = kwargs.get('color', '#69b3a2')
     stroke = kwargs.get('stroke', '#000000')
     c_gradient = kwargs.get('c_gradient', None)
     tooltip = kwargs.get('tooltip', None)
     opacity = kwargs.get('opacity', 0.8)
     cmap = kwargs.get('cmap', 'tab20')
@@ -145,37 +147,67 @@
     # if (y2 is None): y2 = y
 
     if (x1 is None): x1 = np.zeros_like(x) * np.nan
     if (y1 is None): y1 = np.zeros_like(x) * np.nan
     if (x2 is None): x2 = np.zeros_like(x) * np.nan
     if (y2 is None): y2 = np.zeros_like(x) * np.nan
 
+    # Add jitter
+    x = jitter_func(x, jitter=jitter)
+    y = jitter_func(y, jitter=jitter)
+    x1 = jitter_func(x1, jitter=jitter)
+    y1 = jitter_func(y1, jitter=jitter)
+    x2 = jitter_func(x2, jitter=jitter)
+    y2 = jitter_func(y2, jitter=jitter)
+
+    # if jitter is None or jitter is False: jitter=0
+    # if jitter is True: jitter=0.01
+    # if jitter>0:
+    #     if logger is not None: logger.info('Add jitter [%g] to xy-coordinates.' %(jitter))
+    #     x = x + np.random.normal(0, jitter, size=len(x))
+    #     if y is not None: y = y + np.random.normal(0, jitter, size=len(y))
+    #     if x1 is not None: x1 = x1 + np.random.normal(0, jitter, size=len(x1))
+    #     if x2 is not None: x2 = x2 + np.random.normal(0, jitter, size=len(x2))
+    #     if y1 is not None: y1 = y1 + np.random.normal(0, jitter, size=len(y1))
+    #     if y2 is not None: y2 = y2 + np.random.normal(0, jitter, size=len(y2))
+
     # Combine into array
     X = np.c_[x, y]
     # Combine second coordinates into array
     X1 = np.c_[x1, y1]
     X2 = np.c_[x2, y2]
 
     # Scale data
     if scale:
         if logger is not None: logger.info('Scaling xy-coordinates.')
         X = _scale_xy(X)
         X1 = _scale_xy(X1)
         X2 = _scale_xy(X2)
+
     # In case only one (s)ize is defined. Set all points to this size.
     if isinstance(size, (int, float)): size = np.repeat(size, X.shape[0])
     if np.any(size<0):
         if logger is not None: logger.info('[%.0d] sizes are <0 and set to 0.' %(np.sum(size<0)))
         size[size<0]=0
+
     # In case None tooltip is defined. Set all points to this tooltip.
     if tooltip is None: tooltip = np.repeat('', X.shape[0])
+
+    # Set colors
+    color, labels = set_colors(X, color, cmap, c_gradient=c_gradient)
+
     # In case only one opacity is defined. Set all points to this size.
     if isinstance(opacity, (int, float)): opacity = np.repeat(opacity, X.shape[0])
-    # colors
-    color, labels = set_colors(X, color, cmap, c_gradient=c_gradient)
+    if (c_gradient is not None):
+        if logger is not None: logger.info('Set opacity based on the data density.')
+        import colourmap
+        c_rgb = colourmap.gradient_on_density_color(X, colourmap.hex2rgb(color), labels, opaque_type='per_class')
+        opacity = c_rgb[:, 3]
+        # c_hex = c_rgb[:, 0:3]
+
     # In case stroke is None: use same colors as for c.
     if stroke is None:
         stroke = color
     elif isinstance(stroke, str):
         # In case only one stroke is defined. Set all points to this size.
         stroke = np.repeat(stroke, X.shape[0])
 
@@ -323,14 +355,15 @@
         'RADIO_LABEL3': config['label_radio'][2],
         'RADIO_VISIBLE1': config['radio_button_visible'][0],
         'RADIO_VISIBLE2': config['radio_button_visible'][1],
         'RADIO_VISIBLE3': config['radio_button_visible'][2],
         'MOUSEOVER': config['mouseover'],
         'MOUSEMOVE': config['mousemove'],
         'MOUSELEAVE': config['mouseleave'],
+        'SUPPORT': config['support'],
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.scatter', package_path='d3js'))
```

### Comparing `d3blocks-1.2.9/d3blocks/scatter/d3js/d3.v4.min.js` & `d3blocks-1.3.0/d3blocks/scatter/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/scatter/d3js/scatter.html.j2` & `d3blocks-1.3.0/d3blocks/scatter/d3js/scatter.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 Mail        : erdogant@gmail.com
 Github      : https://github.com/d3blocks/d3blocks
 License     : GPL3
 -->
 
 <!doctype html>
 <html lang="en">
-<svg width="{{ WIDTH }}" height="{{ HEIGHT }}"></svg>
 <head>
     <meta charset="UTF-8">
     <title>{{ TITLE }}</title>
 
+    {{ SUPPORT }}
+
     <style>
       body { background: {{ COLOR_BACKGROUND }} }
     </style>
 
 </head>
 <body>
 
+<svg width="{{ WIDTH }}" height="{{ HEIGHT }}"></svg>
+
 <script>
 	{% include "d3.v4.min.js" %}
 </script>
 
 
 <form>
 	<input type="radio" name="radio_states" value="radiobutton1" style="{{ RADIO_VISIBLE1 }}" checked="checked"> <label> {{ RADIO_LABEL1 }} </label>
```

#### html2text {}

```diff
@@ -1,2 +1,3 @@
 
+{{ SUPPORT }}
 #  {{ RADIO_LABEL1 }}  o  {{ RADIO_LABEL2 }}  o  {{ RADIO_LABEL3 }}
```

### Comparing `d3blocks-1.2.9/d3blocks/tests/test_d3blocks.py` & `d3blocks-1.3.0/d3blocks/tests/test_d3blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 import pandas as pd
 import numpy as np
 try:
     import cv2
 except:
     raise ImportError('cv2 must be installed manually. Try to: <pip install opencv-python>')
 
-
-        
-
 class Testd3blocks(unittest.TestCase):
 
     def test_instantiate_d3blocks_no_args(self) -> None:
         """Test instantiation works with defaults"""
         # Initialize
         d3 = D3Blocks()
         assert isinstance(d3, type(D3Blocks()))
@@ -146,19 +143,19 @@
         # Import climate dataset
         df = d3.import_example('climate')
         # Create the timeseries chart.
         d3.timeseries(df, datetime='date', fontsize=10, dt_format='%Y-%m-%d')
 
         d3 = D3Blocks()
         df = d3.import_example('climate')
-        html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S', filepath=None, notebook=False)
+        html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d', filepath=None, notebook=False)
         assert html is not None
-        html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S', filepath=None, notebook=True)
+        html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d', filepath=None, notebook=True)
         assert html is None
-        html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S', filepath='./test.html', notebook=False)
+        html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d', filepath='./test.html', notebook=False)
         assert html is None
         
 
     def test_imageslider(self):
         # Initialize
         d3 = D3Blocks()
         # Import example
@@ -264,15 +261,89 @@
         df = d3.import_example('energy')
         html = d3.particles('D3blocks', filepath=None, notebook=False)
         assert html is not None
         html = d3.particles('D3blocks', filepath=None, notebook=True)
         assert html is None
         html = d3.particles('D3blocks', filepath='test.html', notebook=False)
         assert html is None
-        
+
+    def test_treemap(self):
+        # Load d3blocks
+        from d3blocks import D3Blocks
+        # Initialize
+        d3 = D3Blocks()
+        # Load example data
+        df = d3.import_example('energy')
+        # df = d3.import_example('animals')
+        # Plot
+        d3.treemap(df)
+
+        # Load d3blocks
+        from d3blocks import D3Blocks
+        # Initialize
+        d3 = D3Blocks(chart='Treemap', frame=True)
+        # Import example
+        df = d3.import_example('energy')
+        # Node properties
+        d3.set_node_properties(df)
+        d3.set_edge_properties(df)
+        # Show the chart
+        d3.show()
+
+    def test_tree(self):
+        # Load d3blocks
+        from d3blocks import D3Blocks
+        # Initialize
+        d3 = D3Blocks()
+        # Load example data
+        df = d3.import_example('energy')
+        # Plot
+        d3.tree(df)
+
+        # Load library
+        from d3blocks import D3Blocks
+        # Initialize
+        d3 = D3Blocks(verbose='info', chart='tree', frame=False)
+        # Import example
+        df = d3.import_example('energy')
+        # Set node properties
+        d3.set_node_properties(df)
+        # Set specific properties
+        d3.node_properties.get('Bio-conversion')['size'] = 30
+        d3.node_properties.get('Bio-conversion')['color'] = '#000000'
+        d3.node_properties.get('Bio-conversion')['tooltip'] = 'Title: P Operations<br><img src="https://source.unsplash.com/collection/385548/150x100">'
+        d3.node_properties.get('Bio-conversion')['edge_color'] = '#00FFFF'
+        d3.node_properties.get('Bio-conversion')['edge_size'] = 5
+        d3.node_properties.get('Bio-conversion')['opacity'] = 0.4
+        # Set properties for Losses
+        d3.node_properties.get('Losses')['color'] = '#FF0000'
+        d3.node_properties.get('Losses')['size'] = 15
+        d3.node_properties.get('Losses')['tooltip'] = ''
+        # Set properties for Agriculture
+        d3.node_properties.get('Agriculture')['color'] = '#00FFFF'
+        d3.node_properties.get('Agriculture')['size'] = 5
+        d3.node_properties.get('Agriculture')['edge_color'] = '#89CFF0'
+        d3.node_properties.get('Agriculture')['edge_size'] = 3
+        d3.node_properties.get('Agriculture')['opacity'] = 0.7
+        # Set edge properties
+        d3.set_edge_properties(df)
+        # Show chart
+        d3.show(hierarchy=[1, 2, 3, 4, 5, 6, 7, 8], filepath=r'c:\temp\tree.html')
+
+        # Load d3blocks
+        from d3blocks import D3Blocks
+        # Initialize
+        d3 = D3Blocks(chart='tree', frame=True)
+        # Import example
+        df = d3.import_example('energy')
+        # Node properties
+        d3.set_node_properties(df)
+        d3.set_edge_properties(df)
+        # Show the chart
+        d3.show()
 
     def test_movingbubbles(self):
         # Set color scheme
         d3 = D3Blocks()
         # Generate random data with various states
         df = d3.import_example('random_time', n=10000, c=500, date_start="1-1-2000 00:10:05", date_stop="1-1-2001 23:59:59")
         # Make the moving bubbles chart.
@@ -282,102 +353,117 @@
         df = d3.import_example('random_time', n=10000, c=300, date_start="1-1-2000 00:10:05", date_stop="1-1-2000 23:59:59")
         html = d3.movingbubbles(df, speed={"slow": 1000, "medium": 200, "fast": 10}, filepath=None, notebook=False)
         assert html is not None
         html = d3.movingbubbles(df, speed={"slow": 1000, "medium": 200, "fast": 10}, filepath=None, notebook=True)
         assert html is None
         html = d3.movingbubbles(df, speed={"slow": 1000, "medium": 200, "fast": 10}, filepath='test.html', notebook=False)
         assert html is None
-        
 
     def test_html(self):
         # Violin
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('cancer')
         html = d3.violin(x=df['labels'].values, y=df['age'].values, filepath=None, notebook=False)
         assert html is not None
         html = d3.violin(x=df['labels'].values, y=df['age'].values, filepath=None, notebook=True)
         assert html is None
         html = d3.violin(x=df['labels'].values, y=df['age'].values, filepath='./test.html', notebook=False, showfig=False)
         assert html is None
-        
-        
+
         # Timeseries
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('climate')
         html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S', filepath=None, notebook=False)
         assert html is not None
         html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S', filepath=None, notebook=True)
         assert html is None
         html = d3.timeseries(df, datetime='date', dt_format='%Y-%m-%d %H:%M:%S', filepath='./test.html', notebook=False, showfig=False)
         assert html is None
-        
+
         # Scatter
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('cancer')
         html = d3.scatter(df['x'].values, df['y'].values, filepath=None, notebook=False)
         assert html is not None
         html = d3.scatter(df['x'].values, df['y'].values, filepath=None, notebook=True)
         assert html is None
         html = d3.scatter(df['x'].values, df['y'].values, filepath='./test.html', notebook=False, showfig=False)
         assert html is None
-        
+
         # Sankey
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('energy')
         html = d3.sankey(df, filepath=None, notebook=False)
         assert html is not None
         html = d3.sankey(df, filepath=None, notebook=True)
         assert html is None
         html = d3.sankey(df, filepath='./test.html', notebook=False, showfig=False)
         assert html is None
-        
-        
+
         # Particles
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('energy')
         html = d3.particles('D3blocks', filepath=None, notebook=False)
         assert html is not None
         html = d3.particles('D3blocks', filepath=None, notebook=True)
         assert html is None
         html = d3.particles('D3blocks', filepath='test.html', notebook=False, showfig=False)
         assert html is None
-        
-        
+
         # Movingbubbles
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('random_time', n=10000, c=100, date_start="1-1-2000 00:10:05", date_stop="1-1-2000 23:59:59")
         html = d3.movingbubbles(df, speed={"slow": 1000, "medium": 200, "fast": 10}, filepath=None, notebook=False)
         assert html is not None
         html = d3.movingbubbles(df, speed={"slow": 1000, "medium": 200, "fast": 10}, filepath=None, notebook=True)
         assert html is None
         html = d3.movingbubbles(df, speed={"slow": 1000, "medium": 200, "fast": 10}, filepath='test.html', notebook=False, showfig=False)
         assert html is None
-        
-        
-        # Imageslider
+
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         img_before, img_after = d3.import_example('southern_nebula_internet')
         html = d3.imageslider(img_before, img_after, filepath=None, notebook=False)
         assert html is not None
         html = d3.imageslider(img_before, img_after, filepath=None, notebook=True)
         assert html is None
         html = d3.imageslider(img_before, img_after, filepath='test.html', notebook=False, showfig=False)
         assert html is None
-        
+
         # Chord
         from d3blocks import D3Blocks
         d3 = D3Blocks()
         df = d3.import_example('energy')
         html = d3.chord(df, filepath=None, notebook=False)
         assert html is not None
         html = d3.chord(df, filepath=None, notebook=True)
         assert html is None
         html = d3.chord(df, filepath='test.html', notebook=False, showfig=False)
         assert html is None
-        
+
+        # treemap
+        from d3blocks import D3Blocks
+        d3 = D3Blocks()
+        df = d3.import_example('energy')
+        html = d3.treemap(df, filepath=None, notebook=False)
+        assert html is not None
+        html = d3.treemap(df, filepath=None, notebook=True)
+        assert html is None
+        html = d3.treemap(df, filepath='test.html', notebook=False, showfig=False)
+        assert html is None
+
+        # Tree
+        from d3blocks import D3Blocks
+        d3 = D3Blocks()
+        df = d3.import_example('energy')
+        html = d3.tree(df, filepath=None, notebook=False)
+        assert html is not None
+        html = d3.tree(df, filepath=None, notebook=True)
+        assert html is None
+        html = d3.tree(df, filepath='test.html', notebook=False, showfig=False)
+        assert html is None
```

### Comparing `d3blocks-1.2.9/d3blocks/timeseries/Timeseries.py` & `d3blocks-1.3.0/d3blocks/timeseries/Timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
         'json_data': X,
         'COLOR': config['color'],
         'TITLE': config['title'],
         'FONTSIZE': str(config['fontsize']) + 'px',
         'DT_FORMAT': config['dt_format_js'],
         'WIDTH': config['figsize'][0],
         'HEIGHT': config['figsize'][1],
+        'SUPPORT': config['support'],
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.timeseries', package_path='d3js'))
```

### Comparing `d3blocks-1.2.9/d3blocks/timeseries/d3js/d3.v3.js` & `d3blocks-1.3.0/d3blocks/timeseries/d3js/d3.v3.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/timeseries/d3js/script.js` & `d3blocks-1.3.0/d3blocks/timeseries/d3js/script.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/timeseries/d3js/style.css` & `d3blocks-1.3.0/d3blocks/timeseries/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/timeseries/d3js/timeseries.html.j2` & `d3blocks-1.3.0/d3blocks/timeseries/d3js/timeseries.html.j2`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 -->
 
 <!DOCTYPE html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <title>{{ TITLE }}</title>
+{{ SUPPORT }}
+
 <style>
     {% include "style.css" %}
 
     body {
       font: {{ FONTSIZE }} sans-serif;
     }
+
 </style>
 </head>
 <body>
 
 <script>
 {% include "d3.v3.js" %}
 {% include "script.js" %}
```

#### html2text {}

```diff
@@ -1 +1,2 @@
 
+{{ SUPPORT }}
```

### Comparing `d3blocks-1.2.9/d3blocks/violin/Violin.py` & `d3blocks-1.3.0/d3blocks/violin/Violin.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     config['fontsize'] = kwargs.get('fontsize', 12)
     config['bins'] = kwargs.get('bins', 20)
     config['cmap'] = kwargs.get('cmap', 'inferno')
     config['ylim'] = kwargs.get('ylim', [None, None])
     config['x_order'] = kwargs.get('x_order', None)
     config['reset_properties'] = kwargs.get('reset_properties', True)
     config['notebook'] = kwargs.get('notebook', False)
+    config['fontsize_axis'] = '"' + str(kwargs.get('fontsize_axis', 12)) + 'px"'
+
     # Return
     return config
 
 
 # %% Get unique labels
 def set_labels(labels, logger=None):
     """Set unique labels."""
@@ -253,19 +255,21 @@
         'TITLE': config['title'],
         'WIDTH': config['figsize'][0],
         'HEIGHT': config['figsize'][1],
         'MIN_Y': config['ylim'][0],
         'MAX_Y': config['ylim'][1],
         'X_ORDER': config['x_order'],
         'BINS': config['bins'],
+        'FONTSIZE_AXIS': config['fontsize_axis'],
         'WIDTH_FIG': config['figsize'][0],
         'HEIGHT_FIG': config['figsize'][1],
         'MOUSEOVER': config['mouseover'],
         'MOUSEMOVE': config['mousemove'],
         'MOUSELEAVE': config['mouseleave'],
+        'SUPPORT': config['support'],
     }
 
     try:
         jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
     except:
         jinja_env = Environment(loader=PackageLoader(package_name='d3blocks.violin', package_path='d3js'))
```

### Comparing `d3blocks-1.2.9/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js` & `d3blocks-1.3.0/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/violin/d3js/d3.v4.min.js` & `d3blocks-1.3.0/d3blocks/treemap/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.9/d3blocks/violin/d3js/violin.html.j2` & `d3blocks-1.3.0/d3blocks/violin/d3js/violin.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 <!DOCTYPE html>
 <html lang="en">
 <!--<svg width="900" height="600"></svg>-->
 <head>
     <meta charset="UTF-8">
     <title>{{ TITLE }}</title>
+    {{ SUPPORT }}
 </head>
 <body>
 
 <script>
 {% include "d3.v4.min.js" %}
 {% include "d3-scale-chromatic.v1.min.js" %}
 </script>
@@ -52,23 +53,26 @@
 
 window.addEventListener('DOMContentLoaded', function () {
 
     // Build and Show the Y scale
     var y = d3.scaleLinear()
       .domain([{{MIN_Y}}, {{MAX_Y}}])          // Note that here the Y scale is set manually
       .range([height, 0])
-    svg.append("g").call( d3.axisLeft(y) )
+    svg.append("g")
+      .style("font-size", {{FONTSIZE_AXIS}})
+      .call(d3.axisLeft(y))
     
     // Build and Show the X scale. It is a band scale like for a boxplot: each group has an dedicated RANGE on the axis. This range has a length of x.bandwidth
     var x = d3.scaleBand()
       .range([ 0, width ])
       .domain({{ X_ORDER }})
       .padding(0.05)     // This is important: it is the space between 2 groups. 0 means no padding. 1 is the maximum.
     svg.append("g")
       .attr("transform", "translate(0," + height + ")")
+	  .style("font-size", {{FONTSIZE_AXIS}})
       .call(d3.axisBottom(x))
     
     // Features of the histogram
     var histogram = d3.histogram()
           .domain(y.domain())
           .thresholds(y.ticks({{ BINS }}))    // Important: how many bins approx are going to be made? It is the 'resolution' of the violin plot
           .value(d => d)
```

### Comparing `d3blocks-1.2.9/d3blocks.egg-info/PKG-INFO` & `d3blocks-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: d3blocks
-Version: 1.2.9
-Summary: Python package d3blocks
-Home-page: https://github.com/d3blocks/d3blocks
-Download-URL: https://github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz
-Author: Erdogan Taskesen, Oliver Verver
-Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://d3blocks.github.io/d3blocks/pages/html/index.html">
   <img src="https://github.com/d3blocks/d3blocks/blob/main/logo.png" align="center" width="600" /> 
   </a>
 </p>
 
 
@@ -84,16 +67,16 @@
 | [Scatter](https://d3blocks.github.io/d3blocks/pages/html/Scatter.html)             | ``` d3.scatter()  ```        | [Scatter](https://towardsdatascience.com/get-the-most-out-of-your-scatterplot-by-making-it-interactive-using-d3js-19939e3b046)       |
 | [Heatmap](https://d3blocks.github.io/d3blocks/pages/html/Heatmap.html)             | ``` d3.heatmap()  ```        | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Chord diagram](https://d3blocks.github.io/d3blocks/pages/html/Chord.html)         | ``` d3.chord()  ```          | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Timeseries](https://d3blocks.github.io/d3blocks/pages/html/Timeseries.html)       | ``` d3.timeseries()  ```     | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Image slider](https://d3blocks.github.io/d3blocks/pages/html/Imageslider.html)    | ``` d3.imageslider()  ```    | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Violin plot](https://d3blocks.github.io/d3blocks/pages/html/Violin.html)          | ``` d3.violin()  ```         | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 | [Particles](https://d3blocks.github.io/d3blocks/pages/html/Particles.html)         | ``` d3.particles()  ```      | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Treemap](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html)             | ``` d3.treemap()  ```        | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Tree](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html)                | ``` d3.tree()  ```           | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
 |                                                                                    |                              |                                                                                                                                      |
 
 -------------------------------------------------------------------------
 
 #### References
 * [bl.ocks](https://bl.ocks.org/)
 * [observablehq](https://observablehq.com/top)
-
-
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: d3blocks Version: 1.2.9 Summary: Python package
-d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
-github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz Author: Erdogan Taskesen,
-Oliver Verver Author-email: erdogant@gmail.com License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved Classifier: Operating System :: OS Independent Requires-Python:
->=3 Description-Content-Type: text/markdown License-File: LICENSE
            [https://github.com/d3blocks/d3blocks/blob/main/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
 v/d3blocks)](https://pypi.org/project/d3blocks/) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-blue)](https://d3blocks.github.io/d3blocks/)
 [![LOC](https://sloc.xyz/github/d3blocks/d3blocks/?category=code)](https://
 github.com/d3blocks/d3blocks/) [![Downloads](https://static.pepy.tech/
@@ -79,10 +72,16 @@
 standalone-d3js-charts-3dda98ce97d4) | | [Violin plot](https://
 d3blocks.github.io/d3blocks/pages/html/Violin.html) | ``` d3.violin() ``` |
 [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-library-to-
 create-interactive-and-standalone-d3js-charts-3dda98ce97d4) | | [Particles]
 (https://d3blocks.github.io/d3blocks/pages/html/Particles.html) | ```
 d3.particles() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-
 python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
-| | | | -----------------------------------------------------------------------
--- #### References * [bl.ocks](https://bl.ocks.org/) * [observablehq](https://
+| [Treemap](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html) | ```
+d3.treemap() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-
+python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) |
+| [Tree](https://d3blocks.github.io/d3blocks/pages/html/Treemap.html) | ```
+d3.tree() ``` | [D3Blocks](https://towardsdatascience.com/d3blocks-the-python-
+library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4) | | | |
+| ------------------------------------------------------------------------
+- #### References * [bl.ocks](https://bl.ocks.org/) * [observablehq](https://
 observablehq.com/top)
```

### Comparing `d3blocks-1.2.9/d3blocks.egg-info/SOURCES.txt` & `d3blocks-1.3.0/d3blocks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 d3blocks/imageslider/d3js/style.css
 d3blocks/matrix/Matrix.py
 d3blocks/matrix/__init__.py
 d3blocks/matrix/d3js/__init__.py
 d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
 d3blocks/matrix/d3js/d3.v4.js
 d3blocks/matrix/d3js/matrix.html.j2
-d3blocks/matrix/d3js/matrix.html.j2.new
 d3blocks/movingbubbles/Movingbubbles.py
 d3blocks/movingbubbles/__init__.py
 d3blocks/movingbubbles/d3js/__init__.py
 d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
 d3blocks/movingbubbles/d3js/movingbubbles.html.j2
 d3blocks/movingbubbles/d3js/style.css
 d3blocks/particles/Particles.py
@@ -67,13 +66,21 @@
 d3blocks/timeseries/Timeseries.py
 d3blocks/timeseries/__init__.py
 d3blocks/timeseries/d3js/__init__.py
 d3blocks/timeseries/d3js/d3.v3.js
 d3blocks/timeseries/d3js/script.js
 d3blocks/timeseries/d3js/style.css
 d3blocks/timeseries/d3js/timeseries.html.j2
+d3blocks/tree/Tree.py
+d3blocks/tree/__init__.py
+d3blocks/tree/d3js/__init__.py
+d3blocks/treemap/Treemap.py
+d3blocks/treemap/__init__.py
+d3blocks/treemap/d3js/__init__.py
+d3blocks/treemap/d3js/d3.v4.min.js
+d3blocks/treemap/d3js/treemap.html.j2
 d3blocks/violin/Violin.py
 d3blocks/violin/__init__.py
 d3blocks/violin/d3js/__init__.py
 d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
 d3blocks/violin/d3js/d3.v4.min.js
 d3blocks/violin/d3js/violin.html.j2
```

### Comparing `d3blocks-1.2.9/setup.py` & `d3blocks-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = fh.read()
 setuptools.setup(
      install_requires=['numpy',
                        'pandas',
                        'tqdm',
                        'colourmap>=1.1.10',
                        'jinja2',
-                       'd3graph>=2.3.6',
+                       'd3graph>=2.4.6',
                        'requests',
                        'ismember>=1.0.1',
                        'scikit-learn',
                        'elasticgraph>=0.1.2',
                        ],
      python_requires='>=3',
      name='d3blocks',
```

