# Comparing `tmp/distlib-0.3.6.tar.gz` & `tmp/distlib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/disk2/vinay/projects/distlib/dist/tmpzzabix5t/distlib-0.3.6.tar", last modified: Fri Aug 26 09:31:09 2022, max compression
+gzip compressed data, was "/disk2/vinay/projects/distlib/dist/tmpndf75hlu/distlib-0.3.7.tar", last modified: Mon Jul 17 10:09:03 2023, max compression
```

## Comparing `distlib-0.3.6.tar` & `distlib-0.3.7.tar`

### file list

```diff
@@ -1,213 +1,214 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/PC/
--rw-r--r--   0 vinay     (1000) vinay     (1000)    11846 2019-10-28 11:05:52.000000 distlib-0.3.6/PC/CLISimpleLauncher.vcxproj
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    33362 2022-08-06 08:15:08.000000 distlib-0.3.6/PC/launcher.c
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2012 2019-04-09 07:00:51.000000 distlib-0.3.6/PC/ReadMe.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)    10991 2019-10-28 11:05:52.000000 distlib-0.3.6/PC/GUISimpleLauncher.vcxproj
--rw-r--r--   0 vinay     (1000) vinay     (1000)    19790 2019-04-09 07:00:51.000000 distlib-0.3.6/PC/launcher.ico
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2026 2019-10-28 11:05:52.000000 distlib-0.3.6/PC/SimpleLauncher.sln
--rw-r--r--   0 vinay     (1000) vinay     (1000)       84 2019-04-09 07:00:51.000000 distlib-0.3.6/PC/launcher.rc
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1645 2019-04-09 07:00:51.000000 distlib-0.3.6/CONTRIBUTORS.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/distlib.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     5581 2022-08-26 09:31:08.000000 distlib-0.3.6/distlib.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        8 2022-08-26 09:31:08.000000 distlib-0.3.6/distlib.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     5112 2022-08-26 09:31:08.000000 distlib-0.3.6/distlib.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2022-08-26 09:31:08.000000 distlib-0.3.6/distlib.egg-info/dependency_links.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      254 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bad.tar.bz2
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testsrc/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       32 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/.hidden
--rw-r--r--   0 vinay     (1000) vinay     (1000)       14 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/LICENSE
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testsrc/subdir/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testsrc/subdir/subsubdir/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/subdir/subsubdir/somedata.bin
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testsrc/subdir/lose/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       35 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/subdir/lose/lose.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/subdir/somedata.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testsrc/keep/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       33 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/keep/keep.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)       44 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testsrc/README.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/scripts/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       94 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/foo.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       16 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script4.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       42 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script8.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       24 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script2.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       30 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script3.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       18 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/shell.sh
--rw-r--r--   0 vinay     (1000) vinay     (1000)       97 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script7.pyw
--rw-r--r--   0 vinay     (1000) vinay     (1000)      172 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script6.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       31 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script5.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       32 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/script1.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1000 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/scripts/uwsgi_part
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testdist-0.1/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      540 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testdist-0.1/package.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)      950 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testdist-0.1/LICENSE
--rw-r--r--   0 vinay     (1000) vinay     (1000)      186 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testdist-0.1/testdist.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      448 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testdist-0.1/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)       46 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testdist-0.1/README.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/testdist-0.1/doc/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      153 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/testdist-0.1/doc/index.html
--rw-r--r--   0 vinay     (1000) vinay     (1000)      739 2021-12-08 09:17:19.000000 distlib-0.3.6/tests/compat.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     8018 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/minimext-0.1-cp33-cp33m-linux_x86_64.whl
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    26206 2021-12-12 19:18:32.000000 distlib-0.3.6/tests/test_locators.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      247 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bad.tar.gz
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_archives/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/coverage-3.5.2.tar.gz
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/coverage-3.4b2.tar.gz
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_archives/subdir/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_archives/subdir/subsubdir/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/subdir/subsubdir/Flask-0.9.tar.gz
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/subdir/subsubdir/Django-1.4.1.tar.gz
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/subdir/config-0.3.7-py27-none-any.whl
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/subdir/python-gnupg-0.2.9.tar.gz
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_archives/coverage-3.3.1.tar.gz
--rw-r--r--   0 vinay     (1000) vinay     (1000)       14 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/good.bin
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2205 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/dummy-0.1-py27-none-any.whl
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/keys/
--rw-------   0 vinay     (1000) vinay     (1000)      600 2020-01-10 14:27:00.000000 distlib-0.3.6/tests/keys/random_seed
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/keys/private-keys-v1.d/
--rw-------   0 vinay     (1000) vinay     (1000)     1417 2019-05-11 07:36:52.000000 distlib-0.3.6/tests/keys/private-keys-v1.d/8BE462CC6083085304DBEA3FC423A1276DAF0B2C.key
--rw-------   0 vinay     (1000) vinay     (1000)     1174 2019-05-13 14:46:52.000000 distlib-0.3.6/tests/keys/private-keys-v1.d/89643D011E83504EFB6A88F328153504C3E2C97B.key
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1280 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/keys/trustdb.gpg
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1208 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/keys/pubring.gpg
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-05-11 07:36:52.000000 distlib-0.3.6/tests/keys/.gpg-v21-migrated
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2586 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/keys/secring.gpg
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2909 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/test_testdist-0.1.zip
--rw-r--r--   0 vinay     (1000) vinay     (1000)       35 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/included.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)     8071 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/minimext-0.1-cp32-cp32mu-linux_x86_64.whl
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:09.000000 distlib-0.3.6/tests/test_testdist-0.1/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      673 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/test_testdist-0.1/package.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)      950 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/test_testdist-0.1/LICENSE
--rw-r--r--   0 vinay     (1000) vinay     (1000)      186 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/test_testdist-0.1/testdist.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      436 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/test_testdist-0.1/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)       46 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/test_testdist-0.1/README.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    19054 2022-05-09 09:12:31.000000 distlib-0.3.6/tests/test_scripts.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    10097 2021-08-22 10:10:52.000000 distlib-0.3.6/tests/test_resources.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     8819 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/SETUPTOOLS-PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1890 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/pydist.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)      287 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/good.bin.asc
--rw-r--r--   0 vinay     (1000) vinay     (1000)      993 2021-12-08 07:38:57.000000 distlib-0.3.6/tests/distlib_tests.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    32021 2022-07-09 11:35:28.000000 distlib-0.3.6/tests/test_wheel.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     8678 2020-09-18 10:48:43.000000 distlib-0.3.6/tests/test_manifest.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      217 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/good.tar.bz2
--rw-r--r--   0 vinay     (1000) vinay     (1000)       13 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bad.bin
--rw-r--r--   0 vinay     (1000) vinay     (1000)     3877 2021-12-08 09:58:39.000000 distlib-0.3.6/tests/test_markers.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    10240 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bad.tar
--rw-r--r--   0 vinay     (1000) vinay     (1000)    40939 2022-05-09 06:33:19.000000 distlib-0.3.6/tests/test_util.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      964 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bad.zip
--rw-r--r--   0 vinay     (1000) vinay     (1000)      812 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/good.zip
--rw-r--r--   0 vinay     (1000) vinay     (1000)    42450 2020-09-18 10:49:35.000000 distlib-0.3.6/tests/test_database.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      210 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/good.tar.gz
--rw-r--r--   0 vinay     (1000) vinay     (1000)      960 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bar.zip
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       50 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/truffles-5.0.egg-info
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar.png
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9/choxie/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       24 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9/choxie/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      214 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9/choxie/chocolate.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      111 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9/truffles.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/REQUESTED
--rw-r--r--   0 vinay     (1000) vinay     (1000)      365 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/pydist-exports.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/RECORD
--rw-r--r--   0 vinay     (1000) vinay     (1000)      348 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/pydist.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/INSTALLER
--rw-r--r--   0 vinay     (1000) vinay     (1000)      185 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1.dist-info/METADATA
--rw-r--r--   0 vinay     (1000) vinay     (1000)        6 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar.cfg
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1402 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/strawberry-0.6.egg
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/REQUESTED
--rw-r--r--   0 vinay     (1000) vinay     (1000)      367 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/pydist-exports.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/RECORD
--rw-r--r--   0 vinay     (1000) vinay     (1000)      223 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/pydist.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/INSTALLER
--rw-r--r--   0 vinay     (1000) vinay     (1000)       39 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/RESOURCES
--rw-r--r--   0 vinay     (1000) vinay     (1000)       65 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/babar-0.1.dist-info/METADATA
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/REQUESTED
--rw-r--r--   0 vinay     (1000) vinay     (1000)      319 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/pydist-exports.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/RECORD
--rw-r--r--   0 vinay     (1000) vinay     (1000)      476 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/pydist.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/INSTALLER
--rw-r--r--   0 vinay     (1000) vinay     (1000)      300 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/choxie-2.0.0.9.dist-info/METADATA
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/SOURCES.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)       72 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/requires.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)       17 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/top_level.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)        1 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/not-zip-safe
--rw-r--r--   0 vinay     (1000) vinay     (1000)       37 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)      568 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)        1 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/dependency_links.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/coconuts-aster-10.3.egg-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      117 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/coconuts-aster-10.3.egg-info/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)       54 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/nut-funkyversion.egg-info
--rw-r--r--   0 vinay     (1000) vinay     (1000)      121 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/cheese-2.0.2.egg-info
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1/towel_stuff/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      481 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/towel_stuff-0.1/towel_stuff/__init__.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4.dist-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4.dist-info/REQUESTED
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4.dist-info/RECORD
--rw-r--r--   0 vinay     (1000) vinay     (1000)      323 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4.dist-info/pydist.json
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4.dist-info/INSTALLER
--rw-r--r--   0 vinay     (1000) vinay     (1000)      107 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4.dist-info/METADATA
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/bacon-0.1.egg-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       84 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/bacon-0.1.egg-info/installed-files.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)      143 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/bacon-0.1.egg-info/PKG-INFO
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4/grammar/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       24 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4/grammar/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      162 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/fake_dists/grammar-1.0a4/grammar/utils.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    10240 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/good.tar
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    14596 2021-12-18 14:23:15.000000 distlib-0.3.6/tests/test_index.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     7991 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/minimext-0.1-cp27-none-linux_x86_64.whl
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3136 2021-01-12 17:16:02.000000 distlib-0.3.6/tests/keycert.pem
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1992 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1270 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/LONG_DESC.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    26591 2021-12-14 19:32:34.000000 distlib-0.3.6/tests/test_metadata.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    23162 2021-12-14 20:01:59.000000 distlib-0.3.6/tests/test_version.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1234 2022-05-09 08:06:26.000000 distlib-0.3.6/tests/test_all.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      891 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foo.zip
--rw-r--r--   0 vinay     (1000) vinay     (1000)     9720 2021-08-22 09:58:28.000000 distlib-0.3.6/tests/support.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1827 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/valid_wheel-0.0.1-py3-none-any.whl
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/foofoo/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/foofoo/bar/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        8 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foofoo/bar/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       14 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foofoo/bar/baz.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)        5 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foofoo/bar/bar_resource.bin
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/foofoo/nested/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       12 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foofoo/nested/nested_resource.bin
--rw-r--r--   0 vinay     (1000) vinay     (1000)        8 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foofoo/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       10 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/foofoo/foo_resource.bin
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/tests/bad_wheels/
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1248 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/bad_wheels/dummy-0.1-py27-none-any.whl
--rw-r--r--   0 vinay     (1000) vinay     (1000)     8840 2019-04-09 07:00:51.000000 distlib-0.3.6/tests/SETUPTOOLS-PKG-INFO2
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1213 2022-08-26 09:31:09.000000 distlib-0.3.6/setup.cfg
--rw-r--r--   0 vinay     (1000) vinay     (1000)    14531 2019-04-09 07:00:51.000000 distlib-0.3.6/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     5112 2022-08-26 09:31:09.000000 distlib-0.3.6/PKG-INFO
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-26 09:31:08.000000 distlib-0.3.6/distlib/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    39801 2021-12-15 10:35:33.000000 distlib-0.3.6/distlib/metadata.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    41259 2021-12-08 09:27:42.000000 distlib-0.3.6/distlib/compat.py
--rw-------   0 vinay     (1000) vinay     (1000)    97792 2022-08-06 08:15:40.000000 distlib-0.3.6/distlib/t32.exe
--rw-------   0 vinay     (1000) vinay     (1000)   108032 2022-08-06 08:15:40.000000 distlib-0.3.6/distlib/t64.exe
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    51697 2022-07-09 17:24:37.000000 distlib-0.3.6/distlib/database.py
--rw-------   0 vinay     (1000) vinay     (1000)   101888 2022-08-06 08:15:40.000000 distlib-0.3.6/distlib/w64.exe
--rw-------   0 vinay     (1000) vinay     (1000)    91648 2022-08-06 08:15:40.000000 distlib-0.3.6/distlib/w32.exe
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    18102 2022-05-06 08:38:13.000000 distlib-0.3.6/distlib/scripts.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     5058 2021-12-08 10:51:43.000000 distlib-0.3.6/distlib/markers.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      581 2022-08-26 09:05:41.000000 distlib-0.3.6/distlib/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    43898 2022-07-09 10:47:57.000000 distlib-0.3.6/distlib/wheel.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    10820 2021-05-29 05:35:47.000000 distlib-0.3.6/distlib/resources.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    66262 2021-12-08 09:34:52.000000 distlib-0.3.6/distlib/util.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)   182784 2022-08-06 08:15:40.000000 distlib-0.3.6/distlib/t64-arm.exe
--rw-r--r--   0 vinay     (1000) vinay     (1000)   168448 2022-08-06 08:15:40.000000 distlib-0.3.6/distlib/w64-arm.exe
--rw-r--r--   0 vinay     (1000) vinay     (1000)    23513 2021-09-21 10:06:14.000000 distlib-0.3.6/distlib/version.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    20834 2021-12-18 14:21:28.000000 distlib-0.3.6/distlib/index.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)    14811 2019-04-09 07:00:51.000000 distlib-0.3.6/distlib/manifest.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    51991 2021-12-14 20:05:07.000000 distlib-0.3.6/distlib/locators.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    24738 2022-08-04 19:09:24.000000 distlib-0.3.6/CHANGES.rst
--rw-r--r--   0 vinay     (1000) vinay     (1000)      265 2021-12-08 07:46:10.000000 distlib-0.3.6/MANIFEST.in
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      117 2022-05-09 07:58:27.000000 distlib-0.3.6/pyproject.toml
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3897 2022-07-14 07:51:11.000000 distlib-0.3.6/README.rst
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/PC/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    11846 2019-10-28 11:05:52.000000 distlib-0.3.7/PC/CLISimpleLauncher.vcxproj
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    33362 2022-08-06 08:15:08.000000 distlib-0.3.7/PC/launcher.c
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2012 2019-04-09 07:00:51.000000 distlib-0.3.7/PC/ReadMe.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    10991 2019-10-28 11:05:52.000000 distlib-0.3.7/PC/GUISimpleLauncher.vcxproj
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    19790 2019-04-09 07:00:51.000000 distlib-0.3.7/PC/launcher.ico
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2026 2019-10-28 11:05:52.000000 distlib-0.3.7/PC/SimpleLauncher.sln
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       84 2019-04-09 07:00:51.000000 distlib-0.3.7/PC/launcher.rc
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1645 2019-04-09 07:00:51.000000 distlib-0.3.7/CONTRIBUTORS.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/distlib.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     5599 2023-07-17 10:09:03.000000 distlib-0.3.7/distlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        8 2023-07-17 10:09:03.000000 distlib-0.3.7/distlib.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     5105 2023-07-17 10:09:03.000000 distlib-0.3.7/distlib.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-17 10:09:03.000000 distlib-0.3.7/distlib.egg-info/dependency_links.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      254 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bad.tar.bz2
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testsrc/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       32 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/.hidden
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       14 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/LICENSE
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testsrc/subdir/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testsrc/subdir/subsubdir/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/subdir/subsubdir/somedata.bin
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testsrc/subdir/lose/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       35 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/subdir/lose/lose.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/subdir/somedata.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testsrc/keep/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       33 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/keep/keep.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       44 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testsrc/README.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/scripts/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       94 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/foo.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       16 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script4.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       42 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script8.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       24 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script2.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       30 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script3.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       18 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/shell.sh
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       97 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script7.pyw
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      172 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script6.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       31 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script5.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       32 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/script1.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1000 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/scripts/uwsgi_part
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testdist-0.1/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      540 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testdist-0.1/package.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      950 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testdist-0.1/LICENSE
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      186 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testdist-0.1/testdist.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      448 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testdist-0.1/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       46 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testdist-0.1/README.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/testdist-0.1/doc/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      153 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/testdist-0.1/doc/index.html
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      739 2021-12-08 09:17:19.000000 distlib-0.3.7/tests/compat.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     8018 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/minimext-0.1-cp33-cp33m-linux_x86_64.whl
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    26273 2023-06-06 18:11:10.000000 distlib-0.3.7/tests/test_locators.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      247 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bad.tar.gz
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_archives/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/coverage-3.5.2.tar.gz
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/coverage-3.4b2.tar.gz
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_archives/subdir/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_archives/subdir/subsubdir/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/subdir/subsubdir/Flask-0.9.tar.gz
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/subdir/subsubdir/Django-1.4.1.tar.gz
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/subdir/config-0.3.7-py27-none-any.whl
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/subdir/python-gnupg-0.2.9.tar.gz
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_archives/coverage-3.3.1.tar.gz
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       14 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/good.bin
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2205 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/dummy-0.1-py27-none-any.whl
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/keys/
+-rw-------   0 vinay     (1000) vinay     (1000)      600 2020-01-10 14:27:00.000000 distlib-0.3.7/tests/keys/random_seed
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/keys/private-keys-v1.d/
+-rw-------   0 vinay     (1000) vinay     (1000)     1417 2019-05-11 07:36:52.000000 distlib-0.3.7/tests/keys/private-keys-v1.d/8BE462CC6083085304DBEA3FC423A1276DAF0B2C.key
+-rw-------   0 vinay     (1000) vinay     (1000)     1174 2019-05-13 14:46:52.000000 distlib-0.3.7/tests/keys/private-keys-v1.d/89643D011E83504EFB6A88F328153504C3E2C97B.key
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1280 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/keys/trustdb.gpg
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1208 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/keys/pubring.gpg
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-05-11 07:36:52.000000 distlib-0.3.7/tests/keys/.gpg-v21-migrated
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2586 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/keys/secring.gpg
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2909 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/test_testdist-0.1.zip
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       35 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/included.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     8071 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/minimext-0.1-cp32-cp32mu-linux_x86_64.whl
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/test_testdist-0.1/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      673 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/test_testdist-0.1/package.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      950 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/test_testdist-0.1/LICENSE
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      186 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/test_testdist-0.1/testdist.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      436 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/test_testdist-0.1/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       46 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/test_testdist-0.1/README.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    19054 2022-05-09 09:12:31.000000 distlib-0.3.7/tests/test_scripts.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    10097 2021-08-22 10:10:52.000000 distlib-0.3.7/tests/test_resources.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     8819 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/SETUPTOOLS-PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1890 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/pydist.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      287 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/good.bin.asc
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      993 2021-12-08 07:38:57.000000 distlib-0.3.7/tests/distlib_tests.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    32021 2022-07-09 11:35:28.000000 distlib-0.3.7/tests/test_wheel.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     8678 2020-09-18 10:48:43.000000 distlib-0.3.7/tests/test_manifest.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      217 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/good.tar.bz2
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       13 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bad.bin
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     4297 2022-10-31 20:08:22.000000 distlib-0.3.7/tests/test_markers.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    10240 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bad.tar
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    41491 2023-07-17 09:13:14.000000 distlib-0.3.7/tests/test_util.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      964 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bad.zip
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      812 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/good.zip
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    42501 2022-11-25 08:28:38.000000 distlib-0.3.7/tests/test_database.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      210 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/good.tar.gz
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      148 2023-06-30 17:40:43.000000 distlib-0.3.7/tests/evil.tar.gz
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      960 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bar.zip
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       50 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/truffles-5.0.egg-info
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar.png
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9/choxie/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       24 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9/choxie/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      214 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9/choxie/chocolate.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      111 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9/truffles.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/REQUESTED
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      365 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/pydist-exports.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/RECORD
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      348 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/pydist.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/INSTALLER
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      185 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1.dist-info/METADATA
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        6 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar.cfg
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1402 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/strawberry-0.6.egg
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/REQUESTED
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      367 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/pydist-exports.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/RECORD
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      223 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/pydist.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/INSTALLER
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       39 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/RESOURCES
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       65 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/babar-0.1.dist-info/METADATA
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/REQUESTED
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      319 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/pydist-exports.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/RECORD
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      476 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/pydist.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/INSTALLER
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      300 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/choxie-2.0.0.9.dist-info/METADATA
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/SOURCES.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       72 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/requires.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       17 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/top_level.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        1 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/not-zip-safe
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       37 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/entry_points.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      568 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        1 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/dependency_links.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/coconuts-aster-10.3.egg-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      117 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/coconuts-aster-10.3.egg-info/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       54 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/nut-funkyversion.egg-info
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      121 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/cheese-2.0.2.egg-info
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1/towel_stuff/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      481 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/towel_stuff-0.1/towel_stuff/__init__.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4.dist-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4.dist-info/REQUESTED
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4.dist-info/RECORD
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      323 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4.dist-info/pydist.json
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4.dist-info/INSTALLER
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      107 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4.dist-info/METADATA
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/bacon-0.1.egg-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       84 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/bacon-0.1.egg-info/installed-files.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      143 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/bacon-0.1.egg-info/PKG-INFO
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4/grammar/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       24 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4/grammar/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      162 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/fake_dists/grammar-1.0a4/grammar/utils.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    10240 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/good.tar
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    14746 2022-11-25 08:33:34.000000 distlib-0.3.7/tests/test_index.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     7991 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/minimext-0.1-cp27-none-linux_x86_64.whl
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3136 2021-01-12 17:16:02.000000 distlib-0.3.7/tests/keycert.pem
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1992 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1270 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/LONG_DESC.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    26591 2021-12-14 19:32:34.000000 distlib-0.3.7/tests/test_metadata.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    23770 2023-06-06 18:46:54.000000 distlib-0.3.7/tests/test_version.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1234 2022-05-09 08:06:26.000000 distlib-0.3.7/tests/test_all.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      891 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foo.zip
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     9720 2021-08-22 09:58:28.000000 distlib-0.3.7/tests/support.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1827 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/valid_wheel-0.0.1-py3-none-any.whl
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/foofoo/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/foofoo/bar/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        8 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foofoo/bar/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       14 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foofoo/bar/baz.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        5 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foofoo/bar/bar_resource.bin
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/foofoo/nested/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       12 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foofoo/nested/nested_resource.bin
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        8 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foofoo/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       10 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/foofoo/foo_resource.bin
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/tests/bad_wheels/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1248 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/bad_wheels/dummy-0.1-py27-none-any.whl
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     8840 2019-04-09 07:00:51.000000 distlib-0.3.7/tests/SETUPTOOLS-PKG-INFO2
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1207 2023-07-17 10:09:03.000000 distlib-0.3.7/setup.cfg
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    14531 2019-04-09 07:00:51.000000 distlib-0.3.7/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     5105 2023-07-17 10:09:03.000000 distlib-0.3.7/PKG-INFO
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-17 10:09:03.000000 distlib-0.3.7/distlib/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    39693 2022-11-25 07:18:53.000000 distlib-0.3.7/distlib/metadata.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    41259 2021-12-08 09:27:42.000000 distlib-0.3.7/distlib/compat.py
+-rw-------   0 vinay     (1000) vinay     (1000)    97792 2022-08-06 08:15:40.000000 distlib-0.3.7/distlib/t32.exe
+-rw-------   0 vinay     (1000) vinay     (1000)   108032 2022-08-06 08:15:40.000000 distlib-0.3.7/distlib/t64.exe
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    51910 2022-11-25 11:34:32.000000 distlib-0.3.7/distlib/database.py
+-rw-------   0 vinay     (1000) vinay     (1000)   101888 2022-08-06 08:15:40.000000 distlib-0.3.7/distlib/w64.exe
+-rw-------   0 vinay     (1000) vinay     (1000)    91648 2022-08-06 08:15:40.000000 distlib-0.3.7/distlib/w32.exe
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    18121 2022-11-07 08:11:10.000000 distlib-0.3.7/distlib/scripts.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     5159 2022-10-31 20:08:21.000000 distlib-0.3.7/distlib/markers.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      581 2023-07-17 10:02:46.000000 distlib-0.3.7/distlib/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    43898 2022-07-09 10:47:57.000000 distlib-0.3.7/distlib/wheel.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    10820 2021-05-29 05:35:47.000000 distlib-0.3.7/distlib/resources.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    66979 2023-07-17 09:34:54.000000 distlib-0.3.7/distlib/util.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)   182784 2022-08-06 08:15:40.000000 distlib-0.3.7/distlib/t64-arm.exe
+-rw-r--r--   0 vinay     (1000) vinay     (1000)   168448 2022-08-06 08:15:40.000000 distlib-0.3.7/distlib/w64-arm.exe
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    23777 2023-06-06 18:35:34.000000 distlib-0.3.7/distlib/version.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    20834 2021-12-18 14:21:28.000000 distlib-0.3.7/distlib/index.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    14813 2022-09-01 10:11:56.000000 distlib-0.3.7/distlib/manifest.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    51991 2021-12-14 20:05:07.000000 distlib-0.3.7/distlib/locators.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    25766 2023-07-17 09:59:32.000000 distlib-0.3.7/CHANGES.rst
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      265 2021-12-08 07:46:10.000000 distlib-0.3.7/MANIFEST.in
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      117 2022-05-09 07:58:27.000000 distlib-0.3.7/pyproject.toml
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3897 2022-07-14 07:51:11.000000 distlib-0.3.7/README.rst
```

### Comparing `distlib-0.3.6/PC/CLISimpleLauncher.vcxproj` & `distlib-0.3.7/PC/CLISimpleLauncher.vcxproj`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/PC/launcher.c` & `distlib-0.3.7/PC/launcher.c`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/PC/ReadMe.txt` & `distlib-0.3.7/PC/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/PC/GUISimpleLauncher.vcxproj` & `distlib-0.3.7/PC/GUISimpleLauncher.vcxproj`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/PC/launcher.ico` & `distlib-0.3.7/PC/launcher.ico`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/PC/SimpleLauncher.sln` & `distlib-0.3.7/PC/SimpleLauncher.sln`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/CONTRIBUTORS.txt` & `distlib-0.3.7/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib.egg-info/SOURCES.txt` & `distlib-0.3.7/distlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 tests/bad.tar.bz2
 tests/bad.tar.gz
 tests/bad.zip
 tests/bar.zip
 tests/compat.py
 tests/distlib_tests.py
 tests/dummy-0.1-py27-none-any.whl
+tests/evil.tar.gz
 tests/foo.zip
 tests/good.bin
 tests/good.bin.asc
 tests/good.tar
 tests/good.tar.bz2
 tests/good.tar.gz
 tests/good.zip
```

