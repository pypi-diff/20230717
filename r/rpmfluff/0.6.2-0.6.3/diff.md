# Comparing `tmp/rpmfluff-0.6.2.tar.gz` & `tmp/rpmfluff-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpmfluff-0.6.2.tar", last modified: Tue Oct 18 20:10:23 2022, max compression
+gzip compressed data, was "rpmfluff-0.6.3.tar", last modified: Mon Jul 17 07:07:43 2023, max compression
```

## Comparing `rpmfluff-0.6.2.tar` & `rpmfluff-0.6.3.tar`

### file list

```diff
@@ -1,50 +1,62 @@
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2022-10-18 20:10:23.177768 rpmfluff-0.6.2/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    17987 2021-01-05 12:37:29.105099 rpmfluff-0.6.2/LICENSE
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)       47 2021-01-05 12:37:29.000000 rpmfluff-0.6.2/MANIFEST.in
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      634 2022-10-18 20:10:23.177768 rpmfluff-0.6.2/PKG-INFO
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1356 2021-01-05 12:37:29.105099 rpmfluff-0.6.2/README-releng
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4920 2022-10-18 20:09:07.000000 rpmfluff-0.6.2/README.md
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6379 2022-10-18 19:58:52.762720 rpmfluff-0.6.2/python-rpmfluff.spec
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2021-01-05 12:47:10.844641 rpmfluff-0.6.2/rpmfluff/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1647 2021-01-05 12:37:29.106099 rpmfluff-0.6.2/rpmfluff/__init__.py
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2022-10-18 19:54:34.640954 rpmfluff-0.6.2/rpmfluff/__pycache__/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1225 2022-10-18 19:54:34.604954 rpmfluff-0.6.2/rpmfluff/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1223 2021-01-05 12:38:12.023582 rpmfluff-0.6.2/rpmfluff/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6130 2022-10-18 19:54:34.618954 rpmfluff-0.6.2/rpmfluff/__pycache__/check.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6616 2021-01-05 12:40:17.266990 rpmfluff-0.6.2/rpmfluff/__pycache__/check.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1719 2022-10-18 19:54:34.625954 rpmfluff-0.6.2/rpmfluff/__pycache__/make.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1736 2021-01-05 12:40:17.272990 rpmfluff-0.6.2/rpmfluff/__pycache__/make.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    26585 2022-10-18 19:54:34.631954 rpmfluff-0.6.2/rpmfluff/__pycache__/rpmbuild.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    26981 2021-01-05 12:55:19.922105 rpmfluff-0.6.2/rpmfluff/__pycache__/rpmbuild.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      934 2022-10-18 19:54:34.633954 rpmfluff-0.6.2/rpmfluff/__pycache__/samples.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      932 2021-01-05 12:40:17.277990 rpmfluff-0.6.2/rpmfluff/__pycache__/samples.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2254 2022-10-18 19:54:34.633954 rpmfluff-0.6.2/rpmfluff/__pycache__/sourcefile.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2340 2021-01-05 12:40:17.278990 rpmfluff-0.6.2/rpmfluff/__pycache__/sourcefile.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4018 2022-10-18 19:54:34.634954 rpmfluff-0.6.2/rpmfluff/__pycache__/subpackage.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4264 2021-01-05 12:40:17.278990 rpmfluff-0.6.2/rpmfluff/__pycache__/subpackage.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      981 2022-10-18 19:54:34.634954 rpmfluff-0.6.2/rpmfluff/__pycache__/tarball.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      977 2021-01-05 12:40:17.279990 rpmfluff-0.6.2/rpmfluff/__pycache__/tarball.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    28331 2022-10-18 19:54:34.639954 rpmfluff-0.6.2/rpmfluff/__pycache__/test.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1640 2022-10-18 19:54:34.635954 rpmfluff-0.6.2/rpmfluff/__pycache__/trigger.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1636 2021-01-05 12:40:17.279990 rpmfluff-0.6.2/rpmfluff/__pycache__/trigger.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1763 2022-10-18 19:54:34.619954 rpmfluff-0.6.2/rpmfluff/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1777 2021-01-05 12:40:17.266990 rpmfluff-0.6.2/rpmfluff/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1350 2022-10-18 19:54:34.640954 rpmfluff-0.6.2/rpmfluff/__pycache__/yumrepobuild.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6451 2021-01-05 12:37:29.106099 rpmfluff-0.6.2/rpmfluff/check.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2109 2021-01-05 12:37:29.106099 rpmfluff-0.6.2/rpmfluff/make.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    32286 2021-01-05 12:47:10.829641 rpmfluff-0.6.2/rpmfluff/rpmbuild.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1532 2021-01-05 12:37:29.107099 rpmfluff-0.6.2/rpmfluff/samples.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2367 2021-01-05 12:37:29.107099 rpmfluff-0.6.2/rpmfluff/sourcefile.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3746 2021-01-05 12:37:29.107099 rpmfluff-0.6.2/rpmfluff/subpackage.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1443 2021-01-05 12:37:29.107099 rpmfluff-0.6.2/rpmfluff/tarball.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    35785 2021-01-05 12:37:29.108099 rpmfluff-0.6.2/rpmfluff/test.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2142 2021-01-05 12:37:29.108099 rpmfluff-0.6.2/rpmfluff/trigger.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2496 2021-01-05 12:37:29.108099 rpmfluff-0.6.2/rpmfluff/utils.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2035 2021-01-05 12:37:29.108099 rpmfluff-0.6.2/rpmfluff/yumrepobuild.py
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2022-10-18 20:10:23.177768 rpmfluff-0.6.2/rpmfluff.egg-info/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      634 2022-10-18 20:10:23.000000 rpmfluff-0.6.2/rpmfluff.egg-info/PKG-INFO
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      430 2022-10-18 20:10:23.000000 rpmfluff-0.6.2/rpmfluff.egg-info/SOURCES.txt
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)        1 2022-10-18 20:10:23.000000 rpmfluff-0.6.2/rpmfluff.egg-info/dependency_links.txt
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)        9 2022-10-18 20:10:23.000000 rpmfluff-0.6.2/rpmfluff.egg-info/top_level.txt
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)       38 2022-10-18 20:10:23.177768 rpmfluff-0.6.2/setup.cfg
--rwxr-xr-x   0 jhutar    (1000) jhutar    (1000)     1052 2022-10-18 19:55:45.828165 rpmfluff-0.6.2/setup.py
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 07:07:43.386618 rpmfluff-0.6.3/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    17987 2021-01-05 12:37:29.105099 rpmfluff-0.6.3/LICENSE
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)       47 2021-01-05 12:37:29.000000 rpmfluff-0.6.3/MANIFEST.in
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      614 2023-07-17 07:07:43.385618 rpmfluff-0.6.3/PKG-INFO
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1358 2022-10-19 05:50:02.408222 rpmfluff-0.6.3/README-releng
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     5120 2023-07-17 07:03:42.000000 rpmfluff-0.6.3/README.md
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6585 2023-07-17 06:59:41.593272 rpmfluff-0.6.3/python-rpmfluff.spec
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 06:56:37.285992 rpmfluff-0.6.3/rpmfluff/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1647 2021-01-05 12:37:29.106099 rpmfluff-0.6.3/rpmfluff/__init__.py
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 06:57:08.651209 rpmfluff-0.6.3/rpmfluff/__pycache__/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1225 2022-10-18 19:54:34.604954 rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1616 2023-07-17 06:57:08.629209 rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1223 2021-01-05 12:38:12.023582 rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6130 2022-10-18 19:54:34.618954 rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    10140 2023-07-17 06:57:08.636209 rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6616 2021-01-05 12:40:17.266990 rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1719 2022-10-18 19:54:34.625954 rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2390 2023-07-17 06:57:08.641209 rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1736 2021-01-05 12:40:17.272990 rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    26585 2022-10-18 19:54:34.631954 rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    47157 2023-07-17 06:57:08.644209 rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    26981 2021-01-05 12:55:19.922105 rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      934 2022-10-18 19:54:34.633954 rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      974 2023-07-17 06:57:08.646209 rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      932 2021-01-05 12:40:17.277990 rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2254 2022-10-18 19:54:34.633954 rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3748 2023-07-17 06:57:08.646209 rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2340 2021-01-05 12:40:17.278990 rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4018 2022-10-18 19:54:34.634954 rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     5546 2023-07-17 06:57:08.647209 rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4264 2021-01-05 12:40:17.278990 rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      981 2022-10-18 19:54:34.634954 rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1587 2023-07-17 06:57:08.647209 rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      977 2021-01-05 12:40:17.279990 rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    28331 2022-10-18 19:54:34.639954 rpmfluff-0.6.3/rpmfluff/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    62177 2023-07-17 06:57:08.651209 rpmfluff-0.6.3/rpmfluff/__pycache__/test.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1640 2022-10-18 19:54:34.635954 rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2254 2023-07-17 06:57:08.647209 rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1636 2021-01-05 12:40:17.279990 rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1763 2022-10-18 19:54:34.619954 rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3065 2023-07-17 06:57:08.637209 rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1777 2021-01-05 12:40:17.266990 rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1350 2022-10-18 19:54:34.640954 rpmfluff-0.6.3/rpmfluff/__pycache__/yumrepobuild.cpython-310.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2221 2023-07-17 06:57:08.651209 rpmfluff-0.6.3/rpmfluff/__pycache__/yumrepobuild.cpython-311.pyc
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6451 2021-01-05 12:37:29.106099 rpmfluff-0.6.3/rpmfluff/check.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2109 2021-01-05 12:37:29.106099 rpmfluff-0.6.3/rpmfluff/make.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    32286 2021-01-05 12:47:10.829641 rpmfluff-0.6.3/rpmfluff/rpmbuild.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1532 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/samples.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2367 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/sourcefile.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3746 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/subpackage.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1443 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/tarball.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    35573 2023-07-17 06:56:37.285992 rpmfluff-0.6.3/rpmfluff/test.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2142 2021-01-05 12:37:29.108099 rpmfluff-0.6.3/rpmfluff/trigger.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2496 2021-01-05 12:37:29.108099 rpmfluff-0.6.3/rpmfluff/utils.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2035 2021-01-05 12:37:29.108099 rpmfluff-0.6.3/rpmfluff/yumrepobuild.py
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 07:07:43.385618 rpmfluff-0.6.3/rpmfluff.egg-info/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      614 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/PKG-INFO
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      430 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)        1 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)        9 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/top_level.txt
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)       38 2023-07-17 07:07:43.386618 rpmfluff-0.6.3/setup.cfg
+-rwxr-xr-x   0 jhutar    (1000) jhutar    (1000)     1052 2022-10-18 19:55:45.828165 rpmfluff-0.6.3/setup.py
```

### Comparing `rpmfluff-0.6.2/LICENSE` & `rpmfluff-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/PKG-INFO` & `rpmfluff-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: rpmfluff
-Version: 0.6.2
+Version: 0.6.3
 Summary: Lightweight way of building RPMs, and sabotaging them
 Home-page: https://pagure.io/rpmfluff
 Author: David Malcolm
 Author-email: dmalcolm@redhat.com
 Maintainer: Jan Hutar
 Maintainer-email: jhutar@redhat.com
 License: GPL-2.0+
