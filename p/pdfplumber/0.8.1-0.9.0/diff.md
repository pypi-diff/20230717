# Comparing `tmp/pdfplumber-0.8.1.tar.gz` & `tmp/pdfplumber-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfplumber-0.8.1.tar", last modified: Sat Apr  8 14:48:07 2023, max compression
+gzip compressed data, was "pdfplumber-0.9.0.tar", last modified: Thu Apr 13 12:58:39 2023, max compression
```

## Comparing `pdfplumber-0.8.1.tar` & `pdfplumber-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-08 14:48:07.309422 pdfplumber-0.8.1/
--rw-r--r--   0 jeremy     (501) staff       (20)    31383 2023-04-08 14:46:04.000000 pdfplumber-0.8.1/CHANGELOG.md
--rw-r--r--   0 jeremy     (501) staff       (20)     1086 2018-02-27 13:37:10.000000 pdfplumber-0.8.1/LICENSE.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       66 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)    34272 2023-04-08 14:48:07.309520 pdfplumber-0.8.1/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)    33595 2023-04-08 14:43:10.000000 pdfplumber-0.8.1/README.md
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-08 14:48:07.305942 pdfplumber-0.8.1/pdfplumber/
--rw-r--r--   0 jeremy     (501) staff       (20)      226 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/__init__.py
--rw-r--r--   0 jeremy     (501) staff       (20)      263 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/_typing.py
--rw-r--r--   0 jeremy     (501) staff       (20)       72 2023-04-08 14:44:15.000000 pdfplumber-0.8.1/pdfplumber/_version.py
--rw-r--r--   0 jeremy     (501) staff       (20)     2150 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/cli.py
--rw-r--r--   0 jeremy     (501) staff       (20)     5150 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/container.py
--rw-r--r--   0 jeremy     (501) staff       (20)     3501 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/convert.py
--rw-r--r--   0 jeremy     (501) staff       (20)      816 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/ctm.py
--rw-r--r--   0 jeremy     (501) staff       (20)    12207 2023-04-08 14:43:48.000000 pdfplumber-0.8.1/pdfplumber/display.py
--rw-r--r--   0 jeremy     (501) staff       (20)    15933 2023-04-08 14:43:10.000000 pdfplumber-0.8.1/pdfplumber/page.py
--rw-r--r--   0 jeremy     (501) staff       (20)     4944 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/pdf.py
--rw-r--r--   0 jeremy     (501) staff       (20)        0 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/pdfplumber/py.typed
--rw-r--r--   0 jeremy     (501) staff       (20)    23425 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/table.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-08 14:48:07.307946 pdfplumber-0.8.1/pdfplumber/utils/
--rw-r--r--   0 jeremy     (501) staff       (20)      930 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/utils/__init__.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1580 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/utils/clustering.py
--rw-r--r--   0 jeremy     (501) staff       (20)      636 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/utils/generic.py
--rw-r--r--   0 jeremy     (501) staff       (20)     8352 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/utils/geometry.py
--rw-r--r--   0 jeremy     (501) staff       (20)     2218 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/pdfplumber/utils/pdfinternals.py
--rw-r--r--   0 jeremy     (501) staff       (20)    16282 2023-04-08 14:43:10.000000 pdfplumber-0.8.1/pdfplumber/utils/text.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-08 14:48:07.307266 pdfplumber-0.8.1/pdfplumber.egg-info/
--rwxrwxrwx   0 jeremy     (501) staff       (20)    34272 2023-04-08 14:48:07.000000 pdfplumber-0.8.1/pdfplumber.egg-info/PKG-INFO
--rwxrwxrwx   0 jeremy     (501) staff       (20)     1072 2023-04-08 14:48:07.000000 pdfplumber-0.8.1/pdfplumber.egg-info/SOURCES.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)        1 2023-04-08 14:48:07.000000 pdfplumber-0.8.1/pdfplumber.egg-info/dependency_links.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)       51 2023-04-08 14:48:07.000000 pdfplumber-0.8.1/pdfplumber.egg-info/entry_points.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2022-08-05 21:05:51.000000 pdfplumber-0.8.1/pdfplumber.egg-info/not-zip-safe
--rwxrwxrwx   0 jeremy     (501) staff       (20)       47 2018-02-04 17:48:50.000000 pdfplumber-0.8.1/pdfplumber.egg-info/pbr.json
--rwxrwxrwx   0 jeremy     (501) staff       (20)       48 2023-04-08 14:48:07.000000 pdfplumber-0.8.1/pdfplumber.egg-info/requires.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)       11 2023-04-08 14:48:07.000000 pdfplumber-0.8.1/pdfplumber.egg-info/top_level.txt
--rw-r--r--   0 jeremy     (501) staff       (20)      199 2022-10-01 13:45:28.000000 pdfplumber-0.8.1/requirements-dev.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       48 2022-11-22 17:54:41.000000 pdfplumber-0.8.1/requirements.txt
--rw-r--r--   0 jeremy     (501) staff       (20)      494 2023-04-08 14:48:07.309798 pdfplumber-0.8.1/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)     1638 2022-10-01 13:45:28.000000 pdfplumber-0.8.1/setup.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-08 14:48:07.309326 pdfplumber-0.8.1/tests/
--rw-r--r--   0 jeremy     (501) staff       (20)     6654 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/tests/test_basics.py
--rw-r--r--   0 jeremy     (501) staff       (20)     3681 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/tests/test_ca_warn_report.py
--rw-r--r--   0 jeremy     (501) staff       (20)     5034 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/tests/test_convert.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1037 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/tests/test_ctm.py
--rw-r--r--   0 jeremy     (501) staff       (20)     3080 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/tests/test_dedupe_chars.py
--rw-r--r--   0 jeremy     (501) staff       (20)     3079 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/tests/test_display.py
--rw-r--r--   0 jeremy     (501) staff       (20)     7686 2023-04-08 14:43:10.000000 pdfplumber-0.8.1/tests/test_issues.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1838 2022-11-22 17:54:41.000000 pdfplumber-0.8.1/tests/test_laparams.py
--rw-r--r--   0 jeremy     (501) staff       (20)      370 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/tests/test_list_metadata.py
--rw-r--r--   0 jeremy     (501) staff       (20)     4474 2022-09-19 18:45:46.000000 pdfplumber-0.8.1/tests/test_nics_report.py
--rw-r--r--   0 jeremy     (501) staff       (20)     6740 2023-02-14 03:04:25.000000 pdfplumber-0.8.1/tests/test_table.py
--rw-r--r--   0 jeremy     (501) staff       (20)    14542 2023-04-08 14:43:10.000000 pdfplumber-0.8.1/tests/test_utils.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-13 12:58:39.780285 pdfplumber-0.9.0/
+-rw-r--r--   0 jeremy     (501) staff       (20)    33217 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/CHANGELOG.md
+-rw-r--r--   0 jeremy     (501) staff       (20)     1086 2018-02-27 13:37:10.000000 pdfplumber-0.9.0/LICENSE.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       66 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)    35678 2023-04-13 12:58:39.780443 pdfplumber-0.9.0/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)    35001 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/README.md
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-13 12:58:39.774205 pdfplumber-0.9.0/pdfplumber/
+-rw-r--r--   0 jeremy     (501) staff       (20)      226 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/pdfplumber/__init__.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      263 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/pdfplumber/_typing.py
+-rw-r--r--   0 jeremy     (501) staff       (20)       72 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/pdfplumber/_version.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     2150 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/pdfplumber/cli.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     5496 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/pdfplumber/container.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     3501 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/pdfplumber/convert.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      816 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/pdfplumber/ctm.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    12207 2023-04-13 12:10:36.000000 pdfplumber-0.9.0/pdfplumber/display.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    17356 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/pdfplumber/page.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     4944 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/pdfplumber/pdf.py
+-rw-r--r--   0 jeremy     (501) staff       (20)        0 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/pdfplumber/py.typed
+-rw-r--r--   0 jeremy     (501) staff       (20)    23425 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/pdfplumber/table.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-13 12:58:39.777026 pdfplumber-0.9.0/pdfplumber/utils/
+-rw-r--r--   0 jeremy     (501) staff       (20)      930 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/pdfplumber/utils/__init__.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1580 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/pdfplumber/utils/clustering.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      636 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/pdfplumber/utils/generic.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     8412 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/pdfplumber/utils/geometry.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     2218 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/pdfplumber/utils/pdfinternals.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    20065 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/pdfplumber/utils/text.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-13 12:58:39.776128 pdfplumber-0.9.0/pdfplumber.egg-info/
+-rwxrwxrwx   0 jeremy     (501) staff       (20)    35678 2023-04-13 12:58:39.000000 pdfplumber-0.9.0/pdfplumber.egg-info/PKG-INFO
+-rwxrwxrwx   0 jeremy     (501) staff       (20)     1072 2023-04-13 12:58:39.000000 pdfplumber-0.9.0/pdfplumber.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)        1 2023-04-13 12:58:39.000000 pdfplumber-0.9.0/pdfplumber.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       51 2023-04-13 12:58:39.000000 pdfplumber-0.9.0/pdfplumber.egg-info/entry_points.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2022-08-05 21:05:51.000000 pdfplumber-0.9.0/pdfplumber.egg-info/not-zip-safe
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       47 2018-02-04 17:48:50.000000 pdfplumber-0.9.0/pdfplumber.egg-info/pbr.json
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       48 2023-04-13 12:58:39.000000 pdfplumber-0.9.0/pdfplumber.egg-info/requires.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       11 2023-04-13 12:58:39.000000 pdfplumber-0.9.0/pdfplumber.egg-info/top_level.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      199 2022-10-01 13:45:28.000000 pdfplumber-0.9.0/requirements-dev.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       48 2022-11-22 17:54:41.000000 pdfplumber-0.9.0/requirements.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      494 2023-04-13 12:58:39.780779 pdfplumber-0.9.0/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)     1638 2022-10-01 13:45:28.000000 pdfplumber-0.9.0/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-13 12:58:39.779801 pdfplumber-0.9.0/tests/
+-rw-r--r--   0 jeremy     (501) staff       (20)     6810 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/tests/test_basics.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     3681 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/tests/test_ca_warn_report.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     5034 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/tests/test_convert.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1037 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/tests/test_ctm.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     3080 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/tests/test_dedupe_chars.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     3079 2023-02-14 03:04:25.000000 pdfplumber-0.9.0/tests/test_display.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     9265 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/tests/test_issues.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1838 2022-11-22 17:54:41.000000 pdfplumber-0.9.0/tests/test_laparams.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      370 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/tests/test_list_metadata.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     4474 2022-09-19 18:45:46.000000 pdfplumber-0.9.0/tests/test_nics_report.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     7256 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/tests/test_table.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    16403 2023-04-13 12:56:29.000000 pdfplumber-0.9.0/tests/test_utils.py
```

### Comparing `pdfplumber-0.8.1/CHANGELOG.md` & `pdfplumber-0.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. The format is based on [Keep a Changelog](http://keepachangelog.com/).
 
+## [0.9.0] - 2023-04-13
+
+### Changed
+
+- Make word segmentation (via `WordExtractor.char_begins_new_word(...)`) more explict and rigorous; should help in catching edge-cases in the future. ([6acd580](https://github.com/jsvine/pdfplumber/commit/6acd580) + [ebb93ea](https://github.com/jsvine/pdfplumber/commit/ebb93ea) + [#840](https://github.com/jsvine/pdfplumber/discussions/840#discussioncomment-5312166))
+- Use `curve_edge` objects (instead of just `line` and `rect_edge` objects) in default table-detection strategy. ([6f6b465](https://github.com/jsvine/pdfplumber/commit/6f6b465) + [#858](https://github.com/jsvine/pdfplumber/discussions/858)) 
+- By default, expand ligatures into their consituent letters (e.g., `ﬃ` to `ffi`), and add the `expand_ligatures` boolean parameter to text-extraction methods. ([86e935d](https://github.com/jsvine/pdfplumber/commit/86e935d) + [#598](https://github.com/jsvine/pdfplumber/issues/598))
+
+### Added
+
+- Add `Page.extract_text_lines(...)` method. ([4b37397](https://github.com/jsvine/pdfplumber/commit/4b37397) + [#852](https://github.com/jsvine/pdfplumber/discussions/852))
+- Add `main_group`, `return_groups`, `return_chars` parameters to `Page.search(...)`. ([4b37397](https://github.com/jsvine/pdfplumber/commit/4b37397))
+- Add `.curve_edges` property to `PDF` and `Page`. ([6f6b465](https://github.com/jsvine/pdfplumber/commit/6f6b465))
+
+### Fixed
+
+- Fix handling of bytes-typed fontnames. ([9441ff7](https://github.com/jsvine/pdfplumber/commit/9441ff7) + [#461](https://github.com/jsvine/pdfplumber/discussions/461) + [#842](https://github.com/jsvine/pdfplumber/discussions/842))
+- Fix handling of whitespace-only and empty results of `Page.search(...)`. ([6f6b465](https://github.com/jsvine/pdfplumber/commit/6f6b465) + [#853](https://github.com/jsvine/pdfplumber/discussions/853))
+
 ## [0.8.1] - 2023-04-08
 ### Fixed
 
 - Fix `x0>x1`/etc. error for when drawing rect fills, per new Pillow version ([db136b7](https://github.com/jsvine/pdfplumber/commit/db136b7))
 
 ## [0.8.0] - 2023-02-13
```

### Comparing `pdfplumber-0.8.1/LICENSE.txt` & `pdfplumber-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/PKG-INFO` & `pdfplumber-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pdfplumber
-Version: 0.8.1
-Summary: Plumb a PDF for detailed information about each char, rectangle, and line.
-Home-page: https://github.com/jsvine/pdfplumber
-Author: Jeremy Singer-Vine
-Author-email: jsvine@gmail.com
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # pdfplumber
 
 [![Version](https://img.shields.io/pypi/v/pdfplumber.svg)](https://pypi.python.org/pypi/pdfplumber) ![Tests](https://github.com/jsvine/pdfplumber/workflows/Tests/badge.svg) [![Code coverage](https://codecov.io/gh/jsvine/pdfplumber/branch/stable/graph/badge.svg)](https://codecov.io/gh/jsvine/pdfplumber/branch/stable) [![Support Python versions](https://img.shields.io/pypi/pyversions/pdfplumber.svg)](https://pypi.python.org/pypi/pdfplumber)
 
 Plumb a PDF for detailed information about each text character, rectangle, and line. Plus: Table extraction and visual debugging.
 
 Works best on machine-generated, rather than scanned, PDFs. Built on [`pdfminer.six`](https://github.com/goulu/pdfminer). 
@@ -244,15 +226,17 @@
 |`doctop`| Distance of curve's highest point from top of document.|
 |`linewidth`| Thickness of line.|
 |`fill`| Whether the shape defined by the curve's path is filled.|
 |`stroking_color`|The color of the curve's outline, expressed as a tuple or integer, depending on the “color space” used.|
 |`non_stroking_color`|The curve’s fill color.|
 |`object_type`| "curve"|
 
-Additionally, both `pdfplumber.PDF` and `pdfplumber.Page` provide access to two derived lists of objects: `.rect_edges` (which decomposes each rectangle into its four lines) and `.edges` (which combines `.rect_edges` with `.lines`). 
+#### Derived properties
+
+Additionally, both `pdfplumber.PDF` and `pdfplumber.Page` provide access to several derived lists of objects: `.rect_edges` (which decomposes each rectangle into its four lines), `.curve_edges` (which does the same for `curve` objects), and `.edges` (which combines `.rect_edges`, `.curve_edges`, and `.lines`). 
 
 #### `image` properties
 
 [To be completed.]
 
 ### Obtaining higher-level layout objects via `pdfminer.six`
 
@@ -334,18 +318,19 @@
 ## Extracting text
 
 `pdfplumber` can extract text from any given page (including cropped and derived pages). It can also attempt to preserve the layout of that text, as well as to identify the coordinates of words and search queries. `Page` objects can call the following text-extraction methods:
 
 
 | Method | Description |
 |--------|-------------|
-|`.extract_words(x_tolerance=3, y_tolerance=3, keep_blank_chars=False, use_text_flow=False, horizontal_ltr=True, vertical_ttb=True, extra_attrs=[], split_at_punctuation=False)`| Returns a list of all word-looking things and their bounding boxes. Words are considered to be sequences of characters where (for "upright" characters) the difference between the `x1` of one character and the `x0` of the next is less than or equal to `x_tolerance` *and* where the `doctop` of one character and the `doctop` of the next is less than or equal to `y_tolerance`. A similar approach is taken for non-upright characters, but instead measuring the vertical, rather than horizontal, distances between them. The parameters `horizontal_ltr` and `vertical_ttb` indicate whether the words should be read from left-to-right (for horizontal words) / top-to-bottom (for vertical words). Changing `keep_blank_chars` to `True` will mean that blank characters are treated as part of a word, not as a space between words. Changing `use_text_flow` to `True` will use the PDF's underlying flow of characters as a guide for ordering and segmenting the words, rather than presorting the characters by x/y position. (This mimics how dragging a cursor highlights text in a PDF; as with that, the order does not always appear to be logical.) Passing a list of `extra_attrs`  (e.g., `["fontname", "size"]` will restrict each words to characters that share exactly the same value for each of those [attributes](#char-properties), and the resulting word dicts will indicate those attributes. Setting `split_at_punctuation` to `True` will enforce breaking tokens at punctuations specified by `string.punctuation`; or you can specify the list of separating punctuation by pass a string, e.g., <code>split_at_punctuation='!"&\'()*+,.:;<=>?@[\]^\`\{\|\}~'</code>.  |
 |`.extract_text(x_tolerance=3, y_tolerance=3, layout=False, x_density=7.25, y_density=13, **kwargs)`| Collates all of the page's character objects into a single string.<ul><li><p>When `layout=False`: Adds spaces where the difference between the `x1` of one character and the `x0` of the next is greater than `x_tolerance`. Adds newline characters where the difference between the `doctop` of one character and the `doctop` of the next is greater than `y_tolerance`.</p></li><li><p>When `layout=True` (*experimental feature*): Attempts to mimic the structural layout of the text on the page(s), using `x_density` and `y_density` to determine the minimum number of characters/newlines per "point," the PDF unit of measurement. All remaining `**kwargs` are passed to `.extract_words(...)` (see above), the first step in calculating the layout.</p></li></ul>|
 |`.extract_text_simple(x_tolerance=3, y_tolerance=3)`| A slightly faster but less flexible version of `.extract_text(...)`, using a simpler logic.|
-|`.search(pattern, regex=True, case=True, **kwargs)`|*Experimental feature* that allows you to search a page's text, returning a list of all instances that match the query. For each instance, the response dictionary object contains the matching text, any regex group matches, the bounding box coordinates, and the char objects themselves. `pattern` can be a compiled regular expression, an uncompiled regular expression, or a non-regex string. If `regex` is `False`, the pattern is treated as a non-regex string. If `case` is `False`, the search is performed in a case-insensitive manner. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`.|
+|`.extract_words(x_tolerance=3, y_tolerance=3, keep_blank_chars=False, use_text_flow=False, horizontal_ltr=True, vertical_ttb=True, extra_attrs=[], split_at_punctuation=False, expand_ligatures=True)`| Returns a list of all word-looking things and their bounding boxes. Words are considered to be sequences of characters where (for "upright" characters) the difference between the `x1` of one character and the `x0` of the next is less than or equal to `x_tolerance` *and* where the `doctop` of one character and the `doctop` of the next is less than or equal to `y_tolerance`. A similar approach is taken for non-upright characters, but instead measuring the vertical, rather than horizontal, distances between them. The parameters `horizontal_ltr` and `vertical_ttb` indicate whether the words should be read from left-to-right (for horizontal words) / top-to-bottom (for vertical words). Changing `keep_blank_chars` to `True` will mean that blank characters are treated as part of a word, not as a space between words. Changing `use_text_flow` to `True` will use the PDF's underlying flow of characters as a guide for ordering and segmenting the words, rather than presorting the characters by x/y position. (This mimics how dragging a cursor highlights text in a PDF; as with that, the order does not always appear to be logical.) Passing a list of `extra_attrs`  (e.g., `["fontname", "size"]` will restrict each words to characters that share exactly the same value for each of those [attributes](#char-properties), and the resulting word dicts will indicate those attributes. Setting `split_at_punctuation` to `True` will enforce breaking tokens at punctuations specified by `string.punctuation`; or you can specify the list of separating punctuation by pass a string, e.g., <code>split_at_punctuation='!"&\'()*+,.:;<=>?@[\]^\`\{\|\}~'</code>. Unless you set `expand_ligatures=False`, ligatures such as `ﬁ` will be expanded into their constituent letters (e.g., `fi`).|
+|`.extract_text_lines(layout=False, strip=True, return_chars=True, **kwargs)`|*Experimental feature* that returns a list of dictionaries representing the lines of text on the page. The `strip` parameter works analogously to Python's `str.strip()` method, and returns `text` attributes without their surrounding whitespace. (Only relevant when `layout = True`.) Setting `return_chars` to `False` will exclude the individual character objects from the returned text-line dicts. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`.|
+|`.search(pattern, regex=True, case=True, main_group=0, return_groups=True, return_chars=True, layout=False, **kwargs)`|*Experimental feature* that allows you to search a page's text, returning a list of all instances that match the query. For each instance, the response dictionary object contains the matching text, any regex group matches, the bounding box coordinates, and the char objects themselves. `pattern` can be a compiled regular expression, an uncompiled regular expression, or a non-regex string. If `regex` is `False`, the pattern is treated as a non-regex string. If `case` is `False`, the search is performed in a case-insensitive manner. Setting `main_group` restricts the results to a specific regex group within the `pattern` (default of `0` means the entire match). Setting `return_groups` and/or `return_chars` to `False` will exclude the lists of the matched regex groups and/or characters from being added (as `"groups"` and `"chars"` to the return dicts). The `layout` parameter operates as it does for `.extract_text(...)`. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`. __Note__: Zero-width and all-whitespace matches are discarded, because they (generally) have no explicit position on the page. |
 |`.dedupe_chars(tolerance=1)`| Returns a version of the page with duplicate chars — those sharing the same text, fontname, size, and positioning (within `tolerance` x/y) as other characters — removed. (See [Issue #71](https://github.com/jsvine/pdfplumber/issues/71) to understand the motivation.)|
 
 ## Extracting tables
 
 `pdfplumber`'s approach to table detection borrows heavily from [Anssi Nurminen's master's thesis](http://dspace.cc.tut.fi/dpub/bitstream/handle/123456789/21520/Nurminen.pdf?sequence=3), and is inspired by [Tabula](https://github.com/tabulapdf/tabula-extractor/issues/16). It works like this:
 
 1. For any given PDF page, find the lines that are (a) explicitly defined and/or (b) implied by the alignment of words on the page.
```

### Comparing `pdfplumber-0.8.1/README.md` & `pdfplumber-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pdfplumber
+Version: 0.9.0
+Summary: Plumb a PDF for detailed information about each char, rectangle, and line.
+Home-page: https://github.com/jsvine/pdfplumber
+Author: Jeremy Singer-Vine
+Author-email: jsvine@gmail.com
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # pdfplumber
 
 [![Version](https://img.shields.io/pypi/v/pdfplumber.svg)](https://pypi.python.org/pypi/pdfplumber) ![Tests](https://github.com/jsvine/pdfplumber/workflows/Tests/badge.svg) [![Code coverage](https://codecov.io/gh/jsvine/pdfplumber/branch/stable/graph/badge.svg)](https://codecov.io/gh/jsvine/pdfplumber/branch/stable) [![Support Python versions](https://img.shields.io/pypi/pyversions/pdfplumber.svg)](https://pypi.python.org/pypi/pdfplumber)
 
 Plumb a PDF for detailed information about each text character, rectangle, and line. Plus: Table extraction and visual debugging.
 
 Works best on machine-generated, rather than scanned, PDFs. Built on [`pdfminer.six`](https://github.com/goulu/pdfminer). 
@@ -226,15 +244,17 @@
 |`doctop`| Distance of curve's highest point from top of document.|
 |`linewidth`| Thickness of line.|
 |`fill`| Whether the shape defined by the curve's path is filled.|
 |`stroking_color`|The color of the curve's outline, expressed as a tuple or integer, depending on the “color space” used.|
 |`non_stroking_color`|The curve’s fill color.|
 |`object_type`| "curve"|
 
-Additionally, both `pdfplumber.PDF` and `pdfplumber.Page` provide access to two derived lists of objects: `.rect_edges` (which decomposes each rectangle into its four lines) and `.edges` (which combines `.rect_edges` with `.lines`). 
+#### Derived properties
+
+Additionally, both `pdfplumber.PDF` and `pdfplumber.Page` provide access to several derived lists of objects: `.rect_edges` (which decomposes each rectangle into its four lines), `.curve_edges` (which does the same for `curve` objects), and `.edges` (which combines `.rect_edges`, `.curve_edges`, and `.lines`). 
 
 #### `image` properties
 
 [To be completed.]
 
 ### Obtaining higher-level layout objects via `pdfminer.six`
 
@@ -316,18 +336,19 @@
 ## Extracting text
 
 `pdfplumber` can extract text from any given page (including cropped and derived pages). It can also attempt to preserve the layout of that text, as well as to identify the coordinates of words and search queries. `Page` objects can call the following text-extraction methods:
 
 
 | Method | Description |
 |--------|-------------|
-|`.extract_words(x_tolerance=3, y_tolerance=3, keep_blank_chars=False, use_text_flow=False, horizontal_ltr=True, vertical_ttb=True, extra_attrs=[], split_at_punctuation=False)`| Returns a list of all word-looking things and their bounding boxes. Words are considered to be sequences of characters where (for "upright" characters) the difference between the `x1` of one character and the `x0` of the next is less than or equal to `x_tolerance` *and* where the `doctop` of one character and the `doctop` of the next is less than or equal to `y_tolerance`. A similar approach is taken for non-upright characters, but instead measuring the vertical, rather than horizontal, distances between them. The parameters `horizontal_ltr` and `vertical_ttb` indicate whether the words should be read from left-to-right (for horizontal words) / top-to-bottom (for vertical words). Changing `keep_blank_chars` to `True` will mean that blank characters are treated as part of a word, not as a space between words. Changing `use_text_flow` to `True` will use the PDF's underlying flow of characters as a guide for ordering and segmenting the words, rather than presorting the characters by x/y position. (This mimics how dragging a cursor highlights text in a PDF; as with that, the order does not always appear to be logical.) Passing a list of `extra_attrs`  (e.g., `["fontname", "size"]` will restrict each words to characters that share exactly the same value for each of those [attributes](#char-properties), and the resulting word dicts will indicate those attributes. Setting `split_at_punctuation` to `True` will enforce breaking tokens at punctuations specified by `string.punctuation`; or you can specify the list of separating punctuation by pass a string, e.g., <code>split_at_punctuation='!"&\'()*+,.:;<=>?@[\]^\`\{\|\}~'</code>.  |
 |`.extract_text(x_tolerance=3, y_tolerance=3, layout=False, x_density=7.25, y_density=13, **kwargs)`| Collates all of the page's character objects into a single string.<ul><li><p>When `layout=False`: Adds spaces where the difference between the `x1` of one character and the `x0` of the next is greater than `x_tolerance`. Adds newline characters where the difference between the `doctop` of one character and the `doctop` of the next is greater than `y_tolerance`.</p></li><li><p>When `layout=True` (*experimental feature*): Attempts to mimic the structural layout of the text on the page(s), using `x_density` and `y_density` to determine the minimum number of characters/newlines per "point," the PDF unit of measurement. All remaining `**kwargs` are passed to `.extract_words(...)` (see above), the first step in calculating the layout.</p></li></ul>|
 |`.extract_text_simple(x_tolerance=3, y_tolerance=3)`| A slightly faster but less flexible version of `.extract_text(...)`, using a simpler logic.|
-|`.search(pattern, regex=True, case=True, **kwargs)`|*Experimental feature* that allows you to search a page's text, returning a list of all instances that match the query. For each instance, the response dictionary object contains the matching text, any regex group matches, the bounding box coordinates, and the char objects themselves. `pattern` can be a compiled regular expression, an uncompiled regular expression, or a non-regex string. If `regex` is `False`, the pattern is treated as a non-regex string. If `case` is `False`, the search is performed in a case-insensitive manner. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`.|
+|`.extract_words(x_tolerance=3, y_tolerance=3, keep_blank_chars=False, use_text_flow=False, horizontal_ltr=True, vertical_ttb=True, extra_attrs=[], split_at_punctuation=False, expand_ligatures=True)`| Returns a list of all word-looking things and their bounding boxes. Words are considered to be sequences of characters where (for "upright" characters) the difference between the `x1` of one character and the `x0` of the next is less than or equal to `x_tolerance` *and* where the `doctop` of one character and the `doctop` of the next is less than or equal to `y_tolerance`. A similar approach is taken for non-upright characters, but instead measuring the vertical, rather than horizontal, distances between them. The parameters `horizontal_ltr` and `vertical_ttb` indicate whether the words should be read from left-to-right (for horizontal words) / top-to-bottom (for vertical words). Changing `keep_blank_chars` to `True` will mean that blank characters are treated as part of a word, not as a space between words. Changing `use_text_flow` to `True` will use the PDF's underlying flow of characters as a guide for ordering and segmenting the words, rather than presorting the characters by x/y position. (This mimics how dragging a cursor highlights text in a PDF; as with that, the order does not always appear to be logical.) Passing a list of `extra_attrs`  (e.g., `["fontname", "size"]` will restrict each words to characters that share exactly the same value for each of those [attributes](#char-properties), and the resulting word dicts will indicate those attributes. Setting `split_at_punctuation` to `True` will enforce breaking tokens at punctuations specified by `string.punctuation`; or you can specify the list of separating punctuation by pass a string, e.g., <code>split_at_punctuation='!"&\'()*+,.:;<=>?@[\]^\`\{\|\}~'</code>. Unless you set `expand_ligatures=False`, ligatures such as `ﬁ` will be expanded into their constituent letters (e.g., `fi`).|
+|`.extract_text_lines(layout=False, strip=True, return_chars=True, **kwargs)`|*Experimental feature* that returns a list of dictionaries representing the lines of text on the page. The `strip` parameter works analogously to Python's `str.strip()` method, and returns `text` attributes without their surrounding whitespace. (Only relevant when `layout = True`.) Setting `return_chars` to `False` will exclude the individual character objects from the returned text-line dicts. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`.|
+|`.search(pattern, regex=True, case=True, main_group=0, return_groups=True, return_chars=True, layout=False, **kwargs)`|*Experimental feature* that allows you to search a page's text, returning a list of all instances that match the query. For each instance, the response dictionary object contains the matching text, any regex group matches, the bounding box coordinates, and the char objects themselves. `pattern` can be a compiled regular expression, an uncompiled regular expression, or a non-regex string. If `regex` is `False`, the pattern is treated as a non-regex string. If `case` is `False`, the search is performed in a case-insensitive manner. Setting `main_group` restricts the results to a specific regex group within the `pattern` (default of `0` means the entire match). Setting `return_groups` and/or `return_chars` to `False` will exclude the lists of the matched regex groups and/or characters from being added (as `"groups"` and `"chars"` to the return dicts). The `layout` parameter operates as it does for `.extract_text(...)`. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`. __Note__: Zero-width and all-whitespace matches are discarded, because they (generally) have no explicit position on the page. |
 |`.dedupe_chars(tolerance=1)`| Returns a version of the page with duplicate chars — those sharing the same text, fontname, size, and positioning (within `tolerance` x/y) as other characters — removed. (See [Issue #71](https://github.com/jsvine/pdfplumber/issues/71) to understand the motivation.)|
 
 ## Extracting tables
 
 `pdfplumber`'s approach to table detection borrows heavily from [Anssi Nurminen's master's thesis](http://dspace.cc.tut.fi/dpub/bitstream/handle/123456789/21520/Nurminen.pdf?sequence=3), and is inspired by [Tabula](https://github.com/tabulapdf/tabula-extractor/issues/16). It works like this:
 
 1. For any given PDF page, find the lines that are (a) explicitly defined and/or (b) implied by the alignment of words on the page.
```

### Comparing `pdfplumber-0.8.1/pdfplumber/cli.py` & `pdfplumber-0.9.0/pdfplumber/cli.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/container.py` & `pdfplumber-0.9.0/pdfplumber/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from . import utils
 from ._typing import T_obj, T_obj_list
 from .convert import CSV_COLS_REQUIRED, CSV_COLS_TO_PREPEND, Serializer
 
 
 class Container(object):
-    cached_properties = ["_rect_edges", "_edges", "_objects"]
+    cached_properties = ["_rect_edges", "_curve_edges", "_edges", "_objects"]
 
     @property
     def pages(self) -> Optional[List[Any]]:
         ...  # pragma: nocover
 
     @property
     def objects(self) -> Dict[str, T_obj_list]:
@@ -70,19 +70,27 @@
         if hasattr(self, "_rect_edges"):
             return self._rect_edges
         rect_edges_gen = (utils.rect_to_edges(r) for r in self.rects)
         self._rect_edges: T_obj_list = list(chain(*rect_edges_gen))
         return self._rect_edges
 
     @property
+    def curve_edges(self) -> T_obj_list:
+        if hasattr(self, "_curve_edges"):
+            return self._curve_edges
+        curve_edges_gen = (utils.curve_to_edges(r) for r in self.curves)
+        self._curve_edges: T_obj_list = list(chain(*curve_edges_gen))
+        return self._curve_edges
+
+    @property
     def edges(self) -> T_obj_list:
         if hasattr(self, "_edges"):
             return self._edges
         line_edges = list(map(utils.line_to_edge, self.lines))
-        self._edges: T_obj_list = self.rect_edges + line_edges
+        self._edges: T_obj_list = line_edges + self.rect_edges + self.curve_edges
         return self._edges
 
     @property
     def horizontal_edges(self) -> T_obj_list:
         def test(x: T_obj) -> bool:
             return bool(x["orientation"] == "h")
```

### Comparing `pdfplumber-0.8.1/pdfplumber/convert.py` & `pdfplumber-0.9.0/pdfplumber/convert.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/ctm.py` & `pdfplumber-0.9.0/pdfplumber/ctm.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/display.py` & `pdfplumber-0.9.0/pdfplumber/display.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/page.py` & `pdfplumber-0.9.0/pdfplumber/page.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,35 @@
 )
 
 
 if TYPE_CHECKING:  # pragma: nocover
     from .display import PageImage
     from .pdf import PDF
 
+# via https://git.ghostscript.com/?p=mupdf.git;a=blob;f=source/pdf/pdf-font.c;h=6322cedf2c26cfb312c0c0878d7aff97b4c7470e;hb=HEAD#l774   # noqa
+
+CP936_FONTNAMES = {
+    b"\xcb\xce\xcc\xe5": "SimSun,Regular",
+    b"\xba\xda\xcc\xe5": "SimHei,Regular",
+    b"\xbf\xac\xcc\xe5_GB2312": "SimKai,Regular",
+    b"\xb7\xc2\xcb\xce_GB2312": "SimFang,Regular",
+    b"\xc1\xa5\xca\xe9": "SimLi,Regular",
+}
+
+
+def fix_fontname_bytes(fontname: bytes) -> str:
+    if b"+" in fontname:
+        split_at = fontname.index(b"+") + 1
+        prefix, suffix = fontname[:split_at], fontname[split_at:]
+    else:
+        prefix, suffix = b"", fontname
+
+    suffix_new = CP936_FONTNAMES.get(suffix, str(suffix)[2:-1])
+    return str(prefix)[2:-1] + suffix_new
+
 
 class Page(Container):
     cached_properties: List[str] = Container.cached_properties + ["_layout"]
     is_original: bool = True
     pages = None
 
     def __init__(
@@ -217,14 +238,18 @@
             attr["text"] = obj.get_text()
 
         if isinstance(obj, LTChar):
             gs = obj.graphicstate
             attr["stroking_color"] = gs.scolor
             attr["non_stroking_color"] = gs.ncolor
 
+            # Handle (rare) byte-encoded fontnames
+            if isinstance(attr["fontname"], bytes):
+                attr["fontname"] = fix_fontname_bytes(attr["fontname"])
+
         if "pts" in attr:
             attr["pts"] = list(map(self.point2coord, attr["pts"]))
 
         if "y0" in attr:
             attr["top"] = self.height - attr["y1"]
             attr["bottom"] = self.height - attr["y0"]
             attr["doctop"] = self.initial_doctop + attr["top"]
@@ -302,28 +327,45 @@
         return utils.chars_to_textmap(self.chars, **full_kwargs)
 
     def search(
         self,
         pattern: Union[str, Pattern[str]],
         regex: bool = True,
         case: bool = True,
+        main_group: int = 0,
+        return_chars: bool = True,
+        return_groups: bool = True,
         **kwargs: Any,
     ) -> List[Dict[str, Any]]:
         textmap = self.get_textmap(**kwargs)
-        return textmap.search(pattern, regex=regex, case=case)
+        return textmap.search(
+            pattern,
+            regex=regex,
+            case=case,
+            main_group=main_group,
+            return_chars=return_chars,
+            return_groups=return_groups,
+        )
 
     def extract_text(self, **kwargs: Any) -> str:
         return self.get_textmap(**kwargs).as_string
 
     def extract_text_simple(self, **kwargs: Any) -> str:
         return utils.extract_text_simple(self.chars, **kwargs)
 
     def extract_words(self, **kwargs: Any) -> T_obj_list:
         return utils.extract_words(self.chars, **kwargs)
 
+    def extract_text_lines(
+        self, strip: bool = True, return_chars: bool = True, **kwargs: Any
+    ) -> T_obj_list:
+        return self.get_textmap(**kwargs).extract_text_lines(
+            strip=strip, return_chars=return_chars
+        )
+
     def crop(
         self, bbox: T_bbox, relative: bool = False, strict: bool = True
     ) -> "CroppedPage":
         return CroppedPage(self, bbox, relative=relative, strict=strict)
 
     def within_bbox(
         self, bbox: T_bbox, relative: bool = False, strict: bool = True
```

### Comparing `pdfplumber-0.8.1/pdfplumber/pdf.py` & `pdfplumber-0.9.0/pdfplumber/pdf.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/table.py` & `pdfplumber-0.9.0/pdfplumber/table.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/utils/__init__.py` & `pdfplumber-0.9.0/pdfplumber/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/utils/clustering.py` & `pdfplumber-0.9.0/pdfplumber/utils/clustering.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/utils/generic.py` & `pdfplumber-0.9.0/pdfplumber/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/utils/geometry.py` & `pdfplumber-0.9.0/pdfplumber/utils/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
     return obj.__class__(tuple(obj.items()) + tuple(new_items))
 
 
 def curve_to_edges(curve: T_obj) -> T_obj_list:
     point_pairs = zip(curve["pts"], curve["pts"][1:])
     return [
         {
+            "object_type": "curve_edge",
             "x0": min(p0[0], p1[0]),
             "x1": max(p0[0], p1[0]),
             "top": min(p0[1], p1[1]),
             "doctop": min(p0[1], p1[1]) + (curve["doctop"] - curve["top"]),
             "bottom": max(p0[1], p1[1]),
             "width": abs(p0[0] - p1[0]),
             "height": abs(p0[1] - p1[1]),
@@ -249,20 +250,21 @@
 def line_to_edge(line: T_obj) -> T_obj:
     edge = dict(line)
     edge["orientation"] = "h" if (line["top"] == line["bottom"]) else "v"
     return edge
 
 
 def obj_to_edges(obj: T_obj) -> T_obj_list:
-    return {
-        "line": lambda x: [line_to_edge(x)],
-        "rect": rect_to_edges,
-        "rect_edge": rect_to_edges,
-        "curve": curve_to_edges,
-    }[obj["object_type"]](obj)
+    t = obj["object_type"]
+    if "_edge" in t:
+        return [obj]
+    elif t == "line":
+        return [line_to_edge(obj)]
+    else:
+        return {"rect": rect_to_edges, "curve": curve_to_edges}[t](obj)
 
 
 def filter_edges(
     edges: T_obj_list,
     orientation: Optional[str] = None,
     edge_type: Optional[str] = None,
     min_length: T_num = 1,
```

### Comparing `pdfplumber-0.8.1/pdfplumber/utils/pdfinternals.py` & `pdfplumber-0.9.0/pdfplumber/utils/pdfinternals.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/pdfplumber/utils/text.py` & `pdfplumber-0.9.0/pdfplumber/utils/text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,81 @@
 import inspect
 import itertools
 import re
 import string
 from operator import itemgetter
 from typing import Any, Dict, Generator, List, Match, Optional, Pattern, Tuple, Union
 
-from .._typing import T_bbox, T_num, T_obj, T_obj_iter, T_obj_list
+from .._typing import T_num, T_obj, T_obj_iter, T_obj_list
 from .clustering import cluster_objects
 from .generic import to_list
-from .geometry import merge_bboxes, obj_to_bbox, objects_to_bbox
+from .geometry import objects_to_bbox
 
 DEFAULT_X_TOLERANCE = 3
 DEFAULT_Y_TOLERANCE = 3
 DEFAULT_X_DENSITY = 7.25
 DEFAULT_Y_DENSITY = 13
 
+LIGATURES = {
+    "ﬀ": "ff",
+    "ﬃ": "ffi",
+    "ﬄ": "ffl",
+    "ﬁ": "fi",
+    "ﬂ": "fl",
+    "ﬆ": "st",
+    "ﬅ": "st",
+}
+
 
 class TextMap:
     """
     A TextMap maps each unicode character in the text to an individual `char`
     object (or, in the case of layout-implied whitespace, `None`).
     """
 
     def __init__(self, tuples: List[Tuple[str, Optional[T_obj]]]) -> None:
         self.tuples = tuples
         self.as_string = "".join(map(itemgetter(0), tuples))
 
+    def match_to_dict(
+        self,
+        m: Match[str],
+        main_group: int = 0,
+        return_groups: bool = True,
+        return_chars: bool = True,
+    ) -> Dict[str, Any]:
+        subset = self.tuples[m.start(main_group) : m.end(main_group)]
+        chars = [c for (text, c) in subset if c is not None]
+        x0, top, x1, bottom = objects_to_bbox(chars)
+
+        result = {
+            "text": m.group(main_group),
+            "x0": x0,
+            "top": top,
+            "x1": x1,
+            "bottom": bottom,
+        }
+
+        if return_groups:
+            result["groups"] = m.groups()
+
+        if return_chars:
+            result["chars"] = chars
+
+        return result
+
     def search(
-        self, pattern: Union[str, Pattern[str]], regex: bool = True, case: bool = True
+        self,
+        pattern: Union[str, Pattern[str]],
+        regex: bool = True,
+        case: bool = True,
+        return_groups: bool = True,
+        return_chars: bool = True,
+        main_group: int = 0,
     ) -> List[Dict[str, Any]]:
-        def match_to_dict(m: Match[str]) -> Dict[str, Any]:
-            subset = self.tuples[m.start() : m.end()]
-            chars = [c for (text, c) in subset if c is not None]
-            x0, top, x1, bottom = objects_to_bbox(chars)
-            return {
-                "text": m.group(0),
-                "groups": m.groups(),
-                "x0": x0,
-                "top": top,
-                "x1": x1,
-                "bottom": bottom,
-                "chars": chars,
-            }
 
         if isinstance(pattern, Pattern):
             if regex is False:
                 raise ValueError(
                     "Cannot pass a compiled search pattern *and* regex=False together."
                 )
             if case is False:
@@ -57,15 +87,46 @@
             if regex is False:
                 pattern = re.escape(pattern)
 
             flags = re.I if case is False else 0
             compiled = re.compile(pattern, flags)
 
         gen = re.finditer(compiled, self.as_string)
-        return list(map(match_to_dict, gen))
+        # Remove zero-length matches (can happen, e.g., with optional
+        # patterns in regexes) and whitespace-only matches
+        filtered = filter(lambda m: bool(m.group(main_group).strip()), gen)
+        return [
+            self.match_to_dict(
+                m,
+                return_groups=return_groups,
+                return_chars=return_chars,
+                main_group=main_group,
+            )
+            for m in filtered
+        ]
+
+    def extract_text_lines(
+        self, strip: bool = True, return_chars: bool = True
+    ) -> List[Dict[str, Any]]:
+        """
+        `strip` is analogous to Python's `str.strip()` method, and returns
+        `text` attributes without their surrounding whitespace. Only
+        relevant when the relevant TextMap is created with `layout` = True
+
+        Setting `return_chars` to False will exclude the individual
+        character objects from the returned text-line dicts.
+        """
+        if strip:
+            pat = r" *([^\n]+?) *(\n|$)"
+        else:
+            pat = r"([^\n]+)"
+
+        return self.search(
+            pat, main_group=1, return_chars=return_chars, return_groups=False
+        )
 
 
 class WordMap:
     """
     A WordMap maps words->chars.
     """
 
@@ -81,14 +142,15 @@
         layout_height_chars: int = 0,
         x_density: T_num = DEFAULT_X_DENSITY,
         y_density: T_num = DEFAULT_Y_DENSITY,
         x_shift: T_num = 0,
         y_shift: T_num = 0,
         y_tolerance: T_num = DEFAULT_Y_TOLERANCE,
         presorted: bool = False,
+        expand_ligatures: bool = True,
     ) -> TextMap:
         """
         Given a list of (word, chars) tuples (i.e., a WordMap), return a list of
         (char-text, char) tuples (i.e., a TextMap) that can be used to mimic the
         structural layout of the text on the page(s), using the following approach:
 
         - Sort the words by (doctop, x0) if not already sorted.
@@ -122,14 +184,16 @@
         vertical text.
         """
         _textmap: List[Tuple[str, Optional[T_obj]]] = []
 
         if not len(self.tuples):
             return TextMap(_textmap)
 
+        expansions = LIGATURES if expand_ligatures else {}
+
         if layout:
             if layout_width_chars:
                 if layout_width:
                     raise ValueError(
                         "`layout_width` and `layout_width_chars` cannot both be set."
                     )
             else:
@@ -181,18 +245,21 @@
             num_newlines += num_newlines_prepend
 
             line_len = 0
             for word, chars in sorted(ws, key=lambda x: float(x[0]["x0"])):
                 x_dist = (word["x0"] - x_shift) / x_density if layout else 0
                 num_spaces_prepend = max(min(1, line_len), round(x_dist) - line_len)
                 _textmap += [(" ", None)] * num_spaces_prepend
+                line_len += num_spaces_prepend
+
                 for c in chars:
-                    for letter in c["text"]:
+                    letters = expansions.get(c["text"], c["text"])
+                    for letter in letters:
                         _textmap.append((letter, c))
-                line_len += num_spaces_prepend + len(word["text"])
+                        line_len += 1
 
             # Append spaces at end of line
             if layout:
                 _textmap += [(" ", None)] * (layout_width_chars - line_len)
 
         # Append blank lines at end of text
         if layout:
@@ -216,14 +283,15 @@
         y_tolerance: T_num = DEFAULT_Y_TOLERANCE,
         keep_blank_chars: bool = False,
         use_text_flow: bool = False,
         horizontal_ltr: bool = True,  # Should words be read left-to-right?
         vertical_ttb: bool = True,  # Should vertical words be read top-to-bottom?
         extra_attrs: Optional[List[str]] = None,
         split_at_punctuation: Union[bool, str] = False,
+        expand_ligatures: bool = True,
     ):
         self.x_tolerance = x_tolerance
         self.y_tolerance = y_tolerance
         self.keep_blank_chars = keep_blank_chars
         self.use_text_flow = use_text_flow
         self.horizontal_ltr = horizontal_ltr
         self.vertical_ttb = vertical_ttb
@@ -232,23 +300,27 @@
         # Note: string.punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
         self.split_at_punctuation = (
             string.punctuation
             if split_at_punctuation is True
             else (split_at_punctuation or "")
         )
 
+        self.expansions = LIGATURES if expand_ligatures else {}
+
     def merge_chars(self, ordered_chars: T_obj_list) -> T_obj:
         x0, top, x1, bottom = objects_to_bbox(ordered_chars)
         doctop_adj = ordered_chars[0]["doctop"] - ordered_chars[0]["top"]
         upright = ordered_chars[0]["upright"]
 
         direction = 1 if (self.horizontal_ltr if upright else self.vertical_ttb) else -1
 
         word = {
-            "text": "".join(map(itemgetter("text"), ordered_chars)),
+            "text": "".join(
+                self.expansions.get(c["text"], c["text"]) for c in ordered_chars
+            ),
             "x0": x0,
             "x1": x1,
             "top": top,
             "doctop": top + doctop_adj,
             "bottom": bottom,
             "upright": upright,
             "direction": direction,
@@ -257,73 +329,117 @@
         for key in self.extra_attrs:
             word[key] = ordered_chars[0][key]
 
         return word
 
     def char_begins_new_word(
         self,
-        current_chars: T_obj_list,
-        current_bbox: T_bbox,
-        next_char: T_obj,
+        prev_char: T_obj,
+        curr_char: T_obj,
     ) -> bool:
+        """This method takes several factors into account to determine if
+        `curr_char` represents the beginning of a new word:
+
+        - Whether the text is "upright" (i.e., non-rotated)
+        - Whether the user has specified that horizontal text runs
+          left-to-right (default) or right-to-left, as represented by
+          self.horizontal_ltr
+        - Whether the user has specified that vertical text the text runs
+          top-to-bottom (default) or bottom-to-top, as represented by
+          self.vertical_ttb
+        - The x0, top, x1, and bottom attributes of prev_char and
+          curr_char
+        - The self.x_tolerance and self.y_tolerance settings. Note: In
+          this case, x/y refer to those directions for non-rotated text.
+          For vertical text, they are flipped. A more accurate terminology
+          might be "*intra*line character distance tolerance" and
+          "*inter*line character distance tolerance"
+
+        An important note: The *intra*line distance is measured from the
+        *end* of the previous character to the *beginning* of the current
+        character, while the *inter*line distance is measured from the
+        *top* of the previous character to the *top* of the next
+        character. The reasons for this are partly repository-historical,
+        and partly logical, as successive text lines' bounding boxes often
+        overlap slightly (and we don't want that overlap to be interpreted
+        as the two lines being the same line).
+
+        The upright-ness of the character determines the attributes to
+        compare, while horizontal_ltr/vertical_ttb determine the direction
+        of the comparison.
+        """
 
-        upright = current_chars[0]["upright"]
-        intraline_tol = self.x_tolerance if upright else self.y_tolerance
-        interline_tol = self.y_tolerance if upright else self.x_tolerance
+        # Note: Due to the grouping step earlier in the process,
+        # curr_char["upright"] will always equal prev_char["upright"].
+        if curr_char["upright"]:
+            inter_tol = self.y_tolerance
+            intra_tol = self.x_tolerance
+
+            inter_attr = "top"
+            intra_attr_min = "x0"
+            intra_attr_max = "x1"
+
+            if self.horizontal_ltr:
+                char_min = prev_char
+                char_max = curr_char
+            else:
+                char_min = curr_char
+                char_max = prev_char
+        else:
+            inter_tol = self.x_tolerance
+            intra_tol = self.y_tolerance
 
-        word_x0, word_top, word_x1, word_bottom = current_bbox
+            inter_attr = "x0"
+            intra_attr_min = "top"
+            intra_attr_max = "bottom"
+
+            if self.vertical_ttb:
+                char_min = curr_char
+                char_max = prev_char
+            else:
+                char_min = prev_char
+                char_max = curr_char
 
         return bool(
-            (next_char["x0"] > word_x1 + intraline_tol)
-            or (next_char["x1"] < word_x0 - intraline_tol)
-            or (next_char["top"] > word_bottom + interline_tol)
-            or (next_char["bottom"] < word_top - interline_tol)
+            # Intraline test
+            (char_max[intra_attr_min] > char_min[intra_attr_max] + intra_tol)
+            # Interline test
+            or (char_max[inter_attr] > char_min[inter_attr] + inter_tol)
         )
 
     def iter_chars_to_words(
-        self, chars: T_obj_iter
+        self, ordered_chars: T_obj_iter
     ) -> Generator[T_obj_list, None, None]:
         current_word: T_obj_list = []
-        current_bbox: Optional[T_bbox] = None
 
         def start_next_word(
             new_char: Optional[T_obj],
         ) -> Generator[T_obj_list, None, None]:
             nonlocal current_word
-            nonlocal current_bbox
 
             if current_word:
                 yield current_word
 
             current_word = [] if new_char is None else [new_char]
-            current_bbox = None if new_char is None else obj_to_bbox(new_char)
 
-        for char in chars:
+        for char in ordered_chars:
             text = char["text"]
 
             if not self.keep_blank_chars and text.isspace():
                 yield from start_next_word(None)
 
             elif text in self.split_at_punctuation:
                 yield from start_next_word(char)
                 yield from start_next_word(None)
 
-            elif (
-                current_word
-                and current_bbox
-                and self.char_begins_new_word(current_word, current_bbox, char)
-            ):
+            elif current_word and self.char_begins_new_word(current_word[-1], char):
                 yield from start_next_word(char)
 
             else:
                 current_word.append(char)
-                if current_bbox is None:
-                    current_bbox = obj_to_bbox(char)
-                else:
-                    current_bbox = merge_bboxes([current_bbox, obj_to_bbox(char)])
 
         # Finally, after all chars processed
         if current_word:
             yield current_word
 
     def iter_sort_chars(self, chars: T_obj_iter) -> Generator[T_obj, None, None]:
         def upright_key(x: T_obj) -> int:
@@ -348,21 +464,20 @@
                     yield from reversed(to_yield)
                 else:
                     yield from to_yield
 
     def iter_extract_tuples(
         self, chars: T_obj_iter
     ) -> Generator[Tuple[T_obj, T_obj_list], None, None]:
-        if not self.use_text_flow:
-            chars = self.iter_sort_chars(chars)
+        ordered_chars = chars if self.use_text_flow else self.iter_sort_chars(chars)
 
         grouping_key = itemgetter("upright", *self.extra_attrs)
-        grouped = itertools.groupby(chars, grouping_key)
+        grouped_chars = itertools.groupby(ordered_chars, grouping_key)
 
-        for keyvals, char_group in grouped:
+        for keyvals, char_group in grouped_chars:
             for word_chars in self.iter_chars_to_words(char_group):
                 yield (self.merge_chars(word_chars), word_chars)
 
     def extract_wordmap(self, chars: T_obj_iter) -> WordMap:
         return WordMap(list(self.iter_extract_tuples(chars)))
 
     def extract_words(self, chars: T_obj_list) -> T_obj_list:
@@ -398,15 +513,14 @@
     chars = to_list(chars)
     if len(chars) == 0:
         return ""
 
     if kwargs.get("layout"):
         return chars_to_textmap(chars, **kwargs).as_string
     else:
-        kwargs.update()
         y_tolerance = kwargs.get("y_tolerance", DEFAULT_Y_TOLERANCE)
         extractor = WordExtractor(
             **{k: kwargs[k] for k in WORD_EXTRACTOR_KWARGS if k in kwargs}
         )
         words = extractor.extract_words(chars)
         lines = cluster_objects(words, itemgetter("doctop"), y_tolerance)
         return "\n".join(" ".join(word["text"] for word in line) for line in lines)
```

### Comparing `pdfplumber-0.8.1/pdfplumber.egg-info/PKG-INFO` & `pdfplumber-0.9.0/pdfplumber.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfplumber
-Version: 0.8.1
+Version: 0.9.0
 Summary: Plumb a PDF for detailed information about each char, rectangle, and line.
 Home-page: https://github.com/jsvine/pdfplumber
 Author: Jeremy Singer-Vine
 Author-email: jsvine@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -244,15 +244,17 @@
 |`doctop`| Distance of curve's highest point from top of document.|
 |`linewidth`| Thickness of line.|
 |`fill`| Whether the shape defined by the curve's path is filled.|
 |`stroking_color`|The color of the curve's outline, expressed as a tuple or integer, depending on the “color space” used.|
 |`non_stroking_color`|The curve’s fill color.|
 |`object_type`| "curve"|
 
-Additionally, both `pdfplumber.PDF` and `pdfplumber.Page` provide access to two derived lists of objects: `.rect_edges` (which decomposes each rectangle into its four lines) and `.edges` (which combines `.rect_edges` with `.lines`). 
+#### Derived properties
+
+Additionally, both `pdfplumber.PDF` and `pdfplumber.Page` provide access to several derived lists of objects: `.rect_edges` (which decomposes each rectangle into its four lines), `.curve_edges` (which does the same for `curve` objects), and `.edges` (which combines `.rect_edges`, `.curve_edges`, and `.lines`). 
 
 #### `image` properties
 
 [To be completed.]
 
 ### Obtaining higher-level layout objects via `pdfminer.six`
 
@@ -334,18 +336,19 @@
 ## Extracting text
 
 `pdfplumber` can extract text from any given page (including cropped and derived pages). It can also attempt to preserve the layout of that text, as well as to identify the coordinates of words and search queries. `Page` objects can call the following text-extraction methods:
 
 
 | Method | Description |
 |--------|-------------|
-|`.extract_words(x_tolerance=3, y_tolerance=3, keep_blank_chars=False, use_text_flow=False, horizontal_ltr=True, vertical_ttb=True, extra_attrs=[], split_at_punctuation=False)`| Returns a list of all word-looking things and their bounding boxes. Words are considered to be sequences of characters where (for "upright" characters) the difference between the `x1` of one character and the `x0` of the next is less than or equal to `x_tolerance` *and* where the `doctop` of one character and the `doctop` of the next is less than or equal to `y_tolerance`. A similar approach is taken for non-upright characters, but instead measuring the vertical, rather than horizontal, distances between them. The parameters `horizontal_ltr` and `vertical_ttb` indicate whether the words should be read from left-to-right (for horizontal words) / top-to-bottom (for vertical words). Changing `keep_blank_chars` to `True` will mean that blank characters are treated as part of a word, not as a space between words. Changing `use_text_flow` to `True` will use the PDF's underlying flow of characters as a guide for ordering and segmenting the words, rather than presorting the characters by x/y position. (This mimics how dragging a cursor highlights text in a PDF; as with that, the order does not always appear to be logical.) Passing a list of `extra_attrs`  (e.g., `["fontname", "size"]` will restrict each words to characters that share exactly the same value for each of those [attributes](#char-properties), and the resulting word dicts will indicate those attributes. Setting `split_at_punctuation` to `True` will enforce breaking tokens at punctuations specified by `string.punctuation`; or you can specify the list of separating punctuation by pass a string, e.g., <code>split_at_punctuation='!"&\'()*+,.:;<=>?@[\]^\`\{\|\}~'</code>.  |
 |`.extract_text(x_tolerance=3, y_tolerance=3, layout=False, x_density=7.25, y_density=13, **kwargs)`| Collates all of the page's character objects into a single string.<ul><li><p>When `layout=False`: Adds spaces where the difference between the `x1` of one character and the `x0` of the next is greater than `x_tolerance`. Adds newline characters where the difference between the `doctop` of one character and the `doctop` of the next is greater than `y_tolerance`.</p></li><li><p>When `layout=True` (*experimental feature*): Attempts to mimic the structural layout of the text on the page(s), using `x_density` and `y_density` to determine the minimum number of characters/newlines per "point," the PDF unit of measurement. All remaining `**kwargs` are passed to `.extract_words(...)` (see above), the first step in calculating the layout.</p></li></ul>|
 |`.extract_text_simple(x_tolerance=3, y_tolerance=3)`| A slightly faster but less flexible version of `.extract_text(...)`, using a simpler logic.|
-|`.search(pattern, regex=True, case=True, **kwargs)`|*Experimental feature* that allows you to search a page's text, returning a list of all instances that match the query. For each instance, the response dictionary object contains the matching text, any regex group matches, the bounding box coordinates, and the char objects themselves. `pattern` can be a compiled regular expression, an uncompiled regular expression, or a non-regex string. If `regex` is `False`, the pattern is treated as a non-regex string. If `case` is `False`, the search is performed in a case-insensitive manner. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`.|
+|`.extract_words(x_tolerance=3, y_tolerance=3, keep_blank_chars=False, use_text_flow=False, horizontal_ltr=True, vertical_ttb=True, extra_attrs=[], split_at_punctuation=False, expand_ligatures=True)`| Returns a list of all word-looking things and their bounding boxes. Words are considered to be sequences of characters where (for "upright" characters) the difference between the `x1` of one character and the `x0` of the next is less than or equal to `x_tolerance` *and* where the `doctop` of one character and the `doctop` of the next is less than or equal to `y_tolerance`. A similar approach is taken for non-upright characters, but instead measuring the vertical, rather than horizontal, distances between them. The parameters `horizontal_ltr` and `vertical_ttb` indicate whether the words should be read from left-to-right (for horizontal words) / top-to-bottom (for vertical words). Changing `keep_blank_chars` to `True` will mean that blank characters are treated as part of a word, not as a space between words. Changing `use_text_flow` to `True` will use the PDF's underlying flow of characters as a guide for ordering and segmenting the words, rather than presorting the characters by x/y position. (This mimics how dragging a cursor highlights text in a PDF; as with that, the order does not always appear to be logical.) Passing a list of `extra_attrs`  (e.g., `["fontname", "size"]` will restrict each words to characters that share exactly the same value for each of those [attributes](#char-properties), and the resulting word dicts will indicate those attributes. Setting `split_at_punctuation` to `True` will enforce breaking tokens at punctuations specified by `string.punctuation`; or you can specify the list of separating punctuation by pass a string, e.g., <code>split_at_punctuation='!"&\'()*+,.:;<=>?@[\]^\`\{\|\}~'</code>. Unless you set `expand_ligatures=False`, ligatures such as `ﬁ` will be expanded into their constituent letters (e.g., `fi`).|
+|`.extract_text_lines(layout=False, strip=True, return_chars=True, **kwargs)`|*Experimental feature* that returns a list of dictionaries representing the lines of text on the page. The `strip` parameter works analogously to Python's `str.strip()` method, and returns `text` attributes without their surrounding whitespace. (Only relevant when `layout = True`.) Setting `return_chars` to `False` will exclude the individual character objects from the returned text-line dicts. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`.|
+|`.search(pattern, regex=True, case=True, main_group=0, return_groups=True, return_chars=True, layout=False, **kwargs)`|*Experimental feature* that allows you to search a page's text, returning a list of all instances that match the query. For each instance, the response dictionary object contains the matching text, any regex group matches, the bounding box coordinates, and the char objects themselves. `pattern` can be a compiled regular expression, an uncompiled regular expression, or a non-regex string. If `regex` is `False`, the pattern is treated as a non-regex string. If `case` is `False`, the search is performed in a case-insensitive manner. Setting `main_group` restricts the results to a specific regex group within the `pattern` (default of `0` means the entire match). Setting `return_groups` and/or `return_chars` to `False` will exclude the lists of the matched regex groups and/or characters from being added (as `"groups"` and `"chars"` to the return dicts). The `layout` parameter operates as it does for `.extract_text(...)`. The remaining `**kwargs` are those you would pass to `.extract_text(layout=True, ...)`. __Note__: Zero-width and all-whitespace matches are discarded, because they (generally) have no explicit position on the page. |
 |`.dedupe_chars(tolerance=1)`| Returns a version of the page with duplicate chars — those sharing the same text, fontname, size, and positioning (within `tolerance` x/y) as other characters — removed. (See [Issue #71](https://github.com/jsvine/pdfplumber/issues/71) to understand the motivation.)|
 
 ## Extracting tables
 
 `pdfplumber`'s approach to table detection borrows heavily from [Anssi Nurminen's master's thesis](http://dspace.cc.tut.fi/dpub/bitstream/handle/123456789/21520/Nurminen.pdf?sequence=3), and is inspired by [Tabula](https://github.com/tabulapdf/tabula-extractor/issues/16). It works like this:
 
 1. For any given PDF page, find the lines that are (a) explicitly defined and/or (b) implied by the alignment of words on the page.
```

### Comparing `pdfplumber-0.8.1/pdfplumber.egg-info/SOURCES.txt` & `pdfplumber-0.9.0/pdfplumber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/setup.py` & `pdfplumber-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_basics.py` & `pdfplumber-0.9.0/tests/test_basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,22 @@
 
 
 class Test(unittest.TestCase):
     @classmethod
     def setup_class(self):
         path = os.path.join(HERE, "pdfs/nics-background-checks-2015-11.pdf")
         self.pdf = pdfplumber.open(path)
+        # via http://www.pdfill.com/example/pdf_drawing_new.pdf
+        path_2 = os.path.join(HERE, "pdfs/pdffill-demo.pdf")
+        self.pdf_2 = pdfplumber.open(path_2)
 
     @classmethod
     def teardown_class(self):
         self.pdf.close()
+        self.pdf_2.close()
 
     def test_metadata(self):
         metadata = self.pdf.metadata
         assert isinstance(metadata["Producer"], str)
 
     def test_pagecount(self):
         assert len(self.pdf.pages) == 1
@@ -34,26 +38,26 @@
         assert str(self.pdf.pages[0]) == "<Page:1>"
 
     def test_objects(self):
         assert len(self.pdf.chars)
         assert len(self.pdf.rects)
         assert len(self.pdf.lines)
         assert len(self.pdf.rect_edges)
+        assert len(self.pdf_2.curve_edges)
         # Ensure that caching is working:
         assert id(self.pdf._rect_edges) == id(self.pdf.rect_edges)
+        assert id(self.pdf_2._curve_edges) == id(self.pdf_2.curve_edges)
         assert id(self.pdf.pages[0]._layout) == id(self.pdf.pages[0].layout)
 
     def test_annots(self):
-        # via http://www.pdfill.com/example/pdf_drawing_new.pdf
-        path = os.path.join(HERE, "pdfs/pdffill-demo.pdf")
-        with pdfplumber.open(path) as pdf:
-            assert len(pdf.annots)
-            assert len(pdf.hyperlinks) == 17
-            uri = "http://www.pdfill.com/pdf_drawing.html"
-            assert pdf.hyperlinks[0]["uri"] == uri
+        pdf = self.pdf_2
+        assert len(pdf.annots)
+        assert len(pdf.hyperlinks) == 17
+        uri = "http://www.pdfill.com/pdf_drawing.html"
+        assert pdf.hyperlinks[0]["uri"] == uri
 
         path = os.path.join(HERE, "pdfs/annotations.pdf")
         with pdfplumber.open(path) as pdf:
             assert len(pdf.annots)
 
     def test_crop_and_filter(self):
         def test(obj):
```

### Comparing `pdfplumber-0.8.1/tests/test_ca_warn_report.py` & `pdfplumber-0.9.0/tests/test_ca_warn_report.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_convert.py` & `pdfplumber-0.9.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_ctm.py` & `pdfplumber-0.9.0/tests/test_ctm.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_dedupe_chars.py` & `pdfplumber-0.9.0/tests/test_dedupe_chars.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_display.py` & `pdfplumber-0.9.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_issues.py` & `pdfplumber-0.9.0/tests/test_issues.py`

 * *Files 12% similar despite different names*

```diff
@@ -186,23 +186,66 @@
         util.extract_text() should not raise exception if given pure iterator
         """
         path = os.path.join(HERE, "pdfs/nics-background-checks-2015-11.pdf")
         with pdfplumber.open(path) as pdf:
             chars = (char for char in pdf.chars)
             pdfplumber.utils.extract_text(chars)
 
+    def test_issue_461_and_842(self):
+        """
+        pdfplumber should gracefully handle characters with byte-encoded
+        font names.
+        """
+        before = b"RGJSAP+\xcb\xce\xcc\xe5"
+        after = pdfplumber.page.fix_fontname_bytes(before)
+        assert after == "RGJSAP+SimSun,Regular"
+
+        before = b"\xcb\xce\xcc\xe5"
+        after = pdfplumber.page.fix_fontname_bytes(before)
+        assert after == "SimSun,Regular"
+
+        path = os.path.join(HERE, "pdfs/issue-461-example.pdf")
+        with pdfplumber.open(path) as pdf:
+            page = pdf.pages[0]
+            assert all(isinstance(c["fontname"], str) for c in page.chars)
+            page.dedupe_chars()
+
+        path = os.path.join(HERE, "pdfs/issue-842-example.pdf")
+        with pdfplumber.open(path) as pdf:
+            page = pdf.pages[0]
+            assert all(isinstance(c["fontname"], str) for c in page.chars)
+            page.dedupe_chars()
+
     def test_issue_463(self):
         """
         Extracting annotations should not raise UnicodeDecodeError on utf-16 text
         """
         path = os.path.join(HERE, "pdfs/issue-463-example.pdf")
         with pdfplumber.open(path) as pdf:
             annots = pdf.annots
             annots[0]["contents"] == "日本語"
 
+    def test_issue_598(self):
+        """
+        Ligatures should be translated by default.
+        """
+        path = os.path.join(HERE, "pdfs/issue-598-example.pdf")
+        with pdfplumber.open(path) as pdf:
+            page = pdf.pages[0]
+            a = page.extract_text()
+            assert "fiction" in a
+            assert "ﬁction" not in a
+
+            b = page.extract_text(expand_ligatures=False)
+            assert "ﬁction" in b
+            assert "fiction" not in b
+
+            assert page.extract_words()[53]["text"] == "fiction"
+            assert page.extract_words(expand_ligatures=False)[53]["text"] == "ﬁction"
+
     def test_issue_683(self):
         """
         Page.search ValueError: min() arg is an empty sequence
 
         This ultimately stemmed from a mistaken assumption in
         LayoutEngine.calculate(...) that len(char["text"]) would always equal
         1, which is not true for ligatures. Issue 683 does not provide a PDF,
```

### Comparing `pdfplumber-0.8.1/tests/test_laparams.py` & `pdfplumber-0.9.0/tests/test_laparams.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_nics_report.py` & `pdfplumber-0.9.0/tests/test_nics_report.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-0.8.1/tests/test_table.py` & `pdfplumber-0.9.0/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,7 +207,20 @@
                 "min_words_horizontal": 1,
                 "text_keep_blank_chars": False,
                 "text_tolerance": 3,
                 "intersection_tolerance": 3,
             }
             assert page.extract_table(table_settings)
             assert page.extract_tables(table_settings)
+
+    def test_table_curves(self):
+        # See https://github.com/jsvine/pdfplumber/discussions/808
+        path = os.path.join(HERE, "pdfs/table-curves-example.pdf")
+        with pdfplumber.open(path) as pdf:
+            page = pdf.pages[0]
+            assert len(page.curves)
+            tables = page.extract_tables()
+            assert len(tables) == 1
+            t = tables[0]
+            assert t[-2][-2] == "Uncommon"
+
+            assert len(page.extract_tables({"vertical_strategy": "lines_strict"})) == 0
```

### Comparing `pdfplumber-0.8.1/tests/test_utils.py` & `pdfplumber-0.9.0/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -275,14 +275,56 @@
 
         results = page.search("supreme court", regex=True, case=False)
         assert len(results) == 2
 
         results = page.search(r"supreme\s+(\w+)", regex=False)
         assert len(results) == 0
 
+        results = page.search(r"10 Tuesday", layout=False)
+        assert len(results) == 1
+
+        results = page.search(r"10 Tuesday", layout=True)
+        assert len(results) == 0
+
+    def test_extract_text_lines(self):
+        page = self.pdf_scotus.pages[0]
+        results = page.extract_text_lines()
+        assert len(results) == 28
+        assert "chars" in results[0]
+        assert results[0]["text"] == "Official - Subject to Final Review"
+
+        alt = page.extract_text_lines(layout=True, strip=False, return_chars=False)
+        assert "chars" not in alt[0]
+        assert (
+            alt[0]["text"]
+            == "                                   Official - Subject to Final Review               "  # noqa: E501
+        )
+
+        assert results[10]["text"] == "10 Tuesday, January 13, 2009"
+        assert (
+            alt[10]["text"]
+            == "            10                          Tuesday, January 13, 2009                   "  # noqa: E501
+        )
+        assert (
+            page.extract_text_lines(layout=True)[10]["text"]
+            == "10                          Tuesday, January 13, 2009"
+        )  # noqa: E501
+
+    def test_handle_empty_and_whitespace_search_results(self):
+        # via https://github.com/jsvine/pdfplumber/discussions/853
+        # The searches below should not raise errors but instead
+        # should return empty result-sets.
+        page = self.pdf_scotus.pages[0]
+        for regex in [True, False]:
+            results = page.search("\n", regex=regex)
+            assert len(results) == 0
+
+        assert len(page.search("(sdfsd)?")) == 0
+        assert len(page.search("")) == 0
+
     def test_intersects_bbox(self):
         objs = [
             # Is same as bbox
             {
                 "x0": 0,
                 "top": 0,
                 "x1": 20,
@@ -324,14 +366,22 @@
                 "bottom": 40,
             },
         ]
         bbox = utils.obj_to_bbox(objs[0])
 
         assert utils.intersects_bbox(objs, bbox) == objs[:4]
 
+    def test_merge_bboxes(self):
+        bboxes = [
+            (0, 10, 20, 20),
+            (10, 5, 10, 30),
+        ]
+        merged = utils.merge_bboxes(bboxes)
+        assert merged == (0, 5, 20, 30)
+
     def test_resize_object(self):
         obj = {
             "x0": 5,
             "x1": 10,
             "top": 20,
             "bottom": 30,
             "width": 5,
```