### Comparing `distlib-0.3.6/distlib.egg-info/PKG-INFO` & `distlib-0.3.7/distlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: distlib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Distribution utilities
 Home-page: https://github.com/pypa/distlib
 Author: Vinay Sajip
 Author-email: vinay_sajip@red-dove.com
-License: Python license
+License: PSF-2.0
 Project-URL: Documentation, https://distlib.readthedocs.io/
 Project-URL: Source, https://github.com/pypa/distlib
 Project-URL: Tracker, https://github.com/pypa/distlib/issues
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `distlib-0.3.6/tests/scripts/uwsgi_part` & `distlib-0.3.7/tests/scripts/uwsgi_part`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/testdist-0.1/package.json` & `distlib-0.3.7/tests/testdist-0.1/package.json`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/testdist-0.1/LICENSE` & `distlib-0.3.7/tests/testdist-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/compat.py` & `distlib-0.3.7/tests/compat.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/minimext-0.1-cp33-cp33m-linux_x86_64.whl` & `distlib-0.3.7/tests/minimext-0.1-cp33-cp33m-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_locators.py` & `distlib-0.3.7/tests/test_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,15 @@
         # to get all the dist names by scraping :-(
         n1 = loc1.get_distribution_names()
         n2 = loc2.get_distribution_names()
         self.assertEqual(locator.get_distribution_names(), n1 | n2)
 
     @unittest.skipIf('SKIP_ONLINE' in os.environ, 'Skipping online test')
     @unittest.skipUnless(ssl, 'SSL required for this test.')
+    @unittest.skipIf(True, 'Optimised metadata is not up-to-date')
     def test_dependency_finder(self):
         locator = AggregatingLocator(
             JSONLocator(),
             SimpleScrapingLocator('https://pypi.org/simple/', timeout=3.0),
             scheme='legacy')
         finder = DependencyFinder(locator)
         dists, problems = finder.find('irc (== 5.0.1)')
```