-Platform: UNKNOWN
 License-File: LICENSE
 
 
 rpmfluff provides a python library for building RPM packages, and
 sabotaging them so they are broken in controlled ways.
 
 It is intended for use when validating package analysis tools such as RPM lint.
 It can also be used to construct test cases for package management software
 such as RPM, YUM, and DNF.
-
-
```

### Comparing `rpmfluff-0.6.2/README-releng` & `rpmfluff-0.6.3/README-releng`

 * *Files 24% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 twine upload dist/rpmfluff-....tar.gz
 
 # Now Fedora process
 kinit <FAS_username>@FEDORAPROJECT.ORG
 
 # Build rawhide package
 cd ../python-rpmfluff   # Fedora build
-fedpkg switch-branch master
+fedpkg switch-branch rawhide
 fedpkg pull --rebase
 fedpkg new-sources "../rpmfluff/rpmfluff-<version>.tar.xz"
 meld ../rpmfluff/python-rpmfluff.spec python-rpmfluff.spec
 fedpkg commit
 fedpkg push
 fedpkg build
 
 fedpkg switch-branch f25
-git merge master
+git merge rawhide
 fedpkg push
 fedpkg build
 fedpkg update
```

### Comparing `rpmfluff-0.6.2/README.md` & `rpmfluff-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Author: dmalcolm@redhat.com
 
 Homepage: https://pagure.io/rpmfluff
 
 ## News ##
 