### Comparing `distlib-0.3.6/tests/dummy-0.1-py27-none-any.whl` & `distlib-0.3.7/tests/dummy-0.1-py27-none-any.whl`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keys/random_seed` & `distlib-0.3.7/tests/keys/random_seed`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keys/private-keys-v1.d/8BE462CC6083085304DBEA3FC423A1276DAF0B2C.key` & `distlib-0.3.7/tests/keys/private-keys-v1.d/8BE462CC6083085304DBEA3FC423A1276DAF0B2C.key`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keys/private-keys-v1.d/89643D011E83504EFB6A88F328153504C3E2C97B.key` & `distlib-0.3.7/tests/keys/private-keys-v1.d/89643D011E83504EFB6A88F328153504C3E2C97B.key`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keys/trustdb.gpg` & `distlib-0.3.7/tests/keys/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keys/pubring.gpg` & `distlib-0.3.7/tests/keys/pubring.gpg`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keys/secring.gpg` & `distlib-0.3.7/tests/keys/secring.gpg`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_testdist-0.1.zip` & `distlib-0.3.7/tests/test_testdist-0.1.zip`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/minimext-0.1-cp32-cp32mu-linux_x86_64.whl` & `distlib-0.3.7/tests/minimext-0.1-cp32-cp32mu-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_testdist-0.1/package.json` & `distlib-0.3.7/tests/test_testdist-0.1/package.json`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_testdist-0.1/LICENSE` & `distlib-0.3.7/tests/test_testdist-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_scripts.py` & `distlib-0.3.7/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_resources.py` & `distlib-0.3.7/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/SETUPTOOLS-PKG-INFO` & `distlib-0.3.7/tests/SETUPTOOLS-PKG-INFO`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/pydist.json` & `distlib-0.3.7/tests/pydist.json`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/distlib_tests.py` & `distlib-0.3.7/tests/distlib_tests.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_wheel.py` & `distlib-0.3.7/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_manifest.py` & `distlib-0.3.7/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_markers.py` & `distlib-0.3.7/tests/test_markers.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,20 @@
             self.assertTrue(interpret('python_version >= "3.10"'))
         self.assertTrue(interpret("'%s' in os_name" % os_name))
         self.assertTrue(interpret("'buuuu' not in os_name"))
         self.assertTrue(interpret("'buu' in os_name", {'os_name': 'buuu'}))
         self.assertTrue(interpret(
             "'buuuu' not in os_name and '%s' in os_name" % os_name))
 