+ * 2023-07-17: Remove usage of deprecated rpm.fi by gotmax23 - thanks!
  * 2022-10-18: Change deprecated distutils to setuptools
  * 2020-08-07: Structural changes by msuchy and lots of fixes and improvements by msuchy, dcantrell and tbaeder - thanks!
  * 2019-05-10: Mostly fixes related to rpm changes, thanks ksrot and bcl!
  * 2019-01-31: Fix and new/improved functionality from David Shea (man pages, images, subpackage scriptlets and symlinks properties), thank you!
  * 2018-07-22: BTW we are in pip now, try `pip install rpmfluff`, but fixed small issue with tests for `python3-rpm-4.14.2-0.rc1.1.fc29.2.x86_64` compatibility
  * 2018-02-23: Small fix for Rawhide and executable ELF files - see https://bugzilla.redhat.com/show_bug.cgi?id=1544361
  * 2017-06-28: New minor release of 0.5.3 version, also buch of other versions from last year not included below, oops
@@ -32,14 +33,15 @@
  * 2008-09-08: Fixed 2 small issues and created 0.2-2 version
  * 2008-09-08: Commited new big bunch of changes by David Malcolm and released version 0.2
  * 2008-07-11: Package renamed to python-rpmfluff, now works on the F9, some more changes
  * 2008-07-08: Initial commit of David Malcolm's code from former Table Cloth project
 
 ## Releases ##
 