+        # normalized version comparison correctness
+        self.assertTrue(interpret('python_version > "5.0"', {'python_version': '10.0'}))
+        self.assertTrue(interpret('python_version == "5.0"', {'python_version': '5.0'}))
+        self.assertTrue(interpret('python_version < "5.0"', {'python_version': '5.0b0'}))
+        self.assertTrue(interpret('python_full_version > "5.0"', {'python_full_version': '10.0'}))
+
         # execution context
         self.assertTrue(interpret('python_version == "0.1"',
                                   {'python_version': '0.1'}))
 
         # parentheses and extra
         if sys.platform != 'win32':
             relop = '!='
```

### Comparing `distlib-0.3.6/tests/bad.tar` & `distlib-0.3.7/tests/bad.tar`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_util.py` & `distlib-0.3.7/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,20 @@
         self.check_entry(get_export_entry('foo=foo.bar:main [a=9, 9=8,e, f9=g8]'),
                          'foo', 'foo.bar', 'main', ['a=9', '9=8', 'e', 'f9=g8'])
         self.check_entry(get_export_entry('foo=foo.bar:main[x]'),
                          'foo', 'foo.bar', 'main', ['x'])
         self.check_entry(get_export_entry('foo=abc'), 'foo', 'abc', None, [])
         self.check_entry(get_export_entry('smc++ = smcpp.frontend:console'), 'smc++',
                                           'smcpp.frontend', 'console', [])
+        # See issue #203 - correct name parsing to allow non-name-like names like ","
+        self.check_entry(get_export_entry(', = comma:main'), ',',
+                                          'comma', 'main', [])
+        self.check_entry(get_export_entry(',comma = comma:main'), ',comma',
+                                          'comma', 'main', [])
+
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x:y')
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x [')
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x ]')
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x []')
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x [\\]')
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x [a=]')
         self.assertRaises(DistlibException, get_export_entry, 'foo=foo.bar:x [a,]')
@@ -467,14 +473,18 @@
             ('good.zip', zipfile.ZipFile, 'r', 'namelist'),
             ('good.tar', tarfile.open, 'r', 'getnames'),
             ('good.tar.gz', tarfile.open, 'r:gz', 'getnames'),
             ('good.tar.bz2', tarfile.open, 'r:bz2', 'getnames'),
         )
         bad_archives = ('bad.zip', 'bad.tar', 'bad.tar.gz', 'bad.tar.bz2')
 
+        # Test "evil" tarball on 3.12 *or* on Python with PEP-706 backported
+        if sys.version_info > (3, 12) or hasattr(tarfile, 'data_filter'):
+            bad_archives += ('evil.tar.gz',)
+
         for name, cls, mode, lister in good_archives:
             td = tempfile.mkdtemp()
             archive = None
             try:
                 name = os.path.join(HERE, name)
                 unarchive(name, td)
                 archive = cls(name, mode)
```