+ * [rpmfluff-0.6.3.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.6.3.tar.xz) (MD5: `f62f0e54f1eae70dd0d9926eed0892cb`)
  * [rpmfluff-0.6.2.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.6.2.tar.xz) (MD5: `be164a407b3ae8c3239c5b9352b946fc`)
  * [rpmfluff-0.5.5.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.5.5.tar.xz) (MD5: `03ed0d57ab059aa4a3dd5182ae77473c`)
  * [rpmfluff-0.5.4.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.5.4.tar.xz) (MD5: `dc15e98f125e1a46e47648ff38f627d3`)
  * [rpmfluff-0.5.3.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.5.3.tar.xz) (MD5: `ae0a846c239a60b71bbbcf4e2c84be72`)
  * [rpmfluff-0.4.2.tar.bz2](https://fedorahosted.org/releases/r/p/rpmfluff/rpmfluff-0.4.2.tar.bz2) (MD5: `e8f4e9607128a2817262761592eb8080`) - [python-rpmfluff-0.4.2-1.fc22.src.rpm](https://fedorahosted.org/releases/r/p/rpmfluff/python-rpmfluff-0.4.2-1.fc22.src.rpm)
  * [rpmfluff-0.4.1.tar.bz2](https://fedorahosted.org/releases/r/p/rpmfluff/rpmfluff-0.4.1.tar.bz2) (MD5: `752be6d7ece44535392583c18e007a2e`) - [python-rpmfluff-0.4.1-1.fc22.src.rpm](https://fedorahosted.org/releases/r/p/rpmfluff/python-rpmfluff-0.4.1-1.fc22.src.rpm)
  * [rpmfluff-0.3.tar.bz2](https://fedorahosted.org/releases/r/p/rpmfluff/rpmfluff-0.3.tar.bz2) (MD5: `296472d772ee0cc04e9d9afd35880fd1`) - [python-rpmfluff-0.3-5.fc12.src.rpm](https://fedorahosted.org/releases/r/p/rpmfluff/python-rpmfluff-0.3-5.fc12.src.rpm)
```

### Comparing `rpmfluff-0.6.2/python-rpmfluff.spec` & `rpmfluff-0.6.3/python-rpmfluff.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 %global modname rpmfluff
 
 Name:          python-%{modname}
-Version:       0.6.2
+Version:       0.6.3
 Release:       1%{?dist}
 Summary:       Lightweight way of building RPMs, and sabotaging them
 
 License:       GPLv2+
 URL:           https://pagure.io/rpmfluff
 Source0:       https://pagure.io/releases/%{modname}/%{modname}-%{version}.tar.xz
 
@@ -17,15 +17,14 @@
 \
 It is intended for use when validating package analysis tools such as RPM lint.\
 It can also be used to construct test cases for package management software\
 such as RPM, YUM, and DNF.
 
 %description %{_description}
 
-
 %package -n python3-%{modname}
 Summary:        %{summary}
 %{?python_provide:%python_provide python3-%{modname}}
 BuildRequires:  gcc
 BuildRequires:  python3-devel
 BuildRequires:  python3-rpm
 BuildRequires:  python3-setuptools
@@ -44,21 +43,26 @@
 
 %install
 %py3_install
 
 %check
 python3 -m unittest %{modname}.test
 
-
 %files -n python3-%{modname}
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/*
 
 %changelog
+* Mon Jul 17 2023 Jan Hutar <jhutar@redhat.com> - 0.6.3-1
+- gotmax23: remove usage of deprecated rpm.fi
+
+* Tue Oct 18 2022 Jan Hutar <jhutar@redhat.com> - 0.6.2-1
+- Change deprecated distutils to setuptools
+
 * Wed Aug 12 2020 Jan Hutar <jhutar@redhat.com> - 0.6.1-1
 - jhutar: Expose two more items
 
 * Fri Aug 07 2020 Jan Hutar <jhutar@redhat.com> - 0.6-1
 - jhutar: Workaround for https://github.com/rpm-software-management/rpm/issues/1301
 - msuchy: Do not write %clean by default
 - msuchy: Make build directory in /tmp
```

### Comparing `rpmfluff-0.6.2/rpmfluff/__init__.py` & `rpmfluff-0.6.3/rpmfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/__init__.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/__init__.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/check.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/check.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/make.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/make.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/rpmbuild.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/rpmbuild.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/samples.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/samples.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/sourcefile.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/sourcefile.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/subpackage.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/subpackage.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/tarball.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/tarball.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/test.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/trigger.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/trigger.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/utils.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/utils.cpython-39.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/__pycache__/yumrepobuild.cpython-310.pyc` & `rpmfluff-0.6.3/rpmfluff/__pycache__/yumrepobuild.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/check.py` & `rpmfluff-0.6.3/rpmfluff/check.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/make.py` & `rpmfluff-0.6.3/rpmfluff/make.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/rpmbuild.py` & `rpmfluff-0.6.3/rpmfluff/rpmbuild.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/samples.py` & `rpmfluff-0.6.3/rpmfluff/samples.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/sourcefile.py` & `rpmfluff-0.6.3/rpmfluff/sourcefile.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/subpackage.py` & `rpmfluff-0.6.3/rpmfluff/subpackage.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/tarball.py` & `rpmfluff-0.6.3/rpmfluff/tarball.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/test.py` & `rpmfluff-0.6.3/rpmfluff/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -525,79 +525,78 @@
         rpmsDir = self.rpmbuild.get_rpms_dir()
         self.assert_is_dir(rpmsDir)
 
         for arch in [expectedArch]:
             # FIXME: sort out architecture properly
             rpmFile = self.rpmbuild.get_built_rpm(arch)
             h = get_rpm_header(rpmFile)
-            files = list(h.fiFromHeader())
+            files = list(rpm.files(h))
             self.assertEqual(1, len(files))
-            (filename, _size, mode, _mtime, _flags, _rdev, _inode, _FNlink, _Fstate, _vflags, _user, _group, _md5sum) = files[0]
-            self.assertEqual("/var/spool/foo", filename)
-            self.assertEqual(0o041777, mode)
+            self.assertEqual("/var/spool/foo", files[0].name)
+            self.assertEqual(0o041777, files[0].mode)
 
     def test_installed_symlink(self):
         self.rpmbuild.add_installed_symlink("foo", "bar")
         self.rpmbuild.make()
 
         rpmsDir = self.rpmbuild.get_rpms_dir()
         self.assert_is_dir(rpmsDir)
 
         for arch in [expectedArch]:
             # FIXME: sort out architecture properly
             rpmFile = self.rpmbuild.get_built_rpm(arch)
             h = get_rpm_header(rpmFile)
-            files = list(h.fiFromHeader())
+            files = list(rpm.files(h))
             self.assertEqual(1, len(files))
-            self.assertEqual("/foo", files[0][0])
+            self.assertEqual("/foo", files[0].name)
 
     def test_config_symlink(self):
         self.rpmbuild.add_installed_symlink("foo", "bar", isConfig=True)
         self.rpmbuild.make()
 
         rpmsDir = self.rpmbuild.get_rpms_dir()
         self.assert_is_dir(rpmsDir)
 
         for arch in [expectedArch]:
             # FIXME: sort out architecture properly
             rpmFile = self.rpmbuild.get_built_rpm(arch)
             h = get_rpm_header(rpmFile)
-            files = list(h.fiFromHeader())
+            files = list(rpm.files(h))
             self.assertEqual(1, len(files))
-            self.assertEqual("/foo", files[0][0])
+            self.assertEqual("/foo", files[0].name)
 
     def test_doc_symlink(self):
         self.rpmbuild.add_installed_symlink("foo", "bar", isDoc=True)
         self.rpmbuild.make()
 
         rpmsDir = self.rpmbuild.get_rpms_dir()
         self.assert_is_dir(rpmsDir)
 
         for arch in [expectedArch]:
             # FIXME: sort out architecture properly
             rpmFile = self.rpmbuild.get_built_rpm(arch)
             h = get_rpm_header(rpmFile)
-            files = list(h.fiFromHeader())
+            files = list(rpm.files(h))
             self.assertEqual(1, len(files))
-            self.assertEqual("/foo", files[0][0])
+            self.assertEqual("/foo", files[0].name)
 
     def test_ghost_symlink(self):
         self.rpmbuild.add_installed_symlink("foo", "bar", isGhost=True)
         self.rpmbuild.make()
 
         rpmsDir = self.rpmbuild.get_rpms_dir()
         self.assert_is_dir(rpmsDir)
 
         for arch in [expectedArch]:
             # FIXME: sort out architecture properly
             rpmFile = self.rpmbuild.get_built_rpm(arch)
             h = get_rpm_header(rpmFile)
-            files = list(h.fiFromHeader())
+            files = list(rpm.files(h))
             self.assertEqual(1, len(files))
-            self.assertEqual("/foo", files[0][0])
+            self.assertEqual("/foo", files[0].name)
 
     def test_fake_virus(self):
         """Ensure that adding a fake virus works as expected"""
         self.rpmbuild.add_fake_virus('fake-virus-infectee.exe', 'fake-virus-infectee.exe')
         self.rpmbuild.make()
 
     def test_debuginfo_generation(self):
@@ -631,23 +630,23 @@
                      'host arch is not x86_64 or 32-bit support is missing')
     def test_multiarch_compilation(self):
         """Ensure that building on multiple archs works as expected"""
         self.rpmbuild.buildArchs = ['i386', 'x86_64']
         self.rpmbuild.add_simple_compilation(installPath='/usr/bin/program')
         self.rpmbuild.make()
         hdr = self.rpmbuild.get_built_rpm_header('i386')
-        fi = hdr.fiFromHeader()
-        next(fi)
-        self.assertEqual('/usr/bin/program', fi.FN())
-        self.assertEqual(1, fi.FColor())
+        files = rpm.files(hdr)
+        file = next(files)
+        self.assertEqual('/usr/bin/program', file.name)
+        self.assertEqual(1, file.color)
         hdr = self.rpmbuild.get_built_rpm_header('x86_64')
-        fi = hdr.fiFromHeader()
-        next(fi)
-        self.assertEqual('/usr/bin/program', fi.FN())
-        self.assertEqual(2, fi.FColor())
+        files = rpm.files(hdr)
+        file = next(files)
+        self.assertEqual('/usr/bin/program', file.name)
+        self.assertEqual(2, file.color)
 
     def test_multilib_conflict(self):
         """Ensure that the hooks to create a multilib conflict work as expected"""
         self.rpmbuild.add_multilib_conflict()
         self.rpmbuild.make()
 
     def test_build_warning(self):
@@ -696,20 +695,19 @@
 
     def test_add_file_with_owner_and_group(self):
         self.rpmbuild.add_installed_file('/var/www/html/index.html',
                 SourceFile('index.html', '<p>Hello</p>'),
                 owner='apache', group='apache')
         self.rpmbuild.make()
         hdr = self.rpmbuild.get_built_rpm_header(expectedArch)
-        files = list(hdr.fiFromHeader())
+        files = list(rpm.files(hdr))
         self.assertEqual(1, len(files))
-        (filename, _size, _mode, _mtime, _flags, _rdev, _inode, _FNlink, _Fstate, _vflags, user, group, _md5sum) = files[0]
-        self.assertEqual('/var/www/html/index.html', filename)
-        self.assertEqual('apache', user)
-        self.assertEqual('apache', group)
+        self.assertEqual('/var/www/html/index.html', files[0].name)
+        self.assertEqual('apache', files[0].user)
+        self.assertEqual('apache', files[0].group)
 
     def test_specfile_encoding_utf8(self):
         self.rpmbuild.section_changelog = "* Fri Mar 30 2001 Trond Eivind Glomsr\\u00F8d <teg@redhat.com>\nDo something"
         self.rpmbuild.make()
 
     def test_specfile_encoding_iso8859(self):
         self.rpmbuild.specfileEncoding = 'iso8859_10'
```

### Comparing `rpmfluff-0.6.2/rpmfluff/trigger.py` & `rpmfluff-0.6.3/rpmfluff/trigger.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/utils.py` & `rpmfluff-0.6.3/rpmfluff/utils.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff/yumrepobuild.py` & `rpmfluff-0.6.3/rpmfluff/yumrepobuild.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.2/rpmfluff.egg-info/PKG-INFO` & `rpmfluff-0.6.3/rpmfluff.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: rpmfluff
-Version: 0.6.2
+Version: 0.6.3
 Summary: Lightweight way of building RPMs, and sabotaging them
 Home-page: https://pagure.io/rpmfluff
 Author: David Malcolm
 Author-email: dmalcolm@redhat.com
 Maintainer: Jan Hutar
 Maintainer-email: jhutar@redhat.com
 License: GPL-2.0+
-Platform: UNKNOWN
 License-File: LICENSE
 
 
 rpmfluff provides a python library for building RPM packages, and
 sabotaging them so they are broken in controlled ways.
 
 It is intended for use when validating package analysis tools such as RPM lint.
 It can also be used to construct test cases for package management software
 such as RPM, YUM, and DNF.
-
-
```

### Comparing `rpmfluff-0.6.2/setup.py` & `rpmfluff-0.6.3/setup.py`

 * *Files identical despite different names*