### Comparing `distlib-0.3.6/tests/bad.zip` & `distlib-0.3.7/tests/bad.zip`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/good.zip` & `distlib-0.3.7/tests/good.zip`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_database.py` & `distlib-0.3.7/tests/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,16 +574,17 @@
         self.assertIn('bar.baz', r)
         d = r['bar.baz']
         self.assertIn('foofoo', d)
         self.check_entry(d['foofoo'], 'foofoo', 'baz.foo', 'bazbar', [])
         self.assertIn('real', d)
         e = d['real']
         self.check_entry(e, 'real', 'cgi', 'print_directory', [])
-        import cgi
-        self.assertIs(e.value, cgi.print_directory)
+        if sys.version_info[:2] < (3, 12):
+            import cgi
+            self.assertIs(e.value, cgi.print_directory)
 
         # See issue #78. Test reading an entry_points.txt with leading spaces
 
         TEST_EXPORTS = b"""
         [paste.server_runner]
         main = waitress:serve_paste
         [console_scripts]
```

### Comparing `distlib-0.3.6/tests/bar.zip` & `distlib-0.3.7/tests/bar.zip`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/fake_dists/strawberry-0.6.egg` & `distlib-0.3.7/tests/fake_dists/strawberry-0.6.egg`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/fake_dists/banana-0.4.egg/EGG-INFO/PKG-INFO` & `distlib-0.3.7/tests/fake_dists/banana-0.4.egg/EGG-INFO/PKG-INFO`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/good.tar` & `distlib-0.3.7/tests/good.tar`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_index.py` & `distlib-0.3.7/tests/test_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,24 +305,26 @@
             flag.wait()
             def cleanup():
                 server.stop()
                 server.join()
             self.addCleanup(cleanup)
             return server
 
+        @unittest.skipIf(sys.version_info[:2] > (3, 11), 'Temporary skip')
         def test_ssl_verification(self):
             certfile = os.path.join(HERE, 'keycert.pem')
             server = self.make_https_server(certfile)
             url = 'https://localhost:%d/' % server.port
             req = Request(url)
             self.index.ssl_verifier = HTTPSHandler(certfile)
             response = self.index.send_request(req)
             self.assertEqual(response.code, 200)
 
         @unittest.skipIf(IN_GITHUB_WORKFLOW, 'This test is end-of-line dependent')
+        @unittest.skipIf(sys.version_info[:2] > (3, 11), 'Temporary skip')
         def test_download(self):  # pragma: no cover
             digest = '913093474942c5a564c011f232868517' # for testsrc/README.txt
             certfile = os.path.join(HERE, 'keycert.pem')
             server = self.make_https_server(certfile)
             url = 'https://localhost:%d/README.txt' % server.port
             fd, fn = tempfile.mkstemp()
             os.close(fd)
```

### Comparing `distlib-0.3.6/tests/minimext-0.1-cp27-none-linux_x86_64.whl` & `distlib-0.3.7/tests/minimext-0.1-cp27-none-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/keycert.pem` & `distlib-0.3.7/tests/keycert.pem`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/PKG-INFO` & `distlib-0.3.7/tests/PKG-INFO`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/LONG_DESC.txt` & `distlib-0.3.7/tests/LONG_DESC.txt`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_metadata.py` & `distlib-0.3.7/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/test_version.py` & `distlib-0.3.7/tests/test_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,22 +50,27 @@
         versions = set([v for v, s in self.versions])
         for v, s in self.versions:
             self.assertIn(v, versions)
 
         self.assertEqual(set([NV('1.0')]), set([NV('1.0'), NV('1.0')]))
 
     def test_unsupported_versions(self):
-        unsupported = ('1.2a', '1.2.3b',
+        unsupported = (
+                       # '1.2a', '1.2.3b',  # see issue 200 - not unsupported
                       #'1.02', '1.2a03', '1.2a3.04',
-                      '1.2.dev.2', '1.2dev', '1.2.dev',
+                      '1.2.dev.2',
+                      # '1.2dev', '1.2.dev',  # see issue 200 - these are not unsupported
                       '1.2-', '1.2-a',
                       '1.2.dev2.post2', '1.2.post2.dev3.post4')
 
         for s in unsupported:
-            self.assertRaises(UnsupportedVersionError, NV, s)
+            with self.assertRaises(UnsupportedVersionError) as cm:
+                NV(s)
+                # print(s)
+                # import pdb; pdb.set_trace()
 
     def test_huge_version(self):
         self.assertEqual(str(NV('1980.0')), '1980.0')
 
     def test_comparison(self):
         comparison_doctest_string = r"""
         >>> NV('1.2.0') == '1.2'
@@ -172,31 +177,31 @@
         self.assertEqual(suggest('1.0-alpha1'), '1.0a1')
         self.assertEqual(suggest('1.0c2'), '1.0c2')
         self.assertEqual(suggest('walla walla washington'), None)
         self.assertEqual(suggest('2.4c1'), '2.4c1')
         self.assertEqual(suggest('v1.0'), 'v1.0')
 
         # from setuptools
-        self.assertEqual(suggest('0.4a1.r10'), '0.4a1.post10')
+        # self.assertEqual(suggest('0.4a1.r10'), '0.4a1.post10')  # see issue #200
         self.assertEqual(suggest('0.7a1dev-r66608'), '0.7a1.dev66608')
         self.assertEqual(suggest('0.6a9.dev-r41475'), '0.6a9.dev41475')
-        self.assertEqual(suggest('2.4preview1'), '2.4c1')
-        self.assertEqual(suggest('2.4pre1'), '2.4c1')
+        # self.assertEqual(suggest('2.4preview1'), '2.4c1')  # see issue #200
+        # self.assertEqual(suggest('2.4pre1'), '2.4c1')  # see issue #200
         self.assertEqual(suggest('2.1-rc2'), '2.1c2')
 
         # from pypi
-        self.assertEqual(suggest('0.1dev'), '0.1.dev0')
-        self.assertEqual(suggest('0.1.dev'), '0.1.dev0')
+        # self.assertEqual(suggest('0.1dev'), '0.1.dev0')   # see issue 200 - 0.1dev is now rational
+        # self.assertEqual(suggest('0.1.dev'), '0.1.dev0')  # see issue 200 - 0.1.dev is now rational
 
         # we want to be able to parse Twisted
         # development versions are like post releases in Twisted
         #self.assertEqual(suggest('9.0.0+r2363'), '9.0.0.post2363')
 
         # pre-releases are using markers like "pre1"
-        self.assertEqual(suggest('9.0.0pre1'), '9.0.0c1')
+        # self.assertEqual(suggest('9.0.0pre1'), '9.0.0c1')  # see issue #200
 
         # we want to be able to parse Tcl-TK
         # they us "p1" "p2" for post releases
         self.assertEqual(suggest('1.4p1'), '1.4.post1')
 
     def test_suggestions_other(self):
         suggest = _suggest_semantic_version
@@ -444,14 +449,22 @@
         for op in ('<', '<=', '>', '>=', '~='):
             s = 'foo (%s 1.*)' % op
             self.assertRaises(ValueError, NM, s)
         for v in ('', '1.*.*'):
             s = 'foo (== %s)' % v
             self.assertRaises((SyntaxError, ValueError), NM, s)
 
+    def test_fix_200(self):
+        versions = (
+            ('foo<=0.8.1dev', '0.8.1.dev0'),
+        )
+
+        for v1, v2 in versions:
+            # import pdb; pdb.set_trace()
+            NM(v1).match(v2)
 
 class LegacyVersionTestCase(DistlibTestCase):
     # These tests are the same as distribute's
     def test_equality(self):
         def compare(a, b):
             ka, kb = _legacy_key(a), _legacy_key(b)
             self.assertEqual(ka, kb)
```

### Comparing `distlib-0.3.6/tests/test_all.py` & `distlib-0.3.7/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/foo.zip` & `distlib-0.3.7/tests/foo.zip`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/support.py` & `distlib-0.3.7/tests/support.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/valid_wheel-0.0.1-py3-none-any.whl` & `distlib-0.3.7/tests/valid_wheel-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/bad_wheels/dummy-0.1-py27-none-any.whl` & `distlib-0.3.7/tests/bad_wheels/dummy-0.1-py27-none-any.whl`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/tests/SETUPTOOLS-PKG-INFO2` & `distlib-0.3.7/tests/SETUPTOOLS-PKG-INFO2`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/setup.cfg` & `distlib-0.3.7/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 name = distlib
 version = attr: distlib.__version__
 description = Distribution utilities
 long_description = file: README.rst
 url = https://github.com/pypa/distlib
 author = Vinay Sajip
 author_email = vinay_sajip@red-dove.com
-license = Python license
-license_file = LICENSE.txt
+license = PSF-2.0
+license_files = LICENSE.txt
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Python Software Foundation License
 	Operating System :: OS Independent
 	Programming Language :: Python
```

### Comparing `distlib-0.3.6/LICENSE.txt` & `distlib-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/PKG-INFO` & `distlib-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: distlib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Distribution utilities
 Home-page: https://github.com/pypa/distlib
 Author: Vinay Sajip
 Author-email: vinay_sajip@red-dove.com
-License: Python license
+License: PSF-2.0
 Project-URL: Documentation, https://distlib.readthedocs.io/
 Project-URL: Source, https://github.com/pypa/distlib
 Project-URL: Tracker, https://github.com/pypa/distlib/issues
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `distlib-0.3.6/distlib/metadata.py` & `distlib-0.3.7/distlib/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,25 +132,17 @@
         return _643_FIELDS
     raise MetadataUnrecognizedVersionError(version)
 
 
 def _best_version(fields):
     """Detect the best version depending on the fields used."""
     def _has_marker(keys, markers):
-        for marker in markers:
-            if marker in keys:
-                return True
-        return False
-
-    keys = []
-    for key, value in fields.items():
-        if value in ([], 'UNKNOWN', None):
-            continue
-        keys.append(key)
+        return any(marker in keys for marker in markers)
 
+    keys = [key for key, value in fields.items() if value not in ([], 'UNKNOWN', None)]
     possible_versions = ['1.0', '1.1', '1.2', '1.3', '2.1', '2.2']  # 2.0 removed
 
     # first let's try to see if a field is not part of one of the version
     for key in keys:
         if key not in _241_FIELDS and '1.0' in possible_versions:
             possible_versions.remove('1.0')
             logger.debug('Removed 1.0 due to %s', key)
```

### Comparing `distlib-0.3.6/distlib/compat.py` & `distlib-0.3.7/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/t32.exe` & `distlib-0.3.7/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/t64.exe` & `distlib-0.3.7/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/database.py` & `distlib-0.3.7/distlib/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -899,23 +899,26 @@
 
             *data*: the contents of a setuptools-produced requires.txt file.
             """
             reqs = []
             lines = data.splitlines()
             for line in lines:
                 line = line.strip()
-                if line.startswith('['):
+                # sectioned files have bare newlines (separating sections)
+                if not line:  # pragma: no cover
+                    continue
+                if line.startswith('['):  # pragma: no cover
                     logger.warning('Unexpected line: quitting requirement scan: %r',
                                    line)
                     break
                 r = parse_requirement(line)
-                if not r:
+                if not r:  # pragma: no cover
                     logger.warning('Not recognised as a requirement: %r', line)
                     continue
-                if r.extras:
+                if r.extras:  # pragma: no cover
                     logger.warning('extra requirements in requires.txt are '
                                    'not supported')
                 if not r.constraints:
                     reqs.append(r.name)
                 else:
                     cons = ', '.join('%s%s' % c for c in r.constraints)
                     reqs.append('%s (%s)' % (r.name, cons))
```

### Comparing `distlib-0.3.6/distlib/w64.exe` & `distlib-0.3.7/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/w32.exe` & `distlib-0.3.7/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/scripts.py` & `distlib-0.3.7/distlib/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,23 +164,24 @@
             enquote = False     # assume this will be taken care of
         elif not sysconfig.is_python_build():
             executable = get_executable()
         elif in_venv():  # pragma: no cover
             executable = os.path.join(sysconfig.get_path('scripts'),
                             'python%s' % sysconfig.get_config_var('EXE'))
         else:  # pragma: no cover
-            executable = os.path.join(
-                sysconfig.get_config_var('BINDIR'),
-               'python%s%s' % (sysconfig.get_config_var('VERSION'),
-                               sysconfig.get_config_var('EXE')))
-            if not os.path.isfile(executable):
+            if os.name == 'nt':
                 # for Python builds from source on Windows, no Python executables with
                 # a version suffix are created, so we use python.exe
                 executable = os.path.join(sysconfig.get_config_var('BINDIR'),
                                 'python%s' % (sysconfig.get_config_var('EXE')))
+            else:
+                executable = os.path.join(
+                    sysconfig.get_config_var('BINDIR'),
+                   'python%s%s' % (sysconfig.get_config_var('VERSION'),
+                                   sysconfig.get_config_var('EXE')))
         if options:
             executable = self._get_alternate_executable(executable, options)
 
         if sys.platform.startswith('java'):  # pragma: no cover
             executable = self._fix_jython_executable(executable)
 
         # Normalise case for Windows - COMMENTED OUT
```

### Comparing `distlib-0.3.6/distlib/markers.py` & `distlib-0.3.7/distlib/markers.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 from .compat import string_types
 from .util import in_venv, parse_marker
 from .version import NormalizedVersion as NV
 
 __all__ = ['interpret']
 
 _VERSION_PATTERN = re.compile(r'((\d+(\.\d+)*\w*)|\'(\d+(\.\d+)*\w*)\'|\"(\d+(\.\d+)*\w*)\")')
+_VERSION_MARKERS = {'python_version', 'python_full_version'}
+
+def _is_version_marker(s):
+    return isinstance(s, string_types) and s in _VERSION_MARKERS
 
 def _is_literal(o):
     if not isinstance(o, string_types) or not o:
         return False
     return o[0] in '\'"'
 
 def _get_versions(s):
-    result = []
-    for m in _VERSION_PATTERN.finditer(s):
-        result.append(NV(m.groups()[0]))
-    return set(result)
+    return {NV(m.groups()[0]) for m in _VERSION_PATTERN.finditer(s)}
 
 class Evaluator(object):
     """
-    This class is used to evaluate marker expessions.
+    This class is used to evaluate marker expressions.
     """
 
     operations = {
         '==': lambda x, y: x == y,
         '===': lambda x, y: x == y,
         '~=': lambda x, y: x == y or x > y,
         '!=': lambda x, y: x != y,
@@ -76,19 +77,19 @@
             elhs = expr['lhs']
             erhs = expr['rhs']
             if _is_literal(expr['lhs']) and _is_literal(expr['rhs']):
                 raise SyntaxError('invalid comparison: %s %s %s' % (elhs, op, erhs))
 
             lhs = self.evaluate(elhs, context)
             rhs = self.evaluate(erhs, context)
-            if ((elhs == 'python_version' or erhs == 'python_version') and
+            if ((_is_version_marker(elhs) or _is_version_marker(erhs)) and
                 op in ('<', '<=', '>', '>=', '===', '==', '!=', '~=')):
                 lhs = NV(lhs)
                 rhs = NV(rhs)
-            elif elhs == 'python_version' and op in ('in', 'not in'):
+            elif _is_version_marker(elhs) and op in ('in', 'not in'):
                 lhs = NV(lhs)
                 rhs = _get_versions(rhs)
             result = self.operations[op](lhs, rhs)
         return result
 
 _DIGITS = re.compile(r'\d+\.\d+')
```

### Comparing `distlib-0.3.6/distlib/__init__.py` & `distlib-0.3.7/distlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright (C) 2012-2022 Vinay Sajip.
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 import logging
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 class DistlibException(Exception):
     pass
 
 try:
     from logging import NullHandler
 except ImportError: # pragma: no cover
```

### Comparing `distlib-0.3.6/distlib/wheel.py` & `distlib-0.3.7/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/resources.py` & `distlib-0.3.7/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/util.py` & `distlib-0.3.7/distlib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -703,15 +703,15 @@
                       self.suffix == other.suffix and
                       self.flags == other.flags)
         return result
 
     __hash__ = object.__hash__
 
 
-ENTRY_RE = re.compile(r'''(?P<name>(\w|[-.+])+)
+ENTRY_RE = re.compile(r'''(?P<name>([^\[]\S*))
                       \s*=\s*(?P<callable>(\w+)([:\.]\w+)*)
                       \s*(\[\s*(?P<flags>[\w-]+(=\w+)?(,\s*\w+(=\w+)?)*)\s*\])?
                       ''', re.VERBOSE)
 
 def get_export_entry(specification):
     m = ENTRY_RE.search(specification)
     if not m:
@@ -1245,14 +1245,27 @@
             # See Python issue 17153. If the dest path contains Unicode,
             # tarfile extraction fails on Python 2.x if a member path name
             # contains non-ASCII characters - it leads to an implicit
             # bytes -> unicode conversion using ASCII to decode.
             for tarinfo in archive.getmembers():
                 if not isinstance(tarinfo.name, text_type):
                     tarinfo.name = tarinfo.name.decode('utf-8')
+
+        # Limit extraction of dangerous items, if this Python
+        # allows it easily. If not, just trust the input.
+        # See: https://docs.python.org/3/library/tarfile.html#extraction-filters
+        def extraction_filter(member, path):
+            """Run tarfile.tar_filter, but raise the expected ValueError"""
+            # This is only called if the current Python has tarfile filters
+            try:
+                return tarfile.tar_filter(member, path)
+            except tarfile.FilterError as exc:
+                raise ValueError(str(exc))
+        archive.extraction_filter = extraction_filter
+
         archive.extractall(dest_dir)
 
     finally:
         if archive:
             archive.close()
 
 
@@ -1431,15 +1444,15 @@
             if getattr(self, '_tunnel_host', False):
                 self.sock = sock
                 self._tunnel()
 
             context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
             if hasattr(ssl, 'OP_NO_SSLv2'):
                 context.options |= ssl.OP_NO_SSLv2
-            if self.cert_file:
+            if getattr(self, 'cert_file', None):
                 context.load_cert_chain(self.cert_file, self.key_file)
             kwargs = {}
             if self.ca_certs:
                 context.verify_mode = ssl.CERT_REQUIRED
                 context.load_verify_locations(cafile=self.ca_certs)
                 if getattr(ssl, 'HAS_SNI', False):
                     kwargs['server_hostname'] = self.host
@@ -1904,17 +1917,21 @@
     elif osname[:6] == 'cygwin':
         osname = 'cygwin'
         rel_re = re.compile (r'[\d.]+', re.ASCII)
         m = rel_re.match(release)
         if m:
             release = m.group()
     elif osname[:6] == 'darwin':
-        import _osx_support, distutils.sysconfig
+        import _osx_support
+        try:
+            from distutils import sysconfig
+        except ImportError:
+            import sysconfig
         osname, release, machine = _osx_support.get_platform_osx(
-                                        distutils.sysconfig.get_config_vars(),
+                                        sysconfig.get_config_vars(),
                                         osname, release, machine)
 
     return '%s-%s-%s' % (osname, release, machine)
 
 
 _TARGET_TO_PLAT = {
     'x86' : 'win32',
```

### Comparing `distlib-0.3.6/distlib/t64-arm.exe` & `distlib-0.3.7/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/w64-arm.exe` & `distlib-0.3.7/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/version.py` & `distlib-0.3.7/distlib/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,17 +172,17 @@
     def __repr__(self):
         return "%s(%r)" % (self.__class__.__name__, self._string)
 
     def __str__(self):
         return self._string
 
 
-PEP440_VERSION_RE = re.compile(r'^v?(\d+!)?(\d+(\.\d+)*)((a|b|c|rc)(\d+))?'
-                               r'(\.(post)(\d+))?(\.(dev)(\d+))?'
-                               r'(\+([a-zA-Z\d]+(\.[a-zA-Z\d]+)?))?$')
+PEP440_VERSION_RE = re.compile(r'^v?(\d+!)?(\d+(\.\d+)*)((a|alpha|b|beta|c|rc|pre|preview)(\d+)?)?'
+                               r'(\.(post|r|rev)(\d+)?)?([._-]?(dev)(\d+)?)?'
+                               r'(\+([a-zA-Z\d]+(\.[a-zA-Z\d]+)?))?$', re.I)
 
 
 def _pep_440_key(s):
     s = s.strip()
     m = PEP440_VERSION_RE.match(s)
     if not m:
         raise UnsupportedVersionError('Not a valid version: %s' % s)
@@ -198,23 +198,32 @@
     pre = groups[4:6]
     post = groups[7:9]
     dev = groups[10:12]
     local = groups[13]
     if pre == (None, None):
         pre = ()
     else:
-        pre = pre[0], int(pre[1])
+        if pre[1] is None:
+            pre = pre[0], 0
+        else:
+            pre = pre[0], int(pre[1])
     if post == (None, None):
         post = ()
     else:
-        post = post[0], int(post[1])
+        if post[1] is None:
+            post = post[0], 0
+        else:
+            post = post[0], int(post[1])
     if dev == (None, None):
         dev = ()
     else:
-        dev = dev[0], int(dev[1])
+        if dev[1] is None:
+            dev = dev[0], 0
+        else:
+            dev = dev[0], int(dev[1])
     if local is None:
         local = ()
     else:
         parts = []
         for part in local.split('.'):
             # to ensure that numeric compares as > lexicographic, avoid
             # comparing them directly, but encode a tuple which ensures
```

### Comparing `distlib-0.3.6/distlib/index.py` & `distlib-0.3.7/distlib/index.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/distlib/manifest.py` & `distlib-0.3.7/distlib/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 # Due to the different results returned by fnmatch.translate, we need
 # to do slightly different processing for Python 2.7 and 3.2 ... this needed
 # to be brought in for Python 3.6 onwards.
 #
 _PYTHON_VERSION = sys.version_info[:2]
 
 class Manifest(object):
-    """A list of files built by on exploring the filesystem and filtered by
-    applying various patterns to what we find there.
+    """
+    A list of files built by exploring the filesystem and filtered by applying various
+    patterns to what we find there.
     """
 
     def __init__(self, base=None):
         """
         Initialise an instance.
 
         :param base: The base directory to explore under.
```

### Comparing `distlib-0.3.6/distlib/locators.py` & `distlib-0.3.7/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `distlib-0.3.6/CHANGES.rst` & `distlib-0.3.7/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,60 @@
 Change log for ``distlib``
 --------------------------
 
-0.3.6 (future)
+0.3.8 (future)
 ~~~~~~~~~~~~~~
 
 Released: Not yet.
 
+0.3.7
+~~~~~
+
+Released: 2023-07-17
+
+- database
+
+    - Handle newlines when parsing metadata.
+
+- markers
+
+    - Use version comparison logic for python_full_version. Thanks to Albert
+      Peschar for the patch.
+
+    - Simplify code with a set comprehension. Thanks to Christian Clauss for
+      the patch.
+
+- scripts
+
+    - Fix shebang computation for source builds of Python. Thanks to Eli
+      Schwartz for the patch.
+
+- util
+
+    - Extract tarfiles more safely by incorporating tarfile filters. Thanks to
+      Petr Viktorin for the patch.
+
+    - Check for 'has_cert' attribute before using it. Thanks to Lumir Balhar for
+      the patch.
+
+    - Fix #203: Handle parsing of export entries to allow script names such as
+      "," or ",foo". Thanks to Flavio Amurrio for the report.
+
+- versions
+
+    - Fix #200: Improve conformance to PEP440. Thanks to GitHub user con-f-use
+      for the report.
+
+In addition to the above, an SPDX license identifier is now used.
+
+0.3.6
+~~~~~
+
+Released: 2022-08-26
+
 - scripts
 
     - Fixed #175: Updated launcher executables to better handle the relationship
       between launcher and child process in the Job API.
 
 0.3.5
 ~~~~~
@@ -983,15 +1028,15 @@
 
     - Return RECORD path from write_installed_files (or None if dry_run).
 
     - Explicitly return None from write_shared_locations if dry run.
 
 - metadata
 
-    - Added missing condition in :meth:`todict`.
+    - Added missing condition in :meth:`~distlib.metadata.Metadata.todict`.
 
 - scripts
 
     - Add variants and clobber flag for generation of foo/fooX/foo-X.Y.
 
     - Added .exe manifests for Windows.
```

### Comparing `distlib-0.3.6/README.rst` & `distlib-0.3.7/README.rst`

 * *Files identical despite different names*

